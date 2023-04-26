# Comparing `tmp/scikit-base-0.3.0.tar.gz` & `tmp/scikit-base-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-base-0.3.0.tar", last modified: Tue Apr 18 19:54:19 2023, max compression
+gzip compressed data, was "scikit-base-0.4.0.tar", last modified: Tue Apr 25 14:56:09 2023, max compression
```

## Comparing `scikit-base-0.3.0.tar` & `scikit-base-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.610609 scikit-base-0.3.0/
--rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     6564 2023-04-18 19:54:19.620849 scikit-base-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3272 2023-01-13 21:26:52.000000 scikit-base-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:18.754893 scikit-base-0.3.0/docs/
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:18.974575 scikit-base-0.3.0/docs/source/
--rw-rw-rw-   0        0        0    10150 2023-04-18 19:51:04.000000 scikit-base-0.3.0/docs/source/conf.py
--rw-rw-rw-   0        0        0     3450 2023-04-18 19:53:32.000000 scikit-base-0.3.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.094162 scikit-base-0.3.0/scikit_base.egg-info/
--rw-rw-rw-   0        0        0     6564 2023-04-18 19:54:18.000000 scikit-base-0.3.0/scikit_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1214 2023-04-18 19:54:18.000000 scikit-base-0.3.0/scikit_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 19:54:18.000000 scikit-base-0.3.0/scikit_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      503 2023-04-18 19:54:18.000000 scikit-base-0.3.0/scikit_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2023-04-18 19:54:18.000000 scikit-base-0.3.0/scikit_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.3.0/scikit_base.egg-info/zip-safe
--rw-rw-rw-   0        0        0      340 2023-04-18 19:54:19.622907 scikit-base-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.127791 scikit-base-0.3.0/skbase/
--rw-rw-rw-   0        0        0      468 2023-01-14 10:36:59.000000 scikit-base-0.3.0/skbase/__init__.py
--rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.3.0/skbase/_exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.164242 scikit-base-0.3.0/skbase/base/
--rw-rw-rw-   0        0        0      610 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/base/__init__.py
--rw-rw-rw-   0        0        0    36286 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/base/_base.py
--rw-rw-rw-   0        0        0    24551 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/base/_meta.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.185525 scikit-base-0.3.0/skbase/lookup/
--rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.3.0/skbase/lookup/__init__.py
--rw-rw-rw-   0        0        0    39804 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/lookup/_lookup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.210354 scikit-base-0.3.0/skbase/lookup/tests/
--rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.3.0/skbase/lookup/tests/__init__.py
--rw-rw-rw-   0        0        0    37960 2022-12-31 19:03:49.000000 scikit-base-0.3.0/skbase/lookup/tests/test_lookup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.218532 scikit-base-0.3.0/skbase/testing/
--rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.3.0/skbase/testing/__init__.py
--rw-rw-rw-   0        0        0    34320 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/testing/test_all_objects.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.346286 scikit-base-0.3.0/skbase/testing/utils/
--rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.3.0/skbase/testing/utils/__init__.py
--rw-rw-rw-   0        0        0     9944 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/testing/utils/_conditional_fixtures.py
--rw-rw-rw-   0        0        0    10545 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/testing/utils/_dependencies.py
--rw-rw-rw-   0        0        0    11159 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/testing/utils/deep_equals.py
--rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.3.0/skbase/testing/utils/inspect.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.384143 scikit-base-0.3.0/skbase/testing/utils/tests/
--rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.3.0/skbase/testing/utils/tests/__init__.py
--rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.3.0/skbase/testing/utils/tests/test_check_dependencies.py
--rw-rw-rw-   0        0        0     1746 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/testing/utils/tests/test_deep_equals.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.503196 scikit-base-0.3.0/skbase/tests/
--rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.3.0/skbase/tests/__init__.py
--rw-rw-rw-   0        0        0     5598 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.547565 scikit-base-0.3.0/skbase/tests/mock_package/
--rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.3.0/skbase/tests/mock_package/__init__.py
--rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.3.0/skbase/tests/mock_package/test_mock_package.py
--rw-rw-rw-   0        0        0    38547 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/tests/test_base.py
--rw-rw-rw-   0        0        0     4620 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/tests/test_baseestimator.py
--rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.3.0/skbase/tests/test_exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.555626 scikit-base-0.3.0/skbase/utils/
--rw-rw-rw-   0        0        0      397 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/utils/__init__.py
--rw-rw-rw-   0        0        0     2505 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/utils/_nested_iter.py
-drwxrwxrwx   0        0        0        0 2023-04-18 19:54:19.608559 scikit-base-0.3.0/skbase/validate/
--rw-rw-rw-   0        0        0      311 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/validate/__init__.py
--rw-rw-rw-   0        0        0     3304 2023-04-18 19:51:04.000000 scikit-base-0.3.0/skbase/validate/_types.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.883999 scikit-base-0.4.0/
+-rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     6574 2023-04-25 14:56:09.885000 scikit-base-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3282 2023-04-25 09:18:57.000000 scikit-base-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:08.480030 scikit-base-0.4.0/docs/
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:08.969212 scikit-base-0.4.0/docs/source/
+-rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3459 2023-04-25 10:03:55.000000 scikit-base-0.4.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.049902 scikit-base-0.4.0/scikit_base.egg-info/
+-rw-rw-rw-   0        0        0     6574 2023-04-25 14:56:08.000000 scikit-base-0.4.0/scikit_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1802 2023-04-25 14:56:08.000000 scikit-base-0.4.0/scikit_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 14:56:08.000000 scikit-base-0.4.0/scikit_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      509 2023-04-25 14:56:08.000000 scikit-base-0.4.0/scikit_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2023-04-25 14:56:08.000000 scikit-base-0.4.0/scikit_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.0/scikit_base.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      368 2023-04-25 14:56:09.896003 scikit-base-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.120416 scikit-base-0.4.0/skbase/
+-rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.0/skbase/__init__.py
+-rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.0/skbase/_exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.187719 scikit-base-0.4.0/skbase/base/
+-rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/base/__init__.py
+-rw-rw-rw-   0        0        0    43391 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/base/_base.py
+-rw-rw-rw-   0        0        0    36390 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/base/_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.301366 scikit-base-0.4.0/skbase/base/_pretty_printing/
+-rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/base/_pretty_printing/__init__.py
+-rw-rw-rw-   0        0        0    11926 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.0/skbase/base/_pretty_printing/_pprint.py
+-rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/base/_tagmanager.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.343368 scikit-base-0.4.0/skbase/lookup/
+-rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.0/skbase/lookup/__init__.py
+-rw-rw-rw-   0        0        0    40100 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/lookup/_lookup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.371889 scikit-base-0.4.0/skbase/lookup/tests/
+-rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.0/skbase/lookup/tests/__init__.py
+-rw-rw-rw-   0        0        0    37960 2022-12-31 19:03:49.000000 scikit-base-0.4.0/skbase/lookup/tests/test_lookup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.397889 scikit-base-0.4.0/skbase/testing/
+-rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.0/skbase/testing/__init__.py
+-rw-rw-rw-   0        0        0    36862 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/testing/test_all_objects.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.487337 scikit-base-0.4.0/skbase/testing/utils/
+-rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.0/skbase/testing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/testing/utils/_conditional_fixtures.py
+-rw-rw-rw-   0        0        0    10612 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/testing/utils/_dependencies.py
+-rw-rw-rw-   0        0        0    11410 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/testing/utils/deep_equals.py
+-rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.0/skbase/testing/utils/inspect.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.533351 scikit-base-0.4.0/skbase/testing/utils/tests/
+-rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.0/skbase/testing/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.0/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-rw-rw-   0        0        0     1779 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/testing/utils/tests/test_deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.663932 scikit-base-0.4.0/skbase/tests/
+-rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.0/skbase/tests/__init__.py
+-rw-rw-rw-   0        0        0     8058 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.693945 scikit-base-0.4.0/skbase/tests/mock_package/
+-rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.0/skbase/tests/mock_package/__init__.py
+-rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.0/skbase/tests/mock_package/test_mock_package.py
+-rw-rw-rw-   0        0        0    41396 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/tests/test_base.py
+-rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/tests/test_baseestimator.py
+-rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.0/skbase/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     4567 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/tests/test_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.750463 scikit-base-0.4.0/skbase/utils/
+-rw-rw-rw-   0        0        0      584 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/_check.py
+-rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/_iter.py
+-rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/_nested_iter.py
+-rw-rw-rw-   0        0        0     3225 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.802470 scikit-base-0.4.0/skbase/utils/tests/
+-rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/tests/test_check.py
+-rw-rw-rw-   0        0        0     5045 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/tests/test_iter.py
+-rw-rw-rw-   0        0        0     2314 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/tests/test_nested_iter.py
+-rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/utils/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.849000 scikit-base-0.4.0/skbase/validate/
+-rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/validate/__init__.py
+-rw-rw-rw-   0        0        0    15327 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/validate/_named_objects.py
+-rw-rw-rw-   0        0        0    12468 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/validate/_types.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:56:09.882000 scikit-base-0.4.0/skbase/validate/tests/
+-rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/validate/tests/__init__.py
+-rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/validate/tests/test_iterable_named_objects.py
+-rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.0/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit-base-0.3.0/LICENSE` & `scikit-base-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-base-0.3.0/PKG-INFO` & `scikit-base-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.3.0
+Version: 0.4.0
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
 
