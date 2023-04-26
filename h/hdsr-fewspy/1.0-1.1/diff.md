# Comparing `tmp/hdsr_fewspy-1.0.tar.gz` & `tmp/hdsr_fewspy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.0.tar", last modified: Wed Apr 26 07:45:50 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.1.tar", last modified: Wed Apr 26 12:03:06 2023, max compression
```

## Comparing `hdsr_fewspy-1.0.tar` & `hdsr_fewspy-1.1.tar`

### file list

```diff
@@ -1,65 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0    13090 2023-04-26 07:45:52.000000 hdsr_fewspy-1.0/PKG-INFO
--rw-rw-rw-   0        0        0    12236 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/fewspy/
--rw-rw-rw-   0        0        0      139 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/__init__.py
--rw-rw-rw-   0        0        0    14387 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/fewspy/api_calls/
--rw-rw-rw-   0        0        0      938 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7524 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1262 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2905 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2554 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2791 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0     2170 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1285 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:12:22.000000 hdsr_fewspy-1.0/fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     8145 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     5371 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2218 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0      655 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:34:27.000000 hdsr_fewspy-1.0/fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      328 2023-04-18 12:12:22.000000 hdsr_fewspy-1.0/fewspy/constants/github.py
--rw-rw-rw-   0        0        0      573 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     4278 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      942 2023-04-18 12:12:22.000000 hdsr_fewspy-1.0/fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     6589 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6857 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1786 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0      384 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4332 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/permissions.py
--rw-rw-rw-   0        0        0     5865 2023-04-26 07:45:18.000000 hdsr_fewspy-1.0/fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3537 2023-04-18 12:12:22.000000 hdsr_fewspy-1.0/fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-02-15 20:21:06.000000 hdsr_fewspy-1.0/fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1368 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4248 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      703 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2947 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1333 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0    11668 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     6627 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3952 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      563 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/fewspy/utils/
--rw-rw-rw-   0        0        0        0 2023-02-15 20:21:06.000000 hdsr_fewspy-1.0/fewspy/utils/__init__.py
--rw-rw-rw-   0        0        0     3046 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/fewspy/utils/conversions.py
--rw-rw-rw-   0        0        0     4565 2023-04-18 12:12:22.000000 hdsr_fewspy-1.0/fewspy/utils/date_frequency.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:45:50.000000 hdsr_fewspy-1.0/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    13090 2023-04-26 07:45:49.000000 hdsr_fewspy-1.0/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1726 2023-04-26 07:45:49.000000 hdsr_fewspy-1.0/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 07:45:49.000000 hdsr_fewspy-1.0/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 07:41:14.000000 hdsr_fewspy-1.0/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-04-26 07:45:49.000000 hdsr_fewspy-1.0/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 07:45:49.000000 hdsr_fewspy-1.0/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      414 2023-04-26 07:45:52.000000 hdsr_fewspy-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1626 2023-04-26 07:45:19.000000 hdsr_fewspy-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    14179 2023-04-26 12:03:07.000000 hdsr_fewspy-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13318 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      149 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    14174 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7572 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2937 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2806 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0     2185 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1300 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     8173 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     5380 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2237 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0      670 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      546 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     6599 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3051 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      384 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4258 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      713 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0    11693 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     6652 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3967 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    14179 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-04-26 12:03:03.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-04-26 12:03:07.000000 hdsr_fewspy-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1672 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/setup.py
```

### Comparing `hdsr_fewspy-1.0/LICENSE.txt` & `hdsr_fewspy-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.0/PKG-INFO` & `hdsr_fewspy-1.1/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: hdsr_fewspy
-Version: 1.0
-Summary: An interface for interacting with hdsr github repos
-Home-page: https://github.com/hdsr-mid/hdsr_pygithub
+Name: hdsr-fewspy
+Version: 1.1
+Summary: A python project to get data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
+Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_pygithub/archive/v1.0.tar.gz
-Keywords: interface,interaction,github,files,hdsr
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.1.tar.gz
+Keywords: hdsr,fews,api
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -35,72 +35,76 @@
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
 two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds authentication, authorisation, and 
 throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
-Hdsr_fewspy API support 9 different API calls:
-1. get_parameters:
-2. get_filters:
-3. get_locations:
-4. get_qualifiers: 
-5. get_timezone_id: 
-6. get_samples: 
-7. get_time_series_single: 
-8. get_time_series_multi:
-9: get_time_series_statistics:
-
-An API call can return 6 different output formats:   
+Hdsr_fewspy API support 9 different API calls that can return 6 different output formats:   
 1. xml_file_in_download_dir: The xml response is written to a .xml file in your download_dir
 2. json_file_in_download_dir: The json response is written to a .json file in your download_dir
 3. csv_file_in_download_dir: The json response is converted to csv and written to a .csv file in your download_dir
 4. xml_response_in_memory: the xml response is returned memory meaning you get a list with one or more responses 
 5. json_response_in_memory: the json response is returned memory meaning you get a list with one or more responses        
 6. pandas_dataframe_in_memory: the json response is converted to a pandas dataframe meaning you get one dataframe 
 
-Each API call supports a subset of output formats:
+API call                      | Supported outputs  | Notes 
+------------------------------|--------------------|--------
+get_parameters                | 4, 5, 6            | Returns 1 object (xml/json response or dataframe) 
+get_filters                   | 4, 5               | Returns 1 object (xml/json response)  
+get_locations                 | 4, 5               | Returns 1 object (xml/json response)              
+get_qualifiers                | 4, 5               | Returns 1 object (xml/json response)
+get_timezone_id               | 4, 5               | Returns 1 object (xml/json response)
+get_samples                   | 1, 2               | Not implemented yet
+get_time_series_single        | 4, 5, 6            | Returns a 1 dataframe or a list with >=1 xml/json responses or     
+get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
+get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response) 
 
-API call| Supported outputs | Notes 
---------|-------------------|--------
-1       | 4, 5, 6           | Not implemented yet
-2       | 4, 5              | Not implemented yet  
-3       | 4, 5              | Not implemented yet              
-4       | 4, 5              | Not implemented yet
-5       | 4, 5              | Not implemented yet
-6       | 1, 2              | Not implemented yet
-7       | 4, 5, 6           | One large call can results in multiple small calls. Output 4 and 5 return a list with >=1 responses. Output 6 aggregates all responses and returns one dataframe.    
-8       | 1, 2, 3           | One unique location_parameter_qualifier combination results in >=1 API calls = >=1 responses. For output 1 and 2 each response results in 1 file. Output 3 creates 1 csv per unique combination.
-9       | 4, 5              | Not implemented yet 
+- One large call can result in multiple small calls. Output 4 and 5 return a list with >=1 responses. Output 6 aggregates all responses and returns one dataframe.
+- One unique location_parameter_qualifier combination results in >=1 API calls = >=1 responses. For output 1 and 2 each response results in 1 file. Output 3 creates 1 csv per unique combination.
 
 ### Usage
 
 ###### Preparation
 1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
 HDSR_FEWSPY_EMAIL=<your_hdsr_email>
 HDSR_FEWSPY_TOKEN=<contact renier.kramer.hdsr.nl to get HDSR_FEWSPY_TOKEN>
 ```
 2. Only once per project: install hdsr_fewspy dependency
 ```
