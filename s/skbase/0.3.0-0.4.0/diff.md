# Comparing `tmp/skbase-0.3.0.tar.gz` & `tmp/skbase-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbase-0.3.0.tar", last modified: Mon Jan  9 01:49:13 2023, max compression
+gzip compressed data, was "skbase-0.4.0.tar", last modified: Tue Apr 25 14:55:49 2023, max compression
```

## Comparing `skbase-0.3.0.tar` & `skbase-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.237988 skbase-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-01-09 01:48:59.000000 skbase-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-01-09 01:49:13.237988 skbase-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3221 2023-01-09 01:48:59.000000 skbase-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.229988 skbase-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.233988 skbase-0.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     9851 2023-01-09 01:48:59.000000 skbase-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-01-09 01:48:59.000000 skbase-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-01-09 01:49:13.237988 skbase-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.233988 skbase-0.3.0/skbase/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.233988 skbase-0.3.0/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    35305 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23960 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.233988 skbase-0.3.0/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38799 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.233988 skbase-0.3.0/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36969 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.233988 skbase-0.3.0/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    33524 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.237988 skbase-0.3.0/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9742 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10291 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    10822 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.237988 skbase-0.3.0/skbase/testing/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/testing/utils/tests/test_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.237988 skbase-0.3.0/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5420 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.237988 skbase-0.3.0/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    37478 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/tests/test_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.237988 skbase-0.3.0/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/utils/_nested_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.237988 skbase-0.3.0/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-01-09 01:48:59.000000 skbase-0.3.0/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 01:49:13.233988 skbase-0.3.0/skbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-01-09 01:49:13.000000 skbase-0.3.0/skbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-01-09 01:49:13.000000 skbase-0.3.0/skbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-09 01:49:13.000000 skbase-0.3.0/skbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-01-09 01:49:13.000000 skbase-0.3.0/skbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-01-09 01:49:13.000000 skbase-0.3.0/skbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-09 01:49:12.000000 skbase-0.3.0/skbase.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-25 14:55:41.000000 skbase-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-25 14:55:49.757897 skbase-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-04-25 14:55:41.000000 skbase-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.741897 skbase-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.745897 skbase-0.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-04-25 14:55:41.000000 skbase-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-04-25 14:55:41.000000 skbase-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-25 14:55:49.757897 skbase-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.749897 skbase-0.4.0/skbase/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42244 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35519 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11534 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_pretty_printing/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39083 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36969 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36016 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/testing/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/testing/utils/tests/test_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.753897 skbase-0.4.0/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40245 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14918 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12123 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.757897 skbase-0.4.0/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-04-25 14:55:41.000000 skbase-0.4.0/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:49.749897 skbase-0.4.0/skbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:55:49.000000 skbase-0.4.0/skbase.egg-info/zip-safe
```

### Comparing `skbase-0.3.0/LICENSE` & `skbase-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/PKG-INFO` & `skbase-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.3.0
+Version: 0.4.0
 Summary: Base classes for sklearn-like parametric objects