-:rocket: Version 0.3.0 is now available. Checkout our
+:rocket: Version 0.4.0 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
@@ -103,15 +103,15 @@
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

### Comparing `scikit-base-0.3.0/README.md` & `scikit-base-0.4.0/README.md`

 * *Files 2% similar despite different names*

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

### Comparing `scikit-base-0.3.0/docs/source/conf.py` & `scikit-base-0.4.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `scikit-base-0.3.0/pyproject.toml` & `scikit-base-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-base"
-version = "0.3.0"
+version = "0.4.0"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "Franz Király"},
     {name = "Markus Löning"},
     {name = "Ryan Kuhns"},
 ]
 maintainers = [
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

### Comparing `scikit-base-0.3.0/scikit_base.egg-info/PKG-INFO` & `scikit-base-0.4.0/scikit_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.3.0
+Version: 0.4.0
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
 
-:rocket: Version 0.3.0 is now available. Checkout our
+:rocket: Version 0.4.0 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
@@ -103,15 +103,15 @@
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

### Comparing `scikit-base-0.3.0/scikit_base.egg-info/SOURCES.txt` & `scikit-base-0.4.0/scikit_base.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 scikit_base.egg-info/top_level.txt
 scikit_base.egg-info/zip-safe
 skbase/__init__.py
 skbase/_exceptions.py
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

### Comparing `scikit-base-0.3.0/skbase/_exceptions.py` & `scikit-base-0.4.0/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.3.0/skbase/base/__init__.py` & `scikit-base-0.4.0/skbase/base/__init__.py`

 * *Files 12% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/base/_base.py` & `scikit-base-0.4.0/skbase/base/_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,981 +1,871 @@
+#!/usr/bin/env python3 -u
 # -*- coding: utf-8 -*-
 # copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-# Elements of BaseObject re-use code developed in scikit-learn. These elements
-# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
-# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
-"""Base class template for objects and fittable objects.
-
-templates in this module:
-
-    BaseObject - object with parameters and tags
-    BaseEstimator - BaseObject that can be fitted
-
-Interface specifications below.
-
----
-
-    class name: BaseObject
-
-Parameter inspection and setter methods
-    inspect parameter values      - get_params()
-    setting parameter values      - set_params(**params)
-    list of parameter names       - get_param_names()
-    dict of parameter defaults    - get_param_defaults()
-
-Tag inspection and setter methods
-    inspect tags (all)            - get_tags()
-    inspect tags (one tag)        - get_tag(tag_name: str, tag_value_default=None)
-    inspect tags (class method)   - get_class_tags()
-    inspect tags (one tag, class) - get_class_tag(tag_name:str, tag_value_default=None)
-    setting dynamic tags          - set_tag(**tag_dict: dict)
-    set/clone dynamic tags        - clone_tags(estimator, tag_names=None)
-
-Blueprinting: resetting and cloning, post-init state with same hyper-parameters
-    reset estimator to post-init  - reset()
-    cloneestimator (copy&reset)   - clone()
-
-Testing with default parameters methods
-    getting default parameters (all sets)         - get_test_params()
-    get one test instance with default parameters - create_test_instance()
-    get list of all test instances plus name list - create_test_instances_and_names()
----
-
-    class name: BaseEstimator
-
-Provides all interface points of BaseObject, plus:
-
-Parameter inspection:
-    fitted parameter inspection - get_fitted_params()
-
-State:
-    fitted model/strategy   - by convention, any attributes ending in "_"
-    fitted state flag       - is_fitted (property)
-    fitted state check      - check_is_fitted (raises error if not is_fitted)
-"""
-import inspect
-import warnings
-from collections import defaultdict
-from copy import deepcopy
-from typing import List
-
-from sklearn import clone
-from sklearn.base import BaseEstimator as _BaseEstimator
-
-from skbase._exceptions import NotFittedError
-
-__author__: List[str] = ["mloning", "RNKuhns", "fkiraly"]
-__all__: List[str] = ["BaseEstimator", "BaseObject"]
-
-
-class BaseObject(_BaseEstimator):
-    """Base class for parametric objects with sktime style tag interface.
-
-    Extends scikit-learn's BaseEstimator to include sktime style interface for tags.
+# BaseMetaObject and BaseMetaEstimator re-use code developed in scikit-learn and sktime.
+# These elements are copyrighted by the respective
+# scikit-learn developers (BSD-3-Clause License) and sktime (BSD-3-Clause) developers.
+# For conditions see licensing:
+# scikit-learn: https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
+# sktime:  https://github.com/sktime/sktime/blob/main/LICENSE
+"""Implements functionality for meta objects composed of other objects."""
+from inspect import isclass
+from typing import TYPE_CHECKING, Any, Dict, List, Sequence, Tuple, Union, overload
+
+from sklearn.utils._estimator_html_repr import _VisualBlock
+
+from skbase.base._base import BaseEstimator, BaseObject
+from skbase.utils._iter import _format_seq_to_str, make_strings_unique
+from skbase.validate import is_named_object_tuple
+
+__author__: List[str] = ["mloning", "fkiraly", "RNKuhns"]
+__all__: List[str] = ["BaseMetaEstimator", "BaseMetaObject"]
+
+
+class _MetaObjectMixin:
+    """Parameter and tag management for objects composed of named objects.
+
+    Allows objects to get and set nested parameters when a parameter of the the
+    class has values that follow the named object specification. For example,
+    in a pipeline class with the the "step" parameter accepting named objects,
+    this would allow `get_params` and `set_params` to retrieve and update the
+    parameters of the objects in each step.
+
+    Notes
+    -----
+    Partly adapted from sklearn utils.metaestimator.py and sktime's
+    _HeterogenousMetaEstimator.
     """
 
-    def __init__(self):
-        self._tags_dynamic = {}
-        super(BaseObject, self).__init__()
-
-    def __eq__(self, other):
-        """Equality dunder. Checks equal class and parameters.
-
-        Returns True iff result of get_params(deep=False)
-        results in equal parameter sets.
-
-        Nested BaseObject descendants from get_params are compared via __eq__ as well.
-        """
-        from skbase.testing.utils.deep_equals import deep_equals
-
-        if not isinstance(other, BaseObject):
-            return False
-
-        self_params = self.get_params(deep=False)
-        other_params = other.get_params(deep=False)
-
-        return deep_equals(self_params, other_params)
+    # for default get_params/set_params from _HeterogenousMetaEstimator
+    # _steps_attr points to the attribute of self
+    # which contains the heterogeneous set of estimators
+    # this must be an iterable of (name: str, estimator) pairs for the default
+    _tags = {"named_object_parameters": "steps"}
 
-    def reset(self):
-        """Reset the object to a clean post-init state.
+    def is_composite(self) -> bool:
+        """Check if the object is composite.
 
-        Using reset, runs __init__ with current values of hyper-parameters
-        (result of get_params). This Removes any object attributes, except:
-
-            - hyper-parameters = arguments of __init__
-            - object attributes containing double-underscores, i.e., the string "__"
-
-        Class and object methods, and class attributes are also unaffected.
+        A composite object is an object which contains objects as parameter values.
 
         Returns
         -------
-        self
-            Instance of class reset to a clean post-init state but retaining
-            the current hyper-parameter values.
-
-        Notes
-        -----
-        Equivalent to sklearn.clone but overwrites self. After self.reset()
-        call, self is equal in value to `type(self)(**self.get_params(deep=False))`
-        """
-        # retrieve parameters to copy them later
-        params = self.get_params(deep=False)
-
-        # delete all object attributes in self
-        attrs = [attr for attr in dir(self) if "__" not in attr]
-        cls_attrs = list(dir(type(self)))
-        self_attrs = set(attrs).difference(cls_attrs)
-        for attr in self_attrs:
-            delattr(self, attr)
-
-        # run init with a copy of parameters self had at the start
-        self.__init__(**params)
-
-        return self
-
-    def clone(self):
-        """Obtain a clone of the object with same hyper-parameters.
-
-        A clone is a different object without shared references, in post-init state.
-        This function is equivalent to returning sklearn.clone of self.
-
-        Notes
-        -----
-        Also equal in value to `type(self)(**self.get_params(deep=False))`.
+        bool
+            Whether self contains a parameter whose value is a BaseObject,
+            list of (str, BaseObject) tuples or dict[str, BaseObject].
         """
-        return clone(self)
+        # children of this class are always composite
+        return True
 
-    @classmethod
-    def _get_init_signature(cls):
-        """Get class init sigature.
+    def get_params(self, deep: bool = True) -> Dict[str, Any]:
+        """Get a dict of parameters values for this object.
 
-        Useful in parameter inspection.
+        This expands on `get_params` of standard `BaseObject` by also retrieving
+        components parameters when ``deep=True`` a component's follows the named
+        object API (either sequence of str, BaseObject tuples or dict[str, BaseObject]).
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            Whether to return parameters of components.
+
+            - If True, will return a dict of parameter name : value for this object,
+              including parameters of components.
+            - If False, will return a dict of parameter name : value for this object,
+              but not include parameters of components.
+
+        Returns
+        -------
+        dict[str, Any]
+            Dictionary of parameter name and value pairs. Includes direct parameters
+            and indirect parameters whose values implement `get_params` or follow
+            the named object API (either sequence of str, BaseObject tuples or
+            dict[str, BaseObject]).
+
+            - If ``deep=False`` the name-value pairs for this object's direct
+              parameters (you can see these via `get_param_names`) are returned.
+            - If ``deep=True`` then the parameter name-value pairs are returned
+              for direct and component (indirect) parameters.
+
+              - When a BaseObject's direct parameter value implements `get_params`
+                the component parameters are returned as
+                `[direct_param_name]__[component_param_name]` for 1st level components.
+                Arbitrary levels of component recursion are supported (if the
+                component has parameter's whose values are objects that implement
+                `get_params`). In this case, return parameters follow
+                `[direct_param_name]__[component_param_name]__[param_name]` format.
+              - When a BaseObject's direct parameter value is a sequence of
+                (name, BaseObject) tuples or dict[str, BaseObject] the parameters name
+                and value pairs of all component objects are returned. The
+                parameter naming follows ``scikit-learn`` convention of treating
+                named component objects like they are direct parameters; therefore,
+                the names are assigned as `[component_param_name]__[param_name]`.
+        """
+        # Use tag interface that will be available when mixin is used
+        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
+        return self._get_params(named_object_attr, deep=deep)
+
+    def set_params(self, **kwargs):
+        """Set the object's direct parameters and the parameters of components.
+
+        Valid parameter keys can be listed with ``get_params()``.
+
+        Like `BaseObject` implementation it allows values of indirect parameters
+        of a component to be set when a parameter's value is an object that
+        implements `set_params`. This also also expands the functionality to
+        allow parameter to allow the indirect parameters of components to be set
+        when a parameter's values follow the named object API (either sequence
+        of str, BaseObject tuples or dict[str, BaseObject]).
 
         Returns
         -------
