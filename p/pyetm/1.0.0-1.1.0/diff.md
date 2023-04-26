# Comparing `tmp/pyetm-1.0.0.tar.gz` & `tmp/pyetm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetm-1.0.0.tar", last modified: Mon Apr 24 21:40:47 2023, max compression
+gzip compressed data, was "pyetm-1.1.0.tar", last modified: Wed Apr 26 11:30:47 2023, max compression
```

## Comparing `pyetm-1.0.0.tar` & `pyetm-1.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.265516 pyetm-1.0.0/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    13827 2023-01-10 21:51:08.000000 pyetm-1.0.0/LICENSE
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-04-24 21:40:47.265516 pyetm-1.0.0/PKG-INFO
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      253 2023-01-10 21:51:08.000000 pyetm-1.0.0/README.md
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1324 2023-04-24 21:36:47.000000 pyetm-1.0.0/pyproject.toml
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       38 2023-04-24 21:40:47.266516 pyetm-1.0.0/setup.cfg
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.260516 pyetm-1.0.0/src/
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.261515 pyetm-1.0.0/src/pyetm/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       50 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/__init__.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.262516 pyetm-1.0.0/src/pyetm/client/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       52 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4631 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/account.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10187 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/client.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4067 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/curves.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11611 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/customcurves.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2279 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/gqueries.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4032 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/meritorder.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12654 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/parameters.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12419 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/scenario.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6737 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/session.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2256 2023-02-23 15:22:38.000000 pyetm-1.0.0/src/pyetm/client/transitionpaths.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8278 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/client/utils.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1323 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/exceptions.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.263516 pyetm-1.0.0/src/pyetm/exchange/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       45 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/exchange/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8531 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/exchange/checks.py
--rwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    27650 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/exchange/market.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11632 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/exchange/plotting.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    16503 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/exchange/region.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3231 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/logger.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.263516 pyetm-1.0.0/src/pyetm/myc/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       51 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/myc/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    29510 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/myc/model.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3578 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/optional.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.263516 pyetm-1.0.0/src/pyetm/profiles/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      119 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/profiles/__init__.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.263516 pyetm-1.0.0/src/pyetm/profiles/capacityfactors/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4770 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/profiles/capacityfactors/__init__.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.264515 pyetm-1.0.0/src/pyetm/profiles/weather/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3046 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/profiles/weather/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5718 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/profiles/weather/buildings.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2718 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/profiles/weather/cooling.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10702 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/profiles/weather/households.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5984 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/profiles/weather/smoothing.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.264515 pyetm-1.0.0/src/pyetm/sessions/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      101 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/sessions/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10546 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/sessions/aiohttp.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7600 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/sessions/requests.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.265516 pyetm-1.0.0/src/pyetm/utils/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      277 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4987 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/categorisation.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5115 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/converter.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7153 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/excel.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6207 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/interpolation.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      503 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/lookup.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      559 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/loop.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3704 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/profiles.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4990 2023-04-24 21:36:47.000000 pyetm-1.0.0/src/pyetm/utils/regionalisation.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.261515 pyetm-1.0.0/src/pyetm.egg-info/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-04-24 21:40:47.000000 pyetm-1.0.0/src/pyetm.egg-info/PKG-INFO
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1486 2023-04-24 21:40:47.000000 pyetm-1.0.0/src/pyetm.egg-info/SOURCES.txt
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        1 2023-04-24 21:40:47.000000 pyetm-1.0.0/src/pyetm.egg-info/dependency_links.txt
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      177 2023-04-24 21:40:47.000000 pyetm-1.0.0/src/pyetm.egg-info/requires.txt
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        6 2023-04-24 21:40:47.000000 pyetm-1.0.0/src/pyetm.egg-info/top_level.txt
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-24 21:40:47.265516 pyetm-1.0.0/tests/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1709 2023-04-24 21:36:47.000000 pyetm-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.924389 pyetm-1.1.0/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    13827 2023-01-10 21:51:08.000000 pyetm-1.1.0/LICENSE
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-04-26 11:30:47.923390 pyetm-1.1.0/PKG-INFO
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      253 2023-01-10 21:51:08.000000 pyetm-1.1.0/README.md
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1324 2023-04-26 11:28:26.000000 pyetm-1.1.0/pyproject.toml
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       38 2023-04-26 11:30:47.924389 pyetm-1.1.0/setup.cfg
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.917389 pyetm-1.1.0/src/
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.918390 pyetm-1.1.0/src/pyetm/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       50 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/__init__.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.920390 pyetm-1.1.0/src/pyetm/client/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       52 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4631 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/account.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10187 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/client.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6621 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/client/curves.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11611 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/customcurves.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2279 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/gqueries.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4032 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/meritorder.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12654 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/parameters.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12419 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/scenario.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6737 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/session.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2256 2023-02-23 15:22:38.000000 pyetm-1.1.0/src/pyetm/client/transitionpaths.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8278 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/utils.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1323 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exceptions.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/exchange/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       45 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8531 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/checks.py
+-rwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    27650 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/market.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11632 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/plotting.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    16503 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/region.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3231 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/logger.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/myc/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       51 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/myc/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    29789 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/myc/model.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3578 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/optional.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/profiles/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      119 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/__init__.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/profiles/capacityfactors/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4770 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/capacityfactors/__init__.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.922390 pyetm-1.1.0/src/pyetm/profiles/weather/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3046 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5718 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/buildings.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2718 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/cooling.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10702 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/households.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5984 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/smoothing.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.922390 pyetm-1.1.0/src/pyetm/sessions/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      101 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/sessions/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10546 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/sessions/aiohttp.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7600 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/sessions/requests.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.923390 pyetm-1.1.0/src/pyetm/utils/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      278 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/utils/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4987 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/categorisation.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5131 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/utils/converter.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7153 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/excel.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6207 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/utils/interpolation.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      503 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/lookup.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      559 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/loop.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3704 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/profiles.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4990 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/regionalisation.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.919390 pyetm-1.1.0/src/pyetm.egg-info/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/PKG-INFO
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1486 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/SOURCES.txt
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        1 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/dependency_links.txt
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      177 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/requires.txt
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        6 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/top_level.txt
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.923390 pyetm-1.1.0/tests/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1709 2023-04-24 21:36:47.000000 pyetm-1.1.0/tests/test_utils.py
```

### Comparing `pyetm-1.0.0/LICENSE` & `pyetm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/PKG-INFO` & `pyetm-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyetm
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python-ETM Connector
 Author-email: Rob Calon <robcalon@protonmail.com>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
