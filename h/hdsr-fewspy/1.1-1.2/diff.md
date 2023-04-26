# Comparing `tmp/hdsr_fewspy-1.1.tar.gz` & `tmp/hdsr_fewspy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.1.tar", last modified: Wed Apr 26 12:03:06 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.2.tar", last modified: Wed Apr 26 16:28:17 2023, max compression
```

## Comparing `hdsr_fewspy-1.1.tar` & `hdsr_fewspy-1.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    14179 2023-04-26 12:03:07.000000 hdsr_fewspy-1.1/PKG-INFO
--rw-rw-rw-   0        0        0    13318 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/
--rw-rw-rw-   0        0        0      149 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    14174 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2937 2023-04-26 12:02:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2806 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0     2185 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1300 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     8173 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     5380 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2237 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0      670 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      546 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3051 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      384 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4258 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      713 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0    11693 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     6652 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3967 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:03:05.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    14179 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-04-26 12:03:03.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-26 12:03:02.000000 hdsr_fewspy-1.1/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.1/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-04-26 12:03:07.000000 hdsr_fewspy-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1672 2023-04-26 12:02:06.000000 hdsr_fewspy-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    22492 2023-04-26 16:28:19.000000 hdsr_fewspy-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    21631 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    14174 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7572 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     8173 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     5719 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2636 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     6599 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3051 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      384 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1405 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4258 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      956 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    11635 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     6652 2023-04-26 16:17:41.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3967 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    22492 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-04-26 16:28:19.000000 hdsr_fewspy-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1672 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/setup.py
```

### Comparing `hdsr_fewspy-1.1/LICENSE.txt` & `hdsr_fewspy-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             url=self.url, params=self.filtered_fews_parameters, verify=self.pi_settings.ssl_verify
         )
 
         if self.output_choice in {OutputChoices.json_response_in_memory, OutputChoices.xml_response_in_memory}:
             return response
 
         assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error"
-        # parse the response
+        # parse the response to dataframe
         if response.status_code == 200:
 
             # convert to gdf and snake_case
             df = pd.json_normalize(data=response.json()["locations"])
             df.columns = [camel_to_snake_case(i) for i in df.columns]
             df.set_index("location_id", inplace=True)
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,11 +33,11 @@
             OutputChoices.xml_response_in_memory,
         ]
 
     def run(self) -> ResponseType:
         response = self.retry_backoff_session.get(
             url=self.url, params=self.filtered_fews_parameters, verify=self.pi_settings.ssl_verify
         )
-        # parse the response
+        # parse the response to dataframe
         if response.status_code != 200:
             logger.error(f"FEWS Server responds {response.text}")
         return response
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,25 @@
             assert [isinstance(x, str) for x in self.qualifier_ids]
 
         any_multi = any([len(x) > 1 for x in (self.location_ids, self.parameter_ids, self.qualifier_ids) if x])
         assert (
             any_multi
         ), "Please specify >1 location_ids and/or parameter_ids and/or qualifier_ids. Or use get_time_series_single"
 