-        List
-            The inspected parameter objects (including defaults).
-
-        Raises
-        ------
-        RuntimeError if cls has varargs in __init__.
+        Self
+            Instance of self.
         """
-        # fetch the constructor or the original constructor before
-        # deprecation wrapping if any
-        init = getattr(cls.__init__, "deprecated_original", cls.__init__)
-        if init is object.__init__:
-            # No explicit constructor to introspect
-            return []
-
-        # introspect the constructor arguments to find the model parameters
-        # to represent
-        init_signature = inspect.signature(init)
-
-        # Consider the constructor parameters excluding 'self'
-        parameters = [
-            p
-            for p in init_signature.parameters.values()
-            if p.name != "self" and p.kind != p.VAR_KEYWORD
-        ]
-        for p in parameters:
-            if p.kind == p.VAR_POSITIONAL:
-                raise RuntimeError(
-                    "scikit-learn compatible estimators should always "
-                    "specify their parameters in the signature"
-                    " of their __init__ (no varargs)."
-                    " %s with constructor %s doesn't "
-                    " follow this convention." % (cls, init_signature)
-                )
-        return parameters
+        # Use tag interface that will be available when mixin is used
+        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
+        return self._set_params(named_object_attr, **kwargs)
 
-    @classmethod
-    def get_param_names(cls):
-        """Get object's parameter names.
-
-        Returns
-        -------
-        param_names: list[str]
-            Alphabetically sorted list of parameter names of cls.
-        """
-        parameters = cls._get_init_signature()
-        param_names = sorted([p.name for p in parameters])
-        return param_names
+    def _get_fitted_params(self):
+        """Get fitted parameters.
 
-    @classmethod
-    def get_param_defaults(cls):
-        """Get object's parameter defaults.
+        Method implements logic to retrieve fitted parameters. It is called from
+        get_fitted_params.
 
         Returns
         -------
-        default_dict: dict[str, Any]
-            Keys are all parameters of cls that have a default defined in __init__
-            values are the defaults, as defined in __init__.
+        dict[str, Any]
+            Fitted parameters where keys represent the parameters name (with
+            trailing "_" removed) and the corresponding value is the value of
+            the parameter learned during fit.
         """
-        parameters = cls._get_init_signature()
-        default_dict = {
-            x.name: x.default for x in parameters if x.default != inspect._empty
-        }
-        return default_dict
-
-    def set_params(self, **params):
-        """Set the parameters of this object.
+        fitted_params = self._get_fitted_params_default()
 
-        The method works on simple estimators as well as on nested objects.
-        The latter have parameters of the form ``<component>__<parameter>`` so
-        that it's possible to update each component of a nested object.
+        fitted_named_object_attr = self.get_tag(
+            "fitted_named_object_parameters"
+        )  # type: ignore
 
-        Parameters
-        ----------
-        **params : dict
-            BaseObject parameters.
+        named_objects_fitted_params = self._get_params(
+            fitted_named_object_attr, fitted=True
+        )
 
-        Returns
-        -------
-        self
-            Reference to self (after parameters have been set).
-        """
-        if not params:
-            # Simple optimization to gain speed (inspect is slow)
-            return self
-        valid_params = self.get_params(deep=True)
+        fitted_params.update(named_objects_fitted_params)
 
-        nested_params = defaultdict(dict)  # grouped by prefix
-        for key, value in params.items():
-            key, delim, sub_key = key.partition("__")
-            if key not in valid_params:
-                raise ValueError(
-                    "Invalid parameter %s for object %s. "
-                    "Check the list of available parameters "
-                    "with `object.get_params().keys()`." % (key, self)
-                )
+        return fitted_params
 
-            if delim:
-                nested_params[key][sub_key] = value
-            else:
-                setattr(self, key, value)
-                valid_params[key] = value
+    def _get_params(
+        self, attr: str, deep: bool = True, fitted: bool = False
+    ) -> Dict[str, Any]:
+        """Logic for getting parameters on meta objects/estimators.
 
-        self.reset()
+        Separates out logic for parameter getting on meta objects from public API point.
 
-        # recurse in components
-        for key, sub_params in nested_params.items():
-            valid_params[key].set_params(**sub_params)
+        Parameters
+        ----------
+        attr : str
+            Name of parameter whose values should contain named objects.
+        deep : bool, default=True
+            Whether to return parameters of components.
 
-        return self
+            - If True, will return a dict of parameter name : value for this object,
+              including parameters of components.
+            - If False, will return a dict of parameter name : value for this object,
+              but not include parameters of components.
 
-    @classmethod
-    def get_class_tags(cls):
-        """Get class tags from the class and all its parent classes.
+        fitted : bool, default=False
+            Whether to retrieve the fitted params learned when `fit` is called on
+            ``estimator`` instead of the instances parameters.
 
-        Retrieves tag: value pairs from _tags class attribute. Does not return
-        information from dynamic tags (set via set_tags or clone_tags)
-        that are defined on instances.
+            - If False, then retrieve instance parameters like typical.
+            - If True, the retrieves the parameters learned during "fitting" and
+              stored in attributes ending in "_" (private attributes excluded).
 
         Returns
         -------
-        collected_tags : dict
-            Dictionary of class tag name: tag value pairs. Collected from _tags
-            class attribute via nested inheritance.
+        dict[str, Any]
+            Dictionary of parameter name and value pairs. Includes direct parameters
+            and indirect parameters whose values implement `get_params` or follow
+            the named object API (either sequence of str, BaseObject tuples or
+            dict[str, BaseObject]).
         """
-        collected_tags = {}
+        # Set variables that let us use same code for retrieving params or fitted params
+        if fitted:
+            method = "_get_fitted_params"
+            deepkw = {}
+        else:
+            method = "get_params"
+            deepkw = {"deep": deep}
 
-        # We exclude the last two parent classes: sklearn.base.BaseEstimator and
-        # the basic Python object.
-        for parent_class in reversed(inspect.getmro(cls)[:-2]):
-            if hasattr(parent_class, "_tags"):
-                # Need the if here because mixins might not have _more_tags
-                # but might do redundant work in estimators
-                # (i.e. calling more tags on BaseEstimator multiple times)
-                more_tags = parent_class._tags
-                collected_tags.update(more_tags)
+        # Get the direct params/fitted params
+        out = getattr(super(), method)(**deepkw)
 
-        return deepcopy(collected_tags)
+        if deep and hasattr(self, attr):
+            named_objects = getattr(self, attr)
+            named_objects_ = [
+                (x[0], x[1])
+                for x in self._coerce_to_named_object_tuples(
+                    named_objects, make_unique=False
+                )
+            ]
+            out.update(named_objects_)
+            for name, obj in named_objects_:
+                if hasattr(obj, method):
+                    for key, value in getattr(obj, method)(**deepkw).items():
+                        out["%s__%s" % (name, key)] = value
+        return out
 
-    @classmethod
-    def get_class_tag(cls, tag_name, tag_value_default=None):
-        """Get a class tag's value.
+    def _set_params(self, attr: str, **params):
+        """Logic for setting parameters on meta objects/estimators.
 
-        Does not return information from dynamic tags (set via set_tags or clone_tags)
-        that are defined on instances.
+        Separates out logic for parameter setting on meta objects from public API point.
 
         Parameters
         ----------
-        tag_name : str
-            Name of tag value.
-        tag_value_default : any
-            Default/fallback value if tag is not found.
+        attr : str
+            Name of parameter whose values should contain named objects.
 
         Returns
         -------
-        tag_value :
-            Value of the `tag_name` tag in self. If not found, returns
-            `tag_value_default`.
-        """
-        collected_tags = cls.get_class_tags()
-
-        return collected_tags.get(tag_name, tag_value_default)
-
-    def get_tags(self):
-        """Get tags from estimator class and dynamic tag overrides.
-
-        Returns
-        -------
-        collected_tags : dict
-            Dictionary of tag name : tag value pairs. Collected from _tags
-            class attribute via nested inheritance and then any overrides
-            and new tags from _tags_dynamic object attribute.
+        Self
+            Instance of self.
         """