-Author: Markus Löning
-Author-email: Franz Király <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
+Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.3.0 is now available. Checkout our
+:rocket: Version 0.4.0 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
@@ -104,15 +103,15 @@
 ### pip
 skbase releases are available as source packages and binary wheels via PyPI
 and can be installed using pip. Checkout the full list of pre-compiled [wheels on PyPi](https://pypi.org/simple/skbase/).
 
 To install the core package use:
 
 ```bash
-pip install skbase
+pip install scikit-base
 ```
 
 or, if you want to install with the maximum set of dependencies, use:
 
 ```bash
-pip install skbase[all_extras]
+pip install scikit-base[all_extras]
 ```
```

### Comparing `skbase-0.3.0/README.md` & `skbase-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.3.0 is now available. Checkout our
+:rocket: Version 0.4.0 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
@@ -37,15 +37,15 @@
 ### pip
 skbase releases are available as source packages and binary wheels via PyPI
 and can be installed using pip. Checkout the full list of pre-compiled [wheels on PyPi](https://pypi.org/simple/skbase/).
 
 To install the core package use:
 
 ```bash
-pip install skbase
+pip install scikit-base
 ```
 
 or, if you want to install with the maximum set of dependencies, use:
 
 ```bash
-pip install skbase[all_extras]
+pip install scikit-base[all_extras]
 ```
```

### Comparing `skbase-0.3.0/docs/source/conf.py` & `skbase-0.4.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         {
             "name": "GitHub",
             "url": "https://github.com/sktime/skbase",
             "icon": "fab fa-github",
         },
         {
             "name": "Slack",
-            "url": "https://join.slack.com/t/sktime-group/shared_invite/zt-1cghagwee-sqLJ~eHWGYgzWbqUX937ig",  # noqa: E501
+            "url": "https://join.slack.com/t/skbase/shared_invite/zt-1qke3vzl2-fADjZBZadBlXsLUym5NlhA",  # noqa: E501
             "icon": "fab fa-slack",
         },
         {
             "name": "PyPI",
             "url": "https://pypi.org/project/skbase",
             "icon": "fa-solid fa-box",
         },
```

### Comparing `skbase-0.3.0/pyproject.toml` & `skbase-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "skbase"
-version = "0.3.0"
+version = "0.4.0"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
-    {name = "Franz Király", email = "f.kiraly@ucl.ac.uk"},
+    {name = "Franz Király"},
     {name = "Markus Löning"},
-    {name = "Ryan Kuhns", email = "rk.skbase@gmail.com"},
+    {name = "Ryan Kuhns"},
 ]
 maintainers = [
     {name = "Franz Kiraly", email = "f.kiraly@ucl.ac.uk"},
     {name = "Ryan Kuhns", email = "rk.skbase@gmail.com"},
 ]
 readme = "README.md"
 keywords = [
@@ -36,15 +36,15 @@
 ]
 requires-python = ">=3.7,<3.12"
 dependencies = [
     "scikit-learn>=0.24.0,<1.3.0", "typing-extensions", "pytest"
 ]
 
 [project.optional-dependencies]
-all_extras = ["pandas"]
+all_extras = ["numpy", "pandas"]
 
 dev = [
     "pre-commit",
     "pytest",
     "pytest-cov"
 ]
```

### Comparing `skbase-0.3.0/skbase/_exceptions.py` & `skbase-0.4.0/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/skbase/base/__init__.py` & `skbase-0.4.0/skbase/base/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 The included functionality makes it easy to re-use scikit-learn and
 sktime design principles in your project.
 """
 from typing import List
 
 from skbase.base._base import BaseEstimator, BaseObject
-from skbase.base._meta import BaseMetaEstimator
+from skbase.base._meta import BaseMetaEstimator, BaseMetaObject
 
 __author__: List[str] = ["mloning", "RNKuhns", "fkiraly"]
 __all__: List[str] = [
     "BaseObject",
     "BaseEstimator",
     "BaseMetaEstimator",
+    "BaseMetaObject",
 ]
```

### Comparing `skbase-0.3.0/skbase/base/_base.py` & `skbase-0.4.0/skbase/base/_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,36 +49,46 @@
 
 State:
     fitted model/strategy   - by convention, any attributes ending in "_"
     fitted state flag       - is_fitted (property)
     fitted state check      - check_is_fitted (raises error if not is_fitted)
 """
 import inspect
+import re
 import warnings
 from collections import defaultdict
 from copy import deepcopy
 from typing import List
 
 from sklearn import clone
 from sklearn.base import BaseEstimator as _BaseEstimator
 
 from skbase._exceptions import NotFittedError
+from skbase.base._pretty_printing._object_html_repr import _object_html_repr
+from skbase.base._tagmanager import _FlagManager
 
 __author__: List[str] = ["mloning", "RNKuhns", "fkiraly"]
 __all__: List[str] = ["BaseEstimator", "BaseObject"]
 
 
-class BaseObject(_BaseEstimator):
+class BaseObject(_FlagManager, _BaseEstimator):
     """Base class for parametric objects with sktime style tag interface.
 
     Extends scikit-learn's BaseEstimator to include sktime style interface for tags.
     """
 
+    _config = {
+        "display": "diagram",
+        "print_changed_only": True,
+    }
+
     def __init__(self):
-        self._tags_dynamic = {}
+        """Construct BaseObject."""
+        self._init_flags(flag_attr_name="_tags")
+        self._init_flags(flag_attr_name="_config")
         super(BaseObject, self).__init__()
 
     def __eq__(self, other):
         """Equality dunder. Checks equal class and parameters.
 
         Returns True iff result of get_params(deep=False)
         results in equal parameter sets.
@@ -212,14 +222,54 @@
         """
         parameters = cls._get_init_signature()
         default_dict = {
             x.name: x.default for x in parameters if x.default != inspect._empty
         }
         return default_dict
 
+    def get_params(self, deep=True):
+        """Get a dict of parameters values for this object.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            Whether to return parameters of components.
+
+            * If True, will return a dict of parameter name : value for this object,
+              including parameters of components (= BaseObject-valued parameters).
+            * If False, will return a dict of parameter name : value for this object,
+              but not include parameters of components.
+
+        Returns
+        -------
+        params : dict with str-valued keys
+            Dictionary of parameters, paramname : paramvalue
+            keys-value pairs include:
+
+            * always: all parameters of this object, as via `get_param_names`
+              values are parameter value for that key, of this object
+              values are always identical to values passed at construction
+            * if `deep=True`, also contains keys/value pairs of component parameters
+              parameters of components are indexed as `[componentname]__[paramname]`
+              all parameters of `componentname` appear as `paramname` with its value
+            * if `deep=True`, also contains arbitrary levels of component recursion,
+              e.g., `[componentname]__[componentcomponentname]__[paramname]`, etc
+        """
+        params = {key: getattr(self, key) for key in self.get_param_names()}
+
+        if deep:
+            deep_params = {}
+            for key, value in params.items():
+                if hasattr(value, "get_params"):
+                    deep_items = value.get_params().items()
+                    deep_params.update({f"{key}__{k}": val for k, val in deep_items})
+            params.update(deep_params)
+
+        return params
+
     def set_params(self, **params):
         """Set the parameters of this object.
 
         The method works on simple estimators as well as on nested objects.
         The latter have parameters of the form ``<component>__<parameter>`` so
         that it's possible to update each component of a nested object.
 
@@ -272,27 +322,15 @@
 
         Returns
         -------
         collected_tags : dict
             Dictionary of class tag name: tag value pairs. Collected from _tags
             class attribute via nested inheritance.
         """
-        collected_tags = {}
-
-        # We exclude the last two parent classes: sklearn.base.BaseEstimator and
-        # the basic Python object.
-        for parent_class in reversed(inspect.getmro(cls)[:-2]):
-            if hasattr(parent_class, "_tags"):
-                # Need the if here because mixins might not have _more_tags
-                # but might do redundant work in estimators
-                # (i.e. calling more tags on BaseEstimator multiple times)
-                more_tags = parent_class._tags
-                collected_tags.update(more_tags)
-
-        return deepcopy(collected_tags)
+        return cls._get_class_flags(flag_attr_name="_tags")
 
     @classmethod
     def get_class_tag(cls, tag_name, tag_value_default=None):
         """Get a class tag's value.
 
         Does not return information from dynamic tags (set via set_tags or clone_tags)
         that are defined on instances.
@@ -306,34 +344,31 @@
 
         Returns
         -------
         tag_value :
             Value of the `tag_name` tag in self. If not found, returns
             `tag_value_default`.
         """
-        collected_tags = cls.get_class_tags()
-
-        return collected_tags.get(tag_name, tag_value_default)
+        return cls._get_class_flag(
+            flag_name=tag_name,
+            flag_value_default=tag_value_default,
+            flag_attr_name="_tags",
+        )
 
     def get_tags(self):
         """Get tags from estimator class and dynamic tag overrides.
 
         Returns
         -------
         collected_tags : dict
             Dictionary of tag name : tag value pairs. Collected from _tags
             class attribute via nested inheritance and then any overrides
             and new tags from _tags_dynamic object attribute.
         """
-        collected_tags = self.get_class_tags()
-
-        if hasattr(self, "_tags_dynamic"):
-            collected_tags.update(self._tags_dynamic)
-
-        return deepcopy(collected_tags)
+        return self._get_flags(flag_attr_name="_tags")
 
     def get_tag(self, tag_name, tag_value_default=None, raise_error=True):
         """Get tag value from estimator class and dynamic tag overrides.
 
         Parameters
         ----------
         tag_name : str
@@ -350,22 +385,20 @@
             `raise_error` is True, otherwise it returns `tag_value_default`.
 
         Raises
         ------
         ValueError if raise_error is True i.e. if `tag_name` is not in
         self.get_tags().keys()
         """
-        collected_tags = self.get_tags()
-
-        tag_value = collected_tags.get(tag_name, tag_value_default)
-
-        if raise_error and tag_name not in collected_tags.keys():
-            raise ValueError(f"Tag with name {tag_name} could not be found.")
-
-        return tag_value
+        return self._get_flag(
+            flag_name=tag_name,
+            flag_value_default=tag_value_default,
+            raise_error=raise_error,
+            flag_attr_name="_tags",
+        )
 
     def set_tags(self, **tag_dict):
         """Set dynamic tags to given values.
 
         Parameters
         ----------
         **tag_dict : dict
@@ -376,19 +409,15 @@
         Self
             Reference to self.
 
         Notes
         -----
         Changes object state by settting tag values in tag_dict as dynamic tags in self.
         """
-        tag_update = deepcopy(tag_dict)
-        if hasattr(self, "_tags_dynamic"):
-            self._tags_dynamic.update(tag_update)
-        else:
-            self._tags_dynamic = tag_update
+        self._set_flags(flag_attr_name="_tags", **tag_dict)
 
         return self
 
     def clone_tags(self, estimator, tag_names=None):
         """Clone tags from another estimator as dynamic override.
 
         Parameters
@@ -404,28 +433,49 @@
             Reference to self.
 
         Notes
         -----
         Changes object state by setting tag values in tag_set from estimator as
         dynamic tags in self.
         """
-        tags_est = deepcopy(estimator.get_tags())
+        self._clone_flags(
+            estimator=estimator, flag_names=tag_names, flag_attr_name="_tags"
+        )
 
-        # if tag_set is not passed, default is all tags in estimator
-        if tag_names is None:
-            tag_names = tags_est.keys()
-        else:
-            # if tag_set is passed, intersect keys with tags in estimator
-            if not isinstance(tag_names, list):
-                tag_names = [tag_names]
-            tag_names = [key for key in tag_names if key in tags_est.keys()]
+        return self
+
+    def get_config(self):
+        """Get config flags for self.
+
+        Returns
+        -------
+        config_dict : dict
+            Dictionary of config name : config value pairs. Collected from _config
+            class attribute via nested inheritance and then any overrides
+            and new tags from _onfig_dynamic object attribute.
+        """
+        return self._get_flags(flag_attr_name="_config")
+
+    def set_config(self, **config_dict):
+        """Set config flags to given values.
+
+        Parameters
+        ----------
+        config_dict : dict
+            Dictionary of config name : config value pairs.
 
-        update_dict = {key: tags_est[key] for key in tag_names}
+        Returns
+        -------
+        self : reference to self.
 
-        self.set_tags(**update_dict)
+        Notes
+        -----
+        Changes object state, copies configs in config_dict to self._config_dynamic.
+        """
+        self._set_flags(flag_attr_name="_config", **config_dict)
 
         return self
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator.
 
@@ -635,14 +685,106 @@
         self_attrs = set(attrs).difference(cls_attrs).difference(param_names)
 
         comp_dict = {x: getattr(self, x) for x in self_attrs}
         comp_dict = {x: y for (x, y) in comp_dict.items() if isinstance(y, base_class)}
 
         return comp_dict
 
+    def __repr__(self, n_char_max: int = 700):
+        """Represent class as string.
+
+        This follows the scikit-learn implementation for the string representation
+        of parameterized objects.
+
+        Parameters
+        ----------
+        n_char_max : int
+            Maximum (approximate) number of non-blank characters to render. This
+            can be useful in testing.
+        """
+        from skbase.base._pretty_printing._pprint import _BaseObjectPrettyPrinter
+
+        n_max_elements_to_show = 30  # number of elements to show in sequences
+        # use ellipsis for sequences with a lot of elements
+        pp = _BaseObjectPrettyPrinter(
+            compact=True,
+            indent=1,
+            indent_at_name=True,
+            n_max_elements_to_show=n_max_elements_to_show,
+            changed_only=self.get_config()["print_changed_only"],
+        )
+
+        repr_ = pp.pformat(self)
+
+        # Use bruteforce ellipsis when there are a lot of non-blank characters
+        n_nonblank = len("".join(repr_.split()))
+        if n_nonblank > n_char_max:
+            lim = n_char_max // 2  # apprx number of chars to keep on both ends
+            regex = r"^(\s*\S){%d}" % lim
+            # The regex '^(\s*\S){%d}' matches from the start of the string
+            # until the nth non-blank character:
+            # - ^ matches the start of string
+            # - (pattern){n} matches n repetitions of pattern
+            # - \s*\S matches a non-blank char following zero or more blanks
+            left_match = re.match(regex, repr_)
+            right_match = re.match(regex, repr_[::-1])
+            left_lim = left_match.end() if left_match is not None else 0
+            right_lim = right_match.end() if right_match is not None else 0
+
+            if "\n" in repr_[left_lim:-right_lim]:
+                # The left side and right side aren't on the same line.
+                # To avoid weird cuts, e.g.:
+                # categoric...ore',
+                # we need to start the right side with an appropriate newline
+                # character so that it renders properly as:
+                # categoric...
+                # handle_unknown='ignore',
+                # so we add [^\n]*\n which matches until the next \n
+                regex += r"[^\n]*\n"
+                right_match = re.match(regex, repr_[::-1])
+                right_lim = right_match.end() if right_match is not None else 0
+
+            ellipsis = "..."
+            if left_lim + len(ellipsis) < len(repr_) - right_lim:
+                # Only add ellipsis if it results in a shorter repr
+                repr_ = repr_[:left_lim] + "..." + repr_[-right_lim:]
+
+        return repr_
+
+    @property
+    def _repr_html_(self):
+        """HTML representation of BaseObject.
+
+        This is redundant with the logic of `_repr_mimebundle_`. The latter
+        should be favorted in the long term, `_repr_html_` is only
+        implemented for consumers who do not interpret `_repr_mimbundle_`.
+        """
+        if self.get_config()["display"] != "diagram":
+            raise AttributeError(
+                "_repr_html_ is only defined when the "
+                "`display` configuration option is set to 'diagram'."
+            )
+        return self._repr_html_inner
+
+    def _repr_html_inner(self):
+        """Return HTML representation of class.
+
+        This function is returned by the @property `_repr_html_` to make
+        `hasattr(BaseObject, "_repr_html_") return `True` or `False` depending
+        on `self.get_config()["display"]`.
+        """
+        return _object_html_repr(self)
+
+    def _repr_mimebundle_(self, **kwargs):
+        """Mime bundle used by jupyter kernels to display instances of BaseObject."""
+        output = {"text/plain": repr(self)}
+        if self.get_config()["display"] == "diagram":
+            output["text/html"] = _object_html_repr(self)
+        return output
+
 
 class TagAliaserMixin:
     """Mixin class for tag aliasing and deprecation of old tags.
 
     To deprecate tags, add the TagAliaserMixin to BaseObject or BaseEstimator.
     alias_dict contains the deprecated tags, and supports removal and renaming.
         For removal, add an entry "old_tag_name": ""
@@ -666,14 +808,15 @@
     alias_dict = {"old_tag": "new_tag", "tag_to_remove": ""}
 
     # dictionary of removal version
     # key = old tag; value = version in which tag will be removed, as string
     deprecate_dict = {"old_tag": "0.12.0", "tag_to_remove": "99.99.99"}
 
     def __init__(self):
+        """Construct TagAliaserMixin."""
         super(TagAliaserMixin, self).__init__()
 
     @classmethod
     def get_class_tags(cls):
         """Get class tags from estimator class and all its parent classes.
 
         Returns
@@ -812,22 +955,22 @@
         ------
         DeprecationWarning for each tag in tags that is aliased by cls.alias_dict
         """
         for tag_name in tags:
             if tag_name in cls.alias_dict.keys():
                 version = cls.deprecate_dict[tag_name]
                 new_tag = cls.alias_dict[tag_name]
-                msg = f'tag "{tag_name}" will be removed in sktime version {version}'
+                msg = f"tag {tag_name!r} will be removed in sktime version {version}"
                 if new_tag != "":
                     msg += (
-                        f' and replaced by "{new_tag}", please use "{new_tag}" instead'
+                        f" and replaced by {new_tag!r}, please use {new_tag!r} instead"
                     )
                 else:
-                    msg += ', please remove code that access or sets "{tag_name}"'
-                warnings.warn(msg, category=DeprecationWarning)
+                    msg += ", please remove code that access or sets {tag_name!r}"
+                warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
 
 
 class BaseEstimator(BaseObject):
     """Base class for estimators with scikit-learn and sktime design patterns.
 
     Extends BaseObject to include basic functionality for fittable estimators.
     """
@@ -871,51 +1014,74 @@
         """
         if not self.is_fitted:
             raise NotFittedError(
                 f"This instance of {self.__class__.__name__} has not been fitted yet. "
                 f"Please call `fit` first."
             )
 
-    def get_fitted_params(self):
+    def get_fitted_params(self, deep=True):
         """Get fitted parameters.
 
         State required:
             Requires state to be "fitted".
 
+        Parameters
+        ----------
+        deep : bool, default=True
+            Whether to return fitted parameters of components.
+
+            * If True, will return a dict of parameter name : value for this object,
+              including fitted parameters of fittable components
+              (= BaseEstimator-valued parameters).
+            * If False, will return a dict of parameter name : value for this object,
+              but not include fitted parameters of components.
+
         Returns
         -------
-        fitted_params : dict of fitted parameters, keys are str names of parameters
-            parameters of components are indexed as [componentname]__[paramname]
+        fitted_params : dict with str-valued keys
+            Dictionary of fitted parameters, paramname : paramvalue
+            keys-value pairs include:
+
+            * always: all fitted parameters of this object, as via `get_param_names`
+              values are fitted parameter value for that key, of this object
+            * if `deep=True`, also contains keys/value pairs of component parameters
+              parameters of components are indexed as `[componentname]__[paramname]`
+              all parameters of `componentname` appear as `paramname` with its value
+            * if `deep=True`, also contains arbitrary levels of component recursion,
+              e.g., `[componentname]__[componentcomponentname]__[paramname]`, etc
         """
         if not self.is_fitted:
             raise NotFittedError(
                 f"estimator of type {type(self).__name__} has not been "
                 "fitted yet, please call fit on data before get_fitted_params"
             )
 
-        fitted_params = {}
+        # collect non-nested fitted params of self
+        fitted_params = self._get_fitted_params()
+
+        # the rest is only for nested parameters
+        # so, if deep=False, we simply return here
+        if not deep:
+            return fitted_params
 
         def sh(x):
             """Shorthand to remove all underscores at end of a string."""
             if x.endswith("_"):
                 return sh(x[:-1])
             else:
                 return x
 
         # add all nested parameters from components that are skbase BaseEstimator
         c_dict = self._components()
         for c, comp in c_dict.items():
             if isinstance(comp, BaseEstimator) and comp._is_fitted:
-                c_f_params = comp.get_fitted_params()
+                c_f_params = comp.get_fitted_params(deep=deep)
                 c_f_params = {f"{sh(c)}__{k}": v for k, v in c_f_params.items()}
                 fitted_params.update(c_f_params)
 
-        # add non-nested fitted params of self
-        fitted_params.update(self._get_fitted_params())
-
         # add all nested parameters from components that are sklearn estimators
         # we do this recursively as we have to reach into nested sklearn estimators
         any_components_left_to_process = True
         old_new_params = fitted_params
         # this loop recursively and iteratively processes components inside components
         while any_components_left_to_process:
             new_params = {}
```

### Comparing `skbase-0.3.0/skbase/lookup/__init__.py` & `skbase-0.4.0/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/skbase/lookup/_lookup.py` & `skbase-0.4.0/skbase/lookup/_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Walk package and return metadata on included classes and functions by module.
 all_objects(object_types, filter_tags)
     Look (and optionally filter) BaseObject descendants in a package or module.
 """
 # all_objects is based on the sktime all_estimator retrieval utility, which
 # is based on the sklearn estimator retrieval utility of the same name
 # See https://github.com/scikit-learn/scikit-learn/blob/main/COPYING and
-# https://github.com/alan-turing-institute/sktime/blob/main/LICENSE
+# https://github.com/sktime/sktime/blob/main/LICENSE
 import importlib
 import inspect
 import io
 import os
 import pathlib
 import pkgutil
 import sys
@@ -35,15 +35,15 @@
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
 from skbase.base import BaseObject
-from skbase.validate._types import _check_list_of_str_or_error
+from skbase.validate import check_sequence
 
 # Conditionally import TypedDict based on Python version
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
@@ -378,19 +378,19 @@
         if isinstance(path, (pathlib.Path, str)):
             path_ = str(path.absolute()) if isinstance(path, pathlib.Path) else path
             # Use the provided path and package name to load the module
             # if both available.
             try:
                 loader = _instantiate_loader(package_name, path_)
                 module = _import_module(loader, suppress_import_stdout=False)
-            except ImportError:
+            except ImportError as exc:
                 raise ValueError(
                     f"Unable to import a package named {package_name} based "
                     f"on provided `path`: {path_}."
-                )
+                ) from exc
         else:
             raise ValueError(
                 f"`path` must be a str path or pathlib.Path, but is type {type(path)}."
             )
 
     return module, path_, loader
 
@@ -840,24 +840,24 @@
                     module = importlib.import_module(module_name)
                     sys.stdout = sys.__stdout__
                 else:
                     module = importlib.import_module(module_name)
                 classes = inspect.getmembers(module, inspect.isclass)
                 # Filter classes
                 estimators = [
-                    (name, klass)
-                    for name, klass in classes
-                    if _is_estimator(name, klass)
+                    (klass.__name__, klass)
+                    for _, klass in classes
+                    if _is_estimator(klass.__name__, klass)
                 ]
                 all_estimators.extend(estimators)
             except ModuleNotFoundError as e:
                 # Skip missing soft dependencies
                 if "soft dependency" not in str(e):
                     raise e
-                warnings.warn(str(e), ImportWarning)
+                warnings.warn(str(e), ImportWarning, stacklevel=2)
 
     # Drop duplicates
     all_estimators = set(all_estimators)
 
     # Filter based on given estimator types
     def _is_in_object_types(estimator, object_types):
         return any(
@@ -870,15 +870,21 @@
             (name, estimator)
             for name, estimator in all_estimators
             if _is_in_object_types(estimator, object_types)
         ]
 
     # Filter based on given exclude list
     if exclude_objects:
-        exclude_objects = _check_list_of_str_or_error(exclude_objects, "exclude_object")
+        exclude_objects = check_sequence(
+            exclude_objects,
+            sequence_type=list,
+            element_type=str,
+            coerce_scalar_input=True,
+            sequence_name="exclude_object",
+        )
         all_estimators = [
             (name, estimator)
             for name, estimator in all_estimators
             if name not in exclude_objects
         ]
 
     # Drop duplicates, sort for reproducibility
@@ -897,15 +903,21 @@
         columns = ["object"]
     else:
         columns = ["name", "object"]
 
     # add new tuple entries to all_estimators for each tag in return_tags:
     return_tags = [] if return_tags is None else return_tags
     if return_tags:
-        return_tags = _check_list_of_str_or_error(return_tags, "return_tags")
+        return_tags = check_sequence(
+            return_tags,
+            sequence_type=list,
+            element_type=str,
+            coerce_scalar_input=True,
+            sequence_name="return_tags",
+        )
         # enrich all_estimators by adding the values for all return_tags tags:
         if all_estimators:
             if isinstance(all_estimators[0], tuple):
                 all_estimators = [
                     (name, est) + _get_return_tags(est, return_tags)
                     for (name, est) in all_estimators
                 ]
```

### Comparing `skbase-0.3.0/skbase/lookup/tests/test_lookup.py` & `skbase-0.4.0/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/skbase/testing/test_all_objects.py` & `skbase-0.4.0/skbase/testing/test_all_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,29 +70,35 @@
         instances are generated by create_test_instance class method of object_class
     """
 
     # class variables which can be overridden by descendants
     # ------------------------------------------------------
 
     # package to search for objects
+    # expected type: str, package/module name, relative to python environment root
     package_name = "skbase.tests.mock_package"
 
     # which object types are generated; None=all, or scitype string like "forecaster"
     object_type_filter = None
 
     # list of object types (class names) to exclude
+    # expected type: list of str, str are class names
     exclude_objects = None
 
     # list of tests to exclude
+    # expected type: dict of lists, key:str, value: List[str]
+    # keys are class names of estimators, values are lists of test names to exclude
     excluded_tests = None
 
     # list of valid tags
+    # expected type: list of str, str are tag names
     valid_tags = None
 
     # list of valid base type names
+    # expected type: list of str, str are base type (class) names
     valid_base_types = None
 
     # which sequence the conditional fixtures are generated in
     fixture_sequence = ["object_class", "object_instance"]
 
     # which fixtures are indirect, e.g., have an additional pytest.fixture block
     #   to generate an indirect fixture at runtime. Example: object_instance
@@ -165,15 +171,15 @@
             generator_dict[var] = getattr(self, gen)
 
         return generator_dict
 
     def is_excluded(self, test_name, est):
         """Shorthand to check whether test test_name is excluded for object est."""
         if self.excluded_tests is None:
-            return []
+            return False
         else:
             return test_name in self.excluded_tests.get(est.__name__, [])
 
     # the following functions define fixture generation logic for pytest_generate_tests
     # each function is of signature (test_name:str, **kwargs) -> List of fixtures
     # function with name _generate_[fixture_var] returns list of values for fixture_var
     #   where fixture_var is a fixture variable used in tests
@@ -359,15 +365,14 @@
                 set(test_names_subset).difference(tests_to_exclude)
             )
 
         # the below loops run all the tests and collect the results here:
         results = {}
         # loop A: we loop over all the tests
         for test_name in test_names_subset:
