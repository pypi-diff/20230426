# Comparing `tmp/portfolyo-0.4.5.tar.gz` & `tmp/portfolyo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolyo-0.4.5.tar", last modified: Thu Dec 15 15:51:40 2022, max compression
+gzip compressed data, was "portfolyo-0.5.0.tar", last modified: Wed Apr 26 14:45:37 2023, max compression
```

## Comparing `portfolyo-0.4.5.tar` & `portfolyo-0.5.0.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.126409 portfolyo-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2022-12-15 15:51:25.000000 portfolyo-0.4.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-15 15:51:25.000000 portfolyo-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-12-15 15:51:40.130409 portfolyo-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2022-12-15 15:51:25.000000 portfolyo-0.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.130409 portfolyo-0.4.5/portfolyo/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-15 15:51:40.130409 portfolyo-0.4.5/portfolyo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.122409 portfolyo-0.4.5/portfolyo/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/extendpandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.122409 portfolyo-0.4.5/portfolyo/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/mixins/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/mixins/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/mixins/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/ndframelike.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.122409 portfolyo-0.4.5/portfolyo/core/pfline/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/enable_arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/multi_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/single.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfline/single_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.126409 portfolyo-0.4.5/portfolyo/core/pfstate/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfstate/enable_arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfstate/pfstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/pfstate/pfstate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/core/suppresswarnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.126409 portfolyo-0.4.5/portfolyo/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/dev/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/dev/mockup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.126409 portfolyo-0.4.5/portfolyo/prices/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/prices/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/prices/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/prices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.126409 portfolyo-0.4.5/portfolyo/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.126409 portfolyo-0.4.5/portfolyo/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/changefreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/changeyear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/freq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/isboundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/leftandright.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/peakperiod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/right.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/righttoleft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/round.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/standardize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/tzone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/unitdefinitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/tools/wavg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.126409 portfolyo-0.4.5/portfolyo/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15955 2022-12-15 15:51:25.000000 portfolyo-0.4.5/portfolyo/visualize/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 15:51:40.122409 portfolyo-0.4.5/portfolyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-12-15 15:51:40.000000 portfolyo-0.4.5/portfolyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2022-12-15 15:51:40.000000 portfolyo-0.4.5/portfolyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 15:51:40.000000 portfolyo-0.4.5/portfolyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 15:51:39.000000 portfolyo-0.4.5/portfolyo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-15 15:51:40.000000 portfolyo-0.4.5/portfolyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-15 15:51:40.000000 portfolyo-0.4.5/portfolyo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-15 15:51:25.000000 portfolyo-0.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2022-12-15 15:51:40.130409 portfolyo-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2022-12-15 15:51:25.000000 portfolyo-0.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2022-12-15 15:51:25.000000 portfolyo-0.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-26 14:45:18.000000 portfolyo-0.5.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 14:45:18.000000 portfolyo-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-26 14:45:36.997611 portfolyo-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-26 14:45:18.000000 portfolyo-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/extendpandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/ndframelike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/pfline/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/enable_arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/flat_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/nested_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/pfstate/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/enable_arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/pfstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/pfstate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/suppresswarnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/dev/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/dev/mockup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.993611 portfolyo-0.5.0/portfolyo/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.993611 portfolyo-0.5.0/portfolyo/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/changefreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/changeyear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/isboundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/leftandright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/peakperiod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/right.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/righttoleft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/standardize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/tzone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/unitdefinitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/wavg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.985611 portfolyo-0.5.0/portfolyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 14:45:18.000000 portfolyo-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 14:45:36.997611 portfolyo-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 14:45:18.000000 portfolyo-0.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-26 14:45:19.000000 portfolyo-0.5.0/versioneer.py
```

### Comparing `portfolyo-0.4.5/LICENCE` & `portfolyo-0.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/PKG-INFO` & `portfolyo-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.4.5
+Version: 0.5.0
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
 =========
 
 .. image:: https://img.shields.io/pypi/v/portfolyo
    :target: https://pypi.org/project/portfolyo
    :alt: Pypi
 
-.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci.yaml/badge.svg
-   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci.yaml
-   :alt: Github - CI
+.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-pullreq.yaml/badge.svg
+   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-pullreq.yaml
+   :alt: Github - CI (on pullrequest)
+
+.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-push.yaml/badge.svg
+   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-push.yaml
+   :alt: Github - CI (on push)
 
 .. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/pre-commit.yaml/badge.svg
    :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/pre-commit.yaml
    :alt: Github - Pre-commit
 
 .. image:: https://img.shields.io/codecov/c/gh/rwijtvliet/portfolyo
    :target: https://app.codecov.io/gh/rwijtvliet/portfolyo
```

### Comparing `portfolyo-0.4.5/README.rst` & `portfolyo-0.5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 portfolyo
 =========
 
 .. image:: https://img.shields.io/pypi/v/portfolyo
    :target: https://pypi.org/project/portfolyo
    :alt: Pypi
 
-.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci.yaml/badge.svg
-   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci.yaml
-   :alt: Github - CI
+.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-pullreq.yaml/badge.svg
+   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-pullreq.yaml
+   :alt: Github - CI (on pullrequest)
+
+.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-push.yaml/badge.svg
+   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-push.yaml
+   :alt: Github - CI (on push)
 
 .. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/pre-commit.yaml/badge.svg
    :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/pre-commit.yaml
    :alt: Github - Pre-commit
 
 .. image:: https://img.shields.io/codecov/c/gh/rwijtvliet/portfolyo
    :target: https://app.codecov.io/gh/rwijtvliet/portfolyo
```

### Comparing `portfolyo-0.4.5/portfolyo/__init__.py` & `portfolyo-0.5.0/portfolyo/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Package to analyse and manipulate timeseries related to power and gas offtake portfolios."""
 
 
 from . import _version, dev, tools
 from .core import extendpandas  # extend functionalty of pandas
 from .core import suppresswarnings
 from .core.mixins.plot import plot_pfstates
-from .core.pfline import Kind, MultiPfLine, PfLine, SinglePfLine
+from .core.pfline import FlatPfLine, Kind, NestedPfLine, PfLine
 from .core.pfstate import PfState
 from .prices.hedge import hedge
 from .prices.utils import is_peak_hour
 from .tools.changeyear import characterize_index, map_frame_to_year
 from .tools.freq import FREQUENCIES
 from .tools.standardize import frame as standardize
 from .tools.tzone import force_agnostic, force_aware
```

### Comparing `portfolyo-0.4.5/portfolyo/core/mixins/other.py` & `portfolyo-0.5.0/portfolyo/core/mixins/other.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/core/mixins/plot.py` & `portfolyo-0.5.0/portfolyo/core/mixins/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Module with mixins, to add 'plot-functionality' to PfLine and PfState classes.
 """
 
 from __future__ import annotations
 
-from ...visualize import visualize as vis
-from ... import tools
+from typing import TYPE_CHECKING, Dict
 
-from typing import Dict, TYPE_CHECKING
-import numpy as np
 import matplotlib
+import numpy as np
 from matplotlib import pyplot as plt
 
+from ... import tools
+from ... import visualize as vis
+
 if TYPE_CHECKING:  # needed to avoid circular imports
-    from ..pfstate import PfState
     from ..pfline import PfLine
+    from ..pfstate import PfState
 
 
 DEFAULTHOW = {"r": "bar", "q": "bar", "p": "hline", "w": "area", "f": "area"}
 DEFAULTFMT = {
     "w": "{:,.1f}",
     "q": "{:,.0f}",
     "p": "{:,.2f}",
@@ -59,17 +60,17 @@
             The column to plot. One of {'w', 'q', 'p', 'r'}.
         how : str
             How to plot the data. One of {'jagged', 'bar', 'area', 'step', 'hline'}.
         labelfmt : str
             Labels are added to each datapoint in the specified format. ('' to add no labels)
         Any additional kwargs are passed to the pd.Series.plot function.
         """
-        if col not in self.available:
+        if col not in self.kind.available:
             raise ValueError(
-                f"For this PfLine, parameter ``col`` must be one of {', '.join(self.available)}; got {col}."
+                f"For this PfLine, parameter ``col`` must be one of {', '.join(self.kind.available)}; got {col}."
             )
         vis.plot_timeseries(ax, getattr(self, col), how, labelfmt, **kwargs)
 
     def plot(self: PfLine, cols: str = None) -> plt.Figure:
         """Plot one or more timeseries of the PfLine.
 
         Parameters
@@ -86,20 +87,20 @@
         """
         # Plot on category axis if freq monthly or longer, else on time axis.
         is_category = tools.freq.shortest(self.index.freq, "MS") == "MS"
 
         # If columns are specified, plot these. Else: take defaults, based on what's available
         if cols is None:
             cols = ""
-            if "q" in self.available:
+            if "q" in self.kind.available:
                 cols += "q" if is_category else "w"
-            if "p" in self.available:
+            if "p" in self.kind.available:
                 cols += "p"
         else:
-            cols = [col for col in cols if col in self.available]
+            cols = [col for col in cols if col in self.kind.available]
             if not cols:
                 raise ValueError("No columns to plot.")
 
         # Create the plots.
         size = (10, len(cols) * 3)
         fig, axes = plt.subplots(
             len(cols), 1, sharex=True, sharey=False, squeeze=False, figsize=size
```

### Comparing `portfolyo-0.4.5/portfolyo/core/mixins/text.py` & `portfolyo-0.5.0/portfolyo/core/mixins/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,18 @@
         inter = pd.DataFrame([[".."] * len(df.columns)], [".."], df.columns)
         df = pd.concat([df.iloc[:i1], inter, df.iloc[-i2:]])
     return df
 
 
 def _what(pfl: PfLine) -> str:
     return {
-        pfline.Kind.PRICE_ONLY: "price",
-        pfline.Kind.VOLUME_ONLY: "volume",
-        pfline.Kind.ALL: "price and volume",
+        pfline.Kind.VOLUME: "volume",
+        pfline.Kind.PRICE: "price",
+        pfline.Kind.REVENUE: "revenue",
+        pfline.Kind.COMPLETE: "complete",
     }[pfl.kind]
 
 
 def _index_info(i: pd.DatetimeIndex) -> Iterable[str]:
     """Info about the index."""
     return [
         f". Start: {i[0]                    } (incl)    . Timezone    : {i.tz or 'none'}  ",
@@ -114,15 +115,15 @@
     num_of_ts: int,
     depth: int = 0,
     is_last: bool = True,
     is_only: bool = False,
 ) -> Iterable[str]:
     """Treeview of the portfolio line."""
     out = []
-    tree = _treedict(depth, is_last, isinstance(pfl, pfline.MultiPfLine))
+    tree = _treedict(depth, is_last, isinstance(pfl, pfline.NestedPfLine))
     # Name.
     out.append(tree["00"] + tree["01"] + name)
     # Top-level body block.
     if is_only and depth > 0:
         txtlines = ["(only contributor to parent data; has same values)"]
     else:
         txtlines = _flatdatablock(pfl, cols, num_of_ts)
@@ -153,15 +154,15 @@
 
 
 def _childrenlines(
     pfl: PfLine, cols: Iterable[str], num_of_ts: int, depth: int
 ) -> Iterable[str]:
     """Treeview of only the children."""
     out = []
-    if isinstance(pfl, pfline.SinglePfLine):
+    if isinstance(pfl, pfline.FlatPfLine):
         return out
     for c, (name, child) in enumerate(pfl.items()):
         is_last, is_only = (c == len(pfl) - 1), (len(pfl) == 1)
         out.extend(
             _nestedtree(name, child, cols, num_of_ts, depth + 1, is_last, is_only)
         )
     return out
@@ -169,17 +170,17 @@
 
 # Highest-level functions.
 
 
 def pfl_as_string(pfl: PfLine, flatten: bool, num_of_ts: int, color: bool) -> str:
     lines = [f"PfLine object with {_what(pfl)} information."]
     lines.extend(_index_info(pfl.index))
-    if isinstance(pfl, pfline.MultiPfLine):
+    if isinstance(pfl, pfline.NestedPfLine):
         lines.extend(_children_info(pfl))
-    cols = pfl.available
+    cols = pfl.kind.available
     if flatten:
         lines.extend(_dataheader(cols))
         lines.extend([""])
         lines.extend(_flatdatablock(pfl, cols, num_of_ts))
     else:
         spaces = " " * (MAX_DEPTH + 5)
         lines.extend([spaces + txtline for txtline in _dataheader(cols)])
```

### Comparing `portfolyo-0.4.5/portfolyo/core/ndframelike.py` & `portfolyo-0.5.0/portfolyo/core/ndframelike.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/core/pfline/base.py` & `portfolyo-0.5.0/portfolyo/core/pfline/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,74 +11,90 @@
 import pandas as pd
 
 from ... import tools
 from ...prices import convert, hedge
 from ...prices.utils import duration_bpo
 from ..mixins import OtherOutput, PfLinePlot, PfLineText
 
-# from . import single, multi, interop  #<-- moved to end of file
+# from . import flat, multi, interop  #<-- moved to end of file
 from ..ndframelike import NDFrameLike
 
 # Developer notes: we would like to be able to handle 2 cases with volume AND financial
 # information. We would like to...
 # ... handle the situation where, for some timestamp, the volume q == 0 but the revenue
 #   r != 0, because this occasionally arises for the sourced volume, e.g. after buying
 #   and selling the same volume at unequal price. So: we want to be able to store q and r.
 # ... keep price information even if the volume q == 0, because at a later time this price
 #   might still be needed, e.g. if a perfect hedge becomes unperfect. So: we want to be
 #   able to store q and p.
-# Both cases can be catered to. The first as a 'SinglePfLine', where the timeseries for
+# Both cases can be catered to. The first as a 'FlatPfLine', where the timeseries for
 # q and r are used in the instance creation. The price is not defined at the timestamp in
 # the example, but can be calculated for other timestamps, and downsampling is also still
 # possble.
-# The second is a bit more complex. It is possible as a 'MultiPfLine'. This has then 2
-# 'SinglePfLine' instances as its children: one made from each of the timeseries for q
+# The second is a bit more complex. It is possible as a 'NestedPfLine'. This has then 2
+# 'FlatPfLine' instances as its children: one made from each of the timeseries for q
 # and p.
 
 
 if TYPE_CHECKING:
-    from .multi import MultiPfLine  # noqa
-    from .single import SinglePfLine  # noqa
+    from .flat import FlatPfLine  # noqa
+    from .nested import NestedPfLine  # noqa
 
 
 class Kind(Enum):
     """Enumerate what kind of information (which dimensions) is present in a PfLine."""
 
-    VOLUME_ONLY = "vol"
-    PRICE_ONLY = "pri"
-    ALL = "all"
+    # abbreviation, available columns, summable (pfl1 + pfl2) columns
+    VOLUME = "vol", "wq", "q"
+    PRICE = "pri", "p", "p"
+    REVENUE = "rev", "r", "r"
+    COMPLETE = "all", "wqpr", "qr"
+
+    @classmethod
+    def _missing_(cls, val):
+        for member in cls:
+            if member.value[0] == val:
+                return member
+
+    @property
+    def available(self):
+        return tuple(self.value[1])
+
+    @property
+    def summable(self):
+        return tuple(self.value[2])
 
     def __repr__(self):
-        return f"<{self.value}>"
+        return f"<{self.value[0]}>"
 
     def __str__(self):
-        return self.value
+        return self.value[0]
 
 
 class PfLine(NDFrameLike, PfLineText, PfLinePlot, OtherOutput):
-    """Class to hold a related energy timeseries. This can be volume timeseries with q
-    [MWh] and w [MW], a price timeseries with p [Eur/MWh] or both.
+    """Class to hold a related energy timeseries. This can be volume data (with q
+    [MWh] and w [MW]), price data (with p [Eur/MWh]), revenue data (with r [Eur]), or
+    a combination of all.
     """
 
-    def __new__(cls, data):
+    def __new__(cls, data=None):
         if cls is not PfLine:
             # User actually called a descendent class.
             return super().__new__(cls)
 
         # User actually called PfLine().
 
         elif isinstance(data, PfLine):
             # Data is already a valid instance and can directly be used.
             return data
 
         # User called PfLine and data must be processed by a descendent's __init__
 
-        subclasses = [single.SinglePfLine, multi.MultiPfLine]
         errors = {}
-        for subcls in subclasses:
+        for subcls in [flat.FlatPfLine, nested.NestedPfLine]:
             # Try passing data to subclasses to see if they can handle it.
             try:
                 return subcls(data)
             except (ValueError, TypeError, KeyError) as e:
                 errors[subcls] = e
                 pass
         errormsg = "\n".join(f"- {c.__name__}: {e.args[0]}" for c, e in errors.items())
@@ -86,14 +102,20 @@
             f"Cannot create flat or nested PfLine, with the following reasons:\n{errormsg}"
         )
 
     # Additional abstract methods to be implemented by descendents.
 
     @property
     @abstractmethod