-        collected_tags = self.get_class_tags()
-
-        if hasattr(self, "_tags_dynamic"):
-            collected_tags.update(self._tags_dynamic)
-
-        return deepcopy(collected_tags)
+        # Ensure strict ordering of parameter setting:
+        # 1. All steps
+        if attr in params:
+            setattr(self, attr, params.pop(attr))
+        # 2. Step replacement
+        items = getattr(self, attr)
+        names = []
+        if items:
+            names, _ = zip(*items)
+        for name in list(params.keys()):
+            if "__" not in name and name in names:
+                self._replace_object(attr, name, params.pop(name))
+        # 3. Step parameters and other initialisation arguments
+        super().set_params(**params)  # type: ignore
+        return self
 
-    def get_tag(self, tag_name, tag_value_default=None, raise_error=True):
-        """Get tag value from estimator class and dynamic tag overrides.
+    def _replace_object(self, attr: str, name: str, new_val: Any) -> None:
+        """Replace an object in attribute that contains named objects."""
+        # assumes `name` is a valid object name
+        new_objects = list(getattr(self, attr))
+        for i, (object_name, _) in enumerate(new_objects):
+            if object_name == name:
+                new_objects[i] = (name, new_val)
+                break
+        setattr(self, attr, new_objects)
+
+    @overload
+    def _check_names(self, names: List[str], make_unique: bool = True) -> List[str]:
+        ...  # pragma: no cover
+
+    @overload
+    def _check_names(
+        self, names: Tuple[str, ...], make_unique: bool = True
+    ) -> Tuple[str, ...]:
+        ...  # pragma: no cover
+
+    def _check_names(
+        self, names: Union[List[str], Tuple[str, ...]], make_unique: bool = True
+    ) -> Union[List[str], Tuple[str, ...]]:
+        """Validate that names of named objects follow API rules.
+
+        The names for named objects should:
+
+        - Be unique,
+        - Not be the name of one of the object's direct parameters,
+        - Not contain "__" (which is reserved to denote components in get/set params).
 
         Parameters
         ----------
-        tag_name : str
-            Name of tag to be retrieved
-        tag_value_default : any type, optional; default=None
-            Default/fallback value if tag is not found
-        raise_error : bool
-            whether a ValueError is raised when the tag is not found
+        names : list[str] | tuple[str]
+            The sequence of names from named objects.
+        make_unique : bool, default=True
+            Whether to coerce names to unique strings if they are not.
 
         Returns
         -------
-        tag_value : Any
-            Value of the `tag_name` tag in self. If not found, returns an error if
-            `raise_error` is True, otherwise it returns `tag_value_default`.
-
-        Raises
-        ------
-        ValueError if raise_error is True i.e. if `tag_name` is not in
-        self.get_tags().keys()
-        """
-        collected_tags = self.get_tags()
-
-        tag_value = collected_tags.get(tag_name, tag_value_default)
+        list[str] | tuple[str]
+            A sequence of unique string names that follow named object API rules.
+        """
+        if len(set(names)) != len(names):
+            raise ValueError("Names provided are not unique: {0!r}".format(list(names)))
+        # Get names that match direct parameter
+        invalid_names = set(names).intersection(self.get_params(deep=False))
+        invalid_names = invalid_names.union({name for name in names if "__" in name})
+        if invalid_names:
+            raise ValueError(
+                "Object names conflict with constructor argument or "
+                "contain '__': {0!r}".format(sorted(invalid_names))
+            )
+        if make_unique:
+            names = make_strings_unique(names)
 
-        if raise_error and tag_name not in collected_tags.keys():
-            raise ValueError(f"Tag with name {tag_name} could not be found.")
+        return names
 
-        return tag_value
+    def _coerce_object_tuple(
+        self,
+        obj: Union[BaseObject, Tuple[str, BaseObject]],
+        clone: bool = False,
+    ) -> Tuple[str, BaseObject]:
+        """Coerce object or (str, BaseObject) tuple to (str, BaseObject) tuple.
 
-    def set_tags(self, **tag_dict):
-        """Set dynamic tags to given values.
+        Used to make sure input will work with expected named object tuple API format.
 
         Parameters
         ----------
-        **tag_dict : dict
-            Dictionary of tag name: tag value pairs.
+        objs : BaseObject or (str, BaseObject) tuple
+            Assumes that this has been checked, no checks are performed.
+        clone : bool, default = False.
+            Whether to return clone of estimator in obj (True) or a reference (False).
 
         Returns
         -------
-        Self
-            Reference to self.
+        tuple[str, BaseObject]
+            Named object tuple.
 
-        Notes
-        -----
-        Changes object state by settting tag values in tag_dict as dynamic tags in self.
+            - If `obj` was an object then returns (obj.__class__.__name__, obj).
+            - If `obj` was aleady a (name, object) tuple it is returned (a copy
+              is returned if ``clone=True``).
         """
-        tag_update = deepcopy(tag_dict)
-        if hasattr(self, "_tags_dynamic"):
-            self._tags_dynamic.update(tag_update)
-        else:
-            self._tags_dynamic = tag_update
+        if isinstance(obj, tuple) and len(obj) >= 2:
+            _obj = obj[1]
+            name = obj[0]
 
-        return self
+        else:
+            if isinstance(obj, tuple) and len(obj) == 1:
+                _obj = obj[0]
+            else:
+                _obj = obj
+            name = type(_obj).__name__
 
-    def clone_tags(self, estimator, tag_names=None):
-        """Clone tags from another estimator as dynamic override.
+        if clone:
+            _obj = _obj.clone()
+        return (name, _obj)
+
+    def _check_objects(
+        self,
+        objs: Any,
+        attr_name: str = "steps",
+        cls_type: Union[type, Tuple[type, ...]] = None,
+        allow_dict: bool = False,
+        allow_mix: bool = True,
+        clone: bool = True,
+    ) -> List[Tuple[str, BaseObject]]:
+        """Check that objects is a list of objects or sequence of named objects.
 
         Parameters
         ----------
-        estimator : estimator inheriting from :class:BaseEstimator
-        tag_names : str or list of str, default = None
-            Names of tags to clone. If None then all tags in estimator are used
-            as `tag_names`.
+        objs : Any
+            Should be list of objects, a list of (str, object) tuples or a
+            dict[str, objects]. Any objects should `cls_type` class.
+        attr_name : str, default="steps"
+            Name of checked attribute in error messages.
+        cls_type : class or tuple of classes, default=BaseEstimator.
+            class(es) that all objects are checked to be an instance of.
+        allow_mix : bool, default=True
+            Whether mix of objects and (str, objects) is allowed in `objs.`
+        clone : bool, default=True
+            Whether objects or named objects in `objs` are returned as clones
+            (True) or references (False).
 
         Returns
         -------
-        Self :
-            Reference to self.
+        list[tuple[str, BaseObject]]
+            List of tuples following named object API.
+
+            - If `objs` was already a list of (str, object) tuples then either the
+              same named objects (as with other cases cloned versions are
+              returned if ``clone=True``).
+            - If `objs` was a dict[str, object] then the named objects are unpacked
+              into a list of (str, object) tuples.
+            - If `objs` was a list of objects then string names were generated based
+               on the object's class names (with coercion to unique strings if
+               necessary).
 
-        Notes
-        -----
-        Changes object state by setting tag values in tag_set from estimator as
-        dynamic tags in self.
-        """
-        tags_est = deepcopy(estimator.get_tags())
+        Raises
+        ------
+        TypeError
+            If `objs` is not a list of (str, object) tuples or a dict[str, objects].
+            Also raised if objects in `objs` are not instances of `cls_type`
+            or `cls_type is not None, a class or tuple of classes.
+        """
+        msg = (
+            f"Invalid {attr_name!r} attribute, {attr_name!r} should be a list "
+            "of objects, or a list of (string, object) tuples. "
+        )
 
-        # if tag_set is not passed, default is all tags in estimator
-        if tag_names is None:
-            tag_names = tags_est.keys()
+        if cls_type is None:
+            cls_type = BaseObject
+            _class_name = "BaseObject"
+        elif isclass(cls_type):
+            _class_name = cls_type.__name__  # type: ignore
+        elif isinstance(cls_type, tuple) and all(isclass(c) for c in cls_type):
+            _class_name = _format_seq_to_str(
+                [c.__name__ for c in cls_type], last_sep="or"
+            )
         else:
-            # if tag_set is passed, intersect keys with tags in estimator
-            if not isinstance(tag_names, list):
-                tag_names = [tag_names]
-            tag_names = [key for key in tag_names if key in tags_est.keys()]
-
-        update_dict = {key: tags_est[key] for key in tag_names}
-
-        self.set_tags(**update_dict)
+            raise TypeError("`cls_type` must be a class or tuple of classes.")
 
-        return self
-
-    @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+        msg += f"All objects in {attr_name!r} must be of type {_class_name}"
 
-        Parameters
-        ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
+        if (
+            objs is None
+            or len(objs) == 0
+            or not (isinstance(objs, list) or (allow_dict and isinstance(objs, dict)))
+        ):
+            raise TypeError(msg)
+
+        def is_obj_is_tuple(obj):
+            """Check whether obj is estimator of right type, or (str, est) tuple."""
+            is_est = isinstance(obj, cls_type)
+            is_tuple = is_named_object_tuple(obj, object_type=cls_type)
+
+            return is_est, is_tuple
+
+        # We've already guarded against objs being dict when allow_dict is False
+        # So here we can just check dictionary elements
+        if isinstance(objs, dict) and not all(
+            isinstance(name, str) and isinstance(obj, cls_type)
+            for name, obj in objs.items()
+        ):
+            raise TypeError(msg)
+
+        elif not all(any(is_obj_is_tuple(x)) for x in objs):
+            raise TypeError(msg)
+
+        msg_no_mix = (
+            f"Elements of {attr_name} must either all be objects, "
+            f"or all (str, objects) tuples. A mix of the two is not allowed."
+        )
+        if not allow_mix and not all(is_obj_is_tuple(x)[0] for x in objs):
+            if not all(is_obj_is_tuple(x)[1] for x in objs):
+                raise TypeError(msg_no_mix)
 
-        Returns
-        -------
-        params : dict or list of dict, default = {}
-            Parameters to create testing instances of the class
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`
-        """
-        # if non-default parameters are required, but none have been found, raise error
-        if hasattr(cls, "_required_parameters"):
-            required_parameters = getattr(cls, "_required_parameters", [])
-            if len(required_parameters) > 0:
-                raise ValueError(
-                    f"Estimator: {cls} requires "
-                    f"non-default parameters for construction, "
-                    f"but none were given. Please set them "
-                    f"as given in the extension template"
-                )
+        return self._coerce_to_named_object_tuples(objs, clone=clone, make_unique=True)
 
-        # construct with parameter configuration for testing, otherwise construct with
-        # default parameters (empty dict)
-        params = {}
-        return params
+    def _get_names_and_objects(
+        self,
+        named_objects: Union[
+            Sequence[Union[BaseObject, Tuple[str, BaseObject]]], Dict[str, BaseObject]
+        ],
+        make_unique: bool = False,
+    ) -> Tuple[List[str], List[BaseObject]]:
+        """Return lists of names and object from input that follows named object API.
 