```

### Comparing `pyetm-1.0.0/pyproject.toml` & `pyetm-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyetm"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python-ETM Connector"
 authors = [{name = "Rob Calon", email = "robcalon@protonmail.com"}]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 dependencies = ['requests>=2.26', 'pandas>=2.0']
 keywords = ["ETM", "Energy Transition Model"]
```

### Comparing `pyetm-1.0.0/src/pyetm/client/account.py` & `pyetm-1.1.0/src/pyetm/client/account.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/client.py` & `pyetm-1.1.0/src/pyetm/client/client.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/customcurves.py` & `pyetm-1.1.0/src/pyetm/client/customcurves.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/gqueries.py` & `pyetm-1.1.0/src/pyetm/client/gqueries.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/meritorder.py` & `pyetm-1.1.0/src/pyetm/client/meritorder.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/parameters.py` & `pyetm-1.1.0/src/pyetm/client/parameters.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/scenario.py` & `pyetm-1.1.0/src/pyetm/client/scenario.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/session.py` & `pyetm-1.1.0/src/pyetm/client/session.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/transitionpaths.py` & `pyetm-1.1.0/src/pyetm/client/transitionpaths.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/client/utils.py` & `pyetm-1.1.0/src/pyetm/client/utils.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/exceptions.py` & `pyetm-1.1.0/src/pyetm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/exchange/checks.py` & `pyetm-1.1.0/src/pyetm/exchange/checks.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/exchange/market.py` & `pyetm-1.1.0/src/pyetm/exchange/market.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/exchange/plotting.py` & `pyetm-1.1.0/src/pyetm/exchange/plotting.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/exchange/region.py` & `pyetm-1.1.0/src/pyetm/exchange/region.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/logger.py` & `pyetm-1.1.0/src/pyetm/logger.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/myc/model.py` & `pyetm-1.1.0/src/pyetm/myc/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -214,16 +214,16 @@
             Optional mapping for carrier curves output keys.
         reference : str, default None
             Key of reference scenario. This scenario will be
             excluded from the MYC links and will always be
             placed in front when sorting results.
 
         All key-word arguments are passed directly to the Session
