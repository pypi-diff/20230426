# Comparing `tmp/saqc-2.3.tar.gz` & `tmp/saqc-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saqc-2.3.tar", last modified: Tue Jan 17 20:08:41 2023, max compression
+gzip compressed data, was "saqc-2.4.0.tar", last modified: Tue Apr 25 21:43:39 2023, max compression
```

## Comparing `saqc-2.3.tar` & `saqc-2.4.0.tar`

### file list

```diff
@@ -1,130 +1,103 @@
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.157066 saqc-2.3/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2796 2022-07-08 08:06:22.000000 saqc-2.3/LICENSE.md
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.147065 saqc-2.3/LICENSES/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    34670 2022-07-08 08:06:22.000000 saqc-2.3/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5889 2023-01-17 20:08:41.157066 saqc-2.3/PKG-INFO
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5481 2022-07-08 10:01:10.000000 saqc-2.3/README.md
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.150399 saqc-2.3/dios/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      171 2022-07-08 08:06:22.000000 saqc-2.3/dios/__init__.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.150399 saqc-2.3/dios/dios/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      596 2022-07-08 10:01:10.000000 saqc-2.3/dios/dios/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    24270 2022-10-28 10:02:41.000000 saqc-2.3/dios/dios/base.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    44258 2022-09-29 09:17:59.000000 saqc-2.3/dios/dios/dios.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    17110 2022-07-08 10:01:10.000000 saqc-2.3/dios/dios/indexer.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11590 2022-07-08 10:01:10.000000 saqc-2.3/dios/dios/lib.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      760 2022-07-08 10:01:10.000000 saqc-2.3/dios/dios/operators.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      639 2022-07-08 10:01:10.000000 saqc-2.3/dios/dios/pandas_bridge.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.150399 saqc-2.3/dios/profiling/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      226 2022-07-08 08:06:22.000000 saqc-2.3/dios/profiling/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3327 2022-07-08 10:01:10.000000 saqc-2.3/dios/profiling/generate_testsets.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2880 2022-07-08 10:01:10.000000 saqc-2.3/dios/profiling/memory.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5564 2022-07-08 10:01:10.000000 saqc-2.3/dios/profiling/performance.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1014 2022-07-08 10:01:10.000000 saqc-2.3/dios/setup.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.150399 saqc-2.3/dios/test/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      154 2022-07-08 08:06:22.000000 saqc-2.3/dios/test/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1538 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/run_dios.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2943 2022-10-28 10:02:41.000000 saqc-2.3/dios/test/test__ops__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1563 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test__setget__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1978 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test__setget__aloc.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1072 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test__setget__iloc.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1680 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test__setget__loc.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1098 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test__setitem__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1517 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test_dflike.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2514 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test_dflike__setget__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      489 2022-07-08 08:06:22.000000 saqc-2.3/dios/test/test_magic_methods.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1661 2022-07-08 08:06:22.000000 saqc-2.3/dios/test/test_methods.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9164 2022-07-08 10:01:10.000000 saqc-2.3/dios/test/test_setup.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      346 2022-07-08 10:01:10.000000 saqc-2.3/pyproject.toml
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.150399 saqc-2.3/saqc/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      453 2022-07-08 10:01:10.000000 saqc-2.3/saqc/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3502 2022-07-08 10:01:10.000000 saqc-2.3/saqc/__main__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3490 2022-10-28 10:02:41.000000 saqc-2.3/saqc/constants.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.153732 saqc-2.3/saqc/core/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      487 2022-07-08 10:01:10.000000 saqc-2.3/saqc/core/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7759 2022-12-20 09:39:49.000000 saqc-2.3/saqc/core/core.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    15856 2022-12-20 09:39:49.000000 saqc-2.3/saqc/core/flags.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18070 2022-12-20 09:39:49.000000 saqc-2.3/saqc/core/history.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1180 2022-06-29 17:19:03.000000 saqc-2.3/saqc/core/mixins.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2809 2022-07-08 10:01:10.000000 saqc-2.3/saqc/core/reader.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16141 2023-01-17 07:22:28.000000 saqc-2.3/saqc/core/register.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.153732 saqc-2.3/saqc/core/translation/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      424 2022-12-20 09:39:49.000000 saqc-2.3/saqc/core/translation/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7067 2022-12-20 09:39:49.000000 saqc-2.3/saqc/core/translation/basescheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6397 2022-12-20 09:39:49.000000 saqc-2.3/saqc/core/translation/dmpscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1534 2022-12-20 08:45:34.000000 saqc-2.3/saqc/core/translation/floatscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2770 2022-12-20 09:39:49.000000 saqc-2.3/saqc/core/translation/positionalscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4804 2022-07-08 08:06:22.000000 saqc-2.3/saqc/core/visitor.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.153732 saqc-2.3/saqc/funcs/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1330 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7311 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/breaks.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    13806 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/changepoints.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4834 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/constants.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9302 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/curvefit.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    29263 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/drift.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16980 2023-01-17 14:22:46.000000 saqc-2.3/saqc/funcs/flagtools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11556 2022-11-21 12:53:23.000000 saqc-2.3/saqc/funcs/generic.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    10535 2023-01-13 10:01:29.000000 saqc-2.3/saqc/funcs/interpolation.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2496 2022-12-08 11:28:19.000000 saqc-2.3/saqc/funcs/noise.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    49135 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/outliers.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6480 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/pattern.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20631 2023-01-17 13:54:56.000000 saqc-2.3/saqc/funcs/resampling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5122 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/residuals.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4803 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/rolling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11972 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/scores.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12418 2023-01-17 14:21:42.000000 saqc-2.3/saqc/funcs/tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2309 2022-10-28 10:02:41.000000 saqc-2.3/saqc/funcs/transformation.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.153732 saqc-2.3/saqc/lib/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.3/saqc/lib/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5751 2022-07-08 10:01:10.000000 saqc-2.3/saqc/lib/docurator.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9518 2023-01-10 10:55:08.000000 saqc-2.3/saqc/lib/plotting.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12360 2022-07-08 10:01:10.000000 saqc-2.3/saqc/lib/rolling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20491 2023-01-13 10:09:06.000000 saqc-2.3/saqc/lib/tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    17978 2023-01-13 10:01:29.000000 saqc-2.3/saqc/lib/ts_operators.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1305 2022-10-28 10:02:41.000000 saqc-2.3/saqc/lib/types.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      171 2023-01-17 13:49:11.000000 saqc-2.3/saqc/version.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.150399 saqc-2.3/saqc.egg-info/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5889 2023-01-17 20:08:41.000000 saqc-2.3/saqc.egg-info/PKG-INFO
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2743 2023-01-17 20:08:41.000000 saqc-2.3/saqc.egg-info/SOURCES.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)        1 2023-01-17 20:08:41.000000 saqc-2.3/saqc.egg-info/dependency_links.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       44 2023-01-17 20:08:41.000000 saqc-2.3/saqc.egg-info/entry_points.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      119 2023-01-17 20:08:41.000000 saqc-2.3/saqc.egg-info/requires.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       16 2023-01-17 20:08:41.000000 saqc-2.3/saqc.egg-info/top_level.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       38 2023-01-17 20:08:41.157066 saqc-2.3/setup.cfg
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1576 2023-01-17 13:54:56.000000 saqc-2.3/setup.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.147065 saqc-2.3/tests/
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.157066 saqc-2.3/tests/api/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.3/tests/api/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      542 2022-07-08 10:01:10.000000 saqc-2.3/tests/api/test_creation.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.157066 saqc-2.3/tests/cli/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.3/tests/cli/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3556 2022-10-28 10:02:41.000000 saqc-2.3/tests/cli/test_integration.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.157066 saqc-2.3/tests/core/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.3/tests/core/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    10018 2022-10-28 10:02:41.000000 saqc-2.3/tests/core/test_core.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9450 2022-07-08 10:01:10.000000 saqc-2.3/tests/core/test_flags.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6164 2022-12-20 09:39:49.000000 saqc-2.3/tests/core/test_history.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4205 2022-10-28 10:02:41.000000 saqc-2.3/tests/core/test_reader.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8579 2022-12-20 09:39:49.000000 saqc-2.3/tests/core/test_translator.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.157066 saqc-2.3/tests/funcs/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.3/tests/funcs/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1289 2022-10-28 10:02:41.000000 saqc-2.3/tests/funcs/test_constants_detection.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4200 2022-10-27 12:16:09.000000 saqc-2.3/tests/funcs/test_curvefit.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4353 2023-01-17 14:09:46.000000 saqc-2.3/tests/funcs/test_flagtools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9303 2023-01-17 14:08:03.000000 saqc-2.3/tests/funcs/test_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6613 2022-10-28 10:02:41.000000 saqc-2.3/tests/funcs/test_generic_api_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8531 2022-10-28 10:02:41.000000 saqc-2.3/tests/funcs/test_generic_config_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5505 2022-10-28 10:02:41.000000 saqc-2.3/tests/funcs/test_outlier_detection.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1273 2022-10-28 10:02:41.000000 saqc-2.3/tests/funcs/test_pattern_rec.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4778 2023-01-13 10:01:29.000000 saqc-2.3/tests/funcs/test_proc_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12283 2023-01-13 10:01:29.000000 saqc-2.3/tests/funcs/test_resampling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1113 2023-01-17 13:54:56.000000 saqc-2.3/tests/funcs/test_tools.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.157066 saqc-2.3/tests/fuzzy/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.3/tests/fuzzy/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4972 2022-07-08 10:01:10.000000 saqc-2.3/tests/fuzzy/lib.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5650 2022-10-28 10:02:41.000000 saqc-2.3/tests/fuzzy/test_masking.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-01-17 20:08:41.157066 saqc-2.3/tests/lib/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.3/tests/lib/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2882 2022-07-08 10:01:10.000000 saqc-2.3/tests/lib/test_periodicMask.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7745 2022-07-08 10:01:10.000000 saqc-2.3/tests/lib/test_rolling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2733 2022-07-08 10:01:10.000000 saqc-2.3/tests/lib/test_tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5350 2023-01-13 10:01:29.000000 saqc-2.3/tests/lib/test_ts_operators.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.163224 saqc-2.4.0/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2796 2022-11-18 08:39:03.000000 saqc-2.4.0/LICENSE.md
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.153225 saqc-2.4.0/LICENSES/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    34670 2022-11-18 08:39:03.000000 saqc-2.4.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6130 2023-04-25 21:43:39.163224 saqc-2.4.0/PKG-INFO
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5720 2023-04-25 20:52:46.000000 saqc-2.4.0/README.md
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      346 2022-11-18 08:39:03.000000 saqc-2.4.0/pyproject.toml
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      550 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3507 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/__main__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1604 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/constants.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/core/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      414 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8452 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/core.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16823 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/flags.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5563 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/frame.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18033 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/history.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16349 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/register.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/core/translation/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      466 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7188 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/basescheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6355 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/dmpscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2766 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/positionalscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      760 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/simplescheme.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/funcs/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1330 2022-11-18 08:39:03.000000 saqc-2.4.0/saqc/funcs/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6685 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/breaks.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    13510 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/changepoints.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5010 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/constants.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8250 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/curvefit.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    27888 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/drift.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19297 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/flagtools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8968 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/generic.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20621 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/interpolation.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2531 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/noise.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    58930 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/outliers.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6466 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/pattern.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    15415 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/resampling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4684 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/residuals.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6222 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/rolling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19477 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/scores.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11417 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1943 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/transformation.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/saqc/lib/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/saqc/lib/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3237 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/docs.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9483 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/plotting.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5073 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/rolling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18924 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19963 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/ts_operators.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      942 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/types.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/saqc/parsing/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2303 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/environ.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2800 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/reader.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5704 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/visitor.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      173 2023-04-25 21:43:10.000000 saqc-2.4.0/saqc/version.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc.egg-info/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6130 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/PKG-INFO
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2127 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/SOURCES.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)        1 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/dependency_links.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       44 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/entry_points.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      122 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/requires.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       11 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/top_level.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       38 2023-04-25 21:43:39.163224 saqc-2.4.0/setup.cfg
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1590 2023-04-25 21:30:42.000000 saqc-2.4.0/setup.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/api/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/api/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      538 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/api/test_creation.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/cli/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/cli/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3560 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/cli/test_integration.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/core/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/core/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11372 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_core.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11200 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_flags.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      262 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_frame.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6164 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_history.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4737 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_reader.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8529 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_translator.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/funcs/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/funcs/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1323 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_constants_detection.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7810 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_flagtools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9332 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6300 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_generic_api_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8453 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_generic_config_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6465 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_outlier_detection.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1254 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_pattern_rec.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4715 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_proc_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12142 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_resampling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1111 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_tools.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/fuzzy/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/fuzzy/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4968 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/fuzzy/lib.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5991 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/fuzzy/test_masking.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.163224 saqc-2.4.0/tests/lib/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/lib/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2882 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/lib/test_periodicMask.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1747 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/lib/test_tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7063 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/lib/test_ts_operators.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      531 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/test__main__.py
```

### Comparing `saqc-2.3/LICENSE.md` & `saqc-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saqc-2.3/LICENSES/GPL-3.0-or-later.txt` & `saqc-2.4.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `saqc-2.3/PKG-INFO` & `saqc-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,369 +1,384 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7361 7163  : 2.1.Name: saqc
-00000020: 0a56 6572 7369 6f6e 3a20 322e 330a 5375  .Version: 2.3.Su
-00000030: 6d6d 6172 793a 2041 2074 696d 6573 6572  mmary: A timeser
-00000040: 6965 7320 6461 7461 2071 7561 6c69 7479  ies data quality
-00000050: 2063 6f6e 7472 6f6c 2061 6e64 2070 726f   control and pro
-00000060: 6365 7373 696e 6720 746f 6f6c 2f66 7261  cessing tool/fra
-00000070: 6d65 776f 726b 0a48 6f6d 652d 7061 6765  mework.Home-page
-00000080: 3a20 6874 7470 733a 2f2f 6769 742e 7566  : https://git.uf
-00000090: 7a2e 6465 2f72 646d 2d73 6f66 7477 6172  z.de/rdm-softwar
-000000a0: 652f 7361 7163 0a41 7574 686f 723a 2042  e/saqc.Author: B
-000000b0: 6572 7420 5061 6c6d 2c20 4461 7669 6420  ert Palm, David 
-000000c0: 5363 6861 6566 6572 2c20 466c 6f72 6961  Schaefer, Floria
-000000d0: 6e20 4772 616e 7365 652c 2050 6574 6572  n Gransee, Peter
-000000e0: 204c 7565 6e65 6e73 6368 6c6f 7373 0a41   Luenenschloss.A
-000000f0: 7574 686f 722d 656d 6169 6c3a 2064 6176  uthor-email: dav
-00000100: 6964 2e73 6368 6165 6665 7240 7566 7a2e  id.schaefer@ufz.
-00000110: 6465 0a52 6571 7569 7265 732d 5079 7468  de.Requires-Pyth
-00000120: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
-00000130: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000140: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000150: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000160: 4c49 4345 4e53 452e 6d64 0a4c 6963 656e  LICENSE.md.Licen
-00000170: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000180: 532f 4750 4c2d 332e 302d 6f72 2d6c 6174  S/GPL-3.0-or-lat
-00000190: 6572 2e74 7874 0a0a 3c21 2d2d 0a53 5044  er.txt..<!--.SPD
-000001a0: 582d 4669 6c65 436f 7079 7269 6768 7454  X-FileCopyrightT
-000001b0: 6578 743a 2032 3032 3120 4865 6c6d 686f  ext: 2021 Helmho
-000001c0: 6c74 7a2d 5a65 6e74 7275 6d20 66c3 bc72  ltz-Zentrum f..r
-000001d0: 2055 6d77 656c 7466 6f72 7363 6875 6e67   Umweltforschung
-000001e0: 2047 6d62 4820 2d20 5546 5a0a 0a53 5044   GmbH - UFZ..SPD
-000001f0: 582d 4c69 6365 6e73 652d 4964 656e 7469  X-License-Identi
-00000200: 6669 6572 3a20 4750 4c2d 332e 302d 6f72  fier: GPL-3.0-or
-00000210: 2d6c 6174 6572 0a2d 2d3e 0a0a 3c61 2068  -later.-->..<a h
-00000220: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
-00000230: 2e75 667a 2e64 652f 696e 6465 782e 7068  .ufz.de/index.ph
-00000240: 703f 656e 3d33 3335 3733 223e 0a20 2020  p?en=33573">.   
-00000250: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000260: 3a2f 2f67 6974 2e75 667a 2e64 652f 7264  ://git.ufz.de/rd
-00000270: 6d2d 736f 6674 7761 7265 2f73 6171 632f  m-software/saqc/
-00000280: 7261 772f 6465 7665 6c6f 702f 646f 6373  raw/develop/docs
-00000290: 2f72 6573 6f75 7263 6573 2f69 6d61 6765  /resources/image
-000002a0: 732f 7265 7072 6573 656e 7461 7469 7665  s/representative
-000002b0: 2f55 465a 4c6f 676f 2e70 6e67 2220 7769  /UFZLogo.png" wi
-000002c0: 6474 683d 2234 3030 222f 3e0a 3c2f 613e  dth="400"/>.</a>
-000002d0: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-000002e0: 3a2f 2f77 7777 2e75 667a 2e64 652f 696e  ://www.ufz.de/in
-000002f0: 6465 782e 7068 703f 656e 3d34 3533 3438  dex.php?en=45348
-00000300: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
-00000310: 2268 7474 7073 3a2f 2f67 6974 2e75 667a  "https://git.ufz
-00000320: 2e64 652f 7264 6d2d 736f 6674 7761 7265  .de/rdm-software
-00000330: 2f73 6171 632f 7261 772f 6465 7665 6c6f  /saqc/raw/develo
-00000340: 702f 646f 6373 2f72 6573 6f75 7263 6573  p/docs/resources
-00000350: 2f69 6d61 6765 732f 7265 7072 6573 656e  /images/represen
-00000360: 7461 7469 7665 2f52 444d 4c6f 676f 2e70  tative/RDMLogo.p
-00000370: 6e67 2220 616c 6967 6e3d 2272 6967 6874  ng" align="right
-00000380: 2220 7769 6474 683d 2232 3230 222f 3e0a  " width="220"/>.
-00000390: 3c2f 613e 0a0a 5b21 5b50 726f 6a65 6374  </a>..[![Project
-000003a0: 2053 7461 7475 733a 2041 6374 6976 6520   Status: Active 
-000003b0: e280 9320 5468 6520 7072 6f6a 6563 7420  ... The project 
-000003c0: 6861 7320 7265 6163 6865 6420 6120 7374  has reached a st
-000003d0: 6162 6c65 2c20 7573 6162 6c65 2073 7461  able, usable sta
-000003e0: 7465 2061 6e64 2069 7320 6265 696e 6720  te and is being 
-000003f0: 6163 7469 7665 6c79 2064 6576 656c 6f70  actively develop
-00000400: 6564 2e5d 2868 7474 7073 3a2f 2f77 7777  ed.](https://www
-00000410: 2e72 6570 6f73 7461 7475 732e 6f72 672f  .repostatus.org/
-00000420: 6261 6467 6573 2f6c 6174 6573 742f 6163  badges/latest/ac
-00000430: 7469 7665 2e73 7667 295d 2868 7474 7073  tive.svg)](https
-00000440: 3a2f 2f77 7777 2e72 6570 6f73 7461 7475  ://www.repostatu
-00000450: 732e 6f72 672f 2361 6374 6976 6529 0a0a  s.org/#active)..
-00000460: 0a23 2053 7973 7465 6d20 666f 7220 6175  .# System for au
-00000470: 746f 6d61 7465 6420 5175 616c 6974 7920  tomated Quality 
-00000480: 436f 6e74 726f 6c20 2853 6151 4329 0a0a  Control (SaQC)..
-00000490: 416e 6f6d 616c 6965 7320 616e 6420 6572  Anomalies and er
-000004a0: 726f 7273 2061 7265 2074 6865 2072 756c  rors are the rul
-000004b0: 6520 6e6f 7420 7468 6520 6578 6365 7074  e not the except
-000004c0: 696f 6e20 7768 656e 2077 6f72 6b69 6e67  ion when working
-000004d0: 2077 6974 6820 0a74 696d 6520 7365 7269   with .time seri
-000004e0: 6573 2064 6174 612e 2054 6869 7320 6973  es data. This is
-000004f0: 2065 7370 6563 6961 6c6c 7920 7472 7565   especially true
-00000500: 2c20 6966 2073 7563 6820 6461 7461 206f  , if such data o
-00000510: 7269 6769 6e61 7465 730a 6672 6f6d 2069  riginates.from i
-00000520: 6e2d 7369 7475 206d 6561 7375 7265 6d65  n-situ measureme
-00000530: 6e74 7320 6f66 2065 6e76 6972 6f6e 6d65  nts of environme
-00000540: 6e74 616c 2070 726f 7065 7274 6965 732e  ntal properties.
-00000550: 200a 416c 6d6f 7374 2061 6c6c 2061 7070   .Almost all app
-00000560: 6c69 6361 7469 6f6e 732c 2068 6f77 6576  lications, howev
-00000570: 6572 2c20 696d 706c 6963 696c 7920 7265  er, implicily re
-00000580: 6c79 206f 6e20 6461 7461 2c20 7468 6174  ly on data, that
-00000590: 2063 6f6d 706c 6965 730a 7769 7468 2073   complies.with s
-000005a0: 6f6d 6520 6465 6669 6e69 7469 6f6e 206f  ome definition o
-000005b0: 6620 2763 6f72 7265 6374 272e 200a 496e  f 'correct'. .In
-000005c0: 206f 7264 6572 2074 6f20 696e 6665 7220   order to infer 
-000005d0: 7265 6c69 6162 6c65 2064 6174 6120 7072  reliable data pr
-000005e0: 6f64 7563 7473 2061 6e64 2074 6f6f 6c73  oducts and tools
-000005f0: 2c20 7468 6572 6520 6973 206e 6f20 616c  , there is no al
-00000600: 7465 726e 6174 6976 650a 746f 2071 7561  ternative.to qua
-00000610: 6c69 7479 2063 6f6e 7472 6f6c 2e20 5361  lity control. Sa
-00000620: 5143 2070 726f 7669 6465 7320 616c 6c20  QC provides all 
-00000630: 7468 6520 6275 696c 6469 6e67 2062 6c6f  the building blo
-00000640: 636b 7320 746f 2063 6f6d 666f 7274 6162  cks to comfortab
-00000650: 6c79 0a62 7269 6467 6520 7468 6520 6761  ly.bridge the ga
-00000660: 7020 6265 7477 6565 6e20 2775 7375 616c  p between 'usual
-00000670: 6c79 2066 6175 6c74 7927 2061 6e64 2027  ly faulty' and '
-00000680: 6578 7065 6374 6564 2074 6f20 6265 2063  expected to be c
-00000690: 6f72 7265 6374 6564 2720 696e 200a 6120  orrected' in .a 
-000006a0: 6163 6365 7373 6962 6c65 2c20 636f 6e73  accessible, cons
-000006b0: 6973 7465 6e74 2c20 6f62 6a65 6374 6976  istent, objectiv
-000006c0: 6520 616e 6420 7265 7072 6f64 7563 6962  e and reproducib
-000006d0: 6c65 2077 6179 2e0a 0a46 6f72 2061 2028  le way...For a (
-000006e0: 636f 6e74 696e 6f75 736c 7920 696d 7072  continously impr
-000006f0: 6f76 696e 6729 206f 7665 7276 6965 7720  oving) overview 
-00000700: 6f66 2066 6561 7475 7265 732c 2074 7970  of features, typ
-00000710: 6963 616c 2075 7361 6765 2070 6174 7465  ical usage patte
-00000720: 726e 732c 0a74 6865 2073 7065 6369 6669  rns,.the specifi
-00000730: 6320 7379 7374 656d 2063 6f6d 706f 6e65  c system compone
-00000740: 6e74 7320 616e 6420 686f 7720 746f 2063  nts and how to c
-00000750: 7573 746f 6d69 7a65 2060 5361 5143 6020  ustomize `SaQC` 
-00000760: 746f 2079 6f75 7220 7370 6563 6966 6963  to your specific
-00000770: 0a6e 6565 6473 2c20 706c 6561 7365 2072  .needs, please r
-00000780: 6566 6572 2074 6f20 6f75 720a 5b6f 6e6c  efer to our.[onl
-00000790: 696e 6520 646f 6375 6d65 6e74 6174 696f  ine documentatio
-000007a0: 6e5d 2868 7474 7073 3a2f 2f72 646d 2d73  n](https://rdm-s
-000007b0: 6f66 7477 6172 652e 7061 6765 732e 7566  oftware.pages.uf
-000007c0: 7a2e 6465 2f73 6171 632f 696e 6465 782e  z.de/saqc/index.
-000007d0: 6874 6d6c 292e 0a0a 0a23 2320 496e 7374  html)....## Inst
-000007e0: 616c 6c61 7469 6f6e 0a0a 5361 5143 2069  allation..SaQC i
-000007f0: 7320 6176 6169 6c61 626c 6520 6f6e 2074  s available on t
-00000800: 6865 2050 7974 686f 6e20 5061 636b 6167  he Python Packag
-00000810: 6520 496e 6465 7820 285b 5079 5049 5d28  e Index ([PyPI](
-00000820: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000830: 2f29 2920 616e 640a 6361 6e20 6265 2069  /)) and.can be i
-00000840: 6e73 7461 6c6c 6564 2075 7369 6e67 205b  nstalled using [
-00000850: 7069 705d 2868 7474 7073 3a2f 2f70 6970  pip](https://pip
-00000860: 2e70 7970 612e 696f 2f65 6e2f 7374 6162  .pypa.io/en/stab
-00000870: 6c65 2f29 3a0a 6060 6073 680a 7079 7468  le/):.```sh.pyth
-00000880: 6f6e 202d 6d20 7069 7020 696e 7374 616c  on -m pip instal
-00000890: 6c20 7361 7163 0a60 6060 0a46 6f72 2061  l saqc.```.For a
-000008a0: 206d 6f72 6520 6465 7461 696c 6564 2069   more detailed i
-000008b0: 6e73 7461 6c6c 696f 6e20 6775 6964 652c  nstallion guide,
-000008c0: 2073 6565 2074 6865 205b 696e 7374 616c   see the [instal
-000008d0: 6c61 7469 6f6e 2067 7569 6465 5d28 6874  lation guide](ht
-000008e0: 7470 733a 2f2f 7264 6d2d 736f 6674 7761  tps://rdm-softwa
-000008f0: 7265 2e70 6167 6573 2e75 667a 2e64 652f  re.pages.ufz.de/
-00000900: 7361 7163 2f67 6574 7469 6e67 7374 6172  saqc/gettingstar
-00000910: 7465 642f 496e 7374 616c 6c61 7469 6f6e  ted/Installation
-00000920: 4775 6964 652e 6874 6d6c 292e 0a0a 2323  Guide.html)...##
-00000930: 2055 7361 6765 0a0a 6053 6151 4360 2069   Usage..`SaQC` i
-00000940: 7320 626f 7468 2c20 6120 636f 6d6d 616e  s both, a comman
-00000950: 6420 6c69 6e65 2061 7070 6c69 6361 7469  d line applicati
-00000960: 6f6e 2063 6f6e 7472 6f6c 6c65 6420 6279  on controlled by
-00000970: 2061 2074 6578 7420 6261 7365 6420 636f   a text based co
-00000980: 6e66 6967 7572 6174 696f 6e0a 616e 6420  nfiguration.and 
-00000990: 6120 7079 7468 6f6e 206d 6f64 756c 6520  a python module 
-000009a0: 7769 7468 2061 2073 696d 706c 6520 4150  with a simple AP
-000009b0: 492e 0a0a 2323 2320 5361 5143 2061 7320  I...### SaQC as 
-000009c0: 6120 636f 6d6d 616e 6420 6c69 6e65 2061  a command line a
-000009d0: 7070 6c69 6361 7469 6f6e 0a54 6865 2063  pplication.The c
-000009e0: 6f6d 6d61 6e64 206c 696e 6520 6170 706c  ommand line appl
-000009f0: 6963 6174 696f 6e20 6973 2063 6f6e 7472  ication is contr
-00000a00: 6f6c 6c65 6420 6279 2061 2073 656d 6963  olled by a semic
-00000a10: 6f6c 6f6e 2d73 6570 6172 6174 6564 2074  olon-separated t
-00000a20: 6578 740a 6669 6c65 206c 6973 7469 6e67  ext.file listing
-00000a30: 2074 6865 2076 6172 6961 626c 6573 2069   the variables i
-00000a40: 6e20 7468 6520 6461 7461 7365 7420 616e  n the dataset an
-00000a50: 6420 7468 6520 726f 7574 696e 6573 2074  d the routines t
-00000a60: 6f20 696e 7370 6563 742c 0a71 7561 6c69  o inspect,.quali
-00000a70: 7479 2063 6f6e 7472 6f6c 2061 6e64 2f6f  ty control and/o
-00000a80: 7220 7072 6f63 6573 7320 7468 656d 2e20  r process them. 
-00000a90: 5468 6520 636f 6e74 656e 7420 6f66 2073  The content of s
-00000aa0: 7563 6820 6120 636f 6e66 6967 7572 6174  uch a configurat
-00000ab0: 696f 6e0a 636f 756c 6420 6c6f 6f6b 206c  ion.could look l
-00000ac0: 696b 6520 5b74 6869 735d 2868 7474 7073  ike [this](https
-00000ad0: 3a2f 2f67 6974 2e75 667a 2e64 652f 7264  ://git.ufz.de/rd
-00000ae0: 6d2d 736f 6674 7761 7265 2f73 6171 632f  m-software/saqc/
-00000af0: 7261 772f 6465 7665 6c6f 702f 646f 6373  raw/develop/docs
-00000b00: 2f72 6573 6f75 7263 6573 2f64 6174 612f  /resources/data/
-00000b10: 636f 6e66 6967 2e63 7376 293a 0a0a 6060  config.csv):..``
-00000b20: 600a 7661 726e 616d 6520 2020 203b 2074  `.varname    ; t
-00000b30: 6573 740a 232d 2d2d 2d2d 2d2d 2d2d 2d3b  est.#----------;
-00000b40: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000b80: 2d2d 2d2d 2d2d 0a53 4d32 2020 2020 2020  ------.SM2      
-00000b90: 2020 3b20 7368 6966 7428 6672 6571 3d22    ; shift(freq="
-00000ba0: 3135 4d69 6e22 290a 2753 4d28 317c 3229  15Min").'SM(1|2)
-00000bb0: 2b27 203b 2066 6c61 674d 6973 7369 6e67  +' ; flagMissing
-00000bc0: 2829 0a53 4d31 2020 2020 2020 2020 3b20  ().SM1        ; 
-00000bd0: 666c 6167 5261 6e67 6528 6d69 6e3d 3130  flagRange(min=10
-00000be0: 2c20 6d61 783d 3630 290a 534d 3220 2020  , max=60).SM2   
-00000bf0: 2020 2020 203b 2066 6c61 6752 616e 6765       ; flagRange
-00000c00: 286d 696e 3d31 302c 206d 6178 3d34 3029  (min=10, max=40)
-00000c10: 0a53 4d32 2020 2020 2020 2020 3b20 666c  .SM2        ; fl
-00000c20: 6167 4d41 4428 7769 6e64 6f77 3d22 3330  agMAD(window="30
-00000c30: 6422 2c20 7a3d 332e 3529 0a44 756d 6d79  d", z=3.5).Dummy
-00000c40: 2020 2020 2020 3b20 666c 6167 4765 6e65        ; flagGene
-00000c50: 7269 6328 6669 656c 643d 5b22 534d 3122  ric(field=["SM1"
-00000c60: 2c20 2253 4d32 225d 2c20 6675 6e63 3d28  , "SM2"], func=(
-00000c70: 6973 666c 6167 6765 6428 7829 207c 2069  isflagged(x) | i
-00000c80: 7366 6c61 6767 6564 2879 2929 290a 6060  sflagged(y))).``
-00000c90: 600a 0a41 7320 736f 6f6e 2061 7320 7468  `..As soon as th
-00000ca0: 6520 6261 7369 6320 696e 7075 7473 2c20  e basic inputs, 
-00000cb0: 6461 7461 7365 7420 616e 6420 636f 6e66  dataset and conf
-00000cc0: 6967 7572 6174 696f 6e20 6669 6c65 2c20  iguration file, 
-00000cd0: 6172 650a 7072 6570 6172 6564 2c20 7275  are.prepared, ru
-00000ce0: 6e20 6053 6151 4360 3a0a 6060 6073 680a  n `SaQC`:.```sh.
-00000cf0: 7361 7163 205c 0a20 2020 202d 2d63 6f6e  saqc \.    --con
-00000d00: 6669 6720 5041 5448 5f54 4f5f 434f 4e46  fig PATH_TO_CONF
-00000d10: 4947 5552 4154 494f 4e20 5c0a 2020 2020  IGURATION \.    
-00000d20: 2d2d 6461 7461 2050 4154 485f 544f 5f44  --data PATH_TO_D
-00000d30: 4154 4120 5c0a 2020 2020 2d2d 6f75 7466  ATA \.    --outf
-00000d40: 696c 6520 5041 5448 5f54 4f5f 4f55 5450  ile PATH_TO_OUTP
-00000d50: 5554 0a60 6060 0a0a 4120 6675 6c6c 2060  UT.```..A full `
-00000d60: 5361 5143 6020 7275 6e20 6167 6169 6e73  SaQC` run agains
-00000d70: 7420 7072 6f76 6964 6564 2065 7861 6d70  t provided examp
-00000d80: 6c65 2064 6174 6120 6361 6e20 6265 2069  le data can be i
-00000d90: 6e76 6f6b 6564 2077 6974 683a 0a60 6060  nvoked with:.```
-00000da0: 7368 0a73 6171 6320 5c0a 2020 2020 2d2d  sh.saqc \.    --
-00000db0: 636f 6e66 6967 2068 7474 7073 3a2f 2f67  config https://g
-00000dc0: 6974 2e75 667a 2e64 652f 7264 6d2d 736f  it.ufz.de/rdm-so
-00000dd0: 6674 7761 7265 2f73 6171 632f 7261 772f  ftware/saqc/raw/
-00000de0: 6465 7665 6c6f 702f 646f 6373 2f72 6573  develop/docs/res
-00000df0: 6f75 7263 6573 2f64 6174 612f 636f 6e66  ources/data/conf
-00000e00: 6967 2e63 7376 205c 0a20 2020 202d 2d64  ig.csv \.    --d
-00000e10: 6174 6120 6874 7470 733a 2f2f 6769 742e  ata https://git.
-00000e20: 7566 7a2e 6465 2f72 646d 2d73 6f66 7477  ufz.de/rdm-softw
-00000e30: 6172 652f 7361 7163 2f72 6177 2f64 6576  are/saqc/raw/dev
-00000e40: 656c 6f70 2f64 6f63 732f 7265 736f 7572  elop/docs/resour
-00000e50: 6365 732f 6461 7461 2f64 6174 612e 6373  ces/data/data.cs
-00000e60: 7620 5c0a 2020 2020 2d2d 6f75 7466 696c  v \.    --outfil
-00000e70: 6520 7361 7163 5f74 6573 742e 6373 760a  e saqc_test.csv.
-00000e80: 6060 600a 0a23 2323 2053 6151 4320 6173  ```..### SaQC as
-00000e90: 2061 2070 7974 686f 6e20 6d6f 6475 6c65   a python module
-00000ea0: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-00000eb0: 736e 6970 7065 7420 696d 706c 656d 656e  snippet implemen
-00000ec0: 7473 2074 6865 2073 616d 6520 636f 6e66  ts the same conf
-00000ed0: 6967 7572 6174 696f 6e20 6769 7665 6e20  iguration given 
-00000ee0: 6162 6f76 6520 7468 726f 7567 680a 7468  above through.th
-00000ef0: 6520 5079 7468 6f6e 2d41 5049 3a0a 0a60  e Python-API:..`
-00000f00: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00000f10: 7061 6e64 6173 2061 7320 7064 0a66 726f  pandas as pd.fro
-00000f20: 6d20 7361 7163 2069 6d70 6f72 7420 5361  m saqc import Sa
-00000f30: 5143 0a0a 6461 7461 203d 2070 642e 7265  QC..data = pd.re
-00000f40: 6164 5f63 7376 280a 2020 2020 2268 7474  ad_csv(.    "htt
-00000f50: 7073 3a2f 2f67 6974 2e75 667a 2e64 652f  ps://git.ufz.de/
-00000f60: 7264 6d2d 736f 6674 7761 7265 2f73 6171  rdm-software/saq
-00000f70: 632f 7261 772f 6465 7665 6c6f 702f 646f  c/raw/develop/do
-00000f80: 6373 2f72 6573 6f75 7263 6573 2f64 6174  cs/resources/dat
-00000f90: 612f 6461 7461 2e63 7376 222c 0a20 2020  a/data.csv",.   
-00000fa0: 2069 6e64 6578 5f63 6f6c 3d30 2c20 7061   index_col=0, pa
-00000fb0: 7273 655f 6461 7465 733d 5472 7565 2c0a  rse_dates=True,.
-00000fc0: 290a 0a73 6171 6320 3d20 5361 5143 2864  )..saqc = SaQC(d
-00000fd0: 6174 613d 6461 7461 290a 7361 7163 203d  ata=data).saqc =
-00000fe0: 2028 7361 7163 0a20 2020 2020 2020 202e   (saqc.        .
-00000ff0: 7368 6966 7428 2253 4d32 222c 2066 7265  shift("SM2", fre
-00001000: 713d 2231 354d 696e 2229 0a20 2020 2020  q="15Min").     
-00001010: 2020 202e 666c 6167 4d69 7373 696e 6728     .flagMissing(
-00001020: 2253 4d28 317c 3229 2b22 2c20 7265 6765  "SM(1|2)+", rege
-00001030: 783d 5472 7565 290a 2020 2020 2020 2020  x=True).        
-00001040: 2e66 6c61 6752 616e 6765 2822 534d 3122  .flagRange("SM1"
-00001050: 2c20 6d69 6e3d 3130 2c20 6d61 783d 3630  , min=10, max=60
-00001060: 290a 2020 2020 2020 2020 2e66 6c61 6752  ).        .flagR
-00001070: 616e 6765 2822 534d 3222 2c20 6d69 6e3d  ange("SM2", min=
-00001080: 3130 2c20 6d61 783d 3430 290a 2020 2020  10, max=40).    
-00001090: 2020 2020 2e66 6c61 674d 4144 2822 534d      .flagMAD("SM
-000010a0: 3222 2c20 7769 6e64 6f77 3d22 3330 6422  2", window="30d"
-000010b0: 2c20 7a3d 332e 3529 0a20 2020 2020 2020  , z=3.5).       
-000010c0: 202e 666c 6167 4765 6e65 7269 6328 6669   .flagGeneric(fi
-000010d0: 656c 643d 5b22 534d 3122 2c20 2253 4d32  eld=["SM1", "SM2
-000010e0: 225d 2c20 7461 7267 6574 3d22 4475 6d6d  "], target="Dumm
-000010f0: 7922 2c20 6675 6e63 3d6c 616d 6264 6120  y", func=lambda 
-00001100: 782c 2079 3a20 2869 7366 6c61 6767 6564  x, y: (isflagged
-00001110: 2878 2920 7c20 6973 666c 6167 6765 6428  (x) | isflagged(
-00001120: 7929 2929 290a 6060 600a 0a41 206d 6f72  y)))).```..A mor
-00001130: 6520 6465 7461 696c 6564 2064 6573 6372  e detailed descr
-00001140: 6970 7469 6f6e 206f 6620 7468 6520 5079  iption of the Py
-00001150: 7468 6f6e 2041 5049 2069 7320 6176 6169  thon API is avai
-00001160: 6c61 626c 6520 696e 2074 6865 200a 5b72  lable in the .[r
-00001170: 6573 7065 6374 6976 6520 7365 6374 696f  espective sectio
-00001180: 6e5d 2868 7474 7073 3a2f 2f72 646d 2d73  n](https://rdm-s
-00001190: 6f66 7477 6172 652e 7061 6765 732e 7566  oftware.pages.uf
-000011a0: 7a2e 6465 2f73 6171 632f 6765 7474 696e  z.de/saqc/gettin
-000011b0: 6773 7461 7274 6564 2f54 7574 6f72 6961  gstarted/Tutoria
-000011c0: 6c41 5049 2e68 746d 6c29 0a6f 6620 7468  lAPI.html).of th
-000011d0: 6520 646f 6375 6d65 6e74 6174 696f 6e2e  e documentation.
-000011e0: 0a0a 2323 2043 6861 6e67 656c 6f67 0a41  ..## Changelog.A
-000011f0: 6c6c 206e 6f74 6162 6c65 2063 6861 6e67  ll notable chang
-00001200: 6573 2074 6f20 7468 6973 2070 726f 6a65  es to this proje
-00001210: 6374 2077 696c 6c20 6265 2064 6f63 756d  ct will be docum
-00001220: 656e 7465 6420 696e 205b 4348 414e 4745  ented in [CHANGE
-00001230: 4c4f 472e 6d64 5d28 4348 414e 4745 4c4f  LOG.md](CHANGELO
-00001240: 472e 6d64 292e 0a0a 2323 2047 6574 2069  G.md)...## Get i
-00001250: 6e76 6f6c 7665 640a 0a23 2323 2043 6f6e  nvolved..### Con
-00001260: 7472 6962 7574 696e 670a 596f 7520 666f  tributing.You fo
-00001270: 756e 6420 6120 6275 6720 6f72 2079 6f75  und a bug or you
-00001280: 2077 616e 7420 746f 2073 7567 6765 7374   want to suggest
-00001290: 2073 6f6d 6520 636f 6f6c 2066 6561 7475   some cool featu
-000012a0: 7265 733f 2050 6c65 6173 6520 7265 6665  res? Please refe
-000012b0: 7220 746f 206f 7572 205b 636f 6e74 7269  r to our [contri
-000012c0: 6275 7469 6e67 2067 7569 6465 6c69 6e65  buting guideline
-000012d0: 735d 2843 4f4e 5452 4942 5554 494e 472e  s](CONTRIBUTING.
-000012e0: 6d64 2920 746f 2073 6565 2068 6f77 2079  md) to see how y
-000012f0: 6f75 2063 616e 2063 6f6e 7472 6962 7574  ou can contribut
-00001300: 6520 746f 2053 6151 432e 0a0a 2323 2320  e to SaQC...### 
-00001310: 5573 6572 2073 7570 706f 7274 0a49 6620  User support.If 
-00001320: 796f 7520 6e65 6564 2068 656c 7020 6f72  you need help or
-00001330: 2068 6176 6520 6120 7175 6573 7469 6f6e   have a question
-00001340: 2c20 796f 7520 6361 6e20 7573 6520 7468  , you can use th
-00001350: 6520 5361 5143 2075 7365 7220 7375 7070  e SaQC user supp
-00001360: 6f72 7420 6d61 696c 696e 6720 6c69 7374  ort mailing list
-00001370: 3a20 5b73 6171 632d 7375 7070 6f72 7440  : [saqc-support@
-00001380: 7566 7a2e 6465 5d28 6d61 696c 746f 3a73  ufz.de](mailto:s
-00001390: 6171 632d 7375 7070 6f72 7440 7566 7a2e  aqc-support@ufz.
-000013a0: 6465 290a 0a23 2320 436f 7079 7269 6768  de)..## Copyrigh
-000013b0: 7420 616e 6420 4c69 6365 6e73 650a 436f  t and License.Co
-000013c0: 7079 7269 6768 7428 6329 2032 3032 312c  pyright(c) 2021,
-000013d0: 205b 4865 6c6d 686f 6c74 7a2d 5a65 6e74   [Helmholtz-Zent
-000013e0: 7275 6d20 66c3 bc72 2055 6d77 656c 7466  rum f..r Umweltf
-000013f0: 6f72 7363 6875 6e67 2047 6d62 4820 2d2d  orschung GmbH --
-00001400: 2055 465a 5d28 6874 7470 733a 2f2f 7777   UFZ](https://ww
-00001410: 772e 7566 7a2e 6465 292e 2041 6c6c 2072  w.ufz.de). All r
-00001420: 6967 6874 7320 7265 7365 7276 6564 2e0a  ights reserved..
-00001430: 0a2d 2044 6f63 756d 656e 7461 7469 6f6e  .- Documentation
-00001440: 3a20 5b43 7265 6174 6976 6520 436f 6d6d  : [Creative Comm
-00001450: 6f6e 7320 4174 7472 6962 7574 696f 6e20  ons Attribution 
-00001460: 342e 3020 496e 7465 726e 6174 696f 6e61  4.0 Internationa
-00001470: 6c5d 2868 7474 7073 3a2f 2f63 7265 6174  l](https://creat
-00001480: 6976 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c  ivecommons.org/l
-00001490: 6963 656e 7365 732f 6279 2f34 2e30 2f29  icenses/by/4.0/)
-000014a0: 203c 6120 7265 6c3d 226c 6963 656e 7365   <a rel="license
-000014b0: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-000014c0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-000014d0: 7267 2f6c 6963 656e 7365 732f 6279 2f34  rg/licenses/by/4
-000014e0: 2e30 2f22 3e3c 696d 6720 616c 743d 2243  .0/"><img alt="C
-000014f0: 7265 6174 6976 6520 436f 6d6d 6f6e 7320  reative Commons 
-00001500: 4c69 6365 6e73 6522 2073 7479 6c65 3d22  License" style="
-00001510: 626f 7264 6572 2d77 6964 7468 3a30 2220  border-width:0" 
-00001520: 7372 633d 2268 7474 7073 3a2f 2f69 2e63  src="https://i.c
-00001530: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-00001540: 7267 2f6c 2f62 792f 342e 302f 3830 7831  rg/l/by/4.0/80x1
-00001550: 352e 706e 6722 202f 3e3c 2f61 3e0a 2d20  5.png" /></a>.- 
-00001560: 536f 7572 6365 2063 6f64 653a 205b 474e  Source code: [GN
-00001570: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-00001580: 204c 6963 656e 7365 2033 5d28 6874 7470   License 3](http
-00001590: 733a 2f2f 7777 772e 676e 752e 6f72 672f  s://www.gnu.org/
-000015a0: 6c69 6365 6e73 6573 2f67 706c 2d33 2e30  licenses/gpl-3.0
-000015b0: 2e68 746d 6c29 0a0a 466f 7220 6675 6c6c  .html)..For full
-000015c0: 2064 6574 6169 6c73 2c20 7365 6520 5b4c   details, see [L
-000015d0: 4943 454e 5345 5d28 4c49 4345 4e53 452e  ICENSE](LICENSE.
-000015e0: 6d64 292e 0a0a 2323 2041 636b 6e6f 776c  md)...## Acknowl
-000015f0: 6564 6765 6d65 6e74 730a 2e2e 2e0a 0a23  edgements......#
-00001600: 2320 5075 626c 6963 6174 696f 6e73 0a63  # Publications.c
-00001610: 6f6d 696e 6720 736f 6f6e 2e2e 2e0a 0a23  oming soon.....#
-00001620: 2320 486f 7720 746f 2063 6974 6520 5361  # How to cite Sa
-00001630: 5143 0a49 6620 5361 5143 2069 7320 6164  QC.If SaQC is ad
-00001640: 7661 6e63 696e 6720 796f 7572 2072 6573  vancing your res
-00001650: 6561 7263 682c 2070 6c65 6173 6520 6369  earch, please ci
-00001660: 7465 2061 733a 0a0a 3e20 5363 68c3 a466  te as:..> Sch..f
-00001670: 6572 2c20 4461 7669 643b 2050 616c 6d2c  er, David; Palm,
-00001680: 2042 6572 743b 204c c3bc 6e65 6e73 6368   Bert; L..nensch
-00001690: 6c6f c39f 2c20 5065 7465 722e 2028 3230  lo.., Peter. (20
-000016a0: 3231 292e 2053 7973 7465 6d20 666f 7220  21). System for 
-000016b0: 6175 746f 6d61 7465 6420 5175 616c 6974  automated Qualit
-000016c0: 7920 436f 6e74 726f 6c20 2d20 5361 5143  y Control - SaQC
-000016d0: 2e20 5a65 6e6f 646f 2e20 6874 7470 733a  . Zenodo. https:
-000016e0: 2f2f 646f 692e 6f72 672f 3130 2e35 3238  //doi.org/10.528
-000016f0: 312f 7a65 6e6f 646f 2e35 3838 3835 3437  1/zenodo.5888547
-00001700: 0a                                       .
+00000020: 0a56 6572 7369 6f6e 3a20 322e 342e 300a  .Version: 2.4.0.
+00000030: 5375 6d6d 6172 793a 2041 2074 696d 6573  Summary: A times
+00000040: 6572 6965 7320 6461 7461 2071 7561 6c69  eries data quali
+00000050: 7479 2063 6f6e 7472 6f6c 2061 6e64 2070  ty control and p
+00000060: 726f 6365 7373 696e 6720 746f 6f6c 2f66  rocessing tool/f
+00000070: 7261 6d65 776f 726b 0a48 6f6d 652d 7061  ramework.Home-pa
+00000080: 6765 3a20 6874 7470 733a 2f2f 6769 742e  ge: https://git.
+00000090: 7566 7a2e 6465 2f72 646d 2d73 6f66 7477  ufz.de/rdm-softw
+000000a0: 6172 652f 7361 7163 0a41 7574 686f 723a  are/saqc.Author:
+000000b0: 2042 6572 7420 5061 6c6d 2c20 4461 7669   Bert Palm, Davi
+000000c0: 6420 5363 6861 6566 6572 2c20 466c 6f72  d Schaefer, Flor
+000000d0: 6961 6e20 4772 616e 7365 652c 2050 6574  ian Gransee, Pet
+000000e0: 6572 204c 7565 6e65 6e73 6368 6c6f 7373  er Luenenschloss
+000000f0: 0a41 7574 686f 722d 656d 6169 6c3a 2064  .Author-email: d
+00000100: 6176 6964 2e73 6368 6165 6665 7240 7566  avid.schaefer@uf
+00000110: 7a2e 6465 0a52 6571 7569 7265 732d 5079  z.de.Requires-Py
+00000120: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
+00000130: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000140: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000150: 6f77 6e0a 4c69 6365 6e73 652d 4669 6c65  own.License-File
+00000160: 3a20 4c49 4345 4e53 452e 6d64 0a4c 6963  : LICENSE.md.Lic
+00000170: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000180: 5345 532f 4750 4c2d 332e 302d 6f72 2d6c  SES/GPL-3.0-or-l
+00000190: 6174 6572 2e74 7874 0a0a 3c21 2d2d 0a53  ater.txt..<!--.S
+000001a0: 5044 582d 4669 6c65 436f 7079 7269 6768  PDX-FileCopyrigh
+000001b0: 7454 6578 743a 2032 3032 3120 4865 6c6d  tText: 2021 Helm
+000001c0: 686f 6c74 7a2d 5a65 6e74 7275 6d20 66c3  holtz-Zentrum f.
+000001d0: bc72 2055 6d77 656c 7466 6f72 7363 6875  .r Umweltforschu
+000001e0: 6e67 2047 6d62 4820 2d20 5546 5a0a 0a53  ng GmbH - UFZ..S
+000001f0: 5044 582d 4c69 6365 6e73 652d 4964 656e  PDX-License-Iden
+00000200: 7469 6669 6572 3a20 4750 4c2d 332e 302d  tifier: GPL-3.0-
+00000210: 6f72 2d6c 6174 6572 0a2d 2d3e 0a0a 3c62  or-later.-->..<b
+00000220: 723e 0a3c 6469 7620 616c 6967 6e3d 2263  r>.<div align="c
+00000230: 656e 7465 7222 3e0a 2020 3c69 6d67 2073  enter">.  <img s
+00000240: 7263 3d22 6874 7470 733a 2f2f 6769 742e  rc="https://git.
+00000250: 7566 7a2e 6465 2f72 646d 2d73 6f66 7477  ufz.de/rdm-softw
+00000260: 6172 652f 7361 7163 2f72 6177 2f64 6576  are/saqc/raw/dev
+00000270: 656c 6f70 2f64 6f63 732f 7265 736f 7572  elop/docs/resour
+00000280: 6365 732f 696d 6167 6573 2f72 6570 7265  ces/images/repre
+00000290: 7365 6e74 6174 6976 652f 5361 5143 4c6f  sentative/SaQCLo
+000002a0: 676f 2e70 6e67 2220 7769 6474 683d 2233  go.png" width="3
+000002b0: 3030 223e 0a3c 2f64 6976 3e0a 0a2d 2d2d  00">.</div>..---
+000002c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a5b  --------------.[
+000002d0: 215b 5072 6f6a 6563 7420 5374 6174 7573  ![Project Status
+000002e0: 3a20 4163 7469 7665 20e2 8093 2054 6865  : Active ... The
+000002f0: 2070 726f 6a65 6374 2068 6173 2072 6561   project has rea
+00000300: 6368 6564 2061 2073 7461 626c 652c 2075  ched a stable, u
+00000310: 7361 626c 6520 7374 6174 6520 616e 6420  sable state and 
+00000320: 6973 2062 6569 6e67 2061 6374 6976 656c  is being activel
+00000330: 7920 6465 7665 6c6f 7065 642e 5d28 6874  y developed.](ht
+00000340: 7470 733a 2f2f 7777 772e 7265 706f 7374  tps://www.repost
+00000350: 6174 7573 2e6f 7267 2f62 6164 6765 732f  atus.org/badges/
+00000360: 6c61 7465 7374 2f61 6374 6976 652e 7376  latest/active.sv
+00000370: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
+00000380: 7265 706f 7374 6174 7573 2e6f 7267 2f23  repostatus.org/#
+00000390: 6163 7469 7665 290a 0a23 2020 5361 5143  active)..#  SaQC
+000003a0: 3a20 5379 7374 656d 2066 6f72 2061 7574  : System for aut
+000003b0: 6f6d 6174 6564 2051 7561 6c69 7479 2043  omated Quality C
+000003c0: 6f6e 7472 6f6c 0a0a 416e 6f6d 616c 6965  ontrol..Anomalie
+000003d0: 7320 616e 6420 6572 726f 7273 2061 7265  s and errors are
+000003e0: 2074 6865 2072 756c 6520 6e6f 7420 7468   the rule not th
+000003f0: 6520 6578 6365 7074 696f 6e20 7768 656e  e exception when
+00000400: 2077 6f72 6b69 6e67 2077 6974 6820 0a74   working with .t
+00000410: 696d 6520 7365 7269 6573 2064 6174 612e  ime series data.
+00000420: 2054 6869 7320 6973 2065 7370 6563 6961   This is especia
+00000430: 6c6c 7920 7472 7565 2c20 6966 2073 7563  lly true, if suc
+00000440: 6820 6461 7461 206f 7269 6769 6e61 7465  h data originate
+00000450: 730a 6672 6f6d 2069 6e2d 7369 7475 206d  s.from in-situ m
+00000460: 6561 7375 7265 6d65 6e74 7320 6f66 2065  easurements of e
+00000470: 6e76 6972 6f6e 6d65 6e74 616c 2070 726f  nvironmental pro
+00000480: 7065 7274 6965 732e 200a 416c 6d6f 7374  perties. .Almost
+00000490: 2061 6c6c 2061 7070 6c69 6361 7469 6f6e   all application
+000004a0: 732c 2068 6f77 6576 6572 2c20 696d 706c  s, however, impl
+000004b0: 6963 696c 7920 7265 6c79 206f 6e20 6461  icily rely on da
+000004c0: 7461 2c20 7468 6174 2063 6f6d 706c 6965  ta, that complie
+000004d0: 730a 7769 7468 2073 6f6d 6520 6465 6669  s.with some defi
+000004e0: 6e69 7469 6f6e 206f 6620 2763 6f72 7265  nition of 'corre
+000004f0: 6374 272e 200a 496e 206f 7264 6572 2074  ct'. .In order t
+00000500: 6f20 696e 6665 7220 7265 6c69 6162 6c65  o infer reliable
+00000510: 2064 6174 6120 7072 6f64 7563 7473 2061   data products a
+00000520: 6e64 2074 6f6f 6c73 2c20 7468 6572 6520  nd tools, there 
+00000530: 6973 206e 6f20 616c 7465 726e 6174 6976  is no alternativ
+00000540: 650a 746f 2071 7561 6c69 7479 2063 6f6e  e.to quality con
+00000550: 7472 6f6c 2e20 5361 5143 2070 726f 7669  trol. SaQC provi
+00000560: 6465 7320 616c 6c20 7468 6520 6275 696c  des all the buil
+00000570: 6469 6e67 2062 6c6f 636b 7320 746f 2063  ding blocks to c
+00000580: 6f6d 666f 7274 6162 6c79 0a62 7269 6467  omfortably.bridg
+00000590: 6520 7468 6520 6761 7020 6265 7477 6565  e the gap betwee
+000005a0: 6e20 2775 7375 616c 6c79 2066 6175 6c74  n 'usually fault
+000005b0: 7927 2061 6e64 2027 6578 7065 6374 6564  y' and 'expected
+000005c0: 2074 6f20 6265 2063 6f72 7265 6374 6564   to be corrected
+000005d0: 2720 696e 200a 6120 6163 6365 7373 6962  ' in .a accessib
+000005e0: 6c65 2c20 636f 6e73 6973 7465 6e74 2c20  le, consistent, 
+000005f0: 6f62 6a65 6374 6976 6520 616e 6420 7265  objective and re
+00000600: 7072 6f64 7563 6962 6c65 2077 6179 2e0a  producible way..
+00000610: 0a46 6f72 2061 2028 636f 6e74 696e 6f75  .For a (continou
+00000620: 736c 7920 696d 7072 6f76 696e 6729 206f  sly improving) o
+00000630: 7665 7276 6965 7720 6f66 2066 6561 7475  verview of featu
+00000640: 7265 732c 2074 7970 6963 616c 2075 7361  res, typical usa
+00000650: 6765 2070 6174 7465 726e 732c 0a74 6865  ge patterns,.the
+00000660: 2073 7065 6369 6669 6320 7379 7374 656d   specific system
+00000670: 2063 6f6d 706f 6e65 6e74 7320 616e 6420   components and 
+00000680: 686f 7720 746f 2063 7573 746f 6d69 7a65  how to customize
+00000690: 2060 5361 5143 6020 746f 2079 6f75 7220   `SaQC` to your 
+000006a0: 7370 6563 6966 6963 0a6e 6565 6473 2c20  specific.needs, 
+000006b0: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
+000006c0: 6f75 720a 5b6f 6e6c 696e 6520 646f 6375  our.[online docu
+000006d0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+000006e0: 3a2f 2f72 646d 2d73 6f66 7477 6172 652e  ://rdm-software.
+000006f0: 7061 6765 732e 7566 7a2e 6465 2f73 6171  pages.ufz.de/saq
+00000700: 632f 696e 6465 782e 6874 6d6c 292e 0a0a  c/index.html)...
+00000710: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000720: 0a0a 5361 5143 2069 7320 6176 6169 6c61  ..SaQC is availa
+00000730: 626c 6520 6f6e 2074 6865 2050 7974 686f  ble on the Pytho
+00000740: 6e20 5061 636b 6167 6520 496e 6465 7820  n Package Index 
+00000750: 285b 5079 5049 5d28 6874 7470 733a 2f2f  ([PyPI](https://
+00000760: 7079 7069 2e6f 7267 2f29 2920 616e 640a  pypi.org/)) and.
+00000770: 6361 6e20 6265 2069 6e73 7461 6c6c 6564  can be installed
+00000780: 2075 7369 6e67 205b 7069 705d 2868 7474   using [pip](htt
+00000790: 7073 3a2f 2f70 6970 2e70 7970 612e 696f  ps://pip.pypa.io
+000007a0: 2f65 6e2f 7374 6162 6c65 2f29 3a0a 6060  /en/stable/):.``
+000007b0: 6073 680a 7079 7468 6f6e 202d 6d20 7069  `sh.python -m pi
+000007c0: 7020 696e 7374 616c 6c20 7361 7163 0a60  p install saqc.`
+000007d0: 6060 0a46 6f72 2061 206d 6f72 6520 6465  ``.For a more de
+000007e0: 7461 696c 6564 2069 6e73 7461 6c6c 696f  tailed installio
+000007f0: 6e20 6775 6964 652c 2073 6565 2074 6865  n guide, see the
+00000800: 205b 696e 7374 616c 6c61 7469 6f6e 2067   [installation g
+00000810: 7569 6465 5d28 6874 7470 733a 2f2f 7264  uide](https://rd
+00000820: 6d2d 736f 6674 7761 7265 2e70 6167 6573  m-software.pages
+00000830: 2e75 667a 2e64 652f 7361 7163 2f67 6574  .ufz.de/saqc/get
+00000840: 7469 6e67 7374 6172 7465 642f 496e 7374  tingstarted/Inst
+00000850: 616c 6c61 7469 6f6e 4775 6964 652e 6874  allationGuide.ht
+00000860: 6d6c 292e 0a0a 2323 2055 7361 6765 0a0a  ml)...## Usage..
+00000870: 6053 6151 4360 2069 7320 626f 7468 2c20  `SaQC` is both, 
+00000880: 6120 636f 6d6d 616e 6420 6c69 6e65 2061  a command line a
+00000890: 7070 6c69 6361 7469 6f6e 2063 6f6e 7472  pplication contr
+000008a0: 6f6c 6c65 6420 6279 2061 2074 6578 7420  olled by a text 
+000008b0: 6261 7365 6420 636f 6e66 6967 7572 6174  based configurat
+000008c0: 696f 6e0a 616e 6420 6120 7079 7468 6f6e  ion.and a python
+000008d0: 206d 6f64 756c 6520 7769 7468 2061 2073   module with a s
+000008e0: 696d 706c 6520 4150 492e 0a0a 2323 2320  imple API...### 
+000008f0: 5361 5143 2061 7320 6120 636f 6d6d 616e  SaQC as a comman
+00000900: 6420 6c69 6e65 2061 7070 6c69 6361 7469  d line applicati
+00000910: 6f6e 0a54 6865 2063 6f6d 6d61 6e64 206c  on.The command l
+00000920: 696e 6520 6170 706c 6963 6174 696f 6e20  ine application 
+00000930: 6973 2063 6f6e 7472 6f6c 6c65 6420 6279  is controlled by
+00000940: 2061 2073 656d 6963 6f6c 6f6e 2d73 6570   a semicolon-sep
+00000950: 6172 6174 6564 2074 6578 740a 6669 6c65  arated text.file
+00000960: 206c 6973 7469 6e67 2074 6865 2076 6172   listing the var
+00000970: 6961 626c 6573 2069 6e20 7468 6520 6461  iables in the da
+00000980: 7461 7365 7420 616e 6420 7468 6520 726f  taset and the ro
+00000990: 7574 696e 6573 2074 6f20 696e 7370 6563  utines to inspec
+000009a0: 742c 0a71 7561 6c69 7479 2063 6f6e 7472  t,.quality contr
+000009b0: 6f6c 2061 6e64 2f6f 7220 7072 6f63 6573  ol and/or proces
+000009c0: 7320 7468 656d 2e20 5468 6520 636f 6e74  s them. The cont
+000009d0: 656e 7420 6f66 2073 7563 6820 6120 636f  ent of such a co
+000009e0: 6e66 6967 7572 6174 696f 6e0a 636f 756c  nfiguration.coul
+000009f0: 6420 6c6f 6f6b 206c 696b 6520 5b74 6869  d look like [thi
+00000a00: 735d 2868 7474 7073 3a2f 2f67 6974 2e75  s](https://git.u
+00000a10: 667a 2e64 652f 7264 6d2d 736f 6674 7761  fz.de/rdm-softwa
+00000a20: 7265 2f73 6171 632f 7261 772f 6465 7665  re/saqc/raw/deve
+00000a30: 6c6f 702f 646f 6373 2f72 6573 6f75 7263  lop/docs/resourc
+00000a40: 6573 2f64 6174 612f 636f 6e66 6967 2e63  es/data/config.c
+00000a50: 7376 293a 0a0a 6060 600a 7661 726e 616d  sv):..```.varnam
+00000a60: 6520 2020 203b 2074 6573 740a 232d 2d2d  e    ; test.#---
+00000a70: 2d2d 2d2d 2d2d 2d3b 202d 2d2d 2d2d 2d2d  -------; -------
+00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a53  --------------.S
+00000ac0: 4d32 2020 2020 2020 2020 3b20 7368 6966  M2        ; shif
+00000ad0: 7428 6672 6571 3d22 3135 4d69 6e22 290a  t(freq="15Min").
+00000ae0: 2753 4d28 317c 3229 2b27 203b 2066 6c61  'SM(1|2)+' ; fla
+00000af0: 674d 6973 7369 6e67 2829 0a53 4d31 2020  gMissing().SM1  
+00000b00: 2020 2020 2020 3b20 666c 6167 5261 6e67        ; flagRang
+00000b10: 6528 6d69 6e3d 3130 2c20 6d61 783d 3630  e(min=10, max=60
+00000b20: 290a 534d 3220 2020 2020 2020 203b 2066  ).SM2        ; f
+00000b30: 6c61 6752 616e 6765 286d 696e 3d31 302c  lagRange(min=10,
+00000b40: 206d 6178 3d34 3029 0a53 4d32 2020 2020   max=40).SM2    
+00000b50: 2020 2020 3b20 666c 6167 4d41 4428 7769      ; flagMAD(wi
+00000b60: 6e64 6f77 3d22 3330 6422 2c20 7a3d 332e  ndow="30d", z=3.
+00000b70: 3529 0a44 756d 6d79 2020 2020 2020 3b20  5).Dummy      ; 
+00000b80: 666c 6167 4765 6e65 7269 6328 6669 656c  flagGeneric(fiel
+00000b90: 643d 5b22 534d 3122 2c20 2253 4d32 225d  d=["SM1", "SM2"]
+00000ba0: 2c20 6675 6e63 3d28 6973 666c 6167 6765  , func=(isflagge
+00000bb0: 6428 7829 207c 2069 7366 6c61 6767 6564  d(x) | isflagged
+00000bc0: 2879 2929 290a 6060 600a 0a41 7320 736f  (y))).```..As so
+00000bd0: 6f6e 2061 7320 7468 6520 6261 7369 6320  on as the basic 
+00000be0: 696e 7075 7473 2c20 6461 7461 7365 7420  inputs, dataset 
+00000bf0: 616e 6420 636f 6e66 6967 7572 6174 696f  and configuratio
+00000c00: 6e20 6669 6c65 2c20 6172 650a 7072 6570  n file, are.prep
+00000c10: 6172 6564 2c20 7275 6e20 6053 6151 4360  ared, run `SaQC`
+00000c20: 3a0a 6060 6073 680a 7361 7163 205c 0a20  :.```sh.saqc \. 
+00000c30: 2020 202d 2d63 6f6e 6669 6720 5041 5448     --config PATH
+00000c40: 5f54 4f5f 434f 4e46 4947 5552 4154 494f  _TO_CONFIGURATIO
+00000c50: 4e20 5c0a 2020 2020 2d2d 6461 7461 2050  N \.    --data P
+00000c60: 4154 485f 544f 5f44 4154 4120 5c0a 2020  ATH_TO_DATA \.  
+00000c70: 2020 2d2d 6f75 7466 696c 6520 5041 5448    --outfile PATH
+00000c80: 5f54 4f5f 4f55 5450 5554 0a60 6060 0a0a  _TO_OUTPUT.```..
+00000c90: 4120 6675 6c6c 2060 5361 5143 6020 7275  A full `SaQC` ru
+00000ca0: 6e20 6167 6169 6e73 7420 7072 6f76 6964  n against provid
+00000cb0: 6564 2065 7861 6d70 6c65 2064 6174 6120  ed example data 
+00000cc0: 6361 6e20 6265 2069 6e76 6f6b 6564 2077  can be invoked w
+00000cd0: 6974 683a 0a60 6060 7368 0a73 6171 6320  ith:.```sh.saqc 
+00000ce0: 5c0a 2020 2020 2d2d 636f 6e66 6967 2068  \.    --config h
+00000cf0: 7474 7073 3a2f 2f67 6974 2e75 667a 2e64  ttps://git.ufz.d
+00000d00: 652f 7264 6d2d 736f 6674 7761 7265 2f73  e/rdm-software/s
+00000d10: 6171 632f 7261 772f 6465 7665 6c6f 702f  aqc/raw/develop/
+00000d20: 646f 6373 2f72 6573 6f75 7263 6573 2f64  docs/resources/d
+00000d30: 6174 612f 636f 6e66 6967 2e63 7376 205c  ata/config.csv \
+00000d40: 0a20 2020 202d 2d64 6174 6120 6874 7470  .    --data http
+00000d50: 733a 2f2f 6769 742e 7566 7a2e 6465 2f72  s://git.ufz.de/r
+00000d60: 646d 2d73 6f66 7477 6172 652f 7361 7163  dm-software/saqc
+00000d70: 2f72 6177 2f64 6576 656c 6f70 2f64 6f63  /raw/develop/doc
+00000d80: 732f 7265 736f 7572 6365 732f 6461 7461  s/resources/data
+00000d90: 2f64 6174 612e 6373 7620 5c0a 2020 2020  /data.csv \.    
+00000da0: 2d2d 6f75 7466 696c 6520 7361 7163 5f74  --outfile saqc_t
+00000db0: 6573 742e 6373 760a 6060 600a 0a23 2323  est.csv.```..###
+00000dc0: 2053 6151 4320 6173 2061 2070 7974 686f   SaQC as a pytho
+00000dd0: 6e20 6d6f 6475 6c65 0a0a 5468 6520 666f  n module..The fo
+00000de0: 6c6c 6f77 696e 6720 736e 6970 7065 7420  llowing snippet 
+00000df0: 696d 706c 656d 656e 7473 2074 6865 2073  implements the s
+00000e00: 616d 6520 636f 6e66 6967 7572 6174 696f  ame configuratio
+00000e10: 6e20 6769 7665 6e20 6162 6f76 6520 7468  n given above th
+00000e20: 726f 7567 680a 7468 6520 5079 7468 6f6e  rough.the Python
+00000e30: 2d41 5049 3a0a 0a60 6060 7079 7468 6f6e  -API:..```python
+00000e40: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
+00000e50: 7320 7064 0a66 726f 6d20 7361 7163 2069  s pd.from saqc i
+00000e60: 6d70 6f72 7420 5361 5143 0a0a 6461 7461  mport SaQC..data
+00000e70: 203d 2070 642e 7265 6164 5f63 7376 280a   = pd.read_csv(.
+00000e80: 2020 2020 2268 7474 7073 3a2f 2f67 6974      "https://git
+00000e90: 2e75 667a 2e64 652f 7264 6d2d 736f 6674  .ufz.de/rdm-soft
+00000ea0: 7761 7265 2f73 6171 632f 7261 772f 6465  ware/saqc/raw/de
+00000eb0: 7665 6c6f 702f 646f 6373 2f72 6573 6f75  velop/docs/resou
+00000ec0: 7263 6573 2f64 6174 612f 6461 7461 2e63  rces/data/data.c
+00000ed0: 7376 222c 0a20 2020 2069 6e64 6578 5f63  sv",.    index_c
+00000ee0: 6f6c 3d30 2c20 7061 7273 655f 6461 7465  ol=0, parse_date
+00000ef0: 733d 5472 7565 2c0a 290a 0a73 6171 6320  s=True,.)..saqc 
+00000f00: 3d20 5361 5143 2864 6174 613d 6461 7461  = SaQC(data=data
+00000f10: 290a 7361 7163 203d 2028 7361 7163 0a20  ).saqc = (saqc. 
+00000f20: 2020 2020 2020 202e 7368 6966 7428 2253         .shift("S
+00000f30: 4d32 222c 2066 7265 713d 2231 354d 696e  M2", freq="15Min
+00000f40: 2229 0a20 2020 2020 2020 202e 666c 6167  ").        .flag
+00000f50: 4d69 7373 696e 6728 2253 4d28 317c 3229  Missing("SM(1|2)
+00000f60: 2b22 2c20 7265 6765 783d 5472 7565 290a  +", regex=True).
+00000f70: 2020 2020 2020 2020 2e66 6c61 6752 616e          .flagRan
+00000f80: 6765 2822 534d 3122 2c20 6d69 6e3d 3130  ge("SM1", min=10
+00000f90: 2c20 6d61 783d 3630 290a 2020 2020 2020  , max=60).      
+00000fa0: 2020 2e66 6c61 6752 616e 6765 2822 534d    .flagRange("SM
+00000fb0: 3222 2c20 6d69 6e3d 3130 2c20 6d61 783d  2", min=10, max=
+00000fc0: 3430 290a 2020 2020 2020 2020 2e66 6c61  40).        .fla
+00000fd0: 674d 4144 2822 534d 3222 2c20 7769 6e64  gMAD("SM2", wind
+00000fe0: 6f77 3d22 3330 6422 2c20 7a3d 332e 3529  ow="30d", z=3.5)
+00000ff0: 0a20 2020 2020 2020 202e 666c 6167 4765  .        .flagGe
+00001000: 6e65 7269 6328 6669 656c 643d 5b22 534d  neric(field=["SM
+00001010: 3122 2c20 2253 4d32 225d 2c20 7461 7267  1", "SM2"], targ
+00001020: 6574 3d22 4475 6d6d 7922 2c20 6675 6e63  et="Dummy", func
+00001030: 3d6c 616d 6264 6120 782c 2079 3a20 2869  =lambda x, y: (i
+00001040: 7366 6c61 6767 6564 2878 2920 7c20 6973  sflagged(x) | is
+00001050: 666c 6167 6765 6428 7929 2929 290a 6060  flagged(y)))).``
+00001060: 600a 0a41 206d 6f72 6520 6465 7461 696c  `..A more detail
+00001070: 6564 2064 6573 6372 6970 7469 6f6e 206f  ed description o
+00001080: 6620 7468 6520 5079 7468 6f6e 2041 5049  f the Python API
+00001090: 2069 7320 6176 6169 6c61 626c 6520 696e   is available in
+000010a0: 2074 6865 200a 5b72 6573 7065 6374 6976   the .[respectiv
+000010b0: 6520 7365 6374 696f 6e5d 2868 7474 7073  e section](https
+000010c0: 3a2f 2f72 646d 2d73 6f66 7477 6172 652e  ://rdm-software.
+000010d0: 7061 6765 732e 7566 7a2e 6465 2f73 6171  pages.ufz.de/saq
+000010e0: 632f 6765 7474 696e 6773 7461 7274 6564  c/gettingstarted
+000010f0: 2f54 7574 6f72 6961 6c41 5049 2e68 746d  /TutorialAPI.htm
+00001100: 6c29 0a6f 6620 7468 6520 646f 6375 6d65  l).of the docume
+00001110: 6e74 6174 696f 6e2e 0a0a 2323 2043 6861  ntation...## Cha
+00001120: 6e67 656c 6f67 0a41 6c6c 206e 6f74 6162  ngelog.All notab
+00001130: 6c65 2063 6861 6e67 6573 2074 6f20 7468  le changes to th
+00001140: 6973 2070 726f 6a65 6374 2077 696c 6c20  is project will 
+00001150: 6265 2064 6f63 756d 656e 7465 6420 696e  be documented in
+00001160: 205b 4348 414e 4745 4c4f 472e 6d64 5d28   [CHANGELOG.md](
+00001170: 4348 414e 4745 4c4f 472e 6d64 292e 0a0a  CHANGELOG.md)...
+00001180: 2323 2047 6574 2069 6e76 6f6c 7665 640a  ## Get involved.
+00001190: 0a23 2323 2043 6f6e 7472 6962 7574 696e  .### Contributin
+000011a0: 670a 596f 7520 666f 756e 6420 6120 6275  g.You found a bu
+000011b0: 6720 6f72 2079 6f75 2077 616e 7420 746f  g or you want to
+000011c0: 2073 7567 6765 7374 2073 6f6d 6520 636f   suggest some co
+000011d0: 6f6c 2066 6561 7475 7265 733f 2050 6c65  ol features? Ple
+000011e0: 6173 6520 7265 6665 7220 746f 206f 7572  ase refer to our
+000011f0: 205b 636f 6e74 7269 6275 7469 6e67 2067   [contributing g
+00001200: 7569 6465 6c69 6e65 735d 2843 4f4e 5452  uidelines](CONTR
+00001210: 4942 5554 494e 472e 6d64 2920 746f 2073  IBUTING.md) to s
+00001220: 6565 2068 6f77 2079 6f75 2063 616e 2063  ee how you can c
+00001230: 6f6e 7472 6962 7574 6520 746f 2053 6151  ontribute to SaQ
+00001240: 432e 0a0a 2323 2320 5573 6572 2073 7570  C...### User sup
+00001250: 706f 7274 0a49 6620 796f 7520 6e65 6564  port.If you need
+00001260: 2068 656c 7020 6f72 2068 6176 6520 6120   help or have a 
+00001270: 7175 6573 7469 6f6e 2c20 796f 7520 6361  question, you ca
+00001280: 6e20 7573 6520 7468 6520 5361 5143 2075  n use the SaQC u
+00001290: 7365 7220 7375 7070 6f72 7420 6d61 696c  ser support mail
+000012a0: 696e 6720 6c69 7374 3a20 5b73 6171 632d  ing list: [saqc-
+000012b0: 7375 7070 6f72 7440 7566 7a2e 6465 5d28  support@ufz.de](
+000012c0: 6d61 696c 746f 3a73 6171 632d 7375 7070  mailto:saqc-supp
+000012d0: 6f72 7440 7566 7a2e 6465 290a 0a23 2320  ort@ufz.de)..## 
+000012e0: 436f 7079 7269 6768 7420 616e 6420 4c69  Copyright and Li
+000012f0: 6365 6e73 650a 436f 7079 7269 6768 7428  cense.Copyright(
+00001300: 6329 2032 3032 312c 205b 4865 6c6d 686f  c) 2021, [Helmho
+00001310: 6c74 7a2d 5a65 6e74 7275 6d20 66c3 bc72  ltz-Zentrum f..r
+00001320: 2055 6d77 656c 7466 6f72 7363 6875 6e67   Umweltforschung
+00001330: 2047 6d62 4820 2d2d 2055 465a 5d28 6874   GmbH -- UFZ](ht
+00001340: 7470 733a 2f2f 7777 772e 7566 7a2e 6465  tps://www.ufz.de
+00001350: 292e 2041 6c6c 2072 6967 6874 7320 7265  ). All rights re
+00001360: 7365 7276 6564 2e0a 0a2d 2044 6f63 756d  served...- Docum
+00001370: 656e 7461 7469 6f6e 3a20 5b43 7265 6174  entation: [Creat
+00001380: 6976 6520 436f 6d6d 6f6e 7320 4174 7472  ive Commons Attr
+00001390: 6962 7574 696f 6e20 342e 3020 496e 7465  ibution 4.0 Inte
+000013a0: 726e 6174 696f 6e61 6c5d 2868 7474 7073  rnational](https
+000013b0: 3a2f 2f63 7265 6174 6976 6563 6f6d 6d6f  ://creativecommo
+000013c0: 6e73 2e6f 7267 2f6c 6963 656e 7365 732f  ns.org/licenses/
+000013d0: 6279 2f34 2e30 2f29 203c 6120 7265 6c3d  by/4.0/) <a rel=
+000013e0: 226c 6963 656e 7365 2220 6872 6566 3d22  "license" href="
+000013f0: 6874 7470 3a2f 2f63 7265 6174 6976 6563  http://creativec
+00001400: 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963 656e  ommons.org/licen
+00001410: 7365 732f 6279 2f34 2e30 2f22 3e3c 696d  ses/by/4.0/"><im
+00001420: 6720 616c 743d 2243 7265 6174 6976 6520  g alt="Creative 
+00001430: 436f 6d6d 6f6e 7320 4c69 6365 6e73 6522  Commons License"
+00001440: 2073 7479 6c65 3d22 626f 7264 6572 2d77   style="border-w
+00001450: 6964 7468 3a30 2220 7372 633d 2268 7474  idth:0" src="htt
+00001460: 7073 3a2f 2f69 2e63 7265 6174 6976 6563  ps://i.creativec
+00001470: 6f6d 6d6f 6e73 2e6f 7267 2f6c 2f62 792f  ommons.org/l/by/
+00001480: 342e 302f 3830 7831 352e 706e 6722 202f  4.0/80x15.png" /
+00001490: 3e3c 2f61 3e0a 2d20 536f 7572 6365 2063  ></a>.- Source c
+000014a0: 6f64 653a 205b 474e 5520 4765 6e65 7261  ode: [GNU Genera
+000014b0: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000014c0: 2033 5d28 6874 7470 733a 2f2f 7777 772e   3](https://www.
+000014d0: 676e 752e 6f72 672f 6c69 6365 6e73 6573  gnu.org/licenses
+000014e0: 2f67 706c 2d33 2e30 2e68 746d 6c29 0a0a  /gpl-3.0.html)..
+000014f0: 466f 7220 6675 6c6c 2064 6574 6169 6c73  For full details
+00001500: 2c20 7365 6520 5b4c 4943 454e 5345 5d28  , see [LICENSE](
+00001510: 4c49 4345 4e53 452e 6d64 292e 0a0a 2323  LICENSE.md)...##
+00001520: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
+00001530: 730a 2e2e 2e0a 0a23 2320 5075 626c 6963  s......## Public
+00001540: 6174 696f 6e73 0a63 6f6d 696e 6720 736f  ations.coming so
+00001550: 6f6e 2e2e 2e0a 0a23 2320 486f 7720 746f  on.....## How to
+00001560: 2063 6974 6520 5361 5143 0a49 6620 5361   cite SaQC.If Sa
+00001570: 5143 2069 7320 6164 7661 6e63 696e 6720  QC is advancing 
+00001580: 796f 7572 2072 6573 6561 7263 682c 2070  your research, p
+00001590: 6c65 6173 6520 6369 7465 2061 733a 0a0a  lease cite as:..
+000015a0: 3e20 5363 68c3 a466 6572 2c20 4461 7669  > Sch..fer, Davi
+000015b0: 642c 2050 616c 6d2c 2042 6572 742c 204c  d, Palm, Bert, L
+000015c0: c3bc 6e65 6e73 6368 6c6f c39f 2c20 5065  ..nenschlo.., Pe
+000015d0: 7465 722c 2053 6368 6d69 6474 2c20 4c65  ter, Schmidt, Le
+000015e0: 6e6e 6172 742c 2026 2042 756d 6265 7267  nnart, & Bumberg
+000015f0: 6572 2c20 4a61 6e2e 2028 3230 3233 292e  er, Jan. (2023).
+00001600: 2053 7973 7465 6d20 666f 7220 6175 746f   System for auto
+00001610: 6d61 7465 6420 5175 616c 6974 7920 436f  mated Quality Co
+00001620: 6e74 726f 6c20 2d20 5361 5143 2028 322e  ntrol - SaQC (2.
+00001630: 332e 3029 2e20 5a65 6e6f 646f 2e20 6874  3.0). Zenodo. ht
+00001640: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00001650: 2e35 3238 312f 7a65 6e6f 646f 2e35 3838  .5281/zenodo.588
+00001660: 3835 3437 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d  8547..----------
+00001670: 2d2d 2d2d 2d2d 2d0a 0a3c 6120 6872 6566  -------..<a href
+00001680: 3d22 6874 7470 733a 2f2f 7777 772e 7566  ="https://www.uf
+00001690: 7a2e 6465 2f69 6e64 6578 2e70 6870 3f65  z.de/index.php?e
+000016a0: 6e3d 3333 3537 3322 3e0a 2020 2020 3c69  n=33573">.    <i
+000016b0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000016c0: 6769 742e 7566 7a2e 6465 2f72 646d 2d73  git.ufz.de/rdm-s
+000016d0: 6f66 7477 6172 652f 7361 7163 2f72 6177  oftware/saqc/raw
+000016e0: 2f64 6576 656c 6f70 2f64 6f63 732f 7265  /develop/docs/re
+000016f0: 736f 7572 6365 732f 696d 6167 6573 2f72  sources/images/r
+00001700: 6570 7265 7365 6e74 6174 6976 652f 5546  epresentative/UF
+00001710: 5a4c 6f67 6f2e 706e 6722 2077 6964 7468  ZLogo.png" width
+00001720: 3d22 3430 3022 2f3e 0a3c 2f61 3e0a 0a3c  ="400"/>.</a>..<
+00001730: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001740: 7777 772e 7566 7a2e 6465 2f69 6e64 6578  www.ufz.de/index
+00001750: 2e70 6870 3f65 6e3d 3435 3334 3822 3e0a  .php?en=45348">.
+00001760: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00001770: 7470 733a 2f2f 6769 742e 7566 7a2e 6465  tps://git.ufz.de
+00001780: 2f72 646d 2d73 6f66 7477 6172 652f 7361  /rdm-software/sa
+00001790: 7163 2f72 6177 2f64 6576 656c 6f70 2f64  qc/raw/develop/d
+000017a0: 6f63 732f 7265 736f 7572 6365 732f 696d  ocs/resources/im
+000017b0: 6167 6573 2f72 6570 7265 7365 6e74 6174  ages/representat
+000017c0: 6976 652f 5244 4d4c 6f67 6f2e 706e 6722  ive/RDMLogo.png"
+000017d0: 2061 6c69 676e 3d22 7269 6768 7422 2077   align="right" w
+000017e0: 6964 7468 3d22 3232 3022 2f3e 0a3c 2f61  idth="220"/>.</a
+000017f0: 3e0a                                     >.
```

### Comparing `saqc-2.3/README.md` & `saqc-2.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,342 +2,357 @@
 00000010: 7079 7269 6768 7454 6578 743a 2032 3032  pyrightText: 202
 00000020: 3120 4865 6c6d 686f 6c74 7a2d 5a65 6e74  1 Helmholtz-Zent
 00000030: 7275 6d20 66c3 bc72 2055 6d77 656c 7466  rum f..r Umweltf
 00000040: 6f72 7363 6875 6e67 2047 6d62 4820 2d20  orschung GmbH - 
 00000050: 5546 5a0a 0a53 5044 582d 4c69 6365 6e73  UFZ..SPDX-Licens
 00000060: 652d 4964 656e 7469 6669 6572 3a20 4750  e-Identifier: GP
 00000070: 4c2d 332e 302d 6f72 2d6c 6174 6572 0a2d  L-3.0-or-later.-
-00000080: 2d3e 0a0a 3c61 2068 7265 663d 2268 7474  ->..<a href="htt
-00000090: 7073 3a2f 2f77 7777 2e75 667a 2e64 652f  ps://www.ufz.de/
-000000a0: 696e 6465 782e 7068 703f 656e 3d33 3335  index.php?en=335
-000000b0: 3733 223e 0a20 2020 203c 696d 6720 7372  73">.    <img sr
-000000c0: 633d 2268 7474 7073 3a2f 2f67 6974 2e75  c="https://git.u
-000000d0: 667a 2e64 652f 7264 6d2d 736f 6674 7761  fz.de/rdm-softwa
-000000e0: 7265 2f73 6171 632f 7261 772f 6465 7665  re/saqc/raw/deve
-000000f0: 6c6f 702f 646f 6373 2f72 6573 6f75 7263  lop/docs/resourc
-00000100: 6573 2f69 6d61 6765 732f 7265 7072 6573  es/images/repres
-00000110: 656e 7461 7469 7665 2f55 465a 4c6f 676f  entative/UFZLogo
-00000120: 2e70 6e67 2220 7769 6474 683d 2234 3030  .png" width="400
-00000130: 222f 3e0a 3c2f 613e 0a0a 3c61 2068 7265  "/>.</a>..<a hre
-00000140: 663d 2268 7474 7073 3a2f 2f77 7777 2e75  f="https://www.u
-00000150: 667a 2e64 652f 696e 6465 782e 7068 703f  fz.de/index.php?
-00000160: 656e 3d34 3533 3438 223e 0a20 2020 203c  en=45348">.    <
-00000170: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000180: 2f67 6974 2e75 667a 2e64 652f 7264 6d2d  /git.ufz.de/rdm-
-00000190: 736f 6674 7761 7265 2f73 6171 632f 7261  software/saqc/ra
-000001a0: 772f 6465 7665 6c6f 702f 646f 6373 2f72  w/develop/docs/r
-000001b0: 6573 6f75 7263 6573 2f69 6d61 6765 732f  esources/images/
-000001c0: 7265 7072 6573 656e 7461 7469 7665 2f52  representative/R
-000001d0: 444d 4c6f 676f 2e70 6e67 2220 616c 6967  DMLogo.png" alig
-000001e0: 6e3d 2272 6967 6874 2220 7769 6474 683d  n="right" width=
-000001f0: 2232 3230 222f 3e0a 3c2f 613e 0a0a 5b21  "220"/>.</a>..[!
-00000200: 5b50 726f 6a65 6374 2053 7461 7475 733a  [Project Status:
-00000210: 2041 6374 6976 6520 e280 9320 5468 6520   Active ... The 
-00000220: 7072 6f6a 6563 7420 6861 7320 7265 6163  project has reac
-00000230: 6865 6420 6120 7374 6162 6c65 2c20 7573  hed a stable, us
-00000240: 6162 6c65 2073 7461 7465 2061 6e64 2069  able state and i
-00000250: 7320 6265 696e 6720 6163 7469 7665 6c79  s being actively
-00000260: 2064 6576 656c 6f70 6564 2e5d 2868 7474   developed.](htt
-00000270: 7073 3a2f 2f77 7777 2e72 6570 6f73 7461  ps://www.reposta
-00000280: 7475 732e 6f72 672f 6261 6467 6573 2f6c  tus.org/badges/l
-00000290: 6174 6573 742f 6163 7469 7665 2e73 7667  atest/active.svg
-000002a0: 295d 2868 7474 7073 3a2f 2f77 7777 2e72  )](https://www.r
-000002b0: 6570 6f73 7461 7475 732e 6f72 672f 2361  epostatus.org/#a
-000002c0: 6374 6976 6529 0a0a 0a23 2053 7973 7465  ctive)...# Syste
-000002d0: 6d20 666f 7220 6175 746f 6d61 7465 6420  m for automated 
-000002e0: 5175 616c 6974 7920 436f 6e74 726f 6c20  Quality Control 
-000002f0: 2853 6151 4329 0a0a 416e 6f6d 616c 6965  (SaQC)..Anomalie
-00000300: 7320 616e 6420 6572 726f 7273 2061 7265  s and errors are
-00000310: 2074 6865 2072 756c 6520 6e6f 7420 7468   the rule not th
-00000320: 6520 6578 6365 7074 696f 6e20 7768 656e  e exception when
-00000330: 2077 6f72 6b69 6e67 2077 6974 6820 0a74   working with .t
-00000340: 696d 6520 7365 7269 6573 2064 6174 612e  ime series data.
-00000350: 2054 6869 7320 6973 2065 7370 6563 6961   This is especia
-00000360: 6c6c 7920 7472 7565 2c20 6966 2073 7563  lly true, if suc
-00000370: 6820 6461 7461 206f 7269 6769 6e61 7465  h data originate
-00000380: 730a 6672 6f6d 2069 6e2d 7369 7475 206d  s.from in-situ m
-00000390: 6561 7375 7265 6d65 6e74 7320 6f66 2065  easurements of e
-000003a0: 6e76 6972 6f6e 6d65 6e74 616c 2070 726f  nvironmental pro
-000003b0: 7065 7274 6965 732e 200a 416c 6d6f 7374  perties. .Almost
-000003c0: 2061 6c6c 2061 7070 6c69 6361 7469 6f6e   all application
-000003d0: 732c 2068 6f77 6576 6572 2c20 696d 706c  s, however, impl
-000003e0: 6963 696c 7920 7265 6c79 206f 6e20 6461  icily rely on da
-000003f0: 7461 2c20 7468 6174 2063 6f6d 706c 6965  ta, that complie
-00000400: 730a 7769 7468 2073 6f6d 6520 6465 6669  s.with some defi
-00000410: 6e69 7469 6f6e 206f 6620 2763 6f72 7265  nition of 'corre
-00000420: 6374 272e 200a 496e 206f 7264 6572 2074  ct'. .In order t
-00000430: 6f20 696e 6665 7220 7265 6c69 6162 6c65  o infer reliable
-00000440: 2064 6174 6120 7072 6f64 7563 7473 2061   data products a
-00000450: 6e64 2074 6f6f 6c73 2c20 7468 6572 6520  nd tools, there 
-00000460: 6973 206e 6f20 616c 7465 726e 6174 6976  is no alternativ
-00000470: 650a 746f 2071 7561 6c69 7479 2063 6f6e  e.to quality con
-00000480: 7472 6f6c 2e20 5361 5143 2070 726f 7669  trol. SaQC provi
-00000490: 6465 7320 616c 6c20 7468 6520 6275 696c  des all the buil
-000004a0: 6469 6e67 2062 6c6f 636b 7320 746f 2063  ding blocks to c
-000004b0: 6f6d 666f 7274 6162 6c79 0a62 7269 6467  omfortably.bridg
-000004c0: 6520 7468 6520 6761 7020 6265 7477 6565  e the gap betwee
-000004d0: 6e20 2775 7375 616c 6c79 2066 6175 6c74  n 'usually fault
-000004e0: 7927 2061 6e64 2027 6578 7065 6374 6564  y' and 'expected
-000004f0: 2074 6f20 6265 2063 6f72 7265 6374 6564   to be corrected
-00000500: 2720 696e 200a 6120 6163 6365 7373 6962  ' in .a accessib
-00000510: 6c65 2c20 636f 6e73 6973 7465 6e74 2c20  le, consistent, 
-00000520: 6f62 6a65 6374 6976 6520 616e 6420 7265  objective and re
-00000530: 7072 6f64 7563 6962 6c65 2077 6179 2e0a  producible way..
-00000540: 0a46 6f72 2061 2028 636f 6e74 696e 6f75  .For a (continou
-00000550: 736c 7920 696d 7072 6f76 696e 6729 206f  sly improving) o
-00000560: 7665 7276 6965 7720 6f66 2066 6561 7475  verview of featu
-00000570: 7265 732c 2074 7970 6963 616c 2075 7361  res, typical usa
-00000580: 6765 2070 6174 7465 726e 732c 0a74 6865  ge patterns,.the
-00000590: 2073 7065 6369 6669 6320 7379 7374 656d   specific system
-000005a0: 2063 6f6d 706f 6e65 6e74 7320 616e 6420   components and 
-000005b0: 686f 7720 746f 2063 7573 746f 6d69 7a65  how to customize
-000005c0: 2060 5361 5143 6020 746f 2079 6f75 7220   `SaQC` to your 
-000005d0: 7370 6563 6966 6963 0a6e 6565 6473 2c20  specific.needs, 
-000005e0: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
-000005f0: 6f75 720a 5b6f 6e6c 696e 6520 646f 6375  our.[online docu
-00000600: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00000610: 3a2f 2f72 646d 2d73 6f66 7477 6172 652e  ://rdm-software.
-00000620: 7061 6765 732e 7566 7a2e 6465 2f73 6171  pages.ufz.de/saq
-00000630: 632f 696e 6465 782e 6874 6d6c 292e 0a0a  c/index.html)...
-00000640: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000650: 0a0a 5361 5143 2069 7320 6176 6169 6c61  ..SaQC is availa
-00000660: 626c 6520 6f6e 2074 6865 2050 7974 686f  ble on the Pytho
-00000670: 6e20 5061 636b 6167 6520 496e 6465 7820  n Package Index 
-00000680: 285b 5079 5049 5d28 6874 7470 733a 2f2f  ([PyPI](https://
-00000690: 7079 7069 2e6f 7267 2f29 2920 616e 640a  pypi.org/)) and.
-000006a0: 6361 6e20 6265 2069 6e73 7461 6c6c 6564  can be installed
-000006b0: 2075 7369 6e67 205b 7069 705d 2868 7474   using [pip](htt
-000006c0: 7073 3a2f 2f70 6970 2e70 7970 612e 696f  ps://pip.pypa.io
-000006d0: 2f65 6e2f 7374 6162 6c65 2f29 3a0a 6060  /en/stable/):.``
-000006e0: 6073 680a 7079 7468 6f6e 202d 6d20 7069  `sh.python -m pi
-000006f0: 7020 696e 7374 616c 6c20 7361 7163 0a60  p install saqc.`
-00000700: 6060 0a46 6f72 2061 206d 6f72 6520 6465  ``.For a more de
-00000710: 7461 696c 6564 2069 6e73 7461 6c6c 696f  tailed installio
-00000720: 6e20 6775 6964 652c 2073 6565 2074 6865  n guide, see the
-00000730: 205b 696e 7374 616c 6c61 7469 6f6e 2067   [installation g
-00000740: 7569 6465 5d28 6874 7470 733a 2f2f 7264  uide](https://rd
-00000750: 6d2d 736f 6674 7761 7265 2e70 6167 6573  m-software.pages
-00000760: 2e75 667a 2e64 652f 7361 7163 2f67 6574  .ufz.de/saqc/get
-00000770: 7469 6e67 7374 6172 7465 642f 496e 7374  tingstarted/Inst
-00000780: 616c 6c61 7469 6f6e 4775 6964 652e 6874  allationGuide.ht
-00000790: 6d6c 292e 0a0a 2323 2055 7361 6765 0a0a  ml)...## Usage..
-000007a0: 6053 6151 4360 2069 7320 626f 7468 2c20  `SaQC` is both, 
-000007b0: 6120 636f 6d6d 616e 6420 6c69 6e65 2061  a command line a
-000007c0: 7070 6c69 6361 7469 6f6e 2063 6f6e 7472  pplication contr
-000007d0: 6f6c 6c65 6420 6279 2061 2074 6578 7420  olled by a text 
-000007e0: 6261 7365 6420 636f 6e66 6967 7572 6174  based configurat
-000007f0: 696f 6e0a 616e 6420 6120 7079 7468 6f6e  ion.and a python
-00000800: 206d 6f64 756c 6520 7769 7468 2061 2073   module with a s
-00000810: 696d 706c 6520 4150 492e 0a0a 2323 2320  imple API...### 
-00000820: 5361 5143 2061 7320 6120 636f 6d6d 616e  SaQC as a comman
-00000830: 6420 6c69 6e65 2061 7070 6c69 6361 7469  d line applicati
-00000840: 6f6e 0a54 6865 2063 6f6d 6d61 6e64 206c  on.The command l
-00000850: 696e 6520 6170 706c 6963 6174 696f 6e20  ine application 
-00000860: 6973 2063 6f6e 7472 6f6c 6c65 6420 6279  is controlled by
-00000870: 2061 2073 656d 6963 6f6c 6f6e 2d73 6570   a semicolon-sep
-00000880: 6172 6174 6564 2074 6578 740a 6669 6c65  arated text.file
-00000890: 206c 6973 7469 6e67 2074 6865 2076 6172   listing the var
-000008a0: 6961 626c 6573 2069 6e20 7468 6520 6461  iables in the da
-000008b0: 7461 7365 7420 616e 6420 7468 6520 726f  taset and the ro
-000008c0: 7574 696e 6573 2074 6f20 696e 7370 6563  utines to inspec
-000008d0: 742c 0a71 7561 6c69 7479 2063 6f6e 7472  t,.quality contr
-000008e0: 6f6c 2061 6e64 2f6f 7220 7072 6f63 6573  ol and/or proces
-000008f0: 7320 7468 656d 2e20 5468 6520 636f 6e74  s them. The cont
-00000900: 656e 7420 6f66 2073 7563 6820 6120 636f  ent of such a co
-00000910: 6e66 6967 7572 6174 696f 6e0a 636f 756c  nfiguration.coul
-00000920: 6420 6c6f 6f6b 206c 696b 6520 5b74 6869  d look like [thi
-00000930: 735d 2868 7474 7073 3a2f 2f67 6974 2e75  s](https://git.u
-00000940: 667a 2e64 652f 7264 6d2d 736f 6674 7761  fz.de/rdm-softwa
-00000950: 7265 2f73 6171 632f 7261 772f 6465 7665  re/saqc/raw/deve
-00000960: 6c6f 702f 646f 6373 2f72 6573 6f75 7263  lop/docs/resourc
-00000970: 6573 2f64 6174 612f 636f 6e66 6967 2e63  es/data/config.c
-00000980: 7376 293a 0a0a 6060 600a 7661 726e 616d  sv):..```.varnam
-00000990: 6520 2020 203b 2074 6573 740a 232d 2d2d  e    ; test.#---
-000009a0: 2d2d 2d2d 2d2d 2d3b 202d 2d2d 2d2d 2d2d  -------; -------
-000009b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a53  --------------.S
-000009f0: 4d32 2020 2020 2020 2020 3b20 7368 6966  M2        ; shif
-00000a00: 7428 6672 6571 3d22 3135 4d69 6e22 290a  t(freq="15Min").
-00000a10: 2753 4d28 317c 3229 2b27 203b 2066 6c61  'SM(1|2)+' ; fla
-00000a20: 674d 6973 7369 6e67 2829 0a53 4d31 2020  gMissing().SM1  
-00000a30: 2020 2020 2020 3b20 666c 6167 5261 6e67        ; flagRang
-00000a40: 6528 6d69 6e3d 3130 2c20 6d61 783d 3630  e(min=10, max=60
-00000a50: 290a 534d 3220 2020 2020 2020 203b 2066  ).SM2        ; f
-00000a60: 6c61 6752 616e 6765 286d 696e 3d31 302c  lagRange(min=10,
-00000a70: 206d 6178 3d34 3029 0a53 4d32 2020 2020   max=40).SM2    
-00000a80: 2020 2020 3b20 666c 6167 4d41 4428 7769      ; flagMAD(wi
-00000a90: 6e64 6f77 3d22 3330 6422 2c20 7a3d 332e  ndow="30d", z=3.
-00000aa0: 3529 0a44 756d 6d79 2020 2020 2020 3b20  5).Dummy      ; 
-00000ab0: 666c 6167 4765 6e65 7269 6328 6669 656c  flagGeneric(fiel
-00000ac0: 643d 5b22 534d 3122 2c20 2253 4d32 225d  d=["SM1", "SM2"]
-00000ad0: 2c20 6675 6e63 3d28 6973 666c 6167 6765  , func=(isflagge
-00000ae0: 6428 7829 207c 2069 7366 6c61 6767 6564  d(x) | isflagged
-00000af0: 2879 2929 290a 6060 600a 0a41 7320 736f  (y))).```..As so
-00000b00: 6f6e 2061 7320 7468 6520 6261 7369 6320  on as the basic 
-00000b10: 696e 7075 7473 2c20 6461 7461 7365 7420  inputs, dataset 
-00000b20: 616e 6420 636f 6e66 6967 7572 6174 696f  and configuratio
-00000b30: 6e20 6669 6c65 2c20 6172 650a 7072 6570  n file, are.prep
-00000b40: 6172 6564 2c20 7275 6e20 6053 6151 4360  ared, run `SaQC`
-00000b50: 3a0a 6060 6073 680a 7361 7163 205c 0a20  :.```sh.saqc \. 
-00000b60: 2020 202d 2d63 6f6e 6669 6720 5041 5448     --config PATH
-00000b70: 5f54 4f5f 434f 4e46 4947 5552 4154 494f  _TO_CONFIGURATIO
-00000b80: 4e20 5c0a 2020 2020 2d2d 6461 7461 2050  N \.    --data P
-00000b90: 4154 485f 544f 5f44 4154 4120 5c0a 2020  ATH_TO_DATA \.  
-00000ba0: 2020 2d2d 6f75 7466 696c 6520 5041 5448    --outfile PATH
-00000bb0: 5f54 4f5f 4f55 5450 5554 0a60 6060 0a0a  _TO_OUTPUT.```..
-00000bc0: 4120 6675 6c6c 2060 5361 5143 6020 7275  A full `SaQC` ru
-00000bd0: 6e20 6167 6169 6e73 7420 7072 6f76 6964  n against provid
-00000be0: 6564 2065 7861 6d70 6c65 2064 6174 6120  ed example data 
-00000bf0: 6361 6e20 6265 2069 6e76 6f6b 6564 2077  can be invoked w
-00000c00: 6974 683a 0a60 6060 7368 0a73 6171 6320  ith:.```sh.saqc 
-00000c10: 5c0a 2020 2020 2d2d 636f 6e66 6967 2068  \.    --config h
-00000c20: 7474 7073 3a2f 2f67 6974 2e75 667a 2e64  ttps://git.ufz.d
-00000c30: 652f 7264 6d2d 736f 6674 7761 7265 2f73  e/rdm-software/s
-00000c40: 6171 632f 7261 772f 6465 7665 6c6f 702f  aqc/raw/develop/
-00000c50: 646f 6373 2f72 6573 6f75 7263 6573 2f64  docs/resources/d
-00000c60: 6174 612f 636f 6e66 6967 2e63 7376 205c  ata/config.csv \
-00000c70: 0a20 2020 202d 2d64 6174 6120 6874 7470  .    --data http
-00000c80: 733a 2f2f 6769 742e 7566 7a2e 6465 2f72  s://git.ufz.de/r
-00000c90: 646d 2d73 6f66 7477 6172 652f 7361 7163  dm-software/saqc
-00000ca0: 2f72 6177 2f64 6576 656c 6f70 2f64 6f63  /raw/develop/doc
-00000cb0: 732f 7265 736f 7572 6365 732f 6461 7461  s/resources/data
-00000cc0: 2f64 6174 612e 6373 7620 5c0a 2020 2020  /data.csv \.    
-00000cd0: 2d2d 6f75 7466 696c 6520 7361 7163 5f74  --outfile saqc_t
-00000ce0: 6573 742e 6373 760a 6060 600a 0a23 2323  est.csv.```..###
-00000cf0: 2053 6151 4320 6173 2061 2070 7974 686f   SaQC as a pytho
-00000d00: 6e20 6d6f 6475 6c65 0a0a 5468 6520 666f  n module..The fo
-00000d10: 6c6c 6f77 696e 6720 736e 6970 7065 7420  llowing snippet 
-00000d20: 696d 706c 656d 656e 7473 2074 6865 2073  implements the s
-00000d30: 616d 6520 636f 6e66 6967 7572 6174 696f  ame configuratio
-00000d40: 6e20 6769 7665 6e20 6162 6f76 6520 7468  n given above th
-00000d50: 726f 7567 680a 7468 6520 5079 7468 6f6e  rough.the Python
-00000d60: 2d41 5049 3a0a 0a60 6060 7079 7468 6f6e  -API:..```python
-00000d70: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
-00000d80: 7320 7064 0a66 726f 6d20 7361 7163 2069  s pd.from saqc i
-00000d90: 6d70 6f72 7420 5361 5143 0a0a 6461 7461  mport SaQC..data
-00000da0: 203d 2070 642e 7265 6164 5f63 7376 280a   = pd.read_csv(.
-00000db0: 2020 2020 2268 7474 7073 3a2f 2f67 6974      "https://git
-00000dc0: 2e75 667a 2e64 652f 7264 6d2d 736f 6674  .ufz.de/rdm-soft
-00000dd0: 7761 7265 2f73 6171 632f 7261 772f 6465  ware/saqc/raw/de
-00000de0: 7665 6c6f 702f 646f 6373 2f72 6573 6f75  velop/docs/resou
-00000df0: 7263 6573 2f64 6174 612f 6461 7461 2e63  rces/data/data.c
-00000e00: 7376 222c 0a20 2020 2069 6e64 6578 5f63  sv",.    index_c
-00000e10: 6f6c 3d30 2c20 7061 7273 655f 6461 7465  ol=0, parse_date
-00000e20: 733d 5472 7565 2c0a 290a 0a73 6171 6320  s=True,.)..saqc 
-00000e30: 3d20 5361 5143 2864 6174 613d 6461 7461  = SaQC(data=data
-00000e40: 290a 7361 7163 203d 2028 7361 7163 0a20  ).saqc = (saqc. 
-00000e50: 2020 2020 2020 202e 7368 6966 7428 2253         .shift("S
-00000e60: 4d32 222c 2066 7265 713d 2231 354d 696e  M2", freq="15Min
-00000e70: 2229 0a20 2020 2020 2020 202e 666c 6167  ").        .flag
-00000e80: 4d69 7373 696e 6728 2253 4d28 317c 3229  Missing("SM(1|2)
-00000e90: 2b22 2c20 7265 6765 783d 5472 7565 290a  +", regex=True).
-00000ea0: 2020 2020 2020 2020 2e66 6c61 6752 616e          .flagRan
-00000eb0: 6765 2822 534d 3122 2c20 6d69 6e3d 3130  ge("SM1", min=10
-00000ec0: 2c20 6d61 783d 3630 290a 2020 2020 2020  , max=60).      
-00000ed0: 2020 2e66 6c61 6752 616e 6765 2822 534d    .flagRange("SM
-00000ee0: 3222 2c20 6d69 6e3d 3130 2c20 6d61 783d  2", min=10, max=
-00000ef0: 3430 290a 2020 2020 2020 2020 2e66 6c61  40).        .fla
-00000f00: 674d 4144 2822 534d 3222 2c20 7769 6e64  gMAD("SM2", wind
-00000f10: 6f77 3d22 3330 6422 2c20 7a3d 332e 3529  ow="30d", z=3.5)
-00000f20: 0a20 2020 2020 2020 202e 666c 6167 4765  .        .flagGe
-00000f30: 6e65 7269 6328 6669 656c 643d 5b22 534d  neric(field=["SM
-00000f40: 3122 2c20 2253 4d32 225d 2c20 7461 7267  1", "SM2"], targ
-00000f50: 6574 3d22 4475 6d6d 7922 2c20 6675 6e63  et="Dummy", func
-00000f60: 3d6c 616d 6264 6120 782c 2079 3a20 2869  =lambda x, y: (i
-00000f70: 7366 6c61 6767 6564 2878 2920 7c20 6973  sflagged(x) | is
-00000f80: 666c 6167 6765 6428 7929 2929 290a 6060  flagged(y)))).``
-00000f90: 600a 0a41 206d 6f72 6520 6465 7461 696c  `..A more detail
-00000fa0: 6564 2064 6573 6372 6970 7469 6f6e 206f  ed description o
-00000fb0: 6620 7468 6520 5079 7468 6f6e 2041 5049  f the Python API
-00000fc0: 2069 7320 6176 6169 6c61 626c 6520 696e   is available in
-00000fd0: 2074 6865 200a 5b72 6573 7065 6374 6976   the .[respectiv
-00000fe0: 6520 7365 6374 696f 6e5d 2868 7474 7073  e section](https
-00000ff0: 3a2f 2f72 646d 2d73 6f66 7477 6172 652e  ://rdm-software.
-00001000: 7061 6765 732e 7566 7a2e 6465 2f73 6171  pages.ufz.de/saq
-00001010: 632f 6765 7474 696e 6773 7461 7274 6564  c/gettingstarted
-00001020: 2f54 7574 6f72 6961 6c41 5049 2e68 746d  /TutorialAPI.htm
-00001030: 6c29 0a6f 6620 7468 6520 646f 6375 6d65  l).of the docume
-00001040: 6e74 6174 696f 6e2e 0a0a 2323 2043 6861  ntation...## Cha
-00001050: 6e67 656c 6f67 0a41 6c6c 206e 6f74 6162  ngelog.All notab
-00001060: 6c65 2063 6861 6e67 6573 2074 6f20 7468  le changes to th
-00001070: 6973 2070 726f 6a65 6374 2077 696c 6c20  is project will 
-00001080: 6265 2064 6f63 756d 656e 7465 6420 696e  be documented in
-00001090: 205b 4348 414e 4745 4c4f 472e 6d64 5d28   [CHANGELOG.md](
-000010a0: 4348 414e 4745 4c4f 472e 6d64 292e 0a0a  CHANGELOG.md)...
-000010b0: 2323 2047 6574 2069 6e76 6f6c 7665 640a  ## Get involved.
-000010c0: 0a23 2323 2043 6f6e 7472 6962 7574 696e  .### Contributin
-000010d0: 670a 596f 7520 666f 756e 6420 6120 6275  g.You found a bu
-000010e0: 6720 6f72 2079 6f75 2077 616e 7420 746f  g or you want to
-000010f0: 2073 7567 6765 7374 2073 6f6d 6520 636f   suggest some co
-00001100: 6f6c 2066 6561 7475 7265 733f 2050 6c65  ol features? Ple
-00001110: 6173 6520 7265 6665 7220 746f 206f 7572  ase refer to our
-00001120: 205b 636f 6e74 7269 6275 7469 6e67 2067   [contributing g
-00001130: 7569 6465 6c69 6e65 735d 2843 4f4e 5452  uidelines](CONTR
-00001140: 4942 5554 494e 472e 6d64 2920 746f 2073  IBUTING.md) to s
-00001150: 6565 2068 6f77 2079 6f75 2063 616e 2063  ee how you can c
-00001160: 6f6e 7472 6962 7574 6520 746f 2053 6151  ontribute to SaQ
-00001170: 432e 0a0a 2323 2320 5573 6572 2073 7570  C...### User sup
-00001180: 706f 7274 0a49 6620 796f 7520 6e65 6564  port.If you need
-00001190: 2068 656c 7020 6f72 2068 6176 6520 6120   help or have a 
-000011a0: 7175 6573 7469 6f6e 2c20 796f 7520 6361  question, you ca
-000011b0: 6e20 7573 6520 7468 6520 5361 5143 2075  n use the SaQC u
-000011c0: 7365 7220 7375 7070 6f72 7420 6d61 696c  ser support mail
-000011d0: 696e 6720 6c69 7374 3a20 5b73 6171 632d  ing list: [saqc-
-000011e0: 7375 7070 6f72 7440 7566 7a2e 6465 5d28  support@ufz.de](
-000011f0: 6d61 696c 746f 3a73 6171 632d 7375 7070  mailto:saqc-supp
-00001200: 6f72 7440 7566 7a2e 6465 290a 0a23 2320  ort@ufz.de)..## 
-00001210: 436f 7079 7269 6768 7420 616e 6420 4c69  Copyright and Li
-00001220: 6365 6e73 650a 436f 7079 7269 6768 7428  cense.Copyright(
-00001230: 6329 2032 3032 312c 205b 4865 6c6d 686f  c) 2021, [Helmho
-00001240: 6c74 7a2d 5a65 6e74 7275 6d20 66c3 bc72  ltz-Zentrum f..r
-00001250: 2055 6d77 656c 7466 6f72 7363 6875 6e67   Umweltforschung
-00001260: 2047 6d62 4820 2d2d 2055 465a 5d28 6874   GmbH -- UFZ](ht
-00001270: 7470 733a 2f2f 7777 772e 7566 7a2e 6465  tps://www.ufz.de
-00001280: 292e 2041 6c6c 2072 6967 6874 7320 7265  ). All rights re
-00001290: 7365 7276 6564 2e0a 0a2d 2044 6f63 756d  served...- Docum
-000012a0: 656e 7461 7469 6f6e 3a20 5b43 7265 6174  entation: [Creat
-000012b0: 6976 6520 436f 6d6d 6f6e 7320 4174 7472  ive Commons Attr
-000012c0: 6962 7574 696f 6e20 342e 3020 496e 7465  ibution 4.0 Inte
-000012d0: 726e 6174 696f 6e61 6c5d 2868 7474 7073  rnational](https
-000012e0: 3a2f 2f63 7265 6174 6976 6563 6f6d 6d6f  ://creativecommo
-000012f0: 6e73 2e6f 7267 2f6c 6963 656e 7365 732f  ns.org/licenses/
-00001300: 6279 2f34 2e30 2f29 203c 6120 7265 6c3d  by/4.0/) <a rel=
-00001310: 226c 6963 656e 7365 2220 6872 6566 3d22  "license" href="
-00001320: 6874 7470 3a2f 2f63 7265 6174 6976 6563  http://creativec
-00001330: 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963 656e  ommons.org/licen
-00001340: 7365 732f 6279 2f34 2e30 2f22 3e3c 696d  ses/by/4.0/"><im
-00001350: 6720 616c 743d 2243 7265 6174 6976 6520  g alt="Creative 
-00001360: 436f 6d6d 6f6e 7320 4c69 6365 6e73 6522  Commons License"
-00001370: 2073 7479 6c65 3d22 626f 7264 6572 2d77   style="border-w
-00001380: 6964 7468 3a30 2220 7372 633d 2268 7474  idth:0" src="htt
-00001390: 7073 3a2f 2f69 2e63 7265 6174 6976 6563  ps://i.creativec
-000013a0: 6f6d 6d6f 6e73 2e6f 7267 2f6c 2f62 792f  ommons.org/l/by/
-000013b0: 342e 302f 3830 7831 352e 706e 6722 202f  4.0/80x15.png" /
-000013c0: 3e3c 2f61 3e0a 2d20 536f 7572 6365 2063  ></a>.- Source c
-000013d0: 6f64 653a 205b 474e 5520 4765 6e65 7261  ode: [GNU Genera
-000013e0: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
-000013f0: 2033 5d28 6874 7470 733a 2f2f 7777 772e   3](https://www.
-00001400: 676e 752e 6f72 672f 6c69 6365 6e73 6573  gnu.org/licenses
-00001410: 2f67 706c 2d33 2e30 2e68 746d 6c29 0a0a  /gpl-3.0.html)..
-00001420: 466f 7220 6675 6c6c 2064 6574 6169 6c73  For full details
-00001430: 2c20 7365 6520 5b4c 4943 454e 5345 5d28  , see [LICENSE](
-00001440: 4c49 4345 4e53 452e 6d64 292e 0a0a 2323  LICENSE.md)...##
-00001450: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
-00001460: 730a 2e2e 2e0a 0a23 2320 5075 626c 6963  s......## Public
-00001470: 6174 696f 6e73 0a63 6f6d 696e 6720 736f  ations.coming so
-00001480: 6f6e 2e2e 2e0a 0a23 2320 486f 7720 746f  on.....## How to
-00001490: 2063 6974 6520 5361 5143 0a49 6620 5361   cite SaQC.If Sa
-000014a0: 5143 2069 7320 6164 7661 6e63 696e 6720  QC is advancing 
-000014b0: 796f 7572 2072 6573 6561 7263 682c 2070  your research, p
-000014c0: 6c65 6173 6520 6369 7465 2061 733a 0a0a  lease cite as:..
-000014d0: 3e20 5363 68c3 a466 6572 2c20 4461 7669  > Sch..fer, Davi
-000014e0: 643b 2050 616c 6d2c 2042 6572 743b 204c  d; Palm, Bert; L
-000014f0: c3bc 6e65 6e73 6368 6c6f c39f 2c20 5065  ..nenschlo.., Pe
-00001500: 7465 722e 2028 3230 3231 292e 2053 7973  ter. (2021). Sys
-00001510: 7465 6d20 666f 7220 6175 746f 6d61 7465  tem for automate
-00001520: 6420 5175 616c 6974 7920 436f 6e74 726f  d Quality Contro
-00001530: 6c20 2d20 5361 5143 2e20 5a65 6e6f 646f  l - SaQC. Zenodo
-00001540: 2e20 6874 7470 733a 2f2f 646f 692e 6f72  . https://doi.or
-00001550: 672f 3130 2e35 3238 312f 7a65 6e6f 646f  g/10.5281/zenodo
-00001560: 2e35 3838 3835 3437 0a                   .5888547.
+00000080: 2d3e 0a0a 3c62 723e 0a3c 6469 7620 616c  ->..<br>.<div al
+00000090: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000000a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000000b0: 2f2f 6769 742e 7566 7a2e 6465 2f72 646d  //git.ufz.de/rdm
+000000c0: 2d73 6f66 7477 6172 652f 7361 7163 2f72  -software/saqc/r
+000000d0: 6177 2f64 6576 656c 6f70 2f64 6f63 732f  aw/develop/docs/
+000000e0: 7265 736f 7572 6365 732f 696d 6167 6573  resources/images
+000000f0: 2f72 6570 7265 7365 6e74 6174 6976 652f  /representative/
+00000100: 5361 5143 4c6f 676f 2e70 6e67 2220 7769  SaQCLogo.png" wi
+00000110: 6474 683d 2233 3030 223e 0a3c 2f64 6976  dth="300">.</div
+00000120: 3e0a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  >..-------------
+00000130: 2d2d 2d2d 0a5b 215b 5072 6f6a 6563 7420  ----.[![Project 
+00000140: 5374 6174 7573 3a20 4163 7469 7665 20e2  Status: Active .
+00000150: 8093 2054 6865 2070 726f 6a65 6374 2068  .. The project h
+00000160: 6173 2072 6561 6368 6564 2061 2073 7461  as reached a sta
+00000170: 626c 652c 2075 7361 626c 6520 7374 6174  ble, usable stat
+00000180: 6520 616e 6420 6973 2062 6569 6e67 2061  e and is being a
+00000190: 6374 6976 656c 7920 6465 7665 6c6f 7065  ctively develope
+000001a0: 642e 5d28 6874 7470 733a 2f2f 7777 772e  d.](https://www.
+000001b0: 7265 706f 7374 6174 7573 2e6f 7267 2f62  repostatus.org/b
+000001c0: 6164 6765 732f 6c61 7465 7374 2f61 6374  adges/latest/act
+000001d0: 6976 652e 7376 6729 5d28 6874 7470 733a  ive.svg)](https:
+000001e0: 2f2f 7777 772e 7265 706f 7374 6174 7573  //www.repostatus
+000001f0: 2e6f 7267 2f23 6163 7469 7665 290a 0a23  .org/#active)..#
+00000200: 2020 5361 5143 3a20 5379 7374 656d 2066    SaQC: System f
+00000210: 6f72 2061 7574 6f6d 6174 6564 2051 7561  or automated Qua
+00000220: 6c69 7479 2043 6f6e 7472 6f6c 0a0a 416e  lity Control..An
+00000230: 6f6d 616c 6965 7320 616e 6420 6572 726f  omalies and erro
+00000240: 7273 2061 7265 2074 6865 2072 756c 6520  rs are the rule 
+00000250: 6e6f 7420 7468 6520 6578 6365 7074 696f  not the exceptio
+00000260: 6e20 7768 656e 2077 6f72 6b69 6e67 2077  n when working w
+00000270: 6974 6820 0a74 696d 6520 7365 7269 6573  ith .time series
+00000280: 2064 6174 612e 2054 6869 7320 6973 2065   data. This is e
+00000290: 7370 6563 6961 6c6c 7920 7472 7565 2c20  specially true, 
+000002a0: 6966 2073 7563 6820 6461 7461 206f 7269  if such data ori
+000002b0: 6769 6e61 7465 730a 6672 6f6d 2069 6e2d  ginates.from in-
+000002c0: 7369 7475 206d 6561 7375 7265 6d65 6e74  situ measurement
+000002d0: 7320 6f66 2065 6e76 6972 6f6e 6d65 6e74  s of environment
+000002e0: 616c 2070 726f 7065 7274 6965 732e 200a  al properties. .
+000002f0: 416c 6d6f 7374 2061 6c6c 2061 7070 6c69  Almost all appli
+00000300: 6361 7469 6f6e 732c 2068 6f77 6576 6572  cations, however
+00000310: 2c20 696d 706c 6963 696c 7920 7265 6c79  , implicily rely
+00000320: 206f 6e20 6461 7461 2c20 7468 6174 2063   on data, that c
+00000330: 6f6d 706c 6965 730a 7769 7468 2073 6f6d  omplies.with som
+00000340: 6520 6465 6669 6e69 7469 6f6e 206f 6620  e definition of 
+00000350: 2763 6f72 7265 6374 272e 200a 496e 206f  'correct'. .In o
+00000360: 7264 6572 2074 6f20 696e 6665 7220 7265  rder to infer re
+00000370: 6c69 6162 6c65 2064 6174 6120 7072 6f64  liable data prod
+00000380: 7563 7473 2061 6e64 2074 6f6f 6c73 2c20  ucts and tools, 
+00000390: 7468 6572 6520 6973 206e 6f20 616c 7465  there is no alte
+000003a0: 726e 6174 6976 650a 746f 2071 7561 6c69  rnative.to quali
+000003b0: 7479 2063 6f6e 7472 6f6c 2e20 5361 5143  ty control. SaQC
+000003c0: 2070 726f 7669 6465 7320 616c 6c20 7468   provides all th
+000003d0: 6520 6275 696c 6469 6e67 2062 6c6f 636b  e building block
+000003e0: 7320 746f 2063 6f6d 666f 7274 6162 6c79  s to comfortably
+000003f0: 0a62 7269 6467 6520 7468 6520 6761 7020  .bridge the gap 
+00000400: 6265 7477 6565 6e20 2775 7375 616c 6c79  between 'usually
+00000410: 2066 6175 6c74 7927 2061 6e64 2027 6578   faulty' and 'ex
+00000420: 7065 6374 6564 2074 6f20 6265 2063 6f72  pected to be cor
+00000430: 7265 6374 6564 2720 696e 200a 6120 6163  rected' in .a ac
+00000440: 6365 7373 6962 6c65 2c20 636f 6e73 6973  cessible, consis
+00000450: 7465 6e74 2c20 6f62 6a65 6374 6976 6520  tent, objective 
+00000460: 616e 6420 7265 7072 6f64 7563 6962 6c65  and reproducible
+00000470: 2077 6179 2e0a 0a46 6f72 2061 2028 636f   way...For a (co
+00000480: 6e74 696e 6f75 736c 7920 696d 7072 6f76  ntinously improv
+00000490: 696e 6729 206f 7665 7276 6965 7720 6f66  ing) overview of
+000004a0: 2066 6561 7475 7265 732c 2074 7970 6963   features, typic
+000004b0: 616c 2075 7361 6765 2070 6174 7465 726e  al usage pattern
+000004c0: 732c 0a74 6865 2073 7065 6369 6669 6320  s,.the specific 
+000004d0: 7379 7374 656d 2063 6f6d 706f 6e65 6e74  system component
+000004e0: 7320 616e 6420 686f 7720 746f 2063 7573  s and how to cus
+000004f0: 746f 6d69 7a65 2060 5361 5143 6020 746f  tomize `SaQC` to
+00000500: 2079 6f75 7220 7370 6563 6966 6963 0a6e   your specific.n
+00000510: 6565 6473 2c20 706c 6561 7365 2072 6566  eeds, please ref
+00000520: 6572 2074 6f20 6f75 720a 5b6f 6e6c 696e  er to our.[onlin
+00000530: 6520 646f 6375 6d65 6e74 6174 696f 6e5d  e documentation]
+00000540: 2868 7474 7073 3a2f 2f72 646d 2d73 6f66  (https://rdm-sof
+00000550: 7477 6172 652e 7061 6765 732e 7566 7a2e  tware.pages.ufz.
+00000560: 6465 2f73 6171 632f 696e 6465 782e 6874  de/saqc/index.ht
+00000570: 6d6c 292e 0a0a 0a23 2320 496e 7374 616c  ml)....## Instal
+00000580: 6c61 7469 6f6e 0a0a 5361 5143 2069 7320  lation..SaQC is 
+00000590: 6176 6169 6c61 626c 6520 6f6e 2074 6865  available on the
+000005a0: 2050 7974 686f 6e20 5061 636b 6167 6520   Python Package 
+000005b0: 496e 6465 7820 285b 5079 5049 5d28 6874  Index ([PyPI](ht
+000005c0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f29  tps://pypi.org/)
+000005d0: 2920 616e 640a 6361 6e20 6265 2069 6e73  ) and.can be ins
+000005e0: 7461 6c6c 6564 2075 7369 6e67 205b 7069  talled using [pi
+000005f0: 705d 2868 7474 7073 3a2f 2f70 6970 2e70  p](https://pip.p
+00000600: 7970 612e 696f 2f65 6e2f 7374 6162 6c65  ypa.io/en/stable
+00000610: 2f29 3a0a 6060 6073 680a 7079 7468 6f6e  /):.```sh.python
+00000620: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
+00000630: 7361 7163 0a60 6060 0a46 6f72 2061 206d  saqc.```.For a m
+00000640: 6f72 6520 6465 7461 696c 6564 2069 6e73  ore detailed ins
+00000650: 7461 6c6c 696f 6e20 6775 6964 652c 2073  tallion guide, s
+00000660: 6565 2074 6865 205b 696e 7374 616c 6c61  ee the [installa
+00000670: 7469 6f6e 2067 7569 6465 5d28 6874 7470  tion guide](http
+00000680: 733a 2f2f 7264 6d2d 736f 6674 7761 7265  s://rdm-software
+00000690: 2e70 6167 6573 2e75 667a 2e64 652f 7361  .pages.ufz.de/sa
+000006a0: 7163 2f67 6574 7469 6e67 7374 6172 7465  qc/gettingstarte
+000006b0: 642f 496e 7374 616c 6c61 7469 6f6e 4775  d/InstallationGu
+000006c0: 6964 652e 6874 6d6c 292e 0a0a 2323 2055  ide.html)...## U
+000006d0: 7361 6765 0a0a 6053 6151 4360 2069 7320  sage..`SaQC` is 
+000006e0: 626f 7468 2c20 6120 636f 6d6d 616e 6420  both, a command 
+000006f0: 6c69 6e65 2061 7070 6c69 6361 7469 6f6e  line application
+00000700: 2063 6f6e 7472 6f6c 6c65 6420 6279 2061   controlled by a
+00000710: 2074 6578 7420 6261 7365 6420 636f 6e66   text based conf
+00000720: 6967 7572 6174 696f 6e0a 616e 6420 6120  iguration.and a 
+00000730: 7079 7468 6f6e 206d 6f64 756c 6520 7769  python module wi
+00000740: 7468 2061 2073 696d 706c 6520 4150 492e  th a simple API.
+00000750: 0a0a 2323 2320 5361 5143 2061 7320 6120  ..### SaQC as a 
+00000760: 636f 6d6d 616e 6420 6c69 6e65 2061 7070  command line app
+00000770: 6c69 6361 7469 6f6e 0a54 6865 2063 6f6d  lication.The com
+00000780: 6d61 6e64 206c 696e 6520 6170 706c 6963  mand line applic
+00000790: 6174 696f 6e20 6973 2063 6f6e 7472 6f6c  ation is control
+000007a0: 6c65 6420 6279 2061 2073 656d 6963 6f6c  led by a semicol
+000007b0: 6f6e 2d73 6570 6172 6174 6564 2074 6578  on-separated tex
+000007c0: 740a 6669 6c65 206c 6973 7469 6e67 2074  t.file listing t
+000007d0: 6865 2076 6172 6961 626c 6573 2069 6e20  he variables in 
+000007e0: 7468 6520 6461 7461 7365 7420 616e 6420  the dataset and 
+000007f0: 7468 6520 726f 7574 696e 6573 2074 6f20  the routines to 
+00000800: 696e 7370 6563 742c 0a71 7561 6c69 7479  inspect,.quality
+00000810: 2063 6f6e 7472 6f6c 2061 6e64 2f6f 7220   control and/or 
+00000820: 7072 6f63 6573 7320 7468 656d 2e20 5468  process them. Th
+00000830: 6520 636f 6e74 656e 7420 6f66 2073 7563  e content of suc
+00000840: 6820 6120 636f 6e66 6967 7572 6174 696f  h a configuratio
+00000850: 6e0a 636f 756c 6420 6c6f 6f6b 206c 696b  n.could look lik
+00000860: 6520 5b74 6869 735d 2868 7474 7073 3a2f  e [this](https:/
+00000870: 2f67 6974 2e75 667a 2e64 652f 7264 6d2d  /git.ufz.de/rdm-
+00000880: 736f 6674 7761 7265 2f73 6171 632f 7261  software/saqc/ra
+00000890: 772f 6465 7665 6c6f 702f 646f 6373 2f72  w/develop/docs/r
+000008a0: 6573 6f75 7263 6573 2f64 6174 612f 636f  esources/data/co
+000008b0: 6e66 6967 2e63 7376 293a 0a0a 6060 600a  nfig.csv):..```.
+000008c0: 7661 726e 616d 6520 2020 203b 2074 6573  varname    ; tes
+000008d0: 740a 232d 2d2d 2d2d 2d2d 2d2d 2d3b 202d  t.#----------; -
+000008e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000920: 2d2d 2d2d 0a53 4d32 2020 2020 2020 2020  ----.SM2        
+00000930: 3b20 7368 6966 7428 6672 6571 3d22 3135  ; shift(freq="15
+00000940: 4d69 6e22 290a 2753 4d28 317c 3229 2b27  Min").'SM(1|2)+'
+00000950: 203b 2066 6c61 674d 6973 7369 6e67 2829   ; flagMissing()
+00000960: 0a53 4d31 2020 2020 2020 2020 3b20 666c  .SM1        ; fl
+00000970: 6167 5261 6e67 6528 6d69 6e3d 3130 2c20  agRange(min=10, 
+00000980: 6d61 783d 3630 290a 534d 3220 2020 2020  max=60).SM2     
+00000990: 2020 203b 2066 6c61 6752 616e 6765 286d     ; flagRange(m
+000009a0: 696e 3d31 302c 206d 6178 3d34 3029 0a53  in=10, max=40).S
+000009b0: 4d32 2020 2020 2020 2020 3b20 666c 6167  M2        ; flag
+000009c0: 4d41 4428 7769 6e64 6f77 3d22 3330 6422  MAD(window="30d"
+000009d0: 2c20 7a3d 332e 3529 0a44 756d 6d79 2020  , z=3.5).Dummy  
+000009e0: 2020 2020 3b20 666c 6167 4765 6e65 7269      ; flagGeneri
+000009f0: 6328 6669 656c 643d 5b22 534d 3122 2c20  c(field=["SM1", 
+00000a00: 2253 4d32 225d 2c20 6675 6e63 3d28 6973  "SM2"], func=(is
+00000a10: 666c 6167 6765 6428 7829 207c 2069 7366  flagged(x) | isf
+00000a20: 6c61 6767 6564 2879 2929 290a 6060 600a  lagged(y))).```.
+00000a30: 0a41 7320 736f 6f6e 2061 7320 7468 6520  .As soon as the 
+00000a40: 6261 7369 6320 696e 7075 7473 2c20 6461  basic inputs, da
+00000a50: 7461 7365 7420 616e 6420 636f 6e66 6967  taset and config
+00000a60: 7572 6174 696f 6e20 6669 6c65 2c20 6172  uration file, ar
+00000a70: 650a 7072 6570 6172 6564 2c20 7275 6e20  e.prepared, run 
+00000a80: 6053 6151 4360 3a0a 6060 6073 680a 7361  `SaQC`:.```sh.sa
+00000a90: 7163 205c 0a20 2020 202d 2d63 6f6e 6669  qc \.    --confi
+00000aa0: 6720 5041 5448 5f54 4f5f 434f 4e46 4947  g PATH_TO_CONFIG
+00000ab0: 5552 4154 494f 4e20 5c0a 2020 2020 2d2d  URATION \.    --
+00000ac0: 6461 7461 2050 4154 485f 544f 5f44 4154  data PATH_TO_DAT
+00000ad0: 4120 5c0a 2020 2020 2d2d 6f75 7466 696c  A \.    --outfil
+00000ae0: 6520 5041 5448 5f54 4f5f 4f55 5450 5554  e PATH_TO_OUTPUT
+00000af0: 0a60 6060 0a0a 4120 6675 6c6c 2060 5361  .```..A full `Sa
+00000b00: 5143 6020 7275 6e20 6167 6169 6e73 7420  QC` run against 
+00000b10: 7072 6f76 6964 6564 2065 7861 6d70 6c65  provided example
+00000b20: 2064 6174 6120 6361 6e20 6265 2069 6e76   data can be inv
+00000b30: 6f6b 6564 2077 6974 683a 0a60 6060 7368  oked with:.```sh
+00000b40: 0a73 6171 6320 5c0a 2020 2020 2d2d 636f  .saqc \.    --co
+00000b50: 6e66 6967 2068 7474 7073 3a2f 2f67 6974  nfig https://git
+00000b60: 2e75 667a 2e64 652f 7264 6d2d 736f 6674  .ufz.de/rdm-soft
+00000b70: 7761 7265 2f73 6171 632f 7261 772f 6465  ware/saqc/raw/de
+00000b80: 7665 6c6f 702f 646f 6373 2f72 6573 6f75  velop/docs/resou
+00000b90: 7263 6573 2f64 6174 612f 636f 6e66 6967  rces/data/config
+00000ba0: 2e63 7376 205c 0a20 2020 202d 2d64 6174  .csv \.    --dat
+00000bb0: 6120 6874 7470 733a 2f2f 6769 742e 7566  a https://git.uf
+00000bc0: 7a2e 6465 2f72 646d 2d73 6f66 7477 6172  z.de/rdm-softwar
+00000bd0: 652f 7361 7163 2f72 6177 2f64 6576 656c  e/saqc/raw/devel
+00000be0: 6f70 2f64 6f63 732f 7265 736f 7572 6365  op/docs/resource
+00000bf0: 732f 6461 7461 2f64 6174 612e 6373 7620  s/data/data.csv 
+00000c00: 5c0a 2020 2020 2d2d 6f75 7466 696c 6520  \.    --outfile 
+00000c10: 7361 7163 5f74 6573 742e 6373 760a 6060  saqc_test.csv.``
+00000c20: 600a 0a23 2323 2053 6151 4320 6173 2061  `..### SaQC as a
+00000c30: 2070 7974 686f 6e20 6d6f 6475 6c65 0a0a   python module..
+00000c40: 5468 6520 666f 6c6c 6f77 696e 6720 736e  The following sn
+00000c50: 6970 7065 7420 696d 706c 656d 656e 7473  ippet implements
+00000c60: 2074 6865 2073 616d 6520 636f 6e66 6967   the same config
+00000c70: 7572 6174 696f 6e20 6769 7665 6e20 6162  uration given ab
+00000c80: 6f76 6520 7468 726f 7567 680a 7468 6520  ove through.the 
+00000c90: 5079 7468 6f6e 2d41 5049 3a0a 0a60 6060  Python-API:..```
+00000ca0: 7079 7468 6f6e 0a69 6d70 6f72 7420 7061  python.import pa
+00000cb0: 6e64 6173 2061 7320 7064 0a66 726f 6d20  ndas as pd.from 
+00000cc0: 7361 7163 2069 6d70 6f72 7420 5361 5143  saqc import SaQC
+00000cd0: 0a0a 6461 7461 203d 2070 642e 7265 6164  ..data = pd.read
+00000ce0: 5f63 7376 280a 2020 2020 2268 7474 7073  _csv(.    "https
+00000cf0: 3a2f 2f67 6974 2e75 667a 2e64 652f 7264  ://git.ufz.de/rd
+00000d00: 6d2d 736f 6674 7761 7265 2f73 6171 632f  m-software/saqc/
+00000d10: 7261 772f 6465 7665 6c6f 702f 646f 6373  raw/develop/docs
+00000d20: 2f72 6573 6f75 7263 6573 2f64 6174 612f  /resources/data/
+00000d30: 6461 7461 2e63 7376 222c 0a20 2020 2069  data.csv",.    i
+00000d40: 6e64 6578 5f63 6f6c 3d30 2c20 7061 7273  ndex_col=0, pars
+00000d50: 655f 6461 7465 733d 5472 7565 2c0a 290a  e_dates=True,.).
+00000d60: 0a73 6171 6320 3d20 5361 5143 2864 6174  .saqc = SaQC(dat
+00000d70: 613d 6461 7461 290a 7361 7163 203d 2028  a=data).saqc = (
+00000d80: 7361 7163 0a20 2020 2020 2020 202e 7368  saqc.        .sh
+00000d90: 6966 7428 2253 4d32 222c 2066 7265 713d  ift("SM2", freq=
+00000da0: 2231 354d 696e 2229 0a20 2020 2020 2020  "15Min").       
+00000db0: 202e 666c 6167 4d69 7373 696e 6728 2253   .flagMissing("S
+00000dc0: 4d28 317c 3229 2b22 2c20 7265 6765 783d  M(1|2)+", regex=
+00000dd0: 5472 7565 290a 2020 2020 2020 2020 2e66  True).        .f
+00000de0: 6c61 6752 616e 6765 2822 534d 3122 2c20  lagRange("SM1", 
+00000df0: 6d69 6e3d 3130 2c20 6d61 783d 3630 290a  min=10, max=60).
+00000e00: 2020 2020 2020 2020 2e66 6c61 6752 616e          .flagRan
+00000e10: 6765 2822 534d 3222 2c20 6d69 6e3d 3130  ge("SM2", min=10
+00000e20: 2c20 6d61 783d 3430 290a 2020 2020 2020  , max=40).      
+00000e30: 2020 2e66 6c61 674d 4144 2822 534d 3222    .flagMAD("SM2"
+00000e40: 2c20 7769 6e64 6f77 3d22 3330 6422 2c20  , window="30d", 
+00000e50: 7a3d 332e 3529 0a20 2020 2020 2020 202e  z=3.5).        .
+00000e60: 666c 6167 4765 6e65 7269 6328 6669 656c  flagGeneric(fiel
+00000e70: 643d 5b22 534d 3122 2c20 2253 4d32 225d  d=["SM1", "SM2"]
+00000e80: 2c20 7461 7267 6574 3d22 4475 6d6d 7922  , target="Dummy"
+00000e90: 2c20 6675 6e63 3d6c 616d 6264 6120 782c  , func=lambda x,
+00000ea0: 2079 3a20 2869 7366 6c61 6767 6564 2878   y: (isflagged(x
+00000eb0: 2920 7c20 6973 666c 6167 6765 6428 7929  ) | isflagged(y)
+00000ec0: 2929 290a 6060 600a 0a41 206d 6f72 6520  ))).```..A more 
+00000ed0: 6465 7461 696c 6564 2064 6573 6372 6970  detailed descrip
+00000ee0: 7469 6f6e 206f 6620 7468 6520 5079 7468  tion of the Pyth
+00000ef0: 6f6e 2041 5049 2069 7320 6176 6169 6c61  on API is availa
+00000f00: 626c 6520 696e 2074 6865 200a 5b72 6573  ble in the .[res
+00000f10: 7065 6374 6976 6520 7365 6374 696f 6e5d  pective section]
+00000f20: 2868 7474 7073 3a2f 2f72 646d 2d73 6f66  (https://rdm-sof
+00000f30: 7477 6172 652e 7061 6765 732e 7566 7a2e  tware.pages.ufz.
+00000f40: 6465 2f73 6171 632f 6765 7474 696e 6773  de/saqc/gettings
+00000f50: 7461 7274 6564 2f54 7574 6f72 6961 6c41  tarted/TutorialA
+00000f60: 5049 2e68 746d 6c29 0a6f 6620 7468 6520  PI.html).of the 
+00000f70: 646f 6375 6d65 6e74 6174 696f 6e2e 0a0a  documentation...
+00000f80: 2323 2043 6861 6e67 656c 6f67 0a41 6c6c  ## Changelog.All
+00000f90: 206e 6f74 6162 6c65 2063 6861 6e67 6573   notable changes
+00000fa0: 2074 6f20 7468 6973 2070 726f 6a65 6374   to this project
+00000fb0: 2077 696c 6c20 6265 2064 6f63 756d 656e   will be documen
+00000fc0: 7465 6420 696e 205b 4348 414e 4745 4c4f  ted in [CHANGELO
+00000fd0: 472e 6d64 5d28 4348 414e 4745 4c4f 472e  G.md](CHANGELOG.
+00000fe0: 6d64 292e 0a0a 2323 2047 6574 2069 6e76  md)...## Get inv
+00000ff0: 6f6c 7665 640a 0a23 2323 2043 6f6e 7472  olved..### Contr
+00001000: 6962 7574 696e 670a 596f 7520 666f 756e  ibuting.You foun
+00001010: 6420 6120 6275 6720 6f72 2079 6f75 2077  d a bug or you w
+00001020: 616e 7420 746f 2073 7567 6765 7374 2073  ant to suggest s
+00001030: 6f6d 6520 636f 6f6c 2066 6561 7475 7265  ome cool feature
+00001040: 733f 2050 6c65 6173 6520 7265 6665 7220  s? Please refer 
+00001050: 746f 206f 7572 205b 636f 6e74 7269 6275  to our [contribu
+00001060: 7469 6e67 2067 7569 6465 6c69 6e65 735d  ting guidelines]
+00001070: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
+00001080: 2920 746f 2073 6565 2068 6f77 2079 6f75  ) to see how you
+00001090: 2063 616e 2063 6f6e 7472 6962 7574 6520   can contribute 
+000010a0: 746f 2053 6151 432e 0a0a 2323 2320 5573  to SaQC...### Us
+000010b0: 6572 2073 7570 706f 7274 0a49 6620 796f  er support.If yo
+000010c0: 7520 6e65 6564 2068 656c 7020 6f72 2068  u need help or h
+000010d0: 6176 6520 6120 7175 6573 7469 6f6e 2c20  ave a question, 
+000010e0: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
+000010f0: 5361 5143 2075 7365 7220 7375 7070 6f72  SaQC user suppor
+00001100: 7420 6d61 696c 696e 6720 6c69 7374 3a20  t mailing list: 
+00001110: 5b73 6171 632d 7375 7070 6f72 7440 7566  [saqc-support@uf
+00001120: 7a2e 6465 5d28 6d61 696c 746f 3a73 6171  z.de](mailto:saq
+00001130: 632d 7375 7070 6f72 7440 7566 7a2e 6465  c-support@ufz.de
+00001140: 290a 0a23 2320 436f 7079 7269 6768 7420  )..## Copyright 
+00001150: 616e 6420 4c69 6365 6e73 650a 436f 7079  and License.Copy
+00001160: 7269 6768 7428 6329 2032 3032 312c 205b  right(c) 2021, [
+00001170: 4865 6c6d 686f 6c74 7a2d 5a65 6e74 7275  Helmholtz-Zentru
+00001180: 6d20 66c3 bc72 2055 6d77 656c 7466 6f72  m f..r Umweltfor
+00001190: 7363 6875 6e67 2047 6d62 4820 2d2d 2055  schung GmbH -- U
+000011a0: 465a 5d28 6874 7470 733a 2f2f 7777 772e  FZ](https://www.
+000011b0: 7566 7a2e 6465 292e 2041 6c6c 2072 6967  ufz.de). All rig
+000011c0: 6874 7320 7265 7365 7276 6564 2e0a 0a2d  hts reserved...-
+000011d0: 2044 6f63 756d 656e 7461 7469 6f6e 3a20   Documentation: 
+000011e0: 5b43 7265 6174 6976 6520 436f 6d6d 6f6e  [Creative Common
+000011f0: 7320 4174 7472 6962 7574 696f 6e20 342e  s Attribution 4.
+00001200: 3020 496e 7465 726e 6174 696f 6e61 6c5d  0 International]
+00001210: 2868 7474 7073 3a2f 2f63 7265 6174 6976  (https://creativ
+00001220: 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963  ecommons.org/lic
+00001230: 656e 7365 732f 6279 2f34 2e30 2f29 203c  enses/by/4.0/) <
+00001240: 6120 7265 6c3d 226c 6963 656e 7365 2220  a rel="license" 
+00001250: 6872 6566 3d22 6874 7470 3a2f 2f63 7265  href="http://cre
+00001260: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
+00001270: 2f6c 6963 656e 7365 732f 6279 2f34 2e30  /licenses/by/4.0
+00001280: 2f22 3e3c 696d 6720 616c 743d 2243 7265  /"><img alt="Cre
+00001290: 6174 6976 6520 436f 6d6d 6f6e 7320 4c69  ative Commons Li
+000012a0: 6365 6e73 6522 2073 7479 6c65 3d22 626f  cense" style="bo
+000012b0: 7264 6572 2d77 6964 7468 3a30 2220 7372  rder-width:0" sr
+000012c0: 633d 2268 7474 7073 3a2f 2f69 2e63 7265  c="https://i.cre
+000012d0: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
+000012e0: 2f6c 2f62 792f 342e 302f 3830 7831 352e  /l/by/4.0/80x15.
+000012f0: 706e 6722 202f 3e3c 2f61 3e0a 2d20 536f  png" /></a>.- So
+00001300: 7572 6365 2063 6f64 653a 205b 474e 5520  urce code: [GNU 
+00001310: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
+00001320: 6963 656e 7365 2033 5d28 6874 7470 733a  icense 3](https:
+00001330: 2f2f 7777 772e 676e 752e 6f72 672f 6c69  //www.gnu.org/li
+00001340: 6365 6e73 6573 2f67 706c 2d33 2e30 2e68  censes/gpl-3.0.h
+00001350: 746d 6c29 0a0a 466f 7220 6675 6c6c 2064  tml)..For full d
+00001360: 6574 6169 6c73 2c20 7365 6520 5b4c 4943  etails, see [LIC
+00001370: 454e 5345 5d28 4c49 4345 4e53 452e 6d64  ENSE](LICENSE.md
+00001380: 292e 0a0a 2323 2041 636b 6e6f 776c 6564  )...## Acknowled
+00001390: 6765 6d65 6e74 730a 2e2e 2e0a 0a23 2320  gements......## 
+000013a0: 5075 626c 6963 6174 696f 6e73 0a63 6f6d  Publications.com
+000013b0: 696e 6720 736f 6f6e 2e2e 2e0a 0a23 2320  ing soon.....## 
+000013c0: 486f 7720 746f 2063 6974 6520 5361 5143  How to cite SaQC
+000013d0: 0a49 6620 5361 5143 2069 7320 6164 7661  .If SaQC is adva
+000013e0: 6e63 696e 6720 796f 7572 2072 6573 6561  ncing your resea
+000013f0: 7263 682c 2070 6c65 6173 6520 6369 7465  rch, please cite
+00001400: 2061 733a 0a0a 3e20 5363 68c3 a466 6572   as:..> Sch..fer
+00001410: 2c20 4461 7669 642c 2050 616c 6d2c 2042  , David, Palm, B
+00001420: 6572 742c 204c c3bc 6e65 6e73 6368 6c6f  ert, L..nenschlo
+00001430: c39f 2c20 5065 7465 722c 2053 6368 6d69  .., Peter, Schmi
+00001440: 6474 2c20 4c65 6e6e 6172 742c 2026 2042  dt, Lennart, & B
+00001450: 756d 6265 7267 6572 2c20 4a61 6e2e 2028  umberger, Jan. (
+00001460: 3230 3233 292e 2053 7973 7465 6d20 666f  2023). System fo
+00001470: 7220 6175 746f 6d61 7465 6420 5175 616c  r automated Qual
+00001480: 6974 7920 436f 6e74 726f 6c20 2d20 5361  ity Control - Sa
+00001490: 5143 2028 322e 332e 3029 2e20 5a65 6e6f  QC (2.3.0). Zeno
+000014a0: 646f 2e20 6874 7470 733a 2f2f 646f 692e  do. https://doi.
+000014b0: 6f72 672f 3130 2e35 3238 312f 7a65 6e6f  org/10.5281/zeno
+000014c0: 646f 2e35 3838 3835 3437 0a0a 2d2d 2d2d  do.5888547..----
+000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a3c  -------------..<
+000014e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000014f0: 7777 772e 7566 7a2e 6465 2f69 6e64 6578  www.ufz.de/index
+00001500: 2e70 6870 3f65 6e3d 3333 3537 3322 3e0a  .php?en=33573">.
+00001510: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00001520: 7470 733a 2f2f 6769 742e 7566 7a2e 6465  tps://git.ufz.de
+00001530: 2f72 646d 2d73 6f66 7477 6172 652f 7361  /rdm-software/sa
+00001540: 7163 2f72 6177 2f64 6576 656c 6f70 2f64  qc/raw/develop/d
+00001550: 6f63 732f 7265 736f 7572 6365 732f 696d  ocs/resources/im
+00001560: 6167 6573 2f72 6570 7265 7365 6e74 6174  ages/representat
+00001570: 6976 652f 5546 5a4c 6f67 6f2e 706e 6722  ive/UFZLogo.png"
+00001580: 2077 6964 7468 3d22 3430 3022 2f3e 0a3c   width="400"/>.<
+00001590: 2f61 3e0a 0a3c 6120 6872 6566 3d22 6874  /a>..<a href="ht
+000015a0: 7470 733a 2f2f 7777 772e 7566 7a2e 6465  tps://www.ufz.de
+000015b0: 2f69 6e64 6578 2e70 6870 3f65 6e3d 3435  /index.php?en=45
+000015c0: 3334 3822 3e0a 2020 2020 3c69 6d67 2073  348">.    <img s
+000015d0: 7263 3d22 6874 7470 733a 2f2f 6769 742e  rc="https://git.
+000015e0: 7566 7a2e 6465 2f72 646d 2d73 6f66 7477  ufz.de/rdm-softw
+000015f0: 6172 652f 7361 7163 2f72 6177 2f64 6576  are/saqc/raw/dev
+00001600: 656c 6f70 2f64 6f63 732f 7265 736f 7572  elop/docs/resour
+00001610: 6365 732f 696d 6167 6573 2f72 6570 7265  ces/images/repre
+00001620: 7365 6e74 6174 6976 652f 5244 4d4c 6f67  sentative/RDMLog
+00001630: 6f2e 706e 6722 2061 6c69 676e 3d22 7269  o.png" align="ri
+00001640: 6768 7422 2077 6964 7468 3d22 3232 3022  ght" width="220"
+00001650: 2f3e 0a3c 2f61 3e0a                      />.</a>.
```

### Comparing `saqc-2.3/dios/dios/indexer.py` & `saqc-2.4.0/saqc/core/history.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,493 +1,612 @@
+#!/usr/bin/env python
+
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
+from __future__ import annotations
+
+import copy as _copy
+from typing import Any, Callable, Dict, List, Tuple
+
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_categorical_dtype, is_float_dtype
 
-from . import pandas_bridge as pdextra
-from .base import _DiosBase, _is_bool_dios_like, _is_dios_like
-
+from saqc import UNFLAGGED
 
-class _Indexer:
-    def __init__(self, obj: _DiosBase):
-        self.obj = obj
-        self._data = obj._data
 
-    def _unpack_key(self, key):
+class History:
+    """
+    Saqc internal storage for the history of a (single) flags column.
 
-        key = list(key) if pdextra.is_iterator(key) else key
+    The flag-history (FH) stores the history of a flags column. Each time
+    ``append`` is called a new column is appended to the FH. The column
+    names are increasing integers starting with 0. After initialisation
+    the FH is empty and has no columns at all.
 
-        if isinstance(key, tuple):
-            if len(key) > 2:
-                raise KeyError("To many indexers")
-            rowkey, colkey = key
-        else:
-            rowkey, colkey = key, slice(None)
+    To get the latest flags, that are currently stored in the FH, we provide
+    a ``squeeze()`` method.
 
-        if isinstance(rowkey, tuple) or isinstance(colkey, tuple):
-            raise KeyError(f"{key}. tuples are not allowed.")
+    For more details and a detailed discussion, why this is needed, how this
+    works and possible other implementations, see #GL143 [1].
 
-        rowkey = list(rowkey) if pdextra.is_iterator(rowkey) else rowkey
-        colkey = list(colkey) if pdextra.is_iterator(colkey) else colkey
-        return rowkey, colkey
+    [1] https://git.ufz.de/rdm-software/saqc/-/issues/143
 
-    def _set_value_muli_column(self, rowkey, colkey, value, xloc="loc"):
-        """set value helper for loc and iloc"""
+    Parameters
+    ----------
+    index: pd.Index
+        A index that fit the flags to be insert.
 
-        data = getattr(self._data, xloc)[colkey]
+    See Also
+    --------
+    createHistoryFromData: function to create History from existing data
+    """
 
-        hashable_rkey = pdextra.is_hashable(rowkey)
-        dioslike_value = False
-        iter_value = False
+    def __init__(self, index: pd.Index | None):
+        self._hist = pd.DataFrame(index=index)
+        self._meta = []
+
+    @property
+    def hist(self):
+        return self._hist.astype(float, copy=True)
+
+    @hist.setter
+    def hist(self, value: pd.DataFrame) -> None:
+        self._validateHist(value)
+        if len(value.columns) != len(self._meta):
+            raise ValueError(
+                "passed history does not match existing meta. "
+                "To use a new `hist` with new `meta` use "
+                "'History.createFromData(new_hist, new_meta)'"
+            )
+        self._hist = value.astype("category", copy=True)
 
-        if _is_dios_like(value):
-            dioslike_value = True
-            if hashable_rkey:
-                raise ValueError(f"Incompatible indexer with DictOfSeries")
+    @property
+    def meta(self) -> list[dict[str, Any]]:
+        return list(self._meta)
+
+    @meta.setter
+    def meta(self, value: list[dict[str, Any]]) -> None:
+        self._validateMetaList(value, self._hist)
+        self._meta = _copy.deepcopy(value)
 
-        elif pdextra.is_list_like(value):
-            value = value.values if isinstance(value, pd.Series) else value
-            iter_value = True
-            if len(value) != len(data):
-                raise ValueError(
-                    f"shape mismatch: value array of shape (.., {len(value)}) could "
-                    f"not be broadcast to indexing result of shape (.., {len(data)})"
-                )
-        c = "?"
-        try:
-            for i, c in enumerate(data.index):
-                dat = data.at[c]
-                dat_xloc = getattr(dat, xloc)
-
-                if dioslike_value:
-                    # set to empty series fail; emptySer.loc[:] = [2,1]
-                    # len(scalar) -> would fail, but cannot happen,
-                    # because dioslike+hashable, already was checked
-                    if len(dat_xloc[rowkey]) == 0:
-                        continue
-
-                # unpack the value if necessary
-                if iter_value:
-                    val = value[i]
-                elif dioslike_value:
-                    val = value[c] if c in value else np.nan
-                else:
-                    val = value
+    @property
+    def index(self) -> pd.Index:
+        """
+        The index of FH.
 
-                dat_xloc[rowkey] = val
+        The index is the same for all columns.
 
-        except Exception as e:
-            raise type(e)(f"failed for column {c}: " + str(e)) from e
+        Notes
+        -----
+        The index should always be equal to the flags series,
+        the FH is associated with. If this is messed up
+        something went wrong in saqc internals or in a user-
+        defined test.
+
+        Returns
+        -------
+        index : pd.Index
+        """
+        return self._hist.index
 
+    @property
+    def columns(self) -> pd.Index:
+        """
+        Columns of the FH.
 
-# #############################################################################
+        The columns are always continuously
+        increasing integers, starting from 0.
 
+        Returns
+        -------
+        columns : pd.Index
+        """
+        return self._hist.columns
 
-class _LocIndexer(_Indexer):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    @property
+    def empty(self) -> bool:
+        """
+        Indicator whether History is empty.
 
-    def __getitem__(self, key):
+        True if History is entirely empty (no items).
 
-        rowkey, colkey = self._unpack_key(key)
-        if _is_dios_like(rowkey) or _is_dios_like(colkey):
-            raise ValueError("Could not index with multidimensional key")
+        Returns
+        -------
+        bool
+            If History is empty, return True, if not return False.
+        """
+        return len(self) == 0
 
-        # simple optimisation
-        if pdextra.is_null_slice(rowkey) and pdextra.is_null_slice(colkey):
-            return self.obj.copy()
+    def _insert(self, s: pd.Series, pos: int) -> History:
+        """
+        Insert data at an arbitrary position in the FH.
 
-        data = self._data.loc[colkey].copy()
+        No validation of series is done here.
 
-        # .loc[any, scalar] -> (a single) series
-        # .loc[scalar, scalar] -> (a single) value
-        if pdextra.is_hashable(colkey):
-            new = data.loc[rowkey]
+        Parameters
+        ----------
+        s : pd.Series
+            the series to insert
 
-        # .loc[any, non-scalar]
-        else:
-            k = "?"
-            try:
+        pos : int
+            the position to insert
 
-                for k in data.index:
-                    data.at[k] = data.at[k].loc[rowkey]
+        Returns
+        -------
+        History
+        """
+        # Note:
+        # all following code must handle a passed empty series
 
-            except Exception as e:
-                raise type(e)(f"failed for column {k}: " + str(e)) from e
+        # ensure continuous increasing columns
+        assert 0 <= pos <= len(self.columns)
+        self._hist[pos] = s.astype("category")
+        return self
 
-            # .loc[scalar, non-scalar] -> column-indexed series
-            if pdextra.is_hashable(rowkey):
-                new = data
-
-            # .loc[non-scalar, non-scalar] -> dios
-            else:
-                new = self.obj.copy_empty(columns=False)
-                new._data = data
+    def append(self, value: pd.Series | History, meta: dict | None = None) -> History:
+        """
+        Create a new FH column and insert given pd.Series to it.
 
-        return new
+        Parameters
+        ----------
+        value : pd.Series or History
+            The data to append. Must have dtype float and the index must
+            match the index of the History.
+
+        meta : dict, default None
+            metadata dictionary to store with the series. Ignored if ``value`` is of
+             type History. None defaults to a empty dictionary.
+
+        Returns
+        -------
+        history with appended series
+
+        Raises
+        ------
+        TypeError: if value is not pd.Series
+        ValueError: on index miss-match or wrong dtype
+        """
+        if isinstance(value, History):
+            return self._appendHistory(value)
 
-    def __setitem__(self, key, value):
+        if not isinstance(value, pd.Series):
+            raise TypeError("'value' is not a pd.Series")
 
-        rowkey, colkey = self._unpack_key(key)
-        if _is_dios_like(rowkey) or _is_dios_like(colkey):
-            raise ValueError("Cannot index with multi-dimensional key")
+        if meta is None:
+            meta = {}
+        elif not isinstance(meta, dict):
+            raise TypeError("'meta' must be of type None or dict")
+
+        val = self._validateValue(value)
+        if not val.index.equals(self.index):
+            raise ValueError("Index does not match")
 
-        # .loc[any, scalar] - set on single column
-        if pdextra.is_hashable(colkey):
+        self._insert(val, pos=len(self))
+        self._meta.append(meta.copy())
+        return self
 
-            # .loc[dont-care, new-scalar] = val
-            if colkey not in self.obj.columns:
-                self.obj._insert(colkey, value)
+    def _appendHistory(self, value: History) -> History:
+        """
+        Append multiple columns of a history to self.
 
-            # .loc[any, scalar] = multi-dim
-            elif _is_dios_like(value) or pdextra.is_nested_list_like(value):
-                raise ValueError("Incompatible indexer with multi-dimensional value")
+        Parameters
+        ----------
+        value : History
+            Holding the columns to append
+
+        Returns
+        -------
+        History with appended columns.
+
+        Raises
+        ------
+        ValueError : If the index of the passed history does not match.
+
+        Notes
+        -----
+        This ignores the column names of the passed History.
+        """
+        self._validate(value._hist, value._meta)
+        if not value.index.equals(self.index):
+            raise ValueError("Index does not match")
+
+        # we copy shallow because we only want to set new columns
+        # the actual data copy happens in calls to astype
+        value_hist = value._hist.copy(deep=False)
+        value_meta = value._meta.copy()
+
+        # rename columns, to avoid ``pd.DataFrame.loc`` become confused
+        n = len(self.columns)
+        columns = pd.Index(range(n, n + len(value_hist.columns)))
+        value_hist.columns = columns
+
+        hist = self._hist.astype(float)
+        hist.loc[:, columns] = value_hist.astype(float)
+        self._hist = hist.astype("category")
+        self._meta += value_meta
+        return self
 
-            # .loc[any, scalar] = val
-            else:
-                self._data.at[colkey].loc[rowkey] = value
+    def squeeze(
+        self, raw: bool = False, start: int | None = None, end: int | None = None
+    ) -> pd.Series:
+        """
+        Reduce history to a series, by taking the last set value per row.
 
-        # .loc[any, non-scalar] = any
+        By passing `start` and/or `end` only a slice of the history is used.
+        This can be used to get the values of an earlier test. See the
+        Examples.
+
+        Parameters
+        ----------
+        raw : bool, default False
+            If True, 'unset' values are represented by `nan`,
+            otherwise, 'unset' values are represented by the
+            `UNFLAGGED` (`-inf`) constant
+
+        start : int, default None
+            The first history column to use (inclusive).
+
+        end : int, default None
+            The last history column to use (exclusive).
+
+        Returns
+        -------
+        pandas.Series
+
+        Examples
+        --------
+        >>> from saqc.core.history import History
+        >>> s0 = pd.Series([np.nan, np.nan, 99.])
+        >>> s1 = pd.Series([1., 1., np.nan])
+        >>> s2 = pd.Series([2., np.nan, 2.])
+        >>> h = History(pd.Index([0,1,2])).append(s0).append(s1).append(s2)
+        >>> h
+             0    1    2
+        0   nan  1.0  2.0
+        1   nan  1.0  nan
+        2  99.0  nan  2.0
+
+        Get current flags.
+
+        >>> h.squeeze()
+        0    2.0
+        1    1.0
+        2    2.0
+        dtype: float64
+
+        Get only the flags that the last function had set:
+
+        >>> h.squeeze(start=-1)
+        0    2.0
+        1   -inf
+        2    2.0
+        dtype: float64
+
+        Get the flags before the last function run:
+
+        >>> h.squeeze(end=-1)
+        0     1.0
+        1     1.0
+        2    99.0
+        dtype: float64
+
+        Get only the flags that the 2nd function had set:
+
+        >>> h.squeeze(start=1, end=2)
+        0    1.0
+        1    1.0
+        2   -inf
+        dtype: float64
+        """
+        hist = self._hist.iloc[:, slice(start, end)].astype(float)
+        if hist.empty:
+            result = pd.Series(data=np.nan, index=self._hist.index, dtype=float)
         else:
-            self._set_value_muli_column(rowkey, colkey, value, xloc="loc")
-
-
-# #############################################################################
-
-
-class _iLocIndexer(_Indexer):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def __getitem__(self, key):
-        rowkey, colkey = self._unpack_key(key)
-        if _is_dios_like(rowkey) or _is_dios_like(colkey):
-            raise ValueError("Cannot index with multidimensional key")
-
-        # simple optimisation
-        if pdextra.is_null_slice(rowkey) and pdextra.is_null_slice(colkey):
-            return self.obj.copy()
+            result = hist.ffill(axis=1).iloc[:, -1]
+        if not raw:
+            result = result.fillna(UNFLAGGED)
+        result.name = None
+        return result
+
+    def reindex(
+        self, index: pd.Index, fill_value_last: float = UNFLAGGED, copy: bool = True
+    ) -> History:
+        """
+        Reindex the History. Be careful this alters the past.
 
-        data = self._data.iloc[colkey].copy()
+        Parameters
+        ----------
+        index : pd.Index
+            the index to reindex to.
+
+        fill_value_last : float, default UNFLAGGED
+            value to fill nan's in the last column.
+            Defaults to 0 (UNFLAGGED).
+
+        copy : bool, default True
+            If False, alter the underlying history, otherwise return a copy.
+
+        Returns
+        -------
+        History
+        """
+        # Note: code must handle empty frames
+        out = self.copy() if copy else self
+        hist = out._hist.astype(float).reindex(index=index, copy=False)
+        hist.iloc[:, -1:] = hist.iloc[:, -1:].fillna(fill_value_last)
+        out._hist = hist.astype("category")
+        return out
+
+    def apply(
+        self,
+        index: pd.Index,
+        func: Callable,
+        func_kws: dict,
+        func_handle_df: bool = False,
+        copy: bool = True,
+    ) -> History:
+        """
+        Apply a function on each column in history.
 
-        # .iloc[any, int] -> single series
-        # .iloc[int, int] -> single value
-        if pdextra.is_integer(colkey):
-            new = data.iloc[rowkey]
+        The function must take a `pd.Series` as first arg, which is a column from
+        `hist`. If ``func_handle_df=True`` each functions take a ``pd.DataFrame``
+        as first argument, holding all columns at once.
+        Bear in mind:
+        - the functions mustn't alter the passed objects
+        - the functions are not allowed to add or remove columns
+        - the function must return same type as first argument
+        - the returned object must have same index as the passed ``index`` to ``apply`` as first argument
+
+        Parameters
+        ----------
+        index: pd.Index
+            Index the new history should have. This is used to ensure the passed
+            functions worked correct and also used if the function does not apply,
+            because the initial history is empty. Then the altered empty history is
+            reindexed to this index.
+
+        func : callable
+            function to apply on `History.hist` (flags DataFrame)
+
+        func_kws : dict
+            hist-function keywords dict
+
+        func_handle_df : bool, default False
+            If `True`, the Dataframe under `History`.hist is passed to the given functions,
+            thus the function must handle `pd.Dataframes` as first input. If `False`, each
+            column is passed separately, thus the function must handle those.
+
+        copy : bool, default True
+            If False, alter the underlying history, otherwise return a copy.
+
+
+        Returns
+        -------
+        History with altered columns
+        """
+        hist = pd.DataFrame(index=index)
 
-        # .iloc[any, non-int]
+        # convert data to floats as functions may fail with categorical dtype
+        if func_handle_df:
+            hist = func(self._hist.astype(float, copy=True), **func_kws)
         else:
-            k = "?"
-            try:
+            for pos in self.columns:
+                hist[pos] = func(self._hist[pos].astype(float, copy=True), **func_kws)
 
-                for k in data.index:
-                    data.at[k] = data.at[k].iloc[rowkey]
-
-            except Exception as e:
-                raise type(e)(f"failed for column {k}: " + str(e)) from e
-
-            # .iloc[int, non-int] -> column-indexed series
-            if pdextra.is_integer(rowkey):
-                new = data
-
-            # .iloc[non-int, non-int] -> dios
-            else:
-                new = self.obj.copy_empty(columns=False)
-                new._data = data
-
-        return new
-
-    def __setitem__(self, key, value):
-        rowkey, colkey = self._unpack_key(key)
-        if _is_dios_like(rowkey) or _is_dios_like(colkey):
-            raise ValueError("Cannot index with multidimensional key")
-
-        # .iloc[any, int] = Any
-        if pdextra.is_integer(colkey):
-            if _is_dios_like(value) or pdextra.is_nested_list_like(value):
-                raise ValueError("Incompatible indexer with multi-dimensional value")
-            self._data.iat[colkey].iloc[rowkey] = value
-
-        # .iloc[any, non-int] = Any
+        try:
+            self._validate(hist, self._meta)
+        except Exception as e:
+            raise ValueError(
+                f"result from applied function is not a valid History, because {e}"
+            ) from e
+
+        if copy:
+            history = History(index=None)  # noqa
+            history._meta = self._meta.copy()
         else:
-            self._set_value_muli_column(rowkey, colkey, value, xloc="iloc")
+            history = self
 
+        history._hist = hist.astype("category")
 
-# #############################################################################
+        return history
 
+    def copy(self, deep=True) -> History:
+        """
+        Make a copy of the FH.
 
-class _aLocIndexer(_Indexer):
-    """align Indexer
+        Parameters
+        ----------
+        deep : bool, default True
+            - ``True``: make a deep copy
+            - ``False``: make a shallow copy
+
+        Returns
+        -------
+        copy : History
+            the copied FH
+        """
+        copyfunc = _copy.deepcopy if deep else _copy.copy
+        new = History(self.index)
+        new._hist = self._hist.copy(deep)
+        new._meta = copyfunc(self._meta)
+        return new
 
-    Automatically align (alignable) indexer on all possible axis,
-    and handle indexing with non-existent or missing keys gracefully.
+    def __copy__(self):
+        return self.copy(deep=False)
 
-    Also align (alignable) values before setting them with .loc
-    """
+    def __deepcopy__(self, memo=None):
+        """
+        Parameters
+        ----------
+        memo, default None
+            Standard signature. Unused
+        """
+        return self.copy(deep=True)
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._usebool = True
-
-    def __call__(self, usebool=True):
-        """We are called if the user want to set `usebool=False', which make
-        boolean alignable indexer treat as non-boolean alignable indexer.
-
-        Explanation: A boolean dios indexer align its indices with the indices
-        of the receiving dios like a non-boolean dios indexer also would do.
-        Additionally all rows with False values are kicked too. To disable
-         that `usebool=False` can be given."""
-        self._usebool = usebool
-        return self
+    def __len__(self) -> int:
+        return len(self._hist.columns)
 
-    def __getitem__(self, key):
-        rowkeys, colkeys, lowdim = self._unpack_key_aloc(key)
-        data = pd.Series(dtype="O", index=colkeys)
-        kws = dict(itype=self.obj.itype, cast_policy=self.obj._policy)
+    def __repr__(self):
+        if self.empty:
+            return str(self._hist).replace("DataFrame", "History")
 
-        c = "?"
-        try:
+        r = self._hist.astype(str)
 
-            for i, c in enumerate(data.index):
-                data.at[c] = self._data.at[c].loc[rowkeys[i]]
+        return str(r)[1:]
 
-        except Exception as e:
-            raise type(e)(f"failed for column {c}: " + str(e)) from e
+    # --------------------------------------------------------------------------------
+    # validation
+    #
 
-        if lowdim:
-            return data.squeeze()
-        else:
-            return self.obj._constructor(data=data, fastpath=True, **kws)._finalize(
-                self.obj
+    @classmethod
+    def _validate(
+        cls, hist: pd.DataFrame, meta: List[Any]
+    ) -> Tuple[pd.DataFrame, List]:
+        """
+        check type, columns, index, dtype of hist and if the meta fits also
+        """
+        cls._validateHist(hist)
+        cls._validateMetaList(meta, hist)
+        return hist, meta
+
+    @classmethod
+    def _validateHist(cls, obj):
+        if not isinstance(obj, pd.DataFrame):
+            raise TypeError(
+                f"'hist' must be of type pd.DataFrame, "
+                f"but is of type {type(obj).__name__}"
             )
-
-    def __setitem__(self, key, value):
-        rowkeys, colkeys, _ = self._unpack_key_aloc(key)
-
-        def iter_self(colkeys, position=False):
-            c = "?"
+        if not obj.columns.equals(pd.RangeIndex(len(obj.columns))):
+            raise ValueError(
+                "Columns of 'hist' must consist of "
+                "continuous increasing integers, "
+                "starting with 0."
+            )
+        for c in obj.columns:
             try:
-
-                for i, c in enumerate(colkeys):
-                    dat = self._data.at[c]
-                    rk = rowkeys[i]
-                    if len(dat.loc[rk]) == 0:
-                        continue
-                    yield dat, rk, i if position else c
-
+                cls._validateValue(obj[c])
             except Exception as e:
-                raise type(e)(f"failed for column {c}: " + str(e)) from e
+                raise ValueError(f"Bad column in hist. column '{c}': {e}") from None
+        return obj
 
-        # align columns, for rows use series.loc to align
-        if _is_dios_like(value):
-            colkeys = value.columns.intersection(colkeys)
-            for dat, rk, c in iter_self(colkeys):
-                dat.loc[rk] = value[c]
-
-        # no align, no merci
-        elif pdextra.is_nested_list_like(value):
-            if len(colkeys) != len(value):
+    @classmethod
+    def _validateMetaList(cls, obj, hist=None):
+        if not isinstance(obj, list):
+            raise TypeError(
+                f"'meta' must be of type list, got type {type(obj).__name__}"
+            )
+        if hist is not None:
+            if not len(obj) == len(hist.columns):
                 raise ValueError(
-                    f"shape mismatch: values array of shape "
-                    f"(.., {len(value)}) could not "
-                    f"be broadcast to indexing result of "
-                    f"shape (.., {len(colkeys)})"
+                    "'meta' must have as many entries as columns in 'hist'"
                 )
-            for dat, rk, i in iter_self(colkeys, position=True):
-                dat.loc[rk] = value[i]
+        for i, item in enumerate(obj):
+            try:
+                cls._validateMetaDict(item)
+            except Exception as e:
+                raise ValueError(f"Bad meta. item {i}: {e}") from None
+        return obj
 
-        # align rows by using series.loc
-        elif isinstance(value, pd.Series):
-            for dat, rk, _ in iter_self(colkeys):
-                dat.loc[rk] = value
+    @staticmethod
+    def _validateMetaDict(obj):
+        if not isinstance(obj, dict):
+            raise TypeError("obj must be dict")
+        if not all(isinstance(k, str) for k in obj.keys()):
+            raise ValueError("all keys in dict must be strings")
+        return obj
 
-        # no align, no merci
-        else:
-            for dat, rk, _ in iter_self(colkeys):
-                dat.loc[rk] = value
-
-    def _unpack_key_aloc(self, key):
+    @staticmethod
+    def _validateValue(obj: pd.Series) -> pd.Series:
         """
-        Return a list of row indexer and a list of existing(!) column labels.
-        Both list always have the same length and also could be empty together.
-
-        Note:
-            The items of the row indexer list should be passed to pd.Series.loc[]
-        """
-        # if a single column-key is given, the caller may
-        # want to return a single Series, instead of a dios
-        lowdim = False
-
-        def keys_from_bool_dios_like(key):
-            if not _is_bool_dios_like(key):
-                raise ValueError("Must pass dios-like key with boolean values only.")
-            colkey = self.obj.columns.intersection(key.columns)
-            rowkey = []
-            for c in colkey:
-                b = key[c]
-                rowkey += [self._data.at[c].index.intersection(b[b].index)]
-            return rowkey, colkey, lowdim
-
-        def keys_from_dios_like(key):
-            colkey = self.obj.columns.intersection(key.columns)
-            rowkey = [self._data.at[c].index.intersection(key[c].index) for c in colkey]
-            return rowkey, colkey, lowdim
-
-        rowkey, colkey = self._unpack_key(key)
-
-        if _is_dios_like(colkey) or pdextra.is_nested_list_like(colkey):
-            raise ValueError("Could not index with multi-dimensional column key.")
-
-        # giving the ellipsis as column key, is an alias
-        # for giving `usebool=False`. see self.__call__()
-        if colkey is Ellipsis:
-            self._usebool = False
-            colkey = slice(None)
-
-        # .aloc[dios]
-        if _is_dios_like(rowkey):
-
-            if not pdextra.is_null_slice(colkey):
-                raise ValueError(
-                    f"Could not index with a dios-like indexer as rowkey,"
-                    f"and a column key of that type {type(colkey)}"
-                )
-            if self._usebool:
-                return keys_from_bool_dios_like(rowkey)
-            else:
-                return keys_from_dios_like(rowkey)
-
-        # handle gracefully: scalar
-        elif pdextra.is_hashable(colkey):
-            colkey = [colkey] if colkey in self.obj.columns else []
-            lowdim = True
-
-        # column-alignable: list-like, filter only existing columns
-        elif pdextra.is_list_like(colkey) and not pdextra.is_bool_indexer(colkey):
-            colkey = colkey.values if isinstance(colkey, pd.Series) else colkey
-            colkey = self.obj.columns.intersection(colkey)
-
-        # handle gracefully (automatically)
-        # just a simple optimisation
-        elif pdextra.is_null_slice(colkey):
-            colkey = self.obj.columns
-
-        # not alignable, fall back to .loc (boolean list/series, slice(..), etc.
-        else:
-            colkey = self._data.loc[colkey].index
-
-        if len(colkey) == 0:  # (!) `if not colkey:` fails for pd.Index
-            return [], [], lowdim
-
-        rowkey = self._get_rowkey(rowkey, colkey)
-
-        return rowkey, colkey, lowdim
-
-    def _get_rowkey(self, rowkey, colkey, depth=0):
-
-        if pdextra.is_nested_list_like(rowkey) and depth == 0:
-            rowkey = rowkey.values if isinstance(rowkey, pd.Series) else rowkey
-            if len(rowkey) != len(colkey):
-                raise ValueError(
-                    "Nested arrays indexer must have same (outer) "
-                    "length than the number of selected columns."
-                )
-            indexer = []
-            for i, c in enumerate(colkey):
-                # recurse to get the row indexer from inner element
-                indexer += self._get_rowkey(rowkey[i], [c], depth=depth + 1)
-            rowkey = indexer
-
-        # row-alignable: pd.Series(), align rows to every series in colkey (columns)
-        elif isinstance(rowkey, pd.Series):
-            if self._usebool and pdextra.is_bool_indexer(rowkey):
-                rowkey = [
-                    self._data.at[c].index.intersection(rowkey[rowkey].index)
-                    for c in colkey
-                ]
-            else:
-                rowkey = [
-                    self._data.at[c].index.intersection(rowkey.index) for c in colkey
-                ]
-
-        # handle gracefully: scalar, transform to row-slice
-        elif pdextra.is_hashable(rowkey):
-            rowkey = [slice(rowkey, rowkey)] * len(colkey)
-
-        # handle gracefully: list-like, filter only existing rows
-        # NOTE: dios.aloc[series.index] is processed here
-        elif pdextra.is_list_like(rowkey) and not pdextra.is_bool_indexer(rowkey):
-            rowkey = [self._data.at[c].index.intersection(rowkey) for c in colkey]
-
-        # not alignable
-        # the rowkey is processed by .loc someway in
-        # the calling function - (eg. slice(..), boolean list-like, etc.)
-        else:
-            rowkey = [rowkey] * len(colkey)
-
-        return rowkey
-
-
-# #############################################################################
-
-
-class _AtIndexer(_Indexer):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def _check_key(self, key):
-        if not (
-            isinstance(key, tuple)
-            and len(key) == 2
-            and pdextra.is_hashable(key[0])
-            and pdextra.is_hashable(key[1])
-        ):
-            raise KeyError(
-                f"{key}. `.at` takes exactly one scalar row-key "
-                "and one scalar column-key"
-            )
-
-    def __getitem__(self, key):
-        self._check_key(key)
-        return self._data.at[key[1]].at[key[0]]
-
-    def __setitem__(self, key, value):
-        self._check_key(key)
-        if _is_dios_like(value) or pdextra.is_nested_list_like(value):
+        index is not checked !
+        """
+        if not isinstance(obj, pd.Series):
             raise TypeError(
-                ".at[] cannot be used to set multi-dimensional values, use .aloc[] instead."
+                f"value must be of type pd.Series, got type {type(obj).__name__}"
             )
-        self._data.at[key[1]].at[key[0]] = value
-
+        if not is_float_dtype(obj.dtype) and not is_categorical_dtype(obj.dtype):
+            raise ValueError("dtype must be float or categorical")
+        return obj
 
-# #############################################################################
+    @classmethod
+    def createFromData(cls, hist: pd.DataFrame, meta: List[Dict], copy: bool = False):
+        """
+        Create a History from existing data.
 
+        Parameters
+        ----------
+        hist : pd.Dataframe
+            Data that define the flags of the history.
+
+        meta : List of dict
+            A list holding meta information for each column, therefore it must
+            have the same number of entries as columns exist in `hist`.
+
+        copy : bool, default False
+            If `True`, the input data is copied, otherwise not.
+
+
+        Notes
+        -----
+        To create a very simple History from a flags dataframe ``f`` use
+        ``mask = pd.DataFrame(True, index=f.index, columns=f.columns``
+        and
+        ``meta = [{}] * len(f.columns)``.
+
+        Returns
+        -------
+        History
+        """
+        cls._validate(hist, meta)
 
-class _iAtIndexer(_Indexer):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def _check_key(self, key):
-        if not (
-            isinstance(key, tuple)
-            and len(key) == 2
-            and pdextra.is_integer(key[0])
-            and pdextra.is_integer(key[1])
-        ):
-            raise KeyError(
-                f"{key} `.iat` takes exactly one integer positional "
-                f"row-key and one integer positional scalar column-key"
-            )
+        if copy:
+            hist = hist.copy()
+            meta = _copy.deepcopy(meta)
+
+        history = cls(index=None)  # noqa
+        history._hist = hist.astype("category", copy=False)
+        history._meta = meta
+        return history
+
+
+def createHistoryFromData(
+    hist: pd.DataFrame,
+    meta: List[Dict],
+    copy: bool = False,
+):
+    """
+    Create a History from existing data.
 
-    def __getitem__(self, key):
-        self._check_key(key)
-        return self._data.iat[key[1]].iat[key[0]]
-
-    def __setitem__(self, key, value):
-        self._check_key(key)
-        if _is_dios_like(value) or pdextra.is_nested_list_like(value):
-            raise TypeError(
-                ".iat[] cannot be used to set multi-dimensional values, use .aloc[] instead."
-            )
-        self._data.iat[key[1]].iat[key[0]] = value
+    Parameters
+    ----------
+    hist : pd.Dataframe
+        Data that define the flags of the history.
+
+    meta : List of dict
+        A list holding meta information for each column, therefore it must
+        have the same number of entries as columns exist in `hist`.
+
+    copy : bool, default False
+        If `True`, the input data is copied, otherwise not.
+
+
+    Notes
+    -----
+    To create a very simple History from a flags dataframe ``f`` use
+    ``mask = pd.DataFrame(True, index=f.index, columns=f.columns``
+    and
+    ``meta = [{}] * len(f.columns)``.
+
+    Returns
+    -------
+    History
+    """
+    # todo: expose History, enable this warning
+    # warnings.warn(
+    #     "saqc.createHistoryFromData() will be deprecated soon. "
+    #     "Please use saqc.History.createFromData() instead.",
+    #     category=FutureWarning,
+    # )
+    return History.createFromData(hist, meta, copy)
```

### Comparing `saqc-2.3/saqc/__main__.py` & `saqc-2.4.0/saqc/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from pathlib import Path
 
 import click
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 
-from dios.dios.dios import DictOfSeries
+from saqc.core import DictOfSeries
 from saqc.core.core import TRANSLATION_SCHEMES
-from saqc.core.reader import fromConfig
+from saqc.parsing.reader import fromConfig
 
 logger = logging.getLogger("SaQC")
 
 
 def _setupLogging(loglvl):
     logger.setLevel(loglvl)
     handler = logging.StreamHandler()
@@ -107,21 +107,20 @@
 
     saqc = fromConfig(
         config,
         data=data,
         scheme=TRANSLATION_SCHEMES[scheme or "simple"](),
     )
 
-    data_result = saqc.data.to_df()
+    data_result = saqc.data.to_pandas()
     flags_result = saqc.flags
     if isinstance(flags_result, DictOfSeries):
-        flags_result = flags_result.to_df()
+        flags_result = flags_result.to_pandas()
 
     if outfile:
-
         data_result.columns = pd.MultiIndex.from_product(
             [data_result.columns.tolist(), ["data"]]
         )
 
         if not isinstance(flags_result.columns, pd.MultiIndex):
             flags_result.columns = pd.MultiIndex.from_product(
                 [flags_result.columns.tolist(), ["flags"]]
```

### Comparing `saqc-2.3/saqc/core/core.py` & `saqc-2.4.0/saqc/core/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 from copy import copy as shallowcopy
 from copy import deepcopy
 from typing import Any, Hashable, MutableMapping
 
 import numpy as np
 import pandas as pd
 
-from dios import DictOfSeries, to_dios
-from saqc.core.flags import Flags, initFlagsLike
+from saqc.core.flags import Flags, _HistAccess, initFlagsLike
+from saqc.core.frame import DictOfSeries
 from saqc.core.history import History
 from saqc.core.register import FUNC_MAP
 from saqc.core.translation import (
     DmpScheme,
     FloatScheme,
     PositionalScheme,
     SimpleScheme,
     TranslationScheme,
 )
 from saqc.funcs import FunctionsMixin
-from saqc.lib.tools import concatDios
 
 # warnings
 pd.set_option("mode.chained_assignment", "warn")
+pd.options.mode.copy_on_write = False
 np.seterr(invalid="ignore")
 
 
 TRANSLATION_SCHEMES = {
     "float": FloatScheme,
     "simple": SimpleScheme,
     "dmp": DmpScheme,
@@ -110,14 +110,18 @@
 
     @property
     def flags(self) -> MutableMapping:
         flags = self._scheme.toExternal(self._flags, attrs=self._attrs)
         flags.attrs = self._attrs.copy()
         return flags
 
+    @property
+    def _history(self) -> _HistAccess:
+        return self._flags.history
+
     def __getattr__(self, key):
         """
         All failing attribute accesses are redirected to __getattr__.
         We use this mechanism to make the registered functions appear
         as `SaQC`-methods without actually implementing them.
         """
         from functools import partial
@@ -148,47 +152,57 @@
             return scheme
         raise TypeError(
             f"expected one of the following translation schemes '{TRANSLATION_SCHEMES.keys()} "
             f"or an initialized Translator object, got '{scheme}'"
         )
 
     def _initData(self, data) -> DictOfSeries:
-
         if data is None:
             return DictOfSeries()
-
         if isinstance(data, list):
-            results = []
+            result = DictOfSeries()
+            doubles = pd.Index([])
             for d in data:
-                results.append(self._castToDios(d))
-            return concatDios(results, warn=True, stacklevel=3)
-
-        if isinstance(data, (DictOfSeries, pd.DataFrame, pd.Series)):
-            return self._castToDios(data)
+                new = self._castData(d)
+                doubles = doubles.union(result.columns.intersection(new.columns))
+                result.update(new)
+            if not doubles.empty:
+                warnings.warn(
+                    f"Column(s) {doubles.tolist()} was present multiple "
+                    f"times in input data. Some data was overwritten. "
+                    f"Avoid duplicate columns names over all inputs.",
+                    stacklevel=2,
+                )
+            return result
+        try:
+            return self._castData(data)
+        except ValueError as e:
+            raise e from None
+        except TypeError as e:
+            raise TypeError(
+                "'data' must be of type pandas.Series, "
+                "pandas.DataFrame or saqc.DictOfSeries or "
+                "a list of those or a dict with string keys "
+                "and pandas.Series as values."
+            ) from e
 
-        raise TypeError(
-            "'data' must be of type pandas.Series, "
-            "pandas.DataFrame or dios.DictOfSeries or "
-            "a list of those."
-        )
-
-    def _castToDios(self, data):
+    def _castData(self, data) -> DictOfSeries:
         if isinstance(data, pd.Series):
             if not isinstance(data.name, str):
                 raise ValueError(f"Cannot init from unnamed pd.Series")
             data = data.to_frame()
         if isinstance(data, pd.DataFrame):
             for idx in [data.index, data.columns]:
                 if isinstance(idx, pd.MultiIndex):
-                    raise TypeError("'data' should not have MultiIndex")
-        data = to_dios(data)  # noop for DictOfSeries
-        for c in data.columns:
-            if not isinstance(c, str):
-                raise TypeError("columns labels must be of type string")
-        return data
+                    raise ValueError("'data' should not have MultiIndex")
+        try:
+            # This ensures that values are pd.Series
+            return DictOfSeries(data)
+        except Exception:
+            raise TypeError(f"Cannot cast {type(data)} to DictOfSeries") from None
 
     def _initFlags(self, flags) -> Flags:
         if flags is None:
             return initFlagsLike(self._data)
 
         if isinstance(flags, list):
             result = Flags()
```

### Comparing `saqc-2.3/saqc/core/flags.py` & `saqc-2.4.0/saqc/core/flags.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
-from typing import DefaultDict, Dict, Iterable, Mapping, Tuple, Type, Union
+import typing
+import warnings
+from typing import DefaultDict, Dict, Iterable, Mapping, Tuple, Type, Union, overload
 
 import numpy as np
 import pandas as pd
 
-import dios
-from saqc.core.history import History
+from saqc.core import DictOfSeries, History
 
 _VAL = Union[pd.Series, History]
 DictLike = Union[
     pd.DataFrame,
-    dios.DictOfSeries,
+    DictOfSeries,
     Dict[str, _VAL],
     DefaultDict[str, _VAL],
 ]
 
 _Field = str
 SelectT = Union[
     _Field,
@@ -31,25 +32,25 @@
     Tuple[slice, _Field],
 ]
 ValueT = Union[pd.Series, Iterable, float]
 
 
 class _HistAccess:
     def __init__(self, obj: Flags):
-        self.obj = obj
+        self._obj = obj
 
     def __getitem__(self, key: str) -> History:
-        return self.obj._data[key]
+        return self._obj._data[key]
 
     def __setitem__(self, key: str, value: History):
         if not isinstance(value, History):
             raise TypeError("Not a History")
 
-        self.obj._validateHistForFlags(value)
-        self.obj._data[key] = value
+        self._obj._validateHistForFlags(value)
+        self._obj._data[key] = value
 
 
 class Flags:
     """
     SaQC's flags container.
 
     This container class holds the quality flags associated with the data. It hold key-value pairs, where
@@ -73,19 +74,18 @@
     Examples
     --------
 
     We create an empty instance, by calling ``Flags`` without any arguments and then add a column to it.
 
     .. doctest:: exampleFlags
 
-       >>> from saqc.constants import UNFLAGGED, BAD, DOUBTFUL
-       >>> flags = saqc.Flags()
+       >>> from saqc import UNFLAGGED, BAD, DOUBTFUL, Flags
+       >>> flags = Flags()
        >>> flags
        Empty Flags
-       Columns: []
 
     .. doctest:: exampleFlags
 
        >>> flags['v0'] = pd.Series([BAD,BAD,UNFLAGGED], dtype=float)
        >>> flags # doctest:+NORMALIZE_WHITESPACE
              v0 |
        ======== |
@@ -188,15 +188,14 @@
              0     1     2    3     4
        0  255.0  25.0  25.0  0.0  99.0
        1  255.0   nan   nan  nan  99.0
        2   -inf  25.0  25.0  0.0  99.0
     """
 
     def __init__(self, raw_data: DictLike | Flags | None = None, copy: bool = False):
-
         self._data: dict[str, History]
 
         if raw_data is None:
             raw_data = {}
 
         if isinstance(raw_data, Flags):
             if copy:
@@ -211,15 +210,14 @@
         """
         init from dict-like: keys are flag column, values become
         initial columns of history(s).
         """
         result = {}
 
         for k, item in data.items():
-
             if not isinstance(k, str):
                 raise ValueError("column names must be string")
             if k in result:
                 raise ValueError("raw_data must not have duplicate keys")
 
             # a passed History is not altered. So if the passed History
             # does not fit for Flags, we fail hard.
@@ -256,14 +254,17 @@
     @property
     def _constructor(self) -> Type["Flags"]:
         return type(self)
 
     # ----------------------------------------------------------------------
     # meta data
 
+    def keys(self) -> typing.KeysView:
+        return self._data.keys()
+
     @property
     def columns(self) -> pd.Index:
         """
         Column index of the flags container
 
         Returns
         -------
@@ -315,16 +316,44 @@
 
     def __contains__(self, item):
         return item in self.columns
 
     # ----------------------------------------------------------------------
     # item access
 
+    @overload
     def __getitem__(self, key: str) -> pd.Series:
-        return self._data[key].squeeze()
+        ...
+
+    @overload
+    def __getitem__(self, key: list | pd.Index) -> Flags:
+        ...
+
+    def __getitem__(self, key: str | list | pd.Index) -> pd.Series | Flags:
+        if isinstance(key, str):
+            return self._data[key].squeeze()
+
+        if isinstance(key, slice):
+            key = self.columns[key]
+
+        if isinstance(key, (list, pd.Index)):
+            # only copy necessary data
+            data = self._data
+            try:
+                self._data = {}
+                new = self.copy()
+            finally:
+                self._data = data
+            new._data = {k: self._data[k].copy() for k in key}
+            return new
+
+        raise TypeError(
+            "Key must be of type str, list or index of string or slice,"
+            f"not {type(key)}."
+        )
 
     def __setitem__(self, key: SelectT, value: ValueT):
         # force-KW is only internally available
 
         if isinstance(key, tuple):
             if len(key) != 2:
                 raise KeyError(
@@ -392,15 +421,15 @@
     @property
     def history(self) -> _HistAccess:
         """
         Accessor for the flags history.
 
         Access via ``flags.history['var']``.
         To set a new history use ``flags.history['var'] = value``.
-        The passed value must be a instance of History or must be convertible to a
+        The passed value must be an instance of History or must be convertible to a
         history.
 
         Returns
         -------
         history : History
             Accessor for the flags history
 
@@ -442,53 +471,56 @@
             Standard signature. Unused
         """
         return self.copy(deep=True)
 
     # ----------------------------------------------------------------------
     # transformation and representation
 
-    def toDios(self) -> dios.DictOfSeries:
+    def toDios(self) -> DictOfSeries:
         """
-        Transform the flags container to a ``dios.DictOfSeries``.
+        Transform the flags container to a ``DictOfSeries``.
+
+
+        .. deprecated:: 2.4
+           use `saqc.DictOfSeries(obj)` instead.
 
         Returns
         -------
-        dios.DictOfSeries
+        DictOfSeries
         """
-        di = dios.DictOfSeries(columns=self.columns)
-
-        for k in self._data.keys():
-            di[k] = self[k]
-
-        return di.copy()
+        warnings.warn(
+            "toDios is deprecated, use `saqc.DictOfSeries(obj)` instead.",
+            category=DeprecationWarning,
+        )
+        return DictOfSeries(self).copy()
 
     def toFrame(self) -> pd.DataFrame:
         """
         Transform the flags container to a ``pd.DataFrame``.
 
         Returns
         -------
         pd.DataFrame
         """
-        return self.toDios().to_df()
+        return pd.DataFrame(dict(self))
 
     def __repr__(self) -> str:
-        return str(self.toDios()).replace("DictOfSeries", type(self).__name__)
+        return str(DictOfSeries(self)).replace("DictOfSeries", type(self).__name__)
 
 
 def initFlagsLike(
     reference: Union[pd.Series, DictLike, Flags],
     name: str = None,
 ) -> Flags:
     """
-    Create empty Flags, from an reference data structure.
+    Create empty Flags, from a reference data structure.
 
     Parameters
     ----------
-    reference : pd.DataFrame, pd.Series, dios.DictOfSeries, dict of pd.Series
+    reference : pd.DataFrame, pd.Series, DictOfSeries, dict of pd.Series
         The reference structure to initialize for.
 
     name : str, default None
         Only respected if `reference` is of type ``pd.Series``.
         The column name that is used for the Flags. If ``None``
         the name of the series itself is taken, if it is unset,
         a ValueError is raised.
@@ -520,15 +552,14 @@
                 "either the passed pd.Series must be named or a name must be passed"
             )
         if not isinstance(name, str):
             raise TypeError(f"name must be str not '{type(name).__name__}'")
         reference = reference.to_frame(name=name)
 
     for k, item in reference.items():
-
         if not isinstance(k, str):
             raise TypeError(
                 f"cannot use '{k}' as a column name, currently only string keys are allowed"
             )
         if k in result:
             raise ValueError("reference must not have duplicate column names")
         if not isinstance(item, (pd.Series, History)):
```

### Comparing `saqc-2.3/saqc/core/mixins.py` & `saqc-2.4.0/saqc/funcs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python
+
+# SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+
 # -*- coding: utf-8 -*-
 
 from saqc.funcs.breaks import BreaksMixin
 from saqc.funcs.changepoints import ChangepointsMixin
 from saqc.funcs.constants import ConstantsMixin
 from saqc.funcs.curvefit import CurvefitMixin
 from saqc.funcs.drift import DriftMixin
@@ -15,26 +20,28 @@
 from saqc.funcs.resampling import ResamplingMixin
 from saqc.funcs.residuals import ResidualsMixin
 from saqc.funcs.rolling import RollingMixin
 from saqc.funcs.scores import ScoresMixin
 from saqc.funcs.tools import ToolsMixin
 from saqc.funcs.transformation import TransformationMixin
 
-_MIXINS = (
+
+class FunctionsMixin(
+    BreaksMixin,
+    ChangepointsMixin,
+    ConstantsMixin,
+    CurvefitMixin,
+    DriftMixin,
+    FlagtoolsMixin,
+    GenericMixin,
     InterpolationMixin,
-    PatternMixin,
     NoiseMixin,
+    OutliersMixin,
+    PatternMixin,
+    ResamplingMixin,
     ResidualsMixin,
-    ChangepointsMixin,
     RollingMixin,
-    TransformationMixin,
     ScoresMixin,
-    DriftMixin,
-    CurvefitMixin,
-    ResamplingMixin,
-    ConstantsMixin,
-    GenericMixin,
     ToolsMixin,
-    OutliersMixin,
-    FlagtoolsMixin,
-    BreaksMixin,
-)
+    TransformationMixin,
+):
+    pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `saqc-2.3/saqc/core/reader.py` & `saqc-2.4.0/saqc/parsing/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from pathlib import Path
 from typing import TextIO
 from urllib.error import URLError
 from urllib.request import urlopen
 
 import pandas as pd
 
-from saqc.core.core import SaQC
-from saqc.core.visitor import ConfigFunctionParser
+from saqc import SaQC
 from saqc.lib.tools import isQuoted
+from saqc.parsing.visitor import ConfigFunctionParser
 
 COMMENT = "#"
 SEPARATOR = ";"
 
 
 def _openFile(fname) -> TextIO:
     if isinstance(fname, (str, Path)):
@@ -40,15 +40,14 @@
     try:
         fobj.close()
     except AttributeError:
         pass
 
 
 def readFile(fname) -> pd.DataFrame:
-
     fobj = _openFile(fname)
 
     out = []
     for i, line in enumerate(fobj):
         row = line.strip().split(COMMENT, 1)[0]
         if not row:
             # skip over comment line
@@ -77,15 +76,14 @@
 
 # Todo: needs a (maybe tiny) docstring!
 def fromConfig(fname, *args, **func_kwargs):
     saqc = SaQC(*args, **func_kwargs)
     config = readFile(fname)
 
     for _, field, expr in config.itertuples():
-
         regex = False
         if isQuoted(field):
             fld = field[1:-1]
             regex = True
         else:
             fld = field
```

### Comparing `saqc-2.3/saqc/core/register.py` & `saqc-2.4.0/saqc/core/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 #!/usr/bin/env python
 
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
 from __future__ import annotations
 
 import functools
 import inspect
 import warnings
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Sequence, Tuple, TypeVar
 
 import numpy as np
 import pandas as pd
 from typing_extensions import ParamSpec
 
-import dios
-from saqc.constants import FILTER_ALL, FILTER_NONE, UNFLAGGED
-from saqc.core.flags import Flags, History
+from saqc import FILTER_ALL, FILTER_NONE
+from saqc.core import DictOfSeries, Flags, History
 from saqc.core.translation.basescheme import TranslationScheme
-from saqc.lib.tools import squeezeSequence, toSequence
+from saqc.lib.docs import ParamDict, docurator
+from saqc.lib.tools import isflagged, squeezeSequence, toSequence
 from saqc.lib.types import ExternalFlag, OptionalNone
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
+
+__all__ = [
+    "register",
+    "processing",
+    "flagging",
+]
 
 # NOTE:
 # the global SaQC function store,
 # will be filled by calls to register
 FUNC_MAP: Dict[str, Callable] = {}
 
 _is_list_like = pd.api.types.is_list_like
@@ -132,15 +137,14 @@
     Flags
     """
     out = old_flags.copy()  # the old flags
 
     for col in columns.union(
         new_flags.columns.difference(old_flags.columns)
     ):  # account for newly added columns
-
         if col not in out:  # ensure existence
             out.history[col] = History(index=new_flags.history[col].index)
 
         old_history = out.history[col]
         new_history = new_flags.history[col]
 
         # We only want to add new columns, that were appended during the last
@@ -150,47 +154,45 @@
         squeezed = new_history.squeeze(raw=True, start=start)
         out.history[col] = out.history[col].append(squeezed, meta=meta)
 
     return out
 
 
 def _maskData(
-    data: dios.DictOfSeries, flags: Flags, columns: Sequence[str], thresh: float
-) -> Tuple[dios.DictOfSeries, dios.DictOfSeries]:
+    data: DictOfSeries, flags: Flags, columns: Sequence[str], thresh: float
+) -> Tuple[DictOfSeries, DictOfSeries]:
     """
     Mask data with Nans, if the flags are worse than a threshold.
         - mask only passed `columns` (preselected by `datamask`-kw from decorator)
 
     Returns
     -------
-    masked : dios.DictOfSeries
+    masked : DictOfSeries
         masked data, same dim as original
-    mask : dios.DictOfSeries
+    mask : DictOfSeries
         dios holding iloc-data-pairs for every column in `data`
     """
-    mask = dios.DictOfSeries(columns=columns)
+    mask = DictOfSeries()
 
     # we use numpy here because it is faster
     for c in columns:
-        col_mask = _isflagged(flags[c], thresh)
+        col_mask = isflagged(flags[c].to_numpy(), thresh)
 
         if col_mask.any():
-            col_data = data[c].to_numpy(dtype=np.float64)
-
+            col_data = data[c].to_numpy(dtype=np.float64, copy=True)
             mask[c] = pd.Series(col_data[col_mask], index=np.where(col_mask)[0])
-
             col_data[col_mask] = np.nan
-            data[c] = col_data
+            data[c] = pd.Series(col_data, index=data[c].index)
 
     return data, mask
 
 
 def _unmaskData(
-    data: dios.DictOfSeries, mask: dios.DictOfSeries, columns: pd.Index | None = None
-) -> dios.DictOfSeries:
+    data: DictOfSeries, mask: DictOfSeries, columns: pd.Index | None = None
+) -> DictOfSeries:
     """
     Restore the masked data.
 
     Notes
     -----
     - Even if this returns data, it works inplace !
     - `mask` is not a boolean mask, instead it holds the original values.
@@ -198,15 +200,14 @@
       in the original data.
     """
     if columns is None:
         columns = data.columns  # field was in old, is in mask and is in new
     columns = mask.columns.intersection(columns)
 
     for c in columns:
-
         # ignore
         if data[c].empty or mask[c].empty:
             continue
 
         # get the positions of values to unmask
         candidates = mask[c]
         # if the mask was removed during the function call, don't replace
@@ -258,88 +259,100 @@
 
 def register(
     mask: list[str],
     demask: list[str],
     squeeze: list[str],
     multivariate: bool = False,
     handles_target: bool = False,
+    docstring: dict[str, ParamDict] | None = None,
 ):
     """
     Generalized decorator for any saqc functions.
 
     Before the call of the decorated function:
     - data gets masked by flags according to `dfilter`
 
     After the call of the decorated function:
     - data gets demasked (original data is written back)
     - flags gets squeezed (only one history column append per call)
 
     Parameters
     ----------
     mask : list of string
-        A list of all parameter of the decorated function, that specify a column in
-        data, that is read by the function and therefore should be masked by flags.
+        List of parameters of the decorated function, that specify column(s) in
+        ``SaQC._data``, that are read by the function and therefore should be masked.
 
         The masking takes place before the call of the decorated function and
         temporary sets data to `NaN` at flagged locations. It is undone by ``demask``.
         The threshold of which data is considered to be flagged can be controlled
         via ``dfilter``, a parameter each function takes.
 
     demask : list of string
-        A list of all parameter of the decorated function, that specify a column in
-        data, that was masked (see ``mask``) and needs unmasking after the call.
+        List of parameters of the decorated function, that specify column(s) in
+        ``SaQC._data``, that were masked (see ``mask``) and needs unmasking after the call.
 
-        The unmasking replace all remaining(!) ``NaN`` by its original values from
-        before the call of the decorated function.
+        The unmasking replaces all remaining(!) ``NaN`` inserted in the masking process by
+        its their original values.
 
     squeeze : list of string
-        A list of all parameter of the decorated function, that specify a column in
-        flags, that is written by the function.
+        List of parameters of the decorated function, that specify flag column(s),
+        that are written by the function.
 
         The squeezing combines multiple columns in the history of flags to one
         single column. This is because, multiple writes to flags, (eg. using
         ``flags[:,'a'] = 255`` twice) will result in multiple history columns,
         but should considered as a single column, because only one function call
         happened.
 
     multivariate : bool, default False
-        If ``True``, the decorated function, process multiple data or flags
+        If ``True``, the decorated function, processes multiple data or flag
         columns at once. Therefore the decorated function must handle a list
         of columns in the parameter ``field``.
 
-        If ``False``, the decorated function must take a single column (``str``)
-        in ``field``.
+        If ``False``, the decorated function must define ``field: str``
 
     handles_target : bool, default False
         If ``True``, the decorated function, handles the target parameter by
         itself. Mandatory for multivariate functions.
+
+    docstring : dict, default None
+        Allows to modify the default docstring description of the parameters ``field``,
+        ``target``, ``dfilter`` and ``flag``
+
     """
 
     def outer(func: Callable[P, SaQC]) -> Callable[P, SaQC]:
-
         func_signature = inspect.signature(func)
         _checkDecoratorKeywords(
             func_signature, func.__name__, mask, demask, squeeze, handles_target
         )
+        func = docurator(func, docstring)
 
         @functools.wraps(func)
         def inner(
             saqc,
             field,
             *args,
             regex: bool = False,
             flag: ExternalFlag | OptionalNone = OptionalNone(),
             **kwargs,
         ) -> "SaQC":
-
             # args -> kwargs
             paramnames = tuple(func_signature.parameters.keys())[
                 2:
             ]  # skip (self, field)
-            kwargs = {**dict(zip(paramnames, args)), **kwargs}
+
+            # check for duplicated arguments
+            args_map = dict(zip(paramnames, args))
+            intersection = set(args_map).intersection(set(kwargs))
+            if intersection:
+                raise TypeError(
+                    f"SaQC.{func.__name__}() got multiple values for argument '{intersection.pop()}'"
+                )
+            kwargs = {**args_map, **kwargs}
             kwargs["dfilter"] = _getDfilter(func_signature, saqc._scheme, kwargs)
 
             # translate flag
             if not isinstance(flag, OptionalNone):
                 # translation schemes might want to use a flag
                 # `None` so we introduce a special class here
                 kwargs["flag"] = saqc._scheme(flag)
@@ -462,23 +475,7 @@
     See Also
     --------
         resister: generalization of of this function
     """
     if kwargs:
         raise ValueError("use '@register' to pass keywords")
     return register(mask=[], demask=[], squeeze=[])
-
-
-A = TypeVar("A", np.ndarray, pd.Series)
-
-
-def _isflagged(flagscol: A, thresh: float) -> A:
-    """
-    Return a mask of flags accordingly to `thresh`. Return type is same as flags.
-    """
-    if not isinstance(thresh, (float, int)):
-        raise TypeError(f"thresh must be of type float, not {repr(type(thresh))}")
-
-    if thresh == FILTER_ALL:
-        return flagscol > UNFLAGGED
-
-    return flagscol >= thresh
```

### Comparing `saqc-2.3/saqc/core/translation/basescheme.py` & `saqc-2.4.0/saqc/core/translation/basescheme.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
-from abc import abstractmethod, abstractproperty
+from abc import abstractmethod
 from typing import Any, Dict
 
 import numpy as np
 import pandas as pd
 
-from dios import DictOfSeries
-from saqc.constants import BAD, FILTER_ALL, GOOD, UNFLAGGED
-from saqc.core.flags import Flags
+from saqc import BAD, FILTER_ALL, GOOD, UNFLAGGED
+from saqc.core import DictOfSeries, Flags
 from saqc.lib.types import ExternalFlag
 
 ForwardMap = Dict[ExternalFlag, float]
 BackwardMap = Dict[float, ExternalFlag]
 
 
 class TranslationScheme:  # pragma: no cover
@@ -31,33 +30,60 @@
 
     @abstractmethod
     def __call__(self, flag: ExternalFlag) -> float:
         pass
 
     @abstractmethod
     def toInternal(self, flags: pd.DataFrame | DictOfSeries) -> Flags:
+        """
+        Translate from 'external flags' to 'internal flags'
+
+        Parameters
+        ----------
+        flags : pd.DataFrame
+            The external flags to translate
+
+        Returns
+        -------
+        Flags object
+        """
         pass
 
     @abstractmethod
     def toExternal(self, flags: Flags, attrs: dict | None = None) -> DictOfSeries:
+        """
+        Translate from 'internal flags' to 'external flags'
+
+        Parameters
+        ----------
+        flags : pd.DataFrame
+            The external flags to translate
+
+        attrs : dict or None, default None
+            global meta information of saqc-object
+
+        Returns
+        -------
+        pd.DataFrame
+        """
         pass
 
 
 class MappingScheme(TranslationScheme):
     """
     This class provides the basic translation mechanism and should serve as
-    a base class for every other translation scheme.
+    a base class for most other translation scheme.
 
-    The general translation is realized through dictionary lookups, altough
+    The general translation is realized through dictionary lookups, although
     we might need to extend this logic to also allow calls to translation
-    functions in the future. Currently at least one `dict` defining the
+    functions in the future. Currently, at least one `dict` defining the
     'forward' translation  from 'user flags' -> 'internal flags' needs to be
     provided.
     Optionally a second `dict` can be passed to map 'internal flags' -> 'user flags',
-    if the latter is not given, this 'backward' translation will inferred as
+    if the latter is not given, this 'backward' translation is inferred as
     the inverse of the 'forward' translation.
 
     The translation mechanism imposes a few restrictions:
 
     - The scheme must be well definied, i.e. we need a backward translation for
       every forward translation (each value in `self._forward` needs a key in
       `self._backward`).
@@ -123,15 +149,16 @@
         out = DictOfSeries()
         expected = pd.Index(trans_map.values())
         for field in flags.columns:
             out[field] = flags[field].replace(trans_map)
             diff = pd.Index(out[field]).difference(expected)
             if not diff.empty:
                 raise ValueError(
-                    f"flags were not translated: {diff.drop_duplicates().to_list()}"
+                    f"following flag values could not be "
+                    f"translated: {diff.drop_duplicates().to_list()}"
                 )
         return out
 
     def __call__(self, flag: ExternalFlag) -> float:
         """
         Translate a scalar 'external flag' to an 'internal flag'
 
@@ -196,49 +223,24 @@
     Acts as the default Translator, provides a changeable subset of the
     internal float flags
     """
 
     DFILTER_DEFAULT: float = FILTER_ALL
 
     def __call__(self, flag: float | int) -> float:
-
         try:
             return float(flag)
         except (TypeError, ValueError, OverflowError):
             raise ValueError(f"invalid flag, expected a numerical value, got: {flag}")
 
     def toInternal(self, flags: pd.DataFrame | DictOfSeries) -> Flags:
         try:
             return Flags(flags.astype(float))
         except (TypeError, ValueError, OverflowError):
             raise ValueError(
                 f"invalid flag(s), expected a collection of numerical values, got: {flags}"
             )
 
     def toExternal(self, flags: Flags, attrs: dict | None = None) -> DictOfSeries:
-        out = flags.toDios()
+        out = DictOfSeries(flags)
         out.attrs = attrs or {}
         return out
-
-
-class SimpleScheme(MappingScheme):
-
-    """
-    Acts as the default Translator, provides a changeable subset of the
-    internal float flags
-    """
-
-    _FORWARD = {
-        "UNFLAGGED": UNFLAGGED,
-        "BAD": BAD,
-        "OK": GOOD,
-    }
-
-    _BACKWARD = {
-        UNFLAGGED: "UNFLAGGED",
-        np.nan: "UNFLAGGED",
-        BAD: "BAD",
-        GOOD: "OK",
-    }
-
-    def __init__(self):
-        super().__init__(forward=self._FORWARD, backward=self._BACKWARD)
```

### Comparing `saqc-2.3/saqc/core/translation/dmpscheme.py` & `saqc-2.4.0/saqc/core/translation/dmpscheme.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 import json
 from functools import reduce
 
 import numpy as np
 import pandas as pd
 
-from saqc.constants import BAD, DOUBTFUL, GOOD, UNFLAGGED
-from saqc.core.flags import Flags
-from saqc.core.history import History
+from saqc import BAD, DOUBTFUL, GOOD, UNFLAGGED
+from saqc.core import Flags, History
 from saqc.core.translation.basescheme import BackwardMap, ForwardMap, MappingScheme
+from saqc.lib.tools import getUnionIndex
 
 _QUALITY_CAUSES = [
     "",
     "BATTERY_LOW",
     "BELOW_MINIMUM",
     "ABOVE_MAXIMUM",
     "BELOW_OR_ABOVE_MIN_MAX",
@@ -130,31 +130,29 @@
         Returns
         -------
         translated flags
         """
         tflags = super().toExternal(flags, attrs=attrs)
 
         out = pd.DataFrame(
-            index=reduce(lambda x, y: x.union(y), tflags.indexes).sort_values(),
+            index=getUnionIndex(tflags),
             columns=pd.MultiIndex.from_product([flags.columns, _QUALITY_LABELS]),
         )
 
         for field in tflags.columns:
-
             df = pd.DataFrame(
                 {
                     "quality_flag": tflags[field],
                     "quality_cause": "",
                     "quality_comment": "",
                 }
             )
 
             history = flags.history[field]
             for col in history.columns:
-
                 valid = (history.hist[col] != UNFLAGGED) & history.hist[col].notna()
 
                 # extract from meta
                 meta = history.meta[col]
                 keywords = meta.get("kwargs", {})
                 comment = json.dumps(
                     {
@@ -187,15 +185,14 @@
 
         if not cols.get_level_values(1).isin(_QUALITY_LABELS).all(axis=None):
             raise TypeError(
                 f"DMP-Flags expect the labels {list(_QUALITY_LABELS)} in the secondary level"
             )
 
         for field in df.columns.get_level_values(0):
-
             # we might have NaN injected by DictOfSeries -> DataFrame conversions
             field_df = df[field].dropna(how="all", axis="index")
             flags = field_df["quality_flag"]
             causes = field_df["quality_cause"]
             comments = field_df["quality_comment"]
 
             if not flags.isin(cls._FORWARD.keys()).all(axis=None):
@@ -209,11 +206,11 @@
                 )
 
             if (~flags.isin(("OK", "NIL")) & (causes == "")).any(axis=None):
                 raise ValueError(
                     "quality flags other than 'OK and 'NIL' need a non-empty quality cause"
                 )
 
-            if ((causes == "OTHER") & (comments == "")).any(None):
+            if ((causes == "OTHER") & (comments == "")).any(axis=None):
                 raise ValueError(
                     "quality cause 'OTHER' needs a non-empty quality comment"
                 )
```

### Comparing `saqc-2.3/saqc/core/translation/positionalscheme.py` & `saqc-2.4.0/saqc/core/translation/positionalscheme.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
 from saqc.constants import BAD, DOUBTFUL, GOOD, UNFLAGGED
-from saqc.core.flags import Flags, History
+from saqc.core import Flags, History
 from saqc.core.translation.basescheme import BackwardMap, ForwardMap, MappingScheme
 
 
 class PositionalScheme(MappingScheme):
 
     """
     Implements the translation from and to the flagging scheme implemented by CHS
@@ -55,15 +55,14 @@
         Returns
         -------
         Flags object
         """
 
         data = {}
         for field, field_flags in flags.items():
-
             # explode the flags into sperate columns and drop the leading `9`
             df = pd.DataFrame(
                 field_flags.astype(str).str.slice(start=1).apply(tuple).tolist(),
                 index=field_flags.index,
             ).astype(int)
 
             # the exploded values form the History of `field`
@@ -88,15 +87,15 @@
         -------
         pd.DataFrame
         """
         out = {}
         for field in flags.columns:
             thist = flags.history[field].hist.replace(self._BACKWARD).astype(float)
             # concatenate the single flag values
-            ncols = thist.shape[-1]
+            ncols = len(thist.columns)
             init = 9 * 10**ncols
             bases = 10 ** np.arange(ncols - 1, -1, -1)
 
             tflags = init + (thist * bases).sum(axis=1)
             out[field] = tflags
 
         return pd.DataFrame(out).fillna(-9999).astype(int)
```

### Comparing `saqc-2.3/saqc/core/visitor.py` & `saqc-2.4.0/saqc/parsing/visitor.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 import ast
+import importlib
+
+import numpy as np
 
-from saqc.constants import ENVIRONMENT
 from saqc.core.register import FUNC_MAP
+from saqc.parsing.environ import ENVIRONMENT
 
 
 class ConfigExpressionParser(ast.NodeVisitor):
     """
     Generic configuration functions will be rewritten as lambda functions
     and all defined variables will act as arguments, e.g.:
     ``flagGeneric(func=(x != 4) & (y < 3))`` will be rewritten to
@@ -77,15 +80,14 @@
     def generic_visit(self, node):
         if not isinstance(node, self.SUPPORTED):
             raise TypeError(f"invalid expression: '{node}'")
         return super().generic_visit(node)
 
 
 class ConfigFunctionParser(ast.NodeVisitor):
-
     SUPPORTED_NODES = (
         ast.Call,
         ast.Num,
         ast.Str,
         ast.keyword,
         ast.NameConstant,
         ast.UnaryOp,
@@ -103,15 +105,14 @@
         self.kwargs = {}
 
     def parse(self, node):
         func = self.visit_Call(node)
         return func, self.kwargs
 
     def visit_Call(self, node):
-
         if not isinstance(node, ast.Call):
             raise TypeError("expected function call")
 
         if node.args:
             raise TypeError("only keyword arguments are supported")
 
         if isinstance(node.func, ast.Attribute):
@@ -122,30 +123,44 @@
         if func_name not in FUNC_MAP:
             raise NameError(f"unknown function '{func_name}'")
 
         self.generic_visit(node)
         return func_name
 
     def visit_keyword(self, node):
-
         key, value = node.arg, node.value
         check_tree = True
 
+        imports = {}
         if key == "func":
-            visitor = ConfigExpressionParser(value)
-            args = ast.arguments(
-                posonlyargs=[],
-                kwonlyargs=[],
-                kw_defaults=[],
-                defaults=[],
-                args=[ast.arg(arg=a, annotation=None) for a in visitor.args],
-                kwarg=None,
-                vararg=None,
-            )
-            value = ast.Lambda(args=args, body=value)
+            if (isinstance(value, ast.Name) and value.id in ENVIRONMENT) or (
+                isinstance(value, ast.Constant) and value.value in ENVIRONMENT
+            ):
+                func = ENVIRONMENT[
+                    value.id if isinstance(value, ast.Name) else value.value
+                ]
+                # handle the missing attribute for numpy.ufunc
+                module = getattr(func, "__module__", "numpy")
+                if module.startswith("saqc"):
+                    # if it's an saqc function, we need to import the top level package first
+                    imports["saqc"] = importlib.import_module("saqc")
+                imports[module] = importlib.import_module(module)
+                value = ast.parse(f"{module}.{func.__name__}").body[0].value
+            else:
+                visitor = ConfigExpressionParser(value)
+                args = ast.arguments(
+                    posonlyargs=[],
+                    kwonlyargs=[],
+                    kw_defaults=[],
+                    defaults=[],
+                    args=[ast.arg(arg=a, annotation=None) for a in visitor.args],
+                    kwarg=None,
+                    vararg=None,
+                )
+                value = ast.Lambda(args=args, body=value)
             # NOTE:
             # don't pass the generated functions down
             # to the checks implemented in this class...
             check_tree = False
 
         vnode = ast.Assign(targets=[ast.Name(id=key, ctx=ast.Store())], value=value)
 
@@ -158,16 +173,15 @@
         # real python objects
         co = compile(
             ast.fix_missing_locations(ast.Interactive(body=[vnode])),
             "<ast>",
             mode="single",
         )
         # NOTE: only pass a copy to not clutter the ENVIRONMENT
-        # try:
-        exec(co, {**ENVIRONMENT}, self.kwargs)
+        exec(co, {**ENVIRONMENT, **imports}, self.kwargs)
 
         # let's do some more validity checks
         if check_tree:
             self.generic_visit(value)
 
     def generic_visit(self, node):
         if not isinstance(node, self.SUPPORTED_NODES):
```

### Comparing `saqc-2.3/saqc/funcs/breaks.py` & `saqc-2.4.0/saqc/funcs/breaks.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
-from saqc.constants import BAD, FILTER_ALL
-from saqc.core.register import _isflagged, flagging, register
-from saqc.funcs.changepoints import _assignChangePointCluster
+from saqc import BAD, FILTER_ALL
+from saqc.core import flagging, register
+from saqc.funcs.changepoints import _getChangePoints
+from saqc.lib.tools import isunflagged
 
 if TYPE_CHECKING:
     from saqc.core.core import SaQC
 
 
 class BreaksMixin:
     @register(mask=[], demask=[], squeeze=["field"])
@@ -38,37 +39,25 @@
         flag: float = BAD,
         dfilter: float = FILTER_ALL,
         **kwargs,
     ) -> "SaQC":
         """
         Flag NaNs in data.
 
-        By default only NaNs are flagged, that not already have a flag.
+        By default, only NaNs are flagged, that not already have a flag.
         `dfilter` can be used to pass a flag that is used as threshold.
         Each flag worse than the threshold is replaced by the function.
         This is, because the data gets masked (with NaNs) before the
         function evaluates the NaNs.
-
-        Parameters
-        ----------
-        field : str
-            Column(s) in flags and data.
-
-        flag : float, default BAD
-            Flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
         """
 
         datacol = self._data[field]
         mask = datacol.isna()
 
-        mask = ~_isflagged(self._flags[field], dfilter) & mask
+        mask = isunflagged(self._flags[field], dfilter) & mask
 
         self._flags[mask, field] = flag
         return self
 
     @flagging()
     def flagIsolated(
         self: "SaQC",
@@ -83,34 +72,24 @@
 
         The function flags arbitrarily large groups of values, if they are surrounded by
         sufficiently large data gaps. A gap is a timespan containing either no data at all
         or NaNs only.
 
         Parameters
         ----------
-        field : str
-            Column(s) in flags and data.
-
-        gap_window : str
+        gap_window :
             Minimum gap size required before and after a data group to consider it
             isolated. See condition (2) and (3)
 
-        group_window : str
+        group_window :
             Maximum size of a data chunk to consider it a candidate for an isolated group.
             Data chunks that are bigger than the ``group_window`` are ignored.
             This does not include the possible gaps surrounding it.
             See condition (1).
 
-        flag : float, default BAD
-            Flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
-
         Notes
         -----
         A series of values :math:`x_k,x_{k+1},...,x_{k+n}`, with associated
         timestamps :math:`t_k,t_{k+1},...,t_{k+n}`, is considered to be isolated, if:
 
         1. :math:`t_{k+1} - t_n <` `group_window`
         2. None of the :math:`x_j` with :math:`0 < t_k - t_j <` `gap_window`,
@@ -151,49 +130,43 @@
     def flagJumps(
         self: "SaQC",
         field: str,
         thresh: float,
         window: str,
         min_periods: int = 1,
         flag: float = BAD,
+        dfilter: float = FILTER_ALL,
         **kwargs,
     ) -> "SaQC":
         """
         Flag jumps and drops in data.
 
         Flag data where the mean of its values significantly changes (, where the data "jumps" from one value level to
         another).
         The changes in value level are detected by comparing the mean for two adjacently rolling windows.
         Whenever the difference between the mean in the two windows exceeds `thresh`, the value between the windows
         is flagged a jump.
 
-
         Parameters
         ----------
-        field : str
-            Column(s) in flags and data.
-
-        thresh : float
+        thresh :
             Threshold value by which the mean of data has to jump, to trigger flagging.
 
-        window : str
+        window :
             Size of the two moving windows. This determines the number of observations used
             for calculating the mean in every window.
             The window size should be big enough to yield enough samples for a reliable mean calculation,
             but it should also not be arbitrarily big, since it also limits the density of jumps that can be detected.
             More precisely: Jumps that are not distanced to each other by more than three fourth (3/4) of the
             selected window size, will not be detected reliably.
 
-        min_periods : int, default 1
+        min_periods :
             The minimum number of observations in window required to calculate a valid
             mean value.
 
-        flag : float, default BAD
-            Flag to set.
-
         Examples
         --------
 
         Below picture gives an abstract interpretation of the parameter interplay in case of a positive value jump,
         initialising a new mean level.
 
         .. figure:: /resources/images/flagJumpsPic.png
@@ -202,28 +175,20 @@
            the two windows differ by more than `thresh`, flagging is triggered.
 
         Notes
         -----
 
         Jumps that are not distanced to each other by more than three fourth (3/4) of the
         selected window size, will not be detected reliably.
-
-
-        Returns
-        -------
-        saqc.SaQC
-        """
-        self._data, self._flags = _assignChangePointCluster(
-            self._data,
-            field,
-            self._flags,
+        """
+        mask = _getChangePoints(
+            data=self._data[field],
             stat_func=lambda x, y: np.abs(np.mean(x) - np.mean(y)),
             thresh_func=lambda x, y: thresh,
             window=window,
             min_periods=min_periods,
-            set_flags=True,
-            model_by_resids=False,
-            assign_cluster=False,
-            flag=flag,
-            **kwargs,
+            result="mask",
         )
+
+        mask = isunflagged(self._flags[field], dfilter) & mask
+        self._flags[mask, field] = flag
         return self
```

### Comparing `saqc-2.3/saqc/funcs/changepoints.py` & `saqc-2.4.0/saqc/funcs/changepoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+import typing
 from typing import TYPE_CHECKING, Callable, Tuple
 
 import numba
 import numpy as np
 import pandas as pd
-from typing_extensions import Literal
 
-from dios import DictOfSeries
-from saqc.constants import BAD, UNFLAGGED
-from saqc.core.flags import Flags
-from saqc.core.register import flagging, register
-from saqc.lib.tools import customRoller, filterKwargs
+from saqc import BAD, UNFLAGGED
+from saqc.core import DictOfSeries, Flags, flagging, register
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 class ChangepointsMixin:
     @flagging()
     def flagChangePoints(
         self: "SaQC",
         field: str,
@@ -35,93 +32,76 @@
         min_periods: int | Tuple[int, int],
         reduce_window: str | None = None,
         reduce_func: Callable[[np.ndarray, np.ndarray], int] = lambda x, _: x.argmax(),
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
-        Flag data where it significantly changes.
+        Flag values that represent a system state transition.
 
-        Flag data points, where the parametrization of the process, the data is assumed to
-        generate by, significantly changes.
-
-        The change points detection is based on a sliding window search.
+        Flag data points, where the parametrization of the assumed process generating this data,
+        significantly changes.
 
         Parameters
         ----------
-        field : str
-            A column in flags and data.
-
-        stat_func : Callable
+        stat_func :
              A function that assigns a value to every twin window. The backward-facing
              window content will be passed as the first array, the forward-facing window
              content as the second.
 
-        thresh_func : Callable
+        thresh_func :
             A function that determines the value level, exceeding wich qualifies a
             timestamps func value as denoting a change-point.
 
-        window : str, tuple of str
+        window :
             Size of the moving windows. This is the number of observations used for
             calculating the statistic.
 
             If it is a single frequency offset, it applies for the backward- and the
             forward-facing window.
 
             If two offsets (as a tuple) is passed the first defines the size of the
             backward facing window, the second the size of the forward facing window.
 
-        min_periods : int or tuple of int
+        min_periods :
             Minimum number of observations in a window required to perform the changepoint
             test. If it is a tuple of two int, the first refer to the backward-,
             the second to the forward-facing window.
 
-        reduce_window : str or None, default None
+        reduce_window :
             The sliding window search method is not an exact CP search method and usually
             there wont be detected a single changepoint, but a "region" of change around
             a changepoint.
 
             If `reduce_window` is given, for every window of size `reduce_window`, there
             will be selected the value with index `reduce_func(x, y)` and the others will
             be dropped.
 
             If `reduce_window` is None, the reduction window size equals the twin window
             size, the changepoints have been detected with.
 
-        reduce_func : Callable, default ``lambda x, y: x.argmax()``
+        reduce_func : default argmax
             A function that must return an index value upon input of two arrays x and y.
             First input parameter will hold the result from the stat_func evaluation for
             every reduction window. Second input parameter holds the result from the
             `thresh_func` evaluation.
             The default reduction function just selects the value that maximizes the
             `stat_func`.
-
-        flag : float, default BAD
-            flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
         """
-        self._data, self._flags = _assignChangePointCluster(
-            self._data,
-            field,
-            self._flags,
+        mask = _getChangePoints(
+            data=self._data[field],
             stat_func=stat_func,
             thresh_func=thresh_func,
             window=window,
             min_periods=min_periods,
             reduce_window=reduce_window,
             reduce_func=reduce_func,
-            set_flags=True,
-            model_by_resids=False,
-            assign_cluster=False,
-            flag=flag,
-            **kwargs,
+            result="mask",
         )
+        self._flags[mask, field] = flag
         return self
 
     @register(mask=["field"], demask=[], squeeze=[])
     def assignChangePointCluster(
         self: "SaQC",
         field: str,
         stat_func: Callable[[np.ndarray, np.ndarray], float],
@@ -144,99 +124,85 @@
         Assigns label to the data, aiming to reflect continuous regimes of the processes
         the data is assumed to be generated by. The regime change points detection is
         based on a sliding window search.
 
 
         Parameters
         ----------
-        field : str
-            The reference variable, the deviation from wich determines the flagging.
-
-        stat_func : Callable[[numpy.array, numpy.array], float]
+        stat_func :
             A function that assigns a value to every twin window. Left window content will
             be passed to first variable,
             right window content will be passed to the second.
 
-        thresh_func : Callable[numpy.array, numpy.array], float]
+        thresh_func :
             A function that determines the value level, exceeding wich qualifies a
-            timestamps func func value as denoting a changepoint.
+            timestamps func value as denoting a changepoint.
 
-        window : str, tuple of string
+        window :
             Size of the rolling windows the calculation is performed in. If it is a single
             frequency offset, it applies for the backward- and the forward-facing window.
 
             If two offsets (as a tuple) is passed the first defines the size of the
             backward facing window, the second the size of the forward facing window.
 
-        min_periods : int or tuple of int
+        min_periods :
             Minimum number of observations in a window required to perform the changepoint
             test. If it is a tuple of two int, the first refer to the backward-,
             the second to the forward-facing window.
 
-        reduce_window : {None, str}, default None
+        reduce_window :
             The sliding window search method is not an exact CP search method and usually
-            there wont be detected a single changepoint, but a "region" of change around
+            there won't be detected a single changepoint, but a "region" of change around
             a changepoint. If `reduce_window` is given, for every window of size
             `reduce_window`, there will be selected the value with index `reduce_func(x,
             y)` and the others will be dropped. If `reduce_window` is None, the reduction
             window size equals the twin window size, the changepoints have been detected
             with.
 
-        reduce_func : callable, default lambda x,y: x.argmax()
+        reduce_func : default argmax
             A function that must return an index value upon input of two arrays x and y.
             First input parameter will hold the result from the stat_func evaluation for
             every reduction window. Second input parameter holds the result from the
             thresh_func evaluation. The default reduction function just selects the value
             that maximizes the stat_func.
 
-        model_by_resids : bool, default False
+        model_by_resids :
             If True, the results of `stat_funcs` are written, otherwise the regime labels.
-
-        Returns
-        -------
-        saqc.SaQC
         """
-        reserved = ["assign_cluster", "set_flags", "flag"]
-        kwargs = filterKwargs(kwargs, reserved)
-        self._data, self._flags = _assignChangePointCluster(
-            data=self._data,
-            field=field,
-            flags=self._flags,
+        rtyp = "residual" if model_by_resids else "cluster"
+        cluster = _getChangePoints(
+            data=self._data[field],
             stat_func=stat_func,
             thresh_func=thresh_func,
             window=window,
             min_periods=min_periods,
             reduce_window=reduce_window,
             reduce_func=reduce_func,
-            model_by_resids=model_by_resids,
-            **kwargs,
-            # control args
-            assign_cluster=True,
-            set_flags=False,
+            result=rtyp,  # type: ignore
         )
+        self._data[field] = cluster
+        # we set flags here against our standard policy,
+        # which is not to overwrite existing flags
+        self._flags[:, field] = UNFLAGGED
         return self
 
 
-def _assignChangePointCluster(
-    data: DictOfSeries,
-    field: str,
-    flags: Flags,
+def _getChangePoints(
+    data: pd.Series,
     stat_func: Callable[[np.ndarray, np.ndarray], float],
     thresh_func: Callable[[np.ndarray, np.ndarray], float],
     window: str | Tuple[str, str],
     min_periods: int | Tuple[int, int],
     reduce_window: str | None = None,
     reduce_func: Callable[[np.ndarray, np.ndarray], float] = lambda x, _: x.argmax(),
-    model_by_resids: bool = False,
-    set_flags: bool = False,
-    assign_cluster: bool = True,
-    flag: float = BAD,
-    **kwargs,
-) -> Tuple[DictOfSeries, Flags]:
-    data_ser = data[field].dropna()
+    result: typing.Literal["cluster", "residual", "mask"] = "mask",
+) -> pd.Series:
+    orig_index = data.index
+    data = data.dropna()  # implicit copy
+
     if isinstance(window, (list, tuple)):
         bwd_window, fwd_window = window
     else:
         bwd_window = fwd_window = window
 
     if isinstance(window, (list, tuple)):
         bwd_min_periods, fwd_min_periods = min_periods
@@ -246,93 +212,120 @@
     if reduce_window is None:
         s = int(
             pd.Timedelta(bwd_window).total_seconds()
             + pd.Timedelta(fwd_window).total_seconds()
         )
         reduce_window = f"{s}s"
 
-    roller = customRoller(data_ser, window=bwd_window, min_periods=0)
-    bwd_start, bwd_end = roller.window_indexer.get_window_bounds(len(data_ser))
-
-    roller = customRoller(data_ser, window=fwd_window, forward=True, min_periods=0)
-    fwd_start, fwd_end = roller.window_indexer.get_window_bounds(len(data_ser))
+    for window in [fwd_window, bwd_window, reduce_window]:
+        if isinstance(window, int):
+            raise TypeError(
+                "all parameter defining a size of a window "
+                "must be time-offsets, not integer."
+            )
+
+    # find window bounds arrays..
+    num_index = pd.Series(range(len(data)), index=data.index, dtype=int)
+    # ... for the normal (backwards) case..
+    rolling = num_index.rolling(bwd_window, min_periods=0)
+    bwd_start = rolling.min().to_numpy(dtype=int)
+    bwd_end = rolling.max().to_numpy(dtype=int) + 1
+    # ... and aging for the forward case.
+    rolling = num_index[::-1].rolling(fwd_window, min_periods=0, closed="left")
+    fwd_start = rolling.min().fillna(len(num_index)).to_numpy(dtype=int)[::-1]
+    fwd_end = (rolling.max() + 1).fillna(len(num_index)).to_numpy(dtype=int)[::-1]
 
     min_mask = (fwd_end - fwd_start >= fwd_min_periods) & (
         bwd_end - bwd_start >= bwd_min_periods
     )
 
     fwd_end = fwd_end[min_mask]
     split = bwd_end[min_mask]
     bwd_start = bwd_start[min_mask]
-    masked_index = data_ser.index[min_mask]
+    masked_index = data.index[min_mask]
     check_len = len(fwd_end)
-    data_arr = data_ser.values
+    data_arr = data.values
 
+    # Please keep this as I sometimes need to disable jitting manually
+    # to make it work with my debugger :/
+    # --palmb
     try_to_jit = True
-    jit_sf = numba.jit(stat_func, nopython=True)
-    jit_tf = numba.jit(thresh_func, nopython=True)
-    try:
-        jit_sf(data_arr[bwd_start[0] : bwd_end[0]], data_arr[fwd_start[0] : fwd_end[0]])
-        jit_tf(data_arr[bwd_start[0] : bwd_end[0]], data_arr[fwd_start[0] : fwd_end[0]])
-        stat_func = jit_sf
-        thresh_func = jit_tf
-    except (numba.TypingError, numba.UnsupportedError, IndexError):
-        try_to_jit = False
+    if try_to_jit:
+        jit_sf = numba.jit(stat_func, nopython=True)
+        jit_tf = numba.jit(thresh_func, nopython=True)
+        try:
+            jit_sf(
+                data_arr[bwd_start[0] : bwd_end[0]], data_arr[fwd_start[0] : fwd_end[0]]
+            )
+            jit_tf(
+                data_arr[bwd_start[0] : bwd_end[0]], data_arr[fwd_start[0] : fwd_end[0]]
+            )
+            stat_func = jit_sf
+            thresh_func = jit_tf
+        except (numba.TypingError, numba.UnsupportedError, IndexError):
+            try_to_jit = False
 
     args = data_arr, bwd_start, fwd_end, split, stat_func, thresh_func, check_len
 
     if try_to_jit:
         stat_arr, thresh_arr = _slidingWindowSearchNumba(*args)
     else:
         stat_arr, thresh_arr = _slidingWindowSearch(*args)
 
     result_arr = stat_arr > thresh_arr
 
-    if model_by_resids:
-        residuals = pd.Series(np.nan, index=data[field].index)
+    if result == "residuals":
+        residuals = pd.Series(np.nan, index=orig_index)
         residuals[masked_index] = stat_arr
-        data[field] = residuals
-        flags[:, field] = UNFLAGGED
-        return data, flags
+        return residuals
 
     det_index = masked_index[result_arr]
     detected = pd.Series(True, index=det_index)
     if reduce_window:
-        l = detected.shape[0]
-        roller = customRoller(detected, window=reduce_window, min_periods=1)
-        start, end = roller.window_indexer.get_window_bounds(
-            num_values=l, min_periods=1, closed="both", center=True
-        )
+        length = len(detected)
+
+        # find window bounds arrays
+        num_index = pd.Series(range(length), index=detected.index, dtype=int)
+        rolling = num_index.rolling(window=reduce_window, closed="both", center=True)
+        start = rolling.min().to_numpy(dtype=int)
+        end = (rolling.max() + 1).to_numpy(dtype=int)
 
         detected = _reduceCPCluster(
-            stat_arr[result_arr], thresh_arr[result_arr], start, end, reduce_func, l
+            stat_arr[result_arr],
+            thresh_arr[result_arr],
+            start,
+            end,
+            reduce_func,
+            length,
         )
         det_index = det_index[detected]
 
-    # the changepoint is the point "after" the change - so detected index has to be shifted once with regard to the
-    # data index:
+    # The changepoint is the point "after" the change.
+    # So the detected index has to be shifted by one
+    # with regard to the data index.
     shifted = (
         pd.Series(True, index=det_index)
-        .reindex(data_ser.index, fill_value=False)
+        .reindex(data.index, fill_value=False)
         .shift(fill_value=False)
     )
     det_index = shifted.index[shifted]
 
-    if assign_cluster:
-        cluster = pd.Series(False, index=data[field].index)
-        cluster[det_index] = True
-        cluster = cluster.cumsum()
-        # (better to start cluster labels with number one)
-        cluster += 1
-        data[field] = cluster
-        flags[:, field] = UNFLAGGED
-
-    if set_flags:
-        flags[det_index, field] = flag
-    return data, flags
+    mask = pd.Series(False, index=orig_index)
+    mask[det_index] = True
+    if result == "mask":
+        return mask
+
+    cluster = mask.cumsum()
+    cluster += 1  # start cluster labels with one, not zero
+    if result == "cluster":
+        return cluster
+
+    raise ValueError(
+        f"'result' must be one of 'cluster', 'mask' or 'residuals' not {result}"
+    )
 
 
 @numba.jit(parallel=True, nopython=True)
 def _slidingWindowSearchNumba(
     data_arr, bwd_start, fwd_end, split, stat_func, thresh_func, num_val
 ):
     stat_arr = np.zeros(num_val)
```

### Comparing `saqc-2.3/saqc/funcs/constants.py` & `saqc-2.4.0/saqc/funcs/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 
 import operator
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
-from saqc.constants import BAD
-from saqc.core.register import flagging
-from saqc.lib.tools import customRoller, getFreqDelta, statPass
+from saqc import BAD
+from saqc.core import flagging
+from saqc.lib.rolling import removeRollingRamps
+from saqc.lib.tools import getFreqDelta, statPass
 from saqc.lib.ts_operators import varQC
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 class ConstantsMixin:
     @flagging()
     def flagConstants(
         self: "SaQC",
         field: str,
@@ -42,50 +43,55 @@
 
         Any interval of values y(t),...,y(t+n) is flagged, if:
          - (1): n > ``window``
          - (2): abs(y(t + i) - (t + j)) < `thresh`, for all i,j in [0, 1, ..., n]
 
         Parameters
         ----------
-        field : str
-            A column in flags and data.
-
-        thresh : float
+        thresh :
             Maximum total change allowed per window.
 
-        window : str | int
+        window :
             Size of the moving window. This is the number of observations used
             for calculating the statistic. Each window will be a fixed size.
             If its an offset then this will be the time period of each window.
             Each window will be a variable sized based on the observations included
             in the time-period.
-
-        flag : float, default BAD
-            Flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         if not isinstance(window, (str, int)):
             raise TypeError("window must be offset string or int.")
 
-        d = self._data[field]
+        d: pd.Series = self._data[field]
+
+        if not isinstance(window, int) and not pd.api.types.is_datetime64_any_dtype(
+            d.index
+        ):
+            raise ValueError(
+                f"A time based value for 'window' is only possible for variables "
+                f"with a datetime based index, but variable '{field}' has an index "
+                f"of dtype {d.index.dtype}. Use an integer window instead."
+            )
 
         # min_periods=2 ensures that at least two non-nan values are present
         # in each window and also min() == max() == d[i] is not possible.
-        kws = dict(window=window, min_periods=min_periods, expand=False)
+        min_periods = max(min_periods, 2)
 
         # 1. find starting points of consecutive constant values as a boolean mask
         # 2. fill the whole window with True's
-        rolling = customRoller(d, **kws)
+        rolling = d.rolling(window=window, min_periods=min_periods)
         starting_points_mask = rolling.max() - rolling.min() <= thresh
-        rolling = customRoller(starting_points_mask, **kws, forward=True)
+
+        removeRollingRamps(starting_points_mask, window=window, inplace=True)
+
+        # mimic forward rolling by roll over inverse [::-1]
+        rolling = starting_points_mask[::-1].rolling(
+            window=window, min_periods=min_periods
+        )
         # mimic any()
-        mask = (rolling.sum() > 0) & d.notna()
+        mask = (rolling.sum()[::-1] > 0) & d.notna()
 
         self._flags[mask, field] = flag
         return self
 
     @flagging()
     def flagByVariance(
         self: "SaQC",
@@ -106,40 +112,30 @@
         Any interval of values y(t),..y(t+n) is flagged, if:
 
         (1) n > `window`
         (2) variance(y(t),...,y(t+n) < `thresh`
 
         Parameters
         ----------
-        field : str
-            A column in flags and data.
-
-        window : str | int
+        window :
             Size of the moving window. This is the number of observations used
             for calculating the statistic. Each window will be a fixed size.
             If its an offset then this will be the time period of each window.
             Each window will be sized, based on the number of observations included
             in the time-period.
 
-        thresh : float, default 0.0005
+        thresh :
             Maximum total variance allowed per window.
 
-        maxna : int, default None
+        maxna :
             Maximum number of NaNs allowed in window.
             If more NaNs are present, the window is not flagged.
 
-        maxna_group : int, default None
+        maxna_group :
             Same as `maxna` but for consecutive NaNs.
-
-        flag : float, default BAD
-            Flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         dataseries = self._data[field]
         delta = getFreqDelta(dataseries.index)
         if not delta:
             raise IndexError("Timeseries irregularly sampled!")
 
         if maxna is None:
```

### Comparing `saqc-2.3/saqc/funcs/curvefit.py` & `saqc-2.4.0/saqc/funcs/curvefit.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,31 +9,29 @@
 
 from typing import TYPE_CHECKING, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
-from dios import DictOfSeries
-from saqc.core.flags import Flags
-from saqc.core.register import register
+from saqc.core import DictOfSeries, Flags, register
 from saqc.lib.tools import getFreqDelta
 from saqc.lib.ts_operators import (
     butterFilter,
     polyRoller,
     polyRollerIrregular,
     polyRollerNoMissing,
     polyRollerNoMissingNumba,
     polyRollerNumba,
 )
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
-_FILL_METHODS = Literal[
+FILL_METHODS = Literal[
     "linear",
     "nearest",
     "zero",
     "slinear",
     "quadratic",
     "cubic",
     "spline",
@@ -70,39 +68,32 @@
         Note, that the initial and final window/2 values do not get fitted.
 
         Each residual gets assigned the worst flag present in the interval of
         the original data.
 
         Parameters
         ----------
-        field : str
-             A column in flags and data.
-
-        window : str, int
+        window :
             Size of the window you want to use for fitting. If an integer is passed,
             the size refers to the number of periods for every fitting window. If an
             offset string is passed, the size refers to the total temporal extension. The
             window will be centered around the vaule-to-be-fitted. For regularly sampled
             data always a odd number of periods will be used for the fit (periods-1 if
             periods is even).
 
-        order : int
+        order :
             Degree of the polynomial used for fitting
 
-        min_periods : int or None, default 0
+        min_periods :
             Minimum number of observations in a window required to perform the fit,
             otherwise NaNs will be assigned.
             If ``None``, `min_periods` defaults to 1 for integer windows and to the
             size of the window for offset based windows.
             Passing 0, disables the feature and will result in over-fitting for too
             sparse windows.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         self._data, self._flags = _fitPolynomial(
             data=self._data,
             field=field,
             flags=self._flags,
             window=window,
             order=order,
@@ -114,45 +105,40 @@
     @register(mask=["field"], demask=[], squeeze=[])
     def fitLowpassFilter(
         self: "SaQC",
         field: str,
         cutoff: float | str,
         nyq: float = 0.5,
         filter_order: int = 2,
-        fill_method: _FILL_METHODS = "linear",
+        fill_method: FILL_METHODS = "linear",
         **kwargs,
-    ):
+    ) -> "SaQC":
         """
         Fits the data using the butterworth filter.
 
         Note
         ----
         The data is expected to be regularly sampled.
 
         Parameters
         ----------
-        field: str
-            A column in flags and data.
-
-        cutoff: {float, str}
+        cutoff :
             The cutoff-frequency, either an offset freq string, or expressed in multiples of the sampling rate.
 
-        nyq: float
+        nyq :
             The niquist-frequency. expressed in multiples if the sampling rate.
 
-        fill_method: Literal[‘nearest’, ‘zero’, ‘slinear’, ‘quadratic’, ‘cubic’, ‘spline’, ‘barycentric’, ‘polynomial’]
+        fill_method :
             Fill method to be applied on the data before filtering (butterfilter cant
             handle ''np.nan''). See documentation of pandas.Series.interpolate method for
             details on the methods associated with the different keywords.
 
-        filter_type: Literal["lowpass", "highpass", "bandpass", "bandstop"]
+        filter_type :
             The type of filter. Default is ‘lowpass’.
-
         """
-
         self._data[field] = butterFilter(
             self._data[field],
             cutoff=cutoff,
             nyq=nyq,
             filter_order=filter_order,
             fill_method=fill_method,
             filter_type="lowpass",
@@ -165,61 +151,43 @@
     field: str,
     flags: Flags,
     window: Union[int, str],
     order: int,
     min_periods: int = 0,
     **kwargs,
 ) -> Tuple[DictOfSeries, Flags]:
-
     # TODO: some (rather large) parts are functional similar to saqc.funcs.rolling.roll
     if data[field].empty:
         return data, flags
 
     to_fit = data[field].copy()
     regular = getFreqDelta(to_fit.index)
     if not regular:
         if isinstance(window, int):
             raise NotImplementedError(
                 "Integer based window size is not supported for not-harmonized"
                 "sample series."
             )
         # get interval centers
-        centers = (
-            to_fit.rolling(
-                pd.Timedelta(window) / 2, closed="both", min_periods=min_periods
-            ).count()
-        ).floor()
+        centers = to_fit.rolling(
+            pd.Timedelta(window) / 2, closed="both", min_periods=min_periods
+        ).count()
         centers = centers.drop(centers[centers.isna()].index)
         centers = centers.astype(int)
         fitted = to_fit.rolling(
-            pd.Timedelta(window), closed="both", min_periods=min_periods
+            pd.Timedelta(window), closed="both", min_periods=min_periods, center=True
         ).apply(polyRollerIrregular, args=(centers, order))
-
-        def center_func(x, y=centers):
-            pos = x.index[int(len(x) - y[x.index[-1]])]
-            return y.index.get_loc(pos)
-
-        centers_iloc = (
-            centers.rolling(window, closed="both")
-            .apply(center_func, raw=False)
-            .astype(int)
-        )
-        temp = fitted.copy()
-        for k in centers_iloc.iteritems():
-            fitted.iloc[k[1]] = temp[k[0]]
-        fitted[fitted.index[0] : fitted.index[centers_iloc[0]]] = np.nan
-        fitted[fitted.index[centers_iloc[-1]] : fitted.index[-1]] = np.nan
     else:
         if isinstance(window, str):
             window = pd.Timedelta(window) // regular
         if window % 2 == 0:
             window = int(window - 1)
         if min_periods is None:
             min_periods = window
-        if to_fit.shape[0] < 200000:
+        if len(to_fit) < 200000:
             numba = False
         else:
             numba = True
 
         val_range = np.arange(0, window)
         center_index = window // 2
         if min_periods < window:
```

### Comparing `saqc-2.3/saqc/funcs/drift.py` & `saqc-2.4.0/saqc/funcs/drift.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,64 +2,67 @@
 
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
-
 from __future__ import annotations
 
 import functools
 import inspect
 from typing import TYPE_CHECKING, Callable, Optional, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import curve_fit
 from scipy.spatial.distance import pdist
 from typing_extensions import Literal
 
-from dios import DictOfSeries
-from saqc.constants import BAD
-from saqc.core.register import Flags, flagging, register
-from saqc.funcs.changepoints import _assignChangePointCluster
+from saqc import BAD
+from saqc.core import DictOfSeries, Flags, flagging, register
+from saqc.funcs.changepoints import _getChangePoints
+from saqc.lib.docs import DOC_TEMPLATES
 from saqc.lib.tools import detectDeviants, filterKwargs, toSequence
 from saqc.lib.ts_operators import expDriftModel, linearDriftModel
 from saqc.lib.types import CurveFitter
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 LinkageString = Literal[
     "single", "complete", "average", "weighted", "centroid", "median", "ward"
 ]
 
 MODELDICT = {"linear": linearDriftModel, "exponential": expDriftModel}
 
 
+def cityblock(x: np.ndarray | pd.Series, y: np.ndarray | pd.Series) -> np.ndarray:
+    return pdist(np.array([x, y]), metric="cityblock") / len(x)
+
+
 class DriftMixin:
     @register(
         mask=["field"],
         demask=["field"],
         squeeze=["field"],  # reference is written !
         multivariate=True,
         handles_target=False,
+        docstring=DOC_TEMPLATES["field"],
     )
     def flagDriftFromNorm(
         self: "SaQC",
         field: Sequence[str],
         freq: str,
         spread: float,
         frac: float = 0.5,
-        metric: Callable[[np.ndarray, np.ndarray], float] = lambda x, y: pdist(
-            np.array([x, y]), metric="cityblock"
-        )
-        / len(x),
+        metric: Callable[
+            [np.ndarray | pd.Series, np.ndarray | pd.Series], np.ndarray
+        ] = cityblock,
         method: LinkageString = "single",
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
         Flags data that deviates from an avarage data course.
 
@@ -67,45 +70,35 @@
         that members of a normal group must not exceed. In addition, only a group is considered
         "normal" if it contains more then `frac` percent of the variables in "field".
 
         See the Notes section for a more detailed presentation of the algorithm
 
         Parameters
         ----------
-        field : str
-            A column in flags and data.
-
-        freq : str
+        freq :
             Frequency, that split the data in chunks.
 
-        spread : float
+        spread :
             Maximum spread allowed in the group of *normal* data. See Notes section for more details.
 
-        frac : float, default 0.5
+        frac :
             Fraction defining the normal group. Use a value from the interval [0,1].
             The higher the value, the more stable the algorithm will be. For values below
             0.5 the results are undefined.
 
-        metric : Callable, default ``lambda x,y:pdist(np.array([x,y]),metric="cityblock")/len(x)``
+        metric : default cityblock
             Distance function that takes two arrays as input and returns a scalar float.
             This value is interpreted as the distance of the two input arrays.
             Defaults to the `averaged manhattan metric` (see Notes).
 
-        method : {"single", "complete", "average", "weighted", "centroid", "median", "ward"}, default "single"
+        method :
             Linkage method used for hierarchical (agglomerative) clustering of the data.
             `method` is directly passed to ``scipy.hierarchy.linkage``. See its documentation [1] for
             more details. For a general introduction on hierarchical clustering see [2].
 
-        flag : float, default BAD
-            flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
-
         Notes
         -----
         following steps are performed for every data "segment" of length `freq` in order to find the
         "abnormal" data:
 
         1. Calculate distances :math:`d(x_i,x_j)` for all :math:`x_i` in parameter `field`.
            (with :math:`d` denoting the distance function, specified by `metric`.
@@ -135,21 +128,20 @@
         Documentation of the underlying hierarchical clustering algorithm:
             [1] https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html
         Introduction to Hierarchical clustering:
             [2] https://en.wikipedia.org/wiki/Hierarchical_clustering
         """
         fields = toSequence(field)
 
-        data_to_flag = self._data[fields].to_df()
-        data_to_flag.dropna(inplace=True)
+        data = self._data[fields].to_pandas()
+        data.dropna(inplace=True)
 
-        segments = data_to_flag.groupby(pd.Grouper(freq=freq))
+        segments = data.groupby(pd.Grouper(freq=freq))
         for segment in segments:
-
-            if segment[1].shape[0] <= 1:
+            if len(segment[1]) <= 1:
                 continue
 
             drifters = detectDeviants(
                 segment[1], metric, spread, frac, method, "variables"
             )
 
             for var in drifters:
@@ -166,75 +158,59 @@
     )
     def flagDriftFromReference(
         self: "SaQC",
         field: Sequence[str],
         reference: str,
         freq: str,
         thresh: float,
-        metric: Callable[[np.ndarray, np.ndarray], float] = lambda x, y: pdist(
-            np.array([x, y]), metric="cityblock"
-        )
-        / len(x),
+        metric: Callable[
+            [np.ndarray | pd.Series, np.ndarray | pd.Series], np.ndarray
+        ] = cityblock,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
-        Flags data that deviates from a reference course.
-
-        The deviation is measured by a passed distance function.
+        Flags data that deviates from a reference course. Deviation is measured by a
+        custom distance function.
 
         Parameters
         ----------
-        field : str
-            A column in flags and data.
-
-        freq : str
+        freq :
             Frequency, that split the data in chunks.
 
-        reference : str
+        reference :
             Reference variable, the deviation is calculated from.
 
-        thresh : float
+        thresh :
             Maximum deviation from reference.
 
-        metric : Callable
+        metric : default cityblock
             Distance function. Takes two arrays as input and returns a scalar float.
             This value is interpreted as the mutual distance of the two input arrays.
             Defaults to the `averaged manhattan metric` (see Notes).
 
-        target : None
-            Ignored.
-
-        flag : float, default BAD
-            Flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
-
         Notes
         -----
         It is advisable to choose a distance function, that can be well interpreted in
         the units dimension of the measurement and where the interpretation is invariant over the
         length of the data. That is, why, the "averaged manhatten metric" is set as the metric
         default, since it corresponds to the averaged value distance, two data sets have (as opposed
         by euclidean, for example).
         """
 
         fields = toSequence(field)
 
         if reference not in fields:
             fields.append(reference)
 
-        data_to_flag = self._data[fields].to_df().dropna()
+        data = self._data[fields].to_pandas().dropna()
 
-        segments = data_to_flag.groupby(pd.Grouper(freq=freq))
+        segments = data.groupby(pd.Grouper(freq=freq))
         for segment in segments:
-
-            if segment[1].shape[0] <= 1:
+            if len(segment[1]) <= 1:
                 continue
 
             for i in range(len(fields)):
                 dist = metric(
                     segment[1].iloc[:, i].values, segment[1].loc[:, reference].values
                 )
 
@@ -255,47 +231,41 @@
         """
         The function corrects drifting behavior.
 
         See the Notes section for an overview over the correction algorithm.
 
         Parameters
         ----------
-        field : str
-            Column in data and flags.
-
-        maintenance_field : str
+        maintenance_field :
             Column holding the support-points information.
             The data is expected to have the following form:
             The index of the series represents the beginning of a maintenance
             event, wheras the values represent its endings.
 
-        model : Callable or {'exponential', 'linear'}
-            A modelfunction describing the drift behavior, that is to be corrected.
-            Either use built-in exponential or linear drift model by passing a string, or pass a custom callable.
-            The model function must always contain the keyword parameters 'origin' and 'target'.
-            The starting parameter must always be the parameter, by wich the data is passed to the model.
-            After the data parameter, there can occure an arbitrary number of model calibration arguments in
-            the signature.
-            See the Notes section for an extensive description.
+        model :
+            A model function describing the drift behavior, that is to be corrected.
+            Either use built-in exponential or linear drift model by passing a string,
+            or pass a custom callable. The model function must always contain the keyword
+            parameters 'origin' and 'target'. The starting parameter must always be the
+            parameter, by wich the data is passed to the model. After the data parameter,
+            there can occure an arbitrary number of model calibration arguments in the
+            signature. See the Notes section for an extensive description.
 
-        cal_range : int, default 5
+        cal_range :
             Number of values to calculate the mean of, for obtaining the value level directly
             after and directly before a maintenance event. Needed for shift calibration.
 
-        Returns
-        -------
-        saqc.SaQC
-
         Notes
         -----
         It is assumed, that between support points, there is a drift effect shifting the
         meassurements in a way, that can be described, by a model function M(t, p, origin, target).
         (With 0<=t<=1, p being a parameter set, and origin, target being floats).
 
-        Note, that its possible for the model to have no free parameters p at all. (linear drift mainly)
+        Note, that its possible for the model to have no free parameters p at all
+        (linear drift mainly).
 
         The drift model, directly after the last support point (t=0),
         should evaluate to the origin - calibration level (origin), and directly before the next
         support point (t=1), it should evaluate to the target calibration level (target).
 
 
             M(0, p, origin, target) = origin
@@ -341,34 +311,34 @@
         if self._data[maintenance_field].empty:
             return self
 
         to_correct = self._data[field].copy()
         maint_data = self._data[maintenance_field].copy()
 
         to_correct_clean = to_correct.dropna()
-        d = {"drift_group": np.nan, to_correct.name: to_correct_clean.values}
+        d = {"drift_group": np.nan, field: to_correct_clean.values}
         drift_frame = pd.DataFrame(d, index=to_correct_clean.index)
 
         # group the drift frame
-        for k in range(0, maint_data.shape[0] - 1):
+        for k in range(0, len(maint_data) - 1):
             # assign group numbers for the timespans in between one maintenance ending and the beginning of the next
             # maintenance time itself remains np.nan assigned
             drift_frame.loc[
                 maint_data.values[k] : pd.Timestamp(maint_data.index[k + 1]),
                 "drift_group",
             ] = k
 
         # define target values for correction
         drift_grouper = drift_frame.groupby("drift_group")
         shift_targets = drift_grouper.aggregate(lambda x: x[:cal_range].mean()).shift(
             -1
         )
 
         for k, group in drift_grouper:
-            data_series = group[to_correct.name]
+            data_series = group[field]
             data_fit, data_shiftTarget = _driftFit(
                 data_series, shift_targets.loc[k, :][0], cal_range, model
             )
             data_fit = pd.Series(data_fit, index=group.index)
             data_shiftTarget = pd.Series(data_shiftTarget, index=group.index)
             data_shiftVektor = data_shiftTarget - data_fit
             shiftedData = data_series + data_shiftVektor
@@ -390,46 +360,45 @@
     ) -> "SaQC":
         """
         Function fits the passed model to the different regimes in data[field] and tries to correct
         those values, that have assigned a negative label by data[cluster_field].
 
         Currently, the only correction mode supported is the "parameter propagation."
 
-        This means, any regime :math:`z`, labeled negatively and being modeled by the parameters p, gets corrected via:
+        This means, any regime :math:`z`, labeled negatively and being modeled by the parameters
+        p, gets corrected via:
 
         :math:`z_{correct} = z + (m(p^*) - m(p))`,
 
-        where :math:`p^*` denotes the parameter set belonging to the fit of the nearest not-negatively labeled cluster.
+        where :math:`p^*` denotes the parameter set belonging to the fit of the nearest
+        not-negatively labeled cluster.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the data column, you want to correct.
-
-        cluster_field : str
-            A string denoting the field in data, holding the cluster label for the data you want to correct.
+        cluster_field :
+            A string denoting the field in data, holding the cluster label for the data you want
+            to correct.
 
-        model : Callable
+        model :
             The model function to be fitted to the regimes.
-            It must be a function of the form :math:`f(x, *p)`, where :math:`x` is the ``numpy.array`` holding the
-            independent variables and :math:`p` are the model parameters that are to be obtained by fitting.
-            Depending on the `x_date` parameter, independent variable x will either be the timestamps
-            of every regime transformed to seconds from epoch, or it will be just seconds, counting the regimes length.
+            It must be a function of the form :math:`f(x, *p)`, where :math:`x` is the
+            ``numpy.array`` holding the independent variables and :math:`p` are the model
+            parameters that are to be obtained by fitting. Depending on the `x_date` parameter,
+            independent variable x will either be the timestamps of every regime transformed to
+            seconds from epoch, or it will be just seconds, counting the regimes length.
 
-        tolerance : {None, str}, default None:
+        tolerance :
             If an offset string is passed, a data chunk of length `offset` right at the
-            start and right at the end is ignored when fitting the model. This is to account for the
-            unreliability of data near the changepoints of regimes.
+            start and right at the end is ignored when fitting the model. This is to account
+            for the unreliability of data near the changepoints of regimes.
 
-        epoch : bool, default False
-            If True, use "seconds from epoch" as x input to the model func, instead of "seconds from regime start".
+        epoch :
+            If True, use "seconds from epoch" as x input to the model func, instead of
+            "seconds from regime start".
 
-        Returns
-        -------
-        saqc.SaQC
         """
         cluster_ser = self._data[cluster_field]
         unique_successive = pd.unique(cluster_ser.values)
         data_ser = self._data[field]
         regimes = data_ser.groupby(cluster_ser)
         para_dict = {}
         x_dict = {}
@@ -459,21 +428,21 @@
             x_dict[label] = xdata
             x_mask[label] = valid_mask
 
         first_normal = unique_successive > 0
         first_valid = np.array(
             [
                 ~pd.isna(para_dict[unique_successive[i]]).any()
-                for i in range(0, unique_successive.shape[0])
+                for i in range(0, len(unique_successive))
             ]
         )
         first_valid = np.where(first_normal & first_valid)[0][0]
         last_valid = 1
 
-        for k in range(0, unique_successive.shape[0]):
+        for k in range(0, len(unique_successive)):
             if unique_successive[k] < 0 & (
                 not pd.isna(para_dict[unique_successive[k]]).any()
             ):
                 ydata = data_ser[regimes.groups[unique_successive[k]]].values
                 xdata = x_dict[unique_successive[k]]
                 ypara = para_dict[unique_successive[k]]
                 if k > 0:
@@ -497,85 +466,85 @@
     def correctOffset(
         self: "SaQC",
         field: str,
         max_jump: float,
         spread: float,
         window: str,
         min_periods: int,
-        tolerance: Optional[str] = None,
+        tolerance: str | None = None,
         **kwargs,
     ) -> "SaQC":
         """
         Parameters
         ----------
-        field : str
-            The fieldname of the data column, you want to correct.
-
-        max_jump : float
+        max_jump :
             when searching for changepoints in mean - this is the threshold a mean difference in the
             sliding window search must exceed to trigger changepoint detection.
 
-        spread : float
+        spread :
             threshold denoting the maximum, regimes are allowed to abolutely differ in their means
             to form the "normal group" of values.
 
-        window : str
+        window :
             Size of the adjacent windows that are used to search for the mean changepoints.
 
-        min_periods : int
+        min_periods :
             Minimum number of periods a search window has to contain, for the result of the changepoint
             detection to be considered valid.
 
-        tolerance : {None, str}, default None:
+        tolerance :
             If an offset string is passed, a data chunk of length `offset` right from the
             start and right before the end of any regime is ignored when calculating a regimes mean for data correcture.
             This is to account for the unrelyability of data near the changepoints of regimes.
 
-        Returns
-        -------
-        saqc.SaQC
-        """
-        self = self.copyField(field, field + "_CPcluster")
-        self._data, self._flags = _assignChangePointCluster(
-            self._data,
-            field + "_CPcluster",
-            self._flags,
-            lambda x, y: np.abs(np.mean(x) - np.mean(y)),
-            lambda x, y: max_jump,
+        """
+        # Hint: This whole function does not set any flags
+
+        cluster_field = field + "_CPcluster"
+        self = self.copyField(field, cluster_field)
+        self.data[cluster_field] = _getChangePoints(
+            data=self._data[cluster_field],
+            stat_func=lambda x, y: np.abs(np.mean(x) - np.mean(y)),
+            thresh_func=lambda x, y: max_jump,
             window=window,
             min_periods=min_periods,
+            result="cluster",
         )
         self._data, self._flags = _assignRegimeAnomaly(
-            self._data, field, self._flags, field + "_CPcluster", spread
+            data=self._data,
+            field=field,
+            flags=self._flags,
+            cluster_field=cluster_field,
+            spread=spread,
         )
         self = self.correctRegimeAnomaly(
             field,
-            field + "_CPcluster",
+            cluster_field,
             lambda x, p1: np.array([p1] * x.shape[0]),
             tolerance=tolerance,
         )
-        self = self.dropField(field + "_CPcluster")
+        self = self.dropField(cluster_field)
         return self
 
     @flagging()
     def flagRegimeAnomaly(
         self: "SaQC",
         field: str,
         cluster_field: str,
         spread: float,
         method: LinkageString = "single",
-        metric: Callable[[np.ndarray, np.ndarray], float] = lambda x, y: np.abs(
-            np.nanmean(x) - np.nanmean(y)
-        ),
+        metric: Callable[
+            [np.ndarray | pd.Series, np.ndarray | pd.Series], float
+        ] = lambda x, y: np.abs(np.nanmean(x) - np.nanmean(y)),
         frac: float = 0.5,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
-        Flags anomalous regimes regarding to modelling regimes of field.
+        Flags anomalous regimes regarding to modelling regimes of ``field``.
 
         "Normality" is determined in terms of a maximum spreading distance,
         regimes must not exceed in respect to a certain metric and linkage method.
 
         In addition, only a range of regimes is considered "normal", if it models
         more then `frac` percentage of the valid samples in "field".
 
@@ -583,41 +552,31 @@
 
         Note, that it is possible to perform hypothesis tests for regime equality
         by passing the metric a function for p-value calculation and selecting linkage
         method "complete".
 
         Parameters
         ----------
-        field : str
-            Name of the column to process
-
-        cluster_field : str
+        cluster_field :
             Column in data, holding the cluster labels for the samples in field.
             (has to be indexed equal to field)
 
-        spread : float
+        spread :
             A threshold denoting the value level, up to wich clusters a agglomerated.
 
-        method : {"single", "complete", "average", "weighted", "centroid", "median", "ward"}, default "single"
+        method :
             The linkage method for hierarchical (agglomerative) clustering of the variables.
 
-        metric : Callable, default lambda x,y: np.abs(np.nanmean(x) - np.nanmean(y))
+        metric : default absolute difference of means
             A metric function for calculating the dissimilarity between 2 regimes.
             Defaults to the difference in mean.
 
-        frac : float
+        frac :
             Has to be in [0,1]. Determines the minimum percentage of samples,
             the "normal" group has to comprise to be the normal group actually.
-
-        flag : float, default BAD
-            flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         reserverd = ["set_cluster", "set_flags"]
         kwargs = filterKwargs(kwargs, reserverd)
         self._data, self._flags = _assignRegimeAnomaly(
             data=self._data,
             field=field,
             flags=self._flags,
@@ -660,38 +619,31 @@
 
         Note, that it is possible to perform hypothesis tests for regime equality by
         passing the metric a function for p-value calculation and selecting linkage
         method "complete".
 
         Parameters
         ----------
-        field : str
-            Name of the column to process
-
-        cluster_field : str
+        cluster_field :
             Column in data, holding the cluster labels for the samples in field.
             (has to be indexed equal to field)
 
-        spread : float
+        spread :
             A threshold denoting the value level, up to wich clusters a agglomerated.
 
-        method : {"single", "complete", "average", "weighted", "centroid", "median", "ward"}, default "single"
+        method :
             The linkage method for hierarchical (agglomerative) clustering of the variables.
 
-        metric : Callable, default lambda x,y: np.abs(np.nanmean(x) - np.nanmean(y))
+        metric : default absolute difference of means
             A metric function for calculating the dissimilarity between 2 regimes.
             Defaults to the difference in mean.
 
-        frac : float
+        frac :
             Has to be in [0,1]. Determines the minimum percentage of samples,
             the "normal" group has to comprise to be the normal group actually.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         reserverd = ["set_cluster", "set_flags", "flag"]
         kwargs = filterKwargs(kwargs, reserverd)
         self._data, self._flags = _assignRegimeAnomaly(
             data=self._data,
             field=field,
             flags=self._flags,
@@ -752,20 +704,20 @@
     set_cluster: bool = True,
     set_flags: bool = False,
     flag: float = BAD,
     **kwargs,
 ) -> Tuple[DictOfSeries, Flags]:
     series = data[cluster_field]
     cluster = np.unique(series)
-    cluster_dios = DictOfSeries({i: data[field][series == i] for i in cluster})
+    cluster_dios = DictOfSeries({str(i): data[field][series == i] for i in cluster})
     plateaus = detectDeviants(cluster_dios, metric, spread, frac, method, "samples")
 
     if set_flags:
-        for p in plateaus:
-            flags[cluster_dios.iloc[:, p].index, field] = flag
+        for p, cols in zip(plateaus, cluster_dios.columns[plateaus]):
+            flags[cluster_dios[cols].index, field] = flag
 
     if set_cluster:
         for p in plateaus:
             if cluster[p] > 0:
                 series[series == cluster[p]] = -cluster[p]
 
     data[cluster_field] = series
```

### Comparing `saqc-2.3/saqc/funcs/flagtools.py` & `saqc-2.4.0/saqc/funcs/flagtools.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,91 +3,56 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+import operator
 import warnings
-from typing import TYPE_CHECKING, Any, Union
+from typing import TYPE_CHECKING, Any, Callable, Sequence, Union
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
-from dios import DictOfSeries
-from saqc.constants import BAD, FILTER_ALL, UNFLAGGED
-from saqc.core.register import _isflagged, flagging, register
+from saqc import BAD, FILTER_ALL, UNFLAGGED
+from saqc.core import DictOfSeries, flagging, register
+from saqc.lib.tools import isflagged, toSequence
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 class FlagtoolsMixin:
     @flagging()
     def flagDummy(self: "SaQC", field: str, **kwargs) -> "SaQC":
         """
         Function does nothing but returning data and flags.
-
-        Parameters
-        ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-flagged.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         return self
 
     @register(mask=[], demask=[], squeeze=["field"])
     def forceFlags(self: "SaQC", field: str, flag: float = BAD, **kwargs) -> "SaQC":
         """
         Set whole column to a flag value.
 
-        Parameters
-        ----------
-        field : str
-            columns name that holds the data
-
-        flag : float, default BAD
-            flag to set
-
-        kwargs : dict
-            unused
-
-        Returns
-        -------
-        saqc.SaQC
-
         See Also
         --------
         clearFlags : set whole column to UNFLAGGED
         flagUnflagged : set flag value at all unflagged positions
         """
         self._flags[:, field] = flag
         return self
 
     @register(mask=[], demask=[], squeeze=["field"])
     def clearFlags(self: "SaQC", field: str, **kwargs) -> "SaQC":
         """
         Set whole column to UNFLAGGED.
 
-        Parameters
-        ----------
-        field : str
-            columns name that holds the data
-
-        kwargs : dict
-            unused
-
-        Returns
-        -------
-        saqc.SaQC
-
         Notes
         -----
         This function ignores the ``dfilter`` keyword, because the data is not relevant
         for processing.
         A warning is triggered if the ``flag`` keyword is given, because the flags are
         always set to `UNFLAGGED`.
 
@@ -105,48 +70,32 @@
         return self.forceFlags(field, flag=UNFLAGGED, **kwargs)
 
     @register(mask=[], demask=[], squeeze=["field"])
     def flagUnflagged(self: "SaQC", field: str, flag: float = BAD, **kwargs) -> "SaQC":
         """
         Function sets a flag at all unflagged positions.
 
-        Parameters
-        ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-flagged.
-
-        flag : float, default BAD
-            flag value to set
-
-        kwargs : Dict
-            unused
-
-        Returns
-        -------
-        saqc.SaQC
-
-        Notes
-        -----
-        This function ignores the ``dfilter`` keyword, because the data is not relevant
-        for processing.
-
         See Also
         --------
         clearFlags : set whole column to UNFLAGGED
         forceFlags : set whole column to a flag value
+
+        Notes
+        -----
+        This function ignores the ``dfilter`` keyword, because the data is not relevant for processing.
         """
         unflagged = self._flags[field].isna() | (self._flags[field] == UNFLAGGED)
         self._flags[unflagged, field] = flag
         return self
 
     @register(mask=["field"], demask=["field"], squeeze=["field"])
     def flagManual(
         self: "SaQC",
         field: str,
-        mdata: Union[pd.Series, pd.DataFrame, DictOfSeries, list, np.ndarray],
+        mdata: pd.Series | pd.DataFrame | DictOfSeries | list | np.ndarray,
         method: Literal[
             "left-open", "right-open", "closed", "plain", "ontime"
         ] = "left-open",
         mformat: Literal["start-end", "mflag"] = "start-end",
         mflag: Any = 1,
         flag: float = BAD,
         **kwargs,
@@ -157,22 +106,19 @@
         The data is flagged at locations where `mdata` is equal to a provided flag (`mflag`).
         The format of mdata can be an indexed object, like pd.Series, pd.Dataframe or dios.DictOfSeries,
         but also can be a plain list- or array-like.
         How indexed mdata is aligned to data is specified via the `method` parameter.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-flagged.
-
-        mdata : pd.Series, pd.DataFrame, DictOfSeries, str, list or np.ndarray
+        mdata :
             The Data determining, wich intervals are to be flagged, or a string, denoting under which field the data is
             accessable.
 
-        method : {'plain', 'ontime', 'left-open', 'right-open', 'closed'}, default 'plain'
+        method :
             Defines how mdata is projected on data. Except for the 'plain' method, the methods assume mdata to have an
             index.
 
             * 'plain': mdata must have the same length as data and is projected one-to-one on data.
             * 'ontime': works only with indexed mdata. mdata entries are matched with data entries that have the same index.
             * 'right-open': mdata defines intervals, values are to be projected on.
               The intervals are defined,
@@ -181,37 +127,31 @@
               (2) Or, a Series, where the index contains in the t1 timestamps nd the values the respective t2 stamps.
 
               The value at t_1 gets projected onto all data timestamps t with t_1 <= t < t_2.
 
             * 'left-open': like 'right-open', but the projected interval now covers all t with t_1 < t <= t_2.
             * 'closed': like 'right-open', but the projected interval now covers all t with t_1 <= t <= t_2.
 
-        mformat : {"start-end", "mflag"}, default "start-end"
+        mformat :
 
             * "start-end": mdata is a Series, where every entry indicates an interval to-flag. The index defines the left
               bound, the value defines the right bound.
             * "mflag": mdata is an array like, with entries containing 'mflag',where flags shall be set. See documentation
               for examples.
 
-        mflag : scalar
+        mflag :
             The flag that indicates data points in `mdata`, of wich the projection in data should be flagged.
 
-        flag : float, default BAD
-            flag to set.
-
-        Returns
-        -------
-        saqc.SaQC
-
         Examples
         --------
         An example for mdata
 
         .. doctest:: ExampleFlagManual
 
+           >>> import saqc
            >>> mdata = pd.Series([1, 0, 1], index=pd.to_datetime(['2000-02-01', '2000-03-01', '2000-05-01']))
            >>> mdata
            2000-02-01    1
            2000-03-01    0
            2000-05-01    1
            dtype: int64
 
@@ -226,41 +166,41 @@
            >>> qc = qc.flagManual('daily_data', mdata, mflag=1, mformat='mdata', method='ontime')
            >>> qc.flags['daily_data'] > UNFLAGGED
            2000-01-31    False
            2000-02-01     True
            2000-02-02    False
            2000-03-01    False
            2000-05-01     True
-           Name: daily_data, dtype: bool
+           dtype: bool
 
         With the 'right-open' method, the mdata is forward fill:
 
         .. doctest:: ExampleFlagManual
 
            >>> qc = qc.flagManual('daily_data', mdata, mflag=1, mformat='mdata', method='right-open')
            >>> qc.flags['daily_data'] > UNFLAGGED
            2000-01-31    False
            2000-02-01     True
            2000-02-02     True
            2000-03-01    False
            2000-05-01     True
-           Name: daily_data, dtype: bool
+           dtype: bool
 
         With the 'left-open' method, backward filling is used:
 
         .. doctest:: ExampleFlagManual
 
            >>> qc = qc.flagManual('daily_data', mdata, mflag=1, mformat='mdata', method='left-open')
            >>> qc.flags['daily_data'] > UNFLAGGED
            2000-01-31    False
            2000-02-01     True
            2000-02-02     True
            2000-03-01     True
            2000-05-01     True
-           Name: daily_data, dtype: bool
+           dtype: bool
         """
         dat = self._data[field]
         # internal not-mflag-value -> cant go for np.nan
         not_mflag = -1 if mflag == 0 else 0
         if isinstance(mdata, str):
             mdata = self._data[mdata]
 
@@ -333,72 +273,60 @@
         field: str,
         target: str,
         **kwargs,
     ) -> "SaQC":
         """
         Transfer Flags of one variable to another.
 
-        Parameters
-        ----------
-
-        field : str or List of str
-           Variable or list of variables, the flags of which are to be transferred.
-
-        target : str or List of str
-            Variable or list of variables, the flags of `field` are to be transferred to.
-
-        Returns
-        -------
-        saqc.SaQC
-
         See Also
         --------
         * :py:meth:`saqc.SaQC.flagGeneric`
         * :py:meth:`saqc.SaQC.concatFlags`
 
         Examples
         --------
         First, generate some data with some flags:
 
         .. doctest:: exampleTransfer
 
+           >>> import saqc
            >>> data = pd.DataFrame({'a': [1, 2], 'b': [1, 2], 'c': [1, 2]})
            >>> qc = saqc.SaQC(data)
            >>> qc = qc.flagRange('a', max=1.5)
-           >>> qc.flags.to_df()
-           columns      a    b    c
-           0         -inf -inf -inf
-           1        255.0 -inf -inf
+           >>> qc.flags.to_pandas()
+                  a    b    c
+           0   -inf -inf -inf
+           1  255.0 -inf -inf
 
         Now we can project the flag from `a` to `b` via
 
         .. doctest:: exampleTransfer
 
            >>> qc = qc.transferFlags('a', target='b')
-           >>> qc.flags.to_df()
-           columns      a      b    c
-           0         -inf   -inf -inf
-           1        255.0  255.0 -inf
+           >>> qc.flags.to_pandas()
+                  a      b    c
+           0   -inf   -inf -inf
+           1  255.0  255.0 -inf
 
         You can skip the explicit target parameter designation:
 
         .. doctest:: exampleTransfer
 
            >>> qc = qc.transferFlags('a', 'b')
 
         To project the flags of `a` to both the variables `b` and `c` in one call, align the field and target variables in
         2 lists:
 
         .. doctest:: exampleTransfer
 
            >>> qc = qc.transferFlags(['a','a'], ['b', 'c'])
-           >>> qc.flags.to_df()
-           columns      a      b      c
-           0         -inf   -inf   -inf
-           1        255.0  255.0  255.0
+           >>> qc.flags.to_pandas()
+                  a      b      c
+           0   -inf   -inf   -inf
+           1  255.0  255.0  255.0
         """
         import warnings
 
         warnings.warn(
             f"""The method 'transferFlags' is deprecated and
             will be removed in version 2.5 of SaQC. Please use
             'SaQC.concatFlags(field={field}, target={target}, method="match", squeeze=False)'
@@ -407,127 +335,248 @@
         )
         return self.concatFlags(field, target=target, method="match", squeeze=False)
 
     @flagging()
     def propagateFlags(
         self: "SaQC",
         field: str,
-        window: Union[str, int],
+        window: str | int,
         method: Literal["ffill", "bfill"] = "ffill",
         flag: float = BAD,
         dfilter: float = FILTER_ALL,
         **kwargs,
     ) -> "SaQC":
         """
         Flag values before or after flags set by the last test.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-flagged.
-
-        window : int, str
+        window :
             Size of the repetition window. An integer defines the exact number of repetitions,
             strings are interpreted as time offsets to fill with .
 
-        method : {"ffill", "bfill"}
+        method :
             Direction of repetetion. With "ffill" the subsequent values receive the flag to
             repeat, with "bfill" the previous values.
 
-        flag : float, default BAD
-            Flag to set.
-
-        dfilter : float, default FILTER_ALL
-            Threshold flag.
-
-        Returns
-        -------
-        saqc.SaQC
-
         Examples
         --------
         First, generate some data and some flags:
 
         .. doctest:: propagateFlags
 
+           >>> import saqc
            >>> data = pd.DataFrame({"a": [-3, -2, -1, 0, 1, 2, 3]})
            >>> flags = pd.DataFrame({"a": [-np.inf, -np.inf, -np.inf, 255.0, -np.inf, -np.inf, -np.inf]})
            >>> qc = saqc.SaQC(data=data, flags=flags)
            >>> qc.flags["a"]
            0     -inf
            1     -inf
            2     -inf
            3    255.0
            4     -inf
            5     -inf
            6     -inf
-           Name: a, dtype: float64
+           dtype: float64
 
         Now, to repeat the flag '255.0' two times in direction of ascending indices, execute:
 
         .. doctest:: propagateFlags
 
            >>> qc.propagateFlags('a', window=2, method="ffill").flags["a"]
            0     -inf
            1     -inf
            2     -inf
            3    255.0
            4    255.0
            5    255.0
            6     -inf
-           Name: a, dtype: float64
+           dtype: float64
 
         Choosing "bfill" will result in
 
         .. doctest:: propagateFlags
 
            >>> qc.propagateFlags('a', window=2, method="bfill").flags["a"]
            0     -inf
            1    255.0
            2    255.0
            3    255.0
            4     -inf
            5     -inf
            6     -inf
-           Name: a, dtype: float64
+           dtype: float64
 
         If an explicit flag is passed, it will be used to fill the repetition window
 
         .. doctest:: propagateFlags
 
            >>> qc.propagateFlags('a', window=2, method="bfill", flag=111).flags["a"]
            0     -inf
            1    111.0
            2    111.0
            3    255.0
            4     -inf
            5     -inf
            6     -inf
-           Name: a, dtype: float64
+           dtype: float64
         """
 
         if method not in {"bfill", "ffill"}:
             raise ValueError(f"supported methods are 'bfill', 'ffill', got '{method}'")
 
         # get the last history column
         hc = self._flags.history[field].hist.iloc[:, -1].astype(float)
 
         if method == "bfill":
             hc = hc[::-1]
 
         # get dfilter from meta or get of rid of this and
         # consider everything != np.nan as flag
-        flagged = _isflagged(hc, dfilter)
+        flagged = isflagged(hc, dfilter)
 
         repeated = (
             flagged.rolling(window, min_periods=1, closed="left")
             .max()
             .fillna(0)
             .astype(bool)
         )
 
         if method == "bfill":
             repeated = repeated[::-1]
 
         self._flags[repeated, field] = flag
 
         return self
+
+    @register(
+        mask=["field"],
+        demask=["field"],
+        squeeze=["field"],
+        multivariate=True,
+        handles_target=True,
+    )
+    def andGroup(
+        self: "SaQC",
+        field: str | list[str],
+        group: Sequence["SaQC"] | dict["SaQC", str | Sequence[str]] | None = None,
+        target: str | None = None,
+        flag: float = BAD,
+        **kwargs,
+    ) -> "SaQC":
+        """
+        Flag all values, if all of the given ``field`` values are already flagged.
+
+        Parameters
+        ----------
+        group:
+            A collection of ``SaQC`` objects to check for flags, defaults to the current object.
+
+            1. If given as a sequence of ``SaQC`` objects, all objects are checked for flags of a
+               variable named :py:attr:`field`.
+            2. If given as dictionary the keys are interpreted as ``SaQC`` objects and the corresponding
+               values as variables of the respective ``SaQC`` object to check for flags.
+        """
+        return _groupOperation(
+            base=self,
+            field=field,
+            target=target,
+            func=operator.and_,
+            group=group,
+            flag=flag,
+            **kwargs,
+        )
+
+    @register(
+        mask=["field"],
+        demask=["field"],
+        squeeze=["field"],
+        multivariate=True,
+        handles_target=True,
+    )
+    def orGroup(
+        self: "SaQC",
+        field: str | list[str],
+        group: Sequence["SaQC"] | dict["SaQC", str | Sequence[str]] | None = None,
+        target: str | None = None,
+        flag: float = BAD,
+        **kwargs,
+    ) -> "SaQC":
+        """
+        Flag all values, if at least one of the given ``field`` values is already flagged.
+
+        Parameters
+        ----------
+        group:
+            A collection of ``SaQC`` objects to check for flags, defaults to the current object.
+
+            1. If given as a sequence of ``SaQC`` objects, all objects are checked for flags of a
+               variable named :py:attr:`field`.
+            2. If given as dictionary the keys are interpreted as ``SaQC`` objects and the corresponding
+               values as variables of the respective ``SaQC`` object to check for flags.
+        """
+        return _groupOperation(
+            base=self,
+            field=field,
+            target=target,
+            func=operator.or_,
+            group=group,
+            flag=flag,
+            **kwargs,
+        )
+
+
+def _groupOperation(
+    base: "SaQC",
+    field: str | list[str],
+    func: Callable[[pd.Series, pd.Series], pd.Series],
+    group: Sequence["SaQC"] | dict["SaQC", str | Sequence[str]] | None = None,
+    target: str | list[str] | None = None,
+    flag: float = BAD,
+    **kwargs,
+) -> "SaQC":
+    if target is None:
+        target = field
+    field, target = toSequence(field), toSequence(target)
+
+    if len(target) != 1 and len(target) != len(field):
+        raise ValueError(
+            "'target' needs to be a string or a sequence of the same length as 'field'"
+        )
+
+    # harmonise `group` to type dict[SaQC, list[str]]
+    if group is None:
+        group = {base: field}
+    if not isinstance(group, dict):
+        group = {base if isinstance(qc, str) else qc: field for qc in group}
+    for k, v in group.items():
+        group[k] = toSequence(v)
+
+    # generate mask
+    mask = pd.Series(dtype=bool)
+    dfilter = kwargs.get("dfilter", FILTER_ALL)
+    for qc, fields in group.items():
+        if set(field) - qc._flags.keys():
+            raise KeyError(
+                f"one or more variable(s) in {field} are missing in given SaQC object"
+            )
+        for f in fields:
+            flagged = isflagged(qc._flags[f], thresh=dfilter)
+            if mask.empty:
+                mask = flagged
+            mask = func(mask, flagged)
+
+    # initialize target(s)
+    if len(target) == 1:
+        if target[0] not in base._data:
+            base._data[target[0]] = pd.Series(np.nan, index=mask.index, name=target[0])
+            base._flags[target[0]] = pd.Series(np.nan, index=mask.index, name=target[0])
+    else:
+        for f, t in zip(field, target):
+            if t not in base._data:
+                base = base.copyField(field=f, target=t)
+
+    # write flags
+    for t in target:
+        base._flags[mask, t] = flag
+
+    return base
```

### Comparing `saqc-2.3/saqc/funcs/generic.py` & `saqc-2.4.0/saqc/funcs/generic.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,37 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Any, Protocol, Sequence
 
 import numpy as np
 import pandas as pd
 
-from dios import DictOfSeries
-from saqc.constants import BAD, ENVIRONMENT, FILTER_ALL
-from saqc.core.flags import Flags
-from saqc.core.history import History
-from saqc.core.register import _isflagged, _maskData, register
-from saqc.lib.tools import toSequence
-from saqc.lib.types import GenericFunction, PandasLike
+from saqc import BAD, FILTER_ALL
+from saqc.core import DictOfSeries, Flags, register
+from saqc.lib.tools import isAllBoolean, isflagged, isunflagged, toSequence
+from saqc.parsing.environ import ENVIRONMENT
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
-def _flagSelect(field, flags, label=None):
+class GenericFunction(Protocol):
+    __name__: str
+    __globals__: dict[str, Any]
+
+    def __call__(self, *args: pd.Series) -> pd.Series | pd.DataFrame | DictOfSeries:
+        ...  # pragma: no cover
+
+
+def _flagSelect(field: str, flags: Flags, label: str | None = None) -> pd.Series:
     if label is None:
         return flags[field]
 
     h_meta = flags.history[field].meta
     trg_col = None
 
     for idx, item in enumerate(h_meta):
@@ -41,223 +46,162 @@
     if trg_col is None:
         raise KeyError(f"no such label {label} for field {field}")
 
     out = flags.history[field].hist[trg_col].astype(float)
     return out.fillna(-np.inf)
 
 
-def _prepare(
-    data: DictOfSeries, flags: Flags, columns: Sequence[str], dfilter: float
-) -> Tuple[DictOfSeries, Flags]:
-    fchunk = Flags({f: flags[f] for f in columns})
-    for f in fchunk.columns:
-        fchunk.history[f] = flags.history[f]
-    dchunk, _ = _maskData(
-        data=data.loc[:, columns].copy(), flags=fchunk, columns=columns, thresh=dfilter
-    )
-    return dchunk, fchunk.copy()
-
-
 def _execGeneric(
     flags: Flags,
-    data: PandasLike,
+    data: pd.DataFrame | pd.Series | DictOfSeries,
     func: GenericFunction,
     dfilter: float = FILTER_ALL,
-) -> DictOfSeries:
-
+) -> DictOfSeries | pd.DataFrame | pd.Series:
     globs = {
-        "isflagged": lambda data, label=None: _isflagged(
+        "isflagged": lambda data, label=None: isflagged(
             _flagSelect(data.name, flags, label), thresh=dfilter
         ),
         **ENVIRONMENT,
     }
 
     func.__globals__.update(globs)
 
     if isinstance(data, pd.Series):
         data = data.to_frame()
 
-    out = func(*[data[c] for c in data.columns])
-    if pd.api.types.is_scalar(out):
-        raise ValueError(
+    # set series.name, because `isflagged` relies on it
+    cols = []
+    for c in data.columns:
+        data[c].name = c
+        cols.append(data[c])
+    return func(*cols)
+
+
+def _castResult(obj) -> DictOfSeries:
+    # Note: the actual keys aka. column names
+    # we use here to create a DictOfSeries
+    # are never used, and only exists temporary.
+
+    if isinstance(obj, pd.Series):
+        return DictOfSeries({"0": obj})
+    if pd.api.types.is_dict_like(obj):
+        # includes pd.Series and
+        # everything with keys and __getitem__
+        return DictOfSeries(obj)
+    if pd.api.types.is_list_like(obj):
+        # includes pd.Series and dict
+        return DictOfSeries({str(i): val for i, val in enumerate(obj)})
+
+    if pd.api.types.is_scalar(obj):
+        raise TypeError(
             "generic function should return a sequence object, "
-            f"got '{type(out)}' instead"
+            f"got '{type(obj)}' instead"
         )
-
-    return DictOfSeries(out)
+    raise TypeError(f"unprocessable result type {type(obj)}.")
 
 
 class GenericMixin:
     @register(
-        mask=[],
-        demask=[],
-        squeeze=[],
+        mask=["field"],
+        demask=["field"],
+        squeeze=["field", "target"],
         multivariate=True,
         handles_target=True,
     )
     def processGeneric(
         self: "SaQC",
         field: str | Sequence[str],
         func: GenericFunction,
         target: str | Sequence[str] | None = None,
         dfilter: float = FILTER_ALL,
         **kwargs,
     ) -> "SaQC":
         """
         Generate/process data with user defined functions.
 
-        Formally, what the function does, is the following:
-
-        1.  Let F be a Callable, depending on fields f_1, f_2,...f_K, (F = F(f_1, f_2,...f_K))
-            Than, for every timestamp t_i that occurs in at least one of the timeseries data[f_j] (outer join),
-            The value v_i is computed via:
-            v_i = data([f_1][t_i], data[f_2][t_i], ..., data[f_K][t_i]), if all data[f_j][t_i] do exist
-            v_i = ``np.nan``, if at least one of the data[f_j][t_i] is missing.
-        2.  The result is stored to ``data[target]``, if ``target`` is given or to ``data[field]`` otherwise
+        Call the given ``func`` on the variables given in ``field``.
 
         Parameters
         ----------
-        field : str or list of str
-            The variable(s) passed to func.
-
-        func : callable
+        func :
             Function to call on the variables given in ``field``. The return value will be written
             to ``target`` or ``field`` if the former is not given. This implies, that the function
             needs to accept the same number of arguments (of type pandas.Series) as variables given
             in ``field`` and should return an iterable of array-like objects with the same number
             of elements as given in ``target`` (or ``field`` if ``target`` is not specified).
 
-        target: str or list of str
-            The variable(s) to write the result of ``func`` to. If not given, the variable(s)
-            specified in ``field`` will be overwritten. If a ``target`` is not given, it will be
-            created.
-
-        flag: float, default ``np.nan``
-            The quality flag to set. The default ``np.nan`` states the general idea, that
-            ``processGeneric`` generates 'new' data without any flags.
-
-        dfilter: float, default ``FILTER_ALL``
-            Threshold flag. Flag values greater than ``dfilter`` indicate that the associated
-            data value is inappropiate for further usage.
-
-        Returns
-        -------
-        saqc.SaQC
-
         Note
-        -----
+        ----
         All the numpy functions are available within the generic expressions.
 
         Examples
         --------
         Compute the sum of the variables 'rainfall' and 'snowfall' and save the result to
         a (new) variable 'precipitation'
 
         >>> from saqc import SaQC
         >>> qc = SaQC(pd.DataFrame({'rainfall':[1], 'snowfall':[2]}, index=pd.DatetimeIndex([0])))
         >>> qc = qc.processGeneric(field=["rainfall", "snowfall"], target="precipitation", func=lambda x, y: x + y)
-        >>> qc.data.to_df()
-        columns     rainfall  snowfall  precipitation
+        >>> qc.data.to_pandas()
+                    rainfall  snowfall  precipitation
         1970-01-01         1         2              3
         """
 
         fields = toSequence(field)
         targets = fields if target is None else toSequence(target)
 
-        dchunk, fchunk = _prepare(self._data, self._flags, fields, dfilter)
+        dchunk, fchunk = self._data[fields].copy(), self._flags[fields].copy()
         result = _execGeneric(fchunk, dchunk, func, dfilter=dfilter)
-
-        meta = {
-            "func": "procGeneric",
-            "args": (field, target),
-            "kwargs": {
-                "func": func.__name__,
-                "dfilter": dfilter,
-                **kwargs,
-            },
-        }
+        result = _castResult(result)
 
         # update data & flags
         for i, col in enumerate(targets):
-
-            datacol = result.iloc[:, i]
+            datacol = result[result.columns[i]]
             self._data[col] = datacol
 
             if col not in self._flags:
-                self._flags.history[col] = History(datacol.index)
+                self._flags[col] = pd.Series(np.nan, index=datacol.index)
 
             if not self._flags[col].index.equals(datacol.index):
                 raise ValueError(
                     f"cannot assign function result to the existing variable {repr(col)} "
                     "because of incompatible indices, please choose another 'target'"
                 )
 
-            self._flags.history[col].append(
-                pd.Series(np.nan, index=datacol.index), meta
-            )
+            self._flags[:, col] = np.nan
 
         return self
 
     @register(
-        mask=[],
-        demask=[],
-        squeeze=[],
+        mask=["field"],
+        demask=["field"],
+        squeeze=["field", "target"],
         multivariate=True,
         handles_target=True,
     )
     def flagGeneric(
         self: "SaQC",
         field: str | Sequence[str],
         func: GenericFunction,
         target: str | Sequence[str] | None = None,
         flag: float = BAD,
-        dfilter: float = FILTER_ALL,
         **kwargs,
     ) -> "SaQC":
         """
-        Flag data with user defined functions.
+        Flag data based on a given function.
 
-        Formally, what the function does, is the following:
-        Let X be a Callable, depending on fields f_1, f_2,...f_K, (X = X(f_1, f_2,...f_K))
-        Than for every timestamp t_i in data[field]:
-        data[field][t_i] is flagged if X(data[f_1][t_i], data[f_2][t_i], ..., data[f_K][t_i]) is True.
+        Evaluate ``func`` on all variables given in ``field``.
 
         Parameters
         ----------
-        field : str or list of str
-            The variable(s) passed to func.
-
-        func : callable
-            Function to call on the variables given in ``field``. The function needs to accept the same
-            number of arguments (of type pandas.Series) as variables given in ``field`` and return an
-            iterable of array-like objects of with dtype bool and with the same number of elements as
-            given in ``target`` (or ``field`` if ``target`` is not specified). The function output
-            determines the values to flag.
-
-        target: str or list of str
-            The variable(s) to write the result of ``func`` to. If not given, the variable(s)
-            specified in ``field`` will be overwritten. If a ``target`` is not given, it will be
-            created.
-
-        flag: float, default ``BAD``
-            The quality flag to set. The default ``BAD`` states the general idea, that
-            ``processGeneric`` generates 'new' data without direct relation to the potentially
-            already present flags.
-
-        dfilter: float, default ``FILTER_ALL``
-            Threshold flag. Flag values greater than ``dfilter`` indicate that the associated
-            data value is inappropiate for further usage.
-
-        Returns
-        -------
-        saqc.SaQC
-
-        Note
-        -----
-        All the numpy functions are available within the generic expressions.
+        func :
+            Function to call. The function needs to accept the same number of arguments
+            (of type pandas.Series) as variables given in ``field`` and return an
+            iterable of array-like objects of data type ``bool`` with the same length as
+            ``target``.
 
         Examples
         --------
 
         .. testsetup:: exampleFlagGeneric
 
            qc = saqc.SaQC(pd.DataFrame({'temperature':[0], 'uncertainty':[0], 'rainfall':[0], 'fan':[0]}, index=pd.DatetimeIndex([0])))
@@ -279,55 +223,47 @@
         .. testcode:: exampleFlagGeneric
 
            qc = qc.flagGeneric(field="fan", target="temperature", func=lambda x: np.sqrt(x) < 7)
         """
 
         fields = toSequence(field)
         targets = fields if target is None else toSequence(target)
+        dfilter = kwargs.get("dfilter", BAD)
 
-        dchunk, fchunk = _prepare(self._data, self._flags, fields, dfilter)
+        dchunk, fchunk = self._data[fields].copy(), self._flags[fields].copy()
         result = _execGeneric(fchunk, dchunk, func, dfilter=dfilter)
+        result = _castResult(result)
 
         if len(targets) != len(result.columns):
             raise ValueError(
-                f"the generic function returned {len(result.columns)} field(s), but only {len(targets)} target(s) were given"
+                f"the generic function returned {len(result.columns)} field(s), "
+                f"but {len(targets)} target(s) were given"
             )
 
-        if not result.empty and not (result.dtypes == bool).all():
+        if not result.empty and not isAllBoolean(result):
             raise TypeError(f"generic expression does not return a boolean array")
 
-        meta = {
-            "func": "flagGeneric",
-            "args": (field, target),
-            "kwargs": {
-                "func": func.__name__,
-                "flag": flag,
-                "dfilter": dfilter,
-                **kwargs,
-            },
-        }
-
         # update flags & data
         for i, col in enumerate(targets):
-
-            maskcol = result.iloc[:, i]
+            mask = result[result.columns[i]]
 
             # make sure the column exists
             if col not in self._flags:
-                self._flags.history[col] = History(maskcol.index)
+                self._flags[col] = pd.Series(np.nan, index=mask.index)
+
+            # respect existing flags
+            mask = isunflagged(self._flags[col], thresh=dfilter) & mask
 
             # dummy column to ensure consistency between flags and data
             if col not in self._data:
-                self._data[col] = pd.Series(np.nan, index=maskcol.index)
-
-            flagcol = maskcol.replace({False: np.nan, True: flag}).astype(float)
+                self._data[col] = pd.Series(np.nan, index=mask.index, dtype=float)
 
             # we need equal indices to work on
-            if not self._flags[col].index.equals(maskcol.index):
+            if not self._flags[col].index.equals(mask.index):
                 raise ValueError(
                     f"cannot assign function result to the existing variable {repr(col)} "
                     "because of incompatible indices, please choose another 'target'"
                 )
 
-            self._flags.history[col].append(flagcol, meta)
+            self._flags[mask, col] = flag
 
         return self
```

### Comparing `saqc-2.3/saqc/funcs/noise.py` & `saqc-2.4.0/saqc/funcs/noise.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from typing import TYPE_CHECKING, Callable
 
 import numpy as np
 import pandas as pd
 
 from saqc.constants import BAD
 from saqc.core.register import flagging
-from saqc.lib.tools import statPass
+from saqc.lib.tools import isunflagged, statPass
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 class NoiseMixin:
     @flagging()
     def flagByStatLowPass(
         self: "SaQC",
         field: str,
@@ -32,48 +32,41 @@
         sub_window: str | pd.Timedelta | None = None,
         sub_thresh: float | None = None,
         min_periods: int | None = None,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
-        Flag *chunks* of length, `window`:
+        Flag data chunks of length ``window``, if:
 
-        1. If they excexceed `thresh` with regard to `stat`:
-        2. If all (maybe overlapping) *sub-chunks* of *chunk*, with length `sub_window`,
-           `excexceed `sub_thresh` with regard to `stat`:
+        1. they excexceed ``thresh`` with regard to ``func`` and
+        2. all (maybe overlapping) sub-chunks of the data chunks with length ``sub_window``,
+           exceed ``sub_thresh`` with regard to ``func``
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-flagged.
+        func :
+            Aggregation function applied on every chunk.
 
-        func: Callable[[np.array, pd.Series], float]
-            Function to aggregate chunk contnent with.
+        window :
+            Window (i.e. chunk) size.
 
-        window: str
-            Temporal extension of the chunks to test
+        thresh :
+            Threshold. A given chunk is flagged, if the return value of ``func`` excceeds ``thresh``.
 
-        thresh: float
-            Threshold, that triggers flagging, if exceeded by stat value.
+        sub_window :
+            Window size of sub chunks, that are additionally tested for exceeding ``sub_thresh``
+            with respect to ``func``.
 
-        sub_window: str, default None,
-            Window size of the sub chunks, that are additionally tested for exceeding
-            `sub_thresh` with respect to `stat`.
+        sub_thresh :
+            Threshold. A given sub chunk is flagged, if the return value of ``func` excceeds ``sub_thresh``.
 
-        sub_thresh: float, default None
-
-        min_periods: int, default None
-
-        flag : float, default BAD
-            flag to set
-
-        Returns
-        -------
-        saqc.SaQC
+        min_periods :
+            Minimum number of values needed in a chunk to perfom the test.
+            Ignored if ``window`` is an integer.
         """
 
         datcol = self._data[field]
         if not min_periods:
             min_periods = 0
         if not sub_thresh:
             sub_thresh = thresh
@@ -88,9 +81,10 @@
             window,
             thresh,
             operator.gt,
             sub_window,
             sub_thresh,
             min_periods,
         )
-        self._flags[to_set, field] = flag
+        mask = isunflagged(self._flags[field], kwargs["dfilter"]) & to_set
+        self._flags[mask, field] = flag
         return self
```

### Comparing `saqc-2.3/saqc/funcs/pattern.py` & `saqc-2.4.0/saqc/funcs/pattern.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import dtw
+import numpy as np
 import pandas as pd
 
-from saqc.constants import BAD
-from saqc.core.register import flagging
-from saqc.lib.tools import customRoller
+from saqc import BAD
+from saqc.core import flagging
+from saqc.lib.rolling import removeRollingRamps
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 def calculateDistanceByDTW(
     data: pd.Series, reference: pd.Series, forward=True, normalize=True
 ):
     """
     Calculate the DTW-distance of data to pattern in a rolling calculation.
@@ -65,34 +66,37 @@
     See Also
     --------
     flagPatternByDTW : flag data by DTW
     """
     if reference.hasnans or reference.empty:
         raise ValueError("reference must not have nan's and must not be empty.")
 
-    winsz = reference.index.max() - reference.index.min()
+    winsz: pd.Timedelta = reference.index.max() - reference.index.min()
     reference = reference.to_numpy()
 
     def isPattern(chunk):
-        return dtw.accelerated_dtw(chunk, reference, "euclidean")[0]
+        if forward:
+            return dtw.accelerated_dtw(chunk[::-1], reference, "euclidean")[0]
+        else:
+            return dtw.accelerated_dtw(chunk, reference, "euclidean")[0]
 
     # generate distances, excluding NaNs
-    rolling = customRoller(
-        data.dropna(), window=winsz, forward=forward, expand=False, closed="both"
-    )
-    distances: pd.Series = rolling.apply(isPattern, raw=True)
+    nonas = data.dropna()
+    rollover = nonas[::-1] if forward else nonas
+    arr = rollover.rolling(winsz, closed="both").apply(isPattern, raw=True).to_numpy()
+    distances = pd.Series(arr[::-1] if forward else arr, index=nonas.index)
+    removeRollingRamps(distances, window=winsz, inplace=True)
 
     if normalize:
         distances /= len(reference)
 
     return distances.reindex(index=data.index)  # reinsert NaNs
 
 
 class PatternMixin:
-
     # todo should we mask `reference` even if the func fail if reference has NaNs
     @flagging()
     def flagPatternByDTW(
         self: "SaQC",
         field,
         reference,
         max_distance=0.0,
@@ -110,48 +114,41 @@
         2. for each data chunk extracted from each window, a distance to the given pattern
            is calculated, by the dynamic time warping algorithm [1]
 
         3. if the distance is below the threshold, all the data in the window gets flagged
 
         Parameters
         ----------
-        field : str
-            The name of the data column
-
-        reference : str
+        reference :
             The name in `data` which holds the pattern. The pattern must not have NaNs,
             have a datetime index and must not be empty.
 
-        max_distance : float, default 0.0
+        max_distance :
             Maximum dtw-distance between chunk and pattern, if the distance is lower than
             ``max_distance`` the data gets flagged. With default, ``0.0``, only exact
             matches are flagged.
 
-        normalize : bool, default True
+        normalize :
             If `False`, return unmodified distances.
             If `True`, normalize distances by the number of observations of the reference.
             This helps to make it easier to find a good cutoff threshold for further
             processing. The distances then refer to the mean distance per datapoint,
             expressed in the datas units.
 
-        plot: bool, default False
+        plot :
             Show a calibration plot, which can be quite helpful to find the right threshold
             for `max_distance`. It works best with `normalize=True`. Do not use in automatic
             setups / pipelines. The plot show three lines:
 
             - data: the data the function was called on
             - distances: the calculated distances by the algorithm
             - indicator: have to distinct levels: `0` and the value of `max_distance`.
               If `max_distance` is `0.0` it defaults to `1`. Everywhere where the
               indicator is not `0` the data will be flagged.
 
-        Returns
-        -------
-        saqc.SaQC
-
         Notes
         -----
         The window size of the moving window is set to equal the temporal extension of the
         reference datas datetime index.
 
         References
         ----------
@@ -165,23 +162,20 @@
         distances = calculateDistanceByDTW(dat, ref, forward=True, normalize=normalize)
         winsz = ref.index.max() - ref.index.min()
 
         # prevent nan propagation
         distances = distances.fillna(max_distance + 1)
 
         # find minima filter by threshold
-        fw = customRoller(
-            distances, window=winsz, forward=True, closed="both", expand=True
-        )
-        bw = customRoller(distances, window=winsz, closed="both", expand=True)
-        minima = (fw.min() == bw.min()) & (distances <= max_distance)
+        fw_min = distances[::-1].rolling(window=winsz, closed="both").min()[::-1]
+        bw_min = distances.rolling(window=winsz, closed="both").min()
+        minima = (fw_min == bw_min) & (distances <= max_distance)
 
         # Propagate True's to size of pattern.
-        rolling = customRoller(minima, window=winsz, closed="both", expand=True)
-        mask = rolling.sum() > 0
+        mask = minima.rolling(window=winsz, closed="both").sum() > 0
 
         if plot:
             df = pd.DataFrame()
             df["data"] = dat
             df["distances"] = distances
             df["indicator"] = mask.astype(float) * (max_distance or 1)
             df.plot()
```

### Comparing `saqc-2.3/saqc/funcs/resampling.py` & `saqc-2.4.0/saqc/funcs/resampling.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #! /usr/bin/env python
 
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
-
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Optional, Union
+import warnings
+from typing import TYPE_CHECKING, Callable, Union
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
-from dios import DtItype
-from saqc.core.register import _isflagged, register
-from saqc.funcs.interpolation import _SUPPORTED_METHODS
-from saqc.lib.tools import evalFreqStr, filterKwargs, getFreqDelta
-from saqc.lib.ts_operators import aggregate2Freq, shift2Freq
+from saqc.constants import UNFLAGGED
+from saqc.core import register
+from saqc.core.history import History
+from saqc.lib.docs import DOC_TEMPLATES
+from saqc.lib.tools import filterKwargs, getFreqDelta, isflagged
+from saqc.lib.ts_operators import aggregate2Freq
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 METHOD2ARGS = {
     "inverse_fshift": ("backward", pd.Timedelta),
     "inverse_bshift": ("forward", pd.Timedelta),
     "inverse_nshift": ("nearest", lambda x: pd.Timedelta(x) / 2),
     "inverse_fagg": ("bfill", pd.Timedelta),
@@ -53,360 +54,235 @@
         Note, that the data only gets interpolated at those (regular) timestamps, that have a valid (existing and
         not-na) datapoint preceeding them and one succeeding them within freq range.
         Regular timestamp that do not suffice this condition get nan assigned AND The associated flag will be of value
         ``UNFLAGGED``.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-regularized.
-
-        freq : str
+        freq :
             An offset string. The frequency of the grid you want to interpolate your data at.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         reserved = ["method", "order", "limit", "downgrade"]
         kwargs = filterKwargs(kwargs, reserved)
         return self.interpolateIndex(field, freq, "time", **kwargs)
 
     @register(mask=["field"], demask=[], squeeze=[])
-    def interpolate(
-        self: "SaQC",
-        field: str,
-        freq: str,
-        method: _SUPPORTED_METHODS,
-        order: int = 1,
-        **kwargs,
-    ) -> "SaQC":
-        """
-        A method to "regularize" data by interpolating the data at regular timestamp.
-
-        A series of data is considered "regular", if it is sampled regularly (= having uniform sampling rate).
-
-        Interpolated values will get assigned the worst flag within freq-range.
-
-        There are available all the interpolations from the pandas.Series.interpolate method and they are called by
-        the very same keywords.
-
-        Note, that, to perform a timestamp aware, linear interpolation, you have to pass ``'time'`` as `method`,
-        and NOT ``'linear'``.
-
-        Note, that the data only gets interpolated at those (regular) timestamps, that have a valid (existing and
-        not-na) datapoint preceeding them and one succeeding them within freq range.
-        Regular timestamp that do not suffice this condition get nan assigned AND The associated flag will be of value
-        ``UNFLAGGED``.
-
-        Parameters
-        ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-regularized.
-
-        freq : str
-            An offset string. The frequency of the grid you want to interpolate your data at.
-
-        method : {"linear", "time", "nearest", "zero", "slinear", "quadratic", "cubic", "spline", "barycentric",
-            "polynomial", "krogh", "piecewise_polynomial", "spline", "pchip", "akima"}
-            The interpolation method you want to apply.
-
-        order : int, default 1
-            If your selected interpolation method can be performed at different *orders* - here you pass the desired
-            order.
-
-        Returns
-        -------
-        saqc.SaQC
-        """
-        reserved = ["limit", "downgrade"]
-        kwargs = filterKwargs(kwargs, reserved)
-        return self.interpolateIndex(field, freq, method=method, order=order, **kwargs)
-
-    @register(mask=["field"], demask=[], squeeze=[])
     def shift(
         self: "SaQC",
         field: str,
         freq: str,
         method: Literal["fshift", "bshift", "nshift"] = "nshift",
-        freq_check: Optional[Literal["check", "auto"]] = None,
         **kwargs,
     ) -> "SaQC":
         """
-        Function to shift data and flags to a regular (equidistant) timestamp grid, according to ``method``.
+        Shift data points and flags to a regular frequency grid.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-shifted.
+        freq :
+            Offset string. Sampling rate of the target frequency.
 
-        freq : str
-            An frequency Offset String that will be interpreted as the sampling rate you want the data to be shifted to.
+        method :
+            Method to propagate values:
 
-        method : {'fshift', 'bshift', 'nshift'}, default 'nshift'
-            Specifies how misaligned data-points get propagated to a grid timestamp.
-            Following choices are available:
-
-            * 'nshift' : every grid point gets assigned the nearest value in its range. (range = +/- 0.5 * `freq`)
-            * 'bshift' : every grid point gets assigned its first succeeding value, if one is available in
-              the succeeding sampling interval.
-            * 'fshift' : every grid point gets assigned its ultimately preceding value, if one is available in
-              the preceeding sampling interval.
-
-        freq_check : {None, 'check', 'auto'}, default None
-
-            * ``None`` : do not validate frequency-string passed to `freq`
-            * 'check' : estimate frequency and log a warning if estimate miss matches frequency string passed to `freq`,
-              or if no uniform sampling rate could be estimated
-            * 'auto' : estimate frequency and use estimate. (Ignores `freq` parameter.)
-
-        Returns
-        -------
-        saqc.SaQC
+            * 'nshift' : shift grid points to the nearest time stamp in the range = +/- 0.5 * ``freq``
+            * 'bshift' : shift grid points to the first succeeding time stamp (if any)
+            * 'fshift' : shift grid points to the last preceeding time stamp (if any)
         """
-        datcol = self._data[field]
-        if datcol.empty:
-            return self
-
-        freq = evalFreqStr(freq, freq_check, datcol.index)
-
-        # do the shift
-        datcol = shift2Freq(datcol, method, freq, fill_value=np.nan)
-
-        # do the shift on the history
-        kws = dict(method=method, freq=freq)
-
-        history = self._flags.history[field].apply(
-            index=datcol.index,
-            func_handle_df=True,
-            func=shift2Freq,
-            func_kws={**kws, "fill_value": np.nan},
+        warnings.warn(
+            f"""
+            The method `shift` is deprecated and will be removed with version 2.6 of saqc.
+            To achieve the same behavior please use:
+            `qc.align(field={field}, freq={freq}. method={method})`
+            """,
+            DeprecationWarning,
         )
 
-        self._flags.history[field] = history
-        self._data[field] = datcol
-        return self
+        return self.align(field=field, freq=freq, method=method, **kwargs)
 
     @register(mask=["field"], demask=[], squeeze=[])
     def resample(
         self: "SaQC",
         field: str,
         freq: str,
         func: Callable[[pd.Series], pd.Series] = np.mean,
         method: Literal["fagg", "bagg", "nagg"] = "bagg",
-        maxna: Optional[int] = None,
-        maxna_group: Optional[int] = None,
-        maxna_flags: Optional[int] = None,  # TODO: still a case ??
-        maxna_group_flags: Optional[int] = None,
-        flag_func: Callable[[pd.Series], float] = max,
-        freq_check: Optional[Literal["check", "auto"]] = None,
+        maxna: int | None = None,
+        maxna_group: int | None = None,
         **kwargs,
     ) -> "SaQC":
         """
-        Function to resample the data.
+        Resample data points and flags to a regular frequency.
 
-        The data will be sampled at regular (equidistant) timestamps aka. Grid points.
+        The data will be sampled to regular (equidistant) timestamps.
         Sampling intervals therefore get aggregated with a function, specified by
-        'func' parameter and the result gets projected onto the new timestamps with a
-        method, specified by "method". The following method (keywords) are available:
+        ``func``, the result is projected to the new timestamps using
+        ``method``. The following methods are available:
 
         * ``'nagg'``: all values in the range (+/- `freq`/2) of a grid point get
             aggregated with func and assigned to it.
         * ``'bagg'``: all values in a sampling interval get aggregated with func and
             the result gets assigned to the last grid point.
         * ``'fagg'``: all values in a sampling interval get aggregated with func and
             the result gets assigned to the next grid point.
 
-
-        Note, that. if possible, functions passed to func will get projected
-        internally onto pandas.resample methods, wich results in some reasonable
-        performance boost - however, for this to work, you should pass functions that
-        have the __name__ attribute initialised and the according methods name assigned
-        to it. Furthermore, you shouldnt pass numpys nan-functions (``nansum``,
-        ``nanmean``,...) because those for example, have ``__name__ == 'nansum'`` and
-        they will thus not trigger ``resample.func()``, but the slower ``resample.apply(
-        nanfunc)``. Also, internally, no nans get passed to the functions anyway,
-        so that there is no point in passing the nan functions.
+        Note
+        ----
+        For perfomance reasons, ``func`` will be mapped to pandas.resample methods,
+        if possible. However, for this to work, functions need an initialized
+        ``__name__`` attribute, holding the function's name. Furthermore, you should
+        not pass numpys nan-functions (``nansum``, ``nanmean``,...) because they
+        cannot be optimised and the handling of ``NaN`` is already taken care of.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-resampled.
+        freq :
+            Offset string. Sampling rate of the target frequency grid.
 
-        freq : str
-            An Offset String, that will be interpreted as the frequency you want to
-            resample your data with.
+        func : default mean
+            Aggregation function. See notes for performance considerations.
 
-        func : Callable
-            The function you want to use for aggregation.
-
-        method: {'fagg', 'bagg', 'nagg'}, default 'bagg'
+        method :
             Specifies which intervals to be aggregated for a certain timestamp. (preceding,
             succeeding or "surrounding" interval). See description above for more details.
 
-        maxna : {None, int}, default None
-            Maximum number NaNs in a resampling interval. If maxna is exceeded, the interval
-            is set entirely to NaN.
+        maxna :
+            Maximum number of allowed ``NaN``s in a resampling interval. If exceeded, the
+            entire interval is filled with ``NaN``.
 
-        maxna_group : {None, int}, default None
+        maxna_group :
             Same as `maxna` but for consecutive NaNs.
-
-        maxna_flags : {None, int}, default None
-            Same as `max_invalid`, only applying for the flags. The flag regarded
-            as "invalid" value, is the one passed to empty_intervals_flag (
-            default=``BAD``). Also this is the flag assigned to invalid/empty intervals.
-
-        maxna_group_flags : {None, int}, default None
-            Same as `maxna_flags`, only applying onto flags. The flag regarded as
-            "invalid" value, is the one passed to empty_intervals_flag. Also this is the
-            flag assigned to invalid/empty intervals.
-
-        flag_func : Callable, default: max
-            The function you want to aggregate the flags with. It should be capable of
-            operating on the flags dtype (usually ordered categorical).
-
-        freq_check : {None, 'check', 'auto'}, default None
-
-            * ``None``: do not validate frequency-string passed to `freq`
-            * ``'check'``: estimate frequency and log a warning if estimate miss matchs
-                frequency string passed to 'freq', or if no uniform sampling rate could be
-                estimated
-            * ``'auto'``: estimate frequency and use estimate. (Ignores `freq` parameter.)
-
-        Returns
-        -------
-        saqc.SaQC
         """
 
         datcol = self._data[field]
 
-        # workaround for #GL-333
-        if datcol.empty and self._data.itype in [None, DtItype]:
+        if datcol.empty:
+            # see for #GL-374
             datcol = pd.Series(index=pd.DatetimeIndex([]), dtype=datcol.dtype)
 
-        freq = evalFreqStr(freq, freq_check, datcol.index)
-
         datcol = aggregate2Freq(
             datcol,
             method,
             freq,
             func,
             fill_value=np.nan,
             max_invalid_total=maxna,
             max_invalid_consec=maxna_group,
         )
 
         kws = dict(
             method=method,
             freq=freq,
-            agg_func=flag_func,
+            agg_func=max,
             fill_value=np.nan,
-            max_invalid_total=maxna_flags,
-            max_invalid_consec=maxna_group_flags,
+            max_invalid_total=maxna,
+            max_invalid_consec=maxna_group,
         )
 
         history = self._flags.history[field].apply(
             index=datcol.index,
             func=aggregate2Freq,
             func_kws=kws,
         )
+        meta = {
+            "func": "resample",
+            "args": (),
+            "kwargs": {
+                "freq": freq,
+                "func": func,
+                "method": method,
+                "maxna": maxna,
+                "maxna_group": maxna_group,
+                **kwargs,
+            },
+        }
+        flagcol = pd.Series(UNFLAGGED, index=history.index)
+        history.append(flagcol, meta)
 
         self._data[field] = datcol
         self._flags.history[field] = history
         return self
 
     @register(
         mask=[],
         demask=[],
         squeeze=[],
         handles_target=True,  # target is mandatory in func, so its allowed
+        docstring={"target": DOC_TEMPLATES["target"]},
     )
     def concatFlags(
         self: "SaQC",
         field: str,
-        target: str,
+        target: str | None = None,
         method: Literal[
             "inverse_fagg",
             "inverse_bagg",
             "inverse_nagg",
             "inverse_fshift",
             "inverse_bshift",
             "inverse_nshift",
             "inverse_interpolation",
             "match",
+            "auto",
         ] = "match",
         freq: str | None = None,
         drop: bool = False,
         squeeze: bool = False,
         overwrite: bool = False,
         **kwargs,
     ) -> "SaQC":
         """
-        The Function appends flags history of ``fields`` to flags history of ``target``.
-        Before appending, columns in ``field`` history are projected onto the target index via ``method``
-
-        method: (field_flag associated with "field", source_flags associated with "source")
-
-        * 'inverse_nagg' - all target_flags within the range +/- freq/2 of a field_flag, get assigned this field flags value.
-           (if field_flag > target_flag)
+        Project flags/history of :py:attr:`field` to :py:attr:`target` and adjust to the frequeny grid
+        of :py:attr:`target` by 'undoing' former interpolation, shifting or resampling operations
 
-        * 'inverse_bagg' - all target_flags succeeding a field_flag within the range of "freq", get assigned this field flags
-           value. (if field_flag > target_flag)
-
-        * 'inverse_fagg' - all target_flags preceeding a field_flag within the range of "freq", get assigned this field flags
-           value. (if field_flag > target_flag)
-
-        * 'inverse_interpolation' - all target_flags within the range +/- freq of a field_flag, get assigned this source flags value.
-          (if field_flag > target_flag)
-
-        * 'inverse_nshift' - That target_flag within the range +/- freq/2, that is nearest to a field_flag, gets the source
-          flags value. (if field_flag > target_flag)
-
-        * 'inverse_bshift' - That target_flag succeeding a field flag within the range freq, that is nearest to a
-           field_flag, gets assigned this field flags value. (if field_flag > target_flag)
-
-        * 'inverse_nshift' - That target_flag preceeding a field flag within the range freq, that is nearest to a
-           field_flag, gets assigned this field flags value. (if field_flag > target_flag)
-
-        * 'match' - any target_flag with a timestamp matching a field_flags timestamp gets this field_flags value
-           (if field_flag > target_flag)
-
-        Note, to undo or backtrack a resampling/shifting/interpolation that has been performed with a certain method,
-        you can just pass the associated "inverse" method. Also you should pass the same ``drop`` keyword.
+        Note
+        ----
+        To undo or backtrack resampling, shifting or interpolation operations, use the
+        associated inversion method (e.g. to undo a former interpolation use
+        ``method="inverse_interpolation"``).
 
         Parameters
         ----------
-        field : str
-            Fieldname of flags history to append.
+        method :
+            Method to project the flags of :py:attr:`field` the flags to :py:attr:`target`:
 
-        target : str
-            Field name of flags history to append to.
+           * ``'auto'``: inverse the last alignment/resampling operations
+           * ``'inverse_nagg'``: project a flag of :py:attr:`field` to all timestamps of
+             :py:attr:`target` within the range +/- :py:attr:`freq`/2.
+           * ``'inverse_bagg'``: project a flag of :py:attr:`field` to all preceeding timestamps
+             of :py:attr:`target` within the range :py:attr:`freq`
+           * ``'inverse_fagg'``: project a flag of :py:attr:`field` to all succeeding timestamps
+             of :py:attr:`target` within the range :py:attr:`freq`
+           * ``'inverse_interpolation'`` - project a flag of :py:attr:`field` to all timestamps
+             of :py:attr:`target` within the range +/- :py:attr:`freq`
+           * ``'inverse_nshift'`` - project a flag of :py:attr:`field` to the neaerest timestamps
+             in :py:attr:`target` within the range +/- :py:attr:`freq`/2
+           * ``'inverse_bshift'`` - project a flag of :py:attr:`field` to nearest preceeding
+             timestamps in :py:attr:`target`
+           * ``'inverse_nshift'`` - project a flag of :py:attr:`field` to nearest succeeding
+             timestamps in :py:attr:`target`
+           * ``'match'`` - project a flag of :py:attr:`field` to all identical timestamps
+             :py:attr:`target`
+
+        freq :
+            Projection range. If ``None`` the sampling frequency of :py:attr:`field` is used.
 
-        method : {'inverse_fagg', 'inverse_bagg', 'inverse_nagg', 'inverse_fshift', 'inverse_bshift', 'inverse_nshift', 'match'}, default 'match'
-            The method used for projection of ``field`` flags onto ``target`` flags. See description above for more details.
+        drop :
+            Remove :py:attr:`field` if ``True``
 
-        freq : str or None, default None
-            The ``freq`` determines the projection range for the projection method. See above description for more details.
-            Defaultly (None), the sampling frequency of ``field`` is used.
+        squeeze :
+            Squueze the history into a single column if ``True``. Function specific flag information is lost.
 
-        drop : bool, default False
-            If set to `True`, the `field` column will be removed after processing
-
-        squeeze : bool, default False
-            If set to `True`, the appended flags frame will be squeezed - resulting in function specific flags informations
-            getting lost.
+        overwrite :
+            Overwrite existing flags if ``True``
+        """
 
-        overwrite: bool, default False
-            If set to True, the newly appended flags will overwrite exsiting flags. This might result in a loss of previous
-            flagging information.
+        if target is None:
+            target = field
 
-        Returns
-        -------
-        saqc.SaQC
-        """
         flagscol = self._flags[field]
         target_datcol = self._data[target]
         target_flagscol = self._flags[target]
 
         if target_datcol.empty or flagscol.empty:
             return self
 
@@ -416,27 +292,45 @@
             freq = getFreqDelta(flagscol.index)
             if freq is None and not method == "match":
                 raise ValueError(
                     'To project irregularly sampled data, either use method="match", or '
                     "pass custom projection range to freq parameter."
                 )
 
-        if method[-13:] == "interpolation":
+        if method == "auto":
+            stack = []
+            for meta in self._flags.history[field].meta:
+                func = meta["func"]
+                meth = meta["kwargs"].get("method")
+                if func in ("align", "resample"):
+                    if meth[1:] in ("agg", "shift"):
+                        stack.append(f"inverse_{meth}")
+                    else:
+                        stack.append("inverse_interpolation")
+                elif func == "concatFlags":
+                    stack.pop()
+            if not stack:
+                raise ValueError(
+                    "unable to derive an inversion method, please specify an appropiate 'method'"
+                )
+            method = stack[-1]
+
+        if method.endswith("interpolation"):
             ignore = _getChunkBounds(target_datcol, flagscol, freq)
             func = _inverseInterpolation
             func_kws = dict(freq=freq, chunk_bounds=ignore, target=dummy)
 
-        elif method[-3:] == "agg":
+        elif method.endswith("agg"):
             projection_method = METHOD2ARGS[method][0]
             tolerance = METHOD2ARGS[method][1](freq)
             func = _inverseAggregation
             func_kws = dict(freq=tolerance, method=projection_method, target=dummy)
 
-        elif method[-5:] == "shift":
-            drop_mask = target_datcol.isna() | _isflagged(
+        elif method.endswith("shift"):
+            drop_mask = target_datcol.isna() | isflagged(
                 target_flagscol, kwargs["dfilter"]
             )
             projection_method = METHOD2ARGS[method][0]
             tolerance = METHOD2ARGS[method][1](freq)
             func = _inverseShift
             kws = dict(
                 freq=tolerance,
@@ -450,38 +344,42 @@
             func = lambda x: x
             func_kws = {}
 
         else:
             raise ValueError(f"unknown method {method}")
 
         history = self._flags.history[field].apply(dummy.index, func, func_kws)
-
         if overwrite is False:
-            mask = _isflagged(self._flags[target], thresh=kwargs["dfilter"])
+            mask = isflagged(self._flags[target], thresh=kwargs["dfilter"])
             history._hist[mask] = np.nan
 
-        if squeeze:
-            history = history.squeeze(raw=True)
+        # append a dummy column
+        meta = {
+            "func": f"concatFlags",
+            "args": (),
+            "kwargs": {
+                "field": field,
+                "target": target,
+                "method": method,
+                "freq": freq,
+                "drop": drop,
+                "squeeze": squeeze,
+                "overwrite": overwrite,
+                **kwargs,
+            },
+        }
 
-            meta = {
-                "func": f"concatFlags",
-                "args": (field,),
-                "kwargs": {
-                    "target": target,
-                    "method": method,
-                    "freq": freq,
-                    "drop": drop,
-                    "squeeze": squeeze,
-                    "overwrite": overwrite,
-                    **kwargs,
-                },
-            }
-            self._flags.history[target].append(history, meta)
+        if squeeze:
+            flags = history.squeeze(raw=True)
+            history = History(index=history.index)
         else:
-            self._flags.history[target].append(history)
+            flags = pd.Series(np.nan, index=history.index, dtype=float)
+
+        history.append(flags, meta)
+        self._flags.history[target].append(history)
 
         if drop:
             return self.dropField(field=field)
 
         return self
```

### Comparing `saqc-2.3/saqc/funcs/residuals.py` & `saqc-2.4.0/saqc/funcs/residuals.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-from saqc.core.register import register
+from saqc.core import register
 from saqc.funcs.curvefit import _fitPolynomial
 from saqc.funcs.rolling import _roll
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 class ResidualsMixin:
     @register(mask=["field"], demask=[], squeeze=[])
     def calculatePolynomialResiduals(
         self: "SaQC",
         field: str,
@@ -49,38 +49,31 @@
         Note, that the initial and final window/2 values do not get fitted.
 
         Each residual gets assigned the worst flag present in the interval of
         the original data.
 
         Parameters
         ----------
-        field : str
-            The column, holding the data-to-be-modelled.
-
-        window : {str, int}
+        window :
             The size of the window you want to use for fitting. If an integer is passed,
             the size refers to the number of periods for every fitting window. If an
             offset string is passed, the size refers to the total temporal extension. The
             window will be centered around the vaule-to-be-fitted. For regularly sampled
             timeseries the period number will be casted down to an odd number if even.
 
-        order : int
+        order :
             The degree of the polynomial used for fitting
 
-        min_periods : int or None, default 0
+        min_periods :
             The minimum number of periods, that has to be available in every values
             fitting surrounding for the polynomial fit to be performed. If there are not
             enough values, np.nan gets assigned. Default (0) results in fitting
             regardless of the number of values present (results in overfitting for too
             sparse intervals). To automatically set the minimum number of periods to the
             number of values in an offset defined window size, pass np.nan.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         orig = self._data[field]
         data, _ = _fitPolynomial(
             data=self._data,
             field=field,
             flags=self._flags,
             window=window,
@@ -104,39 +97,29 @@
         """
         Calculate the diff of a rolling-window function and the data.
 
         Note, that the data gets assigned the worst flag present in the original data.
 
         Parameters
         ----------
-        field : str
-            The column to calculate on.
-
-        flags : saqc.Flags
-            Container to store quality flags to data.
-
-        window : {int, str}
+        window :
             The size of the window you want to roll with. If an integer is passed, the size
             refers to the number of periods for every fitting window. If an offset string
             is passed, the size refers to the total temporal extension. For regularly
             sampled timeseries, the period number will be casted down to an odd number if
             ``center=True``.
 
-        func : Callable, default np.mean
+        func : default mean
             Function to roll with.
 
-        min_periods : int, default 0
+        min_periods :
             The minimum number of periods to get a valid value
 
-        center : bool, default True
+        center :
             If True, center the rolling window.
-
-        Returns
-        -------
-        saqc.SaQC
         """
         orig = self._data[field].copy()
         data, _ = _roll(
             data=self._data,
             field=field,
             flags=self._flags,
             window=window,
```

### Comparing `saqc-2.3/saqc/funcs/rolling.py` & `saqc-2.4.0/saqc/funcs/rolling.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,115 @@
 #! /usr/bin/env python
 
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
+from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Union
 
 import numpy as np
 import pandas as pd
 
-from dios import DictOfSeries
-from saqc.core.flags import Flags
-from saqc.core.register import register
+from saqc.core import DictOfSeries, Flags, register
 from saqc.lib.tools import getFreqDelta
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 class RollingMixin:
     @register(mask=["field"], demask=[], squeeze=[])
-    def roll(
+    def rolling(
         self: "SaQC",
         field: str,
-        window: Union[str, int],
+        window: str | int,
         func: Callable[[pd.Series], np.ndarray] = np.mean,
         min_periods: int = 0,
         center: bool = True,
-        **kwargs
+        **kwargs,
     ) -> "SaQC":
         """
         Calculate a rolling-window function on the data.
 
         Note, that the data gets assigned the worst flag present in the original data.
 
         Parameters
         ----------
-        field : str
-            The column to calculate on.
+        window :
+            The size of the window you want to roll with. If an integer is passed, the size
+            refers to the number of periods for every fitting window. If an offset string
+            is passed, the size refers to the total temporal extension. For regularly
+            sampled timeseries, the period number will be casted down to an odd number if
+            ``center=True``.
 
-        flags : saqc.Flags
-            Container to store quality flags to data.
+        func : default mean
+            Function to roll with.
 
-        window : {int, str}
+        min_periods :
+            The minimum number of periods to get a valid value
+
+        center :
+            If True, center the rolling window.
+        """
+        self._data, self._flags = _roll(
+            data=self._data,
+            field=field,
+            flags=self._flags,
+            window=window,
+            func=func,
+            min_periods=min_periods,
+            center=center,
+            **kwargs,
+        )
+        return self
+
+    @register(mask=["field"], demask=[], squeeze=[])
+    def roll(
+        self: "SaQC",
+        field: str,
+        window: Union[str, int],
+        func: Callable[[pd.Series], np.ndarray] = np.mean,
+        min_periods: int = 0,
+        center: bool = True,
+        **kwargs,
+    ) -> "SaQC":
+        """
+        Calculate a rolling-window function on the data.
+
+        Note, that the data gets assigned the worst flag present in the original data.
+
+        Parameters
+        ----------
+        window :
             The size of the window you want to roll with. If an integer is passed, the size
             refers to the number of periods for every fitting window. If an offset string
             is passed, the size refers to the total temporal extension. For regularly
             sampled timeseries, the period number will be casted down to an odd number if
             ``center=True``.
 
-        func : Callable, default np.mean
+        func : default mean
             Function to roll with.
 
-        min_periods : int, default 0
+        min_periods :
             The minimum number of periods to get a valid value
 
-        center : bool, default True
+        center :
             If True, center the rolling window.
-
-        Returns
-        -------
-        saqc.SaQC
         """
+        import warnings
+
+        warnings.warn(
+            """The function `roll` was renamed to `rolling` and will be removed with version 3.0 of saqc
+            Please use `SaQC.rolling` with the same arguments, instead
+            """,
+            DeprecationWarning,
+        )
         self._data, self._flags = _roll(
             data=self._data,
             field=field,
             flags=self._flags,
             window=window,
             func=func,
             min_periods=min_periods,
@@ -81,15 +123,15 @@
     data: DictOfSeries,
     field: str,
     flags: Flags,
     window: Union[str, int],
     func: Callable[[pd.Series], np.ndarray] = np.mean,
     min_periods: int = 0,
     center: bool = True,
-    **kwargs
+    **kwargs,
 ):
     to_fit = data[field].copy()
     if to_fit.empty:
         return data, flags
 
     regular = getFreqDelta(to_fit.index)
     # starting with the annoying case: finding the rolling interval
```

### Comparing `saqc-2.3/saqc/funcs/scores.py` & `saqc-2.4.0/saqc/funcs/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,297 +3,300 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Optional, Sequence, Tuple
+import pickle
+from typing import TYPE_CHECKING, Optional
 
+import matplotlib as mpl
+import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 from typing_extensions import Literal
 
-import saqc.lib.ts_operators as ts_ops
-from saqc.constants import UNFLAGGED
-from saqc.core.register import register
-from saqc.lib.tools import getApply, toSequence
+from saqc import FILTER_NONE, UNFLAGGED
+from saqc.core import processing, register
+from saqc.lib.docs import DOC_TEMPLATES
+from saqc.lib.plotting import makeFig
+from saqc.lib.tools import periodicMask
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
-def _univarScoring(
-    data: pd.Series,
-    window: Optional[str, int] = None,
-    norm_func: Callable = np.nanstd,
-    model_func: Callable = np.nanmean,
-    center: bool = True,
-    min_periods: Optional[int] = None,
-) -> Tuple[pd.Series, pd.Series, pd.Series]:
-    """
-    Calculate (rolling) normalisation scores.
-
-    Parameters
-    ----------
-    data
-        A dictionary of pandas.Series, holding all the data.
-    window : {str, int}, default None
-            Size of the window. Either determined via an Offset String, denoting the windows temporal extension or
-            by an integer, denoting the windows number of periods.
-            `NaN` measurements also count as periods.
-            If `None` is passed, All data points share the same scoring window, which than equals the whole
-            data.
-    model_func
-        Function to calculate the center moment in every window.
-    norm_func
-        Function to calculate the scaling for every window
-    center
-        Weather or not to center the target value in the scoring window. If `False`, the
-        target value is the last value in the window.
-    min_periods
-        Minimum number of valid meassurements in a scoring window, to consider the resulting score valid.
-    """
-    if data.empty:
-        return data, data, data
-    if min_periods is None:
-        min_periods = 0
-
-    if window is None:
-        if data.notna().sum() >= min_periods:
-            # in case of stationary analysis, broadcast statistics to series for compatibility reasons
-            norm = pd.Series(norm_func(data.values), index=data.index)
-            model = pd.Series(model_func(data.values), index=data.index)
-        else:
-            norm = pd.Series(np.nan, index=data.index)
-            model = pd.Series(np.nan, index=data.index)
-    else:
-        # wrap passed func with rolling built in if possible and rolling.apply else
-        roller = data.rolling(window=window, min_periods=min_periods, center=center)
-        norm = getApply(roller, norm_func)
-        model = getApply(roller, model_func)
-
-    score = (data - model) / norm
-    return score, model, norm
+_MPL_DEFAULT_BACKEND = mpl.get_backend()
 
 
-class ScoresMixin:
+class ToolsMixin:
     @register(
-        mask=["field"],
+        mask=[],
         demask=[],
-        squeeze=["target"],
-        multivariate=True,
+        squeeze=[],
         handles_target=True,
+        docstring={"target": DOC_TEMPLATES["target"]},
     )
-    def assignKNNScore(
+    def copyField(
         self: "SaQC",
-        field: Sequence[str],
+        field: str,
         target: str,
-        n: int = 10,
-        func: Callable[[pd.Series], float] = np.sum,
-        freq: float | str | None = np.inf,
-        min_periods: int = 2,
-        method: Literal["ball_tree", "kd_tree", "brute", "auto"] = "ball_tree",
-        metric: str = "minkowski",
-        p: int = 2,
+        overwrite: bool = False,
         **kwargs,
     ) -> "SaQC":
         """
-        TODO: docstring need a rework
-        Score datapoints by an aggregation of the dictances to their k nearest neighbors.
+        Copy data and flags to a new name (preserve flags history).
+        """
+        if field == target:
+            return self
 
-        The function is a wrapper around the NearestNeighbors method from pythons sklearn library (See reference [1]).
+        if target in self._flags.columns.union(self._data.columns):
+            if not overwrite:
+                raise ValueError(f"{target}: already exist")
+            self = self.dropField(field=target)
 
-        The steps taken to calculate the scores are as follows:
+        self._data[target] = self._data[field].copy()
+        self._flags.history[target] = self._flags.history[field].copy()
+
+        return self
+
+    @processing()
+    def dropField(self: "SaQC", field: str, **kwargs) -> "SaQC":
+        """
+        Drops field from the data and flags.
+        """
+        del self._data[field]
+        del self._flags[field]
+        return self
 
-        1. All the timeseries, given through ``field``, are combined to one feature space by an *inner* join on their
-           date time indexes. thus, only samples, that share timestamps across all ``field`` will be included in the
-           feature space.
-        2. Any datapoint/sample, where one ore more of the features is invalid (=np.nan) will get excluded.
-        3. For every data point, the distance to its `n` nearest neighbors is calculated by applying the
-           metric `metric` at grade `p` onto the feature space. The defaults lead to the euclidian to be applied.
-           If `radius` is not None, it sets the upper bound of distance for a neighbor to be considered one of the
-           `n` nearest neighbors. Furthermore, the `freq` argument determines wich samples can be
-           included into a datapoints nearest neighbors list, by segmenting the data into chunks of specified temporal
-           extension and feeding that chunks to the kNN algorithm seperatly.
-        4. For every datapoint, the calculated nearest neighbors distances get aggregated to a score, by the function
-           passed to `func`. The default, ``sum`` obviously just sums up the distances.
-        5. The resulting timeseries of scores gets assigned to the field target.
+    @processing()
+    def renameField(self: "SaQC", field: str, new_name: str, **kwargs) -> "SaQC":
+        """
+        Rename field in data and flags.
 
         Parameters
         ----------
-        field : list of str
-            input variable names.
+        new_name :
+            String, field is to be replaced with.
+        """
+        self._data[new_name] = self._data[field]
+        self._flags.history[new_name] = self._flags.history[field]
+        del self._data[field]
+        del self._flags[field]
+        return self
 
-        target : str, default "kNNscores"
-            A new Column name, where the result is stored.
+    @register(mask=[], demask=[], squeeze=["field"])
+    def selectTime(
+        self: "SaQC",
+        field: str,
+        mode: Literal["periodic", "selection_field"],
+        selection_field: str | None = None,
+        start: str | None = None,
+        end: str | None = None,
+        closed: bool = True,
+        **kwargs,
+    ) -> "SaQC":
+        """
+        Realizes masking within saqc.
 
-        n : int, default 10
-            The number of nearest neighbors to which the distance is comprised in every datapoints scoring calculation.
+        Due to some inner saqc mechanics, it is not straight forwardly possible to exclude
+        values or datachunks from flagging routines. This function replaces flags with UNFLAGGED
+        value, wherever values are to get masked. Furthermore, the masked values get replaced by
+        np.nan, so that they dont effect calculations.
+
+        Here comes a recipe on how to apply a flagging function only on a masked chunk of the variable field:
+
+        1. dublicate "field" in the input data (`copyField`)
+        2. mask the dublicated data (this, `selectTime`)
+        3. apply the tests you only want to be applied onto the masked data chunks (a saqc function)
+        4. project the flags, calculated on the dublicated and masked data onto the original field data
+            (`concateFlags` or `flagGeneric`)
+        5. drop the dublicated data (`dropField`)
 
-        func : Callable[numpy.array, float], default np.sum
-            A function that assigns a score to every one dimensional array, containing the distances
-            to every datapoints `n` nearest neighbors.
-
-        freq : {float, str, None}, default np.inf
-            Determines the segmentation of the data into partitions, the kNN algorithm is
-            applied onto individually.
-
-            * ``np.inf``: Apply Scoring on whole data set at once
-            * ``x`` > 0 : Apply scoring on successive data chunks of periods length ``x``
-            * Offset String : Apply scoring on successive partitions of temporal extension matching the passed offset
-              string
-
-        min_periods : int, default 2
-            The minimum number of periods that have to be present in a partition for the kNN scoring
-            to be applied. If the number of periods present is below `min_periods`, the score for the
-            datapoints in that partition will be np.nan.
-
-        method : {'ball_tree', 'kd_tree', 'brute', 'auto'}, default 'ball_tree'
-            The search algorithm to find each datapoints k nearest neighbors.
-            The keyword just gets passed on to the underlying sklearn method.
-            See reference [1] for more information on the algorithm.
-
-        metric : str, default 'minkowski'
-            The metric the distances to any datapoints neighbors is computed with. The default of `metric`
-            together with the default of `p` result in the euclidian to be applied.
-            The keyword just gets passed on to the underlying sklearn method.
-            See reference [1] for more information on the algorithm.
-
-        p : int, default 2
-            The grade of the metrice specified by parameter `metric`.
-            The keyword just gets passed on to the underlying sklearn method.
-            See reference [1] for more information on the algorithm.
-
-        Returns
-        -------
-        saqc.SaQC
+        To see an implemented example, checkout flagSeasonalRange in the saqc.functions module
 
-        References
+        Parameters
         ----------
-        [1] https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html
-        """
-        if isinstance(target, list):
-            if (len(target) > 1) or (target[0] in self._data.columns):
-                raise ValueError(
-                    f"'target' must not exist and be of length 1. {target} was passed instead."
-                )
-            target = target[0]
-
-        fields = toSequence(field)
-        val_frame = self._data[fields].copy()
-        score_index = val_frame.index_of("shared")
-        score_ser = pd.Series(np.nan, index=score_index, name=target)
+        mode :
+            The masking mode.
+            - "periodic": parameters "period_start", "end" are evaluated to generate a periodical mask
+            - "mask_var": data[mask_var] is expected to be a boolean valued timeseries and is used as mask.
+
+        selection_field :
+            Only effective if mode == "mask_var"
+            Fieldname of the column, holding the data that is to be used as mask. (must be boolean series)
+            Neither the series` length nor its labels have to match data[field]`s index and length. An inner join of the
+            indices will be calculated and values get masked where the values of the inner join are ``True``.
+
+        start :
+            Only effective if mode == "seasonal"
+            String denoting starting point of every period. Formally, it has to be a truncated instance of "mm-ddTHH:MM:SS".
+            Has to be of same length as `end` parameter.
+            See examples section below for some examples.
+
+        end :
+            Only effective if mode == "periodic"
+            String denoting starting point of every period. Formally, it has to be a truncated instance of "mm-ddTHH:MM:SS".
+            Has to be of same length as `end` parameter.
+            See examples section below for some examples.
+
+        closed :
+            Wheather or not to include the mask defining bounds to the mask.
+
+        Examples
+        --------
+        The `period_start` and `end` parameters provide a conveniant way to generate seasonal / date-periodic masks.
+        They have to be strings of the forms: "mm-ddTHH:MM:SS", "ddTHH:MM:SS" , "HH:MM:SS", "MM:SS" or "SS"
+        (mm=month, dd=day, HH=hour, MM=minute, SS=second)
+        Single digit specifications have to be given with leading zeros.
+        `period_start` and `seas   on_end` strings have to be of same length (refer to the same periodicity)
+        The highest date unit gives the period.
+        For example:
+
+        >>> start = "01T15:00:00"
+        >>> end = "13T17:30:00"
+
+        Will result in all values sampled between 15:00 at the first and  17:30 at the 13th of every month get masked
+
+        >>> start = "01:00"
+        >>> end = "04:00"
+
+        All the values between the first and 4th minute of every hour get masked.
+
+        >>> start = "01-01T00:00:00"
+        >>> end = "01-03T00:00:00"
+
+        Mask january and february of evcomprosed in theery year. masking is inclusive always, so in this case the mask will
+        include 00:00:00 at the first of march. To exclude this one, pass:
 
-        val_frame = val_frame.loc[val_frame.index_of("shared")].to_df()
-        val_frame.dropna(inplace=True)
+        >>> start = "01-01T00:00:00"
+        >>> end = "02-28T23:59:59"
 
-        if val_frame.empty:
-            return self
+        To mask intervals that lap over a seasons frame, like nights, or winter, exchange sequence of season start and
+        season end. For example, to mask night hours between 22:00:00 in the evening and 06:00:00 in the morning, pass:
 
-        # partitioning
-        if not freq:
-            freq = val_frame.shape[0]
+        >>> start = "22:00:00"
+        >>> end = "06:00:00"
+        """
+        datcol_idx = self._data[field].index
 
-        if isinstance(freq, str):
-            grouper = pd.Grouper(freq=freq)
+        if mode == "periodic":
+            mask = periodicMask(datcol_idx, start, end, ~closed)
+        elif mode == "selection_field":
+            idx = self._data[selection_field].index.intersection(datcol_idx)
+            mask = self._data[selection_field].loc[idx]
         else:
-            grouper = pd.Series(
-                data=np.arange(0, val_frame.shape[0]), index=val_frame.index
+            raise ValueError(
+                "Keyword passed as masking mode is unknown ({})!".format(mode)
             )
-            grouper = grouper.transform(lambda x: int(np.floor(x / freq)))
-
-        partitions = val_frame.groupby(grouper)
-
-        for _, partition in partitions:
-            if partition.empty or (partition.shape[0] < min_periods):
-                continue
-
-            sample_size = partition.shape[0]
-            nn_neighbors = min(n, max(sample_size, 2) - 1)
-            dist, *_ = ts_ops.kNN(
-                partition.values, nn_neighbors, algorithm=method, metric=metric, p=p
-            )
-            try:
-                resids = getattr(dist, func.__name__)(axis=1)
-            except AttributeError:
-                resids = np.apply_along_axis(func, 1, dist)
-
-            score_ser[partition.index] = resids
-
-        self._flags[target] = pd.Series(UNFLAGGED, index=score_ser.index, dtype=float)
-        self._data[target] = score_ser
 
+        mask = mask.reindex(self._data[field].index, fill_value=False).astype(bool)
+        self._data[field].loc[mask] = np.nan
+        self._flags[mask, field] = UNFLAGGED
         return self
 
-    @register(mask=["field"], demask=[], squeeze=[])
-    def assignZScore(
+    @register(mask=[], demask=[], squeeze=[])
+    def plot(
         self: "SaQC",
         field: str,
-        window: Optional[str] = None,
-        norm_func: Callable = np.nanstd,
-        model_func: Callable = np.nanmean,
-        center: bool = True,
-        min_periods: Optional[int] = None,
+        path: Optional[str] = None,
+        max_gap: Optional[str] = None,
+        history: Optional[Literal["valid", "complete"] | list] = "valid",
+        xscope: Optional[slice] = None,
+        phaseplot: Optional[str] = None,
+        store_kwargs: Optional[dict] = None,
+        ax: mpl.axes.Axes | None = None,
+        ax_kwargs: Optional[dict] = None,
+        dfilter: float = FILTER_NONE,
         **kwargs,
     ) -> "SaQC":
         """
-        Calculate (rolling) Zscores.
+        Plot data and flags or store plot to file.
 
-        See the Notes section for a detailed overview of the calculation
+        There are two modes, 'interactive' and 'store', which are determind through the
+        ``save_path`` keyword. In interactive mode (default) the plot is shown at runtime
+        and the program execution stops until the plot window is closed manually. In
+        store mode the generated plot is stored to disk and no manually interaction is
+        needed.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-flagged. (Here a dummy, for structural reasons)
-        window : {str, int}, default None
-            Size of the window. Either determined via an Offset String, denoting the windows temporal extension or
-            by an integer, denoting the windows number of periods.
-            `NaN` measurements also count as periods.
-            If `None` is passed, All data points share the same scoring window, which than equals the whole
-            data.
-        model_func
-            Function to calculate the center moment in every window.
-        norm_func
-            Function to calculate the scaling for every window
-        center
-            Weather or not to center the target value in the scoring window. If `False`, the
-            target value is the last value in the window.
-        min_periods
-            Minimum number of valid meassurements in a scoring window, to consider the resulting score valid.
-
-        Returns
-        -------
-        data : dios.DictOfSeries
-            A dictionary of pandas.Series, holding all the data.
-        flags : saqc.Flags
-            The quality flags of data
-            Flags values may have changed, relatively to the flags input.
-
-        Notes
-        -----
-        Steps of calculation:
-
-        1. Consider a window :math:`W` of successive points :math:`W = x_{1},...x_{w}`
-        containing the value :math:`y_{K}` wich is to be checked.
-        (The index of :math:`K` depends on the selection of the parameter `center`.)
+        path :
+            If ``None`` is passed, interactive mode is entered; plots are shown immediatly
+            and a user need to close them manually before execution continues.
+            If a filepath is passed instead, store-mode is entered and
+            the plot is stored unter the passed location.
+
+        max_gap :
+            If None, all the points in the data will be connected, resulting in long linear
+            lines, where continous chunks of data is missing. Nans in the data get dropped
+            before plotting. If an offset string is passed, only points that have a distance
+            below `max_gap` get connected via the plotting line.
+
+        history :
+            Discriminate the plotted flags with respect to the tests they originate from.
+
+            * "valid" - Only plot those flags, that do not get altered or "unflagged" by subsequent tests. Only list tests
+              in the legend, that actually contributed flags to the overall resault.
+            * "complete" - plot all the flags set and list all the tests ran on a variable. Suitable for debugging/tracking.
+            * None - just plot the resulting flags for one variable, without any historical meta information.
+            * list of strings - plot only flags set by those tests listed.
+
+        xscope :
+            Parameter, that determines a chunk of the data to be plotted
+            processed. `xscope` can be anything, that is a valid argument to the ``pandas.Series.__getitem__`` method.
+
+        phaseplot :
+            If a string is passed, plot ``field`` in the phase space it forms together with the Variable ``phaseplot``.
+
+        store_kwargs :
+            Keywords to be passed on to the ``matplotlib.pyplot.savefig`` method, handling
+            the figure storing. To store an pickle object of the figure, use the option
+            ``{'pickle': True}``, but note that all other store_kwargs are ignored then.
+            Reopen with: ``pickle.load(open(savepath,'w')).show()``
+
+        ax_kwargs :
+            Axis keywords. Change the axis labeling defaults. Most important keywords:
+            'x_label', 'y_label', 'title', 'fontsize', 'cycleskip'.
+        """
+        data, flags = self._data.copy(), self._flags.copy()
 
-        2. The "moment" :math:`M` for the window gets calculated via :math:`M=` `model_func(:math:`W`)
+        level = kwargs.get("flag", UNFLAGGED)
 
-        3. The "scaling" :math:`N` for the window gets calculated via :math:`N=` `norm_func(:math:`W`)
+        if dfilter < np.inf:
+            data[field].loc[flags[field] >= dfilter] = np.nan
 
-        4. The "score" :math:`S` for the point :math:`x_{k}`gets calculated via :math:`S=(x_{k} - M) / N`
-        """
+        if store_kwargs is None:
+            store_kwargs = {}
+
+        if ax_kwargs is None:
+            ax_kwargs = {}
 
-        if min_periods is None:
-            min_periods = 0
+        if not path:
+            mpl.use(_MPL_DEFAULT_BACKEND)
+        else:
+            mpl.use("Agg")
 
-        score, _, _ = _univarScoring(
-            self._data[field],
-            window=window,
-            norm_func=norm_func,
-            model_func=model_func,
-            center=center,
-            min_periods=min_periods,
+        fig = makeFig(
+            data=data,
+            field=field,
+            flags=flags,
+            level=level,
+            max_gap=max_gap,
+            history=history,
+            xscope=xscope,
+            phaseplot=phaseplot,
+            ax=ax,
+            ax_kwargs=ax_kwargs,
         )
-        self._data[field] = score
+
+        if ax is None and not path:
+            plt.show()
+
+        if path:
+            if store_kwargs.pop("pickle", False):
+                with open(path, "wb") as f:
+                    pickle.dump(fig, f)
+            else:
+                fig.savefig(path, **store_kwargs)
+
         return self
```

### Comparing `saqc-2.3/saqc/funcs/transformation.py` & `saqc-2.4.0/saqc/funcs/transformation.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,65 +8,53 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-from saqc.core.register import register
+from saqc.core import register
 
 if TYPE_CHECKING:
-    from saqc.core.core import SaQC
+    from saqc import SaQC
 
 
 class TransformationMixin:
     @register(mask=["field"], demask=[], squeeze=[])
     def transform(
         self: "SaQC",
         field: str,
-        func: Callable[[pd.Series], pd.Series],
-        freq: Optional[Union[float, str]] = None,
+        func: Callable[[pd.Series | np.ndarray], pd.Series],
+        freq: float | str | None = None,
         **kwargs,
     ) -> "SaQC":
         """
-        Function to transform data columns with a transformation that maps series onto series of the same length.
-
-        Note, that flags get preserved.
+        Transform data by applying a custom function on data chunks of variable size. Existing flags are preserved.
 
         Parameters
         ----------
-        field : str
-            The fieldname of the column, holding the data-to-be-transformed.
-
-        func : Callable[{pd.Series, np.array}, np.array]
-            Function to transform data[field] with.
+        func :
+            Transformation function.
 
-        freq : {None, float, str}, default None
-            Determines the segmentation of the data into partitions, the transformation is applied on individually
+        freq :
+            Size of the data window. The transformation is applied on each window individually
 
-            * ``np.inf``: Apply transformation on whole data set at once
-            * ``x`` > 0 : Apply transformation on successive data chunks of periods length ``x``
-            * Offset String : Apply transformation on successive partitions of temporal extension matching the passed offset
-              string
-
-        Returns
-        -------
-        saqc.SaQC
+            * ``None``: Apply transformation on the entire data set at once
+            * ``int`` : Apply transformation on successive data chunks of the given length. Must be grater than 0.
+            * Offset String : Apply transformation on successive data chunks of the given temporal extension.
         """
         val_ser = self._data[field].copy()
         # partitioning
         if not freq:
-            freq = val_ser.shape[0]
+            freq = len(val_ser)
 
         if isinstance(freq, str):
             grouper = pd.Grouper(freq=freq)
         else:
-            grouper = pd.Series(
-                data=np.arange(0, val_ser.shape[0]), index=val_ser.index
-            )
+            grouper = pd.Series(data=np.arange(0, len(val_ser)), index=val_ser.index)
             grouper = grouper.transform(lambda x: int(np.floor(x / freq)))
 
         partitions = val_ser.groupby(grouper)
 
         for _, partition in partitions:
             if partition.empty:
                 continue
```

### Comparing `saqc-2.3/saqc/lib/plotting.py` & `saqc-2.4.0/saqc/lib/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import itertools
-from typing import Optional, Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
-from saqc.core.flags import Flags
+from saqc.core import DictOfSeries, Flags
 from saqc.lib.tools import toSequence
-from saqc.lib.types import DiosLikeT
 
 STATSDICT = {
     "values total": lambda x, y, z: len(x),
     "invalid total (=NaN)": lambda x, y, z: x.isna().sum(),
     "invalid percentage": lambda x, y, z: round((x.isna().sum()) / len(x), 2),
     "flagged total": lambda x, y, z: (y >= z).sum(),
     "flagged percentage": lambda x, y, z: round(((y >= z).sum()) / len(x), 2),
@@ -52,15 +50,15 @@
     "zorder": 10,
     "edgecolors": "black",
     "s": 70,
 }
 
 
 def makeFig(
-    data: DiosLikeT,
+    data: DictOfSeries,
     field: str,
     flags: Flags,
     level: float,
     max_gap: str | None = None,
     history: Literal["valid", "complete"] | None | list[str] = "valid",
     xscope: slice | None = None,
     phaseplot: str | None = None,
@@ -68,18 +66,18 @@
     ax_kwargs: dict | None = None,
 ):
     """
     Returns a figure object, containing data graph with flag marks for field.
 
     Parameters
     ----------
-    data : {pd.DataFrame, dios.DictOfSeries}
+    data : {pd.DataFrame, DictOfSeries}
         data
 
-    flags : {pd.DataFrame, dios.DictOfSeries, saqc.flagger}
+    flags : {pd.DataFrame, DictOfSeries, saqc.flagger}
         Flags or flagger object
 
     field : str
         Name of the variable-to-plot
 
     level : str, float, default None
         Flaglevel above wich flagged values should be displayed.
@@ -115,15 +113,16 @@
         figure object.
 
     """
 
     if ax_kwargs is None:
         ax_kwargs = {}
     # data retrieval
-    d = data[field]
+    d = data[field].copy(deep=False)
+    d.name = field
     # data slicing:
     xscope = xscope or slice(xscope)
     d = d[xscope]
     flags_vals = flags[field][xscope]
     flags_hist = flags.history[field].hist.loc[xscope]
     flags_meta = flags.history[field].meta
```

### Comparing `saqc-2.3/saqc/lib/tools.py` & `saqc-2.4.0/saqc/lib/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,25 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import collections
+import functools
 import itertools
 import re
 import warnings
-from typing import Callable, Collection, List, Sequence, TypeVar, Union
+from typing import Any, Callable, Collection, List, Sequence, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from scipy import fft
 from scipy.cluster.hierarchy import fcluster, linkage
 
-import dios
-
-# keep this for external imports
-# TODO: fix the external imports
-from saqc.lib.rolling import customRoller
 from saqc.lib.types import CompT
 
 T = TypeVar("T", str, float, int)
 
 
 def assertScalar(name, value, optional=False):
     if optional and value is None:
@@ -167,67 +163,14 @@
     freq = "1" + "mmmhhhdddMMMYYY"[len(season_start)]
     out = mask.groupby(pd.Grouper(freq=freq)).transform(_selector)
     if invert:
         out = ~out
     return out
 
 
-def concatDios(data: List[dios.DictOfSeries], warn: bool = True, stacklevel: int = 2):
-    # fast path for most common case
-    if len(data) == 1 and data[0].columns.is_unique:
-        return data[0]
-
-    result = dios.DictOfSeries()
-    for di in data:
-        for c in di.columns:
-            if c in result.columns:
-                if warn:
-                    warnings.warn(
-                        f"Column {c} already exist. Data is overwritten. "
-                        f"Avoid duplicate columns names over all inputs.",
-                        stacklevel=stacklevel,
-                    )
-            result[c] = di[c]
-
-    return result
-
-
-def mergeDios(left, right, subset=None, join="merge"):
-    # use dios.merge() as soon as it implemented
-    # see https://git.ufz.de/rdm/dios/issues/15
-
-    merged = left.copy()
-    if subset is not None:
-        right_subset_cols = right.columns.intersection(subset)
-    else:
-        right_subset_cols = right.columns
-
-    shared_cols = left.columns.intersection(right_subset_cols)
-
-    for c in shared_cols:
-        l, r = left[c], right[c]
-        if join == "merge":
-            # NOTE:
-            # our merge behavior is nothing more than an
-            # outer join, where the right join argument
-            # overwrites the left at the shared indices,
-            # while on a normal outer join common indices
-            # hold the values from the left join argument
-            r, l = l.align(r, join="outer")
-        else:
-            l, r = l.align(r, join=join)
-        merged[c] = l.combine_first(r)
-
-    newcols = right_subset_cols.difference(left.columns)
-    for c in newcols:
-        merged[c] = right[c].copy()
-
-    return merged
-
-
 def isQuoted(string):
     return bool(re.search(r"'.*'|\".*\"", string))
 
 
 def mutateIndex(index, old_name, new_name):
     pos = index.get_loc(old_name)
     index = index.drop(index[pos])
@@ -241,15 +184,14 @@
     max_rate="10s",
     min_rate="1D",
     optimize=True,
     min_energy=0.2,
     max_freqs=10,
     bins=None,
 ):
-
     """
     Function to estimate the sampling rate of an index.
 
     The function comes with some optional overhead.
     The default options detect sampling rates from 10 seconds to 1 day with a 10 seconds precision
     for sampling rates below one minute, and a one minute precision for rates between 1 minute and
     one day.
@@ -343,46 +285,14 @@
     f_hist, bins = np.histogram(freqs, bins=bins)
     freqs = np.ceil(bins[:-1][f_hist >= 1])
     gcd_freq = np.gcd.reduce((10 * freqs).astype(int)) / 10
 
     return str(int(gcd_freq)) + "min", [str(int(i)) + "min" for i in freqs]
 
 
-def evalFreqStr(freq, check, index):
-    if check in ["check", "auto"]:
-        f_passed = freq
-        freq = index.inferred_freq
-        freqs = [freq]
-        if freq is None:
-            freq, freqs = estimateFrequency(index)
-        if freq is None:
-            warnings.warn("Sampling rate could not be estimated.")
-        if len(freqs) > 1:
-            warnings.warn(
-                f"Sampling rate seems to be not uniform!." f"Detected: {freqs}"
-            )
-
-        if check == "check":
-            f_passed_seconds = pd.Timedelta(f_passed).total_seconds()
-            freq_seconds = pd.Timedelta(freq).total_seconds()
-            if f_passed_seconds != freq_seconds:
-                warnings.warn(
-                    f"Sampling rate estimate ({freq}) missmatches passed frequency ({f_passed})."
-                )
-        elif check == "auto":
-            if freq is None:
-                raise ValueError(
-                    "Frequency estimation for non-empty series failed with no fall back frequency passed."
-                )
-            f_passed = freq
-    else:
-        f_passed = freq
-    return f_passed
-
-
 def detectDeviants(
     data,
     metric,
     norm_spread,
     norm_frac,
     linkage_method="single",
     population="variables",
@@ -393,20 +303,17 @@
 
     "Normality" is determined in terms of a maximum spreading distance, that members of a normal group must not exceed
     in respect to a certain metric and linkage method.
 
     In addition, only a group is considered "normal" if it contains more then `frac` percent of the
     variables in "fields".
 
-    Note, that the function also can be used to detect anormal regimes in a variable by assigning the different regimes
-    dios.DictOfSeries columns and passing this dios.
-
     Parameters
     ----------
-    data : {pandas.DataFrame, dios.DictOfSeries}
+    data : {pandas.DataFrame, DictOfSeries}
         Input data
     metric : Callable[[numpy.array, numpy.array], float]
         A metric function that for calculating the dissimilarity between 2 variables.
     norm_spread : float
         A threshold denoting the distance, members of the "normal" group must not exceed to each other (in terms of the
         metric passed) to qualify their group as the "normal" group.
     norm_frac : float, default 0.5
@@ -416,56 +323,60 @@
         The linkage method used for hierarchical (agglomerative) clustering of the variables.
     population : {"variables", "samples"}
         Wheather to relate the minimum percentage of values needed to form a normal group, to the total number of
         variables or to the total number of samples.
 
     Returns
     -------
-    deviants : List
-        A list containing the column positions of deviant variables in the input frame/dios.
+    deviants : list
+        A list containing the column positions of deviant variables in the input
 
     """
     var_num = len(data.columns)
     if var_num <= 1:
         return []
     dist_mat = np.zeros((var_num, var_num))
     combs = list(itertools.combinations(range(0, var_num), 2))
     for i, j in combs:
-        dist = metric(data.iloc[:, i].values, data.iloc[:, j].values)
+        d_i = data[data.columns[i]]
+        d_j = data[data.columns[j]]
+        dist = metric(d_i.values, d_j.values)
         dist_mat[i, j] = dist
 
     condensed = np.abs(dist_mat[tuple(zip(*combs))])
     Z = linkage(condensed, method=linkage_method)
     cluster = fcluster(Z, norm_spread, criterion="distance")
     if population == "variables":
         counts = collections.Counter(cluster)
         pop_num = var_num
     elif population == "samples":
         counts = {cluster[j]: 0 for j in range(0, var_num)}
         for c in range(var_num):
-            counts[cluster[c]] += data.iloc[:, c].dropna().shape[0]
+            field = data.columns[c]
+            counts[cluster[c]] += data[field].dropna().shape[0]
         pop_num = np.sum(list(counts.values()))
     else:
         raise ValueError(
-            "Not a valid normality criteria keyword passed. Pass either 'variables' or 'population'."
+            "Not a valid normality criteria keyword passed. "
+            "Pass either 'variables' or 'population'."
         )
     norm_cluster = -1
 
     for item in counts.items():
         if item[1] > norm_frac * pop_num:
             norm_cluster = item[0]
             break
 
     if norm_cluster == -1 or counts[norm_cluster] == pop_num:
         return []
     else:
         return [i for i, x in enumerate(cluster) if x != norm_cluster]
 
 
-def getFreqDelta(index):
+def getFreqDelta(index: pd.Index) -> None | pd.Timedelta:
     """
     Function checks if the passed index is regularly sampled.
 
     If yes, the according timedelta value is returned,
 
     If no, ``None`` is returned.
 
@@ -591,7 +502,58 @@
             warnings.warn(
                 f"The keyword {repr(key)} is reserved and will be ignored {msg}",
                 RuntimeWarning,
                 stacklevel=stacklevel,
             )
         kwargs.pop(key, None)
     return kwargs
+
+
+from saqc import FILTER_ALL, UNFLAGGED
+
+A = TypeVar("A", np.ndarray, pd.Series)
+
+
+def isflagged(flagscol: A, thresh: float) -> A:
+    """
+    Return a mask of flags accordingly to `thresh`. Return type is same as flags.
+    """
+    if not isinstance(thresh, (float, int)):
+        raise TypeError(f"thresh must be of type float, not {repr(type(thresh))}")
+
+    if thresh == FILTER_ALL:
+        return flagscol > UNFLAGGED
+
+    return flagscol >= thresh
+
+
+def isunflagged(flagscol: A, thresh: float) -> A:
+    return ~isflagged(flagscol, thresh)
+
+
+def getUnionIndex(obj, default: pd.DatetimeIndex | None = None):
+    assert hasattr(obj, "columns")
+    if default is None:
+        default = pd.DatetimeIndex([])
+    indexes = [obj[k].index for k in obj.columns]
+    if indexes:
+        return functools.reduce(pd.Index.union, indexes).sort_values()
+    return default
+
+
+def getSharedIndex(obj, default: pd.DatetimeIndex | None = None):
+    assert hasattr(obj, "columns")
+    if default is None:
+        default = pd.DatetimeIndex([])
+    indexes = [obj[k].index for k in obj.columns]
+    if indexes:
+        return functools.reduce(pd.Index.intersection, indexes).sort_values()
+    return default
+
+
+def isAllBoolean(obj: Any):
+    if not hasattr(obj, "columns"):
+        return pd.api.types.is_bool_dtype(obj)
+    for c in obj.columns:
+        if not pd.api.types.is_bool_dtype(obj[c]):
+            return False
+    return True
```

### Comparing `saqc-2.3/saqc/lib/ts_operators.py` & `saqc-2.4.0/saqc/lib/ts_operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -272,99 +272,137 @@
 
 def meanQC(data, max_nan_total=np.inf, max_nan_consec=np.inf):
     return np.nanmean(
         data[~validationTrafo(data.isna(), max_nan_total, max_nan_consec)]
     )
 
 
-def interpolateNANs(
-    data, method, order=2, inter_limit=2, downgrade_interpolation=False
+def _interpolWrapper(
+    x, order=1, method="time", limit_area="inside", limit_direction=None
 ):
     """
+    Function that automatically modifies the interpolation level or returns uninterpolated
+    input data if the data configuration breaks the interpolation method at the selected degree.
+    """
+
+    min_vals_dict = {
+        "nearest": 2,
+        "slinear": 2,
+        "quadratic": 3,
+        "cubic": 4,
+        "spline": order + 1,
+        "polynomial": order + 1,
+        "piecewise_polynomial": 2,
+        "pchip": 2,
+        "akima": 2,
+        "cubicspline": 2,
+    }
+    min_vals = min_vals_dict.get(method, 0)
+
+    if (x.size < 3) | (x.count() < min_vals):
+        return x
+    else:
+        return x.interpolate(
+            method=method,
+            order=order,
+            limit_area=limit_area,
+            limit_direction=limit_direction,
+        )
+
+
+def interpolateNANs(data, method, order=2, gap_limit=2, extrapolate=None):
+    """
     The function interpolates nan-values (and nan-grids) in timeseries data. It can
     be passed all the method keywords from the pd.Series.interpolate method and will
     than apply this very methods. Note, that the limit keyword really restricts
-    the interpolation to chunks, not containing more than "limit" nan entries (
+    the interpolation to gaps, not containing more than "limit" nan entries (
     thereby not being identical to the "limit" keyword of pd.Series.interpolate).
 
     :param data:                    pd.Series or np.array. The data series to be interpolated
     :param method:                  String. Method keyword designating interpolation method to use.
     :param order:                   Integer. If your desired interpolation method needs an order to be passed -
                                     here you pass it.
-    :param inter_limit:             Integer. Default = 2. Limit up to which consecutive nan - values in the data get
-                                    replaced by interpolation.
+    :param gap_limit:               Integer or Offset String. Default = 2.
+                                    Number up to which consecutive nan - values in the data get
+                                    replaced by interpolated values.
                                     Its default value suits an interpolation that only will apply to points of an
                                     inserted frequency grid. (regularization by interpolation)
-                                    Gaps wider than "limit" will NOT be interpolated at all.
-    :param downgrade_interpolation:  Boolean. Default False. If True:
+                                    Gaps of size "limit" or greater will NOT be interpolated at all.
+    :param extrapolate:             Str or None. Default None. If True:
                                     If a data chunk not contains enough values for interpolation of the order "order",
                                     the highest order possible will be selected for that chunks interpolation.
 
     :return:
     """
-    inter_limit = int(inter_limit or len(data) + 1)
-    data = pd.Series(data, copy=True)
-    gap_mask = data.isna().rolling(inter_limit, min_periods=0).sum() != inter_limit
 
-    if inter_limit == 2:
-        gap_mask = gap_mask & gap_mask.shift(-1, fill_value=True)
+    # helper variable for checking numerical value of gap limit, if its a numeric value (to avoid comparison to str)
+    gap_check = np.nan if isinstance(gap_limit, str) else gap_limit
+    data = pd.Series(data, copy=True)
+    limit_area = "inside" if not extrapolate else "outside"
+    if gap_check is None:
+        # if there is actually no limit set to the gaps to-be interpolated, generate a dummy mask for the gaps
+        gap_mask = pd.Series(True, index=data.index, name=data.name)
     else:
-        gap_mask = (
-            gap_mask.replace(True, np.nan)
-            .fillna(method="bfill", limit=inter_limit)
-            .replace(np.nan, True)
-            .astype(bool)
-        )
+        if gap_check < 2:
+            # breaks execution down the line and is thus catched here since it basically means "do nothing"
+            return data
+        else:
+            # if there is a limit to the gaps to be interpolated, generate a mask that evaluates to False at the right
+            # side of each too-large gap with a rolling.sum combo
+            gap_mask = data.rolling(gap_limit, min_periods=0).count() > 0
+
+            # correction for initial gap
+            if isinstance(gap_limit, int):
+                gap_mask.iloc[:gap_limit] = True
+
+            if gap_limit == 2:
+                # for the common case of gap_limit=2 (default "harmonisation"), we efficiently back propagate the False
+                # value to fill the whole too-large gap by a shift and a conjunction.
+                gap_mask = gap_mask & gap_mask.shift(-1, fill_value=True)
+            else:
+                # If the gap_size is bigger we make a flip-rolling combo to backpropagate the False values
+                gap_mask = ~(
+                    (~gap_mask[::-1]).rolling(gap_limit, min_periods=0).sum() > 0
+                )[::-1]
 
+    # memorizing the index for later reindexing
     pre_index = data.index
-
-    if data[gap_mask].empty:
+    # drop the gaps that are too large with regard to the gap_limit from the data-to-be interpolated
+    data = data[gap_mask]
+    if data.empty:
         return data
 
-    else:
-        data = data[gap_mask]
-
     if method in ["linear", "time"]:
-
+        # in the case of linear interpolation, not much can go wrong/break so this conditional branch has efficient
+        # finish by just calling pandas interpolation routine to fill the gaps remaining in the data:
         data.interpolate(
-            method=method, inplace=True, limit=inter_limit - 1, limit_area="inside"
+            method=method,
+            inplace=True,
+            limit_area=limit_area,
+            limit_direction=extrapolate,
         )
 
     else:
-        dat_name = data.name
-        gap_mask = (~gap_mask).cumsum()
-        data = pd.merge(gap_mask, data, how="inner", left_index=True, right_index=True)
-
-        def _interpolWrapper(x, wrap_order=order, wrap_method=method):
-            if wrap_order < 0:
-                return x
-            elif x.count() > wrap_order:
-                try:
-                    return x.interpolate(method=wrap_method, order=int(wrap_order))
-                except (NotImplementedError, ValueError):
-                    warnings.warn(
-                        f"Interpolation with method {method} is not supported at order "
-                        f"{wrap_order}. and will be performed at order {wrap_order - 1}"
-                    )
-                    return _interpolWrapper(x, int(wrap_order - 1), wrap_method)
-            elif x.size < 3:
-                return x
-            else:
-                if downgrade_interpolation:
-                    return _interpolWrapper(x, int(x.count() - 1), wrap_method)
-                else:
-                    return x
-
-        data = data.groupby(data.columns[0]).transform(_interpolWrapper)
-        # squeezing the 1-dimensional frame resulting from groupby for consistency
-        # reasons
-        data = data.squeeze(axis=1)
-        data.name = dat_name
+        # if the method that is interpolated with, depends on not only the left and right border points of any gap,
+        # but includes more points, it has to be applied on any data chunk seperated by the too-big gaps individually.
+        # So we use the gap_mask to group the data into chunks and perform the interpolation on every chunk seperatly
+        # with the .transform method of the grouper.
+        gap_mask = (~gap_mask).cumsum()[data.index]
+        chunk_groups = data.groupby(by=gap_mask)
+        data = chunk_groups.transform(
+            _interpolWrapper,
+            **{
+                "order": order,
+                "method": method,
+                "limit_area": limit_area,
+                "limit_direction": extrapolate,
+            },
+        )
+    # finally reinsert the dropped data gaps
     data = data.reindex(pre_index)
-
     return data
 
 
 def aggregate2Freq(
     data: pd.Series,
     method,
     freq,
@@ -595,14 +633,12 @@
 
 
 def linearDriftModel(x, origin, target):
     return origin + x * target
 
 
 def linearInterpolation(data, inter_limit=2):
-    return interpolateNANs(data, "time", inter_limit=inter_limit)
+    return interpolateNANs(data, "time", gap_limit=inter_limit)
 
 
 def polynomialInterpolation(data, inter_limit=2, inter_order=2):
-    return interpolateNANs(
-        data, "polynomial", inter_limit=inter_limit, order=inter_order
-    )
+    return interpolateNANs(data, "polynomial", gap_limit=inter_limit, order=inter_order)
```

### Comparing `saqc-2.3/saqc.egg-info/PKG-INFO` & `saqc-2.4.0/saqc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,369 +1,384 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7361 7163  : 2.1.Name: saqc
-00000020: 0a56 6572 7369 6f6e 3a20 322e 330a 5375  .Version: 2.3.Su
-00000030: 6d6d 6172 793a 2041 2074 696d 6573 6572  mmary: A timeser
-00000040: 6965 7320 6461 7461 2071 7561 6c69 7479  ies data quality
-00000050: 2063 6f6e 7472 6f6c 2061 6e64 2070 726f   control and pro
-00000060: 6365 7373 696e 6720 746f 6f6c 2f66 7261  cessing tool/fra
-00000070: 6d65 776f 726b 0a48 6f6d 652d 7061 6765  mework.Home-page
-00000080: 3a20 6874 7470 733a 2f2f 6769 742e 7566  : https://git.uf
-00000090: 7a2e 6465 2f72 646d 2d73 6f66 7477 6172  z.de/rdm-softwar
-000000a0: 652f 7361 7163 0a41 7574 686f 723a 2042  e/saqc.Author: B
-000000b0: 6572 7420 5061 6c6d 2c20 4461 7669 6420  ert Palm, David 
-000000c0: 5363 6861 6566 6572 2c20 466c 6f72 6961  Schaefer, Floria
-000000d0: 6e20 4772 616e 7365 652c 2050 6574 6572  n Gransee, Peter
-000000e0: 204c 7565 6e65 6e73 6368 6c6f 7373 0a41   Luenenschloss.A
-000000f0: 7574 686f 722d 656d 6169 6c3a 2064 6176  uthor-email: dav
-00000100: 6964 2e73 6368 6165 6665 7240 7566 7a2e  id.schaefer@ufz.
-00000110: 6465 0a52 6571 7569 7265 732d 5079 7468  de.Requires-Pyth
-00000120: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
-00000130: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000140: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000150: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000160: 4c49 4345 4e53 452e 6d64 0a4c 6963 656e  LICENSE.md.Licen
-00000170: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000180: 532f 4750 4c2d 332e 302d 6f72 2d6c 6174  S/GPL-3.0-or-lat
-00000190: 6572 2e74 7874 0a0a 3c21 2d2d 0a53 5044  er.txt..<!--.SPD
-000001a0: 582d 4669 6c65 436f 7079 7269 6768 7454  X-FileCopyrightT
-000001b0: 6578 743a 2032 3032 3120 4865 6c6d 686f  ext: 2021 Helmho
-000001c0: 6c74 7a2d 5a65 6e74 7275 6d20 66c3 bc72  ltz-Zentrum f..r
-000001d0: 2055 6d77 656c 7466 6f72 7363 6875 6e67   Umweltforschung
-000001e0: 2047 6d62 4820 2d20 5546 5a0a 0a53 5044   GmbH - UFZ..SPD
-000001f0: 582d 4c69 6365 6e73 652d 4964 656e 7469  X-License-Identi
-00000200: 6669 6572 3a20 4750 4c2d 332e 302d 6f72  fier: GPL-3.0-or
-00000210: 2d6c 6174 6572 0a2d 2d3e 0a0a 3c61 2068  -later.-->..<a h
-00000220: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
-00000230: 2e75 667a 2e64 652f 696e 6465 782e 7068  .ufz.de/index.ph
-00000240: 703f 656e 3d33 3335 3733 223e 0a20 2020  p?en=33573">.   
-00000250: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000260: 3a2f 2f67 6974 2e75 667a 2e64 652f 7264  ://git.ufz.de/rd
-00000270: 6d2d 736f 6674 7761 7265 2f73 6171 632f  m-software/saqc/
-00000280: 7261 772f 6465 7665 6c6f 702f 646f 6373  raw/develop/docs
-00000290: 2f72 6573 6f75 7263 6573 2f69 6d61 6765  /resources/image
-000002a0: 732f 7265 7072 6573 656e 7461 7469 7665  s/representative
-000002b0: 2f55 465a 4c6f 676f 2e70 6e67 2220 7769  /UFZLogo.png" wi
-000002c0: 6474 683d 2234 3030 222f 3e0a 3c2f 613e  dth="400"/>.</a>
-000002d0: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-000002e0: 3a2f 2f77 7777 2e75 667a 2e64 652f 696e  ://www.ufz.de/in
-000002f0: 6465 782e 7068 703f 656e 3d34 3533 3438  dex.php?en=45348
-00000300: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
-00000310: 2268 7474 7073 3a2f 2f67 6974 2e75 667a  "https://git.ufz
-00000320: 2e64 652f 7264 6d2d 736f 6674 7761 7265  .de/rdm-software
-00000330: 2f73 6171 632f 7261 772f 6465 7665 6c6f  /saqc/raw/develo
-00000340: 702f 646f 6373 2f72 6573 6f75 7263 6573  p/docs/resources
-00000350: 2f69 6d61 6765 732f 7265 7072 6573 656e  /images/represen
-00000360: 7461 7469 7665 2f52 444d 4c6f 676f 2e70  tative/RDMLogo.p
-00000370: 6e67 2220 616c 6967 6e3d 2272 6967 6874  ng" align="right
-00000380: 2220 7769 6474 683d 2232 3230 222f 3e0a  " width="220"/>.
-00000390: 3c2f 613e 0a0a 5b21 5b50 726f 6a65 6374  </a>..[![Project
-000003a0: 2053 7461 7475 733a 2041 6374 6976 6520   Status: Active 
-000003b0: e280 9320 5468 6520 7072 6f6a 6563 7420  ... The project 
-000003c0: 6861 7320 7265 6163 6865 6420 6120 7374  has reached a st
-000003d0: 6162 6c65 2c20 7573 6162 6c65 2073 7461  able, usable sta
-000003e0: 7465 2061 6e64 2069 7320 6265 696e 6720  te and is being 
-000003f0: 6163 7469 7665 6c79 2064 6576 656c 6f70  actively develop
-00000400: 6564 2e5d 2868 7474 7073 3a2f 2f77 7777  ed.](https://www
-00000410: 2e72 6570 6f73 7461 7475 732e 6f72 672f  .repostatus.org/
-00000420: 6261 6467 6573 2f6c 6174 6573 742f 6163  badges/latest/ac
-00000430: 7469 7665 2e73 7667 295d 2868 7474 7073  tive.svg)](https
-00000440: 3a2f 2f77 7777 2e72 6570 6f73 7461 7475  ://www.repostatu
-00000450: 732e 6f72 672f 2361 6374 6976 6529 0a0a  s.org/#active)..
-00000460: 0a23 2053 7973 7465 6d20 666f 7220 6175  .# System for au
-00000470: 746f 6d61 7465 6420 5175 616c 6974 7920  tomated Quality 
-00000480: 436f 6e74 726f 6c20 2853 6151 4329 0a0a  Control (SaQC)..
-00000490: 416e 6f6d 616c 6965 7320 616e 6420 6572  Anomalies and er
-000004a0: 726f 7273 2061 7265 2074 6865 2072 756c  rors are the rul
-000004b0: 6520 6e6f 7420 7468 6520 6578 6365 7074  e not the except
-000004c0: 696f 6e20 7768 656e 2077 6f72 6b69 6e67  ion when working
-000004d0: 2077 6974 6820 0a74 696d 6520 7365 7269   with .time seri
-000004e0: 6573 2064 6174 612e 2054 6869 7320 6973  es data. This is
-000004f0: 2065 7370 6563 6961 6c6c 7920 7472 7565   especially true
-00000500: 2c20 6966 2073 7563 6820 6461 7461 206f  , if such data o
-00000510: 7269 6769 6e61 7465 730a 6672 6f6d 2069  riginates.from i
-00000520: 6e2d 7369 7475 206d 6561 7375 7265 6d65  n-situ measureme
-00000530: 6e74 7320 6f66 2065 6e76 6972 6f6e 6d65  nts of environme
-00000540: 6e74 616c 2070 726f 7065 7274 6965 732e  ntal properties.
-00000550: 200a 416c 6d6f 7374 2061 6c6c 2061 7070   .Almost all app
-00000560: 6c69 6361 7469 6f6e 732c 2068 6f77 6576  lications, howev
-00000570: 6572 2c20 696d 706c 6963 696c 7920 7265  er, implicily re
-00000580: 6c79 206f 6e20 6461 7461 2c20 7468 6174  ly on data, that
-00000590: 2063 6f6d 706c 6965 730a 7769 7468 2073   complies.with s
-000005a0: 6f6d 6520 6465 6669 6e69 7469 6f6e 206f  ome definition o
-000005b0: 6620 2763 6f72 7265 6374 272e 200a 496e  f 'correct'. .In
-000005c0: 206f 7264 6572 2074 6f20 696e 6665 7220   order to infer 
-000005d0: 7265 6c69 6162 6c65 2064 6174 6120 7072  reliable data pr
-000005e0: 6f64 7563 7473 2061 6e64 2074 6f6f 6c73  oducts and tools
-000005f0: 2c20 7468 6572 6520 6973 206e 6f20 616c  , there is no al
-00000600: 7465 726e 6174 6976 650a 746f 2071 7561  ternative.to qua
-00000610: 6c69 7479 2063 6f6e 7472 6f6c 2e20 5361  lity control. Sa
-00000620: 5143 2070 726f 7669 6465 7320 616c 6c20  QC provides all 
-00000630: 7468 6520 6275 696c 6469 6e67 2062 6c6f  the building blo
-00000640: 636b 7320 746f 2063 6f6d 666f 7274 6162  cks to comfortab
-00000650: 6c79 0a62 7269 6467 6520 7468 6520 6761  ly.bridge the ga
-00000660: 7020 6265 7477 6565 6e20 2775 7375 616c  p between 'usual
-00000670: 6c79 2066 6175 6c74 7927 2061 6e64 2027  ly faulty' and '
-00000680: 6578 7065 6374 6564 2074 6f20 6265 2063  expected to be c
-00000690: 6f72 7265 6374 6564 2720 696e 200a 6120  orrected' in .a 
-000006a0: 6163 6365 7373 6962 6c65 2c20 636f 6e73  accessible, cons
-000006b0: 6973 7465 6e74 2c20 6f62 6a65 6374 6976  istent, objectiv
-000006c0: 6520 616e 6420 7265 7072 6f64 7563 6962  e and reproducib
-000006d0: 6c65 2077 6179 2e0a 0a46 6f72 2061 2028  le way...For a (
-000006e0: 636f 6e74 696e 6f75 736c 7920 696d 7072  continously impr
-000006f0: 6f76 696e 6729 206f 7665 7276 6965 7720  oving) overview 
-00000700: 6f66 2066 6561 7475 7265 732c 2074 7970  of features, typ
-00000710: 6963 616c 2075 7361 6765 2070 6174 7465  ical usage patte
-00000720: 726e 732c 0a74 6865 2073 7065 6369 6669  rns,.the specifi
-00000730: 6320 7379 7374 656d 2063 6f6d 706f 6e65  c system compone
-00000740: 6e74 7320 616e 6420 686f 7720 746f 2063  nts and how to c
-00000750: 7573 746f 6d69 7a65 2060 5361 5143 6020  ustomize `SaQC` 
-00000760: 746f 2079 6f75 7220 7370 6563 6966 6963  to your specific
-00000770: 0a6e 6565 6473 2c20 706c 6561 7365 2072  .needs, please r
-00000780: 6566 6572 2074 6f20 6f75 720a 5b6f 6e6c  efer to our.[onl
-00000790: 696e 6520 646f 6375 6d65 6e74 6174 696f  ine documentatio
-000007a0: 6e5d 2868 7474 7073 3a2f 2f72 646d 2d73  n](https://rdm-s
-000007b0: 6f66 7477 6172 652e 7061 6765 732e 7566  oftware.pages.uf
-000007c0: 7a2e 6465 2f73 6171 632f 696e 6465 782e  z.de/saqc/index.
-000007d0: 6874 6d6c 292e 0a0a 0a23 2320 496e 7374  html)....## Inst
-000007e0: 616c 6c61 7469 6f6e 0a0a 5361 5143 2069  allation..SaQC i
-000007f0: 7320 6176 6169 6c61 626c 6520 6f6e 2074  s available on t
-00000800: 6865 2050 7974 686f 6e20 5061 636b 6167  he Python Packag
-00000810: 6520 496e 6465 7820 285b 5079 5049 5d28  e Index ([PyPI](
-00000820: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000830: 2f29 2920 616e 640a 6361 6e20 6265 2069  /)) and.can be i
-00000840: 6e73 7461 6c6c 6564 2075 7369 6e67 205b  nstalled using [
-00000850: 7069 705d 2868 7474 7073 3a2f 2f70 6970  pip](https://pip
-00000860: 2e70 7970 612e 696f 2f65 6e2f 7374 6162  .pypa.io/en/stab
-00000870: 6c65 2f29 3a0a 6060 6073 680a 7079 7468  le/):.```sh.pyth
-00000880: 6f6e 202d 6d20 7069 7020 696e 7374 616c  on -m pip instal
-00000890: 6c20 7361 7163 0a60 6060 0a46 6f72 2061  l saqc.```.For a
-000008a0: 206d 6f72 6520 6465 7461 696c 6564 2069   more detailed i
-000008b0: 6e73 7461 6c6c 696f 6e20 6775 6964 652c  nstallion guide,
-000008c0: 2073 6565 2074 6865 205b 696e 7374 616c   see the [instal
-000008d0: 6c61 7469 6f6e 2067 7569 6465 5d28 6874  lation guide](ht
-000008e0: 7470 733a 2f2f 7264 6d2d 736f 6674 7761  tps://rdm-softwa
-000008f0: 7265 2e70 6167 6573 2e75 667a 2e64 652f  re.pages.ufz.de/
-00000900: 7361 7163 2f67 6574 7469 6e67 7374 6172  saqc/gettingstar
-00000910: 7465 642f 496e 7374 616c 6c61 7469 6f6e  ted/Installation
-00000920: 4775 6964 652e 6874 6d6c 292e 0a0a 2323  Guide.html)...##
-00000930: 2055 7361 6765 0a0a 6053 6151 4360 2069   Usage..`SaQC` i
-00000940: 7320 626f 7468 2c20 6120 636f 6d6d 616e  s both, a comman
-00000950: 6420 6c69 6e65 2061 7070 6c69 6361 7469  d line applicati
-00000960: 6f6e 2063 6f6e 7472 6f6c 6c65 6420 6279  on controlled by
-00000970: 2061 2074 6578 7420 6261 7365 6420 636f   a text based co
-00000980: 6e66 6967 7572 6174 696f 6e0a 616e 6420  nfiguration.and 
-00000990: 6120 7079 7468 6f6e 206d 6f64 756c 6520  a python module 
-000009a0: 7769 7468 2061 2073 696d 706c 6520 4150  with a simple AP
-000009b0: 492e 0a0a 2323 2320 5361 5143 2061 7320  I...### SaQC as 
-000009c0: 6120 636f 6d6d 616e 6420 6c69 6e65 2061  a command line a
-000009d0: 7070 6c69 6361 7469 6f6e 0a54 6865 2063  pplication.The c
-000009e0: 6f6d 6d61 6e64 206c 696e 6520 6170 706c  ommand line appl
-000009f0: 6963 6174 696f 6e20 6973 2063 6f6e 7472  ication is contr
-00000a00: 6f6c 6c65 6420 6279 2061 2073 656d 6963  olled by a semic
-00000a10: 6f6c 6f6e 2d73 6570 6172 6174 6564 2074  olon-separated t
-00000a20: 6578 740a 6669 6c65 206c 6973 7469 6e67  ext.file listing
-00000a30: 2074 6865 2076 6172 6961 626c 6573 2069   the variables i
-00000a40: 6e20 7468 6520 6461 7461 7365 7420 616e  n the dataset an
-00000a50: 6420 7468 6520 726f 7574 696e 6573 2074  d the routines t
-00000a60: 6f20 696e 7370 6563 742c 0a71 7561 6c69  o inspect,.quali
-00000a70: 7479 2063 6f6e 7472 6f6c 2061 6e64 2f6f  ty control and/o
-00000a80: 7220 7072 6f63 6573 7320 7468 656d 2e20  r process them. 
-00000a90: 5468 6520 636f 6e74 656e 7420 6f66 2073  The content of s
-00000aa0: 7563 6820 6120 636f 6e66 6967 7572 6174  uch a configurat
-00000ab0: 696f 6e0a 636f 756c 6420 6c6f 6f6b 206c  ion.could look l
-00000ac0: 696b 6520 5b74 6869 735d 2868 7474 7073  ike [this](https
-00000ad0: 3a2f 2f67 6974 2e75 667a 2e64 652f 7264  ://git.ufz.de/rd
-00000ae0: 6d2d 736f 6674 7761 7265 2f73 6171 632f  m-software/saqc/
-00000af0: 7261 772f 6465 7665 6c6f 702f 646f 6373  raw/develop/docs
-00000b00: 2f72 6573 6f75 7263 6573 2f64 6174 612f  /resources/data/
-00000b10: 636f 6e66 6967 2e63 7376 293a 0a0a 6060  config.csv):..``
-00000b20: 600a 7661 726e 616d 6520 2020 203b 2074  `.varname    ; t
-00000b30: 6573 740a 232d 2d2d 2d2d 2d2d 2d2d 2d3b  est.#----------;
-00000b40: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000b80: 2d2d 2d2d 2d2d 0a53 4d32 2020 2020 2020  ------.SM2      
-00000b90: 2020 3b20 7368 6966 7428 6672 6571 3d22    ; shift(freq="
-00000ba0: 3135 4d69 6e22 290a 2753 4d28 317c 3229  15Min").'SM(1|2)
-00000bb0: 2b27 203b 2066 6c61 674d 6973 7369 6e67  +' ; flagMissing
-00000bc0: 2829 0a53 4d31 2020 2020 2020 2020 3b20  ().SM1        ; 
-00000bd0: 666c 6167 5261 6e67 6528 6d69 6e3d 3130  flagRange(min=10
-00000be0: 2c20 6d61 783d 3630 290a 534d 3220 2020  , max=60).SM2   
-00000bf0: 2020 2020 203b 2066 6c61 6752 616e 6765       ; flagRange
-00000c00: 286d 696e 3d31 302c 206d 6178 3d34 3029  (min=10, max=40)
-00000c10: 0a53 4d32 2020 2020 2020 2020 3b20 666c  .SM2        ; fl
-00000c20: 6167 4d41 4428 7769 6e64 6f77 3d22 3330  agMAD(window="30
-00000c30: 6422 2c20 7a3d 332e 3529 0a44 756d 6d79  d", z=3.5).Dummy
-00000c40: 2020 2020 2020 3b20 666c 6167 4765 6e65        ; flagGene
-00000c50: 7269 6328 6669 656c 643d 5b22 534d 3122  ric(field=["SM1"
-00000c60: 2c20 2253 4d32 225d 2c20 6675 6e63 3d28  , "SM2"], func=(
-00000c70: 6973 666c 6167 6765 6428 7829 207c 2069  isflagged(x) | i
-00000c80: 7366 6c61 6767 6564 2879 2929 290a 6060  sflagged(y))).``
-00000c90: 600a 0a41 7320 736f 6f6e 2061 7320 7468  `..As soon as th
-00000ca0: 6520 6261 7369 6320 696e 7075 7473 2c20  e basic inputs, 
-00000cb0: 6461 7461 7365 7420 616e 6420 636f 6e66  dataset and conf
-00000cc0: 6967 7572 6174 696f 6e20 6669 6c65 2c20  iguration file, 
-00000cd0: 6172 650a 7072 6570 6172 6564 2c20 7275  are.prepared, ru
-00000ce0: 6e20 6053 6151 4360 3a0a 6060 6073 680a  n `SaQC`:.```sh.
-00000cf0: 7361 7163 205c 0a20 2020 202d 2d63 6f6e  saqc \.    --con
-00000d00: 6669 6720 5041 5448 5f54 4f5f 434f 4e46  fig PATH_TO_CONF
-00000d10: 4947 5552 4154 494f 4e20 5c0a 2020 2020  IGURATION \.    
-00000d20: 2d2d 6461 7461 2050 4154 485f 544f 5f44  --data PATH_TO_D
-00000d30: 4154 4120 5c0a 2020 2020 2d2d 6f75 7466  ATA \.    --outf
-00000d40: 696c 6520 5041 5448 5f54 4f5f 4f55 5450  ile PATH_TO_OUTP
-00000d50: 5554 0a60 6060 0a0a 4120 6675 6c6c 2060  UT.```..A full `
-00000d60: 5361 5143 6020 7275 6e20 6167 6169 6e73  SaQC` run agains
-00000d70: 7420 7072 6f76 6964 6564 2065 7861 6d70  t provided examp
-00000d80: 6c65 2064 6174 6120 6361 6e20 6265 2069  le data can be i
-00000d90: 6e76 6f6b 6564 2077 6974 683a 0a60 6060  nvoked with:.```
-00000da0: 7368 0a73 6171 6320 5c0a 2020 2020 2d2d  sh.saqc \.    --
-00000db0: 636f 6e66 6967 2068 7474 7073 3a2f 2f67  config https://g
-00000dc0: 6974 2e75 667a 2e64 652f 7264 6d2d 736f  it.ufz.de/rdm-so
-00000dd0: 6674 7761 7265 2f73 6171 632f 7261 772f  ftware/saqc/raw/
-00000de0: 6465 7665 6c6f 702f 646f 6373 2f72 6573  develop/docs/res
-00000df0: 6f75 7263 6573 2f64 6174 612f 636f 6e66  ources/data/conf
-00000e00: 6967 2e63 7376 205c 0a20 2020 202d 2d64  ig.csv \.    --d
-00000e10: 6174 6120 6874 7470 733a 2f2f 6769 742e  ata https://git.
-00000e20: 7566 7a2e 6465 2f72 646d 2d73 6f66 7477  ufz.de/rdm-softw
-00000e30: 6172 652f 7361 7163 2f72 6177 2f64 6576  are/saqc/raw/dev
-00000e40: 656c 6f70 2f64 6f63 732f 7265 736f 7572  elop/docs/resour
-00000e50: 6365 732f 6461 7461 2f64 6174 612e 6373  ces/data/data.cs
-00000e60: 7620 5c0a 2020 2020 2d2d 6f75 7466 696c  v \.    --outfil
-00000e70: 6520 7361 7163 5f74 6573 742e 6373 760a  e saqc_test.csv.
-00000e80: 6060 600a 0a23 2323 2053 6151 4320 6173  ```..### SaQC as
-00000e90: 2061 2070 7974 686f 6e20 6d6f 6475 6c65   a python module
-00000ea0: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-00000eb0: 736e 6970 7065 7420 696d 706c 656d 656e  snippet implemen
-00000ec0: 7473 2074 6865 2073 616d 6520 636f 6e66  ts the same conf
-00000ed0: 6967 7572 6174 696f 6e20 6769 7665 6e20  iguration given 
-00000ee0: 6162 6f76 6520 7468 726f 7567 680a 7468  above through.th
-00000ef0: 6520 5079 7468 6f6e 2d41 5049 3a0a 0a60  e Python-API:..`
-00000f00: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00000f10: 7061 6e64 6173 2061 7320 7064 0a66 726f  pandas as pd.fro
-00000f20: 6d20 7361 7163 2069 6d70 6f72 7420 5361  m saqc import Sa
-00000f30: 5143 0a0a 6461 7461 203d 2070 642e 7265  QC..data = pd.re
-00000f40: 6164 5f63 7376 280a 2020 2020 2268 7474  ad_csv(.    "htt
-00000f50: 7073 3a2f 2f67 6974 2e75 667a 2e64 652f  ps://git.ufz.de/
-00000f60: 7264 6d2d 736f 6674 7761 7265 2f73 6171  rdm-software/saq
-00000f70: 632f 7261 772f 6465 7665 6c6f 702f 646f  c/raw/develop/do
-00000f80: 6373 2f72 6573 6f75 7263 6573 2f64 6174  cs/resources/dat
-00000f90: 612f 6461 7461 2e63 7376 222c 0a20 2020  a/data.csv",.   
-00000fa0: 2069 6e64 6578 5f63 6f6c 3d30 2c20 7061   index_col=0, pa
-00000fb0: 7273 655f 6461 7465 733d 5472 7565 2c0a  rse_dates=True,.
-00000fc0: 290a 0a73 6171 6320 3d20 5361 5143 2864  )..saqc = SaQC(d
-00000fd0: 6174 613d 6461 7461 290a 7361 7163 203d  ata=data).saqc =
-00000fe0: 2028 7361 7163 0a20 2020 2020 2020 202e   (saqc.        .
-00000ff0: 7368 6966 7428 2253 4d32 222c 2066 7265  shift("SM2", fre
-00001000: 713d 2231 354d 696e 2229 0a20 2020 2020  q="15Min").     
-00001010: 2020 202e 666c 6167 4d69 7373 696e 6728     .flagMissing(
-00001020: 2253 4d28 317c 3229 2b22 2c20 7265 6765  "SM(1|2)+", rege
-00001030: 783d 5472 7565 290a 2020 2020 2020 2020  x=True).        
-00001040: 2e66 6c61 6752 616e 6765 2822 534d 3122  .flagRange("SM1"
-00001050: 2c20 6d69 6e3d 3130 2c20 6d61 783d 3630  , min=10, max=60
-00001060: 290a 2020 2020 2020 2020 2e66 6c61 6752  ).        .flagR
-00001070: 616e 6765 2822 534d 3222 2c20 6d69 6e3d  ange("SM2", min=
-00001080: 3130 2c20 6d61 783d 3430 290a 2020 2020  10, max=40).    
-00001090: 2020 2020 2e66 6c61 674d 4144 2822 534d      .flagMAD("SM
-000010a0: 3222 2c20 7769 6e64 6f77 3d22 3330 6422  2", window="30d"
-000010b0: 2c20 7a3d 332e 3529 0a20 2020 2020 2020  , z=3.5).       
-000010c0: 202e 666c 6167 4765 6e65 7269 6328 6669   .flagGeneric(fi
-000010d0: 656c 643d 5b22 534d 3122 2c20 2253 4d32  eld=["SM1", "SM2
-000010e0: 225d 2c20 7461 7267 6574 3d22 4475 6d6d  "], target="Dumm
-000010f0: 7922 2c20 6675 6e63 3d6c 616d 6264 6120  y", func=lambda 
-00001100: 782c 2079 3a20 2869 7366 6c61 6767 6564  x, y: (isflagged
-00001110: 2878 2920 7c20 6973 666c 6167 6765 6428  (x) | isflagged(
-00001120: 7929 2929 290a 6060 600a 0a41 206d 6f72  y)))).```..A mor
-00001130: 6520 6465 7461 696c 6564 2064 6573 6372  e detailed descr
-00001140: 6970 7469 6f6e 206f 6620 7468 6520 5079  iption of the Py
-00001150: 7468 6f6e 2041 5049 2069 7320 6176 6169  thon API is avai
-00001160: 6c61 626c 6520 696e 2074 6865 200a 5b72  lable in the .[r
-00001170: 6573 7065 6374 6976 6520 7365 6374 696f  espective sectio
-00001180: 6e5d 2868 7474 7073 3a2f 2f72 646d 2d73  n](https://rdm-s
-00001190: 6f66 7477 6172 652e 7061 6765 732e 7566  oftware.pages.uf
-000011a0: 7a2e 6465 2f73 6171 632f 6765 7474 696e  z.de/saqc/gettin
-000011b0: 6773 7461 7274 6564 2f54 7574 6f72 6961  gstarted/Tutoria
-000011c0: 6c41 5049 2e68 746d 6c29 0a6f 6620 7468  lAPI.html).of th
-000011d0: 6520 646f 6375 6d65 6e74 6174 696f 6e2e  e documentation.
-000011e0: 0a0a 2323 2043 6861 6e67 656c 6f67 0a41  ..## Changelog.A
-000011f0: 6c6c 206e 6f74 6162 6c65 2063 6861 6e67  ll notable chang
-00001200: 6573 2074 6f20 7468 6973 2070 726f 6a65  es to this proje
-00001210: 6374 2077 696c 6c20 6265 2064 6f63 756d  ct will be docum
-00001220: 656e 7465 6420 696e 205b 4348 414e 4745  ented in [CHANGE
-00001230: 4c4f 472e 6d64 5d28 4348 414e 4745 4c4f  LOG.md](CHANGELO
-00001240: 472e 6d64 292e 0a0a 2323 2047 6574 2069  G.md)...## Get i
-00001250: 6e76 6f6c 7665 640a 0a23 2323 2043 6f6e  nvolved..### Con
-00001260: 7472 6962 7574 696e 670a 596f 7520 666f  tributing.You fo
-00001270: 756e 6420 6120 6275 6720 6f72 2079 6f75  und a bug or you
-00001280: 2077 616e 7420 746f 2073 7567 6765 7374   want to suggest
-00001290: 2073 6f6d 6520 636f 6f6c 2066 6561 7475   some cool featu
-000012a0: 7265 733f 2050 6c65 6173 6520 7265 6665  res? Please refe
-000012b0: 7220 746f 206f 7572 205b 636f 6e74 7269  r to our [contri
-000012c0: 6275 7469 6e67 2067 7569 6465 6c69 6e65  buting guideline
-000012d0: 735d 2843 4f4e 5452 4942 5554 494e 472e  s](CONTRIBUTING.
-000012e0: 6d64 2920 746f 2073 6565 2068 6f77 2079  md) to see how y
-000012f0: 6f75 2063 616e 2063 6f6e 7472 6962 7574  ou can contribut
-00001300: 6520 746f 2053 6151 432e 0a0a 2323 2320  e to SaQC...### 
-00001310: 5573 6572 2073 7570 706f 7274 0a49 6620  User support.If 
-00001320: 796f 7520 6e65 6564 2068 656c 7020 6f72  you need help or
-00001330: 2068 6176 6520 6120 7175 6573 7469 6f6e   have a question
-00001340: 2c20 796f 7520 6361 6e20 7573 6520 7468  , you can use th
-00001350: 6520 5361 5143 2075 7365 7220 7375 7070  e SaQC user supp
-00001360: 6f72 7420 6d61 696c 696e 6720 6c69 7374  ort mailing list
-00001370: 3a20 5b73 6171 632d 7375 7070 6f72 7440  : [saqc-support@
-00001380: 7566 7a2e 6465 5d28 6d61 696c 746f 3a73  ufz.de](mailto:s
-00001390: 6171 632d 7375 7070 6f72 7440 7566 7a2e  aqc-support@ufz.
-000013a0: 6465 290a 0a23 2320 436f 7079 7269 6768  de)..## Copyrigh
-000013b0: 7420 616e 6420 4c69 6365 6e73 650a 436f  t and License.Co
-000013c0: 7079 7269 6768 7428 6329 2032 3032 312c  pyright(c) 2021,
-000013d0: 205b 4865 6c6d 686f 6c74 7a2d 5a65 6e74   [Helmholtz-Zent
-000013e0: 7275 6d20 66c3 bc72 2055 6d77 656c 7466  rum f..r Umweltf
-000013f0: 6f72 7363 6875 6e67 2047 6d62 4820 2d2d  orschung GmbH --
-00001400: 2055 465a 5d28 6874 7470 733a 2f2f 7777   UFZ](https://ww
-00001410: 772e 7566 7a2e 6465 292e 2041 6c6c 2072  w.ufz.de). All r
-00001420: 6967 6874 7320 7265 7365 7276 6564 2e0a  ights reserved..
-00001430: 0a2d 2044 6f63 756d 656e 7461 7469 6f6e  .- Documentation
-00001440: 3a20 5b43 7265 6174 6976 6520 436f 6d6d  : [Creative Comm
-00001450: 6f6e 7320 4174 7472 6962 7574 696f 6e20  ons Attribution 
-00001460: 342e 3020 496e 7465 726e 6174 696f 6e61  4.0 Internationa
-00001470: 6c5d 2868 7474 7073 3a2f 2f63 7265 6174  l](https://creat
-00001480: 6976 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c  ivecommons.org/l
-00001490: 6963 656e 7365 732f 6279 2f34 2e30 2f29  icenses/by/4.0/)
-000014a0: 203c 6120 7265 6c3d 226c 6963 656e 7365   <a rel="license
-000014b0: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-000014c0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-000014d0: 7267 2f6c 6963 656e 7365 732f 6279 2f34  rg/licenses/by/4
-000014e0: 2e30 2f22 3e3c 696d 6720 616c 743d 2243  .0/"><img alt="C
-000014f0: 7265 6174 6976 6520 436f 6d6d 6f6e 7320  reative Commons 
-00001500: 4c69 6365 6e73 6522 2073 7479 6c65 3d22  License" style="
-00001510: 626f 7264 6572 2d77 6964 7468 3a30 2220  border-width:0" 
-00001520: 7372 633d 2268 7474 7073 3a2f 2f69 2e63  src="https://i.c
-00001530: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-00001540: 7267 2f6c 2f62 792f 342e 302f 3830 7831  rg/l/by/4.0/80x1
-00001550: 352e 706e 6722 202f 3e3c 2f61 3e0a 2d20  5.png" /></a>.- 
-00001560: 536f 7572 6365 2063 6f64 653a 205b 474e  Source code: [GN
-00001570: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-00001580: 204c 6963 656e 7365 2033 5d28 6874 7470   License 3](http
-00001590: 733a 2f2f 7777 772e 676e 752e 6f72 672f  s://www.gnu.org/
-000015a0: 6c69 6365 6e73 6573 2f67 706c 2d33 2e30  licenses/gpl-3.0
-000015b0: 2e68 746d 6c29 0a0a 466f 7220 6675 6c6c  .html)..For full
-000015c0: 2064 6574 6169 6c73 2c20 7365 6520 5b4c   details, see [L
-000015d0: 4943 454e 5345 5d28 4c49 4345 4e53 452e  ICENSE](LICENSE.
-000015e0: 6d64 292e 0a0a 2323 2041 636b 6e6f 776c  md)...## Acknowl
-000015f0: 6564 6765 6d65 6e74 730a 2e2e 2e0a 0a23  edgements......#
-00001600: 2320 5075 626c 6963 6174 696f 6e73 0a63  # Publications.c
-00001610: 6f6d 696e 6720 736f 6f6e 2e2e 2e0a 0a23  oming soon.....#
-00001620: 2320 486f 7720 746f 2063 6974 6520 5361  # How to cite Sa
-00001630: 5143 0a49 6620 5361 5143 2069 7320 6164  QC.If SaQC is ad
-00001640: 7661 6e63 696e 6720 796f 7572 2072 6573  vancing your res
-00001650: 6561 7263 682c 2070 6c65 6173 6520 6369  earch, please ci
-00001660: 7465 2061 733a 0a0a 3e20 5363 68c3 a466  te as:..> Sch..f
-00001670: 6572 2c20 4461 7669 643b 2050 616c 6d2c  er, David; Palm,
-00001680: 2042 6572 743b 204c c3bc 6e65 6e73 6368   Bert; L..nensch
-00001690: 6c6f c39f 2c20 5065 7465 722e 2028 3230  lo.., Peter. (20
-000016a0: 3231 292e 2053 7973 7465 6d20 666f 7220  21). System for 
-000016b0: 6175 746f 6d61 7465 6420 5175 616c 6974  automated Qualit
-000016c0: 7920 436f 6e74 726f 6c20 2d20 5361 5143  y Control - SaQC
-000016d0: 2e20 5a65 6e6f 646f 2e20 6874 7470 733a  . Zenodo. https:
-000016e0: 2f2f 646f 692e 6f72 672f 3130 2e35 3238  //doi.org/10.528
-000016f0: 312f 7a65 6e6f 646f 2e35 3838 3835 3437  1/zenodo.5888547
-00001700: 0a                                       .
+00000020: 0a56 6572 7369 6f6e 3a20 322e 342e 300a  .Version: 2.4.0.
+00000030: 5375 6d6d 6172 793a 2041 2074 696d 6573  Summary: A times
+00000040: 6572 6965 7320 6461 7461 2071 7561 6c69  eries data quali
+00000050: 7479 2063 6f6e 7472 6f6c 2061 6e64 2070  ty control and p
+00000060: 726f 6365 7373 696e 6720 746f 6f6c 2f66  rocessing tool/f
+00000070: 7261 6d65 776f 726b 0a48 6f6d 652d 7061  ramework.Home-pa
+00000080: 6765 3a20 6874 7470 733a 2f2f 6769 742e  ge: https://git.
+00000090: 7566 7a2e 6465 2f72 646d 2d73 6f66 7477  ufz.de/rdm-softw
+000000a0: 6172 652f 7361 7163 0a41 7574 686f 723a  are/saqc.Author:
+000000b0: 2042 6572 7420 5061 6c6d 2c20 4461 7669   Bert Palm, Davi
+000000c0: 6420 5363 6861 6566 6572 2c20 466c 6f72  d Schaefer, Flor
+000000d0: 6961 6e20 4772 616e 7365 652c 2050 6574  ian Gransee, Pet
+000000e0: 6572 204c 7565 6e65 6e73 6368 6c6f 7373  er Luenenschloss
+000000f0: 0a41 7574 686f 722d 656d 6169 6c3a 2064  .Author-email: d
+00000100: 6176 6964 2e73 6368 6165 6665 7240 7566  avid.schaefer@uf
+00000110: 7a2e 6465 0a52 6571 7569 7265 732d 5079  z.de.Requires-Py
+00000120: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
+00000130: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000140: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000150: 6f77 6e0a 4c69 6365 6e73 652d 4669 6c65  own.License-File
+00000160: 3a20 4c49 4345 4e53 452e 6d64 0a4c 6963  : LICENSE.md.Lic
+00000170: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000180: 5345 532f 4750 4c2d 332e 302d 6f72 2d6c  SES/GPL-3.0-or-l
+00000190: 6174 6572 2e74 7874 0a0a 3c21 2d2d 0a53  ater.txt..<!--.S
+000001a0: 5044 582d 4669 6c65 436f 7079 7269 6768  PDX-FileCopyrigh
+000001b0: 7454 6578 743a 2032 3032 3120 4865 6c6d  tText: 2021 Helm
+000001c0: 686f 6c74 7a2d 5a65 6e74 7275 6d20 66c3  holtz-Zentrum f.
+000001d0: bc72 2055 6d77 656c 7466 6f72 7363 6875  .r Umweltforschu
+000001e0: 6e67 2047 6d62 4820 2d20 5546 5a0a 0a53  ng GmbH - UFZ..S
+000001f0: 5044 582d 4c69 6365 6e73 652d 4964 656e  PDX-License-Iden
+00000200: 7469 6669 6572 3a20 4750 4c2d 332e 302d  tifier: GPL-3.0-
+00000210: 6f72 2d6c 6174 6572 0a2d 2d3e 0a0a 3c62  or-later.-->..<b
+00000220: 723e 0a3c 6469 7620 616c 6967 6e3d 2263  r>.<div align="c
+00000230: 656e 7465 7222 3e0a 2020 3c69 6d67 2073  enter">.  <img s
+00000240: 7263 3d22 6874 7470 733a 2f2f 6769 742e  rc="https://git.
+00000250: 7566 7a2e 6465 2f72 646d 2d73 6f66 7477  ufz.de/rdm-softw
+00000260: 6172 652f 7361 7163 2f72 6177 2f64 6576  are/saqc/raw/dev
+00000270: 656c 6f70 2f64 6f63 732f 7265 736f 7572  elop/docs/resour
+00000280: 6365 732f 696d 6167 6573 2f72 6570 7265  ces/images/repre
+00000290: 7365 6e74 6174 6976 652f 5361 5143 4c6f  sentative/SaQCLo
+000002a0: 676f 2e70 6e67 2220 7769 6474 683d 2233  go.png" width="3
+000002b0: 3030 223e 0a3c 2f64 6976 3e0a 0a2d 2d2d  00">.</div>..---
+000002c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a5b  --------------.[
+000002d0: 215b 5072 6f6a 6563 7420 5374 6174 7573  ![Project Status
+000002e0: 3a20 4163 7469 7665 20e2 8093 2054 6865  : Active ... The
+000002f0: 2070 726f 6a65 6374 2068 6173 2072 6561   project has rea
+00000300: 6368 6564 2061 2073 7461 626c 652c 2075  ched a stable, u
+00000310: 7361 626c 6520 7374 6174 6520 616e 6420  sable state and 
+00000320: 6973 2062 6569 6e67 2061 6374 6976 656c  is being activel
+00000330: 7920 6465 7665 6c6f 7065 642e 5d28 6874  y developed.](ht
+00000340: 7470 733a 2f2f 7777 772e 7265 706f 7374  tps://www.repost
+00000350: 6174 7573 2e6f 7267 2f62 6164 6765 732f  atus.org/badges/
+00000360: 6c61 7465 7374 2f61 6374 6976 652e 7376  latest/active.sv
+00000370: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
+00000380: 7265 706f 7374 6174 7573 2e6f 7267 2f23  repostatus.org/#
+00000390: 6163 7469 7665 290a 0a23 2020 5361 5143  active)..#  SaQC
+000003a0: 3a20 5379 7374 656d 2066 6f72 2061 7574  : System for aut
+000003b0: 6f6d 6174 6564 2051 7561 6c69 7479 2043  omated Quality C
+000003c0: 6f6e 7472 6f6c 0a0a 416e 6f6d 616c 6965  ontrol..Anomalie
+000003d0: 7320 616e 6420 6572 726f 7273 2061 7265  s and errors are
+000003e0: 2074 6865 2072 756c 6520 6e6f 7420 7468   the rule not th
+000003f0: 6520 6578 6365 7074 696f 6e20 7768 656e  e exception when
+00000400: 2077 6f72 6b69 6e67 2077 6974 6820 0a74   working with .t
+00000410: 696d 6520 7365 7269 6573 2064 6174 612e  ime series data.
+00000420: 2054 6869 7320 6973 2065 7370 6563 6961   This is especia
+00000430: 6c6c 7920 7472 7565 2c20 6966 2073 7563  lly true, if suc
+00000440: 6820 6461 7461 206f 7269 6769 6e61 7465  h data originate
+00000450: 730a 6672 6f6d 2069 6e2d 7369 7475 206d  s.from in-situ m
+00000460: 6561 7375 7265 6d65 6e74 7320 6f66 2065  easurements of e
+00000470: 6e76 6972 6f6e 6d65 6e74 616c 2070 726f  nvironmental pro
+00000480: 7065 7274 6965 732e 200a 416c 6d6f 7374  perties. .Almost
+00000490: 2061 6c6c 2061 7070 6c69 6361 7469 6f6e   all application
+000004a0: 732c 2068 6f77 6576 6572 2c20 696d 706c  s, however, impl
+000004b0: 6963 696c 7920 7265 6c79 206f 6e20 6461  icily rely on da
+000004c0: 7461 2c20 7468 6174 2063 6f6d 706c 6965  ta, that complie
+000004d0: 730a 7769 7468 2073 6f6d 6520 6465 6669  s.with some defi
+000004e0: 6e69 7469 6f6e 206f 6620 2763 6f72 7265  nition of 'corre
+000004f0: 6374 272e 200a 496e 206f 7264 6572 2074  ct'. .In order t
+00000500: 6f20 696e 6665 7220 7265 6c69 6162 6c65  o infer reliable
+00000510: 2064 6174 6120 7072 6f64 7563 7473 2061   data products a
+00000520: 6e64 2074 6f6f 6c73 2c20 7468 6572 6520  nd tools, there 
+00000530: 6973 206e 6f20 616c 7465 726e 6174 6976  is no alternativ
+00000540: 650a 746f 2071 7561 6c69 7479 2063 6f6e  e.to quality con
+00000550: 7472 6f6c 2e20 5361 5143 2070 726f 7669  trol. SaQC provi
+00000560: 6465 7320 616c 6c20 7468 6520 6275 696c  des all the buil
+00000570: 6469 6e67 2062 6c6f 636b 7320 746f 2063  ding blocks to c
+00000580: 6f6d 666f 7274 6162 6c79 0a62 7269 6467  omfortably.bridg
+00000590: 6520 7468 6520 6761 7020 6265 7477 6565  e the gap betwee
+000005a0: 6e20 2775 7375 616c 6c79 2066 6175 6c74  n 'usually fault
+000005b0: 7927 2061 6e64 2027 6578 7065 6374 6564  y' and 'expected
+000005c0: 2074 6f20 6265 2063 6f72 7265 6374 6564   to be corrected
+000005d0: 2720 696e 200a 6120 6163 6365 7373 6962  ' in .a accessib
+000005e0: 6c65 2c20 636f 6e73 6973 7465 6e74 2c20  le, consistent, 
+000005f0: 6f62 6a65 6374 6976 6520 616e 6420 7265  objective and re
+00000600: 7072 6f64 7563 6962 6c65 2077 6179 2e0a  producible way..
+00000610: 0a46 6f72 2061 2028 636f 6e74 696e 6f75  .For a (continou
+00000620: 736c 7920 696d 7072 6f76 696e 6729 206f  sly improving) o
+00000630: 7665 7276 6965 7720 6f66 2066 6561 7475  verview of featu
+00000640: 7265 732c 2074 7970 6963 616c 2075 7361  res, typical usa
+00000650: 6765 2070 6174 7465 726e 732c 0a74 6865  ge patterns,.the
+00000660: 2073 7065 6369 6669 6320 7379 7374 656d   specific system
+00000670: 2063 6f6d 706f 6e65 6e74 7320 616e 6420   components and 
+00000680: 686f 7720 746f 2063 7573 746f 6d69 7a65  how to customize
+00000690: 2060 5361 5143 6020 746f 2079 6f75 7220   `SaQC` to your 
+000006a0: 7370 6563 6966 6963 0a6e 6565 6473 2c20  specific.needs, 
+000006b0: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
+000006c0: 6f75 720a 5b6f 6e6c 696e 6520 646f 6375  our.[online docu
+000006d0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+000006e0: 3a2f 2f72 646d 2d73 6f66 7477 6172 652e  ://rdm-software.
+000006f0: 7061 6765 732e 7566 7a2e 6465 2f73 6171  pages.ufz.de/saq
+00000700: 632f 696e 6465 782e 6874 6d6c 292e 0a0a  c/index.html)...
+00000710: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000720: 0a0a 5361 5143 2069 7320 6176 6169 6c61  ..SaQC is availa
+00000730: 626c 6520 6f6e 2074 6865 2050 7974 686f  ble on the Pytho
+00000740: 6e20 5061 636b 6167 6520 496e 6465 7820  n Package Index 
+00000750: 285b 5079 5049 5d28 6874 7470 733a 2f2f  ([PyPI](https://
+00000760: 7079 7069 2e6f 7267 2f29 2920 616e 640a  pypi.org/)) and.
+00000770: 6361 6e20 6265 2069 6e73 7461 6c6c 6564  can be installed
+00000780: 2075 7369 6e67 205b 7069 705d 2868 7474   using [pip](htt
+00000790: 7073 3a2f 2f70 6970 2e70 7970 612e 696f  ps://pip.pypa.io
+000007a0: 2f65 6e2f 7374 6162 6c65 2f29 3a0a 6060  /en/stable/):.``
+000007b0: 6073 680a 7079 7468 6f6e 202d 6d20 7069  `sh.python -m pi
+000007c0: 7020 696e 7374 616c 6c20 7361 7163 0a60  p install saqc.`
+000007d0: 6060 0a46 6f72 2061 206d 6f72 6520 6465  ``.For a more de
+000007e0: 7461 696c 6564 2069 6e73 7461 6c6c 696f  tailed installio
+000007f0: 6e20 6775 6964 652c 2073 6565 2074 6865  n guide, see the
+00000800: 205b 696e 7374 616c 6c61 7469 6f6e 2067   [installation g
+00000810: 7569 6465 5d28 6874 7470 733a 2f2f 7264  uide](https://rd
+00000820: 6d2d 736f 6674 7761 7265 2e70 6167 6573  m-software.pages
+00000830: 2e75 667a 2e64 652f 7361 7163 2f67 6574  .ufz.de/saqc/get
+00000840: 7469 6e67 7374 6172 7465 642f 496e 7374  tingstarted/Inst
+00000850: 616c 6c61 7469 6f6e 4775 6964 652e 6874  allationGuide.ht
+00000860: 6d6c 292e 0a0a 2323 2055 7361 6765 0a0a  ml)...## Usage..
+00000870: 6053 6151 4360 2069 7320 626f 7468 2c20  `SaQC` is both, 
+00000880: 6120 636f 6d6d 616e 6420 6c69 6e65 2061  a command line a
+00000890: 7070 6c69 6361 7469 6f6e 2063 6f6e 7472  pplication contr
+000008a0: 6f6c 6c65 6420 6279 2061 2074 6578 7420  olled by a text 
+000008b0: 6261 7365 6420 636f 6e66 6967 7572 6174  based configurat
+000008c0: 696f 6e0a 616e 6420 6120 7079 7468 6f6e  ion.and a python
+000008d0: 206d 6f64 756c 6520 7769 7468 2061 2073   module with a s
+000008e0: 696d 706c 6520 4150 492e 0a0a 2323 2320  imple API...### 
+000008f0: 5361 5143 2061 7320 6120 636f 6d6d 616e  SaQC as a comman
+00000900: 6420 6c69 6e65 2061 7070 6c69 6361 7469  d line applicati
+00000910: 6f6e 0a54 6865 2063 6f6d 6d61 6e64 206c  on.The command l
+00000920: 696e 6520 6170 706c 6963 6174 696f 6e20  ine application 
+00000930: 6973 2063 6f6e 7472 6f6c 6c65 6420 6279  is controlled by
+00000940: 2061 2073 656d 6963 6f6c 6f6e 2d73 6570   a semicolon-sep
+00000950: 6172 6174 6564 2074 6578 740a 6669 6c65  arated text.file
+00000960: 206c 6973 7469 6e67 2074 6865 2076 6172   listing the var
+00000970: 6961 626c 6573 2069 6e20 7468 6520 6461  iables in the da
+00000980: 7461 7365 7420 616e 6420 7468 6520 726f  taset and the ro
+00000990: 7574 696e 6573 2074 6f20 696e 7370 6563  utines to inspec
+000009a0: 742c 0a71 7561 6c69 7479 2063 6f6e 7472  t,.quality contr
+000009b0: 6f6c 2061 6e64 2f6f 7220 7072 6f63 6573  ol and/or proces
+000009c0: 7320 7468 656d 2e20 5468 6520 636f 6e74  s them. The cont
+000009d0: 656e 7420 6f66 2073 7563 6820 6120 636f  ent of such a co
+000009e0: 6e66 6967 7572 6174 696f 6e0a 636f 756c  nfiguration.coul
+000009f0: 6420 6c6f 6f6b 206c 696b 6520 5b74 6869  d look like [thi
+00000a00: 735d 2868 7474 7073 3a2f 2f67 6974 2e75  s](https://git.u
+00000a10: 667a 2e64 652f 7264 6d2d 736f 6674 7761  fz.de/rdm-softwa
+00000a20: 7265 2f73 6171 632f 7261 772f 6465 7665  re/saqc/raw/deve
+00000a30: 6c6f 702f 646f 6373 2f72 6573 6f75 7263  lop/docs/resourc
+00000a40: 6573 2f64 6174 612f 636f 6e66 6967 2e63  es/data/config.c
+00000a50: 7376 293a 0a0a 6060 600a 7661 726e 616d  sv):..```.varnam
+00000a60: 6520 2020 203b 2074 6573 740a 232d 2d2d  e    ; test.#---
+00000a70: 2d2d 2d2d 2d2d 2d3b 202d 2d2d 2d2d 2d2d  -------; -------
+00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a53  --------------.S
+00000ac0: 4d32 2020 2020 2020 2020 3b20 7368 6966  M2        ; shif
+00000ad0: 7428 6672 6571 3d22 3135 4d69 6e22 290a  t(freq="15Min").
+00000ae0: 2753 4d28 317c 3229 2b27 203b 2066 6c61  'SM(1|2)+' ; fla
+00000af0: 674d 6973 7369 6e67 2829 0a53 4d31 2020  gMissing().SM1  
+00000b00: 2020 2020 2020 3b20 666c 6167 5261 6e67        ; flagRang
+00000b10: 6528 6d69 6e3d 3130 2c20 6d61 783d 3630  e(min=10, max=60
+00000b20: 290a 534d 3220 2020 2020 2020 203b 2066  ).SM2        ; f
+00000b30: 6c61 6752 616e 6765 286d 696e 3d31 302c  lagRange(min=10,
+00000b40: 206d 6178 3d34 3029 0a53 4d32 2020 2020   max=40).SM2    
+00000b50: 2020 2020 3b20 666c 6167 4d41 4428 7769      ; flagMAD(wi
+00000b60: 6e64 6f77 3d22 3330 6422 2c20 7a3d 332e  ndow="30d", z=3.
+00000b70: 3529 0a44 756d 6d79 2020 2020 2020 3b20  5).Dummy      ; 
+00000b80: 666c 6167 4765 6e65 7269 6328 6669 656c  flagGeneric(fiel
+00000b90: 643d 5b22 534d 3122 2c20 2253 4d32 225d  d=["SM1", "SM2"]
+00000ba0: 2c20 6675 6e63 3d28 6973 666c 6167 6765  , func=(isflagge
+00000bb0: 6428 7829 207c 2069 7366 6c61 6767 6564  d(x) | isflagged
+00000bc0: 2879 2929 290a 6060 600a 0a41 7320 736f  (y))).```..As so
+00000bd0: 6f6e 2061 7320 7468 6520 6261 7369 6320  on as the basic 
+00000be0: 696e 7075 7473 2c20 6461 7461 7365 7420  inputs, dataset 
+00000bf0: 616e 6420 636f 6e66 6967 7572 6174 696f  and configuratio
+00000c00: 6e20 6669 6c65 2c20 6172 650a 7072 6570  n file, are.prep
+00000c10: 6172 6564 2c20 7275 6e20 6053 6151 4360  ared, run `SaQC`
+00000c20: 3a0a 6060 6073 680a 7361 7163 205c 0a20  :.```sh.saqc \. 
+00000c30: 2020 202d 2d63 6f6e 6669 6720 5041 5448     --config PATH
+00000c40: 5f54 4f5f 434f 4e46 4947 5552 4154 494f  _TO_CONFIGURATIO
+00000c50: 4e20 5c0a 2020 2020 2d2d 6461 7461 2050  N \.    --data P
+00000c60: 4154 485f 544f 5f44 4154 4120 5c0a 2020  ATH_TO_DATA \.  
+00000c70: 2020 2d2d 6f75 7466 696c 6520 5041 5448    --outfile PATH
+00000c80: 5f54 4f5f 4f55 5450 5554 0a60 6060 0a0a  _TO_OUTPUT.```..
+00000c90: 4120 6675 6c6c 2060 5361 5143 6020 7275  A full `SaQC` ru
+00000ca0: 6e20 6167 6169 6e73 7420 7072 6f76 6964  n against provid
+00000cb0: 6564 2065 7861 6d70 6c65 2064 6174 6120  ed example data 
+00000cc0: 6361 6e20 6265 2069 6e76 6f6b 6564 2077  can be invoked w
+00000cd0: 6974 683a 0a60 6060 7368 0a73 6171 6320  ith:.```sh.saqc 
+00000ce0: 5c0a 2020 2020 2d2d 636f 6e66 6967 2068  \.    --config h
+00000cf0: 7474 7073 3a2f 2f67 6974 2e75 667a 2e64  ttps://git.ufz.d
+00000d00: 652f 7264 6d2d 736f 6674 7761 7265 2f73  e/rdm-software/s
+00000d10: 6171 632f 7261 772f 6465 7665 6c6f 702f  aqc/raw/develop/
+00000d20: 646f 6373 2f72 6573 6f75 7263 6573 2f64  docs/resources/d
+00000d30: 6174 612f 636f 6e66 6967 2e63 7376 205c  ata/config.csv \
+00000d40: 0a20 2020 202d 2d64 6174 6120 6874 7470  .    --data http
+00000d50: 733a 2f2f 6769 742e 7566 7a2e 6465 2f72  s://git.ufz.de/r
+00000d60: 646d 2d73 6f66 7477 6172 652f 7361 7163  dm-software/saqc
+00000d70: 2f72 6177 2f64 6576 656c 6f70 2f64 6f63  /raw/develop/doc
+00000d80: 732f 7265 736f 7572 6365 732f 6461 7461  s/resources/data
+00000d90: 2f64 6174 612e 6373 7620 5c0a 2020 2020  /data.csv \.    
+00000da0: 2d2d 6f75 7466 696c 6520 7361 7163 5f74  --outfile saqc_t
+00000db0: 6573 742e 6373 760a 6060 600a 0a23 2323  est.csv.```..###
+00000dc0: 2053 6151 4320 6173 2061 2070 7974 686f   SaQC as a pytho
+00000dd0: 6e20 6d6f 6475 6c65 0a0a 5468 6520 666f  n module..The fo
+00000de0: 6c6c 6f77 696e 6720 736e 6970 7065 7420  llowing snippet 
+00000df0: 696d 706c 656d 656e 7473 2074 6865 2073  implements the s
+00000e00: 616d 6520 636f 6e66 6967 7572 6174 696f  ame configuratio
+00000e10: 6e20 6769 7665 6e20 6162 6f76 6520 7468  n given above th
+00000e20: 726f 7567 680a 7468 6520 5079 7468 6f6e  rough.the Python
+00000e30: 2d41 5049 3a0a 0a60 6060 7079 7468 6f6e  -API:..```python
+00000e40: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
+00000e50: 7320 7064 0a66 726f 6d20 7361 7163 2069  s pd.from saqc i
+00000e60: 6d70 6f72 7420 5361 5143 0a0a 6461 7461  mport SaQC..data
+00000e70: 203d 2070 642e 7265 6164 5f63 7376 280a   = pd.read_csv(.
+00000e80: 2020 2020 2268 7474 7073 3a2f 2f67 6974      "https://git
+00000e90: 2e75 667a 2e64 652f 7264 6d2d 736f 6674  .ufz.de/rdm-soft
+00000ea0: 7761 7265 2f73 6171 632f 7261 772f 6465  ware/saqc/raw/de
+00000eb0: 7665 6c6f 702f 646f 6373 2f72 6573 6f75  velop/docs/resou
+00000ec0: 7263 6573 2f64 6174 612f 6461 7461 2e63  rces/data/data.c
+00000ed0: 7376 222c 0a20 2020 2069 6e64 6578 5f63  sv",.    index_c
+00000ee0: 6f6c 3d30 2c20 7061 7273 655f 6461 7465  ol=0, parse_date
+00000ef0: 733d 5472 7565 2c0a 290a 0a73 6171 6320  s=True,.)..saqc 
+00000f00: 3d20 5361 5143 2864 6174 613d 6461 7461  = SaQC(data=data
+00000f10: 290a 7361 7163 203d 2028 7361 7163 0a20  ).saqc = (saqc. 
+00000f20: 2020 2020 2020 202e 7368 6966 7428 2253         .shift("S
+00000f30: 4d32 222c 2066 7265 713d 2231 354d 696e  M2", freq="15Min
+00000f40: 2229 0a20 2020 2020 2020 202e 666c 6167  ").        .flag
+00000f50: 4d69 7373 696e 6728 2253 4d28 317c 3229  Missing("SM(1|2)
+00000f60: 2b22 2c20 7265 6765 783d 5472 7565 290a  +", regex=True).
+00000f70: 2020 2020 2020 2020 2e66 6c61 6752 616e          .flagRan
+00000f80: 6765 2822 534d 3122 2c20 6d69 6e3d 3130  ge("SM1", min=10
+00000f90: 2c20 6d61 783d 3630 290a 2020 2020 2020  , max=60).      
+00000fa0: 2020 2e66 6c61 6752 616e 6765 2822 534d    .flagRange("SM
+00000fb0: 3222 2c20 6d69 6e3d 3130 2c20 6d61 783d  2", min=10, max=
+00000fc0: 3430 290a 2020 2020 2020 2020 2e66 6c61  40).        .fla
+00000fd0: 674d 4144 2822 534d 3222 2c20 7769 6e64  gMAD("SM2", wind
+00000fe0: 6f77 3d22 3330 6422 2c20 7a3d 332e 3529  ow="30d", z=3.5)
+00000ff0: 0a20 2020 2020 2020 202e 666c 6167 4765  .        .flagGe
+00001000: 6e65 7269 6328 6669 656c 643d 5b22 534d  neric(field=["SM
+00001010: 3122 2c20 2253 4d32 225d 2c20 7461 7267  1", "SM2"], targ
+00001020: 6574 3d22 4475 6d6d 7922 2c20 6675 6e63  et="Dummy", func
+00001030: 3d6c 616d 6264 6120 782c 2079 3a20 2869  =lambda x, y: (i
+00001040: 7366 6c61 6767 6564 2878 2920 7c20 6973  sflagged(x) | is
+00001050: 666c 6167 6765 6428 7929 2929 290a 6060  flagged(y)))).``
+00001060: 600a 0a41 206d 6f72 6520 6465 7461 696c  `..A more detail
+00001070: 6564 2064 6573 6372 6970 7469 6f6e 206f  ed description o
+00001080: 6620 7468 6520 5079 7468 6f6e 2041 5049  f the Python API
+00001090: 2069 7320 6176 6169 6c61 626c 6520 696e   is available in
+000010a0: 2074 6865 200a 5b72 6573 7065 6374 6976   the .[respectiv
+000010b0: 6520 7365 6374 696f 6e5d 2868 7474 7073  e section](https
+000010c0: 3a2f 2f72 646d 2d73 6f66 7477 6172 652e  ://rdm-software.
+000010d0: 7061 6765 732e 7566 7a2e 6465 2f73 6171  pages.ufz.de/saq
+000010e0: 632f 6765 7474 696e 6773 7461 7274 6564  c/gettingstarted
+000010f0: 2f54 7574 6f72 6961 6c41 5049 2e68 746d  /TutorialAPI.htm
+00001100: 6c29 0a6f 6620 7468 6520 646f 6375 6d65  l).of the docume
+00001110: 6e74 6174 696f 6e2e 0a0a 2323 2043 6861  ntation...## Cha
+00001120: 6e67 656c 6f67 0a41 6c6c 206e 6f74 6162  ngelog.All notab
+00001130: 6c65 2063 6861 6e67 6573 2074 6f20 7468  le changes to th
+00001140: 6973 2070 726f 6a65 6374 2077 696c 6c20  is project will 
+00001150: 6265 2064 6f63 756d 656e 7465 6420 696e  be documented in
+00001160: 205b 4348 414e 4745 4c4f 472e 6d64 5d28   [CHANGELOG.md](
+00001170: 4348 414e 4745 4c4f 472e 6d64 292e 0a0a  CHANGELOG.md)...
+00001180: 2323 2047 6574 2069 6e76 6f6c 7665 640a  ## Get involved.
+00001190: 0a23 2323 2043 6f6e 7472 6962 7574 696e  .### Contributin
+000011a0: 670a 596f 7520 666f 756e 6420 6120 6275  g.You found a bu
+000011b0: 6720 6f72 2079 6f75 2077 616e 7420 746f  g or you want to
+000011c0: 2073 7567 6765 7374 2073 6f6d 6520 636f   suggest some co
+000011d0: 6f6c 2066 6561 7475 7265 733f 2050 6c65  ol features? Ple
+000011e0: 6173 6520 7265 6665 7220 746f 206f 7572  ase refer to our
+000011f0: 205b 636f 6e74 7269 6275 7469 6e67 2067   [contributing g
+00001200: 7569 6465 6c69 6e65 735d 2843 4f4e 5452  uidelines](CONTR
+00001210: 4942 5554 494e 472e 6d64 2920 746f 2073  IBUTING.md) to s
+00001220: 6565 2068 6f77 2079 6f75 2063 616e 2063  ee how you can c
+00001230: 6f6e 7472 6962 7574 6520 746f 2053 6151  ontribute to SaQ
+00001240: 432e 0a0a 2323 2320 5573 6572 2073 7570  C...### User sup
+00001250: 706f 7274 0a49 6620 796f 7520 6e65 6564  port.If you need
+00001260: 2068 656c 7020 6f72 2068 6176 6520 6120   help or have a 
+00001270: 7175 6573 7469 6f6e 2c20 796f 7520 6361  question, you ca
+00001280: 6e20 7573 6520 7468 6520 5361 5143 2075  n use the SaQC u
+00001290: 7365 7220 7375 7070 6f72 7420 6d61 696c  ser support mail
+000012a0: 696e 6720 6c69 7374 3a20 5b73 6171 632d  ing list: [saqc-
+000012b0: 7375 7070 6f72 7440 7566 7a2e 6465 5d28  support@ufz.de](
+000012c0: 6d61 696c 746f 3a73 6171 632d 7375 7070  mailto:saqc-supp
+000012d0: 6f72 7440 7566 7a2e 6465 290a 0a23 2320  ort@ufz.de)..## 
+000012e0: 436f 7079 7269 6768 7420 616e 6420 4c69  Copyright and Li
+000012f0: 6365 6e73 650a 436f 7079 7269 6768 7428  cense.Copyright(
+00001300: 6329 2032 3032 312c 205b 4865 6c6d 686f  c) 2021, [Helmho
+00001310: 6c74 7a2d 5a65 6e74 7275 6d20 66c3 bc72  ltz-Zentrum f..r
+00001320: 2055 6d77 656c 7466 6f72 7363 6875 6e67   Umweltforschung
+00001330: 2047 6d62 4820 2d2d 2055 465a 5d28 6874   GmbH -- UFZ](ht
+00001340: 7470 733a 2f2f 7777 772e 7566 7a2e 6465  tps://www.ufz.de
+00001350: 292e 2041 6c6c 2072 6967 6874 7320 7265  ). All rights re
+00001360: 7365 7276 6564 2e0a 0a2d 2044 6f63 756d  served...- Docum
+00001370: 656e 7461 7469 6f6e 3a20 5b43 7265 6174  entation: [Creat
+00001380: 6976 6520 436f 6d6d 6f6e 7320 4174 7472  ive Commons Attr
+00001390: 6962 7574 696f 6e20 342e 3020 496e 7465  ibution 4.0 Inte
+000013a0: 726e 6174 696f 6e61 6c5d 2868 7474 7073  rnational](https
+000013b0: 3a2f 2f63 7265 6174 6976 6563 6f6d 6d6f  ://creativecommo
+000013c0: 6e73 2e6f 7267 2f6c 6963 656e 7365 732f  ns.org/licenses/
+000013d0: 6279 2f34 2e30 2f29 203c 6120 7265 6c3d  by/4.0/) <a rel=
+000013e0: 226c 6963 656e 7365 2220 6872 6566 3d22  "license" href="
+000013f0: 6874 7470 3a2f 2f63 7265 6174 6976 6563  http://creativec
+00001400: 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963 656e  ommons.org/licen
+00001410: 7365 732f 6279 2f34 2e30 2f22 3e3c 696d  ses/by/4.0/"><im
+00001420: 6720 616c 743d 2243 7265 6174 6976 6520  g alt="Creative 
+00001430: 436f 6d6d 6f6e 7320 4c69 6365 6e73 6522  Commons License"
+00001440: 2073 7479 6c65 3d22 626f 7264 6572 2d77   style="border-w
+00001450: 6964 7468 3a30 2220 7372 633d 2268 7474  idth:0" src="htt
+00001460: 7073 3a2f 2f69 2e63 7265 6174 6976 6563  ps://i.creativec
+00001470: 6f6d 6d6f 6e73 2e6f 7267 2f6c 2f62 792f  ommons.org/l/by/
+00001480: 342e 302f 3830 7831 352e 706e 6722 202f  4.0/80x15.png" /
+00001490: 3e3c 2f61 3e0a 2d20 536f 7572 6365 2063  ></a>.- Source c
+000014a0: 6f64 653a 205b 474e 5520 4765 6e65 7261  ode: [GNU Genera
+000014b0: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000014c0: 2033 5d28 6874 7470 733a 2f2f 7777 772e   3](https://www.
+000014d0: 676e 752e 6f72 672f 6c69 6365 6e73 6573  gnu.org/licenses
+000014e0: 2f67 706c 2d33 2e30 2e68 746d 6c29 0a0a  /gpl-3.0.html)..
+000014f0: 466f 7220 6675 6c6c 2064 6574 6169 6c73  For full details
+00001500: 2c20 7365 6520 5b4c 4943 454e 5345 5d28  , see [LICENSE](
+00001510: 4c49 4345 4e53 452e 6d64 292e 0a0a 2323  LICENSE.md)...##
+00001520: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
+00001530: 730a 2e2e 2e0a 0a23 2320 5075 626c 6963  s......## Public
+00001540: 6174 696f 6e73 0a63 6f6d 696e 6720 736f  ations.coming so
+00001550: 6f6e 2e2e 2e0a 0a23 2320 486f 7720 746f  on.....## How to
+00001560: 2063 6974 6520 5361 5143 0a49 6620 5361   cite SaQC.If Sa
+00001570: 5143 2069 7320 6164 7661 6e63 696e 6720  QC is advancing 
+00001580: 796f 7572 2072 6573 6561 7263 682c 2070  your research, p
+00001590: 6c65 6173 6520 6369 7465 2061 733a 0a0a  lease cite as:..
+000015a0: 3e20 5363 68c3 a466 6572 2c20 4461 7669  > Sch..fer, Davi
+000015b0: 642c 2050 616c 6d2c 2042 6572 742c 204c  d, Palm, Bert, L
+000015c0: c3bc 6e65 6e73 6368 6c6f c39f 2c20 5065  ..nenschlo.., Pe
+000015d0: 7465 722c 2053 6368 6d69 6474 2c20 4c65  ter, Schmidt, Le
+000015e0: 6e6e 6172 742c 2026 2042 756d 6265 7267  nnart, & Bumberg
+000015f0: 6572 2c20 4a61 6e2e 2028 3230 3233 292e  er, Jan. (2023).
+00001600: 2053 7973 7465 6d20 666f 7220 6175 746f   System for auto
+00001610: 6d61 7465 6420 5175 616c 6974 7920 436f  mated Quality Co
+00001620: 6e74 726f 6c20 2d20 5361 5143 2028 322e  ntrol - SaQC (2.
+00001630: 332e 3029 2e20 5a65 6e6f 646f 2e20 6874  3.0). Zenodo. ht
+00001640: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+00001650: 2e35 3238 312f 7a65 6e6f 646f 2e35 3838  .5281/zenodo.588
+00001660: 3835 3437 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d  8547..----------
+00001670: 2d2d 2d2d 2d2d 2d0a 0a3c 6120 6872 6566  -------..<a href
+00001680: 3d22 6874 7470 733a 2f2f 7777 772e 7566  ="https://www.uf
+00001690: 7a2e 6465 2f69 6e64 6578 2e70 6870 3f65  z.de/index.php?e
+000016a0: 6e3d 3333 3537 3322 3e0a 2020 2020 3c69  n=33573">.    <i
+000016b0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000016c0: 6769 742e 7566 7a2e 6465 2f72 646d 2d73  git.ufz.de/rdm-s
+000016d0: 6f66 7477 6172 652f 7361 7163 2f72 6177  oftware/saqc/raw
+000016e0: 2f64 6576 656c 6f70 2f64 6f63 732f 7265  /develop/docs/re
+000016f0: 736f 7572 6365 732f 696d 6167 6573 2f72  sources/images/r
+00001700: 6570 7265 7365 6e74 6174 6976 652f 5546  epresentative/UF
+00001710: 5a4c 6f67 6f2e 706e 6722 2077 6964 7468  ZLogo.png" width
+00001720: 3d22 3430 3022 2f3e 0a3c 2f61 3e0a 0a3c  ="400"/>.</a>..<
+00001730: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001740: 7777 772e 7566 7a2e 6465 2f69 6e64 6578  www.ufz.de/index
+00001750: 2e70 6870 3f65 6e3d 3435 3334 3822 3e0a  .php?en=45348">.
+00001760: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00001770: 7470 733a 2f2f 6769 742e 7566 7a2e 6465  tps://git.ufz.de
+00001780: 2f72 646d 2d73 6f66 7477 6172 652f 7361  /rdm-software/sa
+00001790: 7163 2f72 6177 2f64 6576 656c 6f70 2f64  qc/raw/develop/d
+000017a0: 6f63 732f 7265 736f 7572 6365 732f 696d  ocs/resources/im
+000017b0: 6167 6573 2f72 6570 7265 7365 6e74 6174  ages/representat
+000017c0: 6976 652f 5244 4d4c 6f67 6f2e 706e 6722  ive/RDMLogo.png"
+000017d0: 2061 6c69 676e 3d22 7269 6768 7422 2077   align="right" w
+000017e0: 6964 7468 3d22 3232 3022 2f3e 0a3c 2f61  idth="220"/>.</a
+000017f0: 3e0a                                     >.
```

### Comparing `saqc-2.3/saqc.egg-info/SOURCES.txt` & `saqc-2.4.0/saqc.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,33 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
 LICENSES/GPL-3.0-or-later.txt
-dios/__init__.py
-dios/setup.py
-dios/dios/__init__.py
-dios/dios/base.py
-dios/dios/dios.py
-dios/dios/indexer.py
-dios/dios/lib.py
-dios/dios/operators.py
-dios/dios/pandas_bridge.py
-dios/profiling/__init__.py
-dios/profiling/generate_testsets.py
-dios/profiling/memory.py
-dios/profiling/performance.py
-dios/test/__init__.py
-dios/test/run_dios.py
-dios/test/test__ops__.py
-dios/test/test__setget__.py
-dios/test/test__setget__aloc.py
-dios/test/test__setget__iloc.py
-dios/test/test__setget__loc.py
-dios/test/test__setitem__.py
-dios/test/test_dflike.py
-dios/test/test_dflike__setget__.py
-dios/test/test_magic_methods.py
-dios/test/test_methods.py
-dios/test/test_setup.py
 saqc/__init__.py
 saqc/__main__.py
 saqc/constants.py
 saqc/version.py
 saqc.egg-info/PKG-INFO
 saqc.egg-info/SOURCES.txt
 saqc.egg-info/dependency_links.txt
 saqc.egg-info/entry_points.txt
 saqc.egg-info/requires.txt
 saqc.egg-info/top_level.txt
 saqc/core/__init__.py
 saqc/core/core.py
 saqc/core/flags.py
+saqc/core/frame.py
 saqc/core/history.py
-saqc/core/mixins.py
-saqc/core/reader.py
 saqc/core/register.py
-saqc/core/visitor.py
 saqc/core/translation/__init__.py
 saqc/core/translation/basescheme.py
 saqc/core/translation/dmpscheme.py
-saqc/core/translation/floatscheme.py
 saqc/core/translation/positionalscheme.py
+saqc/core/translation/simplescheme.py
 saqc/funcs/__init__.py
 saqc/funcs/breaks.py
 saqc/funcs/changepoints.py
 saqc/funcs/constants.py
 saqc/funcs/curvefit.py
 saqc/funcs/drift.py
 saqc/funcs/flagtools.py
@@ -67,43 +39,47 @@
 saqc/funcs/resampling.py
 saqc/funcs/residuals.py
 saqc/funcs/rolling.py
 saqc/funcs/scores.py
 saqc/funcs/tools.py
 saqc/funcs/transformation.py
 saqc/lib/__init__.py
-saqc/lib/docurator.py
+saqc/lib/docs.py
 saqc/lib/plotting.py
 saqc/lib/rolling.py
 saqc/lib/tools.py
 saqc/lib/ts_operators.py
 saqc/lib/types.py
+saqc/parsing/__init__.py
+saqc/parsing/environ.py
+saqc/parsing/reader.py
+saqc/parsing/visitor.py
+tests/test__main__.py
 tests/api/__init__.py
 tests/api/test_creation.py
 tests/cli/__init__.py
 tests/cli/test_integration.py
 tests/core/__init__.py
 tests/core/test_core.py
 tests/core/test_flags.py
+tests/core/test_frame.py
 tests/core/test_history.py
 tests/core/test_reader.py
 tests/core/test_translator.py
 tests/funcs/__init__.py
 tests/funcs/test_constants_detection.py
-tests/funcs/test_curvefit.py
 tests/funcs/test_flagtools.py
 tests/funcs/test_functions.py
 tests/funcs/test_generic_api_functions.py
 tests/funcs/test_generic_config_functions.py
 tests/funcs/test_outlier_detection.py
 tests/funcs/test_pattern_rec.py
 tests/funcs/test_proc_functions.py
 tests/funcs/test_resampling.py
 tests/funcs/test_tools.py
 tests/fuzzy/__init__.py
 tests/fuzzy/lib.py
 tests/fuzzy/test_masking.py
 tests/lib/__init__.py
 tests/lib/test_periodicMask.py
-tests/lib/test_rolling.py
 tests/lib/test_tools.py
 tests/lib/test_ts_operators.py
```

### Comparing `saqc-2.3/setup.py` & `saqc-2.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,20 +28,21 @@
     long_description_content_type="text/markdown",
     url="https://git.ufz.de/rdm-software/saqc",
     packages=find_packages(exclude=("tests", "docs")),
     python_requires=">=3.8",
     install_requires=[
         "Click",
         "dtw",
+        "fancy_collections",
         "matplotlib>=3.4",
         "numba",
-        "numpy<1.24",
+        "numpy",
         "outlier-utils",
         "pyarrow",
-        "pandas>=1.2,<1.5",
+        "pandas",
         "scikit-learn",
         "scipy",
         "typing_extensions",
     ],
     license_files=("LICENSE.md", "LICENSES/GPL-3.0-or-later.txt"),
     entry_points={
         "console_scripts": ["saqc=saqc.__main__:main"],
```

### Comparing `saqc-2.3/tests/api/test_creation.py` & `saqc-2.4.0/tests/api/test_creation.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import numpy as np
 import pandas as pd
 
-import dios
-
 
 def test_init():
-    from saqc import Flags, SaQC
+    from saqc import DictOfSeries, Flags, SaQC
 
     arr = np.array(
         [
             [0, 1, 2],
             [0, 1, 3],
         ]
     )
     data = pd.DataFrame(arr, columns=list("abc"))
     qc = SaQC(data)
 
     assert isinstance(qc, SaQC)
     assert isinstance(qc._flags, Flags)
-    assert isinstance(qc._data, dios.DictOfSeries)
+    assert isinstance(qc._data, DictOfSeries)
```

### Comparing `saqc-2.3/tests/cli/test_integration.py` & `saqc-2.4.0/tests/cli/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,21 +34,21 @@
     "2016-04-01 00:45:00,nan,nan,nan,nan,29.3679,UNFLAGGED\n",
 ]
 
 POSITIONAL = [
     ",Battery,Battery,SM1,SM1,SM2,SM2\n",
     ",data,flags,data,flags,data,flags\n",
     "Date,,,,,,\n",
-    "2016-04-01 00:00:00,nan,-9999,nan,-9999,29.3157,9000\n",
+    "2016-04-01 00:00:00,nan,-9999,nan,-9999,29.3157,90000\n",
     "2016-04-01 00:05:48,3573.0,9,32.685,90,nan,-9999\n",
-    "2016-04-01 00:15:00,nan,-9999,nan,-9999,29.3157,9000\n",
+    "2016-04-01 00:15:00,nan,-9999,nan,-9999,29.3157,90000\n",
     "2016-04-01 00:20:42,3572.0,9,32.7428,90,nan,-9999\n",
-    "2016-04-01 00:30:00,nan,-9999,nan,-9999,29.3679,9002\n",
+    "2016-04-01 00:30:00,nan,-9999,nan,-9999,29.3679,90002\n",
     "2016-04-01 00:35:37,3572.0,9,32.6186,90,nan,-9999\n",
-    "2016-04-01 00:45:00,nan,-9999,nan,-9999,29.3679,9000\n",
+    "2016-04-01 00:45:00,nan,-9999,nan,-9999,29.3679,90000\n",
 ]
 
 DMP = [
     ",Battery,Battery,Battery,Battery,SM1,SM1,SM1,SM1,SM2,SM2,SM2,SM2\n",
     ",data,quality_flag,quality_cause,quality_comment,data,quality_flag,quality_cause,quality_comment,data,quality_flag,quality_cause,quality_comment\n",
     "Date,,,,,,,,,,,,\n",
     "2016-04-01 00:00:00,nan,nan,nan,nan,nan,nan,nan,nan,29.3157,NIL,,\n",
```

### Comparing `saqc-2.3/tests/core/test_core.py` & `saqc-2.4.0/tests/core/test_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,34 +8,32 @@
 
 import copy
 
 import numpy as np
 import pandas as pd
 import pytest
 
-import saqc
-from saqc.constants import BAD, FILTER_ALL, FILTER_NONE, UNFLAGGED
-from saqc.core import SaQC, initFlagsLike
-from saqc.core.flags import Flags
-from saqc.core.register import flagging, processing, register
+from saqc import BAD, FILTER_ALL, FILTER_NONE, UNFLAGGED, SaQC
+from saqc.core import DictOfSeries, Flags, flagging, initFlagsLike, processing, register
 from saqc.lib.types import OptionalNone
 from tests.common import initData
 
 OPTIONAL = [False, True]
 
 
 @pytest.fixture
 def data():
     return initData(3)
 
 
 @pytest.fixture
 def flags(data, optional):
-    if not optional:
-        return initFlagsLike(data[data.columns[::2]]).toDios()
+    if optional:
+        return None
+    return DictOfSeries(initFlagsLike(data[data.columns[::2]]))
 
 
 def test_errorHandling(data):
     @processing()
     def raisingFunc(saqc, field, **kwargs):
         raise TypeError
 
@@ -54,56 +52,61 @@
 
     @register(mask=["field"], demask=["field"], squeeze=["field"])
     def flagAll(saqc, field, **kwargs):
         saqc._flags[:, field] = BAD
         return saqc
 
     flags = initFlagsLike(data)
-    flags_raw = flags.toDios()
+    flags_raw = DictOfSeries(flags)
     var1, var2 = data.columns[:2]
 
     pflags = SaQC(data, flags=flags_raw).flagAll(var1).flagAll(var2).flags
 
     for c in pflags.columns:
         assert pflags[c].dtype == flags[c].dtype
 
 
 def test_new_call(data):
-    qc = saqc.SaQC(data)
+    qc = SaQC(data)
     qc = qc.flagRange("var1", max=5)
 
 
-def test_copy(data):
-    qc = saqc.SaQC(data)
+def test_SaQC_attributes():
+    """Test if all instance attributes are in SaQC._attributes"""
+    qc = SaQC()
+    for name in [n for n in dir(qc) if not n.startswith("__")]:
+        if hasattr(SaQC, name):  # skip class attributes
+            continue
+        assert name in SaQC._attributes
 
+
+def test_copy(data):
+    qc = SaQC(data)
     qc = qc.flagRange("var1").flagRange("var1", min=0, max=0)
 
     deep = qc.copy(deep=True)
     shallow = qc.copy(deep=False)
-
     for copy in [deep, shallow]:
         assert copy is not qc
-        assert copy._scheme is not qc._scheme
-        assert copy._attrs is not qc._attrs
-
-        assert copy._data is not qc._data
-        assert copy._flags is not qc._flags
+        for name in [n for n in dir(qc) if not n.startswith("__")]:
+            if hasattr(SaQC, name):  # skip class attributes
+                continue
+            qc_attr = getattr(qc, name)
+            other_attr = getattr(copy, name)
+            assert qc_attr is not other_attr
+
+    # History is always copied
+    assert deep._flags._data["var1"] is not qc._flags._data["var1"]
+    assert shallow._flags._data["var1"] is not qc._flags._data["var1"]
 
-        assert copy._data._data is not qc._data._data
-        assert copy._flags._data is not qc._flags._data
+    # underling data NOT copied
+    assert shallow._data["var1"] is qc._data["var1"]
 
     # underling data copied
-    assert deep._data._data.iloc[0] is not qc._data._data.iloc[0]
-    assert (
-        deep._flags._data["var1"].hist.index is not qc._flags._data["var1"].hist.index
-    )
-
-    # underling data NOT copied
-    assert shallow._data._data.iloc[0] is qc._data._data.iloc[0]
-    assert shallow._flags._data["var1"].hist.index is qc._flags._data["var1"].hist.index
+    assert deep._data["var1"] is not qc._data["var1"]
 
 
 def test_sourceTargetCopy():
     """
     test implicit copies
     """
     data = initData(1)
@@ -363,7 +366,52 @@
     def flagFoo(saqc, field, dfilter, **kwargs):
         assert dfilter == internal_flag
         return saqc
 
     field = data.columns[0]
     qc = SaQC(data, scheme="simple")
     qc.flagFoo(field, dfilter=user_flag)
+
+
+@pytest.mark.parametrize(
+    "data, expected",
+    [
+        # 2c + 1c -> 3c
+        (
+            [
+                DictOfSeries(a=pd.Series([1]), b=pd.Series([2])),
+                DictOfSeries(c=pd.Series([3])),
+            ],
+            DictOfSeries(a=pd.Series([1]), b=pd.Series([2]), c=pd.Series([3])),
+        ),
+        # 1c + 1c + 1c -> 3c
+        (
+            [
+                DictOfSeries(a=pd.Series([1])),
+                DictOfSeries(b=pd.Series([2])),
+                DictOfSeries(c=pd.Series([3])),
+            ],
+            DictOfSeries(a=pd.Series([1]), b=pd.Series([2]), c=pd.Series([3])),
+        ),
+    ],
+)
+def test_concatDios(data, expected):
+    result = SaQC(data)
+    assert result.data == expected
+
+
+@pytest.mark.parametrize(
+    "data,expected",
+    [
+        (
+            [
+                DictOfSeries(a=pd.Series([1]), b=pd.Series([2])),
+                DictOfSeries(b=pd.Series([99])),
+            ],
+            DictOfSeries(a=pd.Series([1]), b=pd.Series([99])),
+        )
+    ],
+)
+def test_concatDios_warning(data, expected):
+    with pytest.warns(UserWarning):
+        result = SaQC(data)
+    assert result.data == expected
```

### Comparing `saqc-2.3/tests/core/test_flags.py` & `saqc-2.4.0/tests/core/test_flags.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 
 from typing import Dict, Union
 
 import numpy as np
 import pandas as pd
 import pytest
 
-import dios
-from saqc.constants import UNFLAGGED
-from saqc.core.flags import Flags
-from tests.core.test_history import History
-from tests.core.test_history import is_equal as hist_equal
+import tests.core.test_history as test_hist
+from saqc import UNFLAGGED
+from saqc.core import DictOfSeries, Flags, History
 
 _arrays = [
     np.array([[]]),
     np.zeros((1, 1)),
     np.zeros((3, 4)),
     np.ones((3, 4)),
     np.ones((3, 4)) * np.nan,
@@ -38,26 +36,27 @@
     ),
 ]
 
 testdata = []
 for d in _arrays:
     columns = list("abcdefgh")[: d.shape[1]]
     df = pd.DataFrame(d, dtype=float, columns=columns)
-    dis = dios.DictOfSeries(df)
+    dis = DictOfSeries(df)
     di = {}
     di.update(df.items())
     testdata.append(df)
     testdata.append(di)
     testdata.append(dis)
 
 
 def is_equal(f1, f2):
+    """assert Flags instance equals other"""
     assert f1.columns.equals(f2.columns)
     for c in f1.columns:
-        assert hist_equal(f1.history[c], f2.history[c])
+        assert test_hist.is_equal(f1.history[c], f2.history[c])
 
 
 @pytest.mark.parametrize("data", testdata)
 @pytest.mark.parametrize("copy", [True, False])
 def test_init(data, copy):
     flags = Flags(data, copy=copy)
     assert isinstance(flags, Flags)
@@ -99,15 +98,15 @@
 def test_init_raise_TypeError(data, msg):
     with pytest.raises(TypeError) as e:
         Flags(data)
     assert msg in str(e.value)
 
 
 @pytest.mark.parametrize("data", testdata)
-def test_copy(data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]):
+def test_copy(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
     flags = Flags(data)
     shallow = flags.copy(deep=False)
     deep = flags.copy(deep=True)
 
     # checks
 
     for copy in [deep, shallow]:
@@ -127,17 +126,15 @@
 
     # the underling series data was copied
     for c in deep.columns:
         assert deep._data[c].index is not flags._data[c].index
 
 
 @pytest.mark.parametrize("data", testdata)
-def test_flags_history(
-    data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]
-):
+def test_flags_history(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
     flags = Flags(data)
 
     # get
     for c in flags.columns:
         hist = flags.history[c]
         assert isinstance(hist, History)
         assert len(hist) > 0
@@ -149,15 +146,15 @@
         hist.append(pd.Series(888.0, index=hist.index, dtype=float))
         flags.history[c] = hist
         assert isinstance(hist, History)
         assert len(hist) == hlen + 1
 
 
 @pytest.mark.parametrize("data", testdata)
-def test_get_flags(data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]):
+def test_get_flags(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
     flags = Flags(data)
 
     for c in flags.columns:
         # check obvious
         var = flags[c]
         assert isinstance(var, pd.Series)
         assert not var.empty
@@ -168,15 +165,15 @@
 
         # in particular, a deep copy
         var[:] = 9999.0
         assert all(flags[c] != var)
 
 
 @pytest.mark.parametrize("data", testdata)
-def test_set_flags(data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]):
+def test_set_flags(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
     flags = Flags(data)
 
     for c in flags.columns:
         var = flags[c]
         hlen = len(flags.history[c])
         new = pd.Series(9999.0, index=var.index, dtype=float)
 
@@ -198,15 +195,15 @@
         # check if deep-copied correctly
         new[:] = 7777.0
         assert all(flags.history[c].squeeze() == 8888.0)
 
 
 @pytest.mark.parametrize("data", testdata)
 def test_set_flags_with_mask(
-    data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]
+    data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]
 ):
     flags = Flags(data)
 
     for c in flags.columns:
         var = flags[c]
         mask = var == UNFLAGGED
 
@@ -245,15 +242,15 @@
             wrong_len = vector[:-1]
             with pytest.raises(ValueError):
                 flags[mask, c] = wrong_len
 
 
 @pytest.mark.parametrize("data", testdata)
 def test_set_flags_with_index(
-    data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]
+    data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]
 ):
     flags = Flags(data)
 
     for c in flags.columns:
         var = flags[c]
         mask = var == UNFLAGGED
         index = mask[mask].index
@@ -288,24 +285,24 @@
 
     for c in flags.columns:
         assert df[c].index.equals(flags[c].index)
         assert df[c].equals(flags[c])  # respects nan's
 
 
 @pytest.mark.parametrize("data", testdata)
-def test_to_dios(data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]):
+def test_to_dios(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
     flags = Flags(data)
-    df = flags.toDios()
-
-    assert isinstance(df, dios.DictOfSeries)
-    _validate_flags_equals_frame(flags, df)
+    with pytest.deprecated_call():
+        result = flags.toDios()
+        assert isinstance(result, DictOfSeries)
+        _validate_flags_equals_frame(flags, result)
 
 
 @pytest.mark.parametrize("data", testdata)
-def test_to_frame(data: Union[pd.DataFrame, dios.DictOfSeries, Dict[str, pd.Series]]):
+def test_toFrame(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
     flags = Flags(data)
     df = flags.toFrame()
 
     assert isinstance(df, pd.DataFrame)
     _validate_flags_equals_frame(flags, df)
 
 
@@ -334,7 +331,54 @@
 )
 def test_columns_setter_raises(columns, err):
     flags = Flags(
         {"a": pd.Series([1, 2], dtype=float), "b": pd.Series([1, 2], dtype=float)}
     )
     with pytest.raises(err):
         flags.columns = columns
+
+
+@pytest.mark.parametrize(
+    "data,key,expected",
+    [
+        (dict(a=[0, 1], b=[]), "a", pd.Series([0, 1], dtype=float)),
+        (dict(a=[0, 1], b=[]), "b", pd.Series([], dtype=float)),
+    ],
+)
+def test__getitem__scalar(data, key, expected):
+    flags = Flags({k: pd.Series(v, dtype=float) for k, v in data.items()})
+    result: pd.Series = flags[key]
+    assert isinstance(result, pd.Series)
+    assert result.equals(expected)
+    # assert copying
+    assert flags[key] is not flags[key]
+
+
+@pytest.mark.parametrize(
+    "data,key,expected",
+    [
+        (dict(a=[0, 1], b=[]), [], dict()),
+        (dict(a=[0, 1], b=[]), ["a"], dict(a=[0, 1])),
+        (dict(a=[0, 1], b=[]), ["a", "b"], dict(a=[0, 1], b=[])),
+        (dict(a=[0, 1], b=[]), pd.Index([]), dict()),
+        (dict(a=[0, 1], b=[]), pd.Index(["a"]), dict(a=[0, 1])),
+        (dict(a=[0, 1], b=[]), pd.Index(["a", "b"]), dict(a=[0, 1], b=[])),
+        (dict(a=[0, 1], b=[]), slice(None), dict(a=[0, 1], b=[])),
+        (dict(a=[0, 1], b=[]), slice(0, 1), dict(a=[0, 1])),
+        (dict(a=[0, 1], b=[]), slice(1, 99), dict(b=[])),
+        (dict(a=[0, 1], b=[]), slice(5, 99), dict()),
+    ],
+)
+def test__getitem__listlike_and_slice(data, key, expected):
+    flags = Flags({k: pd.Series(v, dtype=float) for k, v in data.items()})
+    result: Flags = flags[key]
+    assert isinstance(result, Flags)
+    # assert that a new Flags object was created
+    assert flags[key] is not flags[key]
+    # assert that internal data is copied
+    if len(result):
+        left = result._data[result.columns[0]]
+        right = flags._data[result.columns[0]]
+        assert left is not right
+
+    expected = Flags({k: pd.Series(v, dtype=float) for k, v in expected.items()})
+    is_equal(result, expected)
```

### Comparing `saqc-2.3/tests/core/test_history.py` & `saqc-2.4.0/tests/core/test_history.py`

 * *Files identical despite different names*

### Comparing `saqc-2.3/tests/core/test_reader.py` & `saqc-2.4.0/tests/core/test_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,37 +5,36 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pytest
 
-import dios
-from saqc.core.flags import Flags
-from saqc.core.reader import fromConfig, readFile
-from saqc.core.register import flagging
+import saqc.lib.ts_operators as ts_ops
+from saqc.core import DictOfSeries, Flags, SaQC, flagging
+from saqc.parsing.environ import ENVIRONMENT
+from saqc.parsing.reader import fromConfig, readFile
 from tests.common import initData, writeIO
 
 
 @pytest.fixture
-def data() -> dios.DictOfSeries:
+def data() -> DictOfSeries:
     return initData(3)
 
 
 def getTestedVariables(flags: Flags, test: str):
     out = []
     for col in flags.columns:
         for m in flags.history[col].meta:
             if m["func"] == test:
                 out.append(col)
     return out
 
 
 def test_variableRegex(data):
-
     header = f"varname;test"
     function = "flagDummy"
     tests = [
         ("'.*'", data.columns),
         ("'var(1|2)'", [c for c in data.columns if c[-1] in ("1", "2")]),
         ("'var[12]'", [c for c in data.columns if c[-1] in ("1", "2")]),
         ('".*3"', [c for c in data.columns if c[-1] == "3"]),
@@ -88,15 +87,14 @@
     planned = readFile(writeIO(config))
     expected = [4, 5, 6, 10]
     assert (planned.index == expected).all()
 
 
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_configFile(data):
-
     # check that the reader accepts different whitespace patterns
 
     config = f"""
     varname ; test
 
     #temp1      ; flagDummy()
     pre1; flagDummy()
@@ -107,15 +105,14 @@
 
     SM1;flagDummy()
     """
     fromConfig(writeIO(config), data)
 
 
 def test_configChecks(data):
-
     var1, _, var3, *_ = data.columns
 
     @flagging()
     def flagFunc(data, field, flags, arg, opt_arg=None, **kwargs):
         flags[:, field] = np.nan
         return data, flags
 
@@ -130,15 +127,14 @@
     for test, expected in tests:
         fobj = writeIO(header + "\n" + test)
         with pytest.raises(expected):
             fromConfig(fobj, data=data)
 
 
 def test_supportedArguments(data):
-
     # test if the following function arguments
     # are supported (i.e. parsing does not fail)
 
     # TODO: necessary?
 
     @flagging()
     def func(saqc, field, kwarg, **kwargs):
@@ -157,7 +153,25 @@
         f"{var1};func(kwarg=True)",
         f"{var1};func(kwarg=sum([1, 2, 3]))",
     ]
 
     for test in tests:
         fobj = writeIO(header + "\n" + test)
         fromConfig(fobj, data)
+
+
+@pytest.mark.parametrize(
+    "func_string", [k for k, v in ENVIRONMENT.items() if callable(v)]
+)
+def test_funtionArguments(data, func_string):
+    @flagging()
+    def testFunction(saqc, field, func, **kwargs):
+        assert func is ENVIRONMENT[func_string]
+        return saqc
+
+    config = f"""
+    varname ; test
+    {data.columns[0]} ; testFunction(func={func_string})
+    {data.columns[0]} ; testFunction(func="{func_string}")
+    """
+
+    fromConfig(writeIO(config), data)
```

### Comparing `saqc-2.3/tests/core/test_translator.py` & `saqc-2.4.0/tests/core/test_translator.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import json
 from typing import Dict, Sequence, Union
 
 import numpy as np
 import pandas as pd
 import pytest
 
-from saqc.constants import BAD, DOUBTFUL, FILTER_NONE, UNFLAGGED
-from saqc.core.core import SaQC
-from saqc.core.flags import Flags
+from saqc import BAD, DOUBTFUL, FILTER_NONE, UNFLAGGED, SaQC
+from saqc.core import Flags
 from saqc.core.translation import DmpScheme, MappingScheme, PositionalScheme
 from tests.common import initData
 
 
 def _genTranslators():
     for dtype in (str, float, int):
         flags = {
@@ -28,15 +27,14 @@
             **{dtype(f * 10): float(f) for f in range(10)},
         }
         scheme = MappingScheme(flags, {v: k for k, v in flags.items()})
         yield flags, scheme
 
 
 def _genFlags(data: Dict[str, Union[Sequence, pd.Series]]) -> Flags:
-
     flags = Flags()
     for k, v in data.items():
         if not isinstance(v, pd.Series):
             v = pd.Series(
                 v, index=pd.date_range("2012-01-01", freq="1D", periods=len(v))
             )
         flags[k] = v
@@ -72,15 +70,14 @@
         # add an scheme invalid value to the flags
         flags = _genFlags({field: np.array(keys + (max(keys) + 1,))})
         with pytest.raises(ValueError):
             scheme.toExternal(flags)
 
 
 def test_dmpTranslator():
-
     scheme = DmpScheme()
     # generate a bunch of dummy flags
     keys = np.array(tuple(scheme._backward.keys()) * 50)
     flags = _genFlags({"var1": keys, "var2": keys, "var3": keys})
     flags[:, "var1"] = BAD
     flags[:, "var1"] = DOUBTFUL
     flags[:, "var2"] = BAD
@@ -140,35 +137,33 @@
     tflags = scheme.toExternal(flags)
     assert (tflags["var2"].replace(-9999, np.nan).dropna() == 90).all(axis=None)
     assert (tflags["var1"].iloc[1::3] == 90210).all(axis=None)
     assert (tflags["var1"].iloc[2::3] == 90002).all(axis=None)
 
 
 def test_positionalTranslatorIntegration():
-
     data = initData(3)
     col: str = data.columns[0]
 
     scheme = PositionalScheme()
     saqc = SaQC(data=data, scheme=scheme)
     saqc = saqc.flagMissing(col).flagRange(col, min=3, max=10, flag=DOUBTFUL)
     flags = saqc.flags
 
-    for field in flags.columns:
+    for field in flags.keys():
         assert flags[field].astype(str).str.match("^9[012]*$").all()
 
     round_trip = scheme.toExternal(scheme.toInternal(flags))
 
     assert (flags.values == round_trip.values).all()
     assert (flags.index == round_trip.index).all()
     assert (flags.columns == round_trip.columns).all()
 
 
 def test_dmpTranslatorIntegration():
-
     data = initData(1)
     col = data.columns[0]
 
     scheme = DmpScheme()
     saqc = SaQC(data=data, scheme=scheme)
     saqc = saqc.flagMissing(col).flagRange(col, min=3, max=10)
     flags = saqc.flags
@@ -207,15 +202,14 @@
         saqc.flagRange(col, min=3, max=10, cause="SOMETHING_STUPID").flags
 
     with pytest.raises(ValueError):
         saqc.flagRange(col, min=3, max=10, cause="").flags
 
 
 def _buildupSaQCObjects():
-
     """
     return two evaluated saqc objects calling the same functions,
     whereas the flags from the evaluetion of the first objetc are
     used as input flags of the second
     """
     data = initData(3)
     col = data.columns[0]
@@ -229,15 +223,14 @@
         )
         flags = saqc._flags
         out.append(saqc)
     return out
 
 
 def test_translationPreservesFlags():
-
     saqc1, saqc2 = _buildupSaQCObjects()
     flags1 = saqc1._flags
     flags2 = saqc2._flags
 
     for k in flags2.columns:
         got = flags2.history[k].hist
 
@@ -266,15 +259,14 @@
 
         assert hist1.equals(hist21)
         assert hist1.equals(hist22)
         assert hist21.equals(hist22)
 
 
 def test_positionalMulitcallsPreserveState():
-
     saqc1, saqc2 = _buildupSaQCObjects()
 
     scheme = PositionalScheme()
     flags1 = saqc1._flags
     flags2 = saqc2._flags
     tflags1 = scheme.toExternal(flags1).astype(str)
     tflags2 = scheme.toExternal(flags2).astype(str)
```

### Comparing `saqc-2.3/tests/funcs/test_constants_detection.py` & `saqc-2.4.0/tests/funcs/test_constants_detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pytest
 
-from saqc.constants import BAD, UNFLAGGED
+from saqc import BAD, UNFLAGGED
 from saqc.core import SaQC, initFlagsLike
 from tests.common import initData
 
 
 @pytest.fixture
 def data():
     constants_data = initData(
         1, start_date="2011-01-01 00:00:00", end_date="2011-01-01 03:00:00", freq="5min"
     )
-    constants_data.iloc[5:25] = 200
+    for c in constants_data.columns:
+        constants_data[c].iloc[5:25] = 200
     return constants_data
 
 
 def test_constants_flagBasic(data):
     field, *_ = data.columns
     flags = initFlagsLike(data)
     qc = SaQC(data, flags)
```

### Comparing `saqc-2.3/tests/funcs/test_functions.py` & `saqc-2.4.0/tests/funcs/test_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 import pytest
 
-import dios
 import saqc
-from saqc.constants import BAD, DOUBTFUL, UNFLAGGED
-from saqc.core import initFlagsLike
-from saqc.core.core import SaQC
+from saqc import BAD, DOUBTFUL, UNFLAGGED, SaQC
+from saqc.core import DictOfSeries, initFlagsLike
 from tests.common import initData
-from tests.fixtures import char_dict, course_1
+from tests.fixtures import char_dict, course_1  # noqa, todo: fix fixtures
 
 
 @pytest.fixture
 def data():
     return initData(cols=1, start_date="2016-01-01", end_date="2018-12-31", freq="1D")
 
 
@@ -30,15 +28,15 @@
 
 
 def test_statPass():
     data = pd.Series(0, index=pd.date_range("2000", "2001", freq="1D"), name="data")
     noise = [-1, 1] * 10
     data[100:120] = noise
     data[200:210] = noise[:10]
-    data = dios.DictOfSeries(data)
+    data = DictOfSeries(data=data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagByStatLowPass(
         "data", np.std, "20D", 0.999, "5D", 0.999, 0, flag=BAD
     )
     assert (qc.flags["data"].iloc[:100] == UNFLAGGED).all()
     assert (qc.flags["data"].iloc[100:120] == BAD).all()
     assert (qc.flags["data"].iloc[121:] == UNFLAGGED).all()
@@ -51,16 +49,16 @@
     qc = qc.flagRange(field, min=min, max=max, flag=BAD)
     flagged = qc.flags[field] > UNFLAGGED
     expected = (data[field] < min) | (data[field] > max)
     assert all(flagged == expected)
 
 
 def test_flagSesonalRange(data, field):
-    data.iloc[::2] = 0
-    data.iloc[1::2] = 50
+    data[field].iloc[::2] = 0
+    data[field].iloc[1::2] = 50
     nyears = len(data[field].index.year.unique())
 
     tests = [
         (
             {
                 "min": 1,
                 "max": 100,
@@ -87,15 +85,15 @@
     flags = initFlagsLike(data)
     qc = SaQC(data, flags)
     for test, expected in tests:
         newfield = f"{field}_masked"
         start = f"{test['startmonth']:02}-{test['startday']:02}T00:00:00"
         end = f"{test['endmonth']:02}-{test['endday']:02}T00:00:00"
 
-        qc = qc.copyField(field, field + "_masked")
+        qc = qc.copyField(field, newfield)
         qc = qc.selectTime(
             newfield,
             mode="periodic",
             start=start,
             end=end,
             closed=True,
             flag=BAD,
@@ -126,20 +124,20 @@
 
     qc = SaQC(data, flags).forceFlags(field, flag=DOUBTFUL)
     assert all(qc._flags[field] == DOUBTFUL)
 
 
 def test_flagIsolated(data, field):
     flags = initFlagsLike(data)
-    d_len = data.shape[0][0]
-    data.iloc[1:3, 0] = np.nan
-    data.iloc[4:5, 0] = np.nan
+    d_len = len(data[field].index)
+    data[field].iloc[1:3] = np.nan
+    data[field].iloc[4:5] = np.nan
     flags[data[field].index[5:6], field] = BAD
-    data.iloc[11:13, 0] = np.nan
-    data.iloc[15:17, 0] = np.nan
+    data[field].iloc[11:13] = np.nan
+    data[field].iloc[15:17] = np.nan
 
     #              data  flags
     # 2016-01-01   0.0   -inf
     # 2016-01-02   NaN   -inf
     # 2016-01-03   NaN   -inf
     # 2016-01-04   3.0   -inf
     # 2016-01-05   NaN   -inf
@@ -283,15 +281,15 @@
 
 
 def test_transferFlags():
     data = pd.DataFrame({"a": [1, 2], "b": [1, 2], "c": [1, 2]})
     qc = saqc.SaQC(data)
     qc = qc.flagRange("a", max=1.5)
     with pytest.deprecated_call():
-        qc = qc.transferFlags(["a", "a"], ["b", "c"])
+        qc = qc.transferFlags(["a", "a"], ["b", "c"])  # noqa
         assert np.all(qc.flags["b"].values == np.array([UNFLAGGED, BAD]))
         assert np.all(qc.flags["c"].values == np.array([UNFLAGGED, BAD]))
 
 
 def test_flagJumps():
     data = pd.DataFrame(
         {"a": [1, 1, 1, 1, 1, 6, 6, 6, 6, 6]},
```

### Comparing `saqc-2.3/tests/funcs/test_generic_api_functions.py` & `saqc-2.4.0/tests/lib/test_ts_operators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,233 +1,259 @@
-#! /usr/bin/env python
-
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
+from __future__ import annotations
 
-# -*- coding: utf-8 -*-
-
+import numpy as np
 import pandas as pd
 import pytest
+from pandas.testing import assert_series_equal
+
+import saqc.lib.ts_operators as tsops
+
 
-from dios.dios.dios import DictOfSeries
-from saqc import SaQC
-from saqc.constants import BAD, FILTER_ALL, UNFLAGGED
-from saqc.core.flags import Flags
-from saqc.lib.tools import toSequence
-from tests.common import initData
+def test_butterFilter():
+    assert (
+        tsops.butterFilter(pd.Series([1, -1] * 100), cutoff=0.1)
+        - pd.Series([1, -1] * 100)
+    ).mean() < 0.5
 
 
-@pytest.fixture
-def data():
-    return initData()
+T = True
+F = False
 
 
-def test_emptyData():
-    # test that things do not break with empty data sets
-    saqc = SaQC(data=pd.DataFrame({"x": [], "y": []}))
+@pytest.mark.parametrize(
+    "arr,maxc,expected",
+    [
+        (np.array([]), 1, False),
+        (np.array([F]), 1, False),
+        (np.array([F, F, F]), 1, False),
+        #
+        (np.array([T]), 0, True),
+        (np.array([T]), 1, False),
+        #
+        (np.array([F, T, F]), 0, True),
+        (np.array([F, T, F]), 1, False),
+        #
+        (np.array([F, T, T, T, T, F]), 0, True),
+        (np.array([F, T, T, T, T, F]), 1, True),
+        (np.array([F, T, T, T, T, F]), 2, True),
+        (np.array([F, T, T, T, T, F]), 3, True),
+        (np.array([F, T, T, T, T, F]), 4, False),
+        (np.array([F, T, T, T, T, F]), 5, False),
+        #
+        (np.array([F, T, T, F, T, T, F]), 2, False),
+    ],
+)
+def test__exceedConsecutiveNanLimit(arr, maxc, expected):
+    result = tsops._exceedConsecutiveNanLimit(arr, maxc)
+    assert result is expected
 
-    saqc.flagGeneric("x", func=lambda x: x < 0)
-    assert saqc.data.empty
-    assert saqc.flags.empty
 
-    saqc = saqc.processGeneric(field="x", target="y", func=lambda x: x + 2)
-    assert saqc.data.empty
-    assert saqc.flags.empty
+def dtSeries(data, freq="1d"):
+    index = pd.date_range(start="2020", periods=len(data), freq=freq)
+    return pd.Series(data=data, index=index, dtype=float)
 
 
 @pytest.mark.parametrize(
-    "targets, func",
+    "data",
+    [dtSeries([0, 1, 2]), dtSeries([0, np.nan, 2])],
+)
+def test_identity(data):
+    from saqc.lib.ts_operators import identity
+
+    result = identity(data)
+    assert result is data
+
+
+@pytest.mark.parametrize(
+    "data,expected",
     [
-        (["tmp"], lambda x, y: pd.Series(True, index=x.index.union(y.index))),
-        (
-            ["tmp1", "tmp2"],
-            lambda x, y: [pd.Series(True, index=x.index.union(y.index))] * 2,
-        ),
+        (dtSeries([0, 1, 2]), 3),
+        (dtSeries([0, np.nan, 2]), 2),
     ],
 )
-def test_writeTargetFlagGeneric(data, targets, func):
-    expected_meta = {
-        "func": "flagGeneric",
-        "args": (data.columns.tolist(), targets),
-        "kwargs": {
-            "func": func.__name__,
-            "flag": BAD,
-            "dfilter": FILTER_ALL,
-        },
-    }
+def test_count(data, expected):
+    # count is labeled as a dummy function, this means
+    # we need to ensure it exists with a resampler object.
+    resampler = data.resample("2d")
+    assert hasattr(resampler, "count")
 
-    saqc = SaQC(data=data)
-    saqc = saqc.flagGeneric(field=data.columns, target=targets, func=func, flag=BAD)
-    for target in targets:
-        assert saqc._flags.history[target].hist.iloc[0].tolist() == [BAD]
-        assert saqc._flags.history[target].meta[0] == expected_meta
+    from saqc.lib.ts_operators import count
+
+    result = count(data)
+    assert result == expected
 
 
 @pytest.mark.parametrize(
-    "fields, func",
+    "data,expected",
     [
-        (["var1"], lambda x: pd.Series(True, index=x.index)),
         (
-            ["var1", "var2"],
-            lambda x, y: [pd.Series(True, index=x.index.union(y.index))] * 2,
+            dtSeries([1, 2, np.inf, np.nan]),
+            dtSeries([np.log(1), np.log(2), np.inf, np.nan]),
+        ),
+        pytest.param(
+            dtSeries(
+                [
+                    0,
+                    -2,
+                    -1,
+                    -np.inf,
+                ]
+            ),
+            dtSeries([np.nan, np.nan, np.nan, np.nan]),
+            marks=pytest.mark.xfail(reason="zeroLog(0) did not return NaN for 0"),
         ),
     ],
 )
-def test_overwriteFieldFlagGeneric(data, fields, func):
+def test_zeroLog(data, expected):
+    from saqc.lib.ts_operators import zeroLog
 
-    flag = 12
+    result = zeroLog(data)
+    assert_series_equal(result, expected, check_freq=False, check_names=False)
 
-    expected_meta = {
-        "func": "flagGeneric",
-        "args": (fields, fields),
-        "kwargs": {
-            "func": func.__name__,
-            "flag": flag,
-            "dfilter": FILTER_ALL,
-        },
-    }
 
-    saqc = SaQC(
-        data=data.copy(),
-        flags=Flags(
-            {
-                k: pd.Series(data[k] % 2, index=data[k].index).replace(
-                    {0: UNFLAGGED, 1: 127}
-                )
-                for k in data.columns
-            }
+@pytest.mark.parametrize(
+    "data,expected",
+    [
+        (dtSeries([1, 2, 3]), dtSeries([np.nan, 1440, 1440])),
+        (
+            pd.Series(
+                [1, 2, 3],
+                index=pd.DatetimeIndex(["2020-01-01", "2020-01-03", "2020-01-13"]),
+            ),
+            dtSeries([np.nan, 2880, 14400]),
         ),
-    )
+    ],
+)
+def test_deltaT(data, expected):
+    from saqc.lib.ts_operators import deltaT
 
-    res = saqc.flagGeneric(field=fields, func=func, flag=flag)
-    for field in fields:
-        histcol1 = res._flags.history[field].hist[1]
-        assert (histcol1 == flag).all()
-        assert (data[field] == res.data[field]).all(axis=None)
-        assert res._flags.history[field].meta[0] == {}
-        assert res._flags.history[field].meta[1] == expected_meta
+    result = deltaT(data)
+    assert_series_equal(
+        result,
+        expected,
+        check_dtype=False,
+        check_names=False,
+        check_index=False,
+        check_freq=False,
+    )
 
 
 @pytest.mark.parametrize(
-    "targets, func",
-    [
-        (["tmp"], lambda x, y: x + y),
-        (["tmp1", "tmp2"], lambda x, y: (x + y, y * 2)),
-    ],
-)
-def test_writeTargetProcGeneric(data, targets, func):
-    fields = ["var1", "var2"]
-    dfilter = 128
-
-    expected_data = DictOfSeries(
-        func(*[data[f] for f in fields]), columns=toSequence(targets)
-    ).squeeze()
-
-    expected_meta = {
-        "func": "procGeneric",
-        "args": (fields, targets),
-        "kwargs": {
-            "func": func.__name__,
-            "dfilter": dfilter,
-            "label": "generic",
-        },
-    }
-    saqc = SaQC(
-        data=data,
-        flags=Flags({k: pd.Series(127.0, index=data[k].index) for k in data.columns}),
-    )
-    res = saqc.processGeneric(
-        field=fields,
-        target=targets,
-        func=func,
-        dfilter=dfilter,
-        label="generic",
-    )
-    assert (expected_data == res.data[targets].squeeze()).all(axis=None)
-    # check that new histories where created
-    for target in targets:
-        assert res._flags.history[target].hist.iloc[0].isna().all()
-        assert res._flags.history[target].meta[0] == expected_meta
+    "data,expected",
+    [
+        pytest.param(
+            pd.Series(
+                # We use as values the delta of total seconds from the last value.
+                # This way the 'derivative' should be 1 for each result value.
+                [1, 2880, 14400],
+                index=pd.DatetimeIndex(["2020-01-01", "2020-01-03", "2020-01-13"]),
+            ),
+            pd.Series(
+                [np.nan, 1, 1],
+                index=pd.DatetimeIndex(["2020-01-01", "2020-01-03", "2020-01-13"]),
+            ),
+        ),
+    ],
+)
+def test_derivative(data, expected):
+    from saqc.lib.ts_operators import derivative
+
+    result = derivative(data)
+    assert_series_equal(result, expected, check_dtype=False, check_names=False)
 
 
 @pytest.mark.parametrize(
-    "fields, func",
-    [
-        (["var1"], lambda x: x * 2),
-        (["var1", "var2"], lambda x, y: (x + y, y * 2)),
-    ],
-)
-def test_overwriteFieldProcGeneric(data, fields, func):
-    dfilter = 128
-    expected_data = DictOfSeries(
-        func(*[data[f] for f in fields]), columns=fields
-    ).squeeze()
-
-    expected_meta = {
-        "func": "procGeneric",
-        "args": (fields, fields),
-        "kwargs": {
-            "func": func.__name__,
-            "dfilter": dfilter,
-            "label": "generic",
-        },
-    }
-
-    saqc = SaQC(
-        data=data,
-        flags=Flags({k: pd.Series(127.0, index=data[k].index) for k in data.columns}),
-    )
+    "data,expected",
+    [
+        (dtSeries([1, 1, 1]), dtSeries([np.nan, 0, 0])),
+        (dtSeries([1, 10, 100]), dtSeries([np.nan, 9, 90])),
+        (dtSeries([-np.inf, np.inf, 0]), dtSeries([np.nan, np.inf, -np.inf])),
+        (dtSeries([0, np.nan, 0]), dtSeries([np.nan, np.nan, np.nan])),
+    ],
+)
+def test_difference(data, expected):
+    from saqc.lib.ts_operators import difference
 
-    res = saqc.processGeneric(field=fields, func=func, dfilter=dfilter, label="generic")
-    assert (expected_data == res.data[fields].squeeze()).all(axis=None)
-    # check that the histories got appended
-    for field in fields:
-        assert (res._flags.history[field].hist[0] == 127.0).all()
-        assert res._flags.history[field].hist[1].isna().all()
-        assert res._flags.history[field].meta[0] == {}
-        assert res._flags.history[field].meta[1] == expected_meta
+    result = difference(data)
+    assert_series_equal(result, expected, check_names=False)
 
 
-def test_label():
-    dat = pd.DataFrame(
-        {"data1": [1, 1, 5, 2, 1], "data2": [1, 1, 2, 3, 4], "data3": [1, 1, 2, 3, 4]},
-        index=pd.date_range("2000", "2005", periods=5),
-    )
+@pytest.mark.parametrize(
+    "data,expected",
+    [
+        (dtSeries([1, 1, 1]), dtSeries([np.nan, 0, 0])),
+        (dtSeries([1, 10, 100]), dtSeries([np.nan, 0.9, 0.9])),
+        (dtSeries([-np.inf, np.inf, 0]), dtSeries([np.nan, np.nan, -np.inf])),
+        (dtSeries([0, np.nan, 0]), dtSeries([np.nan, np.nan, np.nan])),
+    ],
+)
+def test_rateOfChange(data, expected):
+    from saqc.lib.ts_operators import rateOfChange
 
-    qc = SaQC(dat)
-    qc = qc.flagRange("data1", max=4, label="out of range")
-    qc = qc.flagRange("data1", max=0, label="out of range2")
-    qc = qc.flagGeneric(
-        ["data1", "data3"],
-        target="data2",
-        func=lambda x, y: isflagged(x, "out of range") | isflagged(y),
-    )
-    assert list((qc.flags["data2"] > 0).values) == [False, False, True, False, False]
+    result = rateOfChange(data)
+    assert_series_equal(result, expected, check_names=False)
 
 
 @pytest.mark.parametrize(
-    "kwargs, got, expected",
+    "limit,extrapolate,data,expected",
     [
         (
-            {
-                "lower": 0,
-            },
-            [-9, -2, 1, 2, 9],
-            [0, 0, 1, 2, 9],
+            1,
+            None,
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+        ),
+        (
+            2,
+            "backward",
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [0, 0, np.nan, np.nan, np.nan, 4, np.nan],
+        ),
+        (
+            2,
+            None,
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+        ),
+        (
+            3,
+            None,
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+        ),
+        (
+            3,
+            "forward",
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, 4],
+        ),
+        (
+            4,
+            None,
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [np.nan, 0, 1, 2, 3, 4, np.nan],
+        ),
+        (
+            4,
+            "both",
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [np.nan, 0, 1, 2, 3, 4, np.nan],
+        ),
+        (
+            None,
+            None,
+            [np.nan, 0, np.nan, np.nan, np.nan, 4, np.nan],
+            [np.nan, 0, 1, 2, 3, 4, np.nan],
         ),
-        ({"upper": 3}, [-9, -2, 1, 2, 9], [-9, -2, 1, 2, 3]),
-        ({"lower": -6, "upper": 3}, [-9, -2, 1, 2, 9], [-6, -2, 1, 2, 3]),
     ],
 )
-def test_processGenericClip(kwargs, got, expected):
-    field = "data"
-    got = pd.DataFrame(
-        got, columns=[field], index=pd.date_range("2020-06-30", periods=len(got))
-    )
-    expected = pd.DataFrame(
-        expected,
-        columns=[field],
-        index=pd.date_range("2020-06-30", periods=len(expected)),
+def test_interpolatNANs(limit, extrapolate, data, expected):
+    got = tsops.interpolateNANs(
+        pd.Series(data), gap_limit=limit, method="linear", extrapolate=extrapolate
     )
-    qc = SaQC(got).processGeneric(field, func=lambda x: clip(x, **kwargs))
-    assert (qc._data[field] == expected[field]).all()
+    try:
+        assert got.equals(pd.Series(expected, dtype=float))
+    except AssertionError:
+        print("stop")
```

### Comparing `saqc-2.3/tests/funcs/test_generic_config_functions.py` & `saqc-2.4.0/tests/funcs/test_generic_config_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 
 import ast
 
 import numpy as np
 import pandas as pd
 import pytest
 
-import dios
-from saqc import SaQC
-from saqc.constants import BAD, UNFLAGGED
-from saqc.core import initFlagsLike
-from saqc.core.flags import Flags
-from saqc.core.reader import fromConfig
-from saqc.core.register import register
-from saqc.core.visitor import ConfigFunctionParser
+from saqc import BAD, UNFLAGGED, SaQC
+from saqc.core import DictOfSeries, Flags, initFlagsLike, register
 from saqc.funcs.generic import _execGeneric
+from saqc.parsing.reader import fromConfig
+from saqc.parsing.visitor import ConfigFunctionParser
 from tests.common import initData, writeIO
 
 
 @pytest.fixture
 def data():
     return initData()
 
@@ -32,18 +28,18 @@
 @pytest.fixture
 def data_diff():
     data = initData(cols=3)
     col0 = data[data.columns[0]]
     col1 = data[data.columns[1]]
     mid = len(col0) // 2
     offset = len(col0) // 8
-    return dios.DictOfSeries(
-        data={
-            col0.name: col0.iloc[: mid + offset],
-            col1.name: col1.iloc[mid - offset :],
+    return DictOfSeries(
+        {
+            data.columns[0]: col0.iloc[: mid + offset],
+            data.columns[1]: col1.iloc[mid - offset :],
         }
     )
 
 
 def _compileGeneric(expr):
     tree = ast.parse(expr, mode="eval")
     _, kwargs = ConfigFunctionParser().parse(tree.body)
@@ -91,15 +87,14 @@
     for field, test, expected in tests:
         func = _compileGeneric(f"flagGeneric(func={test})")
         result = _execGeneric(Flags({f: flags[f] for f in field}), data[field], func)
         assert (result == expected).all(axis=None)
 
 
 def test_arithmeticOperators(data):
-
     var1, *_ = data.columns
 
     data = data[var1]
     flags = Flags({var1: pd.Series(UNFLAGGED, index=data.index)})
 
     tests = [
         ("var1 + 100 > 110", data + 100 > 110),
@@ -114,15 +109,15 @@
         func = _compileGeneric(f"processGeneric(func={test})")
         result = _execGeneric(flags, data, func)
         assert (result == expected).all(axis=None)
 
 
 def test_nonReduncingBuiltins(data):
     var1, *_ = data.columns
-    data = data.iloc[1:10, 0]
+    data = data[var1].iloc[1:10]
     flags = Flags({var1: pd.Series(UNFLAGGED, index=data.index)})
 
     tests = [
         ("abs(x)", np.abs(data)),
         ("log(x)", np.log(data)),
         ("exp(x)", np.exp(data)),
     ]
@@ -146,15 +141,14 @@
     for field, test, expected in tests:
         func = _compileGeneric(f"flagGeneric(func={test})")
         result = _execGeneric(Flags({f: flags[f] for f in field}), data[field], func)
         assert (result == expected).all(axis=None)
 
 
 def test_variableAssignments(data):
-
     config = f"""
     varname ; test
     dummy1  ; processGeneric(field=["var1", "var2"], func=x + y)
     dummy2  ; flagGeneric(field=["var1", "var2"], func=x + y > 0)
     """
 
     fobj = writeIO(config)
@@ -214,15 +208,14 @@
     fobj = writeIO(config)
     with pytest.raises(ValueError):
         fromConfig(fobj, data_diff)
 
 
 @pytest.mark.slow
 def test_callableArgumentsUnary(data):
-
     window = 5
 
     @register(mask=["field"], demask=["field"], squeeze=["field"])
     def testFuncUnary(saqc, field, func, **kwargs):
         value = saqc._data[field].rolling(window=window).apply(func)
         saqc._data[field] = value
         return saqc
@@ -235,15 +228,15 @@
     """
 
     tests = [
         # ("sum", np.nansum),
         ("std(exp(x))", lambda x: np.std(np.exp(x))),
     ]
 
-    for (name, func) in tests:
+    for name, func in tests:
         fobj = writeIO(config.format(name))
         result_config = fromConfig(fobj, data).data
         result_api = SaQC(data).testFuncUnary(var, func=func).data
         expected = data[var].rolling(window=window).apply(func)
         assert (result_config[var].dropna() == expected.dropna()).all(axis=None)
         assert (result_api[var].dropna() == expected.dropna()).all(axis=None)
 
@@ -262,25 +255,24 @@
     """
 
     tests = [
         ("x + y", lambda x, y: x + y),
         ("y - (x * 2)", lambda y, x: y - (x * 2)),
     ]
 
-    for (name, func) in tests:
+    for name, func in tests:
         fobj = writeIO(config.format(name))
         result_config = fromConfig(fobj, data).data
         result_api = SaQC(data).testFuncBinary(var1, func=func).data
         expected = func(data[var1], data[var2])
         assert (result_config[var1].dropna() == expected.dropna()).all(axis=None)
         assert (result_api[var1].dropna() == expected.dropna()).all(axis=None)
 
 
 def test_isflagged(data):
-
     var1, var2, *_ = data.columns
     flags = initFlagsLike(data)
     flags[data[var1].index[::2], var1] = BAD
 
     tests = [
         ([var1], f"isflagged(x)", flags[var1] > UNFLAGGED),
         ([var1], f"isflagged(x)", flags[var1] >= BAD),
```

### Comparing `saqc-2.3/tests/funcs/test_outlier_detection.py` & `saqc-2.4.0/tests/funcs/test_outlier_detection.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 
 import numpy as np
 import pandas as pd
 
 # see test/functs/fixtures.py for global fixtures "course_..."
 import pytest
 
-import dios
 import saqc
-from saqc.constants import BAD, UNFLAGGED
-from saqc.core import SaQC, initFlagsLike
+from saqc import BAD, UNFLAGGED
+from saqc.core import DictOfSeries, SaQC, initFlagsLike
 from tests.fixtures import char_dict, course_1, course_2, course_3, course_4
 
 
 @pytest.fixture(scope="module")
 def spiky_data():
     index = pd.date_range(start="2011-01-01", end="2011-01-05", freq="5min")
-    s = pd.Series(np.linspace(1, 2, index.size), index=index, name="spiky_data")
+    s = pd.Series(np.linspace(1, 2, index.size), index=index)
     s.iloc[100] = 100
     s.iloc[1000] = -100
     flag_assertion = [100, 1000]
-    return dios.DictOfSeries(s), flag_assertion
+    return DictOfSeries(spiky_data=s), flag_assertion
 
 
 def test_flagMad(spiky_data):
     data = spiky_data[0]
     field, *_ = data.columns
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagMAD(field, "1H", flag=BAD)
@@ -92,18 +91,18 @@
     data1, characteristics = dat(
         periods=1000, initial_level=5, final_level=15, out_val=50
     )
     data2, characteristics = dat(
         periods=1000, initial_level=20, final_level=1, out_val=30
     )
     fields = ["field1", "field2"]
-    s1, s2 = data1.squeeze(), data2.squeeze()
+    s1, s2 = data1["data"], data2["data"]
     s1 = pd.Series(data=s1.values, index=s1.index)
     s2 = pd.Series(data=s2.values, index=s1.index)
-    data = dios.DictOfSeries([s1, s2], columns=["field1", "field2"])
+    data = DictOfSeries(field1=s1, field2=s2)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagMVScores(
         field=fields,
         trafo=np.log,
         iter_start=0.95,
         n=10,
         flag=BAD,
@@ -128,23 +127,24 @@
 
 
 @pytest.mark.parametrize("dat", [pytest.lazy_fixture("course_2")])
 def test_flagCrossStatistics(dat):
     data1, characteristics = dat(initial_level=0, final_level=0, out_val=0)
     data2, characteristics = dat(initial_level=0, final_level=0, out_val=10)
     fields = ["field1", "field2"]
-    s1, s2 = data1.squeeze(), data2.squeeze()
+    s1, s2 = data1["data"], data2["data"]
     s1 = pd.Series(data=s1.values, index=s1.index)
     s2 = pd.Series(data=s2.values, index=s1.index)
-    data = dios.DictOfSeries([s1, s2], columns=["field1", "field2"])
+    data = DictOfSeries(field1=s1, field2=s2)
     flags = initFlagsLike(data)
 
-    qc = SaQC(data, flags).flagCrossStatistics(
-        fields, thresh=3, method=np.mean, flag=BAD
-    )
+    with pytest.deprecated_call():
+        qc = SaQC(data, flags).flagCrossStatistics(
+            fields, thresh=3, method=np.mean, flag=BAD
+        )
     for field in fields:
         isflagged = qc.flags[field] > UNFLAGGED
         assert isflagged[characteristics["raise"]].all()
 
 
 def test_flagZScores():
     np.random.seed(seed=1)
@@ -154,23 +154,52 @@
         name="data",
     )
     data.iloc[[5, 80]] = 5
     data.iloc[[40]] = -6
     qc = saqc.SaQC(data)
     qc = qc.flagZScore("data", window=None)
 
-    assert (qc.flags.to_df().iloc[[5, 40, 80], 0] > 0).all()
+    assert (qc.flags.to_pandas().iloc[[5, 40, 80], 0] > 0).all()
 
     qc = saqc.SaQC(data)
     qc = qc.flagZScore("data", window=None, min_residuals=10)
 
-    assert (qc.flags.to_df()["data"] < 0).all()
+    assert (qc.flags.to_pandas()["data"] < 0).all()
 
     qc = saqc.SaQC(data)
     qc = qc.flagZScore("data", window="20D")
 
-    assert (qc.flags.to_df().iloc[[40, 80], 0] > 0).all()
+    assert (qc.flags.to_pandas().iloc[[40, 80], 0] > 0).all()
 
     qc = saqc.SaQC(data)
     qc = qc.flagZScore("data", window=20)
 
-    assert (qc.flags.to_df().iloc[[40, 80], 0] > 0).all()
+    assert (qc.flags.to_pandas().iloc[[40, 80], 0] > 0).all()
+
+
+@pytest.mark.parametrize("n", [1, 10])
+@pytest.mark.parametrize("p", [1, 2])
+@pytest.mark.parametrize("thresh", ["auto", 2])
+def test_flagUniLOF(spiky_data, n, p, thresh):
+    data = spiky_data[0]
+    field, *_ = data.columns
+    qc = SaQC(data).flagUniLOF(field, n=n, p=p, thresh=thresh)
+    flag_result = qc.flags[field]
+    test_sum = (flag_result[spiky_data[1]] == BAD).sum()
+    try:
+        assert test_sum == len(spiky_data[1])
+    except AssertionError:
+        print("stop")
+
+
+@pytest.mark.parametrize("vars", [1, 2, 3])
+@pytest.mark.parametrize("p", [1, 2])
+@pytest.mark.parametrize("thresh", ["auto", 2])
+def test_flagLOF(spiky_data, vars, p, thresh):
+    data = pd.DataFrame(
+        {f"data{v}": spiky_data[0].to_pandas().squeeze() for v in range(vars)}
+    )
+    field, *_ = data.columns
+    qc = SaQC(data).flagLOF(field)
+    flag_result = qc.flags[field]
+    test_sum = (flag_result[spiky_data[1]] == BAD).sum()
+    assert test_sum == len(spiky_data[1])
```

### Comparing `saqc-2.3/tests/funcs/test_pattern_rec.py` & `saqc-2.4.0/tests/funcs/test_pattern_rec.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 import pandas as pd
 import pytest
 
-import dios
-from saqc.constants import BAD, UNFLAGGED
-from saqc.core import SaQC, initFlagsLike
+from saqc import BAD, UNFLAGGED, SaQC
+from saqc.core import DictOfSeries, initFlagsLike
 from tests.common import initData
 
 
 @pytest.fixture
 def data():
     return initData(cols=1, start_date="2016-01-01", end_date="2018-12-31", freq="1D")
 
@@ -28,15 +27,15 @@
 @pytest.mark.parametrize("plot", [True, False])
 @pytest.mark.parametrize("normalize", [True, False])
 def test_flagPattern_dtw(plot, normalize):
     data = pd.Series(0, index=pd.date_range(start="2000", end="2001", freq="1d"))
     data.iloc[10:18] = [0, 5, 6, 7, 6, 8, 5, 0]
     pattern = data.iloc[10:18]
 
-    data = dios.DictOfSeries(dict(data=data, pattern_data=pattern))
+    data = DictOfSeries(data=data, pattern_data=pattern)
     flags = initFlagsLike(data, name="data")
     qc = SaQC(data, flags).flagPatternByDTW(
         "data",
         reference="pattern_data",
         plot=plot,
         normalize=normalize,
         flag=BAD,
```

### Comparing `saqc-2.3/tests/funcs/test_proc_functions.py` & `saqc-2.4.0/tests/funcs/test_proc_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 import numpy as np
 import pandas as pd
 
 # see test/functs/fixtures.py for global fixtures "course_..."
 import pytest
 
-import dios
 import saqc
-from saqc.constants import UNFLAGGED
-from saqc.core import SaQC, initFlagsLike
+from saqc import UNFLAGGED, SaQC
+from saqc.core import DictOfSeries, initFlagsLike
 from saqc.lib.ts_operators import linearInterpolation, polynomialInterpolation
-from tests.fixtures import char_dict, course_3, course_5
+from tests.fixtures import char_dict, course_3, course_5  # noqa, todo: fix fixtures
 
 
 def test_rollingInterpolateMissing(course_5):
     data, characteristics = course_5(periods=10, nan_slice=[5, 6])
     field = data.columns[0]
-    data = dios.DictOfSeries(data)
+    data = DictOfSeries(data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).interpolateByRolling(
         field,
         3,
         func=np.median,
         center=True,
         min_periods=0,
@@ -42,42 +41,42 @@
         center=False,
         min_periods=3,
         interpol_flag=UNFLAGGED,
     )
     assert qc.data[field][characteristics["missing"]].isna().all()
 
 
-def test_interpolateMissing(course_5):
+def test_interpolate(course_5):
     data, characteristics = course_5(periods=10, nan_slice=[5])
     field = data.columns[0]
-    data = dios.DictOfSeries(data)
+    data = DictOfSeries(data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags)
 
-    qc_lin = qc.interpolateInvalid(field, method="linear")
-    qc_poly = qc.interpolateInvalid(field, method="polynomial")
+    qc_lin = qc.interpolate(field, method="linear")
+    qc_poly = qc.interpolate(field, method="polynomial")
     assert qc_lin.data[field][characteristics["missing"]].notna().all()
     assert qc_poly.data[field][characteristics["missing"]].notna().all()
 
     data, characteristics = course_5(periods=10, nan_slice=[5, 6, 7])
 
     qc = SaQC(data, flags)
-    qc_lin_1 = qc.interpolateInvalid(field, method="linear", limit=2)
-    qc_lin_2 = qc.interpolateInvalid(field, method="linear", limit=3)
-    qc_lin_3 = qc.interpolateInvalid(field, method="linear", limit=4)
+    qc_lin_1 = qc.interpolate(field, method="linear", limit=2)
+    qc_lin_2 = qc.interpolate(field, method="linear", limit=3)
+    qc_lin_3 = qc.interpolate(field, method="linear", limit=4)
 
     assert qc_lin_1.data[field][characteristics["missing"]].isna().all()
     assert qc_lin_2.data[field][characteristics["missing"]].isna().all()
     assert qc_lin_3.data[field][characteristics["missing"]].notna().all()
 
 
 def test_transform(course_5):
     data, characteristics = course_5(periods=10, nan_slice=[5, 6])
     field = data.columns[0]
-    data = dios.DictOfSeries(data)
+    data = DictOfSeries(data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags)
 
     result = qc.transform(field, func=linearInterpolation)
     assert result.data[field][characteristics["missing"]].isna().all()
 
     result = qc.transform(field, func=lambda x: linearInterpolation(x, inter_limit=3))
@@ -89,15 +88,15 @@
     )
     assert result.data[field][characteristics["missing"]].notna().all()
 
 
 def test_resample(course_5):
     data, _ = course_5(freq="1min", periods=30, nan_slice=[1, 11, 12, 22, 24, 26])
     field = data.columns[0]
-    data = dios.DictOfSeries(data)
+    data = DictOfSeries(data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).resample(
         field,
         "10min",
         np.mean,
         maxna=2,
         maxna_group=1,
@@ -106,29 +105,27 @@
     assert np.isnan(qc.data[field].iloc[1])
     assert np.isnan(qc.data[field].iloc[2])
 
 
 def test_interpolateGrid(course_5, course_3):
     data, _ = course_5()
     data_grid, _ = course_3()
-    data["grid"] = data_grid.to_df()
+    data["grid"] = data_grid["data"]
     flags = initFlagsLike(data)
-    SaQC(data, flags).interpolateIndex(
-        "data", "1h", "time", grid_field="grid", limit=10
-    )
+    SaQC(data, flags).align("data", "1h", "time", grid_field="grid", limit=10)
 
 
 @pytest.mark.slow
 def test_offsetCorrecture():
     data = pd.Series(0, index=pd.date_range("2000", freq="1d", periods=100), name="dat")
     data.iloc[30:40] = -100
     data.iloc[70:80] = 100
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).correctOffset("dat", 40, 20, "3d", 1)
-    assert (qc.data == 0).all()[0]
+    assert (qc.data["dat"] == 0).all()
 
 
 # GL-333
 def test_resampleSingleEmptySeries():
     qc = saqc.SaQC(pd.DataFrame(1, columns=["a"], index=pd.DatetimeIndex([])))
     qc.resample("a", freq="1d")
```

### Comparing `saqc-2.3/tests/funcs/test_resampling.py` & `saqc-2.4.0/tests/funcs/test_resampling.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,148 +6,38 @@
 
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 import pytest
 
-import dios
-from saqc.constants import BAD, UNFLAGGED
-from saqc.core import SaQC, initFlagsLike
-from tests.common import checkDataFlagsInvariants
+from saqc import SaQC
+from saqc.core import DictOfSeries, initFlagsLike
+from tests.common import checkInvariants
 
 
 @pytest.fixture
 def data():
     index = pd.date_range(
         start="1.1.2011 00:00:00", end="1.1.2011 01:00:00", freq="15min"
     )
     index = index.insert(2, pd.Timestamp(2011, 1, 1, 0, 29, 0))
     index = index.insert(2, pd.Timestamp(2011, 1, 1, 0, 28, 0))
     index = index.insert(5, pd.Timestamp(2011, 1, 1, 0, 32, 0))
     index = index.insert(5, pd.Timestamp(2011, 1, 1, 0, 31, 0))
     index = index.insert(0, pd.Timestamp(2010, 12, 31, 23, 57, 0))
     index = index.drop(pd.Timestamp("2011-01-01 00:30:00"))
-    dat = pd.Series(np.linspace(-50, 50, index.size), index=index, name="data")
+    dat = pd.Series(np.linspace(-50, 50, index.size), index=index)
     # good to have some nan
     dat[-3] = np.nan
-    data = dios.DictOfSeries(dat)
+    data = DictOfSeries(data=dat)
     return data
 
 
-@pytest.mark.parametrize(
-    "func, kws",
-    [
-        ("linear", dict()),
-        ("shift", dict(method="nshift")),
-        ("interpolate", dict(method="spline")),
-        ("resample", dict(func=np.nansum, method="nagg")),
-    ],
-)
-def test_wrapper(data, func, kws):
-    field = "data"
-    freq = "15T"
-    flags = initFlagsLike(data)
-
-    # GL-#352
-    # make a History, otherwise nothing important is tested
-    for c in flags.columns:
-        flags[:, c] = BAD
-
-    qc = SaQC(data, flags)
-
-    qc = getattr(qc, func)(field, freq, **kws)
-
-    # check minimal requirements
-    checkDataFlagsInvariants(qc._data, qc._flags, field)
-    assert qc.data[field].index.inferred_freq == freq
-
-
-_SUPPORTED_METHODS = [
-    "linear",
-    "time",
-    "nearest",
-    "zero",
-    "slinear",
-    "quadratic",
-    "cubic",
-    "spline",
-    "barycentric",
-    "polynomial",
-    "krogh",
-    "piecewise_polynomial",
-    "spline",
-    "pchip",
-    "akima",
-]
-
-
-@pytest.mark.parametrize("method", _SUPPORTED_METHODS)
-@pytest.mark.parametrize("fill_history", ["some", "all", "none"])
-def test_gridInterpolation(data, method, fill_history):
-    freq = "15T"
-    field = "data"
-    data = data[field]
-    data = pd.concat([data * np.sin(data), data.shift(1, "2h")]).shift(1, "3s")
-    data = dios.DictOfSeries(data)
-    flags = initFlagsLike(data)
-
-    if fill_history == "none":
-        pass
-
-    if fill_history == "all":
-        for c in flags.columns:
-            flags[:, c] = BAD
-
-    if fill_history == "some":
-        for c in flags.columns:
-            flags[::2, c] = UNFLAGGED
-
-    qc = SaQC(data, flags)
-
-    # we are just testing if the interpolation gets passed to the series without
-    # causing an error:
-    res = qc.interpolate(
-        field,
-        freq,
-        method=method,
-        downcast_interpolation=True,
-    )
-
-    if method == "polynomial":
-        res = qc.interpolate(
-            field,
-            freq,
-            order=2,
-            method=method,
-            downcast_interpolation=True,
-        )
-        res = qc.interpolate(
-            field,
-            freq,
-            order=9,
-            method=method,
-            downcast_interpolation=True,
-        )
-
-    # check minimal requirements
-    checkDataFlagsInvariants(res._data, res._flags, field, identical=False)
-    assert res.data[field].index.inferred_freq == freq
-
-
-@pytest.mark.parametrize(
-    "func, kws",
-    [
-        ("linear", dict()),
-        ("shift", dict(method="nshift")),
-        ("interpolate", dict(method="spline")),
-        ("aggregate", dict(value_func=np.nansum, method="nagg")),
-    ],
-)
-def test_flagsSurviveReshaping(func, kws):
+def test_flagsSurviveReshaping():
     """
     flagging -> reshaping -> test (flags also was reshaped correctly)
     """
     pass
 
 
 def test_flagsSurviveInverseReshaping():
@@ -160,270 +50,345 @@
     """
     flagging -> reshaping -> inverse reshaping -> test (flags == original-flags)
     """
     pass
 
 
 @pytest.mark.parametrize(
-    "reshaper", ["nshift", "fshift", "bshift", "nagg", "bagg", "fagg", "interpolation"]
-)
-def test_harmSingleVarIntermediateFlagging(data, reshaper):
-    flags = initFlagsLike(data)
-    field = "data"
-    freq = "15T"
-
-    pre_data = data.copy()
-    pre_flags = flags.copy()
-    qc = SaQC(data, flags)
-
-    qc = qc.copyField(field, field + "_interpolated")
-    qc = qc.linear(field + "_interpolated", freq=freq)
-    checkDataFlagsInvariants(
-        qc._data, qc._flags, field + "_interpolated", identical=True
-    )
-    assert qc._data[field + "_interpolated"].index.inferred_freq == freq
-
-    # flag something bad
-    qc._flags[
-        qc._data[field + "_interpolated"].index[3:4], field + "_interpolated"
-    ] = BAD
-    qc = qc.concatFlags(
-        field + "_interpolated", method="inverse_" + reshaper, target=field
-    )
-    qc = qc.dropField(field + "_interpolated")
-
-    assert len(qc.data[field]) == len(qc.flags[field])
-    assert qc.data[field].equals(pre_data[field])
-    assert qc.flags[field].index.equals(pre_flags[field].index)
-
-    if "agg" in reshaper:
-        if reshaper == "nagg":
-            start, end = 3, 7
-        elif reshaper == "fagg":
-            start, end = 3, 5
-        elif reshaper == "bagg":
-            start, end = 5, 7
-        else:
-            raise NotImplementedError("untested test case")
-
-        assert all(qc._flags[field].iloc[start:end] > UNFLAGGED)
-        assert all(qc._flags[field].iloc[:start] == UNFLAGGED)
-        assert all(qc._flags[field].iloc[end:] == UNFLAGGED)
-
-    elif "shift" in reshaper:
-        if reshaper == "nshift":
-            exp = [False, False, False, False, True, False, False, False, False]
-        elif reshaper == "fshift":
-            exp = [False, False, False, False, True, False, False, False, False]
-        elif reshaper == "bshift":
-            exp = [False, False, False, False, False, True, False, False, False]
-        else:
-            raise NotImplementedError("untested test case")
-
-        flagged = qc._flags[field] > UNFLAGGED
-        assert all(flagged == exp)
-
-    elif reshaper == "interpolation":
-        pytest.skip("no testcase for interpolation")
-
-    else:
-        raise NotImplementedError("untested test case")
-
-
-@pytest.mark.parametrize(
-    "params, expected",
+    "method, freq, expected",
     [
         (
-            ("nagg", "15Min"),
+            "nagg",
+            "15Min",
             pd.Series(
                 data=[-87.5, -25.0, 0.0, 37.5, 50.0],
                 index=pd.date_range(
                     "2011-01-01 00:00:00", "2011-01-01 01:00:00", freq="15min"
                 ),
             ),
         ),
         (
-            ("nagg", "30Min"),
+            "nagg",
+            "30Min",
             pd.Series(
                 data=[-87.5, -25.0, 87.5],
                 index=pd.date_range(
                     "2011-01-01 00:00:00", "2011-01-01 01:00:00", freq="30min"
                 ),
             ),
         ),
         (
-            ("bagg", "15Min"),
+            "bagg",
+            "15Min",
             pd.Series(
                 data=[-50.0, -37.5, -37.5, 12.5, 37.5, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:45:00", "2011-01-01 01:00:00", freq="15min"
                 ),
             ),
         ),
         (
-            ("bagg", "30Min"),
+            "bagg",
+            "30Min",
             pd.Series(
                 data=[-50.0, -75.0, 50.0, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:30:00", "2011-01-01 01:00:00", freq="30min"
                 ),
             ),
         ),
     ],
 )
-def test_harmSingleVarInterpolationAgg(data, params, expected):
+def test_resampleAggregateInvert(data, method, freq, expected):
     flags = initFlagsLike(data)
     field = "data"
-    h_field = "data_harm"
+    field_aggregated = "data_aggregated"
 
     pre_data = data.copy()
     pre_flaggger = flags.copy()
-    method, freq = params
 
     qc = SaQC(data, flags)
 
-    qc = qc.copyField("data", "data_harm")
-    qc = qc.resample(h_field, freq, func=np.sum, method=method)
+    qc = qc.copyField(field, field_aggregated)
+
+    qc = qc.resample(field_aggregated, freq, func=np.sum, method=method)
+    assert qc._data[field_aggregated].index.freq == pd.Timedelta(freq)
+    assert qc._data[field_aggregated].equals(expected)
+    assert qc._flags.history[field_aggregated].meta[-1]["func"] == "resample"
+    checkInvariants(qc._data, qc._flags, field_aggregated, identical=True)
 
-    checkDataFlagsInvariants(qc._data, qc._flags, h_field, identical=True)
-    assert qc._data[h_field].index.freq == pd.Timedelta(freq)
-    assert qc._data[h_field].equals(expected)
-
-    qc = qc.concatFlags(h_field, target=field, method="inverse_" + method)
-    qc = qc.dropField(h_field)
-    checkDataFlagsInvariants(qc._data, qc._flags, field, identical=True)
+    qc = qc.concatFlags(field_aggregated, target=field, method="inverse_" + method)
     assert qc.data[field].equals(pre_data[field])
     assert qc.flags[field].equals(pre_flaggger[field])
+    checkInvariants(qc._data, qc._flags, field, identical=True)
+
+
+@pytest.mark.parametrize(
+    "method, freq, expected",
+    [
+        (
+            "linear",
+            "15Min",
+            pd.Series(
+                data=[np.nan, -37.5, -25, 6.25, 37.50, 50],
+                index=pd.date_range(
+                    "2010-12-31 23:45:00", "2011-01-01 01:00:00", freq="15Min"
+                ),
+            ),
+        ),
+        (
+            "time",
+            "30Min",
+            pd.Series(
+                data=[np.nan, -37.5, 6.25, 50.0],
+                index=pd.date_range(
+                    "2010-12-31 23:30:00", "2011-01-01 01:00:00", freq="30Min"
+                ),
+            ),
+        ),
+        (
+            "pad",
+            "30Min",
+            pd.Series(
+                data=[np.nan, -37.5, 0, 50.0],
+                index=pd.date_range(
+                    "2010-12-31 23:30:00", "2011-01-01 01:00:00", freq="30Min"
+                ),
+            ),
+        ),
+    ],
+)
+def test_alignInterpolateInvert(data, method, freq, expected):
+    flags = initFlagsLike(data)
+
+    field = "data"
+    field_aligned = "data_aligned"
+
+    pre_data = data.copy()
+    pre_flags = flags.copy()
+
+    qc = SaQC(data, flags)
+
+    qc = qc.copyField(field, field_aligned)
+    qc = qc.align(field_aligned, freq, method=method)
+
+    assert qc.data[field_aligned].equals(expected)
+    checkInvariants(qc._data, qc._flags, field, identical=True)
+
+    qc = qc.concatFlags(field_aligned, target=field, method="inverse_interpolation")
+    assert qc.data[field].equals(pre_data[field])
+    assert qc.flags[field].equals(pre_flags[field])
+    checkInvariants(qc._data, qc._flags, field, identical=True)
 
 
 @pytest.mark.parametrize(
-    "params, expected",
+    "method, freq, expected",
     [
         (
-            ("bshift", "15Min"),
+            "bshift",
+            "15Min",
             pd.Series(
                 data=[-50.0, -37.5, -25.0, 12.5, 37.5, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:45:00", "2011-01-01 01:00:00", freq="15Min"
                 ),
             ),
         ),
         (
-            ("fshift", "15Min"),
+            "fshift",
+            "15Min",
             pd.Series(
                 data=[np.nan, -37.5, -25.0, 0.0, 37.5, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:45:00", "2011-01-01 01:00:00", freq="15Min"
                 ),
             ),
         ),
         (
-            ("nshift", "15min"),
+            "nshift",
+            "15min",
             pd.Series(
                 data=[np.nan, -37.5, -25.0, 12.5, 37.5, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:45:00", "2011-01-01 01:00:00", freq="15Min"
                 ),
             ),
         ),
         (
-            ("bshift", "30Min"),
+            "bshift",
+            "30Min",
             pd.Series(
                 data=[-50.0, -37.5, 12.5, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:30:00", "2011-01-01 01:00:00", freq="30Min"
                 ),
             ),
         ),
         (
-            ("fshift", "30Min"),
+            "fshift",
+            "30Min",
             pd.Series(
                 data=[np.nan, -37.5, 0.0, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:30:00", "2011-01-01 01:00:00", freq="30Min"
                 ),
             ),
         ),
         (
-            ("nshift", "30min"),
+            "nshift",
+            "30min",
             pd.Series(
                 data=[np.nan, -37.5, 12.5, 50.0],
                 index=pd.date_range(
                     "2010-12-31 23:30:00", "2011-01-01 01:00:00", freq="30Min"
                 ),
             ),
         ),
     ],
 )
-def test_harmSingleVarInterpolationShift(data, params, expected):
+def test_alignShiftInvert(data, method, freq, expected):
     flags = initFlagsLike(data)
+
     field = "data"
-    h_field = "data_harm"
+    field_aligned = "data_aligned"
+
     pre_data = data.copy()
     pre_flags = flags.copy()
-    method, freq = params
 
     qc = SaQC(data, flags)
 
-    qc = qc.copyField("data", "data_harm")
-    qc = qc.shift(h_field, freq, method=method)
-    assert qc.data[h_field].equals(expected)
-    checkDataFlagsInvariants(qc._data, qc._flags, field, identical=True)
-
-    qc = qc.concatFlags(h_field, target=field, method="inverse_" + method)
-    checkDataFlagsInvariants(qc._data, qc._flags, field, identical=True)
+    qc = qc.copyField(field, field_aligned)
+    qc = qc.align(field_aligned, freq, method=method)
+    meta = qc._flags.history[field_aligned].meta[-1]
+
+    assert qc.data[field_aligned].equals(expected)
+    assert (meta["func"], meta["kwargs"]["method"]) == ("align", method)
+    checkInvariants(qc._data, qc._flags, field, identical=True)
 
-    qc = qc.dropField(h_field)
+    qc = qc.concatFlags(field_aligned, target=field, method="inverse_" + method)
     assert qc.data[field].equals(pre_data[field])
     assert qc.flags[field].equals(pre_flags[field])
+    checkInvariants(qc._data, qc._flags, field, identical=True)
 
 
-def test_concatFlags():
-    index = pd.to_datetime(
-        [
-            "2020-01-01 00:00",
-            "2020-01-01 00:10",
-            "2020-01-01 00:30",
-            "2020-01-01 00:40",
-            "2020-01-01 01:00",
-        ]
+@pytest.mark.parametrize(
+    "overwrite, expected_col0, expected_col1",
+    [
+        (
+            True,
+            [np.nan, np.nan, np.nan, np.nan, np.nan, np.nan, np.nan, 255, 255],
+            [np.nan, np.nan, np.nan, np.nan, np.nan, 255, np.nan, 255, 255],
+        ),
+        (
+            False,
+            [np.nan, np.nan, np.nan, np.nan, np.nan, np.nan, np.nan, 255, 255],
+            [np.nan, np.nan, np.nan, np.nan, np.nan, 255, np.nan, np.nan, np.nan],
+        ),
+    ],
+)
+def test_concatFlags(data, overwrite, expected_col0, expected_col1):
+    qc = SaQC(data)
+
+    qc = qc.flagRange(field="data", max=20)
+
+    # branch out to another variable
+    qc = qc.flagRange(field="data", target="data_", max=3)
+
+    # bring the flags back again - overwrite
+    qc_concat = qc.concatFlags(
+        "data_", target="data", overwrite=overwrite, squeeze=True
     )
+    hist_concat = qc_concat._flags.history["data"].hist.astype(float)
+    meta_concat = qc_concat._flags.history["data"].meta
+    assert hist_concat[0].equals(pd.Series(expected_col0, index=data["data"].index))
+    assert hist_concat[1].equals(pd.Series(expected_col1, index=data["data"].index))
+    assert meta_concat[-1]["func"] == "concatFlags"
+
+
+@pytest.mark.parametrize(
+    "method, inversion_method, freq",
+    [
+        ("linear", "inverse_interpolation", "15min"),
+        ("bshift", "inverse_bshift", "15Min"),
+        ("fshift", "inverse_fshift", "15Min"),
+        ("nshift", "inverse_nshift", "15min"),
+        ("pad", "inverse_interpolation", "15min"),
+    ],
+)
+def test_alignAutoInvert(data, method, inversion_method, freq):
+    flags = initFlagsLike(data)
+    field = data.columns[0]
+    field_aligned = f"{field}_aligned"
 
-    df = pd.DataFrame(
-        data={
-            "a": [
-                1,
-                2,
-                5,
-                4,
-                3,
-            ]
-        },
-        index=index,
+    qc = SaQC(data, flags)
+    qc = qc.align(field=field, target=field_aligned, method=method, freq=freq)
+    qc = qc.flagDummy(field=field_aligned)
+    qc_expected = qc.concatFlags(
+        field=field_aligned, target=field, method=inversion_method
     )
+    qc_got = qc.concatFlags(field=field_aligned, target=field, method="auto")
 
-    qc = SaQC(df)
+    _assertEqual(qc_expected, qc_got)
 
-    qc = qc.flagRange(field="a", max=4)
 
-    # branch out to another variable
-    qc = qc.flagRange(field="a", target="b", max=3)
+def test_alignMultiAutoInvert(data):
+    flags = initFlagsLike(data)
+    field = data.columns[0]
+    field_aligned = f"{field}_aligned"
 
-    # bring the flags back again
-    qc_overwrite = qc.concatFlags("b", target="a", overwrite=True, squeeze=True)
-    hist_overwrite = qc_overwrite._flags.history["a"].hist.astype(float)
-    assert hist_overwrite[0].equals(
-        pd.Series([np.nan, np.nan, 255.0, np.nan, np.nan], index=index)
+    qc = SaQC(data, flags)
+    qc = qc.align(field=field, target=field_aligned, method="fshift", freq="30Min")
+    qc = qc.align(field=field_aligned, method="time", freq="10Min")
+    qc = qc.flagDummy(field=field_aligned)
+
+    # resolve the last alignment operation
+    _assertEqual(
+        qc.concatFlags(field=field_aligned, target=field, method="auto"),
+        qc.concatFlags(
+            field=field_aligned, target=field, method="inverse_interpolation"
+        ),
     )
-    assert hist_overwrite[1].equals(
-        pd.Series([np.nan, np.nan, 255.0, 255.0, np.nan], index=index)
+    # resolve the first alignment operation
+    _assertEqual(
+        (
+            qc.concatFlags(field=field_aligned, method="auto").concatFlags(
+                field=field_aligned, target=field, method="auto"
+            )
+        ),
+        (
+            qc.concatFlags(
+                field=field_aligned, method="inverse_interpolation"
+            ).concatFlags(field=field_aligned, target=field, method="inverse_fshift")
+        ),
     )
 
-    # bring the flags back again
-    qc_respect = qc.concatFlags("b", target="a", overwrite=False, squeeze=True)
-    hist_respect = qc_respect._flags.history["a"].hist.astype(float)
-    assert hist_respect[0].equals(
-        pd.Series([np.nan, np.nan, 255.0, np.nan, np.nan], index=index)
-    )
-    assert hist_respect[1].equals(
-        pd.Series([np.nan, np.nan, np.nan, 255.0, np.nan], index=index)
+
+def _assertEqual(left: SaQC, right: SaQC):
+    for field in left.data.columns:
+        assert left._data[field].equals(right._data[field])
+        assert left._flags[field].equals(right._flags[field])
+        assert left._flags.history[field].hist.equals(right._flags.history[field].hist)
+        assert left._flags.history[field].meta == right._flags.history[field].meta
+
+
+@pytest.mark.parametrize(
+    "method, inversion_method, freq",
+    [
+        ("bagg", "inverse_bagg", "15Min"),
+        ("fagg", "inverse_fagg", "15Min"),
+        ("nagg", "inverse_nagg", "15min"),
+    ],
+)
+def test_resampleAutoInvert(data, method, inversion_method, freq):
+    flags = initFlagsLike(data)
+    field = data.columns[0]
+    field_aligned = f"{field}_aligned"
+
+    qc = SaQC(data, flags)
+    qc = qc.resample(field=field, target=field_aligned, method=method, freq=freq)
+    qc = qc.flagRange(field=field_aligned, min=0, max=100)
+    qc_expected = qc.concatFlags(
+        field=field_aligned, target=field, method=inversion_method
     )
+    qc_got = qc.concatFlags(field=field_aligned, target=field, method="auto")
+
+    _assertEqual(qc_got, qc_expected)
```

### Comparing `saqc-2.3/tests/fuzzy/lib.py` & `saqc-2.4.0/tests/fuzzy/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,16 @@
     integers,
     lists,
     register_type_strategy,
     sampled_from,
 )
 from hypothesis.strategies._internal.types import _global_type_lookup
 
-import dios
-from saqc.constants import BAD
-from saqc.core import initFlagsLike
+from saqc import BAD
+from saqc.core import DictOfSeries, initFlagsLike
 from saqc.core.register import FUNC_MAP
 
 MAX_EXAMPLES = 50
 # MAX_EXAMPLES = 100000
 
 
 @composite
@@ -42,15 +41,15 @@
     # - Column names need to satisify the following regex: [A-Za-z0-9_-]+
     # - DatetimeIndex needs to be sorted
     # - Integer values larger than 2**53 lead to numerical instabilities during
     #   the integer->float->integer type conversion in _maskData/_unmaskData.
 
     cols = draw(lists(columnNames(), unique=True, min_size=min_cols))
     columns = {c: draw(dataSeries(min_size=3)) for c in cols}
-    return dios.DictOfSeries(columns)
+    return DictOfSeries(columns)
 
 
 @composite
 def dataSeries(
     draw, min_size=0, max_size=100, dtypes=("float32", "float64", "int32", "int64")
 ):
     if np.isscalar(dtypes):
@@ -130,15 +129,14 @@
     func = draw(functions(module))
     kwargs = draw(functionKwargs(func))
     return func, kwargs
 
 
 @contextmanager
 def applyStrategies(strategies: dict):
-
     for dtype, strategy in strategies.items():
         register_type_strategy(dtype, strategy)
 
     yield
 
     for dtype in strategies.keys():
         del _global_type_lookup[dtype]
@@ -150,19 +148,19 @@
     field = draw(sampled_from(sorted(data.columns)))
 
     kwargs = {"data": data, "field": field, "flags": draw(flagses(data))}
 
     i64 = np.iinfo("int64")
 
     strategies = {
-        FreqString: frequencyStrings,
-        ColumnName: lambda _: sampled_from(
-            sorted(c for c in data.columns if c != field)
-        ),
-        IntegerWindow: lambda _: integers(min_value=1, max_value=len(data[field]) - 1),
+        # FreqString: frequencyStrings,
+        # ColumnName: lambda _: sampled_from(
+        #     sorted(c for c in data.columns if c != field)
+        # ),
+        # IntegerWindow: lambda _: integers(min_value=1, max_value=len(data[field]) - 1),
         int: lambda _: integers(min_value=i64.min + 1, max_value=i64.max - 1),
     }
 
     with applyStrategies(strategies):
         for k, v in get_type_hints(func).items():
             if k not in {"data", "field", "flags", "return"}:
                 value = draw(from_type(v))
```

### Comparing `saqc-2.3/tests/fuzzy/test_masking.py` & `saqc-2.4.0/tests/fuzzy/test_masking.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,50 @@
 
 # -*- coding: utf-8 -*-
 
 import pandas as pd
 import pytest
 from hypothesis import given, settings
 
-from saqc.constants import BAD, UNFLAGGED
+from saqc import BAD, UNFLAGGED, DictOfSeries
 from saqc.core.register import _maskData, _unmaskData
 from tests.fuzzy.lib import MAX_EXAMPLES, dataFieldFlags
 
 
 @pytest.mark.slow
 @settings(max_examples=MAX_EXAMPLES, deadline=None)
 @given(data_field_flags=dataFieldFlags())
 def test_maskingMasksData(data_field_flags):
     """
     test if flagged values are replaced by np.nan
     """
     data_in, field, flags = data_field_flags
-    data_masked, mask = _maskData(
-        data_in, flags, columns=[field], thresh=UNFLAGGED
-    )  # thresh UNFLAGGED | np.inf
-    assert data_masked[field].iloc[mask[field].index].isna().all()
-    assert (flags[field].iloc[mask[field].index] > UNFLAGGED).all()
+    data_masked, mask = _maskData(data_in, flags, columns=[field], thresh=UNFLAGGED)
+    assert isinstance(data_masked, DictOfSeries)
+    assert isinstance(mask, DictOfSeries)
+    assert field in data_masked.columns
+    if field in mask.columns:
+        assert data_masked[field].iloc[mask[field].index].isna().all()
+        assert (flags[field].iloc[mask[field].index] > UNFLAGGED).all()
+    else:
+        # if nothing gets masked in a column,
+        # the column does not appear in mask
+        assert (flags[field] == UNFLAGGED).all()
 
 
 @pytest.mark.slow
 @settings(max_examples=MAX_EXAMPLES, deadline=None)
 @given(data_field_flags=dataFieldFlags())
 def test_dataMutationPreventsUnmasking(data_field_flags):
     """test if (un)masking works as expected on data-changes.
 
     if `data` is mutated after `_maskData`, `_unmaskData` should be a no-op
     """
-    filler = -9999
-
     data_in, field, flags = data_field_flags
+    filler = pd.Series(-9999.0, index=data_in[field].index, dtype=float)
 
     data_masked, mask = _maskData(data_in, flags, columns=[field], thresh=UNFLAGGED)
     data_masked[field] = filler
     data_out = _unmaskData(data_masked, mask)
     assert (data_out[field] == filler).all(axis=None)
 
 
@@ -57,15 +62,15 @@
     if `flags` is mutated after `_maskData`, `_unmaskData` should be a no-op
     """
     data_in, field, flags = data_field_flags
 
     data_masked, mask = _maskData(data_in, flags, columns=[field], thresh=UNFLAGGED)
     flags[:, field] = UNFLAGGED
     data_out = _unmaskData(data_masked, mask)
-    assert (data_out.loc[flags[field] == BAD, field].isna()).all(axis=None)
+    assert (data_out[field].loc[flags[field] == BAD].isna()).all(axis=None)
 
 
 @pytest.mark.slow
 @settings(max_examples=MAX_EXAMPLES, deadline=None)
 @given(data_field_flags=dataFieldFlags())
 def test_reshapingPreventsUnmasking(data_field_flags):
     """test if (un)masking works as expected on index-changes.
@@ -100,15 +105,15 @@
     unmasking data should invert the masking
     """
     data_in, field, flags = data_field_flags
 
     data_masked, mask = _maskData(data_in, flags, columns=[field], thresh=UNFLAGGED)
     data_out = _unmaskData(data_masked, mask)
     assert pd.DataFrame.equals(
-        data_out.to_df().astype(float), data_in.to_df().astype(float)
+        data_out.to_pandas().astype(float), data_in.to_pandas().astype(float)
     )
 
 
 # @settings(max_examples=MAX_EXAMPLES, deadline=None)
 # @given(data_field_flags=dataFieldFlags(), func_kwargs=flagFuncsKwargs())
 # def test_maskingPreservesData(data_field_flags, func_kwargs):
 #     """
```

### Comparing `saqc-2.3/tests/lib/test_periodicMask.py` & `saqc-2.4.0/tests/lib/test_periodicMask.py`

 * *Files identical despite different names*