-    @classmethod
-    def create_test_instance(cls, parameter_set="default"):
-        """Construct Estimator instance if possible.
+        Handles input that is dictionary mapping str names of object instances or
+        input that is a list of (str, object) tuples.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
+        named_objects : list[tuple[str, object], ...], list[object], dict[str, object]
+            The objects whose names should be returned.
+        make_unique : bool, default=False
+            Whether names should be made unique.
 
         Returns
         -------
-        instance : instance of the class with default parameters
-
-        Notes
-        -----
-        `get_test_params` can return dict or list of dict.
-        This function takes first or single dict that get_test_params returns, and
-        constructs the object with that.
+        names : list[str]
+            Lists of the names and objects that were input.
+        objs : list[BaseObject]
+            The
         """
-        if "parameter_set" in inspect.getfullargspec(cls.get_test_params).args:
-            params = cls.get_test_params(parameter_set=parameter_set)
+        names: Tuple[str, ...]
+        objs: Tuple[BaseObject, ...]
+        if isinstance(named_objects, dict):
+            names, objs = zip(*named_objects.items())
         else:
-            params = cls.get_test_params()
-
-        if isinstance(params, list) and isinstance(params[0], dict):
-            params = params[0]
-        elif isinstance(params, dict):
-            pass
-        else:
-            raise TypeError(
-                "get_test_params should either return a dict or list of dict."
-            )
-
-        return cls(**params)
+            names, objs = zip(*[self._coerce_object_tuple(x) for x in named_objects])
 
-    @classmethod
-    def create_test_instances_and_names(cls, parameter_set="default"):
-        """Create list of all test instances and a list of names for them.
+        # Optionally make names unique
+        if make_unique:
+            names = make_strings_unique(names)
+        return list(names), list(objs)
+
+    def _coerce_to_named_object_tuples(
+        self,
+        objs: Union[
+            Sequence[Union[BaseObject, Tuple[str, BaseObject]]], Dict[str, BaseObject]
+        ],
+        clone: bool = False,
+        make_unique: bool = True,
+    ) -> List[Tuple[str, BaseObject]]:
+        """Coerce sequence of objects or named objects to list of (str, obj) tuples.
+
+        Input that is sequence of objects, list of (str, obj) tuples or
+        dict[str, object] will be coerced to list of (str, obj) tuples on return.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
+        objs : list of objects, list of (str, object tuples) or dict[str, object]
+            The input should be coerced to list of (str, object) tuples. Should
+            be a sequence of objects, or follow named object API.
+        clone : bool, default=False.
+            Whether objects in the returned list of (str, object) tuples are
+            cloned (True) or references (False).
+        make_unique : bool, default=True
+            Whether the str names in the returned list of (str, object) tuples
+            should be coerced to unique str values (if str names in input
+            are already unique they will not be changed).
 
         Returns
         -------