-
             test_fun = getattr(self, test_name)
             fixture_sequence = self.fixture_sequence
 
             # all arguments except the first one (self)
             fixture_vars = getfullargspec(test_fun)[0][1:]
             fixture_vars = [var for var in fixture_sequence if var in fixture_vars]
 
@@ -399,15 +404,14 @@
                         pytest_fixture_vars,
                         pytest_fixture_prod,
                         pytest_fixture_names,
                     )
 
             # loop B: for each test, we loop over all fixtures
             for params, fixt_name in zip(fixture_prod, fixture_names):
-
                 # this is needed because pytest unwraps 1-tuples automatically
                 # but subsequent code assumes params is k-tuple, no matter what k is
                 if len(fixture_vars) == 1:
                     params = (params,)
                 key = f"{test_name}[{fixt_name}]"
                 args = dict(zip(fixture_vars, params))
 
@@ -516,15 +520,28 @@
         return fixture_vars_return, fixture_prod_return, fixture_names_return
 
 
 class TestAllObjects(BaseFixtureGenerator, QuickTester):
     """Package level tests for BaseObjects."""
 
     def test_create_test_instance(self, object_class):
-        """Check first that create_test_instance logic works."""
+        """Check create_test_instance logic and basic constructor functionality.
+
+        create_test_instance and create_test_instances_and_names are the
+        key methods used to create test instances in testing.
+        If this test does not pass, validity of the other tests cannot be guaranteed.
+
+        Also tests inheritance and super call logic in the constructor.
+
+        Tests that:
+
+        * create_test_instance results in an instance of estimator_class
+        * `__init__` calls `super.__init__`
+        * `_tags_dynamic` attribute for tag inspection is present after construction
+        """
         object_instance = object_class.create_test_instance()
 
         # Check that init does not construct object of other class than itself
         assert isinstance(object_instance, object_class), (
             "object returned by create_test_instance must be an instance of the class, "
             f"found {type(object_instance)}"
         )
@@ -534,15 +551,22 @@
             f"super({object_class.__name__}, self).__init__, "
             "but that does not seem to be the case. Please ensure to call the "
             f"parent class's constructor in {object_class.__name__}.__init__"
         )
         assert hasattr(object_instance, "_tags_dynamic"), msg
 
     def test_create_test_instances_and_names(self, object_class):