+    def kind(self) -> Kind:
+        """Kind of data that is stored in the instance."""
+        ...
+
+    @property
+    @abstractmethod
     def w(self) -> pd.Series:
         """(Flattened) power timeseries in [MW]."""
         ...
 
     @property
     @abstractmethod
     def q(self) -> pd.Series:
@@ -108,23 +130,17 @@
 
     @property
     @abstractmethod
     def r(self) -> pd.Series:
         """(Flattened) revenue timeseries in [Eur]."""
         ...
 
-    @property
-    @abstractmethod
-    def kind(self) -> Kind:
-        """Kind of data that is stored in the instance."""
-        ...
-
     @abstractmethod
     def df(
-        self, cols: Iterable[str], flatten: bool = True, has_units: bool = False
+        self, cols: Iterable[str] = None, flatten: bool = True, has_units: bool = False
     ) -> pd.DataFrame:
         """DataFrame for portfolio line in default units.
 
         Parameters
         ----------
         cols : str, optional (default: all that are available)
             The columns (w, q, p, r) to include in the dataframe.
@@ -139,14 +155,37 @@
 
         Returns
         -------
         pd.DataFrame
         """
         ...
 
+    @property
+    @abstractmethod
+    def volume(self) -> FlatPfLine:
+        """Return (flattened) volume-only PfLine."""
+        ...
+
+    @property
+    @abstractmethod
+    def price(self) -> FlatPfLine:
+        """Return (flattened) price-only PfLine."""
+        ...
+
+    @property
+    @abstractmethod
+    def revenue(self) -> FlatPfLine:
+        """Return (flattened) revenue-only PfLine."""
+        ...
+
+    @abstractmethod
+    def flatten(self) -> FlatPfLine:
+        """Return flat instance, i.e., without children."""
+        ...
+
     @abstractmethod
     def map_to_year(self, year: int, holiday_country: str = None) -> PfLine:
         """Transfer the data to a hypothetical other year.
 
         Parameters
         ----------
         year : int
@@ -175,111 +214,86 @@
     def __bool__(self) -> bool:
         """Return True if object (i.e., its children) contains any non-zero data."""
         ...
 
     # Dunder methods.
 
     @abstractmethod
-    def __setitem__(self, *args, **kwargs):  # Add or overwrite child
-        ...
-
-    @abstractmethod
     def __getitem__(self, *args, **kwargs):  # Get child
         ...
 
-    @abstractmethod
-    def __delitem__(self, *args, **kwargs):  # Remove child
-        ...
-
     # Implemented directly here.
 
-    @property
-    def summable(self) -> str:
-        """Which attributes/colums of this PfLine can be added to those of other PfLines
-        to get consistent/correct new PfLine."""
-        return {Kind.PRICE_ONLY: "p", Kind.VOLUME_ONLY: "q", Kind.ALL: "qr"}[self.kind]
+    # Class should be immutable; remove __setitem__ and __delitem__
+    def __setitem__(self, *args, **kwargs):
+        raise TypeError("PfLine instances are immutable.")
 
-    @property
-    def available(self) -> str:  # which time series have values
-        """Attributes/columns that are available. One of {'wq', 'p', 'wqpr'}."""
-        return {Kind.PRICE_ONLY: "p", Kind.VOLUME_ONLY: "wq", Kind.ALL: "wqpr"}[
-            self.kind
-        ]
-
-    def flatten(self) -> SinglePfLine:
-        """Return flat instance, i.e., without children."""
-        return single.SinglePfLine(self)
-
-    @property
-    def volume(self) -> SinglePfLine:
-        """Return (flattened) volume-only PfLine."""
-        # Design decision: could also be non-flattened.
-        # if isinstance(self, multi.MultiPfLine):
-        #     return multi.MultiPfLine({name: child.volume for name, child in self.items){}})
-        return single.SinglePfLine({"q": self.q})
-
-    @property
-    def price(self) -> SinglePfLine:
-        """Return (flattened) price-only PfLine."""
-        # Design decision: could also be non-flattened if self.kind is not ALL
-        return single.SinglePfLine({"p": self.p})
+    def __delitem__(self, *args, **kwargs):
+        raise TypeError("PfLine instances are immutable.")
 
     def _set_col_val(
         self, col: str, val: Union[pd.Series, float, int, tools.unit.Q_]
-    ) -> SinglePfLine:
+    ) -> FlatPfLine:
         """Set or update a timeseries and return the modified instance."""
 
-        if col == "r" and self.kind is Kind.ALL:
-            raise NotImplementedError(
-                "Cannot set `r` on a price-and-volume portfolio line; first select `.volume`"
-                " or `.price` before applying `.set_r()`."
+        if self.kind is Kind.COMPLETE:
+            raise ValueError(
+                "Cannot set column value when ``.kind`` is Kind.COMPLETE. First select "
+                "the data you wish to keep, e.g. with ``.price``, ``.volume`` or ``.revenue``."
             )
 
-        inop = interop.InOp(**{col: val}).to_timeseries(self.index)
-
-        # Create input data for new (flat) instance.
-        data = {col: getattr(inop, col)}
-        if col in ["w", "q", "r"] and "p" in self.available:
-            data["p"] = self.p
-        elif col in ["p", "r"] and "q" in self.available:
-            data["q"] = self.q
-        return single.SinglePfLine(data)
+        data = {col: s for col, s in self.df(flatten=True).items()}
+        # Ensure volume can be overwritten, by removing conflicting volume information.
+        if col == "q" and "w" in data:
+            del data["w"]
+        elif col == "w" and "q" in data:
+            del data["q"]
+        data[col] = val
+        return flat.FlatPfLine(data)
 
-    def set_w(self, w: Union[pd.Series, float, int, tools.unit.Q_]) -> SinglePfLine:
+    def set_w(self, w: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
         """Set or update power timeseries [MW]; returns modified (and flattened) instance."""
         return self._set_col_val("w", w)
 
-    def set_q(self, q: Union[pd.Series, float, int, tools.unit.Q_]) -> SinglePfLine:
+    def set_q(self, q: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
         """Set or update energy timeseries [MWh]; returns modified (and flattened) instance."""
         return self._set_col_val("q", q)
 
-    def set_p(self, p: Union[pd.Series, float, int, tools.unit.Q_]) -> SinglePfLine:
+    def set_p(self, p: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
         """Set or update price timeseries [Eur/MWh]; returns modified (and flattened) instance."""
         return self._set_col_val("p", p)
 
-    def set_r(self, r: Union[pd.Series, float, int, tools.unit.Q_]) -> SinglePfLine:
+    def set_r(self, r: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
         """Set or update revenue timeseries [MW]; returns modified (and flattened) instance."""
         return self._set_col_val("r", r)
 
-    def set_volume(self, other: PfLine) -> SinglePfLine:
+    def set_volume(self, other: PfLine) -> FlatPfLine:
         """Set or update volume information; returns modified (and flattened) instance."""
-        if not isinstance(other, PfLine) or other.kind is not Kind.VOLUME_ONLY:
+        if not isinstance(other, PfLine) or other.kind is not Kind.VOLUME:
             raise ValueError(
                 "Can only set volume equal to a volume-only PfLine. Use .volume to obtain such a PfLine."
             )
         return self.set_q(other.q)
 
-    def set_price(self, other: PfLine) -> SinglePfLine:
+    def set_price(self, other: PfLine) -> FlatPfLine:
         """Set or update price information; returns modified (and flattened) instance."""
-        if not isinstance(other, PfLine) or other.kind is not Kind.PRICE_ONLY:
+        if not isinstance(other, PfLine) or other.kind is not Kind.PRICE:
             raise ValueError(
                 "Can only set price equal to a price-only PfLine. Use .price to obtain such a PfLine."
             )
         return self.set_p(other.p)
 
+    def set_revenue(self, other: PfLine) -> FlatPfLine:
+        """Set or update revenue information; returns modified (and flattened) instance."""
+        if not isinstance(other, PfLine) or other.kind is not Kind.REVENUE:
+            raise ValueError(
+                "Can only set revenue equal to a revenue-only PfLine. Use .revenue to obtain such a PfLine."
+            )
+        return self.set_r(other.r)
+
     def po(self: PfLine, freq: str = "MS") -> pd.DataFrame:
         """Decompose the portfolio line into peak and offpeak values. Takes simple averages
         of volume [MW] and price [Eur/MWh] - does not hedge!
 
         Parameters
         ----------
         freq : {'MS' (months, default), 'QS' (quarters), 'AS' (years)}
@@ -299,39 +313,39 @@
                 f"Value of paramater ``freq`` must be one of {'MS', 'QS', 'AS'} (got: {freq})."
             )
 
         prods = ("peak", "offpeak")
 
         # Get values.
         dfs = []
-        if "w" in self.available:
+        if "w" in self.kind.available:
             vals = convert.tseries2bpoframe(self.w, freq)
             vals.columns = pd.MultiIndex.from_product([vals.columns, ["w"]])
             dfs.append(vals)
-        if "p" in self.available:
+        if "p" in self.kind.available:
             vals = convert.tseries2bpoframe(self.p, freq)
             vals.columns = pd.MultiIndex.from_product([vals.columns, ["p"]])
             dfs.append(vals)
         df = pd.concat(dfs, axis=1)
 
         # Add duration.
         durs = duration_bpo(df.index)
         durs.columns = pd.MultiIndex.from_product([durs.columns, ["duration"]])
         df = pd.concat([df, durs], axis=1)
 
         # Add additional values and sort.
-        if "q" in self.available:
+        if "q" in self.kind.available:
             for prod in prods:
                 df[(prod, "q")] = df[(prod, "w")] * df[(prod, "duration")]
-        if "r" in self.available:
+        if "r" in self.kind.available:
             for prod in prods:
                 df[(prod, "r")] = (
                     df[(prod, "q")] * df[(prod, "p")]
                 ).pint.to_base_units()
-        i = pd.MultiIndex.from_product([prods, ("duration", *self.available)])
+        i = pd.MultiIndex.from_product([prods, ("duration", *self.kind.available)])
         return df[i]
 
     def hedge_with(
         self: PfLine, p: PfLine, how: str = "val", freq: str = "MS", po: bool = None
     ) -> PfLine:
         """Hedge the volume in the portfolio line with a price curve.
 
@@ -355,15 +369,15 @@
             (or, one volume-price pair for peak, and another volume-price pair for offpeak.)
 
         Notes
         -----
         - If the PfLine contains prices, these are ignored.
         - If ``p`` contains volumes, these are ignored.
         """
-        if self.kind is Kind.PRICE_ONLY:
+        if self.kind is Kind.PRICE:
             raise ValueError(
                 "Cannot hedge a PfLine that does not contain volume information."
             )
         if self.index.freq not in ["15T", "H", "D"]:
             raise ValueError(
                 "Can only hedge a PfLine with daily or (quarter)hourly information."
             )
@@ -375,14 +389,14 @@
             po = self.index.freq in ["15T", "H"]  # default: peak/offpeak if possible
         if po and self.index.freq not in ["15T", "H"]:
             raise ValueError(
                 "Can only hedge with peak and offpeak products if PfLine has (quarter)hourly information."
             )
 
         wout, pout = hedge.hedge(self.w, p.p, how, freq, po)