-        objs : list of instances of cls
-            i-th instance is cls(**cls.get_test_params()[i])
-        names : list of str, same length as objs
-            i-th element is name of i-th instance of obj in tests
-            convention is {cls.__name__}-{i} if more than one instance
-            otherwise {cls.__name__}
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
+        list[tuple[str, BaseObject]]
+            List of tuples following named object API.
+
+            - If `objs` was already a list of (str, object) tuples then either the
+              same named objects (as with other cases cloned versions are
+              returned if ``clone=True``).
+            - If `objs` was a dict[str, object] then the named objects are unpacked
+              into a list of (str, object) tuples.
+            - If `objs` was a list of objects then string names were generated based
+               on the object's class names (with coercion to unique strings if
+               necessary).
         """
-        if "parameter_set" in inspect.getfullargspec(cls.get_test_params).args:
-            param_list = cls.get_test_params(parameter_set=parameter_set)
+        if isinstance(objs, dict):
+            named_objects = [(k, v) for k, v in objs.items()]
         else:
-            param_list = cls.get_test_params()
-
-        objs = []
-        if not isinstance(param_list, (dict, list)):
-            raise RuntimeError(
-                f"Error in {cls.__name__}.get_test_params, "
-                "return must be param dict for class, or list thereof"
+            # Otherwise get named object format
+            if TYPE_CHECKING:
+                assert not isinstance(objs, dict)  # nosec: B1010
+            named_objects = [
+                self._coerce_object_tuple(obj, clone=clone) for obj in objs
+            ]
+        if make_unique:
+            # Unpack names and objects while making names unique
+            names, objs = self._get_names_and_objects(
+                named_objects, make_unique=make_unique
             )
-        if isinstance(param_list, dict):
-            param_list = [param_list]
-        for params in param_list:
-            if not isinstance(params, dict):
-                raise RuntimeError(
-                    f"Error in {cls.__name__}.get_test_params, "
-                    "return must be param dict for class, or list thereof"
-                )
-            objs += [cls(**params)]
-
-        num_instances = len(param_list)
-        if num_instances > 1:
-            names = [cls.__name__ + "-" + str(i) for i in range(num_instances)]
-        else:
-            names = [cls.__name__]
-
-        return objs, names
-
-    @classmethod
-    def _has_implementation_of(cls, method):
-        """Check if method has a concrete implementation in this class.
-
-        This assumes that having an implementation is equivalent to
-            one or more overrides of `method` in the method resolution order.
+            # Repack the objects
+            named_objects = list(zip(names, objs))
+        return named_objects
+
+    def _dunder_concat(
+        self,
+        other,
+        base_class,
+        composite_class,
+        attr_name="steps",
+        concat_order="left",
+        composite_params=None,
+    ):
+        """Logic to concatenate pipelines for dunder parsing.
+
+        This is useful in concrete heterogeneous meta-objects that implement
+        dunders for easy concatenation of pipeline-like composites.
 
         Parameters
         ----------
-        method : str, name of method to check implementation of
+        other : BaseObject subclass
+            An object inheritting from `composite_class` or `base_class`, otherwise
+            `NotImplemented` is returned.
+        base_class : BaseObject subclass
+            Class assumed as base class for self and `other`. ,
+            and estimator components of composite_class, in case of concatenation
+        composite_class : BaseMetaObject or BaseMetaEstimator subclass
+            Class that has parameter `attr_name` stored in attribute of same name
+            that contains list of base_class objects, list of (str, base_class)
+            tuples, or a mixture thereof.
+        attr_name : str, default="steps"
+            Name of the attribute that contains base_class objects,
+            list of (str, base_class) tuples. Concatenation is done for this attribute.
+        concat_order : {"left", "right"}, default="left"
+            Specifies ordering for concatenation.
+
+            - If "left", resulting attr_name will be like
+              self.attr_name + other.attr_name.
+            - If "right", resulting attr_name will be like
+              other.attr_name + self.attr_name.
+
+        composite_params : dict, default=None
+            Parameters of the composite are always set accordingly
+            i.e., contains key-value pairs, and composite_class has key set to value.
 
         Returns
         -------
-        bool, whether method has implementation in cls
-            True if cls.method has been overridden at least once in
-                the inheritance tree (according to method resolution order)
-        """
-        # walk through method resolution order and inspect methods
-        #   of classes and direct parents, "adjacent" classes in mro
-        mro = inspect.getmro(cls)
-        # collect all methods that are not none
-        methods = [getattr(c, method, None) for c in mro]
-        methods = [m for m in methods if m is not None]
-
-        for i in range(len(methods) - 1):
-            # the method has been overridden once iff
-            #  at least two of the methods collected are not equal
-            #  equivalently: some two adjacent methods are not equal
-            overridden = methods[i] != methods[i + 1]
-            if overridden:
-                return True
-
-        return False
-
-    def is_composite(self):
-        """Check if the object is composed of other BaseObjects.
-
-        A composite object is an object which contains objects, as parameters.
-        Called on an instance, since this may differ by instance.
-
-        Returns
-        -------
-        composite: bool
-            Whether an object has any parameters whose values
-            are BaseObjects.
-        """
-        # walk through method resolution order and inspect methods
-        #   of classes and direct parents, "adjacent" classes in mro
-        params = self.get_params(deep=False)
-        composite = any(isinstance(x, BaseObject) for x in params.values())
-
-        return composite
-
-    def _components(self, base_class=None):
-        """Return references to all state changing BaseObject type attributes.
-
-        This *excludes* the blue-print-like components passed in the __init__.
-
-        Caution: this method returns *references* and not *copies*.
-            Writing to the reference will change the respective attribute of self.
-
-        Parameters
-        ----------
-        base_class : class, optional, default=None, must be subclass of BaseObject
-            if not None, sub-sets return dict to only descendants of base_class
-
-        Returns
-        -------
-        dict with key = attribute name, value = reference to that BaseObject attribute
-        dict contains all attributes of self that inherit from BaseObjects, and:
-            whose names do not contain the string "__", e.g., hidden attributes
-            are not class attributes, and are not hyper-parameters (__init__ args)
-        """
-        if base_class is None:
-            base_class = BaseObject
-        if base_class is not None and not inspect.isclass(base_class):
-            raise TypeError(f"base_class must be a class, but found {type(base_class)}")
-        if base_class is not None and not issubclass(base_class, BaseObject):
-            raise TypeError("base_class must be a subclass of BaseObject")
-
-        # retrieve parameter names to exclude them later
-        param_names = self.get_params(deep=False).keys()
-
-        # retrieve all attributes that are BaseObject descendants
-        attrs = [attr for attr in dir(self) if "__" not in attr]
-        cls_attrs = list(dir(type(self)))
-        self_attrs = set(attrs).difference(cls_attrs).difference(param_names)
+        BaseMetaObject or BaseMetaEstimator
+            Instance of `composite_class`, where `attr_name` is set so that self and
+            other are "concatenated".
+
+            - If other is instance of `composite_class` then instance of
+              `composite_class`, where `attr_name` is a concatenation of
+              ``self.attr_name`` and ``other.attr_name``.
+            - If `other` is instance of `base_class`, then instance of `composite_class`
+              is returned where `attr_name` is set so that so that
+              composite_class(attr_name=other) is returned.
+            - If str are all the class names of est, list of est only is used instead
+        """
+        # Validate input
+        if concat_order not in ["left", "right"]:
+            raise ValueError(
+                f"`concat_order` must be 'left' or 'right', but found {concat_order!r}."
+            )
+        if not isinstance(attr_name, str):
+            raise TypeError(f"`attr_name` must be str, but found {type(attr_name)}.")
+        if not isclass(composite_class):
+            raise TypeError("`composite_class` must be a class.")
+        if not isclass(base_class):
+            raise TypeError("`base_class` must be a class.")
+        if not issubclass(composite_class, base_class):
+            raise ValueError("`composite_class` must be a subclass of base_class.")
+        if not isinstance(self, composite_class):
+            raise TypeError("self must be an instance of `composite_class`.")
+
+        def concat(x, y):
+            if concat_order == "left":
+                return x + y
+            else:
+                return y + x
 
-        comp_dict = {x: getattr(self, x) for x in self_attrs}
-        comp_dict = {x: y for (x, y) in comp_dict.items() if isinstance(y, base_class)}
+        # get attr_name from self and other
+        # can be list of ests, list of (str, est) tuples, or list of mixture of these
+        self_attr = getattr(self, attr_name)
+
+        # from that, obtain ests, and original names (may be non-unique)
+        # we avoid _make_strings_unique call too early to avoid blow-up of string
+        self_names, self_objs = self._get_names_and_objects(self_attr)
+        if isinstance(other, composite_class):
+            other_attr = getattr(other, attr_name)
+            other_names, other_objs = other._get_names_and_objects(other_attr)
+        elif isinstance(other, base_class):
+            other_names = [type(other).__name__]
+            other_objs = [other]
+        elif is_named_object_tuple(other, object_type=base_class):
+            other_names = [other[0]]
+            other_objs = [other[1]]
+        else:
+            return NotImplemented
 
-        return comp_dict
+        new_names = concat(self_names, other_names)
+        new_objs = concat(self_objs, other_objs)
+        # create the "steps" param for the composite
+        # if all the names are equal to class names, we eat them away
+        if all(type(x[1]).__name__ == x[0] for x in zip(new_names, new_objs)):
+            step_param = {attr_name: list(new_objs)}
+        else:
+            step_param = {attr_name: list(zip(new_names, new_objs))}
 
+        # retrieve other parameters, from composite_params attribute
+        if composite_params is None:
+            composite_params = {}
+        else:
+            composite_params = composite_params.copy()
 
-class TagAliaserMixin:
-    """Mixin class for tag aliasing and deprecation of old tags.
+        # construct the composite with both step and additional params
+        composite_params.update(step_param)
+        return composite_class(**composite_params)
+
+    def _sk_visual_block_(self):
+        """Logic to help render meta estimator as visual HTML block."""
+        # Use tag interface that will be available when mixin is used
+        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
+        named_objects = getattr(self, named_object_attr)
+        _, objs = self._get_names_and_objects(named_objects)
+
+        def _get_name(name, obj):
+            if obj is None or obj == "passthrough":
+                return f"{name}: passthrough"
+            # Is an estimator
+            return f"{name}: {obj.__class__.__name__}"
+
+        names = [_get_name(name, est) for name, est in self.steps]
+        name_details = [str(obj) for obj in objs]
+        return _VisualBlock(
+            "serial",
+            objs,
+            names=names,
+            name_details=name_details,
+            dash_wrapped=False,
+        )
 
-    To deprecate tags, add the TagAliaserMixin to BaseObject or BaseEstimator.
-    alias_dict contains the deprecated tags, and supports removal and renaming.
-        For removal, add an entry "old_tag_name": ""
-        For renaming, add an entry "old_tag_name": "new_tag_name"
-    deprecate_dict contains the version number of renaming or removal.
-        the keys in deprecate_dict should be the same as in alias_dict.
-        values in deprecate_dict should be strings, the version of removal/renaming.
 
-    The class will ensure that new tags alias old tags and vice versa, during
-    the deprecation period. Informative warnings will be raised whenever the
-    deprecated tags are being accessed.
+class _MetaTagLogicMixin:
+    """Mixin for tag conjunction, disjunction, chain operations for meta-objects.
 
-    When removing tags, ensure to remove the removed tags from this class.
-    If no tags are deprecated anymore (e.g., all deprecated tags are removed/renamed),
-    ensure toremove this class as a parent of BaseObject or BaseEstimator.
+    Contains methods to set tags of a meta-object dependent on component objects.
     """
 