-        """Check that create_test_instances_and_names works."""
+        """Check that create_test_instances_and_names works.
+
+        create_test_instance and create_test_instances_and_names are the
+        key methods used to create test instances in testing.
+        If this test does not pass, validity of the other tests cannot be guaranteed.
+
+        Tests expected function signature of create_test_instances_and_names.
+        """
         objects, names = object_class.create_test_instances_and_names()
 
         assert isinstance(objects, list), (
             "first return of create_test_instances_and_names must be a list, "
             f"found {type(objects)}"
         )
         assert isinstance(names, list), (
@@ -692,26 +716,52 @@
                 f"get_params result of {object_class.__name__} (x) does not match "
                 f"what was passed to set_params (y). "
                 f"Reason for discrepancy: {equals_msg}"
             )
             assert is_equal, msg
 
     def test_clone(self, object_instance):
-        """Check we can call clone from scikit-learn."""
-        object_instance.clone()
-        # object_clone = object_instance.clone()
-        # assert deep_equals(object_clone.get_params(), object_instance.get_params())
+        """Check that clone method does not raise exceptions and results in a clone.
+
+        A clone of an object x is an object that:
+
+        * has same class and parameters as x
+        * is not identical with x
+        * is unfitted (even if x was fitted)
+        """
+        obj_clone = object_instance.clone()
+        assert isinstance(obj_clone, type(object_instance))
+        assert obj_clone is not object_instance
+        if hasattr(obj_clone, "is_fitted"):
+            assert not obj_clone.is_fitted
 
     def test_repr(self, object_instance):
         """Check we can call repr."""
         repr(object_instance)
 
     def test_constructor(self, object_class):
-        """Check that the constructor has correct signature and behaves correctly."""
-        assert getfullargspec(object_class.__init__).varkw is None
+        """Check that the constructor has sklearn compatible signature and behaviour.
+
+        Based on sklearn check_estimator testing of __init__ logic.
+        Uses create_test_instance to create an instance.
+        Assumes test_create_test_instance has passed and certified create_test_instance.
+
+        Tests that:
+
+        * constructor has no varargs
+        * tests that constructor constructs an instance of the class
+        * tests that all parameters are set in init to an attribute of the same name
+        * tests that parameter values are always copied to the attribute and not changed
+        * tests that default parameters are one of the following:
+            None, str, int, float, bool, tuple, function, joblib memory, numpy primitive
+            (other type parameters should be None, default handling should be by writing
+            the default to attribute of a different name, e.g., my_param_ not my_param)
+        """
+        msg = f"constructor __init__ of {object_class} should have no varargs"
+        assert getfullargspec(object_class.__init__).varkw is None, msg
 
         obj = object_class.create_test_instance()
         assert isinstance(obj, object_class)
 
         # Ensure that each parameter is set in init
         init_params = _get_args(type(obj).__init__)
         invalid_attr = set(init_params) - set(vars(obj)) - {"self"}
```

### Comparing `skbase-0.3.0/skbase/testing/utils/_conditional_fixtures.py` & `skbase-0.4.0/skbase/testing/utils/_conditional_fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Exports create_conditional_fixtures_and_names utility
 """
 from copy import deepcopy
 from typing import Callable, Dict, List
 
 from skbase._exceptions import FixtureGenerationError
 from skbase.utils._nested_iter import _remove_single
-from skbase.validate._types import _check_list_of_str
+from skbase.validate import check_sequence
 
 __author__: List[str] = ["fkiraly"]
 __all__: List[str] = ["create_conditional_fixtures_and_names"]
 
 
 def create_conditional_fixtures_and_names(
     test_name: str,
@@ -93,20 +93,27 @@
                         test_name,
                         fixture_var1 = fixture[1], ...,
                         fixture_var(i-1) = fixture[i-1],
                     ), second return is exists; otherwise str(first return)
             return "fixture_str_pt[1]-fixture_str_pt[2]-...-fixture_str_pt[N]"
         fixture names correspond to fixtures with the same indices at picks (from lists)
     """
-    fixture_vars = _check_list_of_str(fixture_vars, name="fixture_vars")
+    fixture_vars = check_sequence(
+        fixture_vars, sequence_type=list, element_type=str, sequence_name="fixture_vars"
+    )
     fixture_vars = [var for var in fixture_vars if var in generator_dict.keys()]
 
     # order fixture_vars according to fixture_sequence if provided
     if fixture_sequence is not None:
-        fixture_sequence = _check_list_of_str(fixture_sequence, name="fixture_sequence")
+        fixture_sequence = check_sequence(
+            fixture_sequence,
+            sequence_type=list,
+            element_type=str,
+            sequence_name="fixture_sequence",
+        )
         ordered_fixture_vars = []
         for fixture_var_name in fixture_sequence:
             if fixture_var_name in fixture_vars:
                 ordered_fixture_vars += [fixture_var_name]
         fixture_vars = ordered_fixture_vars
 
     def get_fixtures(fixture_var, **kwargs):
```

### Comparing `skbase-0.3.0/skbase/testing/utils/_dependencies.py` & `skbase-0.4.0/skbase/testing/utils/_dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,24 +85,23 @@
         class_name = obj.__name__
     elif isinstance(obj, str):
         class_name = obj
     else:
         raise TypeError("obj must be a class, an object, a str, or None")
 
     for package in packages:
-
         try:
             req = Requirement(package)
         except InvalidRequirement:
             msg_version = (
                 f"wrong format for package requirement string, "
                 f'must be PEP 440 compatible requirement string, e.g., "pandas"'
-                f' or "pandas>1.1", but found "{package}"'
+                f' or "pandas>1.1", but found {package!r}'
             )
-            raise InvalidRequirement(msg_version)
+            raise InvalidRequirement(msg_version) from None
 
         package_name = req.name
         package_version_req = req.specifier
 
         # determine the package import
         if package_name in package_import_alias.keys():
             package_import_name = package_import_alias[package_name]
@@ -117,68 +116,68 @@
                 sys.stdout = sys.__stdout__
             else:
                 pkg_ref = import_module(package_import_name)
         # if package cannot be imported, make the user aware of installation requirement
         except ModuleNotFoundError as e:
             msg = (
                 f"{e}. "
-                f"{class_name} requires package '{package}' to be present "
-                f"in the python environment, but '{package}' was not found. "
+                f"{class_name} requires package {package!r} to be present "
+                f"in the python environment, but {package!r} was not found. "
             )
             if obj is not None:
                 msg = msg + (
-                    f"'{package}' is a dependency of {class_name} and required "
+                    f"{package!r} is a dependency of {class_name} and required "
                     f"to construct it. "
                 )
             msg = msg + (
                 f"Please run: `pip install {package}` to "
                 f"install the {package} package. "
             )
 
             if severity == "error":
                 raise ModuleNotFoundError(msg) from e
             elif severity == "warning":
-                warnings.warn(msg)
+                warnings.warn(msg, stacklevel=2)
                 return False
             elif severity == "none":
                 return False
             else:
                 raise RuntimeError(
                     "Error in calling _check_soft_dependencies, severity "
                     'argument must be "error", "warning", or "none",'
-                    f'found "{severity}".'
-                )
+                    f"found {severity!r}."
+                ) from e
 
         # now we check compatibility with the version specifier if non-empty
         if package_version_req != SpecifierSet(""):
             pkg_env_version = pkg_ref.__version__
 
             msg = (
-                f"{class_name} requires package '{package}' to be present "
+                f"{class_name} requires package {package!r} to be present "
                 f"in the python environment, with version {package_version_req}, "
                 f"but incompatible version {pkg_env_version} was found. "
             )
             if obj is not None:
                 msg = msg + (
-                    f"'{package}', with version {package_version_req},"
+                    f"{package!r}, with version {package_version_req},"
                     f"is a dependency of {class_name} and required to construct it. "
                 )
 
             # raise error/warning or return False if version is incompatible
             if pkg_env_version not in package_version_req:
                 if severity == "error":
                     raise ModuleNotFoundError(msg)
                 elif severity == "warning":
-                    warnings.warn(msg)
+                    warnings.warn(msg, stacklevel=2)
                 elif severity == "none":
                     return False
                 else:
                     raise RuntimeError(
                         "Error in calling _check_soft_dependencies, severity argument"
-                        f' must be "error", "warning", or "none", found "{severity}".'
+                        f' must be "error", "warning", or "none", found {severity!r}.'
                     )
 
     # if package can be imported and no version issue was caught for any string,
     # then obj is compatible with the requirements and we should return True
     return True
 
 
@@ -214,17 +213,17 @@
 
     try:
         est_specifier = SpecifierSet(est_specifier_tag)
     except InvalidSpecifier:
         msg_version = (
             f"wrong format for python_version tag, "
             f'must be PEP 440 compatible specifier string, e.g., "<3.9, >= 3.6.3",'
-            f' but found "{est_specifier_tag}"'
+            f" but found {est_specifier_tag!r}"
         )
-        raise InvalidSpecifier(msg_version)
+        raise InvalidSpecifier(msg_version) from None
 
     # python sys version, e.g., "3.8.12"
     sys_version = sys.version.split(" ")[0]
 
     if sys_version in est_specifier:
         return True
     # now we know that est_version is not compatible with sys_version
@@ -239,16 +238,16 @@
             msg += (
                 f" This is due to python version requirements of the {package} package."
             )
 
     if severity == "error":
         raise ModuleNotFoundError(msg)
     elif severity == "warning":
-        warnings.warn(msg)
+        warnings.warn(msg, stacklevel=2)
     elif severity == "none":
         return False
     else:
         raise RuntimeError(
             "Error in calling _check_python_version, severity "
-            f'argument must be "error", "warning", or "none", found "{severity}".'
+            f'argument must be "error", "warning", or "none", found {severity!r}.'
         )
     return True
```

### Comparing `skbase-0.3.0/skbase/testing/utils/deep_equals.py` & `skbase-0.4.0/skbase/testing/utils/deep_equals.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 from skbase.testing.utils._dependencies import _check_soft_dependencies
 
 __author__: List[str] = ["fkiraly"]
 __all__: List[str] = ["deep_equals"]
 
 