-        return single.SinglePfLine({"w": wout, "p": pout})
+        return flat.FlatPfLine({"w": wout, "p": pout})
 
 
 # Must be at end, because they depend on PfLine existing.
-from . import enable_arithmatic, interop, multi, single  # noqa
+from . import enable_arithmatic, flat, interop, nested  # noqa
 
 enable_arithmatic.apply()
```

### Comparing `portfolyo-0.4.5/portfolyo/core/pfline/enable_arithmatic.py` & `portfolyo-0.5.0/portfolyo/core/pfline/enable_arithmatic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,22 @@
 """Enable arithmatic with PfLine classes."""
 
 from __future__ import annotations
 
-import warnings
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
 import pandas as pd
 
 from ... import tools
-from . import base, interop, multi, single
+from . import base, flat, interop, nested
 from .base import Kind
 
 if TYPE_CHECKING:  # needed to avoid circular imports
     from .base import PfLine
 
-# Compatibility:
-#
-# General
-#
-# Physically true:
-# unitA + unitA = unitA
-# unitA * dimensionless = unitA
-# unitA / dimensionless = unitA
-# dimensionless / unitA = 1/unitA
-#
-# In addition, accepted as true:
-# unitA + dimension-agnostic = unitA
-# Eur/MWh * MWh -> all-PfLine
-# Eur/MWh * MW -> all-PfLine
-#
-#
-# Implementation
-#
-# Before anything else: turn 'other' into p-PfLine or q-PfLine if possible, or else into
-# a pd.Series. So, if other is single quantity, or pd.Series, in Eur/MWh, MW, or MWh,
-# this is turned into p-PfLine or q-PfLine.
-#                 other
-#                 0 or 0.0 or None                                 => return self
-#                 Eur/MWh                                          => p-PfLine
-#                 MW, MWh                                          => q-PfLine
-#                 other unit or dimensionless                      => pd.Series
-
-
-class PfLineFlattenedWarning(Warning):
-    pass
-
 
 def _assert_index_compatibility(fn):
     """Check if indices are compatible before calling the wrapped function."""
 
     def wrapper(o1, o2):
         if o1.index.freq != o2.index.freq:
             raise NotImplementedError(
@@ -63,167 +31,226 @@
     return wrapper
 
 
 @_assert_index_compatibility
 def _add_pflines(pfl1: PfLine, pfl2: PfLine):
     """Add two pflines."""
     if pfl1.kind is not pfl2.kind:
-        raise NotImplementedError("Cannot add portfolio lines of unequal kind.")
+        raise NotImplementedError(
+            "Cannot add or subtract portfolio lines of unequal kind."
+        )
+    if type(pfl1) is not type(pfl2):  # ONE is NestedPfLine, ONE is FlatPfLine.
+        raise TypeError(
+            "Addition and subtraction only possible for 2 flat, or 2 nested, PfLines."
+        )
 
-    if isinstance(pfl1, multi.MultiPfLine) and isinstance(pfl2, multi.MultiPfLine):
-        # If BOTH are MultiPfLines, collect children and add those with same name.
-        names = set([*[name for name in pfl1], *[name for name in pfl2]])
-        children = {}
-        for name in names:
+    if isinstance(pfl1, nested.NestedPfLine):  # NestedPfLines.
+        # Collect children and add those with same name.
+        new_children = {}
+        for name in set([*pfl1, *pfl2]):
             if name in pfl1 and name in pfl2:
-                children[name] = pfl1[name] + pfl2[name]
+                new_children[name] = pfl1[name] + pfl2[name]
             elif name in pfl1:
-                children[name] = pfl1[name]
+                new_children[name] = pfl1[name]
             else:
-                children[name] = pfl2[name]
-        return multi.MultiPfLine(children)
-
-    elif isinstance(pfl1, multi.MultiPfLine) or isinstance(pfl2, multi.MultiPfLine):
-        # ONE is MultiPfLine, ONE is SinglePfLine.
-        warnings.warn(
-            "When adding a SinglePfLine and MultiPfLine, the MultiPfLine is flattened.",
-            PfLineFlattenedWarning,
-        )
+                new_children[name] = pfl2[name]
+        return nested.NestedPfLine(new_children)
 
-    # At least one of them is a SinglePfLine.
+    # FlatPfLines.
 
-    dfs = [pfl.df(pfl.summable, flatten=True) for pfl in [pfl1, pfl2]]
-    dfs = tools.intersect.frames(*dfs)  # keep only common rows
-    return single.SinglePfLine(sum(dfs))
+    new_df = sum(tools.intersect.frames(pfl1._df, pfl2._df))  # keep only common rows
+    if pfl1.kind is Kind.COMPLETE:
+        new_df["p"] = new_df["r"] / new_df["q"]
+
+    # new_dfs = tools.intersect.frames(pfl1._df, pfl2._df)  # keep only common rows
+    # new_df = sum(new_dfs)
+    # if pfl1.kind is Kind.COMPLETE:
+    #     # Calculate price from wavg instead of r/q, to handle edge case p1==p2, q==0.
+    #     values = pd.DataFrame({"1": new_dfs[0].p, "2": new_dfs[1].p})
+    #     weights = pd.DataFrame({"1": new_dfs[0].q, "2": new_dfs[1].q})
+    #     new_df["p"] = tools.wavg.dataframe(values, weights, axis=1)
+    return flat.FlatPfLine(new_df, _internal=True)
 
 
-# TODO: Decide if this should return a Single or Multi PfLine
 @_assert_index_compatibility
 def _multiply_pflines(pfl1: PfLine, pfl2: PfLine):
     """Multiply two pflines."""
-    if set([pfl1.kind, pfl2.kind]) != {Kind.PRICE_ONLY, Kind.VOLUME_ONLY}:
-        raise NotImplementedError("Can only multiply volume with price information.")
-
-    if isinstance(pfl1, multi.MultiPfLine) or isinstance(pfl2, multi.MultiPfLine):
-        warnings.warn(
-            "PfLine instances are flattened before multiplication.",
-            PfLineFlattenedWarning,
+    if isinstance(pfl1, nested.NestedPfLine) or isinstance(pfl2, nested.NestedPfLine):
+        raise NotImplementedError(
+            "Multiplication only possible between 2 flat PfLines."
         )
 
-    if pfl1.kind is Kind.PRICE_ONLY:
-        data = {"q": pfl2.q, "p": pfl1.p}
-    else:  # pfl1.kind is Kind.VOLUME_ONLY:
-        data = {"q": pfl1.q, "p": pfl2.p}
-    return single.SinglePfLine(data)
+    if set([pfl1.kind, pfl2.kind]) != {Kind.PRICE, Kind.VOLUME}:
+        raise NotImplementedError("Can only multiply volume with price information.")
+
+    if pfl1.kind is Kind.PRICE:
+        series = pfl2.q, pfl1.p
+    else:
+        series = pfl1.q, pfl2.p
+    series = tools.intersect.frames(*series)
+    return flat.FlatPfLine(series[0] * series[1])
 
 
 @_assert_index_compatibility
 def _multiply_pfline_and_dimensionlessseries(pfl: PfLine, s: pd.Series):
     """Multiply pfline and dimensionless series."""
-    # Scale the price p (kind == 'p') or the volume q (kind == 'q'), returning PfLine of same kind.
-    if isinstance(pfl, multi.MultiPfLine):
-        return multi.MultiPfLine({name: child * s for name, child in pfl.items()})
-    df = pfl.df(pfl.summable)
-    df, s = tools.intersect.frames(df, s)  # keep only common rows
-    return single.SinglePfLine(df.mul(s, axis=0))
+
+    if isinstance(pfl, nested.NestedPfLine):  # NestedPfLine
+        return nested.NestedPfLine({name: child * s for name, child in pfl.items()})
+
+    # FlatPfLine.
+
+    s, df = tools.intersect.frames(s, pfl._df)
+    new_df = pd.DataFrame({col: series * s for col, series in df.items()})
+    if pfl.kind is Kind.COMPLETE:  # correction
+        new_df["p"] = new_df["r"] / new_df["q"]
+    return flat.FlatPfLine(new_df, _internal=True)
 
 
 @_assert_index_compatibility
-def _divide_pflines(pfl1: PfLine, pfl2: PfLine) -> pd.Series:
+def _divide_pflines(pfl1: PfLine, pfl2: PfLine) -> Union[pd.Series, PfLine]:
     """Divide two pflines."""
-    if pfl1.kind is not pfl2.kind or pfl1.kind is Kind.ALL:
+
+    if isinstance(pfl1, nested.NestedPfLine) or isinstance(pfl2, nested.NestedPfLine):
+        raise NotImplementedError("Division only possible between 2 flat PfLines.")
+
+    if pfl1.kind is pfl2.kind:
+        if pfl1.kind is Kind.COMPLETE:
+            raise NotImplementedError(
+                "Cannot divide complete PfLines. First select e.g. .volume or .price."
+            )
+        if pfl1.kind is Kind.PRICE:
+            series = pfl1.p, pfl2.p
+        elif pfl1.kind is Kind.VOLUME:
+            series = pfl1.q, pfl2.q
+        elif pfl1.kind is Kind.REVENUE:
+            series = pfl1.r, pfl2.r
+        series = tools.intersect.frames(*series)
+        s = series[0] / series[1]
+        if not len(s):
+            raise ValueError("Data has no overlapping timestamps.")
+        return s.rename("fraction")  # pint[dimensionless]
+
+    # Unequal kind.
+
+    if pfl1.kind is not Kind.REVENUE:
         raise NotImplementedError(
-            "Can only divide portfolio lines if both contain price-only or both contain volume-only information."
+            "To divide PfLines of unequal kind, the numerator must have revenues."
         )
-    if isinstance(pfl1, multi.MultiPfLine) or isinstance(pfl2, multi.MultiPfLine):
-        warnings.warn(
-            "PfLine instances are flattened before division.",
-            PfLineFlattenedWarning,
+    if pfl2.kind is Kind.PRICE:
+        series = pfl1.r, pfl2.p
+    elif pfl2.kind is Kind.VOLUME:
+        series = pfl1.r, pfl2.q
+    else:
+        raise NotImplementedError(
+            "To divide PfLines of unequal kind, the denominator must have volumes or prices."
         )
-
-    if pfl1.kind is Kind.PRICE_ONLY:
-        series = pfl1.p, pfl2.p
-    else:  # self.kind is Kind.VOlUME_ONLY
-        series = pfl1.q, pfl2.q
     series = tools.intersect.frames(*series)
-    s = series[0] / series[1]
-    return s.rename("fraction")  # pint[dimensionless]
+    return flat.FlatPfLine(series[0] / series[1])
+
+
+@_assert_index_compatibility
+def _unite_pflines(pfl1: PfLine, pfl2: PfLine) -> PfLine:
+    """Unite two pflines."""
+
+    if isinstance(pfl1, nested.NestedPfLine) or isinstance(pfl2, nested.NestedPfLine):
+        raise NotImplementedError("Can only do union if both PfLines are flat.")
+
+    kinds = {pfl1.kind: pfl1, pfl2.kind: pfl2}
+    if pfl1.kind is pfl2.kind:
+        raise NotImplementedError("Cannot do union between PfLines of the same kind.")
+    if Kind.COMPLETE in kinds.keys():
+        raise NotImplementedError(
+            "Cannot do union when one of the operands is a complete PfLines. First"
+            " select e.g. .volume or .price."
+        )
+
+    data = {}
+    if (pfl := kinds.get(Kind.VOLUME)) is not None:
+        data["q"] = pfl.q
+    if (pfl := kinds.get(Kind.PRICE)) is not None:
+        data["p"] = pfl.p
+    if (pfl := kinds.get(Kind.REVENUE)) is not None:
+        data["r"] = pfl.r
+    return flat.FlatPfLine(data)
 
 
 class PfLineArithmatic:
-    METHODS = ["neg", "add", "radd", "sub", "rsub", "mul", "rmul", "truediv"]
+    # Write without initial __ to facilitate identification
 
-    def __neg__(self: PfLine):
-        if isinstance(self, multi.MultiPfLine):
-            return multi.MultiPfLine({name: -child for name, child in self.items()})
-
-        # multiply price (kind == 'p'), volume (kind == 'q') or volume and revenue (kind == 'all') with -1
-        # Workaround to make negation work for pint quantity
-        df = (-self.df(self.summable).pint.dequantify()).pint.quantify()
-        return single.SinglePfLine(df)
-
-    def __add__(self: PfLine, other) -> PfLine:
-        # interpret dim-agnostic 'other' as price
-        default = "p" if self.kind is Kind.PRICE_ONLY else None
-        other = interop.pfline_or_nodimseries(other, self.index, default)
+    def neg__(self: PfLine):
+        return self * -1  # defer to mul
 
+    def add__(self: PfLine, other) -> PfLine:
+        other = interop.pfline_or_nodimseries(other, self.index)
         # other is now None, a PfLine, or dimless Series.
-
         if other is None:
             return self
         elif isinstance(other, base.PfLine):
             return _add_pflines(self, other)
         else:
             raise NotImplementedError("This addition is not defined.")
 
-    __radd__ = __add__
-
-    def __sub__(self: PfLine, other):
-        # interpret non-zero, dim-agnostic 'other' as price
-        default = "p" if self.kind is Kind.PRICE_ONLY else None
-        other = interop.pfline_or_nodimseries(other, self.index, default)
+    radd__ = add__
 
+    def sub__(self: PfLine, other):
+        other = interop.pfline_or_nodimseries(other, self.index)
         # other is now None, a PfLine, or dimless Series.
-
         if other is None:
             return self
         elif isinstance(other, base.PfLine):
-            return _add_pflines(self, -other)
+            return _add_pflines(self, -other)  # defer to add and neg
         else:
             raise NotImplementedError("This subtraction is not defined.")
 
-    def __rsub__(self: PfLine, other):
+    def rsub__(self: PfLine, other):
         return -self + other  # defer to add and neg
 
-    def __mul__(self: PfLine, other) -> PfLine:
-        default = "nodim"  # interpret non-zero, dim-agnostic as dimless (i.e., factor)
-        other = interop.pfline_or_nodimseries(other, self.index, default)
-
+    def mul__(self: PfLine, other) -> PfLine:
+        other = interop.pfline_or_nodimseries(other, self.index, "nodim")
         # other is now None, a PfLine, or dimless Series.
-
         if other is None:
             raise NotImplementedError("This multiplication is not defined.")
         elif isinstance(other, base.PfLine):
             return _multiply_pflines(self, other)
         else:
             return _multiply_pfline_and_dimensionlessseries(self, other)
 
-    __rmul__ = __mul__
-
-    def __truediv__(self: PfLine, other):
-        default = "nodim"  # interpret dim-agnostic as dimless (i.e., factor)
-        other = interop.pfline_or_nodimseries(other, self.index, default)
+    rmul__ = mul__
 
+    def truediv__(self: PfLine, other):
+        other = interop.pfline_or_nodimseries(other, self.index, "nodim")
         # other is now None, a PfLine, or dimless Series.
-
         if other is None:
             raise NotImplementedError("This division is not defined.")
         elif isinstance(other, base.PfLine):
             return _divide_pflines(self, other)
         else:
             return self * (1 / other)  # defer to mul
 
+    def rtruediv__(self: PfLine, other):
+        other = interop.pfline_or_nodimseries(other, self.index, "nodim")
+        # other is now None, a PfLine, or dimless Series.
+        if other is None:
+            raise NotImplementedError("This division is not defined.")
+        elif isinstance(other, base.PfLine):
+            return _divide_pflines(other, self)
+        else:
+            raise NotImplementedError("This division is not defined.")
+
+    def or__(self: PfLine, other):
+        other = interop.pfline_or_nodimseries(other, self.index)
+        # other is now None, a PfLine, or dimless Series.
+        if other is None:
+            return self
+        elif isinstance(other, base.PfLine):
+            return _unite_pflines(self, other)
+        else:
+            raise NotImplementedError("This union is not defined.")
+
+    ror__ = or__
+
 
 def apply():
-    for attr in PfLineArithmatic.METHODS:
-        attrname = f"__{attr}__"
-        setattr(base.PfLine, attrname, getattr(PfLineArithmatic, attrname))
+    for attr in dir(PfLineArithmatic):
+        if attr.endswith("__") and not attr.startswith("__"):
+            setattr(base.PfLine, f"__{attr}", getattr(PfLineArithmatic, attr))
```

### Comparing `portfolyo-0.4.5/portfolyo/core/pfline/multi.py` & `portfolyo-0.5.0/portfolyo/core/pfline/nested.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,149 @@
 """
-Module to create multi-pflines. These behave exactly as single-pflines, with all the
+Module to create nested pflines. These behave exactly as flat pflines, with all the
 same methods. But which include several Pflines as children that can be accessed by
 their name.
 """
 
 from __future__ import annotations
 
-from . import multi_helper
-from .base import PfLine, Kind
+from typing import TYPE_CHECKING, Any, Iterable, Mapping, Union
 
-from typing import Dict, Iterable, Mapping, Optional, Union, Any
-import pandas as pd
 import numpy as np
-import warnings
+import pandas as pd
+
+from ... import tools
+from . import flat, nested_helper
+from .base import Kind, PfLine
 
+if TYPE_CHECKING:
+    from .flat import FlatPfLine
 
-class MultiPfLine(PfLine, Mapping):
+
+class NestedPfLine(PfLine, Mapping):
     """Portfolio line with children.
 
     Children's names can be found by looping over the object and accessed by indexing.
     (name, child)-tuples are available from the .items() method.
 
     Parameters
     ----------
     data: Any
         Generally: object with a mapping from strings to PfLine instances; most commonly a
         dictionary.
     """
 
-    def __new__(cls, data):
+    def __new__(cls, data, *args, **kwargs):
         # Catch case where data is already a valid class instance.
-        if isinstance(data, MultiPfLine):
+        if isinstance(data, NestedPfLine):
             return data
         # Otherwise, do normal thing.
-        return super().__new__(cls, data)
+        return super().__new__(cls)
 
-    def __init__(self, data: Union[MultiPfLine, Mapping[str, PfLine], pd.DataFrame]):
+    def __init__(
+        self,
+        data: Union[NestedPfLine, Mapping[str, PfLine], pd.DataFrame],
+        _internal: bool = False,
+    ):
         if self is data:
             return  # don't continue initialisation, it's already the correct object
-        self._children = {}
-        for name, child in multi_helper.make_mapping(data).items():
-            self[name] = child
 
-    # Implementation of ABC methods.
-
-    @property
-    def index(self) -> pd.DatetimeIndex:
-        return next(iter(self._children.values())).index
-
-    @property
-    def w(self) -> pd.Series:
-        if self.kind is Kind.PRICE_ONLY:
-            return pd.Series(np.nan, self.index, name="w", dtype="pint[MW]")
+        if _internal:
+            children = data
         else:
-            return pd.Series(self.q / self.index.duration, name="w").pint.to("MW")
-
-    @property
-    def q(self) -> pd.Series:
-        # TODO: simply flatten and then return volume-part?
-        if self.kind is Kind.PRICE_ONLY:
-            return pd.Series(np.nan, self.index, name="q", dtype="pint[MWh]")
-        elif (qp_children := self._qp_children) is not None:
-            return qp_children[Kind.VOLUME_ONLY].q
-        else:  # all children have a sensible timeseries for .q
-            return sum(child.q for child in self._children.values()).rename("q")
+            children = {
+                name: self._prepare_child(name, child)
+                for name, child in nested_helper.make_mapping(data).items()
+            }
+        self._children, self._kind = nested_helper.children_and_kind(children)
+        self._df = nested_helper.dataframe(self._children, self._kind)
 
-    @property
-    def p(self) -> pd.Series:
-        # TODO: simply flatten and then return price-part?
-        if self.kind is Kind.VOLUME_ONLY:
-            return pd.Series(np.nan, self.index, name="p", dtype="pint[Eur/MWh]")
-        elif (qp_children := self._qp_children) is not None:
-            return qp_children[Kind.PRICE_ONLY].p
-        elif self.kind is Kind.ALL:  # all children have .kind == 'all'
-            return pd.Series(self.r / self.q, name="p").pint.to("Eur/MWh")
-        else:  # self.kind == 'p', all children have a sensible timeseries for .p
-            return sum(child.p for child in self._children.values()).rename("p")
+    # Implementation of ABC methods.
 
-    @property
-    def r(self) -> pd.Series:
-        if self.kind is not Kind.ALL:
-            return pd.Series(np.nan, self.index, name="r", dtype="pint[Eur]")
-        elif (qp_children := self._qp_children) is not None:
-            q, p = qp_children[Kind.VOLUME_ONLY].q, qp_children[Kind.PRICE_ONLY].p
-            return pd.Series(q * p, name="r").pint.to("Eur")
-        else:  # all children have .kind == 'all'
-            return sum(child.r for child in self._children.values()).rename("r")
+    kind: Kind = property(lambda self: self._kind)
+    index: pd.DatetimeIndex = property(lambda self: self._df.index)
 
-    @property
-    def kind(self) -> Kind:
-        if self._heterogeneous_children:
-            return Kind.ALL
-        return next(iter(self._children.values())).kind
+    def _get_series(self, col, unit) -> pd.Series:
+        if col not in self._df.columns:
+            return pd.Series(np.nan, self.index, name=col, dtype=f"pint[{unit}]")
+        return self._df[col]
+
+    w: pd.Series = property(lambda self: self._get_series("w", "MW"))
+    q: pd.Series = property(lambda self: self._get_series("q", "MWh"))
+    p: pd.Series = property(lambda self: self._get_series("p", "Eur/MWh"))
+    r: pd.Series = property(lambda self: self._get_series("r", "Eur"))
 
     def df(
         self,
         cols: Iterable[str] = None,
         flatten: bool = True,
         *arg,
         has_units: bool = True,
         **kwargs,
     ) -> pd.DataFrame:
         if flatten:
-            # TODO: just do self.flatten().df()?
-            cols = self.available if cols is None else cols
-            series = {col: getattr(self, col) for col in cols}
+            if cols is None:
+                cols = self._df.columns
+            series = {col: getattr(self, col) for col in cols if col in "wqpr"}
             if not has_units:
-                series = {key: s.pint.m for key, s in series.items()}
+                series = {col: s.pint.m for col, s in series.items()}
             return pd.DataFrame(series)
 
-        # One big dataframe. First: collect constituent dataframes.
-        dfs = [self.df(cols, True)]
-        dfdicts = [{n: c.df(cols, False)} for n, c in self._children.items()]
-        dfs.extend([pd.concat(dfdict, axis=1) for dfdict in dfdicts])
-        # Then: make all have same number of levels.
-        n_target = max([df.columns.nlevels for df in dfs])
-        for df in dfs:
-            n_current = df.columns.nlevels
-            keys = [""] * (n_target - n_current)
-            oldcol = df.columns if n_current > 1 else [[item] for item in df.columns]
-            df.columns = pd.MultiIndex.from_tuples(((*item, *keys) for item in oldcol))
-        # Finally: put all together in big new dataframe.
-        return pd.concat(dfs, axis=1)
-
-    def asfreq(self, freq: str = "MS") -> MultiPfLine:
-        if self._heterogeneous_children:
-            warnings.warn(
-                "This portfolio has its price and volume information stored in distinct child porfolios."
-                " The portfolio is flattened before changing its frequency."
+        # One big dataframe.
+        dfs = [self.df(cols, flatten=True)]
+        for name, child in self.items():
+            dfs.append(tools.frame.add_header(child.df(cols, flatten=False), name))
+        return tools.frame.concat(dfs, 1)
+
+    @property
+    def volume(self) -> NestedPfLine:
+        if self.kind is Kind.VOLUME:
+            return self
+        if self.kind is Kind.COMPLETE:
+            return NestedPfLine(
+                {name: child.volume for name, child in self.items()}, _internal=True
             )
-            return self.flatten().asfreq(freq)
-        return MultiPfLine(
-            {name: child.asfreq(freq) for name, child in self._children.items()}
+        raise ValueError("This portfolio line doesn't contain volumes.")
+
+    @property
+    def price(self) -> NestedPfLine:
+        if self.kind is Kind.PRICE:
+            return self
+        if self.kind is Kind.COMPLETE:
+            raise ValueError(
+                "This is a complete portfolio line, i.e., that also contains volume "
+                "information. To get its prices, first .flatten() it."
+            )
+        raise ValueError("This portfolio line doesn't contain prices.")
+
+    @property
+    def revenue(self) -> NestedPfLine:
+        if self.kind is Kind.REVENUE:
+            return self
+        if self.kind is Kind.COMPLETE:
+            return NestedPfLine(
+                {name: child.revenue for name, child in self.items()}, _internal=True
+            )
+        raise ValueError("This portfolio line doesn't contain revenues.")
+
+    def flatten(self) -> FlatPfLine:
+        return flat.FlatPfLine(self._df, _internal=True)
+
+    def asfreq(self, freq: str) -> NestedPfLine:
+        return NestedPfLine(
+            {name: child.asfreq(freq) for name, child in self.items()}, _internal=True
         )
 
-    def map_to_year(self, year: int, holiday_country: str) -> MultiPfLine:
-        return MultiPfLine(
+    def map_to_year(self, year: int, holiday_country: str) -> NestedPfLine:
+        return NestedPfLine(
             {
                 name: child.map_to_year(year, holiday_country)
-                for name, child in self._children.items()
-            }
+                for name, child in self.items()
+            },
+            _internal=True,
         )
 
     @property
     def loc(self) -> _LocIndexer:
         return _LocIndexer(self)
 
     def __eq__(self, other) -> bool:
@@ -151,36 +151,45 @@
             return False
         return self._children == other._children
 
     def __bool__(self) -> bool:
         # True if a) has children of which b) any are true
         return any(self._children.keys())
 
-    def __setitem__(self, name: str, pfl: Union[PfLine, Any]):
-        if name in dir(self):  # cannot use hasattr(): runs the code in the properties
+    def _prepare_child(self, name: str, child: Union[PfLine, Any]) -> PfLine:
+        """Assure that name can be used for a child, and that child is PfLine."""
+        if name in dir(self):  # don't use hasattr(): it runs the code in the properties
             raise ValueError(
                 f"Cannot name child '{name}', this is a reserved attribute name."
             )
         if not isinstance(name, str):
             raise TypeError(
                 f"Parameter ``name`` must be a string; got {name} ({type(name)})."
             )
-        self._children = multi_helper.verify_and_trim_dict({**self, name: PfLine(pfl)})
+        if not isinstance(child, PfLine):
+            child = PfLine(child)
+        return child
 
     def __getitem__(self, name: str):
         if name not in self._children:
             raise KeyError(f"Portfolio line does not have child with name '{name}'.")
         return self._children[name]
 
-    def __delitem__(self, name: str):
-        if name not in self._children:
-            raise KeyError(f"Portfolio line does not have child with name '{name}'.")
-        if len(self._children) == 1:
-            raise RuntimeError("Cannot remove the last child of a portfolio line.")
-        del self._children[name]
+    # Class should be immutable; remove __setitem__ and __delitem__
+    # def __setitem__(self, name: str, child: Union[PfLine, Any]):
+    #     children = {**self._children, name: self._prepare_child(name, child)}
+    #     self._children, _ = nested_helper.children_and_kind(children)
+    #     self._df = nested_helper.dataframe(self._children, self._kind)
+    # def __delitem__(self, name: str):
+    #     if name not in self._children:
+    #         raise KeyError(f"Portfolio line does not have child with name '{name}'.")
+    #     if len(self._children) == 1:
+    #         raise RuntimeError("Cannot remove the last child of a portfolio line.")
+    #     del self._children[name]
+    #     self._df = nested_helper.dataframe(self._children, self._kind)
 
     # Additional methods, unique to this class.
 
     # . Iterate over children.
 
     def items(self):
         """Iterate over children in (name, child)-tuples."""
@@ -197,45 +206,33 @@
     def __getattr__(self, name):
         if name not in self._children:
             raise AttributeError(f"No such attribute '{name}'.")
         return self._children[name]
 
     # . Add and remove not-inplace.
 
-    def set_child(self, name: str, pfl: Union[PfLine, Any]) -> PfLine:
+    def set_child(self, name: str, child: Union[PfLine, Any]) -> PfLine:
         """Sets/adds/updates child; returns new pfline instance without changing current instance."""
-        return MultiPfLine({**self, name: pfl})
+        return NestedPfLine(
+            {**self, name: self._prepare_child(name, child)}, _internal=True
+        )
 
     def drop_child(self, name: str) -> PfLine:
         """Drop child; returns new pfline instance without changing current instance."""
         if name not in self._children:
             raise KeyError(f"Portfolio line does not have child with name '{name}'.")
         if len(self._children) == 1:
             raise RuntimeError("Cannot remove the last child of a portfolio line.")
-        return MultiPfLine({n: child for n, child in self.items() if n != name})
-
-    # . Other.
-
-    @property
-    def _heterogeneous_children(self) -> bool:
-        """Return True if children are not all of same kind."""
-        return bool(self._qp_children)
-
-    @property
-    def _qp_children(self) -> Optional[Dict[Kind, PfLine]]:
-        """Helper method that returns the child providing the volume and the one providing the price."""
-        qp_children = {child.kind: child for child in self._children.values()}
-        if Kind.VOLUME_ONLY in qp_children and Kind.PRICE_ONLY in qp_children:
-            return qp_children
-        else:
-            return None
+        return NestedPfLine(
+            {n: child for n, child in self.items() if n != name}, _internal=True
+        )
 
 
 class _LocIndexer:
-    """Helper class to obtain MultiPfLine instance, whose index is subset of original index."""
+    """Helper class to obtain NestedPfLine instance, whose index is subset of original index."""
 
-    def __init__(self, mpfl):
-        self.mpfl = mpfl
+    def __init__(self, pfl: NestedPfLine):
+        self.pfl = pfl
 
-    def __getitem__(self, arg) -> MultiPfLine:
-        new_dict = {name: child.loc[arg] for name, child in self.mpfl.items()}
-        return MultiPfLine(new_dict)
+    def __getitem__(self, arg) -> NestedPfLine:
+        new_children = {name: child.loc[arg] for name, child in self.pfl.items()}
+        return NestedPfLine(new_children, _internal=True)
```

### Comparing `portfolyo-0.4.5/portfolyo/core/pfline/multi_helper.py` & `portfolyo-0.5.0/portfolyo/core/pfline/nested_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""Verify input data and turn into object needed in MultiPfLine instantiation."""
+"""Verify input data and turn into object needed in NestedPfLine instantiation."""
 
 from __future__ import annotations
 
-from typing import Any, Counter, Dict, Mapping
+from typing import Any, Dict, Mapping, Tuple
 
 import pandas as pd
 
 from ... import tools
 from .base import Kind, PfLine
 
 
 def make_mapping(data: Any) -> Mapping[Any, Any]:
     """From data, create a mapping."""
+    # Shortcut if PfLine is passed.
 
     if isinstance(data, Mapping):
         return data
 
     elif isinstance(data, pd.DataFrame):
         children = {}
         # Get all sub-dataframes (or series) and turn into dictionary.
@@ -24,72 +25,34 @@
         return children
 
     raise TypeError(
         f"Parameter ``data`` must be dict (or other Mapping) or pandas.DataFrame; got {type(data)}."
     )
 
 
-def verify_and_trim_dict(children: Dict[str, PfLine]) -> Dict[str, PfLine]:
-    """Do data checks on dictionary of children so that they fit well together."""
-    # Data check.
-    try:
-        _assert_pfline_kindcompatibility(children)
-    except AssertionError as e:
-        raise ValueError("The data is not suitable for creating a MultiPfLine.") from e
-    # Trim.
-    children = _intersect_indices(children)
-    return children
-
-
-def _assert_pfline_kindcompatibility(children: Dict) -> None:
-    """Check pflines in dictionary, and raise error if their kind is not compatible."""
-
+def children_and_kind(children: Dict[str, PfLine]) -> Tuple[Dict[str, PfLine], Kind]:
+    """Check number, kind, and indices of children; return corrected children and kind."""
+    # Number of children.
     if len(children) == 0:
-        raise AssertionError("Must provide at least 1 child.")
-
-    if len(children) == 1:
-        return  # No possible compatibility errors if only 1 child.
-
-    # Check kind.
-
-    kindcounter = Counter(child.kind for child in children.values())
-
-    if len(kindcounter) == 1:
-        return  # No compatibility error if all children of same kind.
-
-    if (
-        kindcounter[Kind.VOLUME_ONLY] == kindcounter[Kind.PRICE_ONLY] == 1
-        and kindcounter[Kind.ALL] == 0
-    ):
-        return  # Children of distinct can only be combined in this exact setting.
-
-    raise AssertionError(
-        "All children must be of the same kind, or there must be exactly one volume-only "
-        "child and one price-only child."
-    )
-
-
-def _intersect_indices(children: Dict[str, PfLine]) -> Dict[str, PfLine]:
-    """Keep only the overlapping part of each PfLine's index."""
-
-    if len(children) < 2:
-        return children  # No index errors if only 1 child.
-
-    indices = [child.index for child in children.values()]
-
-    # Check frequency.
-
-    freqs = set([i.freq for i in indices])
-    if len(freqs) != 1:
-        raise ValueError(
-            f"PfLines have unequal frequencies; found {', '.join(str(f) for f in freqs)}."
-            " Resample first to obtain equal frequencies."
-        )
-
-    # Check/fix indices.
-    # Workaround for error in pandas intersection (#46702):
-    idx = tools.intersect.indices(*indices)
+        raise ValueError("Must provide at least 1 child.")
+    # Keep only overlapping part of indices.
+    idx = tools.intersect.indices(*[child.index for child in children.values()])
     if len(idx) == 0:
-        raise ValueError("PfLine indices describe non-overlapping periods.")
-
+        raise ValueError("PfLine indices have no overlap.")
     children = {name: child.loc[idx] for name, child in children.items()}
-    return children
+
+    # Kind of children.
+    kindset = set([child.kind for child in children.values()])
+    if len(kindset) != 1:
+        raise ValueError(f"All children must be of the same kind; found {kindset}.")
+    kind = next(iter(kindset))
+
+    return children, kind
+
+
+def dataframe(children: Dict[str, PfLine], kind: Kind) -> pd.DataFrame:
+    """Create dataframe with aggregated values."""
+    # All children have same kind, so same columns. Also, same indices, so same index.
+    df = sum(child._df for child in children.values())
+    if kind is Kind.COMPLETE:
+        df["p"] = df["r"] / df["q"]
+    return df
```

### Comparing `portfolyo-0.4.5/portfolyo/core/pfstate/enable_arithmatic.py` & `portfolyo-0.5.0/portfolyo/core/pfstate/enable_arithmatic.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             name = tools.unit.to_name(value.pint.units)
         except ValueError:
             return value  # has unit, but unknown
 
         if name not in ["p", "q", "w"]:
             return value  # has know unit, but none from which PfLine can be made
 
-        return pfline.SinglePfLine({name: value})
+        return pfline.FlatPfLine({name: value})
 
     # Just a single value.
     if isinstance(value, int) or isinstance(value, float):
         s = pd.Series(value, refindex)
         return _prep_data(s, refindex)
     elif isinstance(value, tools.unit.Q_):
         s = pd.Series(value.magnitude, refindex, dtype=f"pint[{value.units:P}]")
@@ -64,15 +64,17 @@
     values = pd.DataFrame({"s": pfs1.unsourcedprice.p, "o": pfs2.unsourcedprice.p})
     weights = pd.DataFrame({"s": pfs1.unsourced.q, "o": pfs2.unsourced.q})
     unsourcedprice = pfline.PfLine({"p": tools.wavg.dataframe(values, weights, axis=1)})
 
     return pfstate.PfState(offtakevolume, unsourcedprice, sourced)
 
 
-def _multiply_pfstate_and_series(pfs: pfstate.PfState, s: pd.Series) -> pfstate.PfState:
+def _nestedply_pfstate_and_series(
+    pfs: pfstate.PfState, s: pd.Series
+) -> pfstate.PfState:
     """Multiply pfstate and Series."""
     # Scale up volumes (and revenues), leave prices unchanged.
     return pfstate.PfState(pfs.offtakevolume * s, pfs.unsourcedprice, pfs.sourced * s)
 
 
 def _divide_pfstates(pfs1: pfstate.PfState, pfs2: pfstate.PfState) -> pd.DataFrame:
     """Divide two pfstates."""
@@ -81,16 +83,16 @@
         ("offtake", "volume"),
         ("sourced", "volume"),
         ("sourced", "price"),
         ("unsourced", "volume"),
         ("unsourcedprice", "price"),
         ("pnl_cost", "price"),
     ]:
-        pfl1 = getattr(getattr(pfs1, top), bottom)
-        pfl2 = getattr(getattr(pfs2, top), bottom)
+        pfl1 = getattr(getattr(pfs1, top).flatten(), bottom)
+        pfl2 = getattr(getattr(pfs2, top).flatten(), bottom)
         top = top.replace("unsourcedprice", "unsourced")
         series[(top, bottom)] = pfl1 / pfl2
     return pd.DataFrame(series)
 
 
 def _assert_index_compatibility(o1, o2):
     if o1.index.freq != o2.index.freq:
@@ -135,17 +137,17 @@
     def __mul__(self: PfState, other):
 
         other = _prep_data(other, self.index)  # other is now PfState, PfLine, or Series
         _assert_index_compatibility(self, other)
 
         # Other is a Series (but not containing [power], [energy] or [price]).
         if isinstance(other, pd.Series):
-            return _multiply_pfstate_and_series(self, other)
+            return _nestedply_pfstate_and_series(self, other)
 
-        raise NotImplementedError("This multiplication is not defined.")
+        raise NotImplementedError("This nestedplication is not defined.")
 
     __rmul__ = __mul__
 
     def __truediv__(self: PfState, other):
         other = _prep_data(other, self.index)  # other is now PfState, PfLine, or Series
         _assert_index_compatibility(self, other)
```

### Comparing `portfolyo-0.4.5/portfolyo/core/pfstate/pfstate.py` & `portfolyo-0.5.0/portfolyo/core/pfstate/pfstate.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,38 +9,35 @@
 from typing import Iterable, Optional, Union
 
 import pandas as pd
 
 from ... import tools
 from ..mixins import OtherOutput, PfStatePlot, PfStateText
 from ..ndframelike import NDFrameLike
-from ..pfline import MultiPfLine, PfLine
+from ..pfline import NestedPfLine, PfLine
 from .pfstate_helper import make_pflines
 
 
 class PfState(NDFrameLike, PfStateText, PfStatePlot, OtherOutput):
     """Class to hold timeseries information of an energy portfolio, at a specific moment.
 
     Parameters
     ----------
     offtakevolume: PfLine (volume-only)
     unsourcedprice: PfLine (price-only)
-        Must be specified for at least the time period covering the offtake. If it
-        covers any more time, the values are stored, but not shown unless explicitly
-        accessing the .unsourcedprice property.
     sourced : PfLine (price-and-volume), optional
-        - If not specified, assume no sourcing has taken place.
-        - If specified, the intersection of the index of the offtake volume and that of
-          the sourcing are kept.
+        If not specified, assume no sourcing has taken place.
+
+    All PfLines are trimmed to the length of the offtakevolume.
 
     Notes
     -----
     Sign conventions:
     - Volumes (`q`, `w`): >0 if volume flows into the portfolio.
-    - Revenues (`r`): >0 if money flows out of the portfolio (i.e., costs).
+    - Revenues (`r`): >0 if money flows out of the portfolio. Consequently, income is negative.
     - Prices (`p`): normally positive.
 
     Attributes
     ----------
     offtakevolume : volume-only PfLine
         Offtake. Volumes are <=0 for all timestamps (see 'Notes' above).
     sourced : price-and-volume PfLine
@@ -55,19 +52,17 @@
     unsourcedprice : price-only PfLine
         Prices of the unsourced volume.
     netposition : price-and-volume PfLine
         Net portfolio positions. Convenience property for users with a "traders' view".
         Does not follow sign conventions (see 'Notes' above); volumes are <0 if
         portfolio is short and >0 if long. Identical to `.unsourced`, but with sign
         change for volumes and revenues (but not prices).
-    procurement : price-and-volume PfLine
+    pnl_cost : price-and-volume PfLine
         The expected costs needed to source the offtake volume; the sum of the sourced
         and unsourced positions.
-    index : pandas.DateTimeIndex
-        Left timestamp of each delivery period under consideration.
     """
 
     @classmethod
     def from_series(
         cls,
         *,
         pu: pd.Series,
@@ -136,23 +131,23 @@
     @property
     def offtake(self) -> PfLine:
         # Future development: return not volume-only but price-and-volume. (by including offtake prices)
         return self._offtakevolume
 
     @property
     def unsourced(self) -> PfLine:
-        return -(self.offtake.volume + self.sourced.volume) * self.unsourcedprice
+        return -(self.offtake.volume + self.sourced.volume) | self.unsourcedprice
 
     @property
     def netposition(self) -> PfLine:
         return -self.unsourced
 
     @property
     def pnl_cost(self):
-        return MultiPfLine({"sourced": self.sourced, "unsourced": self.unsourced})
+        return NestedPfLine({"sourced": self.sourced, "unsourced": self.unsourced})
 
     @property
     def sourcedfraction(self) -> pd.Series:
         return self.sourced.volume / -self.offtake.volume
 
     @property
     def unsourcedfraction(self) -> pd.Series:
```

### Comparing `portfolyo-0.4.5/portfolyo/core/pfstate/pfstate_helper.py` & `portfolyo-0.5.0/portfolyo/core/pfstate/pfstate_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,68 @@
 """Prepare/verify input data for PfState initialisation."""
 
 
 import warnings
 from typing import Any, Iterable
 
 from ... import tools
-from ..pfline import Kind, MultiPfLine, PfLine, SinglePfLine  # noqa
+from ..pfline import FlatPfLine, Kind, NestedPfLine, PfLine  # noqa
 
 
 def make_pflines(
     offtakevolume: Any, unsourcedprice: Any, sourced: Any = None
 ) -> Iterable[PfLine]:
     """Take offtake, unsourced, sourced information. Do some data massaging and return
     3 PfLines: for offtake volume, unsourced price, and sourced price and volume.
-
-    Note
-    ----
-    Does not intersect the indices; each component maintains its individual index. (In
-    PfState, the offtake's index is used.)
     """
     # Ensure unsourced and offtake are specified.
     if offtakevolume is None or unsourcedprice is None:
         raise ValueError("Must specify offtake volume and unsourced prices.")
 
     # Get everything as PfLine.
     # . Offtake volume.
     offtakevolume = PfLine(offtakevolume)  # force to be PfLine.
-    if offtakevolume.kind is Kind.PRICE_ONLY:
+    if offtakevolume.kind is Kind.PRICE:
         raise ValueError("Parameter ``offtakevolume`` does not contain volume.")
-    elif offtakevolume.kind is Kind.ALL:
+    elif offtakevolume.kind is Kind.COMPLETE:
         warnings.warn(
             "Parameter ``offtakevolume``: also contains price infomation; this is discarded."
         )
         offtakevolume = offtakevolume.volume
     # . Unsourced prices.
     unsourcedprice = PfLine(unsourcedprice)  # force to be PfLine.
-    if unsourcedprice.kind is Kind.VOLUME_ONLY:
+    if unsourcedprice.kind is Kind.VOLUME:
         raise ValueError("Parameter ``unsourcedprice`` does not contain prices.")
-    elif unsourcedprice.kind is Kind.ALL:
+    elif unsourcedprice.kind is Kind.COMPLETE:
         warnings.warn(
             "Parameter ``unsourcedprice``: also contains volume infomation; this is discarded."
         )
         unsourcedprice = unsourcedprice.price
     # . Sourced volume and prices.
     if sourced is not None:
         sourced = PfLine(sourced)
-        if sourced.kind is not Kind.ALL:
+        if sourced.kind is not Kind.COMPLETE:
             raise ValueError("Parameter ``sourced`` does not contain price and volume.")
 
     # Check/fix indices.
     # . Frequencies.
     freqs = [
         o.index.freq for o in (offtakevolume, unsourcedprice, sourced) if o is not None
     ]
     if len(set(freqs)) != 1:
         raise ValueError("PfLines have unequal frequency; resample first.")
-    # . Lengths of offtakevolume and sourced.
+    # . Keep only overlapping part of indices.
+    idx = offtakevolume.index
+    if len(tools.intersect.indices(idx, unsourcedprice.index)) < len(idx):
+        raise ValueError(
+            "Parameter ``unsourcedprice``: does not cover entire delivery period of ``offtakevolume``."
+        )
+    unsourcedprice = unsourcedprice.loc[idx]
     if sourced is not None:
         # Workaround for error in pandas intersection (#46702):
-        idx = tools.intersect.indices(offtakevolume.index, sourced.index)
-        offtakevolume = offtakevolume.loc[idx]
+        if len(tools.intersect.indices(idx, sourced.index)) < len(idx):
+            raise ValueError(
+                "Parameter ``sourced``: does not cover entire delivery period of ``offtakevolume``."
+            )
         sourced = sourced.loc[idx]
-    # . Length of unsourcedprice.
-    if len(tools.intersect.indices(offtakevolume.index, unsourcedprice.index)) < len(
-        offtakevolume.index
-    ):
-        raise ValueError(
-            "Parameter ``unsourcedprice``: does not cover entire delivery"
-            " period of ``offtakevolume`` (and ``sourced``, if specified)."
-        )
 
     return offtakevolume, unsourcedprice, sourced
```

### Comparing `portfolyo-0.4.5/portfolyo/dev/develop.py` & `portfolyo-0.5.0/portfolyo/dev/develop.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,212 +5,212 @@
 import datetime as dt
 from typing import Dict, Union
 
 import numpy as np
 import pandas as pd
 
 from .. import tools
-from ..core.pfline import Kind, MultiPfLine, PfLine, SinglePfLine
+from ..core.pfline import FlatPfLine, Kind, NestedPfLine, PfLine
 from ..core.pfstate import PfState
 from . import mockup
 
 OK_COL_COMBOS = ["w", "q", "p", "pr", "qr", "qp", "wp", "wr"]
 
 
 def get_index(
     freq: str = "D",
     tz: str = "Europe/Berlin",
     startdate: str = None,
     periods: int = None,
     start_of_day: dt.time = None,
     *,
-    _random: bool = True,
+    _seed: bool = True,
 ) -> pd.DatetimeIndex:
     """Get index."""
+    if _seed:
+        np.random.seed(_seed)
     if not periods:
         standard = {"AS": 4, "QS": 5, "MS": 14, "D": 400, "H": 10_000, "15T": 50_000}
         periods = standard.get(freq, 10)
-        if _random:
+        if _seed:
             periods = np.random.randint(periods // 2, periods * 2)
         if tools.freq.up_or_down(freq, "H") <= 0 and tz is None:
             # Shorten index to not include timestamp that do not exist in Europe/Berlin.
             periods = min(periods, 4000)
     if not startdate:
         a, m, d = 2020, 1, 1
-        a += np.random.randint(-4, 4) if _random else (periods % 20 - 10)
+        a += np.random.randint(-4, 4) if _seed else (periods % 20 - 10)
         if tools.freq.up_or_down(freq, "MS") <= 0:
-            m += np.random.randint(0, 12) if _random else (periods % 12)
+            m += np.random.randint(0, 12) if _seed else (periods % 12)
         if tools.freq.up_or_down(freq, "D") <= 0:
-            d += np.random.randint(0, 28) if _random else (periods % 28)
+            d += np.random.randint(0, 28) if _seed else (periods % 28)
         if tools.freq.up_or_down(freq, "H") <= 0 and tz is None:
             # Start index after DST-start to not include timestamps that do not exist in Europe/Berlin.
             m, d = 4, 2
         startdate = f"{a}-{m}-{d}"
     if not start_of_day:
         start_of_day = dt.time(hour=0, minute=0)
     starttime = f"{start_of_day.hour:02}:{start_of_day.minute:02}:00"
     start = f"{startdate} {starttime}"
     return pd.date_range(start, freq=freq, periods=periods, tz=tz)
 
 
 def get_value(
-    name: str = "w", has_unit: bool = True, *, _random: bool = True
+    name: str = None, has_unit: bool = True, magn: float = None, *, _seed: int = None
 ) -> Union[float, tools.unit.Q_]:
     """Get a single value."""
-    if not _random:
-        np.random.seed(0)
-    magn = np.random.random() * 200
+    if _seed:
+        np.random.seed(_seed)
+    if magn is None:
+        magn = np.random.random() * 200
     if not has_unit:
         return magn
     else:
         unit = tools.unit.from_name(name)
         return tools.unit.Q_(magn, unit)
 
 
 def get_series(
     i: pd.DatetimeIndex = None,
-    name: str = "w",
+    name: str = None,
     has_unit: bool = True,
     *,
-    _random: bool = True,
+    _seed: int = None,
 ) -> pd.Series:
     """Get Series with index `i` and name `name`. Values from mock-up functions (if in
     'wqpr') or random between 100 and 200."""
     if i is None:
-        i = get_index(_random=_random)
+        i = get_index(_seed=_seed)
     i.name = "ts_left"
 
-    if not _random:
-        np.random.seed(0)
+    if _seed:
+        np.random.seed(_seed)
 
     if name == "w":
         # random average, and 3 random amplitudes with sum < 1
-        avg = (10 + 30 * np.random.random()) * np.random.choice([1, 10, 100])
+        avg = 30 + 10 * np.random.random()
         ampls = np.random.rand(3) * np.array([0.3, 0.2, 0.1])
         return mockup.w_offtake(i, avg, *ampls, has_unit=has_unit)
     elif name == "q":
         q = get_series(i, "w", True) * i.duration
         q = q.rename("q")
         return q if has_unit else q.pint.m
     elif name == "p":
         # random average, and 3 random amplitudes with sum < 1
-        avg = 50 + 100 * np.random.random()
+        avg = 100 + 20 * np.random.random()
         ampls = np.random.rand(3) * np.array([0.25, 0.04, 0.3])
         return mockup.p_marketprices(i, avg, *ampls, has_unit=has_unit)
     elif name == "r":
         r = get_series(i, "q", has_unit) * get_series(i, "p", has_unit)
         return r.rename("r")
+    elif name == "nodim":
+        dtype = "pint[dimensionless]" if has_unit else float
+        return pd.Series(0.9 + 0.2 * np.random.rand(len(i)), i, dtype=dtype)
     else:
         return pd.Series(100 + 100 * np.random.rand(len(i)), i, name=name)
 
 
 def get_dataframe(
     i: pd.DatetimeIndex = None,
     columns="wp",
     has_unit: bool = True,
     *,
-    _random: bool = True,
+    _seed: int = None,
 ) -> pd.DataFrame:
     """Get DataFrame with index `i` and columns `columns`. Columns (e.g. `q` and `w`)
     are not made consistent."""
     if i is None:
-        i = get_index(_random=_random)
+        i = get_index(_seed=_seed)
     i.name = "ts_left"
-    series = {col: get_series(i, col, has_unit, _random=_random) for col in columns}
+    series = {col: get_series(i, col, has_unit, _seed=_seed) for col in columns}
     return pd.DataFrame(series)
 
 
 # Portfolio line.
 
 
-def get_singlepfline(
-    i: pd.DatetimeIndex = None, kind: Kind = Kind.ALL, *, _random: bool = True
-) -> SinglePfLine:
-    """Get single portfolio line, i.e. without children."""
-    if not isinstance(kind, Kind):
-        kind = Kind(kind)
-    columns = {Kind.VOLUME_ONLY: "q", Kind.PRICE_ONLY: "p", Kind.ALL: "qr"}[kind]
-    return SinglePfLine(get_dataframe(i, columns))
-
-
-def get_multipfline(
-    i: pd.DatetimeIndex = None, kind: Kind = Kind.ALL, *, _random: bool = True
-) -> MultiPfLine:
-    """Get multi portfolio line. With 2 (singlepfline) children of the same ``kind``."""
+def get_flatpfline(
+    i: pd.DatetimeIndex = None, kind: Kind = Kind.COMPLETE, *, _seed: int = None
+) -> FlatPfLine:
+    """Get flat portfolio line, i.e. without children."""
     if not isinstance(kind, Kind):
         kind = Kind(kind)
+    columns = {
+        Kind.VOLUME: "q",
+        Kind.PRICE: "p",
+        Kind.REVENUE: "r",
+        Kind.COMPLETE: "qr",
+    }[kind]
+    return FlatPfLine(get_dataframe(i, columns, _seed=_seed))
+
+
+def get_nestedpfline(
+    i: pd.DatetimeIndex = None, kind: Kind = Kind.COMPLETE, *, _seed: int = None
+) -> NestedPfLine:
+    """Get nested portfolio line. With 2 (flat) children of the same ``kind``."""
     if i is None:
-        i = get_index(_random=_random)
-    return MultiPfLine(
+        i = get_index(_seed=_seed)
+    return NestedPfLine(
         {
-            "A": get_singlepfline(i, kind, _random=_random),
-            "B": get_singlepfline(i, kind, _random=_random),
+            "A": get_flatpfline(i, kind, _seed=_seed),
+            "B": get_flatpfline(i, kind, _seed=_seed),
         }
     )
 
 
-def get_pfline(
+def get_randompfline(
     i: pd.DatetimeIndex = None,
-    kind: Kind = Kind.ALL,
+    kind: Kind = Kind.COMPLETE,
     max_nlevels: int = 3,
     childcount: int = 2,
     prefix: str = "",
     *,
-    _random: bool = True,
+    _seed: int = None,
 ) -> PfLine:
     """Get portfolio line, without children or with children in random number of levels.
     (including the current level; max_nlevels must be >= 1.)"""
-    if not isinstance(kind, Kind):
-        kind = Kind(kind)
     # Gather information.
     if i is None:
-        i = get_index(_random=_random)
-    if not _random:
-        np.random.seed(0)
+        i = get_index(_seed=_seed)
+    if _seed:
+        np.random.seed(_seed)
     nlevels = np.random.randint(0, max_nlevels)
-    # Create single PfLine.
+    # Create flat PfLine.
     if nlevels == 0:
-        return get_singlepfline(i, kind, _random=_random)
-    # Gather information.
-    if childcount == 2 and kind is Kind.ALL and np.random.rand() < 0.33:
-        kinds = [Kind.PRICE_ONLY, Kind.VOLUME_ONLY]
-    else:
-        kinds = [kind] * childcount
-    # Create multi PfLine.
+        return get_flatpfline(i, kind, _seed=_seed)
+    # Create nested PfLine.
     children = {}
-    for c, knd in enumerate(kinds):
+    for c in range(childcount):
         name = f"part {prefix}{c}."
-        children[name] = get_pfline(
-            i, knd, max_nlevels - 1, prefix=f"{prefix}{c}.", _random=_random
+        children[name] = get_randompfline(
+            i, kind, max_nlevels - 1, prefix=f"{prefix}{c}.", _seed=_seed
         )
-    return MultiPfLine(children)
+    return NestedPfLine(children)
 
 
 # Portfolio state.
 
 
-def get_pfstate(
-    i: pd.DatetimeIndex = None, avg=None, *, _random: bool = True
-) -> PfState:
+def get_pfstate(i: pd.DatetimeIndex = None, avg=None, *, _seed: int = None) -> PfState:
     """Get portfolio state."""
     if i is None:
-        i = get_index(_random=_random)
-    if not _random:
-        np.random.seed(0)
+        i = get_index(_seed=_seed)
+    if _seed:
+        np.random.seed(_seed)
     if avg is None:
         avg = 200 ** np.random.rand()  # between 1 and 200
     wo = -1 * mockup.w_offtake(i, avg)
     pu = mockup.p_marketprices(i)
     ws, ps = mockup.wp_sourced(wo)
     return PfState.from_series(wo=wo, pu=pu, ws=ws, ps=ps)
 
 
 def get_pfstates(
-    i: pd.DatetimeIndex = None, num=3, *, _random: bool = True
+    i: pd.DatetimeIndex = None, num=3, *, _seed: int = None
 ) -> Dict[str, PfState]:
     """Get dictionary of portfolio states."""
     if i is None:
-        i = get_index(_random=_random)
+        i = get_index(_seed=_seed)
     names = ["Pf 1", "Portfolio 2 (long name)", "Portfolio number three"]
     for n in range(3, num):
         names.append(f"Portfolio {n+1}")
-    return {name: get_pfstate(i, _random=_random) for name in names[:num]}
+    return {name: get_pfstate(i, _seed=_seed) for name in names[:num]}
```

### Comparing `portfolyo-0.4.5/portfolyo/dev/mockup.py` & `portfolyo-0.5.0/portfolyo/dev/mockup.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     wa = i.map(lambda ts: ts.weekday() + 1) / 7 * np.pi * 2
     # peak fraction: -1 (middle of offpeak hours) .. 1 (middle of peak hours)
     if i.freq in ["H", "15T"]:
         b = np.array([0.5, 0.8, 1, 0.8, 0.5])
         if i.freq == "15T":  # repeat every value 4 times
             b = np.array([[bb, bb, bb, bb] for bb in b]).flatten()
         b = b[: len(i)]  # slice in case i is very short
-        pa = np.convolve(-1 + 2 * i.map(is_peak_hour), b / sum(b), mode="same")
+        pa = np.convolve(-1 + 2 * is_peak_hour(i), b / sum(b), mode="same")
     else:
         pa = np.zeros(len(i))
     # Values
     yv = year_amp * np.cos(ya - 0.35)  # max in feb
     wv = week_amp * np.cos(wa - 1.07)  # max on tuesday
     pv = peak_amp * pa
     s = pd.Series(avg * (1 + yv + wv + pv), i, name="p")
```

### Comparing `portfolyo-0.4.5/portfolyo/prices/convert.py` & `portfolyo-0.5.0/portfolyo/prices/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,20 +227,20 @@
     offpeak    20.311204
     dtype: float64
     """
     # Handle possible units.
     sin, units = (s.pint.magnitude, s.pint.units) if hasattr(s, "pint") else (s, None)
 
     # Do calculations. Use normal mean, because all rows have same duration.
-    grouped = sin.groupby(utils.is_peak_hour).mean()
+    is_peak = utils.is_peak_hour(sin.index)
     sout = pd.Series(
         {
             f"{prefix}base": sin.mean(),
-            f"{prefix}peak": grouped.get(True, np.nan),
-            f"{prefix}offpeak": grouped.get(False, np.nan),
+            f"{prefix}peak": sin[is_peak].mean(),
+            f"{prefix}offpeak": sin[~is_peak].mean(),
         }
     )
 
     # Handle possible units.
     if units is not None:
         sout = sout.astype(f"pint[{units}]")
     return sout
@@ -366,15 +366,15 @@
     """
     if freq not in ("H", "15T"):
         raise ValueError(f"Parameter ``freq`` must be 'H' or '15T'; got '{freq}'.")
 
     df = bpoframe.rename({f"{prefix}{bpo}": bpo for bpo in BPO}, axis=1)  # remove prefx
     df = complete_bpoframe(df)  # make sure we have peak and offpeak columns
     df = tools.changefreq.averagable(df[["peak", "offpeak"]], freq)
-    df["ispeak"] = df.index.map(utils.is_peak_hour)
+    df["ispeak"] = utils.is_peak_hour(df.index)
 
     return df["offpeak"].where(df["ispeak"], df["peak"])
 
 
 def tseries2tseries(s: pd.Series, freq: str = "MS") -> pd.Series:
     """
     Transform timeseries (with possibly variable values) to one with (at certain
```

### Comparing `portfolyo-0.4.5/portfolyo/prices/hedge.py` & `portfolyo-0.5.0/portfolyo/prices/hedge.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,38 +33,43 @@
 
     Notes
     -----
     If the index of `df` doesn't have a .duration attribute, all rows are assumed to be
     of equal duration.
     """
 
-    if not po:
-        if df.index.freq:
-            # Use magnitude only, so that, if w and p are float series, their return
-            # series are also floats (instead of dimensionless Quantities).
-            df["dur"] = df.index.duration.pint.m
-        else:
-            df["dur"] = 1
-
-        # Get single power and price values.
-        p_hedge = (df.p * df.dur).sum() / df.dur.sum()
-        if how == "vol":  # volume hedge
-            # solve for w_hedge: sum (w * duration) == w_hedge * sum (duration)
-            w_hedge = (df.w * df.dur).sum() / df.dur.sum()
-        elif how == "val":  # value hedge
-            # solve for w_hedge: sum (w * duration * p) == w_hedge * sum (duration * p)
-            w_hedge = (df.w * df.dur * df.p).sum() / (df.dur * df.p).sum()
-        else:
-            raise ValueError(f"Parameter `how` must be 'val' or 'vol'; got {how}.")
-        return pd.Series({"w": w_hedge, "p": p_hedge})
-    else:
+    # Split into peak and offpeak.
+
+    if po:
         apply_f = lambda df: _hedge(df, how, po=False)  # noqa
-        s = df.groupby(is_peak_hour).apply(apply_f)
+        # s = df.groupby(is_peak_hour).apply(apply_f) # calls group_f on EACH ts
+        s = df.groupby(is_peak_hour(df.index)).apply(apply_f)  # calls group_f on index
         return s.rename(index={True: "peak", False: "offpeak"}).stack()
 
+    # Don't split into peak and offpeak.
+
+    if df.index.freq:
+        # Use magnitude only, so that, if w and p are float series, their return
+        # series are also floats (instead of dimensionless Quantities).
+        df["dur"] = df.index.duration.pint.m
+    else:
+        df["dur"] = 1
+
+    # Get single power and price values.
+    p_hedge = (df.p * df.dur).sum() / df.dur.sum()
+    if how == "vol":  # volume hedge
+        # solve for w_hedge: sum (w * duration) == w_hedge * sum (duration)
+        w_hedge = (df.w * df.dur).sum() / df.dur.sum()
+    elif how == "val":  # value hedge
+        # solve for w_hedge: sum (w * duration * p) == w_hedge * sum (duration * p)
+        w_hedge = (df.w * df.dur * df.p).sum() / (df.dur * df.p).sum()
+    else:
+        raise ValueError(f"Parameter `how` must be 'val' or 'vol'; got {how}.")
+    return pd.Series({"w": w_hedge, "p": p_hedge})
+
 
 def hedge(
     w: pd.Series,
     p: pd.Series,
     how: str = "val",
     freq: str = "MS",
     po: bool = None,
@@ -122,17 +127,20 @@
     i = win.index.intersection(pin.index)
     df = tools.trim.frame(pd.DataFrame({"w": win, "p": pin}).loc[i, :], freq)
     if len(df) == 0:
         return df["w"], df["p"]  # No full periods; don't do hedge; return empty series
 
     # Do actual hedge.
     group_f = convert.group_function(freq, po)
-    vals = df.groupby(group_f).apply(lambda df: _hedge(df, how, False))
+    grouped_i = pd.MultiIndex.from_arrays(group_f(df.index))  # calls group_f on index
+    apply_f = lambda df: _hedge(df, how, False)  # noqa
+    # vals = df.groupby(group_f).apply(apply_f) # calls group_f on EACH ts
+    vals = df.groupby(grouped_i).apply(apply_f)
     vals.index = pd.MultiIndex.from_tuples(vals.index)
     for c in ["w", "p"]:
-        df[c] = df[c].groupby(group_f).transform(lambda gr: vals.loc[gr.name, c])
+        df[c] = df[c].groupby(grouped_i).transform(lambda gr: vals.loc[gr.name, c])
 
     # Handle possible units.
     if wunits or punits:
         df = df.astype({"w": f"pint[{wunits:P}]", "p": f"pint[{punits:P}]"})
 
     return df["w"], df["p"]
```

### Comparing `portfolyo-0.4.5/portfolyo/prices/utils.py` & `portfolyo-0.5.0/portfolyo/prices/utils.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/testing/testing.py` & `portfolyo-0.5.0/portfolyo/testing/testing.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import functools
 
 import numpy as np
 import pandas as pd
 
 from .. import tools
+from ..tools.unit import Q_
 
 
 @functools.wraps(pd.testing.assert_frame_equal)
 def assert_frame_equal(left, right, *args, **kwargs):
     # Dataframes equal even if *order* of columns is not the same.
     left = tools.unit.drop_units(left).sort_index(axis=1)
     right = tools.unit.drop_units(right).sort_index(axis=1)
@@ -41,7 +42,34 @@
     else:  # normal series of floats or ints
         left = left.replace([np.inf, -np.inf], np.nan)
         right = right.replace([np.inf, -np.inf], np.nan)
         pd.testing.assert_series_equal(left, right, *args, **kwargs)
 
 
 assert_index_equal = pd.testing.assert_index_equal
+
+
+def assert_w_q_compatible(freq: str, w: pd.Series, q: pd.Series):
+    """Assert if timeseries with power- and energy-values are consistent."""
+    if freq == "15T":
+        assert_series_equal(q, w * Q_(0.25, "h"), check_names=False)
+    elif freq == "H":
+        assert_series_equal(q, w * Q_(1, "h"), check_names=False)
+    elif freq == "D":
+        assert (q >= w * Q_(22.99, "h")).all()
+        assert (q <= w * Q_(25.01, "h")).all()
+    elif freq == "MS":
+        assert (q >= w * 27 * Q_(24, "h")).all()
+        assert (q <= w * 32 * Q_(24, "h")).all()
+    elif freq == "QS":
+        assert (q >= w * 89 * Q_(24, "h")).all()
+        assert (q <= w * 93 * Q_(24, "h")).all()
+    elif freq == "AS":
+        assert (q >= w * Q_(8759.9, "h")).all()
+        assert (q <= w * Q_(8784.1, "h")).all()
+    else:
+        raise ValueError(f"Uncaught value for freq: {freq}.")
+
+
+def assert_p_q_r_compatible(r: pd.Series, p: pd.Series, q: pd.Series):
+    """Assert if timeseries with revenue-, power-, and energy-values are consistent."""
+    assert_series_equal(r, q * p, check_names=False)
```

### Comparing `portfolyo-0.4.5/portfolyo/tools/ceil.py` & `portfolyo-0.5.0/portfolyo/tools/ceil.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/changefreq.py` & `portfolyo-0.5.0/portfolyo/tools/changefreq.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/changeyear.py` & `portfolyo-0.5.0/portfolyo/tools/changeyear.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/duration.py` & `portfolyo-0.5.0/portfolyo/tools/duration.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/floor.py` & `portfolyo-0.5.0/portfolyo/tools/floor.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/frame.py` & `portfolyo-0.5.0/portfolyo/tools/frame.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/freq.py` & `portfolyo-0.5.0/portfolyo/tools/freq.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/intersect.py` & `portfolyo-0.5.0/portfolyo/tools/intersect.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     # If we land here, we have at least 2 indices, all are not empty, with equal tz and freq.
 
     distinct_sod = set([i[0].time() for i in idxs])
     if len(distinct_sod) != 1:
         raise ValueError(f"Indices must have equal start-of-day; got {distinct_sod}.")
 
-    # Calculation is cumbersome: pandas DatetimeIndex.intersection not working correctly on timezone-aware indices.
+    # Calculation is cumbersome: pandas DatetimeIndex.intersection not working correctly on timezone-aware indices (#46702)
     values = set(idxs[0])
     for i in idxs[1:]:
         values = values.intersection(set(i))
 
     return pd.DatetimeIndex(sorted(list(values)), freq=freq, name=name, tz=tz)
```

### Comparing `portfolyo-0.4.5/portfolyo/tools/isboundary.py` & `portfolyo-0.5.0/portfolyo/tools/isboundary.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/leftandright.py` & `portfolyo-0.5.0/portfolyo/tools/leftandright.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/peakperiod.py` & `portfolyo-0.5.0/portfolyo/tools/peakperiod.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/right.py` & `portfolyo-0.5.0/portfolyo/tools/right.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/righttoleft.py` & `portfolyo-0.5.0/portfolyo/tools/righttoleft.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/round.py` & `portfolyo-0.5.0/portfolyo/tools/round.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/standardize.py` & `portfolyo-0.5.0/portfolyo/tools/standardize.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/trim.py` & `portfolyo-0.5.0/portfolyo/tools/trim.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/tzone.py` & `portfolyo-0.5.0/portfolyo/tools/tzone.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/unit.py` & `portfolyo-0.5.0/portfolyo/tools/unit.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/unitdefinitions.txt` & `portfolyo-0.5.0/portfolyo/tools/unitdefinitions.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/tools/wavg.py` & `portfolyo-0.5.0/portfolyo/tools/wavg.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/portfolyo/visualize/visualize.py` & `portfolyo-0.5.0/portfolyo/visualize/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 Visualize portfolio lines, etc.
 """
 
-import colorsys
-from collections import namedtuple
-from typing import Iterable, List, Optional
-
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
 from .. import tools
+from .categories import Categories, Category  # noqa
 
 mpl.style.use("seaborn")
 
 # Plotting philosophy for timeseries:
 # Not all plot types (bar, line, step, etc.) are suitable for all quantities.
 #
 # Data dimensionality vs plot type
@@ -51,97 +48,27 @@
 #
 #
 # This module is able to plot all graph types on both timeline x-axis and on categorical
 # x-axis, and add the data labels if there are not too many. It is up to the caller to
 # pick the correct graph type.
 #
 
-
-class Color(namedtuple("RGB", ["r", "g", "b"])):
-    """Class to create an rgb color tuple, with additional methods."""
-
-    def lighten(self, value):
-        """Lighten the color by fraction ``value`` (between 0 and 1). If < 0, darken."""
-        hu, li, sa = np.array(colorsys.rgb_to_hls(*mpl.colors.to_rgb(self)))
-        li += value * ((1 - li) if value > 0 else li)
-        return Color(*[min(max(p, 0), 1) for p in colorsys.hls_to_rgb(hu, li, sa)])
-
-    def darken(self, value):
-        """Darken the color by fraction ``value`` (between 0 and 1)."""
-        return self.lighten(self, -value)
-
-    light = property(lambda self: self.lighten(0.3))
-    xlight = property(lambda self: self.lighten(0.6))
-    dark = property(lambda self: self.lighten(-0.3))
-    xdark = property(lambda self: self.lighten(-0.6))
-
-
-class Colors:
-    class General:
-        PURPLE = Color(0.549, 0.110, 0.706)
-        GREEN = Color(0.188, 0.463, 0.165)
-        BLUE = Color(0.125, 0.247, 0.600)
-        ORANGE = Color(0.961, 0.533, 0.114)
-        RED = Color(0.820, 0.098, 0.114)
-        YELLOW = Color(0.945, 0.855, 0.090)
-        LBLUE = Color(0.067, 0.580, 0.812)
-        LGREEN = Color(0.325, 0.773, 0.082)
-        BLACK = Color(0, 0, 0)
-        WHITE = Color(1, 1, 1)
-
-    class LbCd:  # Lichtblick corporate design
-        YELLOW = Color(*mpl.colors.to_rgb("#FA9610"))
-        SMOKE = Color(*mpl.colors.to_rgb("#465B68"))
-        BERRY = Color(*mpl.colors.to_rgb("#D4496A"))
-        AQUA = Color(*mpl.colors.to_rgb("#0BA3C1"))
-        GREEN = Color(*mpl.colors.to_rgb("#077144"))
-        MOSS = Color(*mpl.colors.to_rgb("#658A7C"))
-
-    class Wqpr:  # Standard colors when plotting a portfolio
-        w = Color(*mpl.colors.to_rgb("#0E524F")).lighten(0.15)
-        q = Color(*mpl.colors.to_rgb("#0E524F"))
-        r = Color(*mpl.colors.to_rgb("#8B7557"))
-        p = Color(*mpl.colors.to_rgb("#E53454"))
-
-
-def _index2labels(index: pd.DatetimeIndex) -> List[str]:
-    """Create labels corresponding to the timestamps in the index."""
-    if index.freq == "AS":
-
-        def label(ts, i):
-            return f"{ts.year}"
-
-    elif index.freq == "QS":
-
-        def label(ts, i):
-            num = ts.quarter
-            return f"Q{num}\n" + (f"{ts.year}" if i == 0 or num == 1 else "")
-
-    elif index.freq == "MS":
-
-        def label(ts, i):
-            num, name = ts.month, ts.month_name()[:3]
-            return f"{name}\n" + (f"{ts.year}" if i == 0 or num == 1 else "")
-
-    else:
-        raise ValueError("Daily (or shorter) data should not be plotted as categories.")
-    return [label(ts, i) for i, ts in enumerate(index)]
+MAX_XLABELS = 20
 
 
-def _categories(ax: plt.Axes, s: pd.Series, cat: bool = None) -> Optional[Iterable]:
-    """Category labels for `s`. Or None, if s should be plotted on time axis."""
-    create = False
+def use_categories(ax: plt.Axes, s: pd.Series, cat: bool = None) -> bool:
+    """Determine if plot should be made with category axis (True) or datetime axis (False)."""
     # We use categorical data if...
     if (ax.lines or ax.collections or ax.containers) and ax.xaxis.have_units():
-        create = True  # ...ax already has category axis; or
+        return True  # ...ax already has category axis; or
     elif cat is None and tools.freq.shortest(s.index.freq, "MS") == "MS":
-        create = True  # ...it's the default for the given frequency; or
+        return True  # ...it's the default for the given frequency; or
     elif cat is True:
-        create = True  # ...user wants it.
-    return _index2labels(s.index) if create else None
+        return True  # ...user wants it.
+    return False
 
 
 docstringliteral_plotparameters = """
 Other parameters
 ----------------
 labelfmt : str, optional (default: '')
     Labels are added to each datapoint in the specified format. ('' to add no labels)
@@ -166,142 +93,132 @@
 def plot_timeseries_as_jagged(
     ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
 ) -> None:
     """Plot timeseries ``s`` to axis ``ax``, as jagged line and/or as markers. Use kwargs
     ``linestyle`` and ``marker`` to specify line style and/or marker style. (Default: line only)."""
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
-    # Plot.
-    categories = _categories(ax, s, cat)
-    if categories:
-        xx = categories
-    else:
-        xx = s.index
-    ax.plot(xx, s.values, **kwargs)
+    if use_categories(ax, s, cat):
+        categories = Categories(s)
+        ax.plot(categories.x(), categories.y(), **kwargs)
+        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
+        set_data_labels(ax, categories.x(), categories.y(), labelfmt, False)
 
-    add_labels(ax, xx, s.values, labelfmt, False)  # add labels to datapoints
+    else:
+        ax.plot(s.index, s.values, **kwargs)
+        set_data_labels(ax, s.index, s.values, labelfmt, False)
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_bar(
     ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
 ) -> None:
     """Plot timeseries ``s`` to axis ``ax``, as bars. Ideally, only used for plots with
     categorical (i.e, non-time) x-axis."""
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
-    # Plot and add labels to datapoints.
-    categories = _categories(ax, s, cat)
-    if categories:
-
-        ax.bar(categories, s.values, 0.8, **kwargs)
-        add_labels(ax, categories, s.values, labelfmt, True)
+    if use_categories(ax, s, cat):
+        categories = Categories(s)
+        ax.bar(categories.x(), categories.y(), 0.8, **kwargs)
+        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
+        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
 
-    else:  # Bad combination: bar graph on time-axis. But allow anyway.
+    else:
+        # Bad combination: bar graph on time-axis. But allow anyway.
 
         # This is slow if there are many elements.
         # x = s.index + 0.5 * (s.index.right - s.index)
         # width = pd.Timedelta(hours=s.index.duration.median().to("h").magnitude * 0.8)
         # ax.bar(x.values, s.values, width, **kwargs)
 
         # This is faster.
         delta = s.index.right - s.index
         x = np.array(list(zip(s.index + 0.1 * delta, s.index + 0.9 * delta))).flatten()
         magnitudes = np.array([[v, 0] for v in s.values.quantity.magnitude]).flatten()
         values = tools.unit.PA_(magnitudes, s.values.quantity.units)
         ax.fill_between(x, 0, values, step="post", **kwargs)
 
-        add_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_area(
     ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
 ) -> None:
     """Plot timeseries ``s`` to axis ``ax``, as stepped area between 0 and value. Ideally,
     only used for plots with time (i.e., non-categorical) axis."""
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
     splot = s.copy()  # modified with additional (repeated) datapoint
     splot[splot.index.right[-1]] = splot.values[-1]
 
-    # Plot and add labels to datapoints.
-    categories = _categories(ax, s, cat)
-    if categories:  # Bad combination: area graph on categorical axis. But allow anyway.
-
-        xplot = np.arange(len(categories) + 1)
-        ax.fill_between(
-            xplot - 0.5, 0, splot.values, step="post", **kwargs
-        )  # center around x-tick
-        ax.set_xticks(xplot)
-        ax.set_xticklabels([*categories, ""])
-        add_labels(ax, range(len(s)), s.values, labelfmt, True)
+    if use_categories(ax, s, cat):
+        # Bad combination: area graph on categorical axis. But allow anyway.
 
-    else:
+        categories = Categories(s)
+        ctgr_extra = Categories(splot)
+        # Center around x-tick:
+        ax.fill_between(ctgr_extra.x() - 0.5, 0, ctgr_extra.y(), step="post", **kwargs)
+        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
+        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
 
+    else:
         ax.fill_between(splot.index, 0, splot.values, step="post", **kwargs)
         delta = s.index.right - s.index
-        add_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_step(
     ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
 ) -> None:
     """Plot timeseries ``s`` to axis ``ax``, as stepped line (horizontal and vertical lines).
     Ideally, only used for plots with time (i.e., non-categorical) axis."""
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
     splot = s.copy()  # modified with additional (repeated) datapoint
     splot[splot.index.right[-1]] = splot.values[-1]
 
-    # Plot add labels to datapoints
-    categories = _categories(ax, s, cat)
-    if categories:  # Bad combination: step graph on categorical axis. But allow anyway.
-
-        xplot = np.arange(len(categories) + 1)
-        ax.step(
-            xplot - 0.5, splot.values, where="post", **kwargs
-        )  # center around x-tick
-        ax.set_xticks(xplot)
-        ax.set_xticklabels([*categories, ""])
-        add_labels(ax, range(len(s)), s.values, labelfmt, True)
+    if use_categories(ax, s, cat):
+        # Bad combination: step graph on categorical axis. But allow anyway.
 
-    else:
+        categories = Categories(s)
+        ctgr_extra = Categories(splot)
+        # Center around x-tick:
+        ax.step(ctgr_extra.x() - 0.5, ctgr_extra.y(), where="post", **kwargs)
+        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
+        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
 
+    else:
         ax.step(splot.index, splot.values, where="post", **kwargs)
         delta = s.index.right - s.index
-        add_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
+        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, True)
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_hline(
     ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
 ) -> None:
     """Plot timeseries ``s`` to axis ``ax``, as horizontal lines. Ideally, only used for
     plots with time (i.e., non-categorical) axis."""
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
-    # Plot and add labels to datapoints
-    categories = _categories(ax, s, cat)
-    if (
-        categories
-    ):  # Bad combination: hline graph on categorical axis. But allow anyway.
-
-        x = np.arange(len(categories))
-        ax.hlines(s.values, x - 0.5, x + 0.5, **kwargs)
-        ax.set_xticks(x)
-        ax.set_xticklabels(categories)
-        add_labels(ax, x, s.values, labelfmt, False)
+    if use_categories(ax, s, cat):
+        # Bad combination: hline graph on categorical axis. But allow anyway.
 
-    else:
+        categories = Categories(s)
+        # Center around x-tick:
+        ax.hlines(categories.y(), categories.x() - 0.5, categories.x() + 0.5, **kwargs)
+        ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
+        set_data_labels(ax, categories.x(), categories.y(), labelfmt, True)
 
+    else:
         delta = s.index.right - s.index
         ax.hlines(s.values, s.index, s.index.right, **kwargs)
-        add_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, False)
+        set_data_labels(ax, s.index + 0.5 * delta, s.values, labelfmt, False)
 
 
 def plot_timeseries(
     ax: plt.Axes,
     s: pd.Series,
     how: str = "jagged",
     labelfmt: str = None,
@@ -381,15 +298,15 @@
         s = s.pint.to_base_units()
         setattr(ax, "_unit", s.pint.units)
 
     ax.set_ylabel(f"{ax._unit:~P}")
     return s
 
 
-def add_labels(
+def set_data_labels(
     ax: plt.Axes, xx, yy, labelfmt, outside: bool = False, maxcount: int = 24
 ):
     """Add labels to axis ``ax``, at locations (``xx``, ``yy``), formatted with
     ``labelfmt``. Don't add labels if more than ``maxcount`` datapoints. If ``outside``,
     put labels of negative values *below* the datapoint."""
     # Don't label if no formatting speficied.
     if not labelfmt:
```

### Comparing `portfolyo-0.4.5/portfolyo.egg-info/PKG-INFO` & `portfolyo-0.5.0/portfolyo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.4.5
+Version: 0.5.0
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
 =========
 
 .. image:: https://img.shields.io/pypi/v/portfolyo
    :target: https://pypi.org/project/portfolyo
    :alt: Pypi
 
-.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci.yaml/badge.svg
-   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci.yaml
-   :alt: Github - CI
+.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-pullreq.yaml/badge.svg
+   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-pullreq.yaml
+   :alt: Github - CI (on pullrequest)
+
+.. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-push.yaml/badge.svg
+   :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/ci-on-push.yaml
+   :alt: Github - CI (on push)
 
 .. image:: https://github.com/rwijtvliet/portfolyo/actions/workflows/pre-commit.yaml/badge.svg
    :target: https://github.com/rwijtvliet/portfolyo/actions/workflows/pre-commit.yaml
    :alt: Github - Pre-commit
 
 .. image:: https://img.shields.io/codecov/c/gh/rwijtvliet/portfolyo
    :target: https://app.codecov.io/gh/rwijtvliet/portfolyo
```

### Comparing `portfolyo-0.4.5/portfolyo.egg-info/SOURCES.txt` & `portfolyo-0.5.0/portfolyo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 portfolyo/core/mixins/__init__.py
 portfolyo/core/mixins/other.py
 portfolyo/core/mixins/plot.py
 portfolyo/core/mixins/text.py
 portfolyo/core/pfline/__init__.py
 portfolyo/core/pfline/base.py
 portfolyo/core/pfline/enable_arithmatic.py
+portfolyo/core/pfline/flat.py
+portfolyo/core/pfline/flat_helper.py
 portfolyo/core/pfline/interop.py
-portfolyo/core/pfline/multi.py
-portfolyo/core/pfline/multi_helper.py
-portfolyo/core/pfline/single.py
-portfolyo/core/pfline/single_helper.py
+portfolyo/core/pfline/nested.py
+portfolyo/core/pfline/nested_helper.py
 portfolyo/core/pfstate/__init__.py
 portfolyo/core/pfstate/enable_arithmatic.py
 portfolyo/core/pfstate/pfstate.py
 portfolyo/core/pfstate/pfstate_helper.py
 portfolyo/dev/__init__.py
 portfolyo/dev/develop.py
 portfolyo/dev/mockup.py
@@ -60,8 +60,10 @@
 portfolyo/tools/standardize.py
 portfolyo/tools/trim.py
 portfolyo/tools/tzone.py
 portfolyo/tools/unit.py
 portfolyo/tools/unitdefinitions.txt
 portfolyo/tools/wavg.py
 portfolyo/visualize/__init__.py
-portfolyo/visualize/visualize.py
+portfolyo/visualize/categories.py
+portfolyo/visualize/colors.py
+portfolyo/visualize/plot.py
```

### Comparing `portfolyo-0.4.5/setup.py` & `portfolyo-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.4.5/versioneer.py` & `portfolyo-0.5.0/versioneer.py`

 * *Files identical despite different names*