-    # dictionary of aliases
-    # key = old tag; value = new tag, aliased by old tag
-    # override this in a child class
-    alias_dict = {"old_tag": "new_tag", "tag_to_remove": ""}
-
-    # dictionary of removal version
-    # key = old tag; value = version in which tag will be removed, as string
-    deprecate_dict = {"old_tag": "0.12.0", "tag_to_remove": "99.99.99"}
-
-    def __init__(self):
-        super(TagAliaserMixin, self).__init__()
-
-    @classmethod
-    def get_class_tags(cls):
-        """Get class tags from estimator class and all its parent classes.
-
-        Returns
-        -------
-        collected_tags : dict
-            Dictionary of tag name : tag value pairs. Collected from _tags
-            class attribute via nested inheritance. NOT overridden by dynamic
-            tags set by set_tags or mirror_tags.
-        """
-        collected_tags = super(TagAliaserMixin, cls).get_class_tags()
-        collected_tags = cls._complete_dict(collected_tags)
-        return collected_tags
-
-    @classmethod
-    def get_class_tag(cls, tag_name, tag_value_default=None):
-        """Get tag value from estimator class (only class tags).
+    def _anytagis(self, tag_name, value, estimators):
+        """Return whether any estimator in list has tag `tag_name` of value `value`.
 
         Parameters
         ----------
-        tag_name : str
-            Name of tag value.
-        tag_value_default : any type
-            Default/fallback value if tag is not found.
+        tag_name : str, name of the tag to check
+        value : value of the tag to check for
+        estimators : list of (str, estimator) pairs to query for the tag/value
 
-        Returns
-        -------
-        tag_value :
-            Value of the `tag_name` tag in self. If not found, returns
-            `tag_value_default`.
+        Return
+        ------
+        bool : True iff at least one estimator in the list has value in tag tag_name
         """
-        cls._deprecate_tag_warn([tag_name])
-        return super(TagAliaserMixin, cls).get_class_tag(
-            tag_name=tag_name, tag_value_default=tag_value_default
-        )
+        tagis = [est.get_tag(tag_name, value) == value for _, est in estimators]
+        return any(tagis)
 
-    def get_tags(self):
-        """Get tags from estimator class and dynamic tag overrides.
-
-        Returns
-        -------
-        collected_tags : dict
-            Dictionary of tag name : tag value pairs. Collected from _tags
-            class attribute via nested inheritance and then any overrides
-            and new tags from _tags_dynamic object attribute.
-        """
-        collected_tags = super(TagAliaserMixin, self).get_tags()
-        collected_tags = self._complete_dict(collected_tags)
-        return collected_tags
+    def _anytagis_then_set(self, tag_name, value, value_if_not, estimators):
+        """Set self's `tag_name` tag to `value` if any estimator on the list has it.
 
-    def get_tag(self, tag_name, tag_value_default=None, raise_error=True):
-        """Get tag value from estimator class and dynamic tag overrides.
+        Writes to self:
+        sets the tag `tag_name` to `value` if `_anytagis(tag_name, value)` is True
+            otherwise sets the tag `tag_name` to `value_if_not`
 
         Parameters
         ----------
-        tag_name : str
-            Name of tag to be retrieved
-        tag_value_default : any type, optional; default=None
-            Default/fallback value if tag is not found
-        raise_error : bool
-            whether a ValueError is raised when the tag is not found
-
-        Returns
-        -------
-        tag_value :
-            Value of the `tag_name` tag in self. If not found, returns an error if
-            raise_error is True, otherwise it returns `tag_value_default`.
-
-        Raises
-        ------
-        ValueError if raise_error is True i.e. if tag_name is not in self.get_tags(
-        ).keys()
+        tag_name : str, name of the tag
+        value : value to check and to set tag to if one of the tag values is `value`
+        value_if_not : value to set in self if none of the tag values is `value`
+        estimators : list of (str, estimator) pairs to query for the tag/value
         """
-        self._deprecate_tag_warn([tag_name])
-        return super(TagAliaserMixin, self).get_tag(
-            tag_name=tag_name,
-            tag_value_default=tag_value_default,
-            raise_error=raise_error,
-        )
-
-    def set_tags(self, **tag_dict):
-        """Set dynamic tags to given values.
-
-        Parameters
-        ----------
-        tag_dict : dict
-            Dictionary of tag name : tag value pairs.
-
-        Returns
-        -------
-        Self :
-            Reference to self.
-
-        Notes
-        -----
-        Changes object state by settting tag values in tag_dict as dynamic tags
-        in self.
-        """
-        self._deprecate_tag_warn(tag_dict.keys())
-
-        tag_dict = self._complete_dict(tag_dict)
-        super(TagAliaserMixin, self).set_tags(**tag_dict)
-        return self
+        if self._anytagis(tag_name=tag_name, value=value, estimators=estimators):
+            self.set_tags(**{tag_name: value})
+        else:
+            self.set_tags(**{tag_name: value_if_not})
 
-    @classmethod
-    def _complete_dict(cls, tag_dict):
-        """Add all aliased and aliasing tags to the dictionary."""
-        alias_dict = cls.alias_dict
-        deprecated_tags = set(tag_dict.keys()).intersection(alias_dict.keys())
-        new_tags = set(tag_dict.keys()).intersection(alias_dict.values())
-
-        if len(deprecated_tags) > 0 or len(new_tags) > 0:
-            new_tag_dict = deepcopy(tag_dict)
-            # for all tag strings being set, write the value
-            #   to all tags that could *be aliased by* the string
-            #   and all tags that could be *aliasing* the string
-            # this way we ensure upwards and downwards compatibility
-            for old_tag, new_tag in alias_dict.items():
-                for tag in tag_dict:
-                    if tag == old_tag and new_tag != "":
-                        new_tag_dict[new_tag] = tag_dict[tag]
-                    if tag == new_tag:
-                        new_tag_dict[old_tag] = tag_dict[tag]
-            return new_tag_dict
-        else:
-            return tag_dict
-
-    @classmethod
-    def _deprecate_tag_warn(cls, tags):
-        """Print warning message for tag deprecation.
+    def _anytag_notnone_val(self, tag_name, estimators):
+        """Return first non-'None' value of tag `tag_name` in estimator list.
 
         Parameters
         ----------
-        tags : list of str
+        tag_name : str, name of the tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
 
-        Raises
+        Return
         ------
-        DeprecationWarning for each tag in tags that is aliased by cls.alias_dict
+        tag_val : first non-'None' value of tag `tag_name` in estimator list.
         """
-        for tag_name in tags:
-            if tag_name in cls.alias_dict.keys():
-                version = cls.deprecate_dict[tag_name]
-                new_tag = cls.alias_dict[tag_name]
-                msg = f'tag "{tag_name}" will be removed in sktime version {version}'
-                if new_tag != "":
-                    msg += (
-                        f' and replaced by "{new_tag}", please use "{new_tag}" instead'
-                    )
-                else:
-                    msg += ', please remove code that access or sets "{tag_name}"'
-                warnings.warn(msg, category=DeprecationWarning)
+        for _, est in estimators:
+            tag_val = est.get_tag(tag_name)
+            if tag_val != "None":
+                return tag_val
+        return tag_val
+
+    def _anytag_notnone_set(self, tag_name, estimators):
+        """Set self's `tag_name` tag to first non-'None' value in estimator list.
+
+        Writes to self:
+        tag with name tag_name, sets to _anytag_notnone_val(tag_name, estimators)
+
+        Parameters
+        ----------
+        tag_name : str, name of the tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
+        """
+        tag_val = self._anytag_notnone_val(tag_name=tag_name, estimators=estimators)
+        if tag_val != "None":
+            self.set_tags(**{tag_name: tag_val})
+
+    def _tagchain_is_linked(
+        self,
+        left_tag_name,
+        mid_tag_name,
+        estimators,
+        left_tag_val=True,
+        mid_tag_val=True,
+    ):
+        """Check whether all tags left of the first mid_tag/val are left_tag/val.
+
+        Useful to check, for instance, whether all instances of estimators
+            left of the first missing value imputer can deal with missing values.
+
+        Parameters
+        ----------
+        left_tag_name : str, name of the left tag
+        mid_tag_name : str, name of the middle tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
+        left_tag_val : value of the left tag, optional, default=True
+        mid_tag_val : value of the middle tag, optional, default=True
+
+        Returns
+        -------
+        chain_is_linked : bool,
+            True iff all "left" tag instances `left_tag_name` have value `left_tag_val`
+            a "left" tag instance is an instance in estimators which is earlier
+            than the first occurrence of `mid_tag_name` with value `mid_tag_val`
+        chain_is_complete : bool,
+            True iff chain_is_linked is True, and
+                there is an occurrence of `mid_tag_name` with value `mid_tag_val`
+        """
+        for _, est in estimators:
+            if est.get_tag(mid_tag_name) == mid_tag_val:
+                return True, True
+            if not est.get_tag(left_tag_name) == left_tag_val:
+                return False, False
+        return True, False
+
+    def _tagchain_is_linked_set(
+        self,
+        left_tag_name,
+        mid_tag_name,
+        estimators,
+        left_tag_val=True,
+        mid_tag_val=True,
+        left_tag_val_not=False,
+        mid_tag_val_not=False,
+    ):
+        """Check if _tagchain_is_linked, then set self left_tag_name and mid_tag_name.
+
+        Writes to self:
+        tag with name left_tag_name, sets to left_tag_val if _tag_chain_is_linked[0]
+            otherwise sets to left_tag_val_not
+        tag with name mid_tag_name, sets to mid_tag_val if _tag_chain_is_linked[1]
+            otherwise sets to mid_tag_val_not
+
+        Parameters
+        ----------
+        left_tag_name : str, name of the left tag
+        mid_tag_name : str, name of the middle tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
+        left_tag_val : value of the left tag, optional, default=True
+        mid_tag_val : value of the middle tag, optional, default=True
+        left_tag_val_not : value to set if not linked, optional, default=False
+        mid_tag_val_not : value to set if not linked, optional, default=False
+        """
+        linked, complete = self._tagchain_is_linked(
+            left_tag_name=left_tag_name,
+            mid_tag_name=mid_tag_name,
+            estimators=estimators,
+            left_tag_val=left_tag_val,
+            mid_tag_val=mid_tag_val,
+        )
+        if linked:
+            self.set_tags(**{left_tag_name: left_tag_val})
+        else:
+            self.set_tags(**{left_tag_name: left_tag_val_not})
+        if complete:
+            self.set_tags(**{mid_tag_name: mid_tag_val})
+        else:
+            self.set_tags(**{mid_tag_name: mid_tag_val_not})
 
 
-class BaseEstimator(BaseObject):
-    """Base class for estimators with scikit-learn and sktime design patterns.
+class BaseMetaObject(_MetaObjectMixin, _MetaTagLogicMixin, BaseObject):
+    """Parameter and tag management for objects composed of named objects.
 
-    Extends BaseObject to include basic functionality for fittable estimators.
+    Allows objects to get and set nested parameters when a parameter of the the
+    class has values that follow the named object specification. For example,
+    in a pipeline class with the the "step" parameter accepting named objects,
+    this would allow `get_params` and `set_params` to retrieve and update the
+    parameters of the objects in each step.
+
+    See Also
+    --------
+    BaseMetaEstimator :
+        Expands on `BaseMetaObject` by adding functionality for getting fitted
+        parameters from a class's component estimators. `BaseEstimator` should
+        be used when you want to create a meta estimator.
     """
 