+# flag variables for available soft dependencies
+pandas_available = _check_soft_dependencies("pandas", severity="none")
+numpy_available = _check_soft_dependencies("numpy", severity="none")
+
+
 def deep_equals(x, y, return_msg=False):
     """Test two objects for equality in value.
 
     Correct if x/y are one of the following valid types:
         types compatible with != comparison
         pd.Series, pd.DataFrame, np.ndarray
         lists, tuples, or dicts of a valid type (recursive)
@@ -66,18 +71,14 @@
 
     if type(x) != type(y):
         return ret(False, f".type, x.type = {type(x)} != y.type = {type(y)}")
 
     # we now know all types are the same
     # so now we compare values
 
-    # flag variables for available soft dependencies
-    pandas_available = _check_soft_dependencies("pandas", severity="none")
-    numpy_available = _check_soft_dependencies("numpy", severity="none")
-
     if numpy_available:
         import numpy as np
 
     # pandas is a soft dependency, so we compare pandas objects separately
     #   and only if pandas is installed in the environment
     if _is_pandas(x) and pandas_available:
         res = _pandas_equals(x, y, return_msg=return_msg)
@@ -89,14 +90,16 @@
             return ret(False, f".dtype, x.dtype = {x.dtype} != y.dtype = {y.dtype}")
         return ret(np.array_equal(x, y, equal_nan=True), ".values")
     # recursion through lists, tuples and dicts
     elif isinstance(x, (list, tuple)):
         return ret(*_tuple_equals(x, y, return_msg=True))
     elif isinstance(x, dict):
         return ret(*_dict_equals(x, y, return_msg=True))
+    elif _is_npnan(x):
+        return ret(_is_npnan(y), f"type(x)={type(x)} != type(y)={type(y)}")
     elif isclass(x):
         return ret(x == y, f".class, x={x.__name__} != y={y.__name__}")
     elif type(x).__name__ == "ForecastingHorizon":
         return ret(*_fh_equals(x, y, return_msg=True))
     # this elif covers case where != is boolean
     # some types return a vector upon !=, this is covered in the next elif
     elif isinstance(x == y, bool):
@@ -105,42 +108,49 @@
     elif numpy_available and np.any(x != y) or any(_coerce_list(x != y)):
         return ret(False, f" !=, {x} != {y}")
 
     return ret(True, "")
 
 
 def _is_pandas(x):
-
     clstr = type(x).__name__
     if clstr in ["DataFrame", "Series"]:
         return True
     if clstr.endswith("Index"):
         return True
     else:
         return False
 
 
 def _is_npndarray(x):
-
     clstr = type(x).__name__
     return clstr == "ndarray"
 
 
+def _is_npnan(x):
+    if numpy_available:
+        import numpy as np
+
+        return isinstance(x, float) and np.isnan(x)
+
+    else:
+        return False
+
+
 def _coerce_list(x):
     """Coerce x to list."""
     if not isinstance(x, (list, tuple)):
         x = [x]
     if isinstance(x, tuple):
         x = list(x)
 
     return x
 
 
 def _pandas_equals(x, y, return_msg=False):
-
     import pandas as pd
 
     def ret(is_equal, msg):
         if return_msg:
             if is_equal:
                 msg = ""
             return is_equal, msg
@@ -171,15 +181,15 @@
                 False, f".columns, x.columns = {x.columns} != y.columns = {y.columns}"
             )
         # if columns are equal and at least one is object, recurse over Series
         if sum(x.dtypes == "object") > 0:
             for c in x.columns:
                 is_equal, msg = deep_equals(x[c], y[c], return_msg=True)
                 if not is_equal:
-                    return ret(False, f'["{c}"]' + msg)
+                    return ret(False, f"[{c!r}]" + msg)
             return ret(True, "")
         else:
             return ret(x.equals(y), f".df_equals, x = {x} != y = {y}")
     elif isinstance(x, pd.Index):
         return ret(x.equals(y), f".index_equals, x = {x} != y = {y}")
```

### Comparing `skbase-0.3.0/skbase/testing/utils/inspect.py` & `skbase-0.4.0/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/skbase/testing/utils/tests/test_check_dependencies.py` & `skbase-0.4.0/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/skbase/testing/utils/tests/test_deep_equals.py` & `skbase-0.4.0/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 EXAMPLES = [
     42,
     [],
     ((((())))),
     [([([([()])])])],
     np.array([2, 3, 4]),
     np.array([2, 4, 5]),
+    3.5,
+    4.2,
+    np.nan,
 ]
 
 
 if _check_soft_dependencies("pandas", severity="none"):
     import pandas as pd
 
     EXAMPLES += [
```

### Comparing `skbase-0.3.0/skbase/tests/conftest.py` & `skbase-0.4.0/skbase/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 SKBASE_BASE_CLASSES = (BaseObject, BaseEstimator)
 SKBASE_MODULES = (
     "skbase",
     "skbase._exceptions",
     "skbase.base",
     "skbase.base._base",
     "skbase.base._meta",
+    "skbase.base._pretty_printing",
+    "skbase.base._pretty_printing._object_html_repr",
+    "skbase.base._pretty_printing._pprint",
+    "skbase.base._tagmanager",
     "skbase.lookup",
     "skbase.lookup.tests",
     "skbase.lookup.tests.test_lookup",
     "skbase.lookup._lookup",
     "skbase.testing",
     "skbase.testing.test_all_objects",
     "skbase.testing.utils",
@@ -37,16 +41,20 @@
     "skbase.testing.utils.tests.test_deep_equals",
     "skbase.tests",
     "skbase.tests.conftest",
     "skbase.tests.test_base",
     "skbase.tests.test_baseestimator",
     "skbase.tests.mock_package.test_mock_package",
     "skbase.utils",
+    "skbase.utils._check",
+    "skbase.utils._iter",
     "skbase.utils._nested_iter",
+    "skbase.utils._utils",
     "skbase.validate",
+    "skbase.validate._named_objects",
     "skbase.validate._types",
 )
 SKBASE_PUBLIC_MODULES = (
     "skbase",
     "skbase.base",
     "skbase.lookup",
     "skbase.lookup.tests",
@@ -64,45 +72,97 @@
     "skbase.tests.test_baseestimator",
     "skbase.tests.mock_package.test_mock_package",
     "skbase.utils",
     "skbase.validate",
 )
 SKBASE_PUBLIC_CLASSES_BY_MODULE = {
     "skbase._exceptions": ("FixtureGenerationError", "NotFittedError"),
-    "skbase.base": ("BaseEstimator", "BaseMetaEstimator", "BaseObject"),
+    "skbase.base": (
+        "BaseEstimator",
+        "BaseMetaEstimator",
+        "BaseMetaObject",
+        "BaseObject",
+    ),
     "skbase.base._base": ("BaseEstimator", "BaseObject"),
-    "skbase.base._meta": ("BaseMetaEstimator",),
+    "skbase.base._meta": ("BaseMetaObject", "BaseMetaEstimator"),
+    "skbase.base._pretty_printing._pprint": ("KeyValTuple", "KeyValTupleParam"),
     "skbase.lookup._lookup": ("ClassInfo", "FunctionInfo", "ModuleInfo"),
     "skbase.testing": ("BaseFixtureGenerator", "QuickTester", "TestAllObjects"),
     "skbase.testing.test_all_objects": (
         "BaseFixtureGenerator",
         "QuickTester",
         "TestAllObjects",
     ),
 }
 SKBASE_CLASSES_BY_MODULE = SKBASE_PUBLIC_CLASSES_BY_MODULE.copy()
-SKBASE_CLASSES_BY_MODULE.update({"skbase.base._meta": ("BaseMetaEstimator",)})
+SKBASE_CLASSES_BY_MODULE.update(
+    {
+        "skbase.base._meta": (
+            "BaseMetaObject",
+            "BaseMetaEstimator",
+            "_MetaObjectMixin",
+            "_MetaTagLogicMixin",
+        ),
+        "skbase.base._pretty_printing._object_html_repr": ("_VisualBlock",),
+        "skbase.base._pretty_printing._pprint": (
+            "KeyValTuple",
+            "KeyValTupleParam",
+            "_BaseObjectPrettyPrinter",
+        ),
+        "skbase.base._tagmanager": ("_FlagManager",),
+    }
+)
 SKBASE_PUBLIC_FUNCTIONS_BY_MODULE = {
     "skbase.lookup": ("all_objects", "get_package_metadata"),
     "skbase.lookup._lookup": ("all_objects", "get_package_metadata"),
     "skbase.testing.utils._conditional_fixtures": (
         "create_conditional_fixtures_and_names",
     ),
     "skbase.testing.utils.deep_equals": ("deep_equals",),
-    "skbase.utils": ("flatten", "is_flat", "unflat_len", "unflatten"),
+    "skbase.validate": (
+        "check_sequence_named_objects",
+        "check_sequence",
+        "check_type",
+        "is_named_object_tuple",
+        "is_sequence",
+        "is_sequence_named_objects",
+    ),
+    "skbase.validate._named_objects": (
+        "check_sequence_named_objects",
+        "is_named_object_tuple",
+        "is_sequence_named_objects",
+    ),
+    "skbase.utils": (
+        "flatten",
+        "is_flat",
+        "make_strings_unique",
+        "subset_dict_keys",
+        "unflat_len",
+        "unflatten",
+    ),
+    "skbase.utils._iter": ("make_strings_unique",),
     "skbase.utils._nested_iter": (
         "flatten",
         "is_flat",
         "unflat_len",
         "unflatten",
     ),
+    "skbase.utils._utils": ("subset_dict_keys",),
+    "skbase.validate._types": ("check_sequence", "check_type", "is_sequence"),
 }
 SKBASE_FUNCTIONS_BY_MODULE = SKBASE_PUBLIC_FUNCTIONS_BY_MODULE.copy()
 SKBASE_FUNCTIONS_BY_MODULE.update(
     {
+        "skbase.base._pretty_printing._object_html_repr": (
+            "_get_visual_block",
+            "_object_html_repr",
+            "_write_base_object_html",
+            "_write_label_html",
+        ),
+        "skbase.base._pretty_printing._pprint": ("_changed_params", "_safe_repr"),
         "skbase.lookup._lookup": (
             "_determine_module_path",
             "_get_return_tags",
             "_is_ignored_module",
             "all_objects",
             "_is_non_public_module",
             "get_package_metadata",
@@ -118,44 +178,61 @@
             "_check_soft_dependencies",
             "_check_python_version",
         ),
         "skbase.testing.utils.deep_equals": (
             "_pandas_equals",
             "_dict_equals",
             "_is_pandas",
+            "_is_npnan",
             "_tuple_equals",
             "_fh_equals",
             "deep_equals",
             "_is_npndarray",
             "_coerce_list",
         ),
         "skbase.testing.utils.inspect": ("_get_args",),
+        "skbase.utils._check": ("_is_scalar_nan",),
+        "skbase.utils._iter": (
+            "_format_seq_to_str",
+            "_remove_type_text",
+            "_scalar_to_seq",
+            "make_strings_unique",
+        ),
         "skbase.utils._nested_iter": (
-            "_remove_single",
             "flatten",
             "is_flat",
+            "_remove_single",
             "unflat_len",
             "unflatten",
         ),
+        "skbase.utils._utils": ("subset_dict_keys",),
+        "skbase.validate._named_objects": (
+            "check_sequence_named_objects",
+            "is_named_object_tuple",
+            "is_sequence_named_objects",
+            "_named_baseobject_error_msg",
+        ),
         "skbase.validate._types": (
-            "_check_iterable_of_class_or_error",
-            "_check_list_of_str",
-            "_check_list_of_str_or_error",
+            "check_sequence",
+            "check_type",
+            "is_sequence",
+            "_convert_scalar_seq_type_input_to_tuple",
         ),
     }
 )
 
 
 # Fixture class for testing tag system
 class Parent(BaseObject):
     """Parent class to test BaseObject's usage."""
 
     _tags = {"A": "1", "B": 2, "C": 1234, "3": "D"}
 
     def __init__(self, a="something", b=7, c=None):
+        """Initialize the class."""
         self.a = a
         self.b = b
         self.c = c
         super().__init__()
 
     def some_method(self):
         """To be implemented by child class."""
