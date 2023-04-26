# Comparing `tmp/kaskada-0.1.5.tar.gz` & `tmp/kaskada-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.1.5.tar", max compression
+gzip compressed data, was "kaskada-0.1.6.tar", max compression
```

## Comparing `kaskada-0.1.5.tar` & `kaskada-0.1.6.tar`

### file list

```diff
@@ -1,88 +1,65 @@
--rw-r--r--   0        0        0     1646 2023-04-19 20:57:42.994947 kaskada-0.1.5/README.md
--rw-r--r--   0        0        0     3874 2023-04-20 13:03:18.953835 kaskada-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7209 2023-04-19 20:57:42.996697 kaskada-0.1.5/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-03-16 21:27:38.249764 kaskada-0.1.5/src/fenlmagic/utils.py
--rw-r--r--   0        0        0       33 2023-04-19 20:57:42.996774 kaskada-0.1.5/src/kaskada/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 20:57:42.996810 kaskada-0.1.5/src/kaskada/api/__init__.py
--rw-r--r--   0        0        0      123 2023-04-20 13:06:11.384170 kaskada-0.1.5/src/kaskada/api/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1476 2023-03-20 16:22:12.166889 kaskada-0.1.5/src/kaskada/api/__pycache__/api_utils.cpython-39.pyc
--rw-r--r--   0        0        0     5241 2023-03-20 16:22:12.171063 kaskada-0.1.5/src/kaskada/api/__pycache__/release.cpython-39.pyc
--rw-r--r--   0        0        0     9143 2023-04-20 13:06:11.389501 kaskada-0.1.5/src/kaskada/api/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     1179 2023-03-16 21:27:38.250104 kaskada-0.1.5/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0     6381 2023-03-16 21:27:38.250435 kaskada-0.1.5/src/kaskada/api/release.py
--rw-r--r--   0        0        0     9503 2023-04-19 22:53:22.424816 kaskada-0.1.5/src/kaskada/api/session.py
--rw-r--r--   0        0        0     5838 2023-04-19 21:28:57.311096 kaskada-0.1.5/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-03-16 21:27:38.251034 kaskada-0.1.5/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-03-16 21:27:38.251117 kaskada-0.1.5/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-03-16 21:27:38.251456 kaskada-0.1.5/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7318 2023-03-16 21:27:38.251739 kaskada-0.1.5/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0     9805 2023-04-05 15:54:29.951572 kaskada-0.1.5/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0     6383 2023-04-20 13:06:11.210937 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/common_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     3427 2023-04-20 13:06:11.247588 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/destinations_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     2419 2023-04-20 13:06:11.215018 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/fenl_diagnostics_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     7611 2023-04-20 13:06:11.243268 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5132 2023-04-20 13:06:11.238064 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2_grpc.cpython-39.pyc
--rw-r--r--   0        0        0     1496 2023-04-20 13:06:10.479718 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/options_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     2389 2023-04-20 13:06:11.198536 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/pulsar_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     8698 2023-04-20 13:06:11.257260 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     4020 2023-04-20 13:06:11.252307 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2_grpc.cpython-39.pyc
--rw-r--r--   0        0        0     3183 2023-04-20 13:06:11.219039 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/schema_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     2097 2023-04-20 13:06:11.223654 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/sources_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     7518 2023-04-20 13:06:11.204897 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5249 2023-04-20 13:06:11.262515 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2_grpc.cpython-39.pyc
--rw-r--r--   0        0        0     3732 2023-03-28 20:07:39.942540 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-39-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3732 2023-04-20 13:06:10.460690 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      357 2023-03-28 20:07:39.964989 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2_grpc.cpython-39-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      357 2023-04-20 13:06:10.485843 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2_grpc.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     5709 2023-04-20 13:06:11.232312 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     4530 2023-04-20 13:06:11.267104 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2_grpc.cpython-39.pyc
--rw-r--r--   0        0        0    13053 2023-04-20 13:03:28.003641 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.002913 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    16901 2023-04-20 13:03:28.002955 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0     6628 2023-04-20 13:03:28.004505 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     5994 2023-04-20 13:03:28.004483 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-04-20 13:03:28.005059 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     6043 2023-04-20 13:03:28.005347 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.006106 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     3526 2023-04-20 13:03:28.006962 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.007312 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     6348 2023-04-20 13:03:28.007747 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-04-20 13:03:28.008449 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0    15562 2023-04-20 13:03:28.009017 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-04-20 13:03:28.009595 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1846 2023-04-20 13:03:28.009925 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.010338 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    21703 2023-04-20 13:03:28.010880 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.012058 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     4981 2023-04-20 13:03:28.012421 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-04-20 13:03:28.013248 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     3561 2023-04-20 13:03:28.014281 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.014445 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    16795 2023-04-20 13:03:28.014973 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-04-20 13:03:28.015692 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4886 2023-04-20 13:03:28.015994 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.016385 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     3258 2023-04-20 13:03:28.017021 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.017508 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2882 2023-04-20 13:03:28.017959 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.018476 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    15322 2023-04-20 13:03:28.019199 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-04-20 13:03:28.019981 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     6835 2023-04-20 13:03:28.020233 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-04-20 13:03:28.020617 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0    11387 2023-04-20 13:03:28.021258 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-04-20 13:03:28.021701 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    26185 2023-04-20 13:03:28.022708 kaskada-0.1.5/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-04-20 13:03:28.023223 kaskada-0.1.5/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8594 2023-04-05 15:54:29.951770 kaskada-0.1.5/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9232 2023-04-05 15:54:29.952092 kaskada-0.1.5/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-03-16 21:27:38.252438 kaskada-0.1.5/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10098 2023-04-05 15:54:29.952252 kaskada-0.1.5/src/kaskada/table.py
--rw-r--r--   0        0        0     6725 2023-04-19 20:57:42.997805 kaskada-0.1.5/src/kaskada/utils.py
--rw-r--r--   0        0        0     4515 2023-03-16 21:27:38.252722 kaskada-0.1.5/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-03-16 21:27:38.254737 kaskada-0.1.5/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-03-16 21:27:38.254889 kaskada-0.1.5/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-03-16 21:27:38.255015 kaskada-0.1.5/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-16 21:27:38.255097 kaskada-0.1.5/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.1.5/setup.py
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-04-26 19:24:50.174096 kaskada-0.1.6/README.md
+-rw-r--r--   0        0        0     3882 2023-04-26 19:24:50.174096 kaskada-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7208 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0     6381 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     9507 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/session.py
+-rw-r--r--   0        0        0     5838 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7337 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0     9833 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0     7394 2023-04-26 19:24:50.738094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:50.734094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    10615 2023-04-26 19:24:50.782094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0     6628 2023-04-26 19:24:50.782094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4489 2023-04-26 19:24:50.822094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-04-26 19:24:50.818094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4191 2023-04-26 19:24:50.862094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:50.886094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     2668 2023-04-26 19:24:50.894094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:50.946094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     3976 2023-04-26 19:24:50.926094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-04-26 19:24:50.970094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10837 2023-04-26 19:24:50.990094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-04-26 19:24:51.010094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-04-26 19:24:51.026094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:51.042094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    13180 2023-04-26 19:24:51.058094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:51.114093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     3398 2023-04-26 19:24:51.094093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-04-26 19:24:51.134093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2805 2023-04-26 19:24:51.146093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:51.198093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    11773 2023-04-26 19:24:51.178093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-04-26 19:24:51.218093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4018 2023-04-26 19:24:51.230093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:51.270093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-04-26 19:24:51.266093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:51.310093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2729 2023-04-26 19:24:51.306093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:51.346093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    11249 2023-04-26 19:24:51.354093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-04-26 19:24:51.382093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5157 2023-04-26 19:24:51.394093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:51.418093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0     8140 2023-04-26 19:24:51.422093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-04-26 19:24:51.458093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16491 2023-04-26 19:24:51.454093 kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-04-26 19:24:51.486092 kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8622 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9272 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10126 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/table.py
+-rw-r--r--   0        0        0     6753 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4543 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.1.6/setup.py
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.1.6/PKG-INFO
```

### Comparing `kaskada-0.1.5/README.md` & `kaskada-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/pyproject.toml` & `kaskada-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.1.5"
+version = "0.1.6"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
@@ -43,14 +43,15 @@
 types-typed-ast = "^1.5.8.3"
 autoflake = "^2.0.0"
 autopep8 = "^2.0.1"
 types-protobuf = "^4.21.0.5"
 Sphinx = "5.3.0"
 sphinx-rtd-theme = "1.2.0"
 sphinx-autodoc-typehints = "1.22"
+sphinx-autoapi = "2.1.0"
 tomli = "2.0.1"
 
 [tool.poe.tasks]
 [tool.poe.tasks.clean]
 help = "Remove generated files"
 cmd = """
         # multiline commands including comments work too!
@@ -120,15 +121,15 @@
 
 [tool.poe.tasks.docs-generate]
 help = "Generates documentation from docstrings"
 cmd = "sphinx-apidoc -f -E  -M -o docs/source src/ src/clients/python/kaskada/kaskada"
 
 [tool.poe.tasks.docs]
 help = "Generated and build HTML docs"
-sequence = ["docs-generate", "docs-build"]
+sequence = ["docs-build"]
 
 [tool.isort]
 profile = "black"
 skip = ["src/kaskada/kaskada"]
 
 [tool.mypy]
 exclude = ["src/kaskada/kaskada"]
```

### Comparing `kaskada-0.1.5/src/fenlmagic/__init__.py` & `kaskada-0.1.6/src/fenlmagic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Integration with IPython (Notebooks) for Fenl.
 
     Raises:
         UsageError: when improper arguments are provided
 """
-
+# pylint: disable=no-member
 from __future__ import print_function
 
 import os
 
 import IPython
 import pandas
 from google.protobuf import wrappers_pb2 as wrappers
 from IPython.core.error import UsageError
 from IPython.core.magic import Magics, cell_magic, line_cell_magic, magics_class
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 
-import kaskada.client as client
 import kaskada.kaskada.v1alpha.query_service_pb2 as query_pb
-import kaskada.query as query
 from fenlmagic.utils import arg_to_response_type