-        that is used in combination with the pyETM.client. In this
-        module the pyETM.Client uses a Requests Session object as
+        that is used in combination with the pyetm.client. In this
+        module the pyetm.Client uses a Requests Session object as
         backend.
 
         Keyword Arguments
         -----------------
         base_url: str, default None
             Base url to which the session connects, all request urls
             will be merged with the base url to create a destination.
@@ -541,27 +541,31 @@
                     # connect scenario and get curves
                     client.scenario_id = scenario_id
 
                     # get method for carrier curves
                     attr = f"hourly_{carrier}_curves"
                     curves = getattr(client, attr)
 
+                    # continue with disabled merit order
+                    if curves.empty:
+                        continue
+
                     # set column name
                     curves.columns.names = ['KEY']
 
                     # check for categorisation
                     if mapping is not None:
 
                         # categorise curves
                         curves = categorise_curves(
                             curves, mapping, columns=columns,
                             include_keys=include_keys, invert_sign=invert_sign)
 
                     # append curves to list
-                    items.append(curves)
+                    items.append(curves.reset_index(drop=True))
 
         # handle exception
         except Exception as exc:
             log_exception(exc, logger=_logger)
 
         # construct frame for carrier
         frame = pd.concat(items, axis=1, keys=midx)
@@ -595,16 +599,20 @@
                     _logger.debug("> collecting hourly price curve for " +
                         "'%s', '%s', '%s', '%s'", *case)
 
                     # connect scenario and get curves
                     client.scenario_id = scenario_id
                     curves = client.hourly_electricity_price_curve
 
+                    # continue with disabled merit order
+                    if curves.empty:
+                        continue
+
                     # append curves to list
-                    items.append(curves)
+                    items.append(curves.reset_index(drop=True))
 
         # handle exception
         except Exception as exc:
             log_exception(exc, logger=_logger)
 
         # construct frame for carrier
         frame = pd.concat(items, axis=1, keys=midx)