```

### Comparing `skbase-0.3.0/skbase/tests/mock_package/test_mock_package.py` & `skbase-0.4.0/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/skbase/tests/test_base.py` & `skbase-0.4.0/skbase/tests/test_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,19 +65,19 @@
     "test_create_test_instances_and_names",
     "test_has_implementation_of",
     "test_eq_dunder",
 ]
 
 import inspect
 from copy import deepcopy
+from typing import Any, Dict, Type
 
 import numpy as np
 import pytest
 import scipy.sparse as sp
-from sklearn import config_context
 
 # TODO: Update with import of skbase clone function once implemented
 from sklearn.base import clone
 
 from skbase.base import BaseEstimator, BaseObject
 from skbase.tests.conftest import Child, Parent
 from skbase.tests.mock_package.test_mock_package import CompositionDummy
@@ -196,21 +196,21 @@
 @pytest.fixture
 def fixture_reset_tester():
     """Pytest fixture for ResetTester."""
     return ResetTester
 
 
 @pytest.fixture
-def fixture_class_child_tags(fixture_class_child):
+def fixture_class_child_tags(fixture_class_child: Type[Child]):
     """Pytest fixture for tags of Child."""
     return fixture_class_child.get_class_tags()
 
 
 @pytest.fixture
-def fixture_object_instance_set_tags(fixture_tag_class_object):
+def fixture_object_instance_set_tags(fixture_tag_class_object: Child):
     """Fixture class instance to test tag setting."""
     fixture_tag_set = {"A": 42424243, "E": 3}
     return fixture_tag_class_object.set_tags(**fixture_tag_set)
 
 
 @pytest.fixture
 def fixture_object_tags():
@@ -262,29 +262,31 @@
 
 @pytest.fixture
 def fixture_class_instance_no_param_interface():
     """Pytest fixture class instance for NoParamInterface."""
     return NoParamInterface()
 
 
-def test_get_class_tags(fixture_class_child, fixture_class_child_tags):
+def test_get_class_tags(
+    fixture_class_child: Type[Child], fixture_class_child_tags: Any
+):
     """Test get_class_tags class method of BaseObject for correctness.
 
     Raises
     ------
     AssertError if inheritance logic in get_class_tags is incorrect
     """
     child_tags = fixture_class_child.get_class_tags()
 
     msg = "Inheritance logic in BaseObject.get_class_tags is incorrect"
 
     assert child_tags == fixture_class_child_tags, msg
 
 
-def test_get_class_tag(fixture_class_child, fixture_class_child_tags):
+def test_get_class_tag(fixture_class_child: Type[Child], fixture_class_child_tags: Any):
     """Test get_class_tag class method of BaseObject for correctness.
 
     Raises
     ------
     AssertError if inheritance logic in get_tag is incorrect
     AssertError if default override logic in get_tag is incorrect
     """
@@ -303,29 +305,29 @@
 
     msg = "Default override logic in BaseObject.get_class_tag is incorrect"
 
     assert child_tag_default == "bar", msg
     assert child_tag_default_none is None, msg
 
 
-def test_get_tags(fixture_tag_class_object, fixture_object_tags):
+def test_get_tags(fixture_tag_class_object: Child, fixture_object_tags: Dict[str, Any]):
     """Test get_tags method of BaseObject for correctness.
 
     Raises
     ------
     AssertError if inheritance logic in get_tags is incorrect
     """
     object_tags = fixture_tag_class_object.get_tags()
 
     msg = "Inheritance logic in BaseObject.get_tags is incorrect"
 
     assert object_tags == fixture_object_tags, msg
 
 
-def test_get_tag(fixture_tag_class_object, fixture_object_tags):
+def test_get_tag(fixture_tag_class_object: Child, fixture_object_tags: Dict[str, Any]):
     """Test get_tag method of BaseObject for correctness.
 
     Raises
     ------
     AssertError if inheritance logic in get_tag is incorrect
     AssertError if default override logic in get_tag is incorrect
     """
@@ -347,29 +349,29 @@
 
     msg = "Default override logic in BaseObject.get_tag is incorrect"
 
     assert object_tag_default == "bar", msg
     assert object_tag_default_none is None, msg
 
 
-def test_get_tag_raises(fixture_tag_class_object):
+def test_get_tag_raises(fixture_tag_class_object: Child):
     """Test that get_tag method raises error for unknown tag.
 
     Raises
     ------
     AssertError if get_tag does not raise error for unknown tag.
     """
     with pytest.raises(ValueError, match=r"Tag with name"):
         fixture_tag_class_object.get_tag("bar")
 
 
 def test_set_tags(
-    fixture_object_instance_set_tags,
-    fixture_object_set_tags,
-    fixture_object_dynamic_tags,
+    fixture_object_instance_set_tags: Any,
+    fixture_object_set_tags: Dict[str, Any],
+    fixture_object_dynamic_tags: Dict[str, int],
 ):
     """Test set_tags method of BaseObject for correctness.
 
     Raises
     ------
     AssertionError if override logic in set_tags is incorrect
     """
@@ -377,15 +379,17 @@
 
     assert (
         fixture_object_instance_set_tags._tags_dynamic == fixture_object_dynamic_tags
     ), msg
     assert fixture_object_instance_set_tags.get_tags() == fixture_object_set_tags, msg
 
 
-def test_set_tags_works_with_missing_tags_dynamic_attribute(fixture_tag_class_object):
+def test_set_tags_works_with_missing_tags_dynamic_attribute(
+    fixture_tag_class_object: Child,
+):
     """Test set_tags will still work if _tags_dynamic is missing."""
     base_obj = deepcopy(fixture_tag_class_object)
     delattr(base_obj, "_tags_dynamic")
     assert not hasattr(base_obj, "_tags_dynamic")
     base_obj.set_tags(some_tag="something")
     tags = base_obj.get_tags()
     assert hasattr(base_obj, "_tags_dynamic")
@@ -456,29 +460,33 @@
     test_obj = TestClass()
     test_obj.clone_tags(another_base_obj)
     test_obj_tags = test_obj.get_tags()
     for tag in another_base_obj_tags:
         assert test_obj_tags.get(tag) == another_base_obj_tags[tag]
 
 
-def test_is_composite(fixture_composition_dummy):
+def test_is_composite(fixture_composition_dummy: Type[CompositionDummy]):
     """Test is_composite tag for correctness.
 
     Raises
     ------
     AssertionError if logic behind is_composite is incorrect
     """
     non_composite = fixture_composition_dummy(foo=42)
     composite = fixture_composition_dummy(foo=non_composite)
 
     assert not non_composite.is_composite()
     assert composite.is_composite()
 
 
-def test_components(fixture_object, fixture_class_parent, fixture_composition_dummy):
+def test_components(
+    fixture_object: Type[BaseObject],
+    fixture_class_parent: Type[Parent],
+    fixture_composition_dummy: Type[CompositionDummy],
+):
     """Test component retrieval.
 
     Raises
     ------
     AssertionError if logic behind _components is incorrect, logic tested:
         calling _components on a non-composite returns an empty dict
         calling _components on a composite returns name/BaseObject pair in dict,
@@ -503,15 +511,15 @@
     assert comp_comps["foo_"] is not composite.foo
 
     assert comp_comps == comp_comps_baseobject_filter
     assert comp_comps_filter == {}
 
 
 def test_components_raises_error_base_class_is_not_class(
-    fixture_object, fixture_composition_dummy
+    fixture_object: Type[BaseObject], fixture_composition_dummy: Type[CompositionDummy]
 ):
     """Test _component method raises error if base_class param is not class."""
     non_composite = fixture_composition_dummy(foo=42)
     composite = fixture_composition_dummy(foo=non_composite)
     with pytest.raises(
         TypeError, match="base_class must be a class, but found <class 'int'>"
     ):
@@ -522,29 +530,29 @@
         TypeError,
         match=msg,
     ):
         composite._components(fixture_object())
 
 
 def test_components_raises_error_base_class_is_not_baseobject_subclass(
-    fixture_composition_dummy,
+    fixture_composition_dummy: Type[CompositionDummy],
 ):
     """Test _component method raises error if base_class is not BaseObject subclass."""
 
     class SomeClass:
         pass
 
     composite = fixture_composition_dummy(foo=SomeClass())
     with pytest.raises(TypeError, match="base_class must be a subclass of BaseObject"):
         composite._components(SomeClass)
 
 
 # Test parameter interface (get_params, set_params, reset and related methods)
 # Some tests of get_params and set_params are adapted from sklearn tests
-def test_reset(fixture_reset_tester):
+def test_reset(fixture_reset_tester: Type[ResetTester]):
     """Test reset method for correct behaviour, on a simple estimator.
 
     Raises
     ------
     AssertionError if logic behind reset is incorrect, logic tested:
         reset should remove any object attributes that are not hyper-parameters,
         with the exception of attributes containing double-underscore "__"
@@ -563,63 +571,67 @@
     assert not hasattr(x, "d")
     assert not hasattr(x, "_d")
     assert not hasattr(x, "d_")
     assert hasattr(x, "f__o__o") and x.f__o__o == 252
     assert hasattr(x, "foo")
 
 
-def test_reset_composite(fixture_reset_tester):
+def test_reset_composite(fixture_reset_tester: Type[ResetTester]):
     """Test reset method for correct behaviour, on a composite estimator."""
     y = fixture_reset_tester(42)
     x = fixture_reset_tester(a=y)
 
     x.foo(y)
     x.d.foo()
 
     x.reset()
 
     assert hasattr(x, "a")
     assert not hasattr(x, "d")
     assert not hasattr(x.a, "d")
 
 
-def test_get_init_signature(fixture_class_parent):
+def test_get_init_signature(fixture_class_parent: Type[Parent]):
     """Test error is raised when invalid init signature is used."""
     init_sig = fixture_class_parent._get_init_signature()
     init_sig_is_list = isinstance(init_sig, list)
     init_sig_elements_are_params = all(
         isinstance(p, inspect.Parameter) for p in init_sig
     )
     assert (
         init_sig_is_list and init_sig_elements_are_params
     ), "`_get_init_signature` is not returning expected result."
 
 
-def test_get_init_signature_raises_error_for_invalid_signature(fixture_invalid_init):
+def test_get_init_signature_raises_error_for_invalid_signature(
+    fixture_invalid_init: Type[InvalidInitSignatureTester],
+):
     """Test error is raised when invalid init signature is used."""
     with pytest.raises(RuntimeError):
         fixture_invalid_init._get_init_signature()
 
 
 def test_get_param_names(
-    fixture_object, fixture_class_parent, fixture_class_parent_expected_params
+    fixture_object: Type[BaseObject],
+    fixture_class_parent: Type[Parent],
+    fixture_class_parent_expected_params: Dict[str, Any],
 ):
     """Test that get_param_names returns list of string parameter names."""
     param_names = fixture_class_parent.get_param_names()
     assert param_names == sorted([*fixture_class_parent_expected_params])
 
     param_names = fixture_object.get_param_names()
     assert param_names == []
 
 
 def test_get_params(
-    fixture_class_parent,
-    fixture_class_parent_expected_params,
-    fixture_class_instance_no_param_interface,
-    fixture_composition_dummy,
+    fixture_class_parent: Type[Parent],
+    fixture_class_parent_expected_params: Dict[str, Any],
+    fixture_class_instance_no_param_interface: NoParamInterface,
+    fixture_composition_dummy: Type[CompositionDummy],
 ):
     """Test get_params returns expected parameters."""
     # Simple test of returned params
     base_obj = fixture_class_parent()
     params = base_obj.get_params()
     assert params == fixture_class_parent_expected_params
 