-    # tuple of non-BaseObject classes that count as nested objects
-    # get_fitted_params will retrieve parameters from these, too
-    # override in descendant class - common choice: BaseEstimator from sklearn
-    GET_FITTED_PARAMS_NESTING = ()
-
-    def __init__(self):
-        """Construct BaseEstimator."""
-        self._is_fitted = False
-        super(BaseEstimator, self).__init__()
-
-    @property
-    def is_fitted(self):
-        """Whether `fit` has been called.
-
-        Inspects object's `_is_fitted` attribute that should initialize to False
-        during object construction, and be set to True in calls to an object's
-        `fit` method.
-
-        Returns
-        -------
-        bool
-            Whether the estimator has been `fit`.
-        """
-        return self._is_fitted
-
-    def check_is_fitted(self):
-        """Check if the estimator has been fitted.
-
-        Inspects object's `_is_fitted` attribute that should initialize to False
-        during object construction, and be set to True in calls to an object's
-        `fit` method.
-
-        Raises
-        ------
-        NotFittedError
-            If the estimator has not been fitted yet.
-        """
-        if not self.is_fitted:
-            raise NotFittedError(
-                f"This instance of {self.__class__.__name__} has not been fitted yet. "
-                f"Please call `fit` first."
-            )
-
-    def get_fitted_params(self):
-        """Get fitted parameters.
-
-        State required:
-            Requires state to be "fitted".
-
-        Returns
-        -------
-        fitted_params : dict of fitted parameters, keys are str names of parameters
-            parameters of components are indexed as [componentname]__[paramname]
-        """
-        if not self.is_fitted:
-            raise NotFittedError(
-                f"estimator of type {type(self).__name__} has not been "
-                "fitted yet, please call fit on data before get_fitted_params"
-            )
-
-        fitted_params = {}
-
-        def sh(x):
-            """Shorthand to remove all underscores at end of a string."""
-            if x.endswith("_"):
-                return sh(x[:-1])
-            else:
-                return x
-
-        # add all nested parameters from components that are skbase BaseEstimator
-        c_dict = self._components()
-        for c, comp in c_dict.items():
-            if isinstance(comp, BaseEstimator) and comp._is_fitted:
-                c_f_params = comp.get_fitted_params()
-                c_f_params = {f"{sh(c)}__{k}": v for k, v in c_f_params.items()}
-                fitted_params.update(c_f_params)
-
-        # add non-nested fitted params of self
-        fitted_params.update(self._get_fitted_params())
-
-        # add all nested parameters from components that are sklearn estimators
-        # we do this recursively as we have to reach into nested sklearn estimators
-        any_components_left_to_process = True
-        old_new_params = fitted_params
-        # this loop recursively and iteratively processes components inside components
-        while any_components_left_to_process:
-            new_params = {}
-            for c, comp in old_new_params.items():
-                if isinstance(comp, self.GET_FITTED_PARAMS_NESTING):
-                    c_f_params = self._get_fitted_params_default(comp)
-                    c_f_params = {f"{sh(c)}__{k}": v for k, v in c_f_params.items()}
-                    new_params.update(c_f_params)
-            fitted_params.update(new_params)
-            old_new_params = new_params.copy()
-            n_new_params = len(new_params)
-            any_components_left_to_process = n_new_params > 0
-
-        return fitted_params
-
-    def _get_fitted_params_default(self, obj=None):
-        """Obtain fitted params of object, per sklearn convention.
-
-        Extracts a dict with {paramstr : paramvalue} contents,
-        where paramstr are all string names of "fitted parameters".
-
-        A "fitted attribute" of obj is one that ends in "_" but does not start with "_".
-        "fitted parameters" are names of fitted attributes, minus the "_" at the end.
-
-        Parameters
-        ----------
-        obj : any object, optional, default=self
-
-        Returns
-        -------
-        fitted_params : dict with str keys
-            fitted parameters, keyed by names of fitted parameter
-        """
-        obj = obj if obj else self
-
-        # default retrieves all self attributes ending in "_"
-        # and returns them with keys that have the "_" removed
-        #
-        # get all attributes ending in "_", exclude any that start with "_" (private)
-        fitted_params = [
-            attr for attr in dir(obj) if attr.endswith("_") and not attr.startswith("_")
-        ]
-        # remove the "_" at the end
-        fitted_param_dict = {
-            p[:-1]: getattr(obj, p) for p in fitted_params if hasattr(obj, p)
-        }
-
-        return fitted_param_dict
-
-    def _get_fitted_params(self):
-        """Get fitted parameters.
 
-        private _get_fitted_params, called from get_fitted_params
+class BaseMetaEstimator(_MetaObjectMixin, _MetaTagLogicMixin, BaseEstimator):
+    """Parameter and tag management for estimators composed of named objects.
 
-        State required:
-            Requires state to be "fitted".
-
-        Returns
-        -------
-        fitted_params : dict with str keys
-            fitted parameters, keyed by names of fitted parameter
-        """
-        return self._get_fitted_params_default()
+    Allows estimators to get and set nested parameters when a parameter of the the
+    class has values that follow the named object specification. For example,
+    in a pipeline class with the the "step" parameter accepting named objects,
+    this would allow `get_params` and `set_params` to retrieve and update the
+    parameters of the objects in each step.
+
+    See Also
+    --------
+    BaseMetaObject :
+        Provides similar functionality to  `BaseMetaEstimator` for getting
+        parameters from a class's component objects, but does not have the
+        estimator interface.
+    """
```

### Comparing `scikit-base-0.3.0/skbase/lookup/__init__.py` & `scikit-base-0.4.0/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.3.0/skbase/lookup/_lookup.py` & `scikit-base-0.4.0/skbase/lookup/_lookup.py`

 * *Files 2% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/lookup/tests/test_lookup.py` & `scikit-base-0.4.0/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.3.0/skbase/testing/test_all_objects.py` & `scikit-base-0.4.0/skbase/testing/test_all_objects.py`

 * *Files 3% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/testing/utils/_conditional_fixtures.py` & `scikit-base-0.4.0/skbase/testing/utils/_conditional_fixtures.py`

 * *Files 3% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/testing/utils/_dependencies.py` & `scikit-base-0.4.0/skbase/testing/utils/_dependencies.py`

 * *Files 2% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/testing/utils/deep_equals.py` & `scikit-base-0.4.0/skbase/testing/utils/deep_equals.py`

 * *Files 1% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/testing/utils/inspect.py` & `scikit-base-0.4.0/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.3.0/skbase/testing/utils/tests/test_check_dependencies.py` & `scikit-base-0.4.0/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.3.0/skbase/testing/utils/tests/test_deep_equals.py` & `scikit-base-0.4.0/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files 2% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/tests/mock_package/test_mock_package.py` & `scikit-base-0.4.0/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.3.0/skbase/tests/test_base.py` & `scikit-base-0.4.0/skbase/tests/test_base.py`

 * *Files 4% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/tests/test_baseestimator.py` & `scikit-base-0.4.0/skbase/tests/test_baseestimator.py`

 * *Files 10% similar despite different names*

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

### Comparing `scikit-base-0.3.0/skbase/tests/test_exceptions.py` & `scikit-base-0.4.0/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