@@ -718,19 +726,19 @@
         urls += "?title=" + urls.index.to_series().str.join("%20")
 
         return pd.Series(urls, name='URL').sort_index()
 
     def to_excel(self,
         filepath: str | None = None,
         midx: tuple | pd.MultiIndex | None = None,
-        input_parameters: pd.DataFrame | None = None,
-        output_values: pd.DataFrame | None = None,
-        myc_urls: pd.Series | None = None,
-        include_hourly_curves: bool = False,
-        include_price_curves: bool = False,
+        input_parameters: bool | pd.DataFrame = True,
+        output_values: bool | pd.DataFrame = True,
+        myc_urls: bool | pd.Series = True,
+        hourly_carrier_curves: bool = False,
+        hourly_price_curves: bool = False,
         carriers: Carrier | list[Carrier] | None = None,
         mapping: pd.DataFrame | None = None,
         columns: list[str] | None = None,
         include_keys: bool = False,
         invert_sign: bool = False,
         ) -> None:
         """Export results of model to Excel.
@@ -741,37 +749,34 @@
             File path or existing ExcelWriter, defaults
             to filename with current datetime in current
             working directory.
         midx : tuple or pd.MultiIndex, default None
             Tuple or MultiIndex with column names
             of columns to include in file. Defaults
             to all columns.
-        input_parameters : pd.DataFrame, default None
-            DataFrame to write on the inputs sheet
-            of the Excel. Defaults to get_input_values
-            method with specified midx.
-        output_values : pd.DataFrame, default None
-            DataFrame to write on the outputs sheet
-            of the Excel. Defaults to get_output_values
-            method with specified midx.
-        myc_urls : pd.Series, default None
-            Series to write on the url sheet
-            of the Excel. Default to make_myc_urls
-            method with specified midx.
-        include_hourly_curves : bool, default False
+        input_parameters : bool or pd.DataFrame, default True
+            Include input parameters in export. Can be overwritten with
+            custom parameters by passing a DataFrame instead.
+        output_values : bool or pd.DataFrame, default True
+            Include gquery results in export. Can be overwritten with
+            custom curves by passing a DataFrame instead.
+        myc_urls : bool or pd.Series, default True
+            Include myc urls in export. Can be overwritten with
+            custom myc urls by passing a Series instead.
+        hourly_carrier_curves : bool, default False
             Include hourly carrier curves for specified
             carriers in exported result. Defaults to
             exclude carriers.
-        include_price_curves : bool, default False
+        hourly_price_curves : bool, default False
             Include hourly price curves for the
             selected session ids. Defaults to exclude
             the price curves.
         carriers : str | list, default None
             Carrier of list of carriers to export when
-            including hourlu carrier curves. Defaults
+            including hourly carrier curves. Defaults
             to include all carriers.
         mapping : DataFrame, default None
             DataFrame with mapping of ETM keys and carrier in a multiindex
             and mapping values in columns. Defaults to mapping passed on
             initialisation or is excluded when not passed on model
             initialisation.
         columns : list, default None
@@ -828,59 +833,56 @@
         if not Path(filepath).parent.exists:
             raise FileNotFoundError("Path to file does not exist: '{filepath}'")
 
         # create workbook
         workbook = xlsxwriter.Workbook(str(filepath))
 
         # default inputs
-        if input_parameters is None:
+        if input_parameters is True:
             input_parameters = self.get_input_parameters(midx=midx)
 
-        # add inputs to workbook
-        add_frame('INPUT_PARAMETERS', input_parameters, workbook,
-            index_width=[80, 18], column_width=18)
+        # write input parameters
+        if input_parameters is not False:
+            add_frame('INPUT_PARAMETERS', input_parameters, workbook,
+                index_width=[80, 18], column_width=18)
 
         # default outputs
-        if output_values is None:
+        if output_values is True:
             output_values = self.get_output_values(midx=midx)
 
-        # add outputs to workbook
-        add_frame('OUTPUT_VALUES', output_values, workbook,
-            index_width=[80, 18], column_width=18)
-
-        """Allow for modified carrier curves as well"""
+        # write output values
+        if output_values is not False:
+            add_frame('OUTPUT_VALUES', output_values, workbook,
+                index_width=[80, 18], column_width=18)
 
         # iterate over carriers
-        if include_hourly_curves:
+        if hourly_carrier_curves is True:
             for carrier in carriers:
 
                 # get carrier curves
                 curves = self.get_hourly_carrier_curves(carrier,
                     midx=midx, mapping=mapping, columns=columns,
                     include_keys=include_keys, invert_sign=invert_sign)
 
                 # add to excel
                 name = carrier.upper()
                 add_frame(name, curves, workbook, column_width=18)
 
-        """Allow for modified price curves as well"""
-
-        # include price curves
-        if include_price_curves:
-
-            # get and add hourly price curves
+        # include hourly price curves
+        if hourly_price_curves is True:
             curves = self.get_hourly_price_curves(midx=midx)
             add_frame('EPRICE', curves, workbook, column_width=18)
 
         # default urls
-        if myc_urls is None:
+        if myc_urls is True:
             myc_urls = self.make_myc_urls(midx=midx)
 
         # add urls to workbook
-        if not myc_urls.empty:
-            add_series('ETM_URLS', myc_urls, workbook,
-                index_width=18, column_width=80)
+        if myc_urls is not False:
+            if not myc_urls.empty:
+                add_series('ETM_URLS', myc_urls, workbook,
+                    index_width=18, column_width=80)
 
         # write workbook
         workbook.close()
 
         _logger.info("exported results to '%s'", filepath)
```

### Comparing `pyetm-1.0.0/src/pyetm/optional.py` & `pyetm-1.1.0/src/pyetm/optional.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/profiles/capacityfactors/__init__.py` & `pyetm-1.1.0/src/pyetm/profiles/capacityfactors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/profiles/weather/__init__.py` & `pyetm-1.1.0/src/pyetm/profiles/weather/__init__.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/profiles/weather/buildings.py` & `pyetm-1.1.0/src/pyetm/profiles/weather/buildings.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/profiles/weather/cooling.py` & `pyetm-1.1.0/src/pyetm/profiles/weather/cooling.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/profiles/weather/households.py` & `pyetm-1.1.0/src/pyetm/profiles/weather/households.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/profiles/weather/smoothing.py` & `pyetm-1.1.0/src/pyetm/profiles/weather/smoothing.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/sessions/aiohttp.py` & `pyetm-1.1.0/src/pyetm/sessions/aiohttp.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/sessions/requests.py` & `pyetm-1.1.0/src/pyetm/sessions/requests.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/utils/categorisation.py` & `pyetm-1.1.0/src/pyetm/utils/categorisation.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/utils/converter.py` & `pyetm-1.1.0/src/pyetm/utils/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """conversion methods"""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 import pandas as pd
 
 from pyetm import Client
-from pyetm.myc import Model
+from pyetm.myc import MYCClient
 from pyetm.logger import get_modulelogger
 from pyetm.optional import import_optional_dependency
 
 _logger = get_modulelogger(__name__)
 
-def copy_study_session_ids(session_ids: pd.Series | Model,
+def copy_study_session_ids(session_ids: pd.Series | MYCClient,
     study: str | None = None, metadata: dict | None = None,
     keep_compatible: bool = False, **kwargs) -> pd.Series:
     """make a copy of an existing study. The returned
     session ids are decoupled from the original study,
     but contain the same values"""
 
     # load study session ids from model
-    if isinstance(session_ids, Model):
+    if isinstance(session_ids, MYCClient):
         kwargs = {**session_ids._kwargs, **kwargs}
         session_ids = session_ids.session_ids.copy()
 
     # make series-like object
     if not isinstance(session_ids, pd.Series):
         session_ids = pd.Series(session_ids, name='SESSION')
 
@@ -42,24 +42,24 @@
 
     # set study if applicable
     if study is not None:
         session_ids = session_ids.index.set_levels([study], level='STUDY')
 
     return session_ids
 
-def copy_study_configuration(filepath: str, model: Model,
+def copy_study_configuration(filepath: str, model: MYCClient,
     study: str | None = None, copy_session_ids: bool = True,
     metadata: dict | None = None, keep_compatible: bool = False) -> None:
     """copy study configuration"""
 
     # pylint: disable=C0415
     # Due to optional import
 
     from pathlib import Path
-    from pyETM.utils import add_series, add_frame
+    from pyetm.utils import add_series, add_frame
 
     if TYPE_CHECKING:
         # import xlsxwriter
         import xlsxwriter
 
     else:
         # import optional dependency
```

### Comparing `pyetm-1.0.0/src/pyetm/utils/excel.py` & `pyetm-1.1.0/src/pyetm/utils/excel.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/utils/interpolation.py` & `pyetm-1.1.0/src/pyetm/utils/interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #     Do note that the heat network order is not returned or
 #     interpolated by this function.
 
 #     Parameters
 #     ----------
 #     clients: list
-#         List of pyETM.client.Client objects that
+#         List of pyetm.client.Client objects that
 #         are used to interpolate the scenario.
 #     cfill : string, default 'linear'
 #         Method for filling continious user values
 #         between years of passed scenarios. Passed
 #         method is directly passed to interpolation
 #         function of a DataFrame.
 #     dfill : string, default 'ffill'
@@ -50,16 +50,16 @@
 
 #         # check if clients in listlike object
 #         if not isinstance(clients, list):
 #             clients = list(clients)
 
 #         # check client in list
 #         for client in clients:
-#             if not isinstance(client, pyETM.Client):
-#                 raise TypeError('client must be of type pyETM.client.Client')
+#             if not isinstance(client, pyetm.Client):
+#                 raise TypeError('client must be of type pyetm.client.Client')
 
 #         # validate area codes and sort area codes
 #         self._validate_area_codes(clients)
 #         clients = self._sort_clients(clients)
 
 #         # check scenario parameters
 #         self._validate_scenario_parameters(clients)
@@ -69,15 +69,15 @@
 
 #     def __init__(self, clients):
 #         """"initialize interpolator
 
 #         Parameters
 #         ----------
 #         clients : list
-#             List of pyETM.client.Client objects that
+#             List of pyetm.client.Client objects that
 #             are used to interpolate the scenario. Clients
 #             are by end year on initialization."""
 
 #         # set clients
 #         self.clients = clients
 
 #     def interpolate(self, cfill='linear', dfill='ffill'):
```

### Comparing `pyetm-1.0.0/src/pyetm/utils/loop.py` & `pyetm-1.1.0/src/pyetm/utils/loop.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/utils/profiles.py` & `pyetm-1.1.0/src/pyetm/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm/utils/regionalisation.py` & `pyetm-1.1.0/src/pyetm/utils/regionalisation.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/src/pyetm.egg-info/PKG-INFO` & `pyetm-1.1.0/src/pyetm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyetm
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python-ETM Connector
 Author-email: Rob Calon <robcalon@protonmail.com>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
```

### Comparing `pyetm-1.0.0/src/pyetm.egg-info/SOURCES.txt` & `pyetm-1.1.0/src/pyetm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyetm-1.0.0/tests/test_utils.py` & `pyetm-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