@@ -634,23 +646,26 @@
     # Since NoParamInterface does not have get_params we should just return
     # "foo" and "bar" in params and no other parameters
     composite = fixture_composition_dummy(foo=fixture_class_instance_no_param_interface)
     params = composite.get_params()
     assert "foo" in params and "bar" in params and len(params) == 2
 
 
-def test_get_params_invariance(fixture_class_parent, fixture_composition_dummy):
+def test_get_params_invariance(
+    fixture_class_parent: Type[Parent],
+    fixture_composition_dummy: Type[CompositionDummy],
+):
     """Test that get_params(deep=False) is subset of get_params(deep=True)."""
     composite = fixture_composition_dummy(foo=fixture_class_parent(), bar=84)
     shallow_params = composite.get_params(deep=False)
     deep_params = composite.get_params(deep=True)
     assert all(item in deep_params.items() for item in shallow_params.items())
 
 
-def test_get_params_after_set_params(fixture_class_parent):
+def test_get_params_after_set_params(fixture_class_parent: Type[Parent]):
     """Test that get_params returns the same thing before and after set_params.
 
     Based on scikit-learn check in check_estimator.
     """
     base_obj = fixture_class_parent()
 
     orig_params = base_obj.get_params(deep=False)
@@ -683,17 +698,17 @@
                 assert set(test_params.keys()) == set(curr_params.keys()), msg
                 for k, v in curr_params.items():
                     assert test_params[k] is v, msg
         test_params[param_name] = default_value
 
 
 def test_set_params(
-    fixture_class_parent,
-    fixture_class_parent_expected_params,
-    fixture_composition_dummy,
+    fixture_class_parent: Type[Parent],
+    fixture_class_parent_expected_params: Dict[str, Any],
+    fixture_composition_dummy: Type[CompositionDummy],
 ):
     """Test set_params works as expected."""
     # Simple case of setting a parameter
     base_obj = fixture_class_parent()
     base_obj.set_params(b="updated param value")
     expected_params = deepcopy(fixture_class_parent_expected_params)
     expected_params["b"] = "updated param value"
@@ -707,15 +722,16 @@
     assert (
         params["foo__b"] == "updated param value"
         and composite.foo.b == "updated param value"
     )
 
 
 def test_set_params_raises_error_non_existent_param(
-    fixture_class_parent_instance, fixture_composition_dummy
+    fixture_class_parent_instance: Parent,
+    fixture_composition_dummy: Type[CompositionDummy],
 ):
     """Test set_params raises an error when passed a non-existent parameter name."""
     # non-existing parameter in svc
     with pytest.raises(ValueError):
         fixture_class_parent_instance.set_params(
             non_existant_param="updated param value"
         )
@@ -723,15 +739,16 @@
     # non-existing parameter of composite
     composite = fixture_composition_dummy(foo=fixture_class_parent_instance, bar=84)
     with pytest.raises(ValueError):
         composite.set_params(foo__non_existant_param=True)
 
 
 def test_set_params_raises_error_non_interface_composite(
-    fixture_class_instance_no_param_interface, fixture_composition_dummy
+    fixture_class_instance_no_param_interface: NoParamInterface,
+    fixture_composition_dummy: Type[CompositionDummy],
 ):
     """Test set_params raises error when setting param of non-conforming composite."""
     # When a composite is made up of a class that doesn't have the BaseObject
     # parameter interface, we should get a AttributeError when trying to
     # set the composite's params
     composite = fixture_composition_dummy(foo=fixture_class_instance_no_param_interface)
     with pytest.raises(AttributeError):
@@ -749,52 +766,56 @@
     est = BadObject()
     msg = "'BadObject' object has no attribute 'param'"
 
     with pytest.raises(AttributeError, match=msg):
         est.get_params()
 
 
-def test_set_params_with_no_param_to_set_returns_object(fixture_class_parent):
+def test_set_params_with_no_param_to_set_returns_object(
+    fixture_class_parent: Type[Parent],
+):
     """Test set_params correctly returns self when no parameters are set."""
     base_obj = fixture_class_parent()
     orig_params = deepcopy(base_obj.get_params())
     base_obj_set_params = base_obj.set_params()
     assert (
         isinstance(base_obj_set_params, fixture_class_parent)
         and base_obj_set_params.get_params() == orig_params
     )
 
 
 # This section tests the clone functionality
 # These have been adapted from sklearn's tests of clone to use the clone
 # method that is included as part of the BaseObject interface
-def test_clone(fixture_class_parent_instance):
+def test_clone(fixture_class_parent_instance: Parent):
     """Test that clone is making a deep copy as expected."""
     # Creates a BaseObject and makes a copy of its original state
     # (which, in this case, is the current state of the BaseObject),
     # and check that the obtained copy is a correct deep copy.
     new_base_obj = fixture_class_parent_instance.clone()
     assert fixture_class_parent_instance is not new_base_obj
     assert fixture_class_parent_instance.get_params() == new_base_obj.get_params()
 
 
-def test_clone_2(fixture_class_parent_instance):
+def test_clone_2(fixture_class_parent_instance: Parent):
     """Test that clone does not copy attributes not set in constructor."""
     # We first create an estimator, give it an own attribute, and
     # make a copy of its original state. Then we check that the copy doesn't
     # have the specific attribute we manually added to the initial estimator.
 
     # base_obj = fixture_class_parent(a=7.0, b="some_str")
     fixture_class_parent_instance.own_attribute = "test"
     new_base_obj = fixture_class_parent_instance.clone()
     assert not hasattr(new_base_obj, "own_attribute")
 
 
 def test_clone_raises_error_for_nonconforming_objects(
-    fixture_invalid_init, fixture_buggy, fixture_modify_param
+    fixture_invalid_init: Type[InvalidInitSignatureTester],
+    fixture_buggy: Type[Buggy],
+    fixture_modify_param: Type[ModifyParam],
 ):
     """Test that clone raises an error on nonconforming BaseObjects."""
     buggy = fixture_buggy()
     buggy.a = 2
     with pytest.raises(RuntimeError):
         buggy.clone()
 
@@ -803,146 +824,185 @@
         varg_obj.clone()
 
     obj_that_modifies = fixture_modify_param(a=[0])
     with pytest.raises(RuntimeError):
         obj_that_modifies.clone()
 
 