-pip install hdsr_fewspy 
-or 
-conda install hdsr_fewspy -c hdsr-mid
+pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
 3. Run imports and instantiate hdsr_fewspy API 
 ```
+from hdsr_fewspy imoprt Api
+from hdsr_fewspy import PiSettings
+
 # instantiate API using default settings:
-api = Api()
+api = Api()  
 
 # or instantiate API using custom settings:
-custom_
-api 
-```
+custom_settings = PiSettings(
+   settings_name="blablabla",            
+   document_version=1.25",
+   ssl_verify=True,
+   domain="localhost",
+   port="8080",
+   service="FewsWebServices",
+   filter_id="INTERNAL-API",
+   module_instance_ids="WerkFilter",
+   time_zone=0.0,
+)
+api = Api(pi_settings=custom_settings)
 
+# or if you want download responses (xml, json, csv), then you need to specify a download_dir.
+# The files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/  
+api = Api(output_directory_root=<path_to_your_directory>)
+```
 
 ###### Examples different API calls
 1. Example get_time_series_single
 ```
 api = Api()
 
 responses = api.get_time_series_single(
@@ -153,52 +157,52 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (25 april 2023)
+### Test Coverage (26 april 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
-Name                                                         Stmts   Miss  Cover
---------------------------------------------------------------------------------
-fewspy\__init__.py                                               4      0   100%
-fewspy\api.py                                                   98     13    87%
-fewspy\api_calls\__init__.py                                    18      0   100%
-fewspy\api_calls\base.py                                       100     12    88%
-fewspy\api_calls\get_filters.py                                 25      0   100%
-fewspy\api_calls\get_locations.py                               44      2    95%
-fewspy\api_calls\get_parameters.py                              40      1    98%
-fewspy\api_calls\get_qualifiers.py                              36     12    67%
-fewspy\api_calls\get_samples.py                                 26      8    69%
-fewspy\api_calls\get_timezone_id.py                             26      1    96%
-fewspy\api_calls\time_series\base.py                            91      6    93%
-fewspy\api_calls\time_series\get_time_series_multi.py           67      5    93%
-fewspy\api_calls\time_series\get_time_series_single.py          28      1    96%
-fewspy\api_calls\time_series\get_time_series_statistics.py      12      0   100%
-fewspy\constants\choices.py                                     89      3    97%
-fewspy\constants\custom_types.py                                 2      0   100%
-fewspy\constants\github.py                                       7      0   100%
-fewspy\constants\paths.py                                       12      0   100%
-fewspy\constants\pi_settings.py                                 50      4    92%
-fewspy\constants\request_settings.py                            11      0   100%
-fewspy\converters\download.py                                   93      4    96%
-fewspy\converters\json_to_df_timeseries.py                     112      8    93%
-fewspy\converters\manager.py                                    27      0   100%
-fewspy\converters\xml_to_python_obj.py                         105     26    75%
-fewspy\exceptions.py                                            12      0   100%
-fewspy\permissions.py                                           67      5    93%
-fewspy\retry_session.py                                         68     12    82%
-fewspy\secrets.py                                               64     20    69%
-fewspy\utils\conversions.py                                     45     17    62%
-fewspy\utils\date_frequency.py                                  46      5    89%
-setup.py                                                        10     10     0%
---------------------------------------------------------------------------------
-TOTAL                                                         1435    175    88%
+Name                                                              Stmts   Miss  Cover
+-------------------------------------------------------------------------------------
+hdsr_fewspy\__init__.py                                               4      0   100%
+hdsr_fewspy\api.py                                                   98     13    87%
+hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
+hdsr_fewspy\api_calls\base.py                                       100     12    88%
+hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
+hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
+hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
+hdsr_fewspy\api_calls\get_qualifiers.py                              36     12    67%
+hdsr_fewspy\api_calls\get_samples.py                                 26      8    69%
+hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
+hdsr_fewspy\api_calls\time_series\base.py                            91      6    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           67      5    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_single.py          28      1    96%
+hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      12      0   100%
+hdsr_fewspy\constants\choices.py                                     89      3    97%
+hdsr_fewspy\constants\custom_types.py                                 2      0   100%
+hdsr_fewspy\constants\github.py                                       8      0   100%
+hdsr_fewspy\constants\paths.py                                       11      0   100%
+hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
+hdsr_fewspy\constants\request_settings.py                            11      0   100%
+hdsr_fewspy\converters\download.py                                   93      4    96%
+hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
+hdsr_fewspy\converters\manager.py                                    27      0   100%
+hdsr_fewspy\converters\utils.py                                      45     17    62%
+hdsr_fewspy\converters\xml_to_python_obj.py                         105     26    75%
+hdsr_fewspy\date_frequency.py                                        46      5    89%
+hdsr_fewspy\exceptions.py                                            12      0   100%
+hdsr_fewspy\permissions.py                                           67      5    93%
+hdsr_fewspy\retry_session.py                                         68     12    82%
+hdsr_fewspy\secrets.py                                               64     20    69%
+setup.py                                                             10     10     0%
+-------------------------------------------------------------------------------------
+TOTAL                                                              1458    178    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.0/README.md` & `hdsr_fewspy-1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: hdsr_fewspy
+Version: 1.1
+Summary: A python project to get data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
+Home-page: https://github.com/hdsr-mid/hdsr_fewspy
+Author: Renier Kramer
+Author-email: renier.kramer@hdsr.nl
+License: MIT
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.1.tar.gz
+Keywords: hdsr,fews,api
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE.txt
+
 ### Context
 * Created: February 2023
 * Author: Renier Kramer, renier.kramer@hdsr.nl
 * Python version: >3.7
 
 [hkvfewspy]: https://github.com/HKV-products-services/hkvfewspy
 [fewspy]: https://github.com/d2hydro/fewspy
@@ -13,72 +35,76 @@
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
 two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds authentication, authorisation, and 
 throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
-Hdsr_fewspy API support 9 different API calls:
-1. get_parameters:
-2. get_filters:
-3. get_locations:
-4. get_qualifiers: 
-5. get_timezone_id: 
-6. get_samples: 
-7. get_time_series_single: 
-8. get_time_series_multi:
-9: get_time_series_statistics:
-
-An API call can return 6 different output formats:   
+Hdsr_fewspy API support 9 different API calls that can return 6 different output formats:   
 1. xml_file_in_download_dir: The xml response is written to a .xml file in your download_dir
 2. json_file_in_download_dir: The json response is written to a .json file in your download_dir
 3. csv_file_in_download_dir: The json response is converted to csv and written to a .csv file in your download_dir
 4. xml_response_in_memory: the xml response is returned memory meaning you get a list with one or more responses 
 5. json_response_in_memory: the json response is returned memory meaning you get a list with one or more responses        
 6. pandas_dataframe_in_memory: the json response is converted to a pandas dataframe meaning you get one dataframe 
 
-Each API call supports a subset of output formats:
+API call                      | Supported outputs  | Notes 
+------------------------------|--------------------|--------
+get_parameters                | 4, 5, 6            | Returns 1 object (xml/json response or dataframe) 
+get_filters                   | 4, 5               | Returns 1 object (xml/json response)  
+get_locations                 | 4, 5               | Returns 1 object (xml/json response)              
+get_qualifiers                | 4, 5               | Returns 1 object (xml/json response)
+get_timezone_id               | 4, 5               | Returns 1 object (xml/json response)
+get_samples                   | 1, 2               | Not implemented yet
+get_time_series_single        | 4, 5, 6            | Returns a 1 dataframe or a list with >=1 xml/json responses or     
+get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
+get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response) 
 