+        if self.output_choice != OutputChoices.csv_file_in_download_dir:
+            logger.warning(f"flag_threshold is not used for output_choice {self.output_choice}")
+            if self.drop_missing_values == True:  # noqa
+                logger.warning(f"drop_missing_values is not used for output_choice {self.output_choice}")
+
     @property
     def allowed_output_choices(self) -> List[str]:
         return [
             OutputChoices.xml_file_in_download_dir,
-            OutputChoices.csv_file_in_download_dir,
             OutputChoices.json_file_in_download_dir,
+            OutputChoices.csv_file_in_download_dir,
         ]
 
     def run(self) -> List[Path]:
         all_file_paths = []
         cartesian_parameters_list = self._get_cartesian_parameters_list(parameters=self.initial_fews_parameters)
         for index, request_params in enumerate(cartesian_parameters_list):
             date_ranges, date_range_freq = DateFrequencyBuilder.create_date_ranges_and_frequency_used(
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,37 @@
 from hdsr_fewspy.constants.choices import OutputChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
 from hdsr_fewspy.converters.json_to_df_timeseries import response_jsons_to_one_df
 from hdsr_fewspy.date_frequency import DateFrequencyBuilder
 from typing import List
 from typing import Union
 
+import logging
 import pandas as pd
 
 
+logger = logging.getLogger(__name__)
+
+
 class GetTimeSeriesSingle(GetTimeSeriesBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.validate_constructor()
 
     def validate_constructor(self):
         assert isinstance(self.location_ids, str) and self.location_ids and "," not in self.location_ids
         assert isinstance(self.parameter_ids, str) and self.parameter_ids and "," not in self.parameter_ids
         if self.qualifier_ids:
             assert isinstance(self.qualifier_ids, str) and "," not in self.qualifier_ids
 
+        if self.output_choice != OutputChoices.pandas_dataframe_in_memory:
+            logger.warning(f"flag_threshold is not used for output_choice {self.output_choice}")
+            if self.drop_missing_values == True:  # noqa
+                logger.warning(f"drop_missing_values is not used for output_choice {self.output_choice}")
+
     @property
     def allowed_output_choices(self) -> List[str]:
         return [
             OutputChoices.json_response_in_memory,
             OutputChoices.xml_response_in_memory,
             OutputChoices.pandas_dataframe_in_memory,
         ]
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.2/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/constants/paths.py` & `hdsr_fewspy-1.2/hdsr_fewspy/constants/paths.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from pathlib import Path
 
 
 G_DRIVE = Path("G:/")
 
-BASE_DIR = Path(__file__).parent.parent.parent
-TEST_INPUT_DIR = BASE_DIR / "hdsr_fewspy" / "tests" / "data" / "input"
-DEFAULT_OUTPUT_FOLDER = G_DRIVE / "hdsr_fewspy_output"
-
+BASE_DIR = Path(__file__).parent.parent
 assert BASE_DIR.is_dir()
 assert BASE_DIR.name == "hdsr_fewspy", f"BASE_DIR must be hdsr_fewspy, but is {BASE_DIR.name}"
+TEST_INPUT_DIR = BASE_DIR / "tests" / "data" / "input"
+DEFAULT_OUTPUT_FOLDER = G_DRIVE / "hdsr_fewspy_output"
 
 SECRETS_ENV_PATH = G_DRIVE / "secrets.env"
 GITHUB_PERSONAL_ACCESS_TOKEN = "GITHUB_PERSONAL_ACCESS_TOKEN"
 HDSR_FEWSPY_EMAIL = "HDSR_FEWSPY_EMAIL"
 HDSR_FEWSPY_TOKEN = "HDSR_FEWSPY_TOKEN"
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.2/hdsr_fewspy/constants/pi_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/constants/request_settings.py` & `hdsr_fewspy-1.2/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.2/hdsr_fewspy/converters/download.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.2/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.2/hdsr_fewspy/converters/manager.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.2/hdsr_fewspy/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.2/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.2/hdsr_fewspy/date_frequency.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/permissions.py` & `hdsr_fewspy-1.2/hdsr_fewspy/permissions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.2/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/secrets.py` & `hdsr_fewspy-1.2/hdsr_fewspy/secrets.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 @pytest.fixture(scope="session")
 def fixture_api_sa_with_download_dir(tmpdir_factory):
     output_dir = tmpdir_factory.mktemp("hdsr_fewspy_test_dir")  # tmpdir_factory can do session scope. nice!
     output_dir_path = Path(output_dir)
     assert output_dir_path.is_dir()
     api = Api(pi_settings=pi_settings_sa, output_directory_root=output_dir_path)
+    assert isinstance(api.output_dir, Path)
     assert api.pi_settings.base_url == pi_settings_sa.base_url
     assert api.pi_settings.ssl_verify == True  # noqa
     assert api.pi_settings.settings_name == "standalone"
     assert api.pi_settings.filter_id == "INTERNAL-API"
     assert api.pi_settings.service == "FewsWebServices"
     assert api.pi_settings.module_instance_ids == "WerkFilter"
     return api
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 
 import pytest
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
 
+a = {
+    "version": "1.25",
+    "filters": [
+        {
+            "id": "INTERNAL-API",
+            "name": "INTERNAL-API",
+            "child": [{"id": "INTERNAL-API.RUWMET", "name": "Ruwe metingen (punt)"}],
+        }
+    ],
+}
+
 
 def test_sa_filters_json(fixture_api_sa_no_download_dir):
     response = fixture_api_sa_no_download_dir.get_filters(output_choice=OutputChoices.json_response_in_memory)
     assert response.status_code == 200
 
 
 def test_sa_filters_dataframe(fixture_api_sa_no_download_dir):
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,15 @@
             location_ids=request_data.location_ids,
             parameter_ids=request_data.parameter_ids,
             start_time=request_data.start_time,
             end_time=request_data.end_time,
             output_choice=OutputChoices.json_response_in_memory,
         )
     except Exception as err:
-        msg = (
-            "invalid output_choice 'json_response_in_memory'. GetTimeSeriesMulti has valid_output_choices "
-            "['xml_file_in_download_dir', 'csv_file_in_download_dir', 'json_file_in_download_dir']. See earlier "
-            "logging why we use GetTimeSeriesMulti."
-        )
+        msg = "invalid output_choice 'json_response_in_memory'. GetTimeSeriesMulti has valid_output_choices ['xml_file_in_download_dir', 'json_file_in_download_dir', 'csv_file_in_download_dir']. See earlier logging why we use GetTimeSeriesMulti."
         assert err.args[0] == msg
 
 
 def test_sa_multi_timeseries_1_ok_json_download(fixture_api_sa_with_download_dir):
     """OutputChoices.json_file_in_download_dir"""
     api = fixture_api_sa_with_download_dir
     request_data = fixtures_requests.RequestTimeSeriesMulti1
```

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.2/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,11 +44,12 @@
 hdsr_fewspy/converters/xml_to_python_obj.py
 hdsr_fewspy/tests/__init__.py
 hdsr_fewspy/tests/fixtures.py
 hdsr_fewspy/tests/fixtures_requests.py
 hdsr_fewspy/tests/test_sa_get_filters.py
 hdsr_fewspy/tests/test_sa_get_locations.py
 hdsr_fewspy/tests/test_sa_get_parameters.py
+hdsr_fewspy/tests/test_sa_get_qualifiers.py
 hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
 hdsr_fewspy/tests/test_sa_get_timeseries_single.py
 hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
 hdsr_fewspy/tests/test_sa_timezone_id.py
```

### Comparing `hdsr_fewspy-1.1/pyproject.toml` & `hdsr_fewspy-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.1/setup.py` & `hdsr_fewspy-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.1"
+version = "1.2"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
```