+from kaskada import client, query
 
 
 class QueryResult(object):
     dataframe: pandas.DataFrame = None
 
     def __init__(
         self, expression: str, query_response: query_pb.CreateQueryResponse  # type: ignore[valid-type]
```

### Comparing `kaskada-0.1.5/src/kaskada/api/api_utils.py` & `kaskada-0.1.6/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/api/release.py` & `kaskada-0.1.6/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/api/session.py` & `kaskada-0.1.6/src/kaskada/api/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,22 +199,22 @@
         engine_command = "serve"
 
         manager_cmd = [str(manager_binary_path)] + self.__get_manager_configs_as_args()
         logger.debug(f"Manager start command: {manager_cmd}")
         engine_cmd = [engine_binary_path, engine_command]
         logger.debug(f"Engine start command: {engine_cmd}")
         logger.info("Initializing manager process")
-        logger.info("Logging manager STDOUT to {manager_std_out}")
-        logger.info("Logging manager STDERR to {manager_std_err}")
+        logger.info(f"Logging manager STDOUT to {manager_std_out}")
+        logger.info(f"Logging manager STDERR to {manager_std_err}")
         manager_process = api_utils.run_subprocess(
             manager_cmd, manager_std_err, manager_std_out
         )
         logger.info("Initializing engine process")
-        logger.info("Logging engine STDOUT to {engine_std_out}")
-        logger.info("Logging engine STDERR to {engine_std_err}")
+        logger.info(f"Logging engine STDOUT to {engine_std_out}")
+        logger.info(f"Logging engine STDERR to {engine_std_err}")
         engine_process = api_utils.run_subprocess(
             engine_cmd, engine_std_err, engine_std_out
         )
         return (manager_process, engine_process)
 
     def __download_latest_release(self):
         """Downloads the latest release version to the binary path."""
```

### Comparing `kaskada-0.1.5/src/kaskada/client.py` & `kaskada-0.1.6/src/kaskada/client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/formatters.css` & `kaskada-0.1.6/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/formatters.js` & `kaskada-0.1.6/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/formatters.py` & `kaskada-0.1.6/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/formatters_helpers.py` & `kaskada-0.1.6/src/kaskada/formatters_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+# pylint: disable=no-member
 from datetime import datetime
 
 import pandas
 from domonic.html import b, pre, td, tr
 from google.protobuf.message import Message
 
-import kaskada.kaskada.v1alpha.schema_pb2 as schema_pb2
+from kaskada.kaskada.v1alpha import schema_pb2
 
 """
 NOTES:
 
 Use `hasattr(obj, prop) to test if an object has a property`
 Use `obj.HasField(prop) to test if an object has a specific one-of`
 """
```

### Comparing `kaskada-0.1.5/src/kaskada/formatters_shared.py` & `kaskada-0.1.6/src/kaskada/formatters_shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member
 import operator
 import pprint
 from typing import Optional
 
 import pandas as pd
 from domonic.html import pre, table, td, th, tr
 from domonic.utils import Utils
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/options_pb2.cpython-39.pyc` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,119 @@
-00000000: 610d 0d0a 0000 0000 2038 4164 3607 0000  a....... 8Ad6...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
-00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
-00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
-00000070: a00c a100 5a0d 6401 6407 6c01 6d0e 5a0f  ....Z.d.d.l.m.Z.
-00000080: 0100 6505 a00c a100 a010 6408 a101 5a11  ..e.......d...Z.
-00000090: 6409 5a12 6511 6a13 640a 1900 5a14 6503  d.Z.e.j.d...Z.e.
-000000a0: 6a15 640b 6b02 7292 650f 6a16 a017 6514  j.d.k.r.e.j...e.
-000000b0: a101 0100 640c 6511 5f18 640d 6511 5f19  ....d.e._.d.e._.
-000000c0: 640c 5300 290e 7a1f 4765 6e65 7261 7465  d.S.).z.Generate
-000000d0: 6420 7072 6f74 6f63 6f6c 2062 7566 6665  d protocol buffe
-000000e0: 7220 636f 6465 2ee9 0000 0000 2901 da0a  r code......)...
-000000f0: 6465 7363 7269 7074 6f72 2901 da0f 6465  descriptor)...de
-00000100: 7363 7269 7074 6f72 5f70 6f6f 6c29 01da  scriptor_pool)..
-00000110: 076d 6573 7361 6765 2901 da0a 7265 666c  .message)...refl
-00000120: 6563 7469 6f6e 2901 da0f 7379 6d62 6f6c  ection)...symbol
-00000130: 5f64 6174 6162 6173 6529 01da 0e64 6573  _database)...des
-00000140: 6372 6970 746f 725f 7062 3273 a801 0000  criptor_pb2s....
-00000150: 0a25 6b61 736b 6164 612f 6b61 736b 6164  .%kaskada/kaskad
-00000160: 612f 7631 616c 7068 612f 6f70 7469 6f6e  a/v1alpha/option
-00000170: 732e 7072 6f74 6f12 176b 6173 6b61 6461  s.proto..kaskada
-00000180: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00000190: 1a20 676f 6f67 6c65 2f70 726f 746f 6275  . google/protobu
-000001a0: 662f 6465 7363 7269 7074 6f72 2e70 726f  f/descriptor.pro
-000001b0: 746f 3a3d 0a09 7365 6e73 6974 6976 6512  to:=..sensitive.
-000001c0: 1d2e 676f 6f67 6c65 2e70 726f 746f 6275  ..google.protobu
-000001d0: 662e 4669 656c 644f 7074 696f 6e73 18d0  f.FieldOptions..
-000001e0: 8603 2001 2808 5209 7365 6e73 6974 6976  .. .(.R.sensitiv
-000001f0: 6542 fc01 0a1b 636f 6d2e 6b61 736b 6164  eB....com.kaskad
-00000200: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-00000210: 6142 0c4f 7074 696f 6e73 5072 6f74 6f50  aB.OptionsProtoP
-00000220: 015a 5167 6974 6875 622e 636f 6d2f 6b61  .ZQgithub.com/ka
-00000230: 736b 6164 612d 6169 2f6b 6173 6b61 6461  skada-ai/kaskada
-00000240: 2f67 656e 2f70 726f 746f 2f67 6f2f 6b61  /gen/proto/go/ka
-00000250: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
-00000260: 616c 7068 613b 6b61 736b 6164 6176 3161  alpha;kaskadav1a
-00000270: 6c70 6861 a202 034b 4b58 aa02 174b 6173  lpha...KKX...Kas
-00000280: 6b61 6461 2e4b 6173 6b61 6461 2e56 3161  kada.Kaskada.V1a
-00000290: 6c70 6861 ca02 174b 6173 6b61 6461 5c4b  lpha...Kaskada\K
-000002a0: 6173 6b61 6461 5c56 3161 6c70 6861 e202  askada\V1alpha..
-000002b0: 234b 6173 6b61 6461 5c4b 6173 6b61 6461  #Kaskada\Kaskada
-000002c0: 5c56 3161 6c70 6861 5c47 5042 4d65 7461  \V1alpha\GPBMeta
-000002d0: 6461 7461 ea02 194b 6173 6b61 6461 3a3a  data...Kaskada::
-000002e0: 4b61 736b 6164 613a 3a56 3161 6c70 6861  Kaskada::V1alpha
-000002f0: 6206 7072 6f74 6f33 6950 c300 00da 0973  b.proto3iP.....s
-00000300: 656e 7369 7469 7665 464e 73fc 0000 000a  ensitiveFNs.....
-00000310: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
-00000320: 6b61 6461 2e76 3161 6c70 6861 420c 4f70  kada.v1alphaB.Op
-00000330: 7469 6f6e 7350 726f 746f 5001 5a51 6769  tionsProtoP.ZQgi
-00000340: 7468 7562 2e63 6f6d 2f6b 6173 6b61 6461  thub.com/kaskada
-00000350: 2d61 692f 6b61 736b 6164 612f 6765 6e2f  -ai/kaskada/gen/
-00000360: 7072 6f74 6f2f 676f 2f6b 6173 6b61 6461  proto/go/kaskada
-00000370: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
-00000380: 3b6b 6173 6b61 6461 7631 616c 7068 61a2  ;kaskadav1alpha.
-00000390: 0203 4b4b 58aa 0217 4b61 736b 6164 612e  ..KKX...Kaskada.
-000003a0: 4b61 736b 6164 612e 5631 616c 7068 61ca  Kaskada.V1alpha.
-000003b0: 0217 4b61 736b 6164 615c 4b61 736b 6164  ..Kaskada\Kaskad
-000003c0: 615c 5631 616c 7068 61e2 0223 4b61 736b  a\V1alpha..#Kask
-000003d0: 6164 615c 4b61 736b 6164 615c 5631 616c  ada\Kaskada\V1al
-000003e0: 7068 615c 4750 424d 6574 6164 6174 61ea  pha\GPBMetadata.
-000003f0: 0219 4b61 736b 6164 613a 3a4b 6173 6b61  ..Kaskada::Kaska
-00000400: 6461 3a3a 5631 616c 7068 6129 1ada 075f  da::V1alpha)..._
-00000410: 5f64 6f63 5f5f da0f 676f 6f67 6c65 2e70  _doc__..google.p
-00000420: 726f 746f 6275 6672 0200 0000 da0b 5f64  rotobufr......_d
-00000430: 6573 6372 6970 746f 7272 0300 0000 da10  escriptorr......
-00000440: 5f64 6573 6372 6970 746f 725f 706f 6f6c  _descriptor_pool
-00000450: 7204 0000 00da 085f 6d65 7373 6167 6572  r......_messager
-00000460: 0500 0000 da0b 5f72 6566 6c65 6374 696f  ......_reflectio
-00000470: 6e72 0600 0000 da10 5f73 796d 626f 6c5f  nr......_symbol_
-00000480: 6461 7461 6261 7365 da07 4465 6661 756c  database..Defaul
-00000490: 74da 075f 7379 6d5f 6462 7207 0000 005a  t.._sym_dbr....Z
-000004a0: 2767 6f6f 676c 655f 646f 745f 7072 6f74  'google_dot_prot
-000004b0: 6f62 7566 5f64 6f74 5f64 6573 6372 6970  obuf_dot_descrip
-000004c0: 746f 725f 5f70 6232 da11 4164 6453 6572  tor__pb2..AddSer
-000004d0: 6961 6c69 7a65 6446 696c 65da 0a44 4553  ializedFile..DES
-000004e0: 4352 4950 544f 525a 1653 454e 5349 5449  CRIPTORZ.SENSITI
-000004f0: 5645 5f46 4945 4c44 5f4e 554d 4245 52da  VE_FIELD_NUMBER.
-00000500: 1265 7874 656e 7369 6f6e 735f 6279 5f6e  .extensions_by_n
-00000510: 616d 6572 0800 0000 da12 5f55 5345 5f43  amer......_USE_C
-00000520: 5f44 4553 4352 4950 544f 5253 da0c 4669  _DESCRIPTORS..Fi
-00000530: 656c 644f 7074 696f 6e73 da11 5265 6769  eldOptions..Regi
-00000540: 7374 6572 4578 7465 6e73 696f 6eda 085f  sterExtension.._
-00000550: 6f70 7469 6f6e 73da 135f 7365 7269 616c  options.._serial
-00000560: 697a 6564 5f6f 7074 696f 6e73 a900 721a  ized_options..r.
-00000570: 0000 0072 1a00 0000 fa2f 2f73 7263 2f73  ...r.....//src/s
-00000580: 7263 2f6b 6173 6b61 6461 2f6b 6173 6b61  rc/kaskada/kaska
-00000590: 6461 2f76 3161 6c70 6861 2f6f 7074 696f  da/v1alpha/optio
-000005a0: 6e73 5f70 6232 2e70 79da 083c 6d6f 6475  ns_pb2.py..<modu
-000005b0: 6c65 3e04 0000 0073 1c00 0000 0401 0c01  le>....s........
-000005c0: 0c01 0c01 0c01 0c03 0803 0c03 0e03 0401  ................
-000005d0: 0a02 0a01 0c02 0601                      ........
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 2320 4765 6e65 7261  f-8 -*-.# Genera
+00000020: 7465 6420 6279 2074 6865 2070 726f 746f  ted by the proto
+00000030: 636f 6c20 6275 6666 6572 2063 6f6d 7069  col buffer compi
+00000040: 6c65 722e 2020 444f 204e 4f54 2045 4449  ler.  DO NOT EDI
+00000050: 5421 0a23 2073 6f75 7263 653a 206b 6173  T!.# source: kas
+00000060: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+00000070: 6c70 6861 2f6f 7074 696f 6e73 2e70 726f  lpha/options.pro
+00000080: 746f 0a22 2222 4765 6e65 7261 7465 6420  to."""Generated 
+00000090: 7072 6f74 6f63 6f6c 2062 7566 6665 7220  protocol buffer 
+000000a0: 636f 6465 2e22 2222 0a66 726f 6d20 676f  code.""".from go
+000000b0: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+000000c0: 7465 726e 616c 2069 6d70 6f72 7420 6275  ternal import bu
+000000d0: 696c 6465 7220 6173 205f 6275 696c 6465  ilder as _builde
+000000e0: 720a 6672 6f6d 2067 6f6f 676c 652e 7072  r.from google.pr
+000000f0: 6f74 6f62 7566 2069 6d70 6f72 7420 6465  otobuf import de
+00000100: 7363 7269 7074 6f72 2061 7320 5f64 6573  scriptor as _des
+00000110: 6372 6970 746f 720a 6672 6f6d 2067 6f6f  criptor.from goo
+00000120: 676c 652e 7072 6f74 6f62 7566 2069 6d70  gle.protobuf imp
+00000130: 6f72 7420 6465 7363 7269 7074 6f72 5f70  ort descriptor_p
+00000140: 6f6f 6c20 6173 205f 6465 7363 7269 7074  ool as _descript
+00000150: 6f72 5f70 6f6f 6c0a 6672 6f6d 2067 6f6f  or_pool.from goo
+00000160: 676c 652e 7072 6f74 6f62 7566 2069 6d70  gle.protobuf imp
+00000170: 6f72 7420 7379 6d62 6f6c 5f64 6174 6162  ort symbol_datab
+00000180: 6173 6520 6173 205f 7379 6d62 6f6c 5f64  ase as _symbol_d
+00000190: 6174 6162 6173 650a 2320 4040 7072 6f74  atabase.# @@prot
+000001a0: 6f63 5f69 6e73 6572 7469 6f6e 5f70 6f69  oc_insertion_poi
+000001b0: 6e74 2869 6d70 6f72 7473 290a 0a5f 7379  nt(imports).._sy
+000001c0: 6d5f 6462 203d 205f 7379 6d62 6f6c 5f64  m_db = _symbol_d
+000001d0: 6174 6162 6173 652e 4465 6661 756c 7428  atabase.Default(
+000001e0: 290a 0a0a 6672 6f6d 2067 6f6f 676c 652e  )...from google.
+000001f0: 7072 6f74 6f62 7566 2069 6d70 6f72 7420  protobuf import 
+00000200: 6465 7363 7269 7074 6f72 5f70 6232 2061  descriptor_pb2 a
+00000210: 7320 676f 6f67 6c65 5f64 6f74 5f70 726f  s google_dot_pro
+00000220: 746f 6275 665f 646f 745f 6465 7363 7269  tobuf_dot_descri
+00000230: 7074 6f72 5f5f 7062 320a 0a0a 4445 5343  ptor__pb2...DESC
+00000240: 5249 5054 4f52 203d 205f 6465 7363 7269  RIPTOR = _descri
+00000250: 7074 6f72 5f70 6f6f 6c2e 4465 6661 756c  ptor_pool.Defaul
+00000260: 7428 292e 4164 6453 6572 6961 6c69 7a65  t().AddSerialize
+00000270: 6446 696c 6528 6227 5c6e 256b 6173 6b61  dFile(b'\n%kaska
+00000280: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
+00000290: 6861 2f6f 7074 696f 6e73 2e70 726f 746f  ha/options.proto
+000002a0: 5c78 3132 5c78 3137 6b61 736b 6164 612e  \x12\x17kaskada.
+000002b0: 6b61 736b 6164 612e 7631 616c 7068 615c  kaskada.v1alpha\
+000002c0: 7831 6120 676f 6f67 6c65 2f70 726f 746f  x1a google/proto
+000002d0: 6275 662f 6465 7363 7269 7074 6f72 2e70  buf/descriptor.p
+000002e0: 726f 746f 3a3d 5c6e 5c74 7365 6e73 6974  roto:=\n\tsensit
+000002f0: 6976 655c 7831 325c 7831 642e 676f 6f67  ive\x12\x1d.goog
+00000300: 6c65 2e70 726f 746f 6275 662e 4669 656c  le.protobuf.Fiel
+00000310: 644f 7074 696f 6e73 5c78 3138 5c78 6430  dOptions\x18\xd0
+00000320: 5c78 3836 5c78 3033 205c 7830 3128 5c78  \x86\x03 \x01(\x
+00000330: 3038 525c 7473 656e 7369 7469 7665 425c  08R\tsensitiveB\
+00000340: 7866 635c 7830 315c 6e5c 7831 625c 7836  xfc\x01\n\x1b\x6
+00000350: 336f 6d2e 6b61 736b 6164 612e 6b61 736b  3om.kaskada.kask
+00000360: 6164 612e 7631 616c 7068 6142 5c78 3063  ada.v1alphaB\x0c
+00000370: 4f70 7469 6f6e 7350 726f 746f 505c 7830  OptionsProtoP\x0
+00000380: 315a 5167 6974 6875 622e 636f 6d2f 6b61  1ZQgithub.com/ka
+00000390: 736b 6164 612d 6169 2f6b 6173 6b61 6461  skada-ai/kaskada
+000003a0: 2f67 656e 2f70 726f 746f 2f67 6f2f 6b61  /gen/proto/go/ka
+000003b0: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+000003c0: 616c 7068 613b 6b61 736b 6164 6176 3161  alpha;kaskadav1a
+000003d0: 6c70 6861 5c78 6132 5c78 3032 5c78 3033  lpha\xa2\x02\x03
+000003e0: 4b4b 585c 7861 615c 7830 325c 7831 374b  KKX\xaa\x02\x17K
+000003f0: 6173 6b61 6461 2e4b 6173 6b61 6461 2e56  askada.Kaskada.V
+00000400: 3161 6c70 6861 5c78 6361 5c78 3032 5c78  1alpha\xca\x02\x
+00000410: 3137 4b61 736b 6164 615c 5c4b 6173 6b61  17Kaskada\\Kaska
+00000420: 6461 5c5c 5631 616c 7068 615c 7865 325c  da\\V1alpha\xe2\
+00000430: 7830 3223 4b61 736b 6164 615c 5c4b 6173  x02#Kaskada\\Kas
+00000440: 6b61 6461 5c5c 5631 616c 7068 615c 5c47  kada\\V1alpha\\G
+00000450: 5042 4d65 7461 6461 7461 5c78 6561 5c78  PBMetadata\xea\x
+00000460: 3032 5c78 3139 4b61 736b 6164 613a 3a4b  02\x19Kaskada::K
+00000470: 6173 6b61 6461 3a3a 5631 616c 7068 6162  askada::V1alphab
+00000480: 5c78 3036 7072 6f74 6f33 2729 0a0a 5f67  \x06proto3').._g
+00000490: 6c6f 6261 6c73 203d 2067 6c6f 6261 6c73  lobals = globals
+000004a0: 2829 0a5f 6275 696c 6465 722e 4275 696c  ()._builder.Buil
+000004b0: 644d 6573 7361 6765 416e 6445 6e75 6d44  dMessageAndEnumD
+000004c0: 6573 6372 6970 746f 7273 2844 4553 4352  escriptors(DESCR
+000004d0: 4950 544f 522c 205f 676c 6f62 616c 7329  IPTOR, _globals)
+000004e0: 0a5f 6275 696c 6465 722e 4275 696c 6454  ._builder.BuildT
+000004f0: 6f70 4465 7363 7269 7074 6f72 7341 6e64  opDescriptorsAnd
+00000500: 4d65 7373 6167 6573 2844 4553 4352 4950  Messages(DESCRIP
+00000510: 544f 522c 2027 6b61 736b 6164 612e 6b61  TOR, 'kaskada.ka
+00000520: 736b 6164 612e 7631 616c 7068 612e 6f70  skada.v1alpha.op
+00000530: 7469 6f6e 735f 7062 3227 2c20 5f67 6c6f  tions_pb2', _glo
+00000540: 6261 6c73 290a 6966 205f 6465 7363 7269  bals).if _descri
+00000550: 7074 6f72 2e5f 5553 455f 435f 4445 5343  ptor._USE_C_DESC
+00000560: 5249 5054 4f52 5320 3d3d 2046 616c 7365  RIPTORS == False
+00000570: 3a0a 2020 676f 6f67 6c65 5f64 6f74 5f70  :.  google_dot_p
+00000580: 726f 746f 6275 665f 646f 745f 6465 7363  rotobuf_dot_desc
+00000590: 7269 7074 6f72 5f5f 7062 322e 4669 656c  riptor__pb2.Fiel
+000005a0: 644f 7074 696f 6e73 2e52 6567 6973 7465  dOptions.Registe
+000005b0: 7245 7874 656e 7369 6f6e 2873 656e 7369  rExtension(sensi
+000005c0: 7469 7665 290a 0a20 2044 4553 4352 4950  tive)..  DESCRIP
+000005d0: 544f 522e 5f6f 7074 696f 6e73 203d 204e  TOR._options = N
+000005e0: 6f6e 650a 2020 4445 5343 5249 5054 4f52  one.  DESCRIPTOR
+000005f0: 2e5f 7365 7269 616c 697a 6564 5f6f 7074  ._serialized_opt
+00000600: 696f 6e73 203d 2062 275c 6e5c 3033 3363  ions = b'\n\033c
+00000610: 6f6d 2e6b 6173 6b61 6461 2e6b 6173 6b61  om.kaskada.kaska
+00000620: 6461 2e76 3161 6c70 6861 425c 3031 344f  da.v1alphaB\014O
+00000630: 7074 696f 6e73 5072 6f74 6f50 5c30 3031  ptionsProtoP\001
+00000640: 5a51 6769 7468 7562 2e63 6f6d 2f6b 6173  ZQgithub.com/kas
+00000650: 6b61 6461 2d61 692f 6b61 736b 6164 612f  kada-ai/kaskada/
+00000660: 6765 6e2f 7072 6f74 6f2f 676f 2f6b 6173  gen/proto/go/kas
+00000670: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+00000680: 6c70 6861 3b6b 6173 6b61 6461 7631 616c  lpha;kaskadav1al
+00000690: 7068 615c 3234 325c 3030 325c 3030 334b  pha\242\002\003K
+000006a0: 4b58 5c32 3532 5c30 3032 5c30 3237 4b61  KX\252\002\027Ka
+000006b0: 736b 6164 612e 4b61 736b 6164 612e 5631  skada.Kaskada.V1
+000006c0: 616c 7068 615c 3331 325c 3030 325c 3032  alpha\312\002\02
+000006d0: 374b 6173 6b61 6461 5c5c 4b61 736b 6164  7Kaskada\\Kaskad
+000006e0: 615c 5c56 3161 6c70 6861 5c33 3432 5c30  a\\V1alpha\342\0
+000006f0: 3032 234b 6173 6b61 6461 5c5c 4b61 736b  02#Kaskada\\Kask
+00000700: 6164 615c 5c56 3161 6c70 6861 5c5c 4750  ada\\V1alpha\\GP
+00000710: 424d 6574 6164 6174 615c 3335 325c 3030  BMetadata\352\00
+00000720: 325c 3033 314b 6173 6b61 6461 3a3a 4b61  2\031Kaskada::Ka
+00000730: 736b 6164 613a 3a56 3161 6c70 6861 270a  skada::V1alpha'.
+00000740: 2320 4040 7072 6f74 6f63 5f69 6e73 6572  # @@protoc_inser
+00000750: 7469 6f6e 5f70 6f69 6e74 286d 6f64 756c  tion_point(modul
+00000760: 655f 7363 6f70 6529 0a                   e_scope).
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/pulsar_pb2.cpython-39.pyc` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,150 +1,176 @@
-00000000: 610d 0d0a 0000 0000 2038 4164 e90d 0000  a....... 8Ad....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
-00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
-00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
-00000070: a00c a100 5a0d 6401 6407 6c01 6d0e 5a0f  ....Z.d.d.l.m.Z.
-00000080: 0100 6401 6408 6c10 6d11 5a12 0100 6505  ..d.d.l.m.Z...e.
-00000090: a00c a100 a013 6409 a101 5a14 6514 6a15  ......d...Z.e.j.
-000000a0: 640a 1900 5a16 6514 6a15 640b 1900 5a17  d...Z.e.j.d...Z.
-000000b0: 6509 a018 640a 6507 6a19 6601 6516 640c  e...d.e.j.f.e.d.
-000000c0: 640d 9c02 a103 5a1a 650d a01b 651a a101  d.....Z.e...e...
-000000d0: 0100 6509 a018 640b 6507 6a19 6601 6517  ..e...d.e.j.f.e.
-000000e0: 640c 640d 9c02 a103 5a1c 650d a01b 651c  d.d.....Z.e...e.
-000000f0: a101 0100 6503 6a1d 640e 6b02 9001 720e  ....e.j.d.k...r.
-00000100: 640f 6514 5f1e 6410 6514 5f1f 640f 6516  d.e._.d.e._.d.e.
-00000110: 6a20 6411 1900 5f1e 6412 6516 6a20 6411  j d..._.d.e.j d.
-00000120: 1900 5f1f 6413 6516 5f21 6414 6516 5f22  .._.d.e._!d.e._"
-00000130: 6415 6517 5f21 6416 6517 5f22 640f 5300  d.e._!d.e._"d.S.
-00000140: 2917 7a1f 4765 6e65 7261 7465 6420 7072  ).z.Generated pr
-00000150: 6f74 6f63 6f6c 2062 7566 6665 7220 636f  otocol buffer co
-00000160: 6465 2ee9 0000 0000 2901 da0a 6465 7363  de......)...desc
-00000170: 7269 7074 6f72 2901 da0f 6465 7363 7269  riptor)...descri
-00000180: 7074 6f72 5f70 6f6f 6c29 01da 076d 6573  ptor_pool)...mes
-00000190: 7361 6765 2901 da0a 7265 666c 6563 7469  sage)...reflecti
-000001a0: 6f6e 2901 da0f 7379 6d62 6f6c 5f64 6174  on)...symbol_dat
-000001b0: 6162 6173 6529 01da 0d74 696d 6573 7461  abase)...timesta
-000001c0: 6d70 5f70 6232 2901 da0b 6f70 7469 6f6e  mp_pb2)...option
-000001d0: 735f 7062 3273 5c03 0000 0a24 6b61 736b  s_pb2s\....$kask
-000001e0: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-000001f0: 7068 612f 7075 6c73 6172 2e70 726f 746f  pha/pulsar.proto
-00000200: 1217 6b61 736b 6164 612e 6b61 736b 6164  ..kaskada.kaskad
-00000210: 612e 7631 616c 7068 611a 1f67 6f6f 676c  a.v1alpha..googl
-00000220: 652f 7072 6f74 6f62 7566 2f74 696d 6573  e/protobuf/times
-00000230: 7461 6d70 2e70 726f 746f 1a25 6b61 736b  tamp.proto.%kask
-00000240: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-00000250: 7068 612f 6f70 7469 6f6e 732e 7072 6f74  pha/options.prot
-00000260: 6f22 8502 0a0c 5075 6c73 6172 436f 6e66  o"....PulsarConf
-00000270: 6967 122c 0a12 6272 6f6b 6572 5f73 6572  ig.,..broker_ser
-00000280: 7669 6365 5f75 726c 1801 2001 2809 5210  vice_url.. .(.R.
-00000290: 6272 6f6b 6572 5365 7276 6963 6555 726c  brokerServiceUrl
-000002a0: 122a 0a11 6164 6d69 6e5f 7365 7276 6963  .*..admin_servic
-000002b0: 655f 7572 6c18 0220 0128 0952 0f61 646d  e_url.. .(.R.adm
-000002c0: 696e 5365 7276 6963 6555 726c 121f 0a0b  inServiceUrl....
-000002d0: 6175 7468 5f70 6c75 6769 6e18 0320 0128  auth_plugin.. .(
-000002e0: 0952 0a61 7574 6850 6c75 6769 6e12 250a  .R.authPlugin.%.
-000002f0: 0b61 7574 685f 7061 7261 6d73 1804 2001  .auth_params.. .
-00000300: 2809 4204 80b5 1801 520a 6175 7468 5061  (.B.....R.authPa
-00000310: 7261 6d73 1216 0a06 7465 6e61 6e74 1805  rams....tenant..
-00000320: 2001 2809 5206 7465 6e61 6e74 121c 0a09   .(.R.tenant....
-00000330: 6e61 6d65 7370 6163 6518 0620 0128 0952  namespace.. .(.R
-00000340: 096e 616d 6573 7061 6365 121d 0a0a 746f  .namespace....to
-00000350: 7069 635f 6e61 6d65 1807 2001 2809 5209  pic_name.. .(.R.
-00000360: 746f 7069 634e 616d 6522 c401 0a12 5075  topicName"....Pu
-00000370: 6c73 6172 5375 6273 6372 6970 7469 6f6e  lsarSubscription
-00000380: 123d 0a06 636f 6e66 6967 1801 2001 280b  .=..config.. .(.
-00000390: 3225 2e6b 6173 6b61 6461 2e6b 6173 6b61  2%.kaskada.kaska
-000003a0: 6461 2e76 3161 6c70 6861 2e50 756c 7361  da.v1alpha.Pulsa
-000003b0: 7243 6f6e 6669 6752 0663 6f6e 6669 6712  rConfigR.config.
-000003c0: 270a 0f73 7562 7363 7269 7074 696f 6e5f  '..subscription_
-000003d0: 6964 1802 2001 2809 520e 7375 6273 6372  id.. .(.R.subscr
-000003e0: 6970 7469 6f6e 4964 1246 0a11 6c61 7374  iptionId.F..last
-000003f0: 5f70 7562 6c69 7368 5f74 696d 6518 0320  _publish_time.. 
-00000400: 0128 0b32 1a2e 676f 6f67 6c65 2e70 726f  .(.2..google.pro
-00000410: 746f 6275 662e 5469 6d65 7374 616d 7052  tobuf.TimestampR
-00000420: 0f6c 6173 7450 7562 6c69 7368 5469 6d65  .lastPublishTime
-00000430: 42fb 010a 1b63 6f6d 2e6b 6173 6b61 6461  B....com.kaskada
-00000440: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00000450: 420b 5075 6c73 6172 5072 6f74 6f50 015a  B.PulsarProtoP.Z
-00000460: 5167 6974 6875 622e 636f 6d2f 6b61 736b  Qgithub.com/kask
-00000470: 6164 612d 6169 2f6b 6173 6b61 6461 2f67  ada-ai/kaskada/g
-00000480: 656e 2f70 726f 746f 2f67 6f2f 6b61 736b  en/proto/go/kask
-00000490: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-000004a0: 7068 613b 6b61 736b 6164 6176 3161 6c70  pha;kaskadav1alp
-000004b0: 6861 a202 034b 4b58 aa02 174b 6173 6b61  ha...KKX...Kaska
-000004c0: 6461 2e4b 6173 6b61 6461 2e56 3161 6c70  da.Kaskada.V1alp
-000004d0: 6861 ca02 174b 6173 6b61 6461 5c4b 6173  ha...Kaskada\Kas
-000004e0: 6b61 6461 5c56 3161 6c70 6861 e202 234b  kada\V1alpha..#K
-000004f0: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
-00000500: 3161 6c70 6861 5c47 5042 4d65 7461 6461  1alpha\GPBMetada
-00000510: 7461 ea02 194b 6173 6b61 6461 3a3a 4b61  ta...Kaskada::Ka
-00000520: 736b 6164 613a 3a56 3161 6c70 6861 6206  skada::V1alphab.
-00000530: 7072 6f74 6f33 da0c 5075 6c73 6172 436f  proto3..PulsarCo
-00000540: 6e66 6967 da12 5075 6c73 6172 5375 6273  nfig..PulsarSubs
-00000550: 6372 6970 7469 6f6e 7a22 6b61 736b 6164  criptionz"kaskad
-00000560: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-00000570: 612e 7075 6c73 6172 5f70 6232 2902 da0a  a.pulsar_pb2)...
-00000580: 4445 5343 5249 5054 4f52 da0a 5f5f 6d6f  DESCRIPTOR..__mo
-00000590: 6475 6c65 5f5f 464e 73fb 0000 000a 1b63  dule__FNs......c
-000005a0: 6f6d 2e6b 6173 6b61 6461 2e6b 6173 6b61  om.kaskada.kaska
-000005b0: 6461 2e76 3161 6c70 6861 420b 5075 6c73  da.v1alphaB.Puls
-000005c0: 6172 5072 6f74 6f50 015a 5167 6974 6875  arProtoP.ZQgithu
-000005d0: 622e 636f 6d2f 6b61 736b 6164 612d 6169  b.com/kaskada-ai
-000005e0: 2f6b 6173 6b61 6461 2f67 656e 2f70 726f  /kaskada/gen/pro
-000005f0: 746f 2f67 6f2f 6b61 736b 6164 612f 6b61  to/go/kaskada/ka
-00000600: 736b 6164 612f 7631 616c 7068 613b 6b61  skada/v1alpha;ka
-00000610: 736b 6164 6176 3161 6c70 6861 a202 034b  skadav1alpha...K
-00000620: 4b58 aa02 174b 6173 6b61 6461 2e4b 6173  KX...Kaskada.Kas
-00000630: 6b61 6461 2e56 3161 6c70 6861 ca02 174b  kada.V1alpha...K
-00000640: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
-00000650: 3161 6c70 6861 e202 234b 6173 6b61 6461  1alpha..#Kaskada
-00000660: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
-00000670: 5c47 5042 4d65 7461 6461 7461 ea02 194b  \GPBMetadata...K
-00000680: 6173 6b61 6461 3a3a 4b61 736b 6164 613a  askada::Kaskada:
-00000690: 3a56 3161 6c70 6861 5a0b 6175 7468 5f70  :V1alphaZ.auth_p
-000006a0: 6172 616d 7373 0400 0000 80b5 1801 e98a  aramss..........
-000006b0: 0000 0069 8f01 0000 6992 0100 0069 5602  ...i....i....iV.
-000006c0: 0000 2923 da07 5f5f 646f 635f 5fda 0f67  ..)#..__doc__..g
-000006d0: 6f6f 676c 652e 7072 6f74 6f62 7566 7202  oogle.protobufr.
-000006e0: 0000 00da 0b5f 6465 7363 7269 7074 6f72  ....._descriptor
-000006f0: 7203 0000 00da 105f 6465 7363 7269 7074  r......_descript
-00000700: 6f72 5f70 6f6f 6c72 0400 0000 da08 5f6d  or_poolr......_m
-00000710: 6573 7361 6765 7205 0000 00da 0b5f 7265  essager......_re
-00000720: 666c 6563 7469 6f6e 7206 0000 00da 105f  flectionr......_
-00000730: 7379 6d62 6f6c 5f64 6174 6162 6173 65da  symbol_database.
-00000740: 0744 6566 6175 6c74 da07 5f73 796d 5f64  .Default.._sym_d
-00000750: 6272 0700 0000 5a26 676f 6f67 6c65 5f64  br....Z&google_d
-00000760: 6f74 5f70 726f 746f 6275 665f 646f 745f  ot_protobuf_dot_
-00000770: 7469 6d65 7374 616d 705f 5f70 6232 da17  timestamp__pb2..
-00000780: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-00000790: 7631 616c 7068 6172 0800 0000 da30 6b61  v1alphar.....0ka
-000007a0: 736b 6164 615f 646f 745f 6b61 736b 6164  skada_dot_kaskad
-000007b0: 615f 646f 745f 7631 616c 7068 615f 646f  a_dot_v1alpha_do
-000007c0: 745f 6f70 7469 6f6e 735f 5f70 6232 da11  t_options__pb2..
-000007d0: 4164 6453 6572 6961 6c69 7a65 6446 696c  AddSerializedFil
-000007e0: 6572 0b00 0000 da15 6d65 7373 6167 655f  er......message_
-000007f0: 7479 7065 735f 6279 5f6e 616d 655a 0d5f  types_by_nameZ._
-00000800: 5055 4c53 4152 434f 4e46 4947 5a13 5f50  PULSARCONFIGZ._P
-00000810: 554c 5341 5253 5542 5343 5249 5054 494f  ULSARSUBSCRIPTIO
-00000820: 4eda 1c47 656e 6572 6174 6564 5072 6f74  N..GeneratedProt
-00000830: 6f63 6f6c 4d65 7373 6167 6554 7970 65da  ocolMessageType.
-00000840: 074d 6573 7361 6765 7209 0000 00da 0f52  .Messager......R
-00000850: 6567 6973 7465 724d 6573 7361 6765 720a  egisterMessager.
-00000860: 0000 00da 125f 5553 455f 435f 4445 5343  ....._USE_C_DESC
-00000870: 5249 5054 4f52 53da 085f 6f70 7469 6f6e  RIPTORS.._option
-00000880: 73da 135f 7365 7269 616c 697a 6564 5f6f  s.._serialized_o
-00000890: 7074 696f 6e73 da0e 6669 656c 6473 5f62  ptions..fields_b
-000008a0: 795f 6e61 6d65 da11 5f73 6572 6961 6c69  y_name.._seriali
-000008b0: 7a65 645f 7374 6172 74da 0f5f 7365 7269  zed_start.._seri
-000008c0: 616c 697a 6564 5f65 6e64 a900 7224 0000  alized_end..r$..
-000008d0: 0072 2400 0000 fa2e 2f73 7263 2f73 7263  .r$...../src/src
-000008e0: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
-000008f0: 2f76 3161 6c70 6861 2f70 756c 7361 725f  /v1alpha/pulsar_
-00000900: 7062 322e 7079 da08 3c6d 6f64 756c 653e  pb2.py..<module>
-00000910: 0400 0000 733c 0000 0004 010c 010c 010c  ....s<..........
-00000920: 010c 010c 0308 030c 010c 030e 040a 010a  ................
-00000930: 010c 0102 0102 fe08 050a 020c 0102 0102  ................
-00000940: fe08 050a 020c 0206 0106 010c 010c 0106  ................
-00000950: 0106 0106 01                             .....
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 2320 4765 6e65 7261  f-8 -*-.# Genera
+00000020: 7465 6420 6279 2074 6865 2070 726f 746f  ted by the proto
+00000030: 636f 6c20 6275 6666 6572 2063 6f6d 7069  col buffer compi
+00000040: 6c65 722e 2020 444f 204e 4f54 2045 4449  ler.  DO NOT EDI
+00000050: 5421 0a23 2073 6f75 7263 653a 206b 6173  T!.# source: kas
+00000060: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+00000070: 6c70 6861 2f70 756c 7361 722e 7072 6f74  lpha/pulsar.prot
+00000080: 6f0a 2222 2247 656e 6572 6174 6564 2070  o."""Generated p
+00000090: 726f 746f 636f 6c20 6275 6666 6572 2063  rotocol buffer c
+000000a0: 6f64 652e 2222 220a 6672 6f6d 2067 6f6f  ode.""".from goo
+000000b0: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
+000000c0: 6572 6e61 6c20 696d 706f 7274 2062 7569  ernal import bui
+000000d0: 6c64 6572 2061 7320 5f62 7569 6c64 6572  lder as _builder
+000000e0: 0a66 726f 6d20 676f 6f67 6c65 2e70 726f  .from google.pro
+000000f0: 746f 6275 6620 696d 706f 7274 2064 6573  tobuf import des
+00000100: 6372 6970 746f 7220 6173 205f 6465 7363  criptor as _desc
+00000110: 7269 7074 6f72 0a66 726f 6d20 676f 6f67  riptor.from goog
+00000120: 6c65 2e70 726f 746f 6275 6620 696d 706f  le.protobuf impo
+00000130: 7274 2064 6573 6372 6970 746f 725f 706f  rt descriptor_po
+00000140: 6f6c 2061 7320 5f64 6573 6372 6970 746f  ol as _descripto
+00000150: 725f 706f 6f6c 0a66 726f 6d20 676f 6f67  r_pool.from goog
+00000160: 6c65 2e70 726f 746f 6275 6620 696d 706f  le.protobuf impo
+00000170: 7274 2073 796d 626f 6c5f 6461 7461 6261  rt symbol_databa
+00000180: 7365 2061 7320 5f73 796d 626f 6c5f 6461  se as _symbol_da
+00000190: 7461 6261 7365 0a23 2040 4070 726f 746f  tabase.# @@proto
+000001a0: 635f 696e 7365 7274 696f 6e5f 706f 696e  c_insertion_poin
+000001b0: 7428 696d 706f 7274 7329 0a0a 5f73 796d  t(imports).._sym
+000001c0: 5f64 6220 3d20 5f73 796d 626f 6c5f 6461  _db = _symbol_da
+000001d0: 7461 6261 7365 2e44 6566 6175 6c74 2829  tabase.Default()
+000001e0: 0a0a 0a66 726f 6d20 6b61 736b 6164 612e  ...from kaskada.
+000001f0: 6b61 736b 6164 612e 7631 616c 7068 6120  kaskada.v1alpha 
+00000200: 696d 706f 7274 206f 7074 696f 6e73 5f70  import options_p
+00000210: 6232 2061 7320 6b61 736b 6164 615f 646f  b2 as kaskada_do
+00000220: 745f 6b61 736b 6164 615f 646f 745f 7631  t_kaskada_dot_v1
+00000230: 616c 7068 615f 646f 745f 6f70 7469 6f6e  alpha_dot_option
+00000240: 735f 5f70 6232 0a0a 0a44 4553 4352 4950  s__pb2...DESCRIP
+00000250: 544f 5220 3d20 5f64 6573 6372 6970 746f  TOR = _descripto
+00000260: 725f 706f 6f6c 2e44 6566 6175 6c74 2829  r_pool.Default()
+00000270: 2e41 6464 5365 7269 616c 697a 6564 4669  .AddSerializedFi
+00000280: 6c65 2862 275c 6e24 6b61 736b 6164 612f  le(b'\n$kaskada/
+00000290: 6b61 736b 6164 612f 7631 616c 7068 612f  kaskada/v1alpha/
+000002a0: 7075 6c73 6172 2e70 726f 746f 5c78 3132  pulsar.proto\x12
+000002b0: 5c78 3137 6b61 736b 6164 612e 6b61 736b  \x17kaskada.kask
+000002c0: 6164 612e 7631 616c 7068 615c 7831 6125  ada.v1alpha\x1a%
+000002d0: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
+000002e0: 7631 616c 7068 612f 6f70 7469 6f6e 732e  v1alpha/options.
+000002f0: 7072 6f74 6f5c 225c 7838 355c 7830 325c  proto\"\x85\x02\
+00000300: 6e5c 7830 6350 756c 7361 7243 6f6e 6669  n\x0cPulsarConfi
+00000310: 675c 7831 322c 5c6e 5c78 3132 5c78 3632  g\x12,\n\x12\x62
+00000320: 726f 6b65 725f 7365 7276 6963 655f 7572  roker_service_ur
+00000330: 6c5c 7831 385c 7830 3120 5c78 3031 285c  l\x18\x01 \x01(\
+00000340: 7452 5c78 3130 5c78 3632 726f 6b65 7253  tR\x10\x62rokerS
+00000350: 6572 7669 6365 5572 6c5c 7831 322a 5c6e  erviceUrl\x12*\n
+00000360: 5c78 3131 5c78 3631 5c78 3634 6d69 6e5f  \x11\x61\x64min_
+00000370: 7365 7276 6963 655f 7572 6c5c 7831 385c  service_url\x18\
+00000380: 7830 3220 5c78 3031 285c 7452 5c78 3066  x02 \x01(\tR\x0f
+00000390: 5c78 3631 5c78 3634 6d69 6e53 6572 7669  \x61\x64minServi
+000003a0: 6365 5572 6c5c 7831 325c 7831 665c 6e5c  ceUrl\x12\x1f\n\
+000003b0: 7830 625c 7836 3175 7468 5f70 6c75 6769  x0b\x61uth_plugi
+000003c0: 6e5c 7831 385c 7830 3320 5c78 3031 285c  n\x18\x03 \x01(\
+000003d0: 7452 5c6e 6175 7468 506c 7567 696e 5c78  tR\nauthPlugin\x
+000003e0: 3132 255c 6e5c 7830 625c 7836 3175 7468  12%\n\x0b\x61uth
+000003f0: 5f70 6172 616d 735c 7831 385c 7830 3420  _params\x18\x04 
+00000400: 5c78 3031 285c 7442 5c78 3034 5c78 3830  \x01(\tB\x04\x80
+00000410: 5c78 6235 5c78 3138 5c78 3031 525c 6e61  \xb5\x18\x01R\na
+00000420: 7574 6850 6172 616d 735c 7831 325c 7831  uthParams\x12\x1
+00000430: 365c 6e5c 7830 3674 656e 616e 745c 7831  6\n\x06tenant\x1
+00000440: 385c 7830 3520 5c78 3031 285c 7452 5c78  8\x05 \x01(\tR\x
+00000450: 3036 7465 6e61 6e74 5c78 3132 5c78 3163  06tenant\x12\x1c
+00000460: 5c6e 5c74 6e61 6d65 7370 6163 655c 7831  \n\tnamespace\x1
+00000470: 385c 7830 3620 5c78 3031 285c 7452 5c74  8\x06 \x01(\tR\t
+00000480: 6e61 6d65 7370 6163 655c 7831 325c 7831  namespace\x12\x1
+00000490: 645c 6e5c 6e74 6f70 6963 5f6e 616d 655c  d\n\ntopic_name\
+000004a0: 7831 385c 7830 3720 5c78 3031 285c 7452  x18\x07 \x01(\tR
+000004b0: 5c74 746f 7069 634e 616d 655c 225c 7861  \ttopicName\"\xa
+000004c0: 385c 7830 315c 6e5c 7831 3250 756c 7361  8\x01\n\x12Pulsa
+000004d0: 7253 7562 7363 7269 7074 696f 6e5c 7831  rSubscription\x1
+000004e0: 323d 5c6e 5c78 3036 5c78 3633 6f6e 6669  2=\n\x06\x63onfi
+000004f0: 675c 7831 385c 7830 3120 5c78 3031 285c  g\x18\x01 \x01(\
+00000500: 7830 625c 7833 3225 2e6b 6173 6b61 6461  x0b\x32%.kaskada
+00000510: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000520: 2e50 756c 7361 7243 6f6e 6669 6752 5c78  .PulsarConfigR\x
+00000530: 3036 5c78 3633 6f6e 6669 675c 7831 325c  06\x63onfig\x12\
+00000540: 275c 6e5c 7830 6673 7562 7363 7269 7074  '\n\x0fsubscript
+00000550: 696f 6e5f 6964 5c78 3138 5c78 3032 205c  ion_id\x18\x02 \
+00000560: 7830 3128 5c74 525c 7830 6573 7562 7363  x01(\tR\x0esubsc
+00000570: 7269 7074 696f 6e49 645c 7831 322a 5c6e  riptionId\x12*\n
+00000580: 5c78 3131 6c61 7374 5f70 7562 6c69 7368  \x11last_publish
+00000590: 5f74 696d 655c 7831 385c 7830 3320 5c78  _time\x18\x03 \x
+000005a0: 3031 285c 7830 3352 5c78 3066 6c61 7374  01(\x03R\x0flast
+000005b0: 5075 626c 6973 6854 696d 6542 5c78 6662  PublishTimeB\xfb
+000005c0: 5c78 3031 5c6e 5c78 3162 5c78 3633 6f6d  \x01\n\x1b\x63om
+000005d0: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+000005e0: 2e76 3161 6c70 6861 425c 7830 6250 756c  .v1alphaB\x0bPul
+000005f0: 7361 7250 726f 746f 505c 7830 315a 5167  sarProtoP\x01ZQg
+00000600: 6974 6875 622e 636f 6d2f 6b61 736b 6164  ithub.com/kaskad
+00000610: 612d 6169 2f6b 6173 6b61 6461 2f67 656e  a-ai/kaskada/gen
+00000620: 2f70 726f 746f 2f67 6f2f 6b61 736b 6164  /proto/go/kaskad
+00000630: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
+00000640: 613b 6b61 736b 6164 6176 3161 6c70 6861  a;kaskadav1alpha
+00000650: 5c78 6132 5c78 3032 5c78 3033 4b4b 585c  \xa2\x02\x03KKX\
+00000660: 7861 615c 7830 325c 7831 374b 6173 6b61  xaa\x02\x17Kaska
+00000670: 6461 2e4b 6173 6b61 6461 2e56 3161 6c70  da.Kaskada.V1alp
+00000680: 6861 5c78 6361 5c78 3032 5c78 3137 4b61  ha\xca\x02\x17Ka
+00000690: 736b 6164 615c 5c4b 6173 6b61 6461 5c5c  skada\\Kaskada\\
+000006a0: 5631 616c 7068 615c 7865 325c 7830 3223  V1alpha\xe2\x02#
+000006b0: 4b61 736b 6164 615c 5c4b 6173 6b61 6461  Kaskada\\Kaskada
+000006c0: 5c5c 5631 616c 7068 615c 5c47 5042 4d65  \\V1alpha\\GPBMe
+000006d0: 7461 6461 7461 5c78 6561 5c78 3032 5c78  tadata\xea\x02\x
+000006e0: 3139 4b61 736b 6164 613a 3a4b 6173 6b61  19Kaskada::Kaska
+000006f0: 6461 3a3a 5631 616c 7068 6162 5c78 3036  da::V1alphab\x06
+00000700: 7072 6f74 6f33 2729 0a0a 5f67 6c6f 6261  proto3').._globa
+00000710: 6c73 203d 2067 6c6f 6261 6c73 2829 0a5f  ls = globals()._
+00000720: 6275 696c 6465 722e 4275 696c 644d 6573  builder.BuildMes
+00000730: 7361 6765 416e 6445 6e75 6d44 6573 6372  sageAndEnumDescr
+00000740: 6970 746f 7273 2844 4553 4352 4950 544f  iptors(DESCRIPTO
+00000750: 522c 205f 676c 6f62 616c 7329 0a5f 6275  R, _globals)._bu
+00000760: 696c 6465 722e 4275 696c 6454 6f70 4465  ilder.BuildTopDe
+00000770: 7363 7269 7074 6f72 7341 6e64 4d65 7373  scriptorsAndMess
+00000780: 6167 6573 2844 4553 4352 4950 544f 522c  ages(DESCRIPTOR,
+00000790: 2027 6b61 736b 6164 612e 6b61 736b 6164   'kaskada.kaskad
+000007a0: 612e 7631 616c 7068 612e 7075 6c73 6172  a.v1alpha.pulsar
+000007b0: 5f70 6232 272c 205f 676c 6f62 616c 7329  _pb2', _globals)
+000007c0: 0a69 6620 5f64 6573 6372 6970 746f 722e  .if _descriptor.
+000007d0: 5f55 5345 5f43 5f44 4553 4352 4950 544f  _USE_C_DESCRIPTO
+000007e0: 5253 203d 3d20 4661 6c73 653a 0a0a 2020  RS == False:..  
+000007f0: 4445 5343 5249 5054 4f52 2e5f 6f70 7469  DESCRIPTOR._opti
+00000800: 6f6e 7320 3d20 4e6f 6e65 0a20 2044 4553  ons = None.  DES
+00000810: 4352 4950 544f 522e 5f73 6572 6961 6c69  CRIPTOR._seriali
+00000820: 7a65 645f 6f70 7469 6f6e 7320 3d20 6227  zed_options = b'
+00000830: 5c6e 5c30 3333 636f 6d2e 6b61 736b 6164  \n\033com.kaskad
+00000840: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000850: 6142 5c30 3133 5075 6c73 6172 5072 6f74  aB\013PulsarProt
+00000860: 6f50 5c30 3031 5a51 6769 7468 7562 2e63  oP\001ZQgithub.c
+00000870: 6f6d 2f6b 6173 6b61 6461 2d61 692f 6b61  om/kaskada-ai/ka
+00000880: 736b 6164 612f 6765 6e2f 7072 6f74 6f2f  skada/gen/proto/
+00000890: 676f 2f6b 6173 6b61 6461 2f6b 6173 6b61  go/kaskada/kaska
+000008a0: 6461 2f76 3161 6c70 6861 3b6b 6173 6b61  da/v1alpha;kaska
+000008b0: 6461 7631 616c 7068 615c 3234 325c 3030  dav1alpha\242\00
+000008c0: 325c 3030 334b 4b58 5c32 3532 5c30 3032  2\003KKX\252\002
+000008d0: 5c30 3237 4b61 736b 6164 612e 4b61 736b  \027Kaskada.Kask
+000008e0: 6164 612e 5631 616c 7068 615c 3331 325c  ada.V1alpha\312\
+000008f0: 3030 325c 3032 374b 6173 6b61 6461 5c5c  002\027Kaskada\\
+00000900: 4b61 736b 6164 615c 5c56 3161 6c70 6861  Kaskada\\V1alpha
+00000910: 5c33 3432 5c30 3032 234b 6173 6b61 6461  \342\002#Kaskada
+00000920: 5c5c 4b61 736b 6164 615c 5c56 3161 6c70  \\Kaskada\\V1alp
+00000930: 6861 5c5c 4750 424d 6574 6164 6174 615c  ha\\GPBMetadata\
+00000940: 3335 325c 3030 325c 3033 314b 6173 6b61  352\002\031Kaska
+00000950: 6461 3a3a 4b61 736b 6164 613a 3a56 3161  da::Kaskada::V1a
+00000960: 6c70 6861 270a 2020 5f50 554c 5341 5243  lpha'.  _PULSARC
+00000970: 4f4e 4649 472e 6669 656c 6473 5f62 795f  ONFIG.fields_by_
+00000980: 6e61 6d65 5b27 6175 7468 5f70 6172 616d  name['auth_param
+00000990: 7327 5d2e 5f6f 7074 696f 6e73 203d 204e  s']._options = N
+000009a0: 6f6e 650a 2020 5f50 554c 5341 5243 4f4e  one.  _PULSARCON
+000009b0: 4649 472e 6669 656c 6473 5f62 795f 6e61  FIG.fields_by_na
+000009c0: 6d65 5b27 6175 7468 5f70 6172 616d 7327  me['auth_params'
+000009d0: 5d2e 5f73 6572 6961 6c69 7a65 645f 6f70  ]._serialized_op
+000009e0: 7469 6f6e 7320 3d20 6227 5c32 3030 5c32  tions = b'\200\2
+000009f0: 3635 5c30 3330 5c30 3031 270a 2020 5f67  65\030\001'.  _g
+00000a00: 6c6f 6261 6c73 5b27 5f50 554c 5341 5243  lobals['_PULSARC
+00000a10: 4f4e 4649 4727 5d2e 5f73 6572 6961 6c69  ONFIG']._seriali
+00000a20: 7a65 645f 7374 6172 743d 3130 350a 2020  zed_start=105.  
+00000a30: 5f67 6c6f 6261 6c73 5b27 5f50 554c 5341  _globals['_PULSA
+00000a40: 5243 4f4e 4649 4727 5d2e 5f73 6572 6961  RCONFIG']._seria
+00000a50: 6c69 7a65 645f 656e 643d 3336 360a 2020  lized_end=366.  
+00000a60: 5f67 6c6f 6261 6c73 5b27 5f50 554c 5341  _globals['_PULSA
+00000a70: 5253 5542 5343 5249 5054 494f 4e27 5d2e  RSUBSCRIPTION'].
+00000a80: 5f73 6572 6961 6c69 7a65 645f 7374 6172  _serialized_star
+00000a90: 743d 3336 390a 2020 5f67 6c6f 6261 6c73  t=369.  _globals
+00000aa0: 5b27 5f50 554c 5341 5253 5542 5343 5249  ['_PULSARSUBSCRI
+00000ab0: 5054 494f 4e27 5d2e 5f73 6572 6961 6c69  PTION']._seriali
+00000ac0: 7a65 645f 656e 643d 3533 370a 2320 4040  zed_end=537.# @@
+00000ad0: 7072 6f74 6f63 5f69 6e73 6572 7469 6f6e  protoc_insertion
+00000ae0: 5f70 6f69 6e74 286d 6f64 756c 655f 7363  _point(module_sc
+00000af0: 6f70 6529 0a                             ope).
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,200 +1,88 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: kaskada/kaskada/v1alpha/common.proto
+# source: kaskada/kaskada/v1alpha/query_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
+from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
+from kaskada.kaskada.v1alpha import destinations_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_destinations__pb2
 from kaskada.kaskada.v1alpha import fenl_diagnostics_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_fenl__diagnostics__pb2
-from kaskada.kaskada.v1alpha import pulsar_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_pulsar__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
+from kaskada.kaskada.v1alpha import view_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_view__service__pb2
+from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/common.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a$kaskada/kaskada/v1alpha/pulsar.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"\xd5\x01\n\nSourceData\x12#\n\x0cparquet_path\x18\x01 \x01(\tH\x00R\x0bparquetPath\x12\x1b\n\x08\x63sv_path\x18\x02 \x01(\tH\x00R\x07\x63svPath\x12\x1b\n\x08\x63sv_data\x18\x03 \x01(\tH\x00R\x07\x63svData\x12^\n\x13pulsar_subscription\x18\x04 \x01(\x0b\x32+.kaskada.kaskada.v1alpha.PulsarSubscriptionH\x00R\x12pulsarSubscriptionB\x08\n\x06source\"]\n\tFileInput\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x10\n\x03uri\x18\x02 \x01(\tR\x03uri\"c\n\x0b\x46ileResults\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x14\n\x05paths\x18\x02 \x03(\tR\x05paths\"\xf5\x01\n\x0bTableConfig\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04uuid\x18\x06 \x01(\tR\x04uuid\x12(\n\x10time_column_name\x18\x02 \x01(\tR\x0etimeColumnName\x12L\n\x13subsort_column_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11subsortColumnName\x12*\n\x11group_column_name\x18\x04 \x01(\tR\x0fgroupColumnName\x12\x1a\n\x08grouping\x18\x05 \x01(\tR\x08grouping\"g\n\rTableMetadata\x12\x37\n\x06schema\x18\x01 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x12\x1d\n\nfile_count\x18\x02 \x01(\x03R\tfileCount\"\xe6\x01\n\x0cPreparedFile\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emin_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cminEventTime\x12@\n\x0emax_event_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12\x19\n\x08num_rows\x18\x04 \x01(\x03R\x07numRows\x12#\n\rmetadata_path\x18\x05 \x01(\tR\x0cmetadataPath\"\xb5\x02\n\tSlicePlan\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x12K\n\x07percent\x18\x02 \x01(\x0b\x32/.kaskada.kaskada.v1alpha.SlicePlan.PercentSliceH\x00R\x07percent\x12U\n\x0b\x65ntity_keys\x18\x03 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SlicePlan.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x01 \x03(\tR\nentityKeysB\x07\n\x05slice\",\n\x04Uuid\x12\x12\n\x04high\x18\x01 \x01(\x04R\x04high\x12\x10\n\x03low\x18\x02 \x01(\x04R\x03low\"\x9f\x02\n\x0cSliceRequest\x12N\n\x07percent\x18\x01 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SliceRequest.PercentSliceH\x00R\x07percent\x12X\n\x0b\x65ntity_keys\x18\x02 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.SliceRequest.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x02 \x03(\tR\nentityKeysB\x07\n\x05slice\"\xc4\x01\n\x08\x41nalysis\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x1f\n\x0b\x63\x61n_execute\x18\x03 \x01(\x08R\ncanExecute\x12\x1d\n\nfree_names\x18\x04 \x03(\tR\tfreeNames\"/\n\x0eRequestDetails\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId*O\n\x08\x46ileType\x12\x19\n\x15\x46ILE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11\x46ILE_TYPE_PARQUET\x10\x01\x12\x11\n\rFILE_TYPE_CSV\x10\x02*\x9b\x01\n\x11PerEntityBehavior\x12#\n\x1fPER_ENTITY_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1b\n\x17PER_ENTITY_BEHAVIOR_ALL\x10\x01\x12\x1d\n\x19PER_ENTITY_BEHAVIOR_FINAL\x10\x02\x12%\n!PER_ENTITY_BEHAVIOR_FINAL_AT_TIME\x10\x03\x42\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0b\x43ommonProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
-
-_FILETYPE = DESCRIPTOR.enum_types_by_name['FileType']
-FileType = enum_type_wrapper.EnumTypeWrapper(_FILETYPE)
-_PERENTITYBEHAVIOR = DESCRIPTOR.enum_types_by_name['PerEntityBehavior']
-PerEntityBehavior = enum_type_wrapper.EnumTypeWrapper(_PERENTITYBEHAVIOR)
-FILE_TYPE_UNSPECIFIED = 0
-FILE_TYPE_PARQUET = 1
-FILE_TYPE_CSV = 2
-PER_ENTITY_BEHAVIOR_UNSPECIFIED = 0
-PER_ENTITY_BEHAVIOR_ALL = 1
-PER_ENTITY_BEHAVIOR_FINAL = 2
-PER_ENTITY_BEHAVIOR_FINAL_AT_TIME = 3
-
-
-_SOURCEDATA = DESCRIPTOR.message_types_by_name['SourceData']
-_FILEINPUT = DESCRIPTOR.message_types_by_name['FileInput']
-_FILERESULTS = DESCRIPTOR.message_types_by_name['FileResults']
-_TABLECONFIG = DESCRIPTOR.message_types_by_name['TableConfig']
-_TABLEMETADATA = DESCRIPTOR.message_types_by_name['TableMetadata']
-_PREPAREDFILE = DESCRIPTOR.message_types_by_name['PreparedFile']
-_SLICEPLAN = DESCRIPTOR.message_types_by_name['SlicePlan']
-_SLICEPLAN_PERCENTSLICE = _SLICEPLAN.nested_types_by_name['PercentSlice']
-_SLICEPLAN_ENTITYKEYSSLICE = _SLICEPLAN.nested_types_by_name['EntityKeysSlice']
-_UUID = DESCRIPTOR.message_types_by_name['Uuid']
-_SLICEREQUEST = DESCRIPTOR.message_types_by_name['SliceRequest']
-_SLICEREQUEST_PERCENTSLICE = _SLICEREQUEST.nested_types_by_name['PercentSlice']
-_SLICEREQUEST_ENTITYKEYSSLICE = _SLICEREQUEST.nested_types_by_name['EntityKeysSlice']
-_ANALYSIS = DESCRIPTOR.message_types_by_name['Analysis']
-_REQUESTDETAILS = DESCRIPTOR.message_types_by_name['RequestDetails']
-SourceData = _reflection.GeneratedProtocolMessageType('SourceData', (_message.Message,), {
-  'DESCRIPTOR' : _SOURCEDATA,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.SourceData)
-  })
-_sym_db.RegisterMessage(SourceData)
-
-FileInput = _reflection.GeneratedProtocolMessageType('FileInput', (_message.Message,), {
-  'DESCRIPTOR' : _FILEINPUT,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.FileInput)
-  })
-_sym_db.RegisterMessage(FileInput)
-
-FileResults = _reflection.GeneratedProtocolMessageType('FileResults', (_message.Message,), {
-  'DESCRIPTOR' : _FILERESULTS,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.FileResults)
-  })
-_sym_db.RegisterMessage(FileResults)
-
-TableConfig = _reflection.GeneratedProtocolMessageType('TableConfig', (_message.Message,), {
-  'DESCRIPTOR' : _TABLECONFIG,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.TableConfig)
-  })
-_sym_db.RegisterMessage(TableConfig)
-
-TableMetadata = _reflection.GeneratedProtocolMessageType('TableMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _TABLEMETADATA,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.TableMetadata)
-  })
-_sym_db.RegisterMessage(TableMetadata)
-
-PreparedFile = _reflection.GeneratedProtocolMessageType('PreparedFile', (_message.Message,), {
-  'DESCRIPTOR' : _PREPAREDFILE,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.PreparedFile)
-  })
-_sym_db.RegisterMessage(PreparedFile)
-
-SlicePlan = _reflection.GeneratedProtocolMessageType('SlicePlan', (_message.Message,), {
-
-  'PercentSlice' : _reflection.GeneratedProtocolMessageType('PercentSlice', (_message.Message,), {
-    'DESCRIPTOR' : _SLICEPLAN_PERCENTSLICE,
-    '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.SlicePlan.PercentSlice)
-    })
-  ,
-
-  'EntityKeysSlice' : _reflection.GeneratedProtocolMessageType('EntityKeysSlice', (_message.Message,), {
-    'DESCRIPTOR' : _SLICEPLAN_ENTITYKEYSSLICE,
-    '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.SlicePlan.EntityKeysSlice)
-    })
-  ,
-  'DESCRIPTOR' : _SLICEPLAN,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.SlicePlan)
-  })
-_sym_db.RegisterMessage(SlicePlan)
-_sym_db.RegisterMessage(SlicePlan.PercentSlice)
-_sym_db.RegisterMessage(SlicePlan.EntityKeysSlice)
-
-Uuid = _reflection.GeneratedProtocolMessageType('Uuid', (_message.Message,), {
-  'DESCRIPTOR' : _UUID,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.Uuid)
-  })
-_sym_db.RegisterMessage(Uuid)
-
-SliceRequest = _reflection.GeneratedProtocolMessageType('SliceRequest', (_message.Message,), {
-
-  'PercentSlice' : _reflection.GeneratedProtocolMessageType('PercentSlice', (_message.Message,), {
-    'DESCRIPTOR' : _SLICEREQUEST_PERCENTSLICE,
-    '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.SliceRequest.PercentSlice)
-    })
-  ,
-
-  'EntityKeysSlice' : _reflection.GeneratedProtocolMessageType('EntityKeysSlice', (_message.Message,), {
-    'DESCRIPTOR' : _SLICEREQUEST_ENTITYKEYSSLICE,
-    '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.SliceRequest.EntityKeysSlice)
-    })
-  ,
-  'DESCRIPTOR' : _SLICEREQUEST,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.SliceRequest)
-  })
-_sym_db.RegisterMessage(SliceRequest)
-_sym_db.RegisterMessage(SliceRequest.PercentSlice)
-_sym_db.RegisterMessage(SliceRequest.EntityKeysSlice)
-
-Analysis = _reflection.GeneratedProtocolMessageType('Analysis', (_message.Message,), {
-  'DESCRIPTOR' : _ANALYSIS,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.Analysis)
-  })
-_sym_db.RegisterMessage(Analysis)
-
-RequestDetails = _reflection.GeneratedProtocolMessageType('RequestDetails', (_message.Message,), {
-  'DESCRIPTOR' : _REQUESTDETAILS,
-  '__module__' : 'kaskada.kaskada.v1alpha.common_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.RequestDetails)
-  })
-_sym_db.RegisterMessage(RequestDetails)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+kaskada/kaskada/v1alpha/query_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a*kaskada/kaskada/v1alpha/destinations.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\x1a*kaskada/kaskada/v1alpha/view_service.proto\x1a\x17validate/validate.proto\"\xc9\x07\n\x05Query\x12\x1e\n\x08query_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x07queryId\x12\'\n\nexpression\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nexpression\x12\x46\n\x0b\x64\x65stination\x18h \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x12@\n\rdata_token_id\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0b\x64\x61taTokenId\x12\x38\n\x05views\x18\x04 \x03(\x0b\x32\x1d.kaskada.kaskada.v1alpha.ViewB\x03\xe0\x41\x03R\x05views\x12V\n\x0fresult_behavior\x18\x05 \x01(\x0e\x32-.kaskada.kaskada.v1alpha.Query.ResultBehaviorR\x0eresultBehavior\x12=\n\x06limits\x18\x06 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.Query.LimitsR\x06limits\x12;\n\x05slice\x18\x07 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x05slice\x12H\n\x12\x63hanged_since_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x63hangedSinceTime\x12\x46\n\x11\x66inal_result_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\x12@\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x1a+\n\x06Limits\x12!\n\x0cpreview_rows\x18\x01 \x01(\x03R\x0bpreviewRows\x1a)\n\x11RedisBulkResponse\x12\x14\n\x05shape\x18\x01 \x03(\x05R\x05shape\"\xa0\x01\n\x0eResultBehavior\x12\x1f\n\x1bRESULT_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1f\n\x1bRESULT_BEHAVIOR_ALL_RESULTS\x10\x01\x12!\n\x1dRESULT_BEHAVIOR_FINAL_RESULTS\x10\x02\x12)\n%RESULT_BEHAVIOR_FINAL_RESULTS_AT_TIME\x10\x03J\x04\x08\x65\x10\x66J\x04\x08\x66\x10gJ\x04\x08g\x10h\"\xac\x01\n\x0cQueryOptions\x12\x17\n\x07\x64ry_run\x18\x01 \x01(\x08R\x06\x64ryRun\x12\x33\n\x15\x65xperimental_features\x18\x02 \x01(\x08R\x14\x65xperimentalFeatures\x12%\n\x0estream_metrics\x18\x03 \x01(\x08R\rstreamMetrics\x12\'\n\x0fpresign_results\x18\x04 \x01(\x08R\x0epresignResults\"\x96\x01\n\x12\x43reateQueryRequest\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.QueryR\x05query\x12J\n\rquery_options\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.QueryOptionsR\x0cqueryOptions\"\x91\n\n\x13\x43reateQueryResponse\x12H\n\x05state\x18\x01 \x01(\x0e\x32\x32.kaskada.kaskada.v1alpha.CreateQueryResponse.StateR\x05state\x12K\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x33.kaskada.kaskada.v1alpha.CreateQueryResponse.ConfigR\x06\x63onfig\x12Q\n\x08\x61nalysis\x18\x03 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.CreateQueryResponse.AnalysisR\x08\x61nalysis\x12S\n\x10\x66\x65nl_diagnostics\x18\x04 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12N\n\x07metrics\x18\x05 \x01(\x0b\x32\x34.kaskada.kaskada.v1alpha.CreateQueryResponse.MetricsR\x07metrics\x12P\n\x0frequest_details\x18\x06 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\x12\x19\n\x08query_id\x18\x07 \x01(\tR\x07queryId\x12\x46\n\x0b\x64\x65stination\x18h \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x1a\x64\n\x08\x41nalysis\x12\x1f\n\x0b\x63\x61n_execute\x18\x01 \x01(\x08R\ncanExecute\x12\x37\n\x06schema\x18\x02 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x1ax\n\x06\x43onfig\x12\"\n\rdata_token_id\x18\x01 \x01(\tR\x0b\x64\x61taTokenId\x12J\n\rslice_request\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x0csliceRequest\x1a\xbe\x02\n\x07Metrics\x12@\n\x0etime_preparing\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\rtimePreparing\x12@\n\x0etime_computing\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\rtimeComputing\x12!\n\x0coutput_files\x18\x03 \x01(\x03R\x0boutputFiles\x12(\n\x10total_input_rows\x18\x04 \x01(\x03R\x0etotalInputRows\x12\x30\n\x14processed_input_rows\x18\x05 \x01(\x03R\x12processedInputRows\x12\x30\n\x14produced_output_rows\x18\x06 \x01(\x03R\x12producedOutputRows\"\x82\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATE_ANALYSIS\x10\x01\x12\x13\n\x0fSTATE_PREPARING\x10\x02\x12\x13\n\x0fSTATE_COMPUTING\x10\x03\x12\x11\n\rSTATE_SUCCESS\x10\x04\x12\x11\n\rSTATE_FAILURE\x10\x05J\x04\x08\x65\x10\x66J\x04\x08\x66\x10gJ\x04\x08g\x10h\"5\n\x0fGetQueryRequest\x12\"\n\x08query_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x07queryId\"M\n\x10GetQueryResponse\x12\x39\n\x05query\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.QueryB\x03\xe0\x41\x03R\x05query\"t\n\x12ListQueriesRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\'\n\tpage_size\x18\x02 \x01(\x05\x42\n\xfa\x42\x07\x1a\x05\x18\xe8\x07(\x00R\x08pageSize\x12\x1d\n\npage_token\x18\x03 \x01(\tR\tpageToken\"\xc9\x01\n\x13ListQueriesResponse\x12\x38\n\x07queries\x18\x01 \x03(\x0b\x32\x1e.kaskada.kaskada.v1alpha.QueryR\x07queries\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\x12P\n\x0frequest_details\x18\x03 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails2\xaa\x03\n\x0cQueryService\x12\x8b\x01\n\x0b\x43reateQuery\x12+.kaskada.kaskada.v1alpha.CreateQueryRequest\x1a,.kaskada.kaskada.v1alpha.CreateQueryResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x05query\"\x10/v1alpha/queries0\x01\x12\x86\x01\n\x08GetQuery\x12(.kaskada.kaskada.v1alpha.GetQueryRequest\x1a).kaskada.kaskada.v1alpha.GetQueryResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1alpha/queries/{query_id=*}\x12\x82\x01\n\x0bListQueries\x12+.kaskada.kaskada.v1alpha.ListQueriesRequest\x1a,.kaskada.kaskada.v1alpha.ListQueriesResponse\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/v1alpha/queriesB\x81\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x11QueryServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.query_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\013CommonProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _FILETYPE._serialized_start=2148
-  _FILETYPE._serialized_end=2227
-  _PERENTITYBEHAVIOR._serialized_start=2230
-  _PERENTITYBEHAVIOR._serialized_end=2385
-  _SOURCEDATA._serialized_start=255
-  _SOURCEDATA._serialized_end=468
-  _FILEINPUT._serialized_start=470
-  _FILEINPUT._serialized_end=563
-  _FILERESULTS._serialized_start=565
-  _FILERESULTS._serialized_end=664
-  _TABLECONFIG._serialized_start=667
-  _TABLECONFIG._serialized_end=912
-  _TABLEMETADATA._serialized_start=914
-  _TABLEMETADATA._serialized_end=1017
-  _PREPAREDFILE._serialized_start=1020
-  _PREPAREDFILE._serialized_end=1250
-  _SLICEPLAN._serialized_start=1253
-  _SLICEPLAN._serialized_end=1562
-  _SLICEPLAN_PERCENTSLICE._serialized_start=1461
-  _SLICEPLAN_PERCENTSLICE._serialized_end=1501
-  _SLICEPLAN_ENTITYKEYSSLICE._serialized_start=1503
-  _SLICEPLAN_ENTITYKEYSSLICE._serialized_end=1553
-  _UUID._serialized_start=1564
-  _UUID._serialized_end=1608
-  _SLICEREQUEST._serialized_start=1611
-  _SLICEREQUEST._serialized_end=1898
-  _SLICEREQUEST_PERCENTSLICE._serialized_start=1461
-  _SLICEREQUEST_PERCENTSLICE._serialized_end=1501
-  _SLICEREQUEST_ENTITYKEYSSLICE._serialized_start=1839
-  _SLICEREQUEST_ENTITYKEYSSLICE._serialized_end=1889
-  _ANALYSIS._serialized_start=1901
-  _ANALYSIS._serialized_end=2097
-  _REQUESTDETAILS._serialized_start=2099
-  _REQUESTDETAILS._serialized_end=2146
+  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\021QueryServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
+  _QUERY.fields_by_name['query_id']._options = None
+  _QUERY.fields_by_name['query_id']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['expression']._options = None
+  _QUERY.fields_by_name['expression']._serialized_options = b'\372B\004r\002\020\001'
+  _QUERY.fields_by_name['views']._options = None
+  _QUERY.fields_by_name['views']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['create_time']._options = None
+  _QUERY.fields_by_name['create_time']._serialized_options = b'\340A\003'
+  _GETQUERYREQUEST.fields_by_name['query_id']._options = None
+  _GETQUERYREQUEST.fields_by_name['query_id']._serialized_options = b'\372B\004r\002\020\001'
+  _GETQUERYRESPONSE.fields_by_name['query']._options = None
+  _GETQUERYRESPONSE.fields_by_name['query']._serialized_options = b'\340A\003'
+  _LISTQUERIESREQUEST.fields_by_name['page_size']._options = None
+  _LISTQUERIESREQUEST.fields_by_name['page_size']._serialized_options = b'\372B\007\032\005\030\350\007(\000'
+  _QUERYSERVICE.methods_by_name['CreateQuery']._options = None
+  _QUERYSERVICE.methods_by_name['CreateQuery']._serialized_options = b'\202\323\344\223\002\031:\005query\"\020/v1alpha/queries'
+  _QUERYSERVICE.methods_by_name['GetQuery']._options = None
+  _QUERYSERVICE.methods_by_name['GetQuery']._serialized_options = b'\202\323\344\223\002\037\022\035/v1alpha/queries/{query_id=*}'
+  _QUERYSERVICE.methods_by_name['ListQueries']._options = None
+  _QUERYSERVICE.methods_by_name['ListQueries']._serialized_options = b'\202\323\344\223\002\022\022\020/v1alpha/queries'
+  _globals['_QUERY']._serialized_start=470
+  _globals['_QUERY']._serialized_end=1439
+  _globals['_QUERY_LIMITS']._serialized_start=1172
+  _globals['_QUERY_LIMITS']._serialized_end=1215
+  _globals['_QUERY_REDISBULKRESPONSE']._serialized_start=1217
+  _globals['_QUERY_REDISBULKRESPONSE']._serialized_end=1258
+  _globals['_QUERY_RESULTBEHAVIOR']._serialized_start=1261
+  _globals['_QUERY_RESULTBEHAVIOR']._serialized_end=1421
+  _globals['_QUERYOPTIONS']._serialized_start=1442
+  _globals['_QUERYOPTIONS']._serialized_end=1614
+  _globals['_CREATEQUERYREQUEST']._serialized_start=1617
+  _globals['_CREATEQUERYREQUEST']._serialized_end=1767
+  _globals['_CREATEQUERYRESPONSE']._serialized_start=1770
+  _globals['_CREATEQUERYRESPONSE']._serialized_end=3067
+  _globals['_CREATEQUERYRESPONSE_ANALYSIS']._serialized_start=2373
+  _globals['_CREATEQUERYRESPONSE_ANALYSIS']._serialized_end=2473
+  _globals['_CREATEQUERYRESPONSE_CONFIG']._serialized_start=2475
+  _globals['_CREATEQUERYRESPONSE_CONFIG']._serialized_end=2595
+  _globals['_CREATEQUERYRESPONSE_METRICS']._serialized_start=2598
+  _globals['_CREATEQUERYRESPONSE_METRICS']._serialized_end=2916
+  _globals['_CREATEQUERYRESPONSE_STATE']._serialized_start=2919
+  _globals['_CREATEQUERYRESPONSE_STATE']._serialized_end=3049
+  _globals['_GETQUERYREQUEST']._serialized_start=3069
+  _globals['_GETQUERYREQUEST']._serialized_end=3122
+  _globals['_GETQUERYRESPONSE']._serialized_start=3124
+  _globals['_GETQUERYRESPONSE']._serialized_end=3201
+  _globals['_LISTQUERIESREQUEST']._serialized_start=3203
+  _globals['_LISTQUERIESREQUEST']._serialized_end=3319
+  _globals['_LISTQUERIESRESPONSE']._serialized_start=3322
+  _globals['_LISTQUERIESRESPONSE']._serialized_end=3523
+  _globals['_QUERYSERVICE']._serialized_start=3526
+  _globals['_QUERYSERVICE']._serialized_end=3952
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,202 +1,136 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: kaskada/kaskada/v1alpha/compute_service.proto
+# source: kaskada/kaskada/v2alpha/query_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
 from kaskada.kaskada.v1alpha import destinations_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_destinations__pb2
 from kaskada.kaskada.v1alpha import fenl_diagnostics_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_fenl__diagnostics__pb2
-from kaskada.kaskada.v1alpha import plan_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_plan__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
+from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-kaskada/kaskada/v1alpha/compute_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a*kaskada/kaskada/v1alpha/destinations.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a\"kaskada/kaskada/v1alpha/plan.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"`\n\nFeatureSet\x12<\n\x08\x66ormulas\x18\x01 \x03(\x0b\x32 .kaskada.kaskada.v1alpha.FormulaR\x08\x66ormulas\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\"`\n\x07\x46ormula\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07\x66ormula\x18\x02 \x01(\tR\x07\x66ormula\x12\'\n\x0fsource_location\x18\x03 \x01(\tR\x0esourceLocation\"\xf9\x02\n\x0c\x43omputeTable\x12<\n\x06\x63onfig\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.TableConfigR\x06\x63onfig\x12\x42\n\x08metadata\x18\x02 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\x08metadata\x12J\n\tfile_sets\x18\x03 \x03(\x0b\x32-.kaskada.kaskada.v1alpha.ComputeTable.FileSetR\x08\x66ileSets\x1a\x9a\x01\n\x07\x46ileSet\x12\x41\n\nslice_plan\x18\x01 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\x12L\n\x0eprepared_files\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.PreparedFileR\rpreparedFiles\"\x1e\n\x08PlanHash\x12\x12\n\x04hash\x18\x01 \x01(\x0cR\x04hash\"\"\n GetCurrentSnapshotVersionRequest\"N\n!GetCurrentSnapshotVersionResponse\x12)\n\x10snapshot_version\x18\x01 \x01(\x05R\x0fsnapshotVersion\"\xb0\x04\n\x0e\x43ompileRequest\x12=\n\x06tables\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x44\n\x0b\x66\x65\x61ture_set\x18\x02 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.FeatureSetR\nfeatureSet\x12J\n\rslice_request\x18\x03 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x0csliceRequest\x12_\n\x0f\x65xpression_kind\x18\x04 \x01(\x0e\x32\x36.kaskada.kaskada.v1alpha.CompileRequest.ExpressionKindR\x0e\x65xpressionKind\x12\"\n\x0c\x65xperimental\x18\x05 \x01(\x08R\x0c\x65xperimental\x12Z\n\x13per_entity_behavior\x18\x06 \x01(\x0e\x32*.kaskada.kaskada.v1alpha.PerEntityBehaviorR\x11perEntityBehavior\"l\n\x0e\x45xpressionKind\x12\x1f\n\x1b\x45XPRESSION_KIND_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45XPRESSION_KIND_COMPLETE\x10\x01\x12\x1b\n\x17\x45XPRESSION_KIND_FORMULA\x10\x02\"\xe0\x03\n\x0f\x43ompileResponse\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x38\n\x04plan\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12\x42\n\x0bresult_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\nresultType\x12\x1d\n\nfree_names\x18\x05 \x03(\tR\tfreeNames\x12\x45\n\x0ctable_slices\x18\x06 \x03(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\x0btableSlices\x12/\n\x13incremental_enabled\x18\x07 \x01(\x08R\x12incrementalEnabled\x12>\n\tplan_hash\x18\x08 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\"\xc3\x05\n\x0e\x45xecuteRequest\x12\x38\n\x04plan\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x12\x46\n\x06limits\x18\x05 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ExecuteRequest.LimitsR\x06limits\x12u\n\x17\x63ompute_snapshot_config\x18\x06 \x01(\x0b\x32=.kaskada.kaskada.v1alpha.ExecuteRequest.ComputeSnapshotConfigR\x15\x63omputeSnapshotConfig\x12?\n\rchanged_since\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x63hangedSince\x12\x46\n\x11\x66inal_result_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\x1a+\n\x06Limits\x12!\n\x0cpreview_rows\x18\x01 \x01(\x03R\x0bpreviewRows\x1a{\n\x15\x43omputeSnapshotConfig\x12#\n\routput_prefix\x18\x01 \x01(\tR\x0coutputPrefix\x12=\n\x0bresume_from\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nresumeFrom\"\xd2\x08\n\x0f\x45xecuteResponse\x12=\n\x05state\x18\x01 \x01(\x0e\x32\'.kaskada.kaskada.v1alpha.LongQueryStateR\x05state\x12\"\n\ris_query_done\x18\x02 \x01(\x08R\x0bisQueryDone\x12X\n\x08progress\x18\x03 \x01(\x0b\x32<.kaskada.kaskada.v1alpha.ExecuteResponse.ProgressInformationR\x08progress\x12J\n\x12\x66light_record_path\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x10\x66lightRecordPath\x12\x42\n\x0eplan_yaml_path\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0cplanYamlPath\x12\x65\n\x11\x63ompute_snapshots\x18\x06 \x03(\x0b\x32\x38.kaskada.kaskada.v1alpha.ExecuteResponse.ComputeSnapshotR\x10\x63omputeSnapshots\x12\x46\n\x0b\x64\x65stination\x18\x07 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x1a\xed\x02\n\x13ProgressInformation\x12(\n\x10total_input_rows\x18\x01 \x01(\x03R\x0etotalInputRows\x12\x30\n\x14processed_input_rows\x18\x02 \x01(\x03R\x12processedInputRows\x12#\n\rbuffered_rows\x18\x03 \x01(\x03R\x0c\x62ufferedRows\x12\x36\n\x17processed_buffered_rows\x18\x08 \x01(\x03R\x15processedBufferedRows\x12$\n\x0emin_event_time\x18\x04 \x01(\x03R\x0cminEventTime\x12$\n\x0emax_event_time\x18\x05 \x01(\x03R\x0cmaxEventTime\x12\x1f\n\x0boutput_time\x18\x06 \x01(\x03R\noutputTime\x12\x30\n\x14produced_output_rows\x18\x07 \x01(\x03R\x12producedOutputRows\x1a\xd2\x01\n\x0f\x43omputeSnapshot\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emax_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12>\n\tplan_hash\x18\x03 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\x12)\n\x10snapshot_version\x18\x04 \x01(\x05R\x0fsnapshotVersion*\x8a\x01\n\x0eLongQueryState\x12 \n\x1cLONG_QUERY_STATE_UNSPECIFIED\x10\x00\x12\x1c\n\x18LONG_QUERY_STATE_INITIAL\x10\x01\x12\x1c\n\x18LONG_QUERY_STATE_RUNNING\x10\x02\x12\x1a\n\x16LONG_QUERY_STATE_FINAL\x10\x03\x32\xe3\x02\n\x0e\x43omputeService\x12\\\n\x07\x43ompile\x12\'.kaskada.kaskada.v1alpha.CompileRequest\x1a(.kaskada.kaskada.v1alpha.CompileResponse\x12^\n\x07\x45xecute\x12\'.kaskada.kaskada.v1alpha.ExecuteRequest\x1a(.kaskada.kaskada.v1alpha.ExecuteResponse0\x01\x12\x92\x01\n\x19GetCurrentSnapshotVersion\x12\x39.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionRequest\x1a:.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionResponseB\x83\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x13\x43omputeServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+kaskada/kaskada/v2alpha/query_service.proto\x12\x17kaskada.kaskada.v2alpha\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a*kaskada/kaskada/v1alpha/destinations.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\x1a\x17validate/validate.proto\":\n\x0fLatestDataToken\x12\'\n\rdata_token_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x0b\x64\x61taTokenId\"@\n\x11SpecificDataToken\x12+\n\rdata_token_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61taTokenId\"\xd4\x01\n\tDataToken\x12V\n\x11latest_data_token\x18\x01 \x01(\x0b\x32(.kaskada.kaskada.v2alpha.LatestDataTokenH\x00R\x0flatestDataToken\x12\\\n\x13specific_data_token\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v2alpha.SpecificDataTokenH\x00R\x11specificDataTokenB\x11\n\ndata_token\x12\x03\xf8\x42\x01\"Z\n\tQueryView\x12$\n\tview_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08viewName\x12\'\n\nexpression\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nexpression\"V\n\nAllResults\x12H\n\x12\x63hanged_since_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x63hangedSinceTime\"\xa0\x01\n\x0c\x46inalResults\x12H\n\x12\x63hanged_since_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x63hangedSinceTime\x12\x46\n\x11\x66inal_result_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\"\xa6\x01\n\x12\x46inalResultsAtTime\x12H\n\x12\x63hanged_since_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x63hangedSinceTime\x12\x46\n\x11\x66inal_result_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\"\xa0\x02\n\x0eResultBehavior\x12\x46\n\x0b\x61ll_results\x18\x01 \x01(\x0b\x32#.kaskada.kaskada.v2alpha.AllResultsH\x00R\nallResults\x12L\n\rfinal_results\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v2alpha.FinalResultsH\x00R\x0c\x66inalResults\x12`\n\x15\x66inal_results_at_time\x18\x03 \x01(\x0b\x32+.kaskada.kaskada.v2alpha.FinalResultsAtTimeH\x00R\x12\x66inalResultsAtTimeB\x16\n\x0fresult_behavior\x12\x03\xf8\x42\x01\"0\n\x0bQueryLimits\x12!\n\x0cpreview_rows\x18\x01 \x01(\x03R\x0bpreviewRows\"F\n\nQueryViews\x12\x38\n\x05views\x18\x01 \x03(\x0b\x32\".kaskada.kaskada.v2alpha.QueryViewR\x05views\"\x9a\x03\n\x0bQueryConfig\x12\x41\n\ndata_token\x18\x01 \x01(\x0b\x32\".kaskada.kaskada.v2alpha.DataTokenR\tdataToken\x12;\n\x05slice\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x05slice\x12\x46\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x12P\n\x0fresult_behavior\x18\x04 \x01(\x0b\x32\'.kaskada.kaskada.v2alpha.ResultBehaviorR\x0eresultBehavior\x12<\n\x06limits\x18\x05 \x01(\x0b\x32$.kaskada.kaskada.v2alpha.QueryLimitsR\x06limits\x12\x33\n\x15\x65xperimental_features\x18\x06 \x03(\tR\x14\x65xperimentalFeatures\"\"\n\nCSVResults\x12\x14\n\x05paths\x18\x01 \x03(\tR\x05paths\"&\n\x0eParquetResults\x12\x14\n\x05paths\x18\x01 \x03(\tR\x05paths\"(\n\x10RedisBulkResults\x12\x14\n\x05paths\x18\x01 \x03(\tR\x05paths\"V\n\x0bQueryOutput\x12G\n\x0c\x66ile_results\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.FileResultsR\x0b\x66ileResults\"\xda\x01\n\x0cQueryResults\x12<\n\x06output\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v2alpha.QueryOutputR\x06output\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x37\n\x06schema\x18\x03 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\"\xc3\x02\n\x0cQueryMetrics\x12@\n\x0etime_preparing\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\rtimePreparing\x12@\n\x0etime_computing\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\rtimeComputing\x12!\n\x0coutput_files\x18\x03 \x01(\x03R\x0boutputFiles\x12(\n\x10total_input_rows\x18\x04 \x01(\x03R\x0etotalInputRows\x12\x30\n\x14processed_input_rows\x18\x05 \x01(\x03R\x12processedInputRows\x12\x30\n\x14produced_output_rows\x18\x06 \x01(\x03R\x12producedOutputRows\"\xa3\x04\n\x05Query\x12\x1e\n\x08query_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x07queryId\x12@\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12@\n\x0bupdate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\nupdateTime\x12\'\n\nexpression\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nexpression\x12>\n\x05views\x18\x05 \x01(\x0b\x32#.kaskada.kaskada.v2alpha.QueryViewsB\x03\xe0\x41\x03R\x05views\x12\x41\n\x06\x63onfig\x18\x06 \x01(\x0b\x32$.kaskada.kaskada.v2alpha.QueryConfigB\x03\xe0\x41\x03R\x06\x63onfig\x12>\n\x05state\x18\x07 \x01(\x0e\x32#.kaskada.kaskada.v2alpha.QueryStateB\x03\xe0\x41\x03R\x05state\x12\x44\n\x07results\x18\x08 \x01(\x0b\x32%.kaskada.kaskada.v2alpha.QueryResultsB\x03\xe0\x41\x03R\x07results\x12\x44\n\x07metrics\x18\t \x01(\x0b\x32%.kaskada.kaskada.v2alpha.QueryMetricsB\x03\xe0\x41\x03R\x07metrics\"\xcf\x01\n\x12\x43reateQueryRequest\x12\'\n\nexpression\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nexpression\x12\x39\n\x05views\x18\x02 \x01(\x0b\x32#.kaskada.kaskada.v2alpha.QueryViewsR\x05views\x12<\n\x06\x63onfig\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v2alpha.QueryConfigR\x06\x63onfig\x12\x17\n\x07\x64ry_run\x18\x04 \x01(\x08R\x06\x64ryRun\"\x9d\x01\n\x13\x43reateQueryResponse\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v2alpha.QueryR\x05query\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"8\n\x12\x44\x65leteQueryRequest\x12\"\n\x08query_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x07queryId\"g\n\x13\x44\x65leteQueryResponse\x12P\n\x0frequest_details\x18\x01 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"^\n\x0fGetQueryRequest\x12\"\n\x08query_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x07queryId\x12\'\n\x0fpresign_results\x18\x02 \x01(\x08R\x0epresignResults\"\x9a\x01\n\x10GetQueryResponse\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v2alpha.QueryR\x05query\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"t\n\x12ListQueriesRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\'\n\tpage_size\x18\x02 \x01(\x05\x42\n\xfa\x42\x07\x1a\x05\x18\xe8\x07(\x00R\x08pageSize\x12\x1d\n\npage_token\x18\x03 \x01(\tR\tpageToken\"\xc9\x01\n\x13ListQueriesResponse\x12\x38\n\x07queries\x18\x01 \x03(\x0b\x32\x1e.kaskada.kaskada.v2alpha.QueryR\x07queries\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\x12P\n\x0frequest_details\x18\x03 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails*\xc5\x01\n\nQueryState\x12\x1b\n\x17QUERY_STATE_UNSPECIFIED\x10\x00\x12\x18\n\x14QUERY_STATE_COMPILED\x10\x01\x12\x19\n\x15QUERY_STATE_PREPARING\x10\x02\x12\x18\n\x14QUERY_STATE_PREPARED\x10\x03\x12\x19\n\x15QUERY_STATE_COMPUTING\x10\x04\x12\x17\n\x13QUERY_STATE_SUCCESS\x10\x05\x12\x17\n\x13QUERY_STATE_FAILURE\x10\x06\x32\xae\x04\n\x0cQueryService\x12\x83\x01\n\x0b\x43reateQuery\x12+.kaskada.kaskada.v2alpha.CreateQueryRequest\x1a,.kaskada.kaskada.v2alpha.CreateQueryResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/v2alpha/query\x12\x8d\x01\n\x0b\x44\x65leteQuery\x12+.kaskada.kaskada.v2alpha.DeleteQueryRequest\x1a,.kaskada.kaskada.v2alpha.DeleteQueryResponse\"#\x82\xd3\xe4\x93\x02\x1d*\x1b/v2alpha/query/{query_id=*}\x12\x84\x01\n\x08GetQuery\x12(.kaskada.kaskada.v2alpha.GetQueryRequest\x1a).kaskada.kaskada.v2alpha.GetQueryResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v2alpha/query/{query_id=*}\x12\x80\x01\n\x0bListQueries\x12+.kaskada.kaskada.v2alpha.ListQueriesRequest\x1a,.kaskada.kaskada.v2alpha.ListQueriesResponse\"\x16\x82\xd3\xe4\x93\x02\x10\x12\x0e/v2alpha/queryB\x81\x02\n\x1b\x63om.kaskada.kaskada.v2alphaB\x11QueryServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v2alpha;kaskadav2alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V2alpha\xca\x02\x17Kaskada\\Kaskada\\V2alpha\xe2\x02#Kaskada\\Kaskada\\V2alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V2alphab\x06proto3')
 
-_LONGQUERYSTATE = DESCRIPTOR.enum_types_by_name['LongQueryState']
-LongQueryState = enum_type_wrapper.EnumTypeWrapper(_LONGQUERYSTATE)
-LONG_QUERY_STATE_UNSPECIFIED = 0
-LONG_QUERY_STATE_INITIAL = 1
-LONG_QUERY_STATE_RUNNING = 2
-LONG_QUERY_STATE_FINAL = 3
-
-
-_FEATURESET = DESCRIPTOR.message_types_by_name['FeatureSet']
-_FORMULA = DESCRIPTOR.message_types_by_name['Formula']
-_COMPUTETABLE = DESCRIPTOR.message_types_by_name['ComputeTable']
-_COMPUTETABLE_FILESET = _COMPUTETABLE.nested_types_by_name['FileSet']
-_PLANHASH = DESCRIPTOR.message_types_by_name['PlanHash']
-_GETCURRENTSNAPSHOTVERSIONREQUEST = DESCRIPTOR.message_types_by_name['GetCurrentSnapshotVersionRequest']
-_GETCURRENTSNAPSHOTVERSIONRESPONSE = DESCRIPTOR.message_types_by_name['GetCurrentSnapshotVersionResponse']
-_COMPILEREQUEST = DESCRIPTOR.message_types_by_name['CompileRequest']
-_COMPILERESPONSE = DESCRIPTOR.message_types_by_name['CompileResponse']
-_EXECUTEREQUEST = DESCRIPTOR.message_types_by_name['ExecuteRequest']
-_EXECUTEREQUEST_LIMITS = _EXECUTEREQUEST.nested_types_by_name['Limits']
-_EXECUTEREQUEST_COMPUTESNAPSHOTCONFIG = _EXECUTEREQUEST.nested_types_by_name['ComputeSnapshotConfig']
-_EXECUTERESPONSE = DESCRIPTOR.message_types_by_name['ExecuteResponse']
-_EXECUTERESPONSE_PROGRESSINFORMATION = _EXECUTERESPONSE.nested_types_by_name['ProgressInformation']
-_EXECUTERESPONSE_COMPUTESNAPSHOT = _EXECUTERESPONSE.nested_types_by_name['ComputeSnapshot']
-_COMPILEREQUEST_EXPRESSIONKIND = _COMPILEREQUEST.enum_types_by_name['ExpressionKind']
-FeatureSet = _reflection.GeneratedProtocolMessageType('FeatureSet', (_message.Message,), {
-  'DESCRIPTOR' : _FEATURESET,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.FeatureSet)
-  })
-_sym_db.RegisterMessage(FeatureSet)
-
-Formula = _reflection.GeneratedProtocolMessageType('Formula', (_message.Message,), {
-  'DESCRIPTOR' : _FORMULA,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.Formula)
-  })
-_sym_db.RegisterMessage(Formula)
-
-ComputeTable = _reflection.GeneratedProtocolMessageType('ComputeTable', (_message.Message,), {
-
-  'FileSet' : _reflection.GeneratedProtocolMessageType('FileSet', (_message.Message,), {
-    'DESCRIPTOR' : _COMPUTETABLE_FILESET,
-    '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ComputeTable.FileSet)
-    })
-  ,
-  'DESCRIPTOR' : _COMPUTETABLE,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ComputeTable)
-  })
-_sym_db.RegisterMessage(ComputeTable)
-_sym_db.RegisterMessage(ComputeTable.FileSet)
-
-PlanHash = _reflection.GeneratedProtocolMessageType('PlanHash', (_message.Message,), {
-  'DESCRIPTOR' : _PLANHASH,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.PlanHash)
-  })
-_sym_db.RegisterMessage(PlanHash)
-
-GetCurrentSnapshotVersionRequest = _reflection.GeneratedProtocolMessageType('GetCurrentSnapshotVersionRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCURRENTSNAPSHOTVERSIONREQUEST,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionRequest)
-  })
-_sym_db.RegisterMessage(GetCurrentSnapshotVersionRequest)
-
-GetCurrentSnapshotVersionResponse = _reflection.GeneratedProtocolMessageType('GetCurrentSnapshotVersionResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCURRENTSNAPSHOTVERSIONRESPONSE,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionResponse)
-  })
-_sym_db.RegisterMessage(GetCurrentSnapshotVersionResponse)
-
-CompileRequest = _reflection.GeneratedProtocolMessageType('CompileRequest', (_message.Message,), {
-  'DESCRIPTOR' : _COMPILEREQUEST,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.CompileRequest)
-  })
-_sym_db.RegisterMessage(CompileRequest)
-
-CompileResponse = _reflection.GeneratedProtocolMessageType('CompileResponse', (_message.Message,), {
-  'DESCRIPTOR' : _COMPILERESPONSE,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.CompileResponse)
-  })
-_sym_db.RegisterMessage(CompileResponse)
-
-ExecuteRequest = _reflection.GeneratedProtocolMessageType('ExecuteRequest', (_message.Message,), {
-
-  'Limits' : _reflection.GeneratedProtocolMessageType('Limits', (_message.Message,), {
-    'DESCRIPTOR' : _EXECUTEREQUEST_LIMITS,
-    '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ExecuteRequest.Limits)
-    })
-  ,
-
-  'ComputeSnapshotConfig' : _reflection.GeneratedProtocolMessageType('ComputeSnapshotConfig', (_message.Message,), {
-    'DESCRIPTOR' : _EXECUTEREQUEST_COMPUTESNAPSHOTCONFIG,
-    '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ExecuteRequest.ComputeSnapshotConfig)
-    })
-  ,
-  'DESCRIPTOR' : _EXECUTEREQUEST,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ExecuteRequest)
-  })
-_sym_db.RegisterMessage(ExecuteRequest)
-_sym_db.RegisterMessage(ExecuteRequest.Limits)
-_sym_db.RegisterMessage(ExecuteRequest.ComputeSnapshotConfig)
-
-ExecuteResponse = _reflection.GeneratedProtocolMessageType('ExecuteResponse', (_message.Message,), {
-
-  'ProgressInformation' : _reflection.GeneratedProtocolMessageType('ProgressInformation', (_message.Message,), {
-    'DESCRIPTOR' : _EXECUTERESPONSE_PROGRESSINFORMATION,
-    '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ExecuteResponse.ProgressInformation)
-    })
-  ,
-
-  'ComputeSnapshot' : _reflection.GeneratedProtocolMessageType('ComputeSnapshot', (_message.Message,), {
-    'DESCRIPTOR' : _EXECUTERESPONSE_COMPUTESNAPSHOT,
-    '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ExecuteResponse.ComputeSnapshot)
-    })
-  ,
-  'DESCRIPTOR' : _EXECUTERESPONSE,
-  '__module__' : 'kaskada.kaskada.v1alpha.compute_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.ExecuteResponse)
-  })
-_sym_db.RegisterMessage(ExecuteResponse)
-_sym_db.RegisterMessage(ExecuteResponse.ProgressInformation)
-_sym_db.RegisterMessage(ExecuteResponse.ComputeSnapshot)
-
-_COMPUTESERVICE = DESCRIPTOR.services_by_name['ComputeService']
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v2alpha.query_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\023ComputeServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _LONGQUERYSTATE._serialized_start=3933
-  _LONGQUERYSTATE._serialized_end=4071
-  _FEATURESET._serialized_start=343
-  _FEATURESET._serialized_end=439
-  _FORMULA._serialized_start=441
-  _FORMULA._serialized_end=537
-  _COMPUTETABLE._serialized_start=540
-  _COMPUTETABLE._serialized_end=917
-  _COMPUTETABLE_FILESET._serialized_start=763
-  _COMPUTETABLE_FILESET._serialized_end=917
-  _PLANHASH._serialized_start=919
-  _PLANHASH._serialized_end=949
-  _GETCURRENTSNAPSHOTVERSIONREQUEST._serialized_start=951
-  _GETCURRENTSNAPSHOTVERSIONREQUEST._serialized_end=985
-  _GETCURRENTSNAPSHOTVERSIONRESPONSE._serialized_start=987
-  _GETCURRENTSNAPSHOTVERSIONRESPONSE._serialized_end=1065
-  _COMPILEREQUEST._serialized_start=1068
-  _COMPILEREQUEST._serialized_end=1628
-  _COMPILEREQUEST_EXPRESSIONKIND._serialized_start=1520
-  _COMPILEREQUEST_EXPRESSIONKIND._serialized_end=1628
-  _COMPILERESPONSE._serialized_start=1631
-  _COMPILERESPONSE._serialized_end=2111
-  _EXECUTEREQUEST._serialized_start=2114
-  _EXECUTEREQUEST._serialized_end=2821
-  _EXECUTEREQUEST_LIMITS._serialized_start=2653
-  _EXECUTEREQUEST_LIMITS._serialized_end=2696
-  _EXECUTEREQUEST_COMPUTESNAPSHOTCONFIG._serialized_start=2698
-  _EXECUTEREQUEST_COMPUTESNAPSHOTCONFIG._serialized_end=2821
-  _EXECUTERESPONSE._serialized_start=2824
-  _EXECUTERESPONSE._serialized_end=3930
-  _EXECUTERESPONSE_PROGRESSINFORMATION._serialized_start=3352
-  _EXECUTERESPONSE_PROGRESSINFORMATION._serialized_end=3717
-  _EXECUTERESPONSE_COMPUTESNAPSHOT._serialized_start=3720
-  _EXECUTERESPONSE_COMPUTESNAPSHOT._serialized_end=3930
-  _COMPUTESERVICE._serialized_start=4074
-  _COMPUTESERVICE._serialized_end=4429
+  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v2alphaB\021QueryServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v2alpha;kaskadav2alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V2alpha\312\002\027Kaskada\\Kaskada\\V2alpha\342\002#Kaskada\\Kaskada\\V2alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V2alpha'
+  _LATESTDATATOKEN.fields_by_name['data_token_id']._options = None
+  _LATESTDATATOKEN.fields_by_name['data_token_id']._serialized_options = b'\340A\003'
+  _SPECIFICDATATOKEN.fields_by_name['data_token_id']._options = None
+  _SPECIFICDATATOKEN.fields_by_name['data_token_id']._serialized_options = b'\372B\004r\002\020\001'
+  _DATATOKEN.oneofs_by_name['data_token']._options = None
+  _DATATOKEN.oneofs_by_name['data_token']._serialized_options = b'\370B\001'
+  _QUERYVIEW.fields_by_name['view_name']._options = None
+  _QUERYVIEW.fields_by_name['view_name']._serialized_options = b'\372B\004r\002\020\001'
+  _QUERYVIEW.fields_by_name['expression']._options = None
+  _QUERYVIEW.fields_by_name['expression']._serialized_options = b'\372B\004r\002\020\001'
+  _RESULTBEHAVIOR.oneofs_by_name['result_behavior']._options = None
+  _RESULTBEHAVIOR.oneofs_by_name['result_behavior']._serialized_options = b'\370B\001'
+  _QUERY.fields_by_name['query_id']._options = None
+  _QUERY.fields_by_name['query_id']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['create_time']._options = None
+  _QUERY.fields_by_name['create_time']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['update_time']._options = None
+  _QUERY.fields_by_name['update_time']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['expression']._options = None
+  _QUERY.fields_by_name['expression']._serialized_options = b'\372B\004r\002\020\001'
+  _QUERY.fields_by_name['views']._options = None
+  _QUERY.fields_by_name['views']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['config']._options = None
+  _QUERY.fields_by_name['config']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['state']._options = None
+  _QUERY.fields_by_name['state']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['results']._options = None
+  _QUERY.fields_by_name['results']._serialized_options = b'\340A\003'
+  _QUERY.fields_by_name['metrics']._options = None
+  _QUERY.fields_by_name['metrics']._serialized_options = b'\340A\003'
+  _CREATEQUERYREQUEST.fields_by_name['expression']._options = None
+  _CREATEQUERYREQUEST.fields_by_name['expression']._serialized_options = b'\372B\004r\002\020\001'
+  _DELETEQUERYREQUEST.fields_by_name['query_id']._options = None
+  _DELETEQUERYREQUEST.fields_by_name['query_id']._serialized_options = b'\372B\004r\002\020\001'
+  _GETQUERYREQUEST.fields_by_name['query_id']._options = None
+  _GETQUERYREQUEST.fields_by_name['query_id']._serialized_options = b'\372B\004r\002\020\001'
+  _LISTQUERIESREQUEST.fields_by_name['page_size']._options = None
+  _LISTQUERIESREQUEST.fields_by_name['page_size']._serialized_options = b'\372B\007\032\005\030\350\007(\000'
+  _QUERYSERVICE.methods_by_name['CreateQuery']._options = None
+  _QUERYSERVICE.methods_by_name['CreateQuery']._serialized_options = b'\202\323\344\223\002\023:\001*\"\016/v2alpha/query'
+  _QUERYSERVICE.methods_by_name['DeleteQuery']._options = None
+  _QUERYSERVICE.methods_by_name['DeleteQuery']._serialized_options = b'\202\323\344\223\002\035*\033/v2alpha/query/{query_id=*}'
+  _QUERYSERVICE.methods_by_name['GetQuery']._options = None
+  _QUERYSERVICE.methods_by_name['GetQuery']._serialized_options = b'\202\323\344\223\002\035\022\033/v2alpha/query/{query_id=*}'
+  _QUERYSERVICE.methods_by_name['ListQueries']._options = None
+  _QUERYSERVICE.methods_by_name['ListQueries']._serialized_options = b'\202\323\344\223\002\020\022\016/v2alpha/query'
+  _globals['_QUERYSTATE']._serialized_start=4484
+  _globals['_QUERYSTATE']._serialized_end=4681
+  _globals['_LATESTDATATOKEN']._serialized_start=393
+  _globals['_LATESTDATATOKEN']._serialized_end=451
+  _globals['_SPECIFICDATATOKEN']._serialized_start=453
+  _globals['_SPECIFICDATATOKEN']._serialized_end=517
+  _globals['_DATATOKEN']._serialized_start=520
+  _globals['_DATATOKEN']._serialized_end=732
+  _globals['_QUERYVIEW']._serialized_start=734
+  _globals['_QUERYVIEW']._serialized_end=824
+  _globals['_ALLRESULTS']._serialized_start=826
+  _globals['_ALLRESULTS']._serialized_end=912
+  _globals['_FINALRESULTS']._serialized_start=915
+  _globals['_FINALRESULTS']._serialized_end=1075
+  _globals['_FINALRESULTSATTIME']._serialized_start=1078
+  _globals['_FINALRESULTSATTIME']._serialized_end=1244
+  _globals['_RESULTBEHAVIOR']._serialized_start=1247
+  _globals['_RESULTBEHAVIOR']._serialized_end=1535
+  _globals['_QUERYLIMITS']._serialized_start=1537
+  _globals['_QUERYLIMITS']._serialized_end=1585
+  _globals['_QUERYVIEWS']._serialized_start=1587
+  _globals['_QUERYVIEWS']._serialized_end=1657
+  _globals['_QUERYCONFIG']._serialized_start=1660
+  _globals['_QUERYCONFIG']._serialized_end=2070
+  _globals['_CSVRESULTS']._serialized_start=2072
+  _globals['_CSVRESULTS']._serialized_end=2106
+  _globals['_PARQUETRESULTS']._serialized_start=2108
+  _globals['_PARQUETRESULTS']._serialized_end=2146
+  _globals['_REDISBULKRESULTS']._serialized_start=2148
+  _globals['_REDISBULKRESULTS']._serialized_end=2188
+  _globals['_QUERYOUTPUT']._serialized_start=2190
+  _globals['_QUERYOUTPUT']._serialized_end=2276
+  _globals['_QUERYRESULTS']._serialized_start=2279
+  _globals['_QUERYRESULTS']._serialized_end=2497
+  _globals['_QUERYMETRICS']._serialized_start=2500
+  _globals['_QUERYMETRICS']._serialized_end=2823
+  _globals['_QUERY']._serialized_start=2826
+  _globals['_QUERY']._serialized_end=3373
+  _globals['_CREATEQUERYREQUEST']._serialized_start=3376
+  _globals['_CREATEQUERYREQUEST']._serialized_end=3583
+  _globals['_CREATEQUERYRESPONSE']._serialized_start=3586
+  _globals['_CREATEQUERYRESPONSE']._serialized_end=3743
+  _globals['_DELETEQUERYREQUEST']._serialized_start=3745
+  _globals['_DELETEQUERYREQUEST']._serialized_end=3801
+  _globals['_DELETEQUERYRESPONSE']._serialized_start=3803
+  _globals['_DELETEQUERYRESPONSE']._serialized_end=3906
+  _globals['_GETQUERYREQUEST']._serialized_start=3908
+  _globals['_GETQUERYREQUEST']._serialized_end=4002
+  _globals['_GETQUERYRESPONSE']._serialized_start=4005
+  _globals['_GETQUERYRESPONSE']._serialized_end=4159
+  _globals['_LISTQUERIESREQUEST']._serialized_start=4161
+  _globals['_LISTQUERIESREQUEST']._serialized_end=4277
+  _globals['_LISTQUERIESRESPONSE']._serialized_start=4280
+  _globals['_LISTQUERIESRESPONSE']._serialized_end=4481
+  _globals['_QUERYSERVICE']._serialized_start=4684
+  _globals['_QUERYSERVICE']._serialized_end=5242
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,49 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: kaskada/kaskada/v1alpha/data_token_service.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0kaskada/kaskada/v1alpha/data_token_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$kaskada/kaskada/v1alpha/common.proto\"\x9b\x02\n\tDataToken\x12\'\n\rdata_token_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x0b\x64\x61taTokenId\x12\x61\n\x0etable_versions\x18\x02 \x03(\x0b\x32\x35.kaskada.kaskada.v1alpha.DataToken.TableVersionsEntryB\x03\xe0\x41\x03R\rtableVersions\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x1a@\n\x12TableVersionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x03R\x05value:\x02\x38\x01\"9\n\x13GetDataTokenRequest\x12\"\n\rdata_token_id\x18\x01 \x01(\tR\x0b\x64\x61taTokenId\"\xab\x01\n\x14GetDataTokenResponse\x12\x41\n\ndata_token\x18\x01 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.DataTokenR\tdataToken\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails2\xb0\x01\n\x10\x44\x61taTokenService\x12\x9b\x01\n\x0cGetDataToken\x12,.kaskada.kaskada.v1alpha.GetDataTokenRequest\x1a-.kaskada.kaskada.v1alpha.GetDataTokenResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1alpha/data_tokens/{data_token_id=*}B\x85\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x15\x44\x61taTokenServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
-
-
-_DATATOKEN = DESCRIPTOR.message_types_by_name['DataToken']
-_DATATOKEN_TABLEVERSIONSENTRY = _DATATOKEN.nested_types_by_name['TableVersionsEntry']
-_GETDATATOKENREQUEST = DESCRIPTOR.message_types_by_name['GetDataTokenRequest']
-_GETDATATOKENRESPONSE = DESCRIPTOR.message_types_by_name['GetDataTokenResponse']
-DataToken = _reflection.GeneratedProtocolMessageType('DataToken', (_message.Message,), {
-
-  'TableVersionsEntry' : _reflection.GeneratedProtocolMessageType('TableVersionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _DATATOKEN_TABLEVERSIONSENTRY,
-    '__module__' : 'kaskada.kaskada.v1alpha.data_token_service_pb2'
-    # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.DataToken.TableVersionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _DATATOKEN,
-  '__module__' : 'kaskada.kaskada.v1alpha.data_token_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.DataToken)
-  })
-_sym_db.RegisterMessage(DataToken)
-_sym_db.RegisterMessage(DataToken.TableVersionsEntry)
-
-GetDataTokenRequest = _reflection.GeneratedProtocolMessageType('GetDataTokenRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETDATATOKENREQUEST,
-  '__module__' : 'kaskada.kaskada.v1alpha.data_token_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.GetDataTokenRequest)
-  })
-_sym_db.RegisterMessage(GetDataTokenRequest)
-
-GetDataTokenResponse = _reflection.GeneratedProtocolMessageType('GetDataTokenResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETDATATOKENRESPONSE,
-  '__module__' : 'kaskada.kaskada.v1alpha.data_token_service_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.GetDataTokenResponse)
-  })
-_sym_db.RegisterMessage(GetDataTokenResponse)
-
-_DATATOKENSERVICE = DESCRIPTOR.services_by_name['DataTokenService']
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.data_token_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\025DataTokenServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
   _DATATOKEN_TABLEVERSIONSENTRY._options = None
   _DATATOKEN_TABLEVERSIONSENTRY._serialized_options = b'8\001'
   _DATATOKEN.fields_by_name['data_token_id']._options = None
   _DATATOKEN.fields_by_name['data_token_id']._serialized_options = b'\340A\003'
   _DATATOKEN.fields_by_name['table_versions']._options = None
   _DATATOKEN.fields_by_name['table_versions']._serialized_options = b'\340A\003'
   _DATATOKEN.fields_by_name['create_time']._options = None
   _DATATOKEN.fields_by_name['create_time']._serialized_options = b'\340A\003'
   _DATATOKENSERVICE.methods_by_name['GetDataToken']._options = None
   _DATATOKENSERVICE.methods_by_name['GetDataToken']._serialized_options = b'\202\323\344\223\002(\022&/v1alpha/data_tokens/{data_token_id=*}'
-  _DATATOKEN._serialized_start=212
-  _DATATOKEN._serialized_end=495
-  _DATATOKEN_TABLEVERSIONSENTRY._serialized_start=431
-  _DATATOKEN_TABLEVERSIONSENTRY._serialized_end=495
-  _GETDATATOKENREQUEST._serialized_start=497
-  _GETDATATOKENREQUEST._serialized_end=554
-  _GETDATATOKENRESPONSE._serialized_start=557
-  _GETDATATOKENRESPONSE._serialized_end=728
-  _DATATOKENSERVICE._serialized_start=731
-  _DATATOKENSERVICE._serialized_end=907
+  _globals['_DATATOKEN']._serialized_start=212
+  _globals['_DATATOKEN']._serialized_end=495
+  _globals['_DATATOKEN_TABLEVERSIONSENTRY']._serialized_start=431
+  _globals['_DATATOKEN_TABLEVERSIONSENTRY']._serialized_end=495
+  _globals['_GETDATATOKENREQUEST']._serialized_start=497
+  _globals['_GETDATATOKENREQUEST']._serialized_end=554
+  _globals['_GETDATATOKENRESPONSE']._serialized_start=557
+  _globals['_GETDATATOKENRESPONSE']._serialized_end=728
+  _globals['_DATATOKENSERVICE']._serialized_start=731
+  _globals['_DATATOKENSERVICE']._serialized_end=907
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: kaskada/kaskada/v1alpha/fenl_diagnostics.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x12\x17kaskada.kaskada.v1alpha\"\x84\x01\n\x0f\x46\x65nlDiagnostics\x12R\n\x10\x66\x65nl_diagnostics\x18\x01 \x03(\x0b\x32\'.kaskada.kaskada.v1alpha.FenlDiagnosticR\x0f\x66\x65nlDiagnostics\x12\x1d\n\nnum_errors\x18\x02 \x01(\x03R\tnumErrors\"\x9b\x01\n\x0e\x46\x65nlDiagnostic\x12=\n\x08severity\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.SeverityR\x08severity\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12\x1c\n\tformatted\x18\x04 \x01(\tR\tformatted*\x86\x01\n\x08Severity\x12\x18\n\x14SEVERITY_UNSPECIFIED\x10\x00\x12\x10\n\x0cSEVERITY_BUG\x10\x01\x12\x12\n\x0eSEVERITY_ERROR\x10\x02\x12\x14\n\x10SEVERITY_WARNING\x10\x03\x12\x11\n\rSEVERITY_NOTE\x10\x04\x12\x11\n\rSEVERITY_HELP\x10\x05\x42\x84\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x14\x46\x65nlDiagnosticsProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
-_SEVERITY = DESCRIPTOR.enum_types_by_name['Severity']
-Severity = enum_type_wrapper.EnumTypeWrapper(_SEVERITY)
-SEVERITY_UNSPECIFIED = 0
-SEVERITY_BUG = 1
-SEVERITY_ERROR = 2
-SEVERITY_WARNING = 3
-SEVERITY_NOTE = 4
-SEVERITY_HELP = 5
-
-
-_FENLDIAGNOSTICS = DESCRIPTOR.message_types_by_name['FenlDiagnostics']
-_FENLDIAGNOSTIC = DESCRIPTOR.message_types_by_name['FenlDiagnostic']
-FenlDiagnostics = _reflection.GeneratedProtocolMessageType('FenlDiagnostics', (_message.Message,), {
-  'DESCRIPTOR' : _FENLDIAGNOSTICS,
-  '__module__' : 'kaskada.kaskada.v1alpha.fenl_diagnostics_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.FenlDiagnostics)
-  })
-_sym_db.RegisterMessage(FenlDiagnostics)
-
-FenlDiagnostic = _reflection.GeneratedProtocolMessageType('FenlDiagnostic', (_message.Message,), {
-  'DESCRIPTOR' : _FENLDIAGNOSTIC,
-  '__module__' : 'kaskada.kaskada.v1alpha.fenl_diagnostics_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.FenlDiagnostic)
-  })
-_sym_db.RegisterMessage(FenlDiagnostic)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.fenl_diagnostics_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\024FenlDiagnosticsProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _SEVERITY._serialized_start=369
-  _SEVERITY._serialized_end=503
-  _FENLDIAGNOSTICS._serialized_start=76
-  _FENLDIAGNOSTICS._serialized_end=208
-  _FENLDIAGNOSTIC._serialized_start=211
-  _FENLDIAGNOSTIC._serialized_end=366
+  _globals['_SEVERITY']._serialized_start=369
+  _globals['_SEVERITY']._serialized_end=503
+  _globals['_FENLDIAGNOSTICS']._serialized_start=76
+  _globals['_FENLDIAGNOSTICS']._serialized_end=208
+  _globals['_FENLDIAGNOSTIC']._serialized_start=211
+  _globals['_FENLDIAGNOSTIC']._serialized_end=366
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: kaskada/kaskada/v1alpha/options.proto
+# source: kaskada/kaskada/v1alpha/sources.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
+from kaskada.kaskada.v1alpha import pulsar_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_pulsar__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kaskada/kaskada/v1alpha/options.proto\x12\x17kaskada.kaskada.v1alpha\x1a google/protobuf/descriptor.proto:=\n\tsensitive\x12\x1d.google.protobuf.FieldOptions\x18\xd0\x86\x03 \x01(\x08R\tsensitiveB\xfc\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0cOptionsProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
-
-
-SENSITIVE_FIELD_NUMBER = 50000
-sensitive = DESCRIPTOR.extensions_by_name['sensitive']
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kaskada/kaskada/v1alpha/sources.proto\x12\x17kaskada.kaskada.v1alpha\x1a$kaskada/kaskada/v1alpha/pulsar.proto\"\x97\x01\n\x06Source\x12\x42\n\x07kaskada\x18\x01 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.KaskadaSourceH\x00R\x07kaskada\x12?\n\x06pulsar\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarSourceH\x00R\x06pulsarB\x08\n\x06source\"\x0f\n\rKaskadaSource\"M\n\x0cPulsarSource\x12=\n\x06\x63onfig\x18\x01 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarConfigR\x06\x63onfigB\xfc\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0cSourcesProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.sources_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(sensitive)
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\014OptionsProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
+  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\014SourcesProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
+  _globals['_SOURCE']._serialized_start=105
+  _globals['_SOURCE']._serialized_end=256
+  _globals['_KASKADASOURCE']._serialized_start=258
+  _globals['_KASKADASOURCE']._serialized_end=273
+  _globals['_PULSARSOURCE']._serialized_start=275
+  _globals['_PULSARSOURCE']._serialized_end=352
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: kaskada/kaskada/v1alpha/pulsar.proto
+# source: kaskada/kaskada/v1alpha/preparation_service.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from kaskada.kaskada.v1alpha import options_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_options__pb2
+from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/pulsar.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a%kaskada/kaskada/v1alpha/options.proto\"\x85\x02\n\x0cPulsarConfig\x12,\n\x12\x62roker_service_url\x18\x01 \x01(\tR\x10\x62rokerServiceUrl\x12*\n\x11\x61\x64min_service_url\x18\x02 \x01(\tR\x0f\x61\x64minServiceUrl\x12\x1f\n\x0b\x61uth_plugin\x18\x03 \x01(\tR\nauthPlugin\x12%\n\x0b\x61uth_params\x18\x04 \x01(\tB\x04\x80\xb5\x18\x01R\nauthParams\x12\x16\n\x06tenant\x18\x05 \x01(\tR\x06tenant\x12\x1c\n\tnamespace\x18\x06 \x01(\tR\tnamespace\x12\x1d\n\ntopic_name\x18\x07 \x01(\tR\ttopicName\"\xc4\x01\n\x12PulsarSubscription\x12=\n\x06\x63onfig\x18\x01 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarConfigR\x06\x63onfig\x12\'\n\x0fsubscription_id\x18\x02 \x01(\tR\x0esubscriptionId\x12\x46\n\x11last_publish_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0flastPublishTimeB\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0bPulsarProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
-
-
-
-_PULSARCONFIG = DESCRIPTOR.message_types_by_name['PulsarConfig']
-_PULSARSUBSCRIPTION = DESCRIPTOR.message_types_by_name['PulsarSubscription']
-PulsarConfig = _reflection.GeneratedProtocolMessageType('PulsarConfig', (_message.Message,), {
-  'DESCRIPTOR' : _PULSARCONFIG,
-  '__module__' : 'kaskada.kaskada.v1alpha.pulsar_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.PulsarConfig)
-  })
-_sym_db.RegisterMessage(PulsarConfig)
-
-PulsarSubscription = _reflection.GeneratedProtocolMessageType('PulsarSubscription', (_message.Message,), {
-  'DESCRIPTOR' : _PULSARSUBSCRIPTION,
-  '__module__' : 'kaskada.kaskada.v1alpha.pulsar_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.PulsarSubscription)
-  })
-_sym_db.RegisterMessage(PulsarSubscription)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n1kaskada/kaskada/v1alpha/preparation_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a$kaskada/kaskada/v1alpha/common.proto\"\xaa\x02\n\x12PrepareDataRequest\x12\x44\n\x0bsource_data\x18\x01 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.SourceDataR\nsourceData\x12<\n\x06\x63onfig\x18\x02 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.TableConfigR\x06\x63onfig\x12,\n\x12output_path_prefix\x18\x03 \x01(\tR\x10outputPathPrefix\x12\x1f\n\x0b\x66ile_prefix\x18\x04 \x01(\tR\nfilePrefix\x12\x41\n\nslice_plan\x18\x05 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\"|\n\x13PrepareDataResponse\x12\x17\n\x07prep_id\x18\x01 \x01(\x05R\x06prepId\x12L\n\x0eprepared_files\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.PreparedFileR\rpreparedFiles\"\x19\n\x17GetCurrentPrepIDRequest\"3\n\x18GetCurrentPrepIDResponse\x12\x17\n\x07prep_id\x18\x01 \x01(\x05R\x06prepId2\xf7\x01\n\x12PreparationService\x12h\n\x0bPrepareData\x12+.kaskada.kaskada.v1alpha.PrepareDataRequest\x1a,.kaskada.kaskada.v1alpha.PrepareDataResponse\x12w\n\x10GetCurrentPrepID\x12\x30.kaskada.kaskada.v1alpha.GetCurrentPrepIDRequest\x1a\x31.kaskada.kaskada.v1alpha.GetCurrentPrepIDResponseB\x87\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x17PreparationServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.preparation_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\013PulsarProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _PULSARCONFIG.fields_by_name['auth_params']._options = None
-  _PULSARCONFIG.fields_by_name['auth_params']._serialized_options = b'\200\265\030\001'
-  _PULSARCONFIG._serialized_start=138
-  _PULSARCONFIG._serialized_end=399
-  _PULSARSUBSCRIPTION._serialized_start=402
-  _PULSARSUBSCRIPTION._serialized_end=598
+  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\027PreparationServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
+  _globals['_PREPAREDATAREQUEST']._serialized_start=117
+  _globals['_PREPAREDATAREQUEST']._serialized_end=415
+  _globals['_PREPAREDATARESPONSE']._serialized_start=417
+  _globals['_PREPAREDATARESPONSE']._serialized_end=541
+  _globals['_GETCURRENTPREPIDREQUEST']._serialized_start=543
+  _globals['_GETCURRENTPREPIDREQUEST']._serialized_end=568
+  _globals['_GETCURRENTPREPIDRESPONSE']._serialized_start=570
+  _globals['_GETCURRENTPREPIDRESPONSE']._serialized_end=621
+  _globals['_PREPARATIONSERVICE']._serialized_start=624
+  _globals['_PREPARATIONSERVICE']._serialized_end=871
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/spec_pb2.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: kaskada/kaskada/v1alpha/spec.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from kaskada.kaskada.v1alpha import materialization_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_materialization__service__pb2
 from kaskada.kaskada.v1alpha import query_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2
 from kaskada.kaskada.v1alpha import table_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_table__service__pb2
 from kaskada.kaskada.v1alpha import view_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_view__service__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"kaskada/kaskada/v1alpha/spec.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x35kaskada/kaskada/v1alpha/materialization_service.proto\x1a+kaskada/kaskada/v1alpha/query_service.proto\x1a+kaskada/kaskada/v1alpha/table_service.proto\x1a*kaskada/kaskada/v1alpha/view_service.proto\"\x83\x02\n\x04Spec\x12\x36\n\x06tables\x18\x01 \x03(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x06tables\x12\x33\n\x05views\x18\x02 \x03(\x0b\x32\x1d.kaskada.kaskada.v1alpha.ViewR\x05views\x12\x38\n\x07queries\x18\x03 \x03(\x0b\x32\x1e.kaskada.kaskada.v1alpha.QueryR\x07queries\x12T\n\x10materializations\x18\x04 \x03(\x0b\x32(.kaskada.kaskada.v1alpha.MaterializationR\x10materializationsB\xf9\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\tSpecProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
-
-
-_SPEC = DESCRIPTOR.message_types_by_name['Spec']
-Spec = _reflection.GeneratedProtocolMessageType('Spec', (_message.Message,), {
-  'DESCRIPTOR' : _SPEC,
-  '__module__' : 'kaskada.kaskada.v1alpha.spec_pb2'
-  # @@protoc_insertion_point(class_scope:kaskada.kaskada.v1alpha.Spec)
-  })
-_sym_db.RegisterMessage(Spec)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.spec_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\tSpecProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _SPEC._serialized_start=253
-  _SPEC._serialized_end=512
+  _globals['_SPEC']._serialized_start=253
+  _globals['_SPEC']._serialized_end=512
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py` & `kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/materialization.py` & `kaskada-0.1.6/src/kaskada/materialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member
 import logging
 import sys
 import uuid
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Dict, List, Optional
```

### Comparing `kaskada-0.1.5/src/kaskada/query.py` & `kaskada-0.1.6/src/kaskada/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member
 import datetime
 import logging
 import sys
 from enum import Enum
 from typing import List, Optional, Union
 
 import grpc
@@ -106,15 +107,16 @@
         expression (str): A Fenl expression to compute
         result_behavior (str, optional):
             Determines which results are returned. Either "all-results" (default), or "final-results" which returns
             only the final values for each entity.
         response_as (ResponseType):
             Determines how the response is returned.  Either "parquet" (default) or "csv".
         data_token_id (str, optional):
-            Enables repeatable queries. Queries performed against the same dataToken are always run against the same input data.
+            Enables repeatable queries.
+            Queries performed against the same dataToken are always run against the same input data.
         dry_run(bool, optional):
             When `True`, the query is validated and if there are no errors, the resultant schema is returned.
             No actual computation of results is performed.
         changed_since_time (datetime.datetime, optional):
             Time bound (inclusive) after which results will be output.
         final_result_time (Union[str, datetime.datetime], optional):
             Time bound (inclusive) at which results will be output.
```

### Comparing `kaskada-0.1.5/src/kaskada/slice_filters.py` & `kaskada-0.1.6/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/src/kaskada/table.py` & `kaskada-0.1.6/src/kaskada/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member
 import logging
 import sys
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import google.protobuf.wrappers_pb2 as wrappers
 import grpc
```

### Comparing `kaskada-0.1.5/src/kaskada/utils.py` & `kaskada-0.1.6/src/kaskada/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member
 import datetime
 import re
 import unicodedata
 from pathlib import Path
 from typing import Union
 
 import grpc
```

### Comparing `kaskada-0.1.5/src/kaskada/view.py` & `kaskada-0.1.6/src/kaskada/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member
 import logging
 import sys
 from typing import Optional, Union
 
 import grpc
 
 import kaskada.kaskada.v1alpha.view_service_pb2 as view_pb
```

### Comparing `kaskada-0.1.5/vendor/validate/validate.proto` & `kaskada-0.1.6/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/vendor/validate/validate_pb2.py` & `kaskada-0.1.6/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/vendor/validate/validate_pb2.pyi` & `kaskada-0.1.6/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.5/setup.py` & `kaskada-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n#### Generate documentation \nWe use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and \ngenerate an HTML formatted version of the codes documentation. \n\n* `poetry run poe docs` : generates and builds the docs \n* `poetry run poe docs-generate` : generates the docs (.rst files)\n* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)\n\nThe generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. \n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kaskada-0.1.5/PKG-INFO` & `kaskada-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.1.5
+Version: 0.1.6
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