-API call| Supported outputs | Notes 
---------|-------------------|--------
-1       | 4, 5, 6           | Not implemented yet
-2       | 4, 5              | Not implemented yet  
-3       | 4, 5              | Not implemented yet              
-4       | 4, 5              | Not implemented yet
-5       | 4, 5              | Not implemented yet
-6       | 1, 2              | Not implemented yet
-7       | 4, 5, 6           | One large call can results in multiple small calls. Output 4 and 5 return a list with >=1 responses. Output 6 aggregates all responses and returns one dataframe.    
-8       | 1, 2, 3           | One unique location_parameter_qualifier combination results in >=1 API calls = >=1 responses. For output 1 and 2 each response results in 1 file. Output 3 creates 1 csv per unique combination.
-9       | 4, 5              | Not implemented yet 
+- One large call can result in multiple small calls. Output 4 and 5 return a list with >=1 responses. Output 6 aggregates all responses and returns one dataframe.
+- One unique location_parameter_qualifier combination results in >=1 API calls = >=1 responses. For output 1 and 2 each response results in 1 file. Output 3 creates 1 csv per unique combination.
 
 ### Usage
 
 ###### Preparation
 1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
 HDSR_FEWSPY_EMAIL=<your_hdsr_email>
 HDSR_FEWSPY_TOKEN=<contact renier.kramer.hdsr.nl to get HDSR_FEWSPY_TOKEN>
 ```
 2. Only once per project: install hdsr_fewspy dependency
 ```
-pip install hdsr_fewspy 
-or 
-conda install hdsr_fewspy -c hdsr-mid
+pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
 3. Run imports and instantiate hdsr_fewspy API 
 ```
+from hdsr_fewspy imoprt Api
+from hdsr_fewspy import PiSettings
+
 # instantiate API using default settings:
-api = Api()
+api = Api()  
 
 # or instantiate API using custom settings:
-custom_
-api 
-```
+custom_settings = PiSettings(
+   settings_name="blablabla",            
+   document_version=1.25",
+   ssl_verify=True,
+   domain="localhost",
+   port="8080",
+   service="FewsWebServices",
+   filter_id="INTERNAL-API",
+   module_instance_ids="WerkFilter",
+   time_zone=0.0,
+)
+api = Api(pi_settings=custom_settings)
 