-def test_clone_param_is_none(fixture_class_parent):
+def test_clone_param_is_none(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter set to None."""
     base_obj = fixture_class_parent(c=None)
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
     assert base_obj.c is new_base_obj.c
     assert base_obj.c is new_base_obj2.c
 
 
-def test_clone_empty_array(fixture_class_parent):
+def test_clone_empty_array(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter is scipy sparse matrix.
 
     This test is based on scikit-learn regression test to make sure clone
     works with default parameter set to scipy sparse matrix.
     """
     # Regression test for cloning estimators with empty arrays
     base_obj = fixture_class_parent(c=np.array([]))
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
     np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
     np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
 
 
-def test_clone_sparse_matrix(fixture_class_parent):
+def test_clone_sparse_matrix(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter is scipy sparse matrix.
 
     This test is based on scikit-learn regression test to make sure clone
     works with default parameter set to scipy sparse matrix.
     """
     base_obj = fixture_class_parent(c=sp.csr_matrix(np.array([[0]])))
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
     np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
     np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
 
 
-def test_clone_nan(fixture_class_parent):
+def test_clone_nan(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter is np.nan.
 
     This test is based on scikit-learn regression test to make sure clone
     works with default parameter set to np.nan.
     """
     # Regression test for cloning estimators with default parameter as np.nan
     base_obj = fixture_class_parent(c=np.nan)
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
 
     assert base_obj.c is new_base_obj.c
     assert base_obj.c is new_base_obj2.c
 
 
-def test_clone_estimator_types(fixture_class_parent):
+def test_clone_estimator_types(fixture_class_parent: Type[Parent]):
     """Test clone works for parameters that are types rather than instances."""
     base_obj = fixture_class_parent(c=fixture_class_parent)
     new_base_obj = base_obj.clone()
 
     assert base_obj.c == new_base_obj.c
 
 
-def test_clone_class_rather_than_instance_raises_error(fixture_class_parent):
+def test_clone_class_rather_than_instance_raises_error(
+    fixture_class_parent: Type[Parent],
+):
     """Test clone raises expected error when cloning a class instead of an instance."""
     msg = "You should provide an instance of scikit-learn estimator"
     with pytest.raises(TypeError, match=msg):
         clone(fixture_class_parent)
 
 
 # Tests of BaseObject pretty printing representation inspired by sklearn
-def test_baseobject_repr(fixture_class_parent, fixture_composition_dummy):
+def test_baseobject_repr(
+    fixture_class_parent: Type[Parent],
+    fixture_composition_dummy: Type[CompositionDummy],
+):
     """Test BaseObject repr works as expected."""
     # Simple test where all parameters are left at defaults
     # Should not see parameters and values in printed representation
+
     base_obj = fixture_class_parent()
     assert repr(base_obj) == "Parent()"
 
-    # Check that we can alter the detail about params that is printed
-    # using config_context with ``print_changed_only=False``
-    with config_context(print_changed_only=False):
-        assert repr(base_obj) == "Parent(a='something', b=7, c=None)"
+    # Check that local config works as expected
+    base_obj.set_config(print_changed_only=False)
+    assert repr(base_obj) == "Parent(a='something', b=7, c=None)"
+
+    # Test with dict parameter (note that dict is sorted by keys when printed)
+    # not printed in order it was created
+    base_obj = fixture_class_parent(c={"c": 1, "a": 2})
+    assert repr(base_obj) == "Parent(c={'a': 2, 'c': 1})"
+
+    # Now test when one params values are named object tuples
+    named_objs = [
+        ("step 1", fixture_class_parent()),
+        ("step 2", fixture_class_parent()),
+    ]
+    base_obj = fixture_class_parent(c=named_objs)
+    assert repr(base_obj) == "Parent(c=[('step 1', Parent()), ('step 2', Parent())])"
+
+    # Or when they are just lists of tuples or just tuples as param
+    base_obj = fixture_class_parent(c=[("one", 1), ("two", 2)])
+    assert repr(base_obj) == "Parent(c=[('one', 1), ('two', 2)])"
+
+    base_obj = fixture_class_parent(c=(1, 2, 3))
+    assert repr(base_obj) == "Parent(c=(1, 2, 3))"
 
     simple_composite = fixture_composition_dummy(foo=fixture_class_parent())
     assert repr(simple_composite) == "CompositionDummy(foo=Parent())"
 
     long_base_obj_repr = fixture_class_parent(a=["long_params"] * 1000)
     assert len(repr(long_base_obj_repr)) == 535
 
+    named_objs = [(f"Step {i+1}", Child()) for i in range(25)]
+    base_comp = CompositionDummy(foo=Parent(c=Child(c=named_objs)))
+    assert len(repr(base_comp)) == 1362
+
 
-def test_baseobject_str(fixture_class_parent_instance):
+def test_baseobject_str(fixture_class_parent_instance: Parent):
     """Test BaseObject string representation works."""
-    str(fixture_class_parent_instance)
+    assert (
+        str(fixture_class_parent_instance) == "Parent()"
+    ), "String representation of instance not working."
 
+    # Check that local config works as expected
+    fixture_class_parent_instance.set_config(print_changed_only=False)
+    assert str(fixture_class_parent_instance) == "Parent(a='something', b=7, c=None)"
 
-def test_baseobject_repr_mimebundle_(fixture_class_parent_instance):
+
+def test_baseobject_repr_mimebundle_(fixture_class_parent_instance: Parent):
     """Test display configuration controls output."""
     # Checks the display configuration flag controls the json output
-    with config_context(display="diagram"):
-        output = fixture_class_parent_instance._repr_mimebundle_()
-        assert "text/plain" in output
-        assert "text/html" in output
-
-    with config_context(display="text"):
-        output = fixture_class_parent_instance._repr_mimebundle_()
-        assert "text/plain" in output
-        assert "text/html" not in output
+    fixture_class_parent_instance.set_config(display="diagram")
+    output = fixture_class_parent_instance._repr_mimebundle_()
+    assert "text/plain" in output
+    assert "text/html" in output
+
+    fixture_class_parent_instance.set_config(display="text")
+    output = fixture_class_parent_instance._repr_mimebundle_()
+    assert "text/plain" in output
+    assert "text/html" not in output
 
 
-def test_repr_html_wraps(fixture_class_parent_instance):
+def test_repr_html_wraps(fixture_class_parent_instance: Parent):
     """Test display configuration flag controls the html output."""
-    with config_context(display="diagram"):
-        output = fixture_class_parent_instance._repr_html_()
-        assert "<style>" in output
-
-    with config_context(display="text"):
-        msg = "_repr_html_ is only defined when"
-        with pytest.raises(AttributeError, match=msg):
-            fixture_class_parent_instance._repr_html_()
+    fixture_class_parent_instance.set_config(display="diagram")
+    output = fixture_class_parent_instance._repr_html_()
+    assert "<style>" in output
+
+    fixture_class_parent_instance.set_config(display="text")
+    msg = "_repr_html_ is only defined when"
+    with pytest.raises(AttributeError, match=msg):
+        fixture_class_parent_instance._repr_html_()
 
 
 # Test BaseObject's ability to generate test instances
-def test_get_test_params(fixture_class_parent_instance):
+def test_get_test_params(fixture_class_parent_instance: Parent):
     """Test get_test_params returns empty dictionary."""
     base_obj = fixture_class_parent_instance
     test_params = base_obj.get_test_params()
     assert isinstance(test_params, dict) and len(test_params) == 0
 
 
-def test_get_test_params_raises_error_when_params_required(fixture_required_param):
+def test_get_test_params_raises_error_when_params_required(
+    fixture_required_param: Type[RequiredParam],
+):
     """Test get_test_params raises an error when parameters are required."""
     with pytest.raises(ValueError):
         fixture_required_param(7).get_test_params()
 
 
-def test_create_test_instance(fixture_class_parent, fixture_class_parent_instance):
+def test_create_test_instance(
+    fixture_class_parent: Type[Parent], fixture_class_parent_instance: Parent
+):
     """Test first that create_test_instance logic works."""
     base_obj = fixture_class_parent.create_test_instance()
 
     # Check that init does not construct object of other class than itself
     assert isinstance(base_obj, fixture_class_parent_instance.__class__), (
         "Object returned by create_test_instance must be an instance of the class, "
         f"but found {type(base_obj)}."
@@ -953,60 +1013,82 @@
         f"super({fixture_class_parent.__name__}, self).__init__, "
         "but that does not seem to be the case. Please ensure to call the "
         f"parent class's constructor in {fixture_class_parent.__name__}.__init__"
     )
     assert hasattr(base_obj, "_tags_dynamic"), msg
 
 
-def test_create_test_instances_and_names(fixture_class_parent_instance):
+def test_create_test_instances_and_names(fixture_class_parent_instance: Parent):
     """Test that create_test_instances_and_names works."""
     base_objs, names = fixture_class_parent_instance.create_test_instances_and_names()
 
     assert isinstance(base_objs, list), (
         "First return of create_test_instances_and_names must be a list, "
         f"but found {type(base_objs)}."
     )
     assert isinstance(names, list), (
         "Second return of create_test_instances_and_names must be a list, "
         f"but found {type(names)}."
     )
 
     assert all(
-        [isinstance(est, fixture_class_parent_instance.__class__) for est in base_objs]
+        isinstance(est, fixture_class_parent_instance.__class__) for est in base_objs
     ), (
         "List elements of first return returned by create_test_instances_and_names "
         "all must be an instance of the class"
     )
 
-    assert all([isinstance(name, str) for name in names]), (
+    assert all(isinstance(name, str) for name in names), (
         "List elements of second return returned by create_test_instances_and_names"
         " all must be strings."
     )
 
     assert len(base_objs) == len(names), (
         "The two lists returned by create_test_instances_and_names must have "
         "equal length."
     )
 
 
 # Tests _has_implementation_of interface
 def test_has_implementation_of(
-    fixture_class_parent_instance, fixture_class_child_instance
+    fixture_class_parent_instance: Parent, fixture_class_child_instance: Child
 ):
     """Test _has_implementation_of detects methods in class with overrides in mro."""
     # When the class overrides a parent classes method should return True
     assert fixture_class_child_instance._has_implementation_of("some_method")
     # When class implements method first time it shoudl return False
     assert not fixture_class_child_instance._has_implementation_of("some_other_method")
 
     # If the method is defined the first time in the parent class it should not
     # return _has_implementation_of == True
     assert not fixture_class_parent_instance._has_implementation_of("some_method")
 
 
+class ConfigTester(BaseObject):
+    _config = {"foo_config": 42, "bar": "a"}
+
+    clsvar = 210
+
+    def __init__(self, a, b=42):
+        self.a = a
+        self.b = b
+        self.c = 84
+
+
+class AnotherConfigTester(BaseObject):
+    _config = {"print_changed_only": False, "bar": "a"}
+
+    clsvar = 210
+
+    def __init__(self, a, b=42):
+        self.a = a
+        self.b = b
+        self.c = 84
+
+
 class FittableCompositionDummy(BaseEstimator):
     """Potentially composite object, for testing."""
 
     def __init__(self, foo, bar=84):
         self.foo = foo
         self.foo_ = deepcopy(foo)
         self.bar = bar
```

### Comparing `skbase-0.3.0/skbase/tests/test_baseestimator.py` & `skbase-0.4.0/skbase/tests/test_baseestimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,19 @@
     composite = FittableCompositionDummy(foo=deepcopy(non_composite))
 
     non_composite.fit()
     composite.fit()
 
     non_comp_f_params = non_composite.get_fitted_params()
     comp_f_params = composite.get_fitted_params()
+    comp_f_params_shallow = composite.get_fitted_params(deep=False)
 
     assert isinstance(non_comp_f_params, dict)
     assert set(non_comp_f_params.keys()) == {"foo"}
 
     assert isinstance(comp_f_params, dict)
     assert set(comp_f_params) == {"foo", "foo__foo"}
+    assert set(comp_f_params_shallow) == {"foo"}
     assert comp_f_params["foo"] is composite.foo_
     assert comp_f_params["foo"] is not composite.foo
+    assert comp_f_params_shallow["foo"] is composite.foo_
+    assert comp_f_params_shallow["foo"] is not composite.foo
```

### Comparing `skbase-0.3.0/skbase/tests/test_exceptions.py` & `skbase-0.4.0/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.3.0/skbase.egg-info/PKG-INFO` & `skbase-0.4.0/skbase.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.3.0
+Version: 0.4.0
 Summary: Base classes for sklearn-like parametric objects
-Author: Markus Löning
-Author-email: Franz Király <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
+Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.3.0 is now available. Checkout our
+:rocket: Version 0.4.0 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
@@ -104,15 +103,15 @@
 ### pip
 skbase releases are available as source packages and binary wheels via PyPI
 and can be installed using pip. Checkout the full list of pre-compiled [wheels on PyPi](https://pypi.org/simple/skbase/).
 
 To install the core package use:
 
 ```bash
-pip install skbase
+pip install scikit-base
 ```
 
 or, if you want to install with the maximum set of dependencies, use:
 
 ```bash
-pip install skbase[all_extras]
+pip install scikit-base[all_extras]
 ```
```

### Comparing `skbase-0.3.0/skbase.egg-info/SOURCES.txt` & `skbase-0.4.0/skbase.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 skbase.egg-info/dependency_links.txt
 skbase.egg-info/requires.txt
 skbase.egg-info/top_level.txt
 skbase.egg-info/zip-safe
 skbase/base/__init__.py
 skbase/base/_base.py
 skbase/base/_meta.py
+skbase/base/_tagmanager.py
+skbase/base/_pretty_printing/__init__.py
+skbase/base/_pretty_printing/_object_html_repr.py
+skbase/base/_pretty_printing/_pprint.py
 skbase/lookup/__init__.py
 skbase/lookup/_lookup.py
 skbase/lookup/tests/__init__.py
 skbase/lookup/tests/test_lookup.py
 skbase/testing/__init__.py
 skbase/testing/test_all_objects.py
 skbase/testing/utils/__init__.py
@@ -29,13 +33,26 @@
 skbase/testing/utils/tests/test_check_dependencies.py
 skbase/testing/utils/tests/test_deep_equals.py
 skbase/tests/__init__.py
 skbase/tests/conftest.py
 skbase/tests/test_base.py
 skbase/tests/test_baseestimator.py
 skbase/tests/test_exceptions.py
+skbase/tests/test_meta.py
 skbase/tests/mock_package/__init__.py
 skbase/tests/mock_package/test_mock_package.py
 skbase/utils/__init__.py
+skbase/utils/_check.py
+skbase/utils/_iter.py
 skbase/utils/_nested_iter.py
+skbase/utils/_utils.py
+skbase/utils/tests/__init__.py
+skbase/utils/tests/test_check.py
+skbase/utils/tests/test_iter.py
+skbase/utils/tests/test_nested_iter.py
+skbase/utils/tests/test_utils.py
 skbase/validate/__init__.py
-skbase/validate/_types.py
+skbase/validate/_named_objects.py
+skbase/validate/_types.py
+skbase/validate/tests/__init__.py
+skbase/validate/tests/test_iterable_named_objects.py
+skbase/validate/tests/test_type_validations.py
```

