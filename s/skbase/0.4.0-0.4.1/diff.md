# Comparing `tmp/skbase-0.4.0.tar.gz` & `tmp/skbase-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbase-0.4.0.tar", last modified: Tue Apr 25 14:55:49 2023, max compression
+gzip compressed data, was "skbase-0.4.1.tar", last modified: Wed Apr 26 19:06:04 2023, max compression
```

## Comparing `skbase-0.4.0.tar` & `skbase-0.4.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-25 14:55:41.000000 skbase-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-25 14:55:49.757897 skbase-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-04-25 14:55:41.000000 skbase-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.741897 skbase-0.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.745897 skbase-0.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-04-25 14:55:41.000000 skbase-0.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-04-25 14:55:41.000000 skbase-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-25 14:55:49.757897 skbase-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.749897 skbase-0.4.0/skbase/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42244 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    35519 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11534 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_pretty_printing/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39083 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36969 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36016 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/testing/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/tests/test_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    40245 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14918 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    12123 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/tests/test_type_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.749897 skbase-0.4.0/skbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-26 19:05:53.000000 skbase-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-26 19:06:04.796428 skbase-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-04-26 19:05:53.000000 skbase-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.788428 skbase-0.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-04-26 19:05:53.000000 skbase-0.4.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-04-26 19:05:53.000000 skbase-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-26 19:06:04.796428 skbase-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42244 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_pretty_printing/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38915 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36016 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/testing/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/tests/test_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40245 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14918 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12123 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/zip-safe
```

### Comparing `skbase-0.4.0/LICENSE` & `skbase-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/PKG-INFO` & `skbase-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.0
+Version: 0.4.1
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.0 is now available. Checkout our
+:rocket: Version 0.4.1 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
```

### Comparing `skbase-0.4.0/README.md` & `skbase-0.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.0 is now available. Checkout our
+:rocket: Version 0.4.1 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
```

### Comparing `skbase-0.4.0/docs/source/conf.py` & `skbase-0.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/pyproject.toml` & `skbase-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skbase"
-version = "0.4.0"
+version = "0.4.1"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "Franz Király"},
     {name = "Markus Löning"},
     {name = "Ryan Kuhns"},
 ]
 maintainers = [
```

### Comparing `skbase-0.4.0/skbase/_exceptions.py` & `skbase-0.4.1/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/base/__init__.py` & `skbase-0.4.1/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/base/_base.py` & `skbase-0.4.1/skbase/base/_base.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/base/_meta.py` & `skbase-0.4.1/skbase/base/_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 # For conditions see licensing:
 # scikit-learn: https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
 # sktime:  https://github.com/sktime/sktime/blob/main/LICENSE
 """Implements functionality for meta objects composed of other objects."""
 from inspect import isclass
 from typing import TYPE_CHECKING, Any, Dict, List, Sequence, Tuple, Union, overload
 
-from sklearn.utils._estimator_html_repr import _VisualBlock
-
 from skbase.base._base import BaseEstimator, BaseObject
+from skbase.base._pretty_printing._object_html_repr import _VisualBlock
 from skbase.utils._iter import _format_seq_to_str, make_strings_unique
 from skbase.validate import is_named_object_tuple
 
 __author__: List[str] = ["mloning", "fkiraly", "RNKuhns"]
 __all__: List[str] = ["BaseMetaEstimator", "BaseMetaObject"]
 
 
@@ -653,25 +652,26 @@
         # construct the composite with both step and additional params
         composite_params.update(step_param)
         return composite_class(**composite_params)
 
     def _sk_visual_block_(self):
         """Logic to help render meta estimator as visual HTML block."""
         # Use tag interface that will be available when mixin is used
-        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
-        named_objects = getattr(self, named_object_attr)
+        named_object_attr_name = self.get_tag("named_object_parameters")  # type: ignore
+        named_object_attr = getattr(self, named_object_attr_name)
+        named_objects = self._coerce_to_named_object_tuples(named_object_attr)
         _, objs = self._get_names_and_objects(named_objects)
 
         def _get_name(name, obj):
             if obj is None or obj == "passthrough":
                 return f"{name}: passthrough"
             # Is an estimator
             return f"{name}: {obj.__class__.__name__}"
 
-        names = [_get_name(name, est) for name, est in self.steps]
+        names = [_get_name(name, est) for name, est in named_objects]
         name_details = [str(obj) for obj in objs]
         return _VisualBlock(
             "serial",
             objs,
             names=names,
             name_details=name_details,
             dash_wrapped=False,
```

### Comparing `skbase-0.4.0/skbase/base/_pretty_printing/_object_html_repr.py` & `skbase-0.4.1/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Many elements of this code were developed in scikit-learn. These elements
 # are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
 # conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
 """Functionality to represent instance of BaseObject as html."""
 
 import html
 import uuid
-from contextlib import closing, suppress
+from contextlib import closing
 from io import StringIO
 from string import Template
 
 __author__ = ["RNKuhns"]
 
 
 class _VisualBlock:
@@ -87,15 +87,15 @@
     else:
         out.write(f"<label>{name}</label>")
     out.write("</div></div>")  # outer_class inner_class
 
 
 def _get_visual_block(base_object):
     """Generate information about how to display a BaseObject."""
-    with suppress(AttributeError):
+    if hasattr(base_object, "_sk_visual_block_"):
         return base_object._sk_visual_block_()
 
     if isinstance(base_object, str):
         return _VisualBlock(
             "single", base_object, names=base_object, name_details=base_object
         )
     elif base_object is None:
```

### Comparing `skbase-0.4.0/skbase/base/_pretty_printing/_pprint.py` & `skbase-0.4.1/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/base/_tagmanager.py` & `skbase-0.4.1/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/lookup/__init__.py` & `skbase-0.4.1/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/lookup/_lookup.py` & `skbase-0.4.1/skbase/lookup/_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,85 +164,87 @@
     class_filter : objects or iterable of objects
         Classes that `klass` is checked against.
 
     Returns
     -------
     is_subclass : bool
         Whether the input class is a subclass of the `class_filter`.
+        If `class_filter` was `None`, returns `True`.
     """
     if class_filter is None:
-        is_subclass = True
-    else:
-        if isinstance(class_filter, Iterable) and not isinstance(class_filter, tuple):
-            class_filter = tuple(class_filter)
-        if issubclass(klass, class_filter):
-            is_subclass = True
-        else:
-            is_subclass = False
-    return is_subclass
+        return True
 
+    if isinstance(class_filter, Iterable) and not isinstance(class_filter, tuple):
+        class_filter = tuple(class_filter)
+    return issubclass(klass, class_filter)
 
-def _filter_by_tags(
-    klass: type,
-    tag_filter: Optional[Union[str, Sequence[str], Mapping[str, Any]]] = None,
-) -> bool:
-    """Determine if a class has a tag or has certain values for a tag.
+
+def _filter_by_tags(obj, tag_filter=None, as_dataframe=True):
+    """Check whether estimator satisfies tag_filter condition.
 
     Parameters
     ----------
-    klass : object
-        Class to check.
-    tag_filter : str, iterable of str or dict
-        Filter used to determine if `klass` has tag or expected tag values.
+    obj : BaseObject, an sktime estimator
+    tag_filter : dict of (str or list of str), default=None
+        subsets the returned estimators as follows:
+        each key/value pair is statement in "and"/conjunction
+
+        * key is tag name to sub-set on
+        * value str or list of string are tag values
+        * condition is "key must be equal to value, or in set(value)"
 
     Returns
     -------
-    has_tag : bool
-        Whether the input class has tags defined by the `tag_filter`.
+    cond_sat: bool, whether estimator satisfies condition in `tag_filter`
+        if `tag_filter` was None, returns `True`
     """
     if tag_filter is None:
         return True
 
-    if hasattr(klass, "get_class_tags"):
-        klass_tags = klass.get_class_tags()
+    if not isinstance(tag_filter, (str, Iterable, dict)):
+        raise TypeError(
+            "tag_filter argument of _filter_by_tags must be "
+            "a dict with str keys, str, or iterable of str, "
+            f"but found tag_filter of type {type(tag_filter)}"
+        )
 
-    else:
-        # If the object doesn't have tag interface it can't have the tags in tag_filter
+    if not hasattr(obj, "get_class_tag"):
         return False
-    # If a string is supplied verify it is in the returned tag dict
+
+    klass_tags = obj.get_class_tags().keys()
+
+    # case: tag_filter is string
     if isinstance(tag_filter, str):
-        has_tag = tag_filter in klass_tags
+        return tag_filter in klass_tags
+
+    # case: tag_filter is iterable of str but not dict
     # If a iterable of strings is provided, check that all are in the returned tag_dict
-    elif (
-        isinstance(tag_filter, Iterable)
-        and not isinstance(tag_filter, dict)
-        and all([isinstance(t, str) for t in tag_filter])
-    ):
-        has_tag = all([tag in klass_tags for tag in tag_filter])
-    # If a dict is supplied verify that tag and value are acceptable
-    elif isinstance(tag_filter, dict) and all(isinstance(k, str) for k in tag_filter):
-        has_tag = False  # default to tag being filtered out unless it passes below
-        for tag, value in tag_filter.items():
-            if not isinstance(value, Iterable):
-                value = [value]
-            if tag in klass_tags:
-                has_tag = klass_tags[tag] in set(value)
-            else:
-                has_tag = False
-            # We can break the loop and return has_tag as False if it is ever False
-            if not has_tag:
-                break
-    else:
+    if isinstance(tag_filter, Iterable) and not isinstance(tag_filter, dict):
+        if not all(isinstance(t, str) for t in tag_filter):
+            raise ValueError(
+                "tag_filter argument of _filter_by_tags must be "
+                f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
+            )
+        return all(tag in klass_tags for tag in tag_filter)
+
+    # case: tag_filter is dict
+    if not all(isinstance(t, str) for t in tag_filter.keys()):
         raise ValueError(
-            "`tag_filter` should be a string tag name, iterable of string tag names, "
-            "or a dictionary mapping tag names to allowable values. "
-            f"But `tag_filter` has type {type(tag_filter)}."
+            "tag_filter argument of _filter_by_tags must be "
+            f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
         )
 
-    return has_tag
+    cond_sat = True
+
+    for key, value in tag_filter.items():
+        if not isinstance(value, list):
+            value = [value]
+        cond_sat = cond_sat and obj.get_class_tag(key) in set(value)
+
+    return cond_sat
 
 
 def _walk(root, exclude=None, prefix=""):
     """Recursively return all modules and sub-modules as list of strings.
 
     Unlike pkgutil.walk_packages, does not import modules on exclusion list.
 
@@ -855,25 +857,18 @@
                     raise e
                 warnings.warn(str(e), ImportWarning, stacklevel=2)
 
     # Drop duplicates
     all_estimators = set(all_estimators)
 
     # Filter based on given estimator types
-    def _is_in_object_types(estimator, object_types):
-        return any(
-            inspect.isclass(x) and issubclass(estimator, x) for x in object_types
-        )
-
     if object_types:
-        object_types = _check_object_types(object_types, class_lookup)
+        obj_types = _check_object_types(object_types, class_lookup)
         all_estimators = [
-            (name, estimator)
-            for name, estimator in all_estimators
-            if _is_in_object_types(estimator, object_types)
+            (n, est) for (n, est) in all_estimators if _filter_by_class(est, obj_types)
         ]
 
     # Filter based on given exclude list
     if exclude_objects:
         exclude_objects = check_sequence(
             exclude_objects,
             sequence_type=list,
```

### Comparing `skbase-0.4.0/skbase/lookup/tests/test_lookup.py` & `skbase-0.4.1/skbase/lookup/tests/test_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     """Check output of get_package_metadata is expected type."""
     if not (isinstance(results, dict) and all(isinstance(k, str) for k in results)):
         return False
     for k, mod_metadata in results.items():
         if not isinstance(mod_metadata, dict):
             return False
         # Verify expected metadata keys are in the module's metadata dict
-        if not all([k in mod_metadata for k in MODULE_METADATA_EXPECTED_KEYS]):
+        if not all(k in mod_metadata for k in MODULE_METADATA_EXPECTED_KEYS):
             return False
         # Verify keys with string values have string values
         if not all(
             isinstance(mod_metadata[k], str) for k in ("path", "name", "authors")
         ):
             return False
         # Verify keys with bool values have bool valeus
@@ -391,23 +391,23 @@
     assert _filter_by_tags(Parent, {"A": "1", "B": 2}) is True
     # All keys in dict are in tag_filter, but at least 1 value doesn't match
     assert _filter_by_tags(Parent, {"A": 1, "B": 2}) is False
     # Atleast 1 key in dict is not in tag_filter
     assert _filter_by_tags(Parent, {"E": 1, "B": 2}) is False
 
     # Iterable tags should be all strings
-    with pytest.raises(ValueError, match=r"`tag_filter` should be.*"):
+    with pytest.raises(ValueError, match=r"tag_filter"):
         assert _filter_by_tags(Parent, ("A", "B", 3))
 
     # Tags that aren't iterable have to be strings
-    with pytest.raises(ValueError, match=r"`tag_filter` should be.*"):
+    with pytest.raises(TypeError, match=r"tag_filter"):
         assert _filter_by_tags(Parent, 7.0)
 
     # Dictionary tags should have string keys
-    with pytest.raises(ValueError, match=r"`tag_filter` should be.*"):
+    with pytest.raises(ValueError, match=r"tag_filter"):
         assert _filter_by_tags(Parent, {7: 11})
 
 
 def test_walk_returns_expected_format(fixture_skbase_root_path):
     """Check walk function returns expected format."""
 
     def _test_walk_return(p):
```

### Comparing `skbase-0.4.0/skbase/testing/test_all_objects.py` & `skbase-0.4.1/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/testing/utils/_conditional_fixtures.py` & `skbase-0.4.1/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/testing/utils/_dependencies.py` & `skbase-0.4.1/skbase/testing/utils/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/testing/utils/deep_equals.py` & `skbase-0.4.1/skbase/testing/utils/deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/testing/utils/inspect.py` & `skbase-0.4.1/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/testing/utils/tests/test_check_dependencies.py` & `skbase-0.4.1/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/testing/utils/tests/test_deep_equals.py` & `skbase-0.4.1/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/tests/conftest.py` & `skbase-0.4.1/skbase/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/tests/mock_package/test_mock_package.py` & `skbase-0.4.1/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/tests/test_base.py` & `skbase-0.4.1/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/tests/test_baseestimator.py` & `skbase-0.4.1/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/tests/test_exceptions.py` & `skbase-0.4.1/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/tests/test_meta.py` & `skbase-0.4.1/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/__init__.py` & `skbase-0.4.1/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/_check.py` & `skbase-0.4.1/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/_iter.py` & `skbase-0.4.1/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/_nested_iter.py` & `skbase-0.4.1/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/_utils.py` & `skbase-0.4.1/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/tests/test_check.py` & `skbase-0.4.1/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/tests/test_iter.py` & `skbase-0.4.1/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/tests/test_nested_iter.py` & `skbase-0.4.1/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/utils/tests/test_utils.py` & `skbase-0.4.1/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/validate/__init__.py` & `skbase-0.4.1/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/validate/_named_objects.py` & `skbase-0.4.1/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/validate/_types.py` & `skbase-0.4.1/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/validate/tests/test_iterable_named_objects.py` & `skbase-0.4.1/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase/validate/tests/test_type_validations.py` & `skbase-0.4.1/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.0/skbase.egg-info/PKG-INFO` & `skbase-0.4.1/skbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.0
+Version: 0.4.1
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.0 is now available. Checkout our
+:rocket: Version 0.4.1 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
```

### Comparing `skbase-0.4.0/skbase.egg-info/SOURCES.txt` & `skbase-0.4.1/skbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