+# or if you want download responses (xml, json, csv), then you need to specify a download_dir.
+# The files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/  
+api = Api(output_directory_root=<path_to_your_directory>)
+```
 
 ###### Examples different API calls
 1. Example get_time_series_single
 ```
 api = Api()
 
 responses = api.get_time_series_single(
@@ -131,52 +157,52 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (25 april 2023)
+### Test Coverage (26 april 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
-Name                                                         Stmts   Miss  Cover
---------------------------------------------------------------------------------
-fewspy\__init__.py                                               4      0   100%
-fewspy\api.py                                                   98     13    87%
-fewspy\api_calls\__init__.py                                    18      0   100%
-fewspy\api_calls\base.py                                       100     12    88%
-fewspy\api_calls\get_filters.py                                 25      0   100%
-fewspy\api_calls\get_locations.py                               44      2    95%
-fewspy\api_calls\get_parameters.py                              40      1    98%
-fewspy\api_calls\get_qualifiers.py                              36     12    67%
-fewspy\api_calls\get_samples.py                                 26      8    69%
-fewspy\api_calls\get_timezone_id.py                             26      1    96%
-fewspy\api_calls\time_series\base.py                            91      6    93%
-fewspy\api_calls\time_series\get_time_series_multi.py           67      5    93%
-fewspy\api_calls\time_series\get_time_series_single.py          28      1    96%
-fewspy\api_calls\time_series\get_time_series_statistics.py      12      0   100%
-fewspy\constants\choices.py                                     89      3    97%
-fewspy\constants\custom_types.py                                 2      0   100%
-fewspy\constants\github.py                                       7      0   100%
-fewspy\constants\paths.py                                       12      0   100%
-fewspy\constants\pi_settings.py                                 50      4    92%
-fewspy\constants\request_settings.py                            11      0   100%
-fewspy\converters\download.py                                   93      4    96%
-fewspy\converters\json_to_df_timeseries.py                     112      8    93%
-fewspy\converters\manager.py                                    27      0   100%
-fewspy\converters\xml_to_python_obj.py                         105     26    75%
-fewspy\exceptions.py                                            12      0   100%
-fewspy\permissions.py                                           67      5    93%
-fewspy\retry_session.py                                         68     12    82%
-fewspy\secrets.py                                               64     20    69%
-fewspy\utils\conversions.py                                     45     17    62%
-fewspy\utils\date_frequency.py                                  46      5    89%
-setup.py                                                        10     10     0%
---------------------------------------------------------------------------------
-TOTAL                                                         1435    175    88%
+Name                                                              Stmts   Miss  Cover
+-------------------------------------------------------------------------------------
+hdsr_fewspy\__init__.py                                               4      0   100%
+hdsr_fewspy\api.py                                                   98     13    87%
+hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
+hdsr_fewspy\api_calls\base.py                                       100     12    88%
+hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
+hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
+hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
+hdsr_fewspy\api_calls\get_qualifiers.py                              36     12    67%
+hdsr_fewspy\api_calls\get_samples.py                                 26      8    69%
+hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
+hdsr_fewspy\api_calls\time_series\base.py                            91      6    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           67      5    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_single.py          28      1    96%
+hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      12      0   100%
+hdsr_fewspy\constants\choices.py                                     89      3    97%
+hdsr_fewspy\constants\custom_types.py                                 2      0   100%
+hdsr_fewspy\constants\github.py                                       8      0   100%
+hdsr_fewspy\constants\paths.py                                       11      0   100%
+hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
+hdsr_fewspy\constants\request_settings.py                            11      0   100%
+hdsr_fewspy\converters\download.py                                   93      4    96%
+hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
+hdsr_fewspy\converters\manager.py                                    27      0   100%
+hdsr_fewspy\converters\utils.py                                      45     17    62%
+hdsr_fewspy\converters\xml_to_python_obj.py                         105     26    75%
+hdsr_fewspy\date_frequency.py                                        46      5    89%
+hdsr_fewspy\exceptions.py                                            12      0   100%
+hdsr_fewspy\permissions.py                                           67      5    93%
+hdsr_fewspy\retry_session.py                                         68     12    82%
+hdsr_fewspy\secrets.py                                               64     20    69%
+setup.py                                                             10     10     0%
+-------------------------------------------------------------------------------------
+TOTAL                                                              1458    178    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
@@ -250,7 +276,9 @@
   - pip:
     - <a pip package>==<version>
 ```
 You can also write a requirements.txt file:
 ```
 > pip list --format=freeze > <path_to_project>/requirements.txt
 ```
+
+
```

### Comparing `hdsr_fewspy-1.0/fewspy/api.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from datetime import datetime
-from fewspy import api_calls
-from fewspy import exceptions
-from fewspy.constants.choices import TimeZoneChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.constants.pi_settings import pi_settings_production
-from fewspy.constants.pi_settings import PiSettings
-from fewspy.constants.request_settings import default_request_settings
-from fewspy.constants.request_settings import RequestSettings
-from fewspy.permissions import Permissions
-from fewspy.retry_session import RetryBackoffSession
+from hdsr_fewspy import api_calls
+from hdsr_fewspy import exceptions
+from hdsr_fewspy.constants.choices import TimeZoneChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.constants.pi_settings import pi_settings_production
+from hdsr_fewspy.constants.pi_settings import PiSettings
+from hdsr_fewspy.constants.request_settings import default_request_settings
+from hdsr_fewspy.constants.request_settings import RequestSettings
+from hdsr_fewspy.permissions import Permissions
+from hdsr_fewspy.retry_session import RetryBackoffSession
 from pathlib import Path
 from typing import List
 from typing import Optional
 from typing import Union
 
 import geopandas as gpd
 import logging
@@ -169,40 +169,42 @@
         location_id: str,
         parameter_id: str,
         qualifier_id: str = None,
         thinning: int = None,
         omit_empty_timeseries: bool = True,
     ) -> ResponseType:
         """
-        Example response PI_JSON =
-            {'timeSeries': [{'header': {'endDate': {'date': '2012-01-02',
-                                            'time': '00:00:00'},
-                                'firstValueTime': {'date': '2012-01-01',
-                                                   'time': '00:15:00'},
-                                'lastValueTime': {'date': '2012-01-02',
-                                                  'time': '00:00:00'},
-                                'lat': '52.08992726570302',
-                                'locationId': 'OW433001',
-                                'lon': '4.9547458967486095',
-                                'maxValue': '-0.28',
-                                'minValue': '-0.44',
-                                'missVal': '-999.0',
-                                'moduleInstanceId': 'WerkFilter',
-                                'parameterId': 'H.G.0',
-                                'startDate': {'date': '2012-01-01',
-                                              'time': '00:00:00'},
-                                'stationName': 'HAANWIJKERSLUIS_4330-w_Leidsche '
-                                               'Rijn',
-                                'timeStep': {'unit': 'nonequidistant'},
-                                'type': 'instantaneous',
-                                'units': 'mNAP',
-                                'valueCount': '102',
-                                'x': '125362.0',
-                                'y': '455829.0',
-                                'z': '-0.18'}}],
+        Example response PI_JSON = {
+            "timeSeries": [
+                {
+                    "header": {
+                        "endDate": {"date": "2012-01-02", "time": "00:00:00"},
+                        "firstValueTime": {"date": "2012-01-01", "time": "00:15:00"},
+                        "lastValueTime": {"date": "2012-01-02", "time": "00:00:00"},
+                        "lat": "52.08992726570302",
+                        "locationId": "OW433001",
+                        "lon": "4.9547458967486095",
+                        "maxValue": "-0.28",
+                        "minValue": "-0.44",
+                        "missVal": "-999.0",
+                        "moduleInstanceId": "WerkFilter",
+                        "parameterId": "H.G.0",
+                        "startDate": {"date": "2012-01-01", "time": "00:00:00"},
+                        "stationName": "HAANWIJKERSLUIS_4330-w_Leidsche " "Rijn",
+                        "timeStep": {"unit": "nonequidistant"},
+                        "type": "instantaneous",
+                        "units": "mNAP",
+                        "valueCount": "102",
+                        "x": "125362.0",
+                        "y": "455829.0",
+                        "z": "-0.18",
+                    }
+                }
+            ]
+        }
         """
         api_call = api_calls.GetTimeSeriesStatistics(
             start_time=start_time,
             end_time=end_time,
             location_ids=location_id,
             parameter_ids=parameter_id,
             qualifier_ids=qualifier_id,
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/base.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import abstractmethod
-from fewspy.constants.choices import ApiParameters
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.constants.pi_settings import PiSettings
-from fewspy.constants.request_settings import RequestSettings
-from fewspy.converters.manager import ResponseManager
-from fewspy.retry_session import RetryBackoffSession
-from fewspy.utils.conversions import datetime_to_fews_str
-from fewspy.utils.conversions import snake_to_camel_case
+from hdsr_fewspy.constants.choices import ApiParameters
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.constants.pi_settings import PiSettings
+from hdsr_fewspy.constants.request_settings import RequestSettings
+from hdsr_fewspy.converters.manager import ResponseManager
+from hdsr_fewspy.converters.utils import datetime_to_fews_str
+from hdsr_fewspy.converters.utils import snake_to_camel_case
+from hdsr_fewspy.retry_session import RetryBackoffSession
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
@@ -48,15 +48,15 @@
     @abstractmethod
     def required_request_args(self) -> List[str]:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def allowed_output_choices(self) -> List[str]:
-        """Every GetRequest has its own list with >=1 fewspy.constants.choices.OutputChoices."""
+        """Every GetRequest has its own list with >=1 hdsr_fewspy.constants.choices.OutputChoices."""
         raise NotImplementedError
 
     def validate_base_constructor(self):
         all_parameters = self._unpack_all_parameters()
         msg = "code error required_request_args"
         for x in self.required_request_args:
             if x not in self.allowed_request_args:
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from fewspy.api_calls.base import GetRequest
-from fewspy.constants.choices import ApiParameters
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.api_calls.base import GetRequest
+from hdsr_fewspy.constants.choices import ApiParameters
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
 from typing import List
 
 import logging
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_locations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from fewspy.api_calls.base import GetRequest
-from fewspy.constants.choices import ApiParameters
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.utils.conversions import camel_to_snake_case
-from fewspy.utils.conversions import geo_datum_to_crs
-from fewspy.utils.conversions import xy_array_to_point
+from hdsr_fewspy.api_calls.base import GetRequest
+from hdsr_fewspy.constants.choices import ApiParameters
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.converters.utils import camel_to_snake_case
+from hdsr_fewspy.converters.utils import geo_datum_to_crs
+from hdsr_fewspy.converters.utils import xy_array_to_point
 from typing import List
 from typing import Union
 
 import geopandas as gpd
 import logging
 import pandas as pd
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fewspy.api_calls.base import GetRequest
-from fewspy.constants.choices import ApiParameters
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.utils.conversions import camel_to_snake_case
+from hdsr_fewspy.api_calls.base import GetRequest
+from hdsr_fewspy.constants.choices import ApiParameters
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.converters.utils import camel_to_snake_case
 from typing import List
 from typing import Union
 
 import logging
 import pandas as pd
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from fewspy.api_calls.base import GetRequest
-from fewspy.constants.choices import ApiParameters
-from fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.api_calls.base import GetRequest
+from hdsr_fewspy.constants.choices import ApiParameters
+from hdsr_fewspy.constants.choices import OutputChoices
 from typing import List
 from typing import Tuple
 from xml.etree import ElementTree
 
 import logging
 import pandas as pd
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_samples.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
-from fewspy.api_calls.base import GetRequest
-from fewspy.constants.choices import ApiParameters
-from fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.api_calls.base import GetRequest
+from hdsr_fewspy.constants.choices import ApiParameters
+from hdsr_fewspy.constants.choices import OutputChoices
 from typing import List
 
 import logging
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from fewspy.api_calls.base import GetRequest
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.api_calls.base import GetRequest
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
 from typing import List
 
 import logging
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import abstractmethod
 from datetime import datetime
-from fewspy.api_calls.base import GetRequest
-from fewspy.constants.choices import ApiParameters
-from fewspy.constants.choices import PiRestDocumentFormatChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.converters.xml_to_python_obj import parse
-from fewspy.utils.conversions import datetime_to_fews_str
-from fewspy.utils.date_frequency import DateFrequencyBuilder
+from hdsr_fewspy.api_calls.base import GetRequest
+from hdsr_fewspy.constants.choices import ApiParameters
+from hdsr_fewspy.constants.choices import PiRestDocumentFormatChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.converters.utils import datetime_to_fews_str
+from hdsr_fewspy.converters.xml_to_python_obj import parse
+from hdsr_fewspy.date_frequency import DateFrequencyBuilder
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import logging
 import pandas as pd
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from fewspy.api_calls.time_series.base import GetTimeSeriesBase
-from fewspy.constants.choices import OutputChoices
-from fewspy.utils.date_frequency import DateFrequencyBuilder
+from hdsr_fewspy.api_calls.time_series.base import GetTimeSeriesBase
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.date_frequency import DateFrequencyBuilder
 from pathlib import Path
 from typing import Dict
 from typing import List
 
 import logging
 import pandas as pd
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fewspy.api_calls.time_series.base import GetTimeSeriesBase
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.converters.json_to_df_timeseries import response_jsons_to_one_df
-from fewspy.utils.date_frequency import DateFrequencyBuilder
+from hdsr_fewspy.api_calls.time_series.base import GetTimeSeriesBase
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.converters.json_to_df_timeseries import response_jsons_to_one_df
+from hdsr_fewspy.date_frequency import DateFrequencyBuilder
 from typing import List
 from typing import Union
 
 import pandas as pd
 
 
 class GetTimeSeriesSingle(GetTimeSeriesBase):
```

### Comparing `hdsr_fewspy-1.0/fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from fewspy.api_calls.time_series.get_time_series_single import GetTimeSeriesSingle
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.api_calls.time_series.get_time_series_single import GetTimeSeriesSingle
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
 from typing import List
 
 import logging
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdsr_fewspy-1.0/fewspy/constants/choices.py` & `hdsr_fewspy-1.1/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.0/fewspy/constants/paths.py` & `hdsr_fewspy-1.1/hdsr_fewspy/constants/paths.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 
 
 G_DRIVE = Path("G:/")
 
 BASE_DIR = Path(__file__).parent.parent.parent
-TEST_INPUT_DIR = BASE_DIR / "fewspy" / "tests" / "data" / "input"
+TEST_INPUT_DIR = BASE_DIR / "hdsr_fewspy" / "tests" / "data" / "input"
 DEFAULT_OUTPUT_FOLDER = G_DRIVE / "hdsr_fewspy_output"
 
 assert BASE_DIR.is_dir()
-assert TEST_INPUT_DIR.is_dir()
 assert BASE_DIR.name == "hdsr_fewspy", f"BASE_DIR must be hdsr_fewspy, but is {BASE_DIR.name}"
 
 SECRETS_ENV_PATH = G_DRIVE / "secrets.env"
 GITHUB_PERSONAL_ACCESS_TOKEN = "GITHUB_PERSONAL_ACCESS_TOKEN"
 HDSR_FEWSPY_EMAIL = "HDSR_FEWSPY_EMAIL"
 HDSR_FEWSPY_TOKEN = "HDSR_FEWSPY_TOKEN"
```

### Comparing `hdsr_fewspy-1.0/fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.1/hdsr_fewspy/constants/pi_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import asdict
 from dataclasses import dataclass
-from fewspy.constants.choices import TimeZoneChoices
+from hdsr_fewspy.constants import github
+from hdsr_pygithub import GithubFileDownloader
 from typing import Dict
 
 import logging
+import pandas as pd
 import typing
 import validators
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -91,30 +93,61 @@
             raise AssertionError(f"test_url '{self.test_url}' must be valid")
 
     @property
     def all_fields(self) -> Dict:
         return asdict(self)
 
 
-pi_settings_sa = PiSettings(
-    settings_name="default stand-alone",
-    document_version=1.25,
-    ssl_verify=True,
-    domain="localhost",
-    port=8080,
-    service="FewsWebServices",
-    filter_id="INTERNAL-API",
-    module_instance_ids="WerkFilter",  # "ImportOpvlWater",
-    time_zone=TimeZoneChoices.gmt,
-)
-
-pi_settings_production = PiSettings(
-    settings_name="default production",
-    document_version=1.25,
-    ssl_verify=True,
-    domain="webwis-prd01.ad.hdsr.nl",
-    port=8081,
-    service="OwdPiService",
-    filter_id="owdapi-opvlwater-noneq",
-    module_instance_ids="WerkFilter",
-    time_zone=TimeZoneChoices.gmt,
-)
+class GithubPiSettings:
+
+    expected_columns = [
+        "settings_name",
+        "document_version",
+        "ssl_verify",
+        "domain",
+        "port",
+        "service",
+        "filter_id",
+        "module_instance_ids",
+        "time_zone",
+    ]
+
+    @classmethod
+    def _read_github(cls, settings_name: str) -> pd.Series:
+        logger.info(f"get_on_the_fly_pi_settings for setttings_name {settings_name}")
+        github_downloader = GithubFileDownloader(
+            target_file=github.GITHUB_HDSR_FEWSPY_AUTH_SETTINGS_TARGET_FILE,
+            allowed_period_no_updates=github.GITHUB_HDSR_FEWSPY_AUTH_ALLOWED_PERIOD_NO_UPDATES,
+            repo_name=github.GITHUB_HDSR_FEWSPY_AUTH_REPO_NAME,
+            branch_name=github.GITHUB_HDSR_FEWSPY_AUTH_BRANCH_NAME,
+            repo_organisation=github.GITHUB_ORGANISATION,
+        )
+        df = pd.read_csv(filepath_or_buffer=github_downloader.get_download_url(), sep=";")
+        df_slice = df[df["settings_name"] == settings_name]
+        if df_slice.empty:
+            available_setting_names = df["settings_name"].tolist()
+            msg = f"pi settings_name {settings_name} is not in available setting_names {available_setting_names}"
+            raise AssertionError(msg)
+        assert len(df_slice) == 1, "code error"
+        assert sorted(df.columns) == sorted(cls.expected_columns), "code_error"
+        pd_series = df_slice.iloc[0]
+        return pd_series
+
+    @classmethod
+    def get_pi_settings(cls, settings_name: str) -> PiSettings:
+        pd_series = cls._read_github(settings_name=settings_name)
+        pi_settings = PiSettings(
+            settings_name=pd_series["settings_name"],
+            document_version=pd_series["document_version"],
+            ssl_verify=bool(pd_series["ssl_verify"]),
+            domain=pd_series["domain"],
+            port=int(pd_series["port"]),
+            service=pd_series["service"],
+            filter_id=pd_series["filter_id"],
+            module_instance_ids=pd_series["module_instance_ids"],
+            time_zone=float(pd_series["time_zone"]),
+        )
+        return pi_settings
+
+
+pi_settings_sa = GithubPiSettings.get_pi_settings(settings_name="standalone")
+pi_settings_production = GithubPiSettings.get_pi_settings(settings_name="production")
```

### Comparing `hdsr_fewspy-1.0/fewspy/constants/request_settings.py` & `hdsr_fewspy-1.1/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.0/fewspy/converters/download.py` & `hdsr_fewspy-1.1/hdsr_fewspy/converters/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fewspy.constants.custom_types import ResponseType
-from fewspy.converters.json_to_df_timeseries import response_jsons_to_one_df
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.converters.json_to_df_timeseries import response_jsons_to_one_df
 from pathlib import Path
 from typing import Dict
 from typing import List
 
 import json
 import logging
 import requests
```

### Comparing `hdsr_fewspy-1.0/fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.1/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import datetime
-from fewspy.constants.choices import TimeZoneChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.utils.conversions import camel_to_snake_case
-from fewspy.utils.conversions import dict_to_datetime
+from hdsr_fewspy.constants.choices import TimeZoneChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.converters.utils import camel_to_snake_case
+from hdsr_fewspy.converters.utils import dict_to_datetime
 from typing import List
 from typing import Tuple
 
 import pandas as pd
 
 
 DATETIME_KEYS = ["start_date", "end_date"]
```

### Comparing `hdsr_fewspy-1.0/fewspy/converters/manager.py` & `hdsr_fewspy-1.1/hdsr_fewspy/converters/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.custom_types import ResponseType
-from fewspy.converters.download import CsvDownloadDir
-from fewspy.converters.download import JsonDownloadDir
-from fewspy.converters.download import XmlDownloadDir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.converters.download import CsvDownloadDir
+from hdsr_fewspy.converters.download import JsonDownloadDir
+from hdsr_fewspy.converters.download import XmlDownloadDir
 from pathlib import Path
 from typing import List
 
 import logging
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdsr_fewspy-1.0/fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.1/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.0/fewspy/permissions.py` & `hdsr_fewspy-1.1/hdsr_fewspy/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fewspy.constants import github
-from fewspy.exceptions import NoPermissionInHdsrFewspyAuthError
-from fewspy.exceptions import UserInvalidTokenHdsrFewspyAuthError
-from fewspy.exceptions import UserNotFoundInHdsrFewspyAuthError
-from fewspy.secrets import Secrets
+from hdsr_fewspy.constants import github
+from hdsr_fewspy.exceptions import NoPermissionInHdsrFewspyAuthError
+from hdsr_fewspy.exceptions import UserInvalidTokenHdsrFewspyAuthError
+from hdsr_fewspy.exceptions import UserNotFoundInHdsrFewspyAuthError
+from hdsr_fewspy.secrets import Secrets
 from hdsr_pygithub import GithubFileDownloader
 from typing import Dict
 from typing import List
 
 import logging
 import pandas as pd
 import validators
@@ -40,15 +40,15 @@
 
     @property
     def permissions_row(self) -> pd.Series:
         if self._permission_row is not None:
             return self._permission_row
         logger.info("determine permissions")
         github_downloader = GithubFileDownloader(
-            target_file=github.GITHUB_HDSR_FEWSPY_AUTH_TARGET_FILE,
+            target_file=github.GITHUB_HDSR_FEWSPY_AUTH_USERS_TARGET_FILE,
             allowed_period_no_updates=github.GITHUB_HDSR_FEWSPY_AUTH_ALLOWED_PERIOD_NO_UPDATES,
             repo_name=github.GITHUB_HDSR_FEWSPY_AUTH_REPO_NAME,
             branch_name=github.GITHUB_HDSR_FEWSPY_AUTH_BRANCH_NAME,
             repo_organisation=github.GITHUB_ORGANISATION,
         )
         df = pd.read_csv(filepath_or_buffer=github_downloader.get_download_url(), sep=";")
```

### Comparing `hdsr_fewspy-1.0/fewspy/retry_session.py` & `hdsr_fewspy-1.1/hdsr_fewspy/retry_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from fewspy import exceptions
-from fewspy.constants.pi_settings import PiSettings
-from fewspy.constants.request_settings import RequestSettings
+from hdsr_fewspy import exceptions
+from hdsr_fewspy.constants.pi_settings import PiSettings
+from hdsr_fewspy.constants.request_settings import RequestSettings
 from pathlib import Path
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from time import sleep
 from typing import List
 from typing import Optional
 from typing import Tuple
```

### Comparing `hdsr_fewspy-1.0/fewspy/secrets.py` & `hdsr_fewspy-1.1/hdsr_fewspy/secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dotenv import load_dotenv
-from fewspy.constants.paths import GITHUB_PERSONAL_ACCESS_TOKEN
-from fewspy.constants.paths import HDSR_FEWSPY_EMAIL
-from fewspy.constants.paths import HDSR_FEWSPY_TOKEN
-from fewspy.constants.paths import SECRETS_ENV_PATH
+from hdsr_fewspy.constants.paths import GITHUB_PERSONAL_ACCESS_TOKEN
+from hdsr_fewspy.constants.paths import HDSR_FEWSPY_EMAIL
+from hdsr_fewspy.constants.paths import HDSR_FEWSPY_TOKEN
+from hdsr_fewspy.constants.paths import SECRETS_ENV_PATH
 from pathlib import Path
 
 import logging
 import os
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/fixtures.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from fewspy.api import Api
-from fewspy.constants.pi_settings import pi_settings_sa
+from hdsr_fewspy.api import Api
+from hdsr_fewspy.constants.pi_settings import pi_settings_sa
 from pathlib import Path
 
 import pytest
 
 
 @pytest.fixture(scope="session")
 def fixture_api_sa_no_download_dir():
     api = Api(pi_settings=pi_settings_sa)
     assert api.pi_settings.base_url == pi_settings_sa.base_url
     assert api.pi_settings.ssl_verify == True  # noqa
-    assert api.pi_settings.settings_name == "default stand-alone"
+    assert api.pi_settings.settings_name == "standalone"
     assert api.pi_settings.filter_id == "INTERNAL-API"
     assert api.pi_settings.service == "FewsWebServices"
     assert api.pi_settings.module_instance_ids == "WerkFilter"
     return api
 
 
 @pytest.fixture(scope="session")
 def fixture_api_sa_with_download_dir(tmpdir_factory):
     output_dir = tmpdir_factory.mktemp("hdsr_fewspy_test_dir")  # tmpdir_factory can do session scope. nice!
     output_dir_path = Path(output_dir)
     assert output_dir_path.is_dir()
     api = Api(pi_settings=pi_settings_sa, output_directory_root=output_dir_path)
     assert api.pi_settings.base_url == pi_settings_sa.base_url
     assert api.pi_settings.ssl_verify == True  # noqa
-    assert api.pi_settings.settings_name == "default stand-alone"
+    assert api.pi_settings.settings_name == "standalone"
     assert api.pi_settings.filter_id == "INTERNAL-API"
     assert api.pi_settings.service == "FewsWebServices"
     assert api.pi_settings.module_instance_ids == "WerkFilter"
     return api
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
-from fewspy.constants.paths import TEST_INPUT_DIR
-from fewspy.converters.xml_to_python_obj import parse
+from hdsr_fewspy.constants.paths import TEST_INPUT_DIR
+from hdsr_fewspy.converters.xml_to_python_obj import parse
 from pathlib import Path
 from typing import Dict
 
 import json
 import pandas as pd
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.tests.fixtures import fixture_api_sa_no_download_dir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_no_download_dir
 
 import pytest
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.tests.fixtures import fixture_api_sa_no_download_dir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_no_download_dir
 
 import geopandas as gpd
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.tests.fixtures import fixture_api_sa_no_download_dir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_no_download_dir
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
 
 
 def test_sa_parameters_json(fixture_api_sa_no_download_dir):
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.converters.xml_to_python_obj import parse
-from fewspy.tests import fixtures_requests
-from fewspy.tests.fixtures import fixture_api_sa_no_download_dir
-from fewspy.tests.fixtures import fixture_api_sa_with_download_dir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.converters.xml_to_python_obj import parse
+from hdsr_fewspy.tests import fixtures_requests
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_no_download_dir
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_with_download_dir
 
 import json
 import pandas as pd
 import pytest
 
 
 # silence flake8
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.converters.xml_to_python_obj import parse
-from fewspy.tests import fixtures_requests
-from fewspy.tests.fixtures import fixture_api_sa_no_download_dir
-from fewspy.tests.fixtures import fixture_api_sa_with_download_dir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.converters.xml_to_python_obj import parse
+from hdsr_fewspy.tests import fixtures_requests
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_no_download_dir
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_with_download_dir
 
 import pandas as pd
 import pytest
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.tests import fixtures_requests
-from fewspy.tests.fixtures import fixture_api_sa_no_download_dir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.tests import fixtures_requests
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_no_download_dir
 
 import pytest
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
```

### Comparing `hdsr_fewspy-1.0/fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from fewspy.constants.choices import OutputChoices
-from fewspy.constants.choices import TimeZoneChoices
-from fewspy.tests.fixtures import fixture_api_sa_no_download_dir
+from hdsr_fewspy.constants.choices import OutputChoices
+from hdsr_fewspy.constants.choices import TimeZoneChoices
+from hdsr_fewspy.tests.fixtures import fixture_api_sa_no_download_dir
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
 
 
 def test_sa_timezone_response(fixture_api_sa_no_download_dir):
```

### Comparing `hdsr_fewspy-1.0/fewspy/utils/conversions.py` & `hdsr_fewspy-1.1/hdsr_fewspy/converters/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from fewspy.constants.choices import TimeZoneChoices
+from hdsr_fewspy.constants.choices import TimeZoneChoices
 from shapely.geometry import Point
 from typing import List
 
 import numpy as np
 
 
 GEODATUM_MAPPING = {
```

### Comparing `hdsr_fewspy-1.0/fewspy/utils/date_frequency.py` & `hdsr_fewspy-1.1/hdsr_fewspy/date_frequency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fewspy.constants.request_settings import RequestSettings
+from hdsr_fewspy.constants.request_settings import RequestSettings
 from typing import List
 from typing import Tuple
 
 import logging
 import pandas as pd
```

### Comparing `hdsr_fewspy-1.0/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: hdsr-fewspy
-Version: 1.0
-Summary: An interface for interacting with hdsr github repos
-Home-page: https://github.com/hdsr-mid/hdsr_pygithub
-Author: Renier Kramer
-Author-email: renier.kramer@hdsr.nl
-License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_pygithub/archive/v1.0.tar.gz
-Keywords: interface,interaction,github,files,hdsr
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.txt
-
 ### Context
 * Created: February 2023
 * Author: Renier Kramer, renier.kramer@hdsr.nl
 * Python version: >3.7
 
 [hkvfewspy]: https://github.com/HKV-products-services/hkvfewspy
 [fewspy]: https://github.com/d2hydro/fewspy
@@ -35,72 +13,76 @@
 
 ### Description
 A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService: FEWS-WIS or FEWS-EFCIS. 
 Note that this project only works on HDSR's internal network, so within the VDI. The project combines the best from 
 two existing fewspy projects: [fewspy] and [hkvfewspy]. On top of that it adds authentication, authorisation, and 
 throttling. The latter is to minimize request load on HDSR's internal FEWS instances. 
 
-Hdsr_fewspy API support 9 different API calls:
-1. get_parameters:
-2. get_filters:
-3. get_locations:
-4. get_qualifiers: 
-5. get_timezone_id: 
-6. get_samples: 
-7. get_time_series_single: 
-8. get_time_series_multi:
-9: get_time_series_statistics:
-
-An API call can return 6 different output formats:   
+Hdsr_fewspy API support 9 different API calls that can return 6 different output formats:   
 1. xml_file_in_download_dir: The xml response is written to a .xml file in your download_dir
 2. json_file_in_download_dir: The json response is written to a .json file in your download_dir
 3. csv_file_in_download_dir: The json response is converted to csv and written to a .csv file in your download_dir
 4. xml_response_in_memory: the xml response is returned memory meaning you get a list with one or more responses 
 5. json_response_in_memory: the json response is returned memory meaning you get a list with one or more responses        
 6. pandas_dataframe_in_memory: the json response is converted to a pandas dataframe meaning you get one dataframe 
 
-Each API call supports a subset of output formats:
+API call                      | Supported outputs  | Notes 
+------------------------------|--------------------|--------
+get_parameters                | 4, 5, 6            | Returns 1 object (xml/json response or dataframe) 
+get_filters                   | 4, 5               | Returns 1 object (xml/json response)  
+get_locations                 | 4, 5               | Returns 1 object (xml/json response)              
+get_qualifiers                | 4, 5               | Returns 1 object (xml/json response)
+get_timezone_id               | 4, 5               | Returns 1 object (xml/json response)
+get_samples                   | 1, 2               | Not implemented yet
+get_time_series_single        | 4, 5, 6            | Returns a 1 dataframe or a list with >=1 xml/json responses or     
+get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
+get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response) 
 
-API call| Supported outputs | Notes 
---------|-------------------|--------
-1       | 4, 5, 6           | Not implemented yet
-2       | 4, 5              | Not implemented yet  
-3       | 4, 5              | Not implemented yet              
-4       | 4, 5              | Not implemented yet
-5       | 4, 5              | Not implemented yet
-6       | 1, 2              | Not implemented yet
-7       | 4, 5, 6           | One large call can results in multiple small calls. Output 4 and 5 return a list with >=1 responses. Output 6 aggregates all responses and returns one dataframe.    
-8       | 1, 2, 3           | One unique location_parameter_qualifier combination results in >=1 API calls = >=1 responses. For output 1 and 2 each response results in 1 file. Output 3 creates 1 csv per unique combination.
-9       | 4, 5              | Not implemented yet 
+- One large call can result in multiple small calls. Output 4 and 5 return a list with >=1 responses. Output 6 aggregates all responses and returns one dataframe.
+- One unique location_parameter_qualifier combination results in >=1 API calls = >=1 responses. For output 1 and 2 each response results in 1 file. Output 3 creates 1 csv per unique combination.
 
 ### Usage
 
 ###### Preparation
 1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
 HDSR_FEWSPY_EMAIL=<your_hdsr_email>
 HDSR_FEWSPY_TOKEN=<contact renier.kramer.hdsr.nl to get HDSR_FEWSPY_TOKEN>
 ```
 2. Only once per project: install hdsr_fewspy dependency
 ```
-pip install hdsr_fewspy 
-or 
-conda install hdsr_fewspy -c hdsr-mid
+pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
 3. Run imports and instantiate hdsr_fewspy API 
 ```
+from hdsr_fewspy imoprt Api
+from hdsr_fewspy import PiSettings
+
 # instantiate API using default settings:
-api = Api()
+api = Api()  
 
 # or instantiate API using custom settings:
-custom_
-api 
-```
+custom_settings = PiSettings(
+   settings_name="blablabla",            
+   document_version=1.25",
+   ssl_verify=True,
+   domain="localhost",
+   port="8080",
+   service="FewsWebServices",
+   filter_id="INTERNAL-API",
+   module_instance_ids="WerkFilter",
+   time_zone=0.0,
+)
+api = Api(pi_settings=custom_settings)
 
+# or if you want download responses (xml, json, csv), then you need to specify a download_dir.
+# The files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/  
+api = Api(output_directory_root=<path_to_your_directory>)
+```
 
 ###### Examples different API calls
 1. Example get_time_series_single
 ```
 api = Api()
 
 responses = api.get_time_series_single(
@@ -153,52 +135,52 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (25 april 2023)
+### Test Coverage (26 april 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
-Name                                                         Stmts   Miss  Cover
---------------------------------------------------------------------------------
-fewspy\__init__.py                                               4      0   100%
-fewspy\api.py                                                   98     13    87%
-fewspy\api_calls\__init__.py                                    18      0   100%
-fewspy\api_calls\base.py                                       100     12    88%
-fewspy\api_calls\get_filters.py                                 25      0   100%
-fewspy\api_calls\get_locations.py                               44      2    95%
-fewspy\api_calls\get_parameters.py                              40      1    98%
-fewspy\api_calls\get_qualifiers.py                              36     12    67%
-fewspy\api_calls\get_samples.py                                 26      8    69%
-fewspy\api_calls\get_timezone_id.py                             26      1    96%
-fewspy\api_calls\time_series\base.py                            91      6    93%
-fewspy\api_calls\time_series\get_time_series_multi.py           67      5    93%
-fewspy\api_calls\time_series\get_time_series_single.py          28      1    96%
-fewspy\api_calls\time_series\get_time_series_statistics.py      12      0   100%
-fewspy\constants\choices.py                                     89      3    97%
-fewspy\constants\custom_types.py                                 2      0   100%
-fewspy\constants\github.py                                       7      0   100%
-fewspy\constants\paths.py                                       12      0   100%
-fewspy\constants\pi_settings.py                                 50      4    92%
-fewspy\constants\request_settings.py                            11      0   100%
-fewspy\converters\download.py                                   93      4    96%
-fewspy\converters\json_to_df_timeseries.py                     112      8    93%
-fewspy\converters\manager.py                                    27      0   100%
-fewspy\converters\xml_to_python_obj.py                         105     26    75%
-fewspy\exceptions.py                                            12      0   100%
-fewspy\permissions.py                                           67      5    93%
-fewspy\retry_session.py                                         68     12    82%
-fewspy\secrets.py                                               64     20    69%
-fewspy\utils\conversions.py                                     45     17    62%
-fewspy\utils\date_frequency.py                                  46      5    89%
-setup.py                                                        10     10     0%
---------------------------------------------------------------------------------
-TOTAL                                                         1435    175    88%
+Name                                                              Stmts   Miss  Cover
+-------------------------------------------------------------------------------------
+hdsr_fewspy\__init__.py                                               4      0   100%
+hdsr_fewspy\api.py                                                   98     13    87%
+hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
+hdsr_fewspy\api_calls\base.py                                       100     12    88%
+hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
+hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
+hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
+hdsr_fewspy\api_calls\get_qualifiers.py                              36     12    67%
+hdsr_fewspy\api_calls\get_samples.py                                 26      8    69%
+hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
+hdsr_fewspy\api_calls\time_series\base.py                            91      6    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           67      5    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_single.py          28      1    96%
+hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      12      0   100%
+hdsr_fewspy\constants\choices.py                                     89      3    97%
+hdsr_fewspy\constants\custom_types.py                                 2      0   100%
+hdsr_fewspy\constants\github.py                                       8      0   100%
+hdsr_fewspy\constants\paths.py                                       11      0   100%
+hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
+hdsr_fewspy\constants\request_settings.py                            11      0   100%
+hdsr_fewspy\converters\download.py                                   93      4    96%
+hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
+hdsr_fewspy\converters\manager.py                                    27      0   100%
+hdsr_fewspy\converters\utils.py                                      45     17    62%
+hdsr_fewspy\converters\xml_to_python_obj.py                         105     26    75%
+hdsr_fewspy\date_frequency.py                                        46      5    89%
+hdsr_fewspy\exceptions.py                                            12      0   100%
+hdsr_fewspy\permissions.py                                           67      5    93%
+hdsr_fewspy\retry_session.py                                         68     12    82%
+hdsr_fewspy\secrets.py                                               64     20    69%
+setup.py                                                             10     10     0%
+-------------------------------------------------------------------------------------
+TOTAL                                                              1458    178    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
@@ -272,9 +254,7 @@
   - pip:
     - <a pip package>==<version>
 ```
 You can also write a requirements.txt file:
 ```
 > pip list --format=freeze > <path_to_project>/requirements.txt
 ```
-
-
```

### Comparing `hdsr_fewspy-1.0/pyproject.toml` & `hdsr_fewspy-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.0/setup.py` & `hdsr_fewspy-1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.0"
+version = "1.1"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
@@ -20,25 +20,29 @@
     "validators",
 ]
 
 tests_require = ["pytest", "pytest-cov"]
 
 setup(
     name="hdsr_fewspy",
-    packages=find_packages(include=["fewspy", "fewspy.*"]),
+    packages=find_packages(include=["hdsr_fewspy", "hdsr_fewspy.*"]),
     version=version,
     license="MIT",
-    description="An interface for interacting with hdsr github repos",
+    description="A python project to get data (locations, timeseries, etc.) from a HDSR FEWS PiWebService",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Renier Kramer",
     author_email="renier.kramer@hdsr.nl",
-    url="https://github.com/hdsr-mid/hdsr_pygithub",
-    download_url=f"https://github.com/hdsr-mid/hdsr_pygithub/archive/v{version}.tar.gz",
-    keywords=["interface", "interaction", "github", "files", "hdsr"],
+    url="https://github.com/hdsr-mid/hdsr_fewspy",
+    download_url=f"https://github.com/hdsr-mid/hdsr_fewspy/archive/v{version}.tar.gz",
+    keywords=[
+        "hdsr",
+        "fews",
+        "api",
+    ],
     zip_safe=False,
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={"test": tests_require},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

