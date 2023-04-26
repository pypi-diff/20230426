# Comparing `tmp/qiboconnection-0.7.2.tar.gz` & `tmp/qiboconnection-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiboconnection-0.7.2.tar", last modified: Wed Mar 15 10:22:27 2023, max compression
+gzip compressed data, was "qiboconnection-0.8.0.tar", last modified: Tue Apr 25 14:48:45 2023, max compression
```

## Comparing `qiboconnection-0.7.2.tar` & `qiboconnection-0.8.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.204064 qiboconnection-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-15 10:22:27.204064 qiboconnection-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-15 10:22:27.204064 qiboconnection-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.196065 qiboconnection-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.200065 qiboconnection-0.7.2/src/qiboconnection/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35423 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.200065 qiboconnection-0.7.2/src/qiboconnection/constants/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/constants/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.200065 qiboconnection-0.7.2/src/qiboconnection/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/device_characteristics_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/device_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/offline_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/online_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/quantum_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/quantum_device_calibration_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/quantum_device_characteristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/simulator_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/simulator_device_characteristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/devices/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/live_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/live_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/runcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/saved_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/saved_experiment_listing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.204064 qiboconnection-0.7.2/src/qiboconnection/typings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/live_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/runcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/typings/saved_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/src/qiboconnection/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.200065 qiboconnection-0.7.2/src/qiboconnection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-15 10:22:27.000000 qiboconnection-0.7.2/src/qiboconnection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-15 10:22:27.000000 qiboconnection-0.7.2/src/qiboconnection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 10:22:27.000000 qiboconnection-0.7.2/src/qiboconnection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 10:22:27.000000 qiboconnection-0.7.2/src/qiboconnection.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-15 10:22:27.000000 qiboconnection-0.7.2/src/qiboconnection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-15 10:22:27.000000 qiboconnection-0.7.2/src/qiboconnection.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:22:27.204064 qiboconnection-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_live_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_live_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_runcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_runcard_typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_saved_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_saved_experiment_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_saved_experiment_typings.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-15 10:21:44.000000 qiboconnection-0.7.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.106653 qiboconnection-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.118653 qiboconnection-0.8.0/src/qiboconnection/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35447 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.122653 qiboconnection-0.8.0/src/qiboconnection/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/constants/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.126653 qiboconnection-0.8.0/src/qiboconnection/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/device_characteristics_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/device_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/offline_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/online_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_calibration_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_characteristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device_characteristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/live_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/live_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/runcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/saved_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/saved_experiment_listing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.130653 qiboconnection-0.8.0/src/qiboconnection/typings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/live_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/runcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/saved_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.118653 qiboconnection-0.8.0/src/qiboconnection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:48:44.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28880 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_live_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_live_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_runcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_runcard_typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_saved_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_saved_experiment_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_saved_experiment_typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_util.py
```

### Comparing `qiboconnection-0.7.2/LICENSE` & `qiboconnection-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/PKG-INFO` & `qiboconnection-0.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiboconnection
-Version: 0.7.2
+Version: 0.8.0
 Summary: manage the remote connection to send qibo experiment to the quantum devices and simulators
 Home-page: https://github.com/qilimanjaro-tech/qiboconnection
 Author: Qibo team
 Author-email: info@qilimanjaro.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10.0
```

### Comparing `qiboconnection-0.7.2/pyproject.toml` & `qiboconnection-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
-version = "0.7.2"
+version = "0.8.0"
 version_files = [
     "src/qiboconnection/__init__.py",
     "pyproject.toml:version"
 ]
 tag_format = "v$version"
 update_changelog_on_bump = true
```

### Comparing `qiboconnection-0.7.2/setup.py` & `qiboconnection-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/api.py` & `qiboconnection-0.8.0/src/qiboconnection/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,15 @@
             device_ids=device_ids,
         )
         return self._wait_and_return_results(deadline=deadline, interval=interval, job_ids=job_ids)
 
     """ REMOTE PLOTTING """
 
     @typechecked
-    def create_liveplot(
+    async def create_liveplot(
         self,
         plot_type: str = LivePlotType.LINES.value,
         title: str | None = None,
         x_label: str | None = None,
         y_label: str | None = None,
         z_label: str | None = None,
         x_axis: npt.NDArray[np.int_] | List[int] | None = None,
@@ -498,25 +498,25 @@
             path=f"{self.LIVE_PLOTTING_PATH}", data={}
         )
         if status_code != 200:
             raise RemoteExecutionException(
                 message="Live-plotting connection data could not be retrieved.", status_code=status_code
             )
         plotting_response = PlottingResponse.from_response(**response)
-        self._live_plots.create_live_plot(
+        await self._live_plots.create_live_plot(
             plot_id=plotting_response.plot_id,
             websocket_url=plotting_response.websocket_url,
             plot_type=LivePlotType(plot_type),
             labels=LivePlotLabels(title=title, x_label=x_label, y_label=y_label, z_label=z_label),
             axis=LivePlotAxis(x_axis=x_axis, y_axis=y_axis),
         )
         return plotting_response.plot_id
 
     @typechecked
-    def send_plot_points(
+    async def send_plot_points(
         self,
         plot_id: int,
         x: npt.NDArray[np.float_ | np.int_] | list[float] | list[int] | float | int,
         y: npt.NDArray[np.float_ | np.int_] | list[float] | list[int] | float | int,
         z: npt.NDArray[np.float_ | np.int_] | list[float] | list[int] | float | int | None = None,
     ):
         """Sends point(s) to a specific plot.
@@ -525,15 +525,15 @@
             x: x coord of the point to send info to
             y: y coord of the point to send info to
             z: z coord of the point to send info to
 
         Returns:
             None
         """
-        return self._live_plots.send_data(plot_id=plot_id, x=x, y=y, z=z)
+        return await self._live_plots.send_data(plot_id=plot_id, x=x, y=y, z=z)
 
     """ SAVED EXPERIMENTS """
 
     @typechecked
     def save_experiment(
         self,
         name: str,
```

### Comparing `qiboconnection-0.7.2/src/qiboconnection/api_utils.py` & `qiboconnection-0.8.0/src/qiboconnection/api_utils.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/config.py` & `qiboconnection-0.8.0/src/qiboconnection/config.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/connection.py` & `qiboconnection-0.8.0/src/qiboconnection/connection.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/device.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/device_characteristics_util.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/device_characteristics_util.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/device_details.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/device_details.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/devices.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/devices.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/offline_device.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/offline_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/online_device.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/online_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/quantum_device.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/quantum_device_calibration_details.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_calibration_details.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/quantum_device_characteristics.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_characteristics.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/simulator_device.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/simulator_device_characteristics.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device_characteristics.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/devices/util.py` & `qiboconnection-0.8.0/src/qiboconnection/devices/util.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/errors.py` & `qiboconnection-0.8.0/src/qiboconnection/errors.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/job.py` & `qiboconnection-0.8.0/src/qiboconnection/job.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/job_result.py` & `qiboconnection-0.8.0/src/qiboconnection/job_result.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/live_plots.py` & `qiboconnection-0.8.0/src/qiboconnection/live_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,26 @@
 
 @dataclass
 class LivePlots(ABC):
     """Job class to manage the job experiment to be remotely sent"""
 
     _live_plots: dict = field(default_factory=dict)
 
-    def create_live_plot(
+    async def create_live_plot(
         self, plot_id: int, plot_type: LivePlotType, websocket_url: str, labels: LivePlotLabels, axis: LivePlotAxis
     ):
         """Creates a new LivePlot with the provided information and appends it to the internal _live_plots dict"""
         self._live_plots[plot_id] = LivePlot(
             plot_id=plot_id,
             plot_type=plot_type,
             websocket_url=websocket_url,
             labels=labels,
             axis=axis,
         )
+        await self._live_plots[plot_id].start_up()
 
     def _get_live_plot(self, plot_id: int) -> LivePlot:
         """
         Internal getter that returns the liveplot instance associatied to the provided plot_id
         Args:
             plot_id: id of the plot to be retrieved.
         """
@@ -87,15 +88,15 @@
             if live_plot.plot_type == LivePlotType.HEATMAP and (
                 live_plot.axis.x_axis is None or live_plot.axis.y_axis is None
             ):
                 raise ValueError("HEATMAP plots need to have axis provided on live-plot creation.")
 
             return self._method(*args, **kwargs)
 
-    def send_data(
+    async def send_data(
         self,
         plot_id: int,
         x: npt.NDArray[np.float_ | np.int_] | list[float] | list[int] | float | int,
         y: npt.NDArray[np.float_ | np.int_] | list[float] | list[int] | float | int,
         z: npt.NDArray[np.float_ | np.int_] | list[float] | list[int] | float | int | None,
     ):
         """
@@ -113,12 +114,13 @@
             plot_type=live_plot.plot_type,
             x=x,
             y=y,
             z=z,
             labels=live_plot.labels,
             axis=live_plot.axis,
         )
-        self._send_data(live_plot=live_plot, data_packet=data_packet)
+        await self._send_data(live_plot=live_plot, data_packet=data_packet)
 
     @CheckDataAndPlotTypeCompatibility
     def _send_data(self, live_plot: LivePlot, data_packet: LivePlotPacket):
+        """Actually sends the data using the live_plot's socket"""
         return live_plot.send_data(data=data_packet)
```

### Comparing `qiboconnection-0.7.2/src/qiboconnection/runcard.py` & `qiboconnection-0.8.0/src/qiboconnection/runcard.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/saved_experiment.py` & `qiboconnection-0.8.0/src/qiboconnection/saved_experiment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/saved_experiment_listing.py` & `qiboconnection-0.8.0/src/qiboconnection/saved_experiment_listing.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/typings/algorithm.py` & `qiboconnection-0.8.0/src/qiboconnection/typings/algorithm.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/typings/auth_config.py` & `qiboconnection-0.8.0/src/qiboconnection/typings/auth_config.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/typings/connection.py` & `qiboconnection-0.8.0/src/qiboconnection/typings/connection.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/typings/device.py` & `qiboconnection-0.8.0/src/qiboconnection/typings/device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/typings/job.py` & `qiboconnection-0.8.0/src/qiboconnection/typings/job.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/typings/live_plot.py` & `qiboconnection-0.8.0/src/qiboconnection/typings/live_plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -96,14 +96,24 @@
         return self._y
 
     @property
     def z(self):
         """z getter."""
         return self._z
 
+    @property
+    def idx(self):
+        """idx getter."""
+        return self._idx
+
+    @property
+    def idy(self):
+        """idy getter."""
+        return self._idy
+
     def _parse_to_points(
         self,
         x: int | float | list[int] | list[float] | npt.NDArray[np.int_ | np.float_],
         y: int | float | list[int] | list[float] | npt.NDArray[np.int_ | np.float_],
         z: int | float | list[int] | list[float] | npt.NDArray[np.int_ | np.float_] | None = None,
         idx: int | list[int] | npt.NDArray[np.int_] | None = None,
         idy: int | list[int] | npt.NDArray[np.int_] | None = None,
@@ -155,14 +165,30 @@
                     self._idx == other._idx,
                     self._idy == other._idy,
                 ]
             )
         return False
 
 
+def _ensure_packet_types(packets: List):
+    """Ensures all elements are valid LivePlotPackets"""
+    if not all(isinstance(packet, LivePlotPacket) for packet in packets):
+        raise ValueError("Not all packets were LivePlotPackets")
+
+
+def _ensure_packet_compatibility(packets: List):
+    """Ensures all elements of packets are from a same compatible Liveplot"""
+    same_plot_id = (packet.plot_id == packets[0].plot_id for packet in packets)
+    same_plot_type = (packet.plot_type == packets[0].plot_type for packet in packets)
+    same_labels = (packet.labels == packets[0].labels for packet in packets)
+    same_axis = (packet.axis == packets[0].axis for packet in packets)
+    if not (all(same_plot_id) and all(same_plot_type) and all(same_labels) and all(same_axis)):
+        raise ValueError("Trying to agglutinate data packets with different information")
+
+
 @dataclass
 class LivePlotPacket(ABC):
     """Packet with the needed information for sending in each message we want to throw over the live-plotting ws."""
 
     plot_id: int
     plot_type: LivePlotType
     data: LivePlotPoints
@@ -254,7 +280,35 @@
         }
 
     def to_json(self) -> str:
         """
         Serializes the info of the class in a json-formatted string
         """
         return json.dumps(self.to_dict())
+
+    @classmethod
+    def agglutinate(cls, packets: List):
+        """Build a single LivePlotPacket from a list of LivePlotPackets with the data merged"""
+
+        if not packets:
+            return None
+
+        _ensure_packet_types(packets=packets)
+        _ensure_packet_compatibility(packets=packets)
+
+        extended_x: list[int] | list[float] = list[float]()
+        extended_y: list[int] | list[float] = list[float]()
+        extended_z: list[int] | list[float] = list[float]()
+        extended_idx: list[int] = list[int]()
+        extended_idy: list[int] = list[int]()
+        extended_x.extend((packet.data.x for packet in packets))
+        extended_y.extend((packet.data.y for packet in packets))
+        extended_z.extend((packet.data.z for packet in packets))
+        extended_idx.extend((packet.data.idx for packet in packets))
+        extended_idy.extend((packet.data.idy for packet in packets))
+        return cls(
+            plot_id=packets[0].plot_id,
+            plot_type=packets[0].plot_type,
+            data=LivePlotPoints(x=extended_x, y=extended_y, z=extended_z, idx=extended_idx, idy=extended_idy),
+            labels=packets[0].labels,
+            axis=packets[0].axis,
+        )
```

### Comparing `qiboconnection-0.7.2/src/qiboconnection/typings/saved_experiment.py` & `qiboconnection-0.8.0/src/qiboconnection/typings/saved_experiment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection/util.py` & `qiboconnection-0.8.0/src/qiboconnection/util.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/src/qiboconnection.egg-info/PKG-INFO` & `qiboconnection-0.8.0/src/qiboconnection.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiboconnection
-Version: 0.7.2
+Version: 0.8.0
 Summary: manage the remote connection to send qibo experiment to the quantum devices and simulators
 Home-page: https://github.com/qilimanjaro-tech/qiboconnection
 Author: Qibo team
 Author-email: info@qilimanjaro.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10.0
```

### Comparing `qiboconnection-0.7.2/src/qiboconnection.egg-info/SOURCES.txt` & `qiboconnection-0.8.0/src/qiboconnection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_algorithm.py` & `qiboconnection-0.8.0/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_api.py` & `qiboconnection-0.8.0/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """API testing"""
+import asyncio
 from dataclasses import asdict
 from unittest.mock import MagicMock, patch
 
 import pandas as pd
 import pytest
 
 from qiboconnection.api import API
 from qiboconnection.devices.devices import Devices
 from qiboconnection.devices.util import create_device
 from qiboconnection.errors import ConnectionException, RemoteExecutionException
 from qiboconnection.runcard import Runcard
 from qiboconnection.saved_experiment import SavedExperiment
 from qiboconnection.saved_experiment_listing import SavedExperimentListing
+from qiboconnection.typings.live_plot import PlottingResponse
 
 from .data import experiment_dict, results_dict, runcard_dict, web_responses
+from .utils import get_current_event_loop_or_create
 
 
 def test_api_constructor(mocked_api: API):
     """Test API class constructor"""
     assert isinstance(mocked_api, API)
 
 
@@ -184,14 +187,68 @@
     with pytest.raises(RemoteExecutionException):
         mocked_api.select_device_ids(device_ids=[1])
 
     mocked_web_call.assert_called_with(self=mocked_api._connection, path=f"{mocked_api.DEVICES_CALL_PATH}/1")
     assert mocked_api._selected_devices == []
 
 
+@patch("websockets.connect", autospec=True)
+@patch("qiboconnection.connection.Connection.send_post_auth_remote_api_call", autospec=True)
+def test_create_live_plot(mocked_web_call: MagicMock, mocked_websockets_connect: MagicMock, mocked_api: API):
+    """Test the creation of a liveplot using the api"""
+
+    loop = get_current_event_loop_or_create()
+    mocked_connection_future = loop.create_future()
+    mocked_connection_future.set_result(MagicMock())
+    mocked_websockets_connect.return_value = mocked_connection_future
+
+    mocked_web_call.return_value = PlottingResponse(websocket_url="test_url", plot_id=1).to_dict(), 200
+
+    plot_id = asyncio.run(mocked_api.create_liveplot())
+
+    mocked_web_call.assert_called_with(self=mocked_api._connection, path=mocked_api.LIVE_PLOTTING_PATH, data={})
+    mocked_websockets_connect.assert_called_with("test_url")
+    assert plot_id == 1
+
+
+@patch("qiboconnection.connection.Connection.send_post_auth_remote_api_call", autospec=True)
+def test_create_live_plot_with_unexpected_response(mocked_web_call: MagicMock, mocked_api: API):
+    """Test the creation of a liveplot using the api"""
+
+    mocked_web_call.return_value = {}, 400
+
+    with pytest.raises(RemoteExecutionException):
+        _ = asyncio.run(mocked_api.create_liveplot())
+
+
+@patch("qiboconnection.live_plot.LivePlot.send_data", autospec=True)
+@patch("websockets.connect", autospec=True)
+@patch("qiboconnection.connection.Connection.send_post_auth_remote_api_call", autospec=True)
+def test_send_plot_points(
+    mocked_web_call: MagicMock,
+    mocked_websockets_connect: MagicMock,
+    mocked_live_plot_send_data: MagicMock,
+    mocked_api: API,
+):
+    """Test the creation of a liveplot using the api"""
+
+    loop = get_current_event_loop_or_create()
+    mocked_connection_future = loop.create_future()
+    mocked_connection_future.set_result(MagicMock())
+    mocked_websockets_connect.return_value = mocked_connection_future
+
+    mocked_web_call.return_value = PlottingResponse(websocket_url="test_url", plot_id=1).to_dict(), 200
+
+    plot_id = asyncio.run(mocked_api.create_liveplot())
+
+    asyncio.run(mocked_api.send_plot_points(plot_id=plot_id, x=0, y=0))
+
+    mocked_live_plot_send_data.assert_called()
+
+
 @patch("qiboconnection.connection.Connection.send_post_auth_remote_api_call", autospec=True)
 def test_save_experiment(mocked_web_call: MagicMock, mocked_api: API):
     """Tests API.save_experiment() method"""
     mocked_web_call.return_value = web_responses.saved_experiments.create_response
 
     name = "MyDemoExperiment"
     description = "A test saved experiment"
```

### Comparing `qiboconnection-0.7.2/tests/test_connection.py` & `qiboconnection-0.8.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_device.py` & `qiboconnection-0.8.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_devices.py` & `qiboconnection-0.8.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_environment.py` & `qiboconnection-0.8.0/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_errors.py` & `qiboconnection-0.8.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_job.py` & `qiboconnection-0.8.0/tests/test_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         job_status=job_status,
         id=23,
         nshots=10,
     )
     expected_job_request = JobRequest(
         user_id=user_id,
         device_id=simulator_device.id,
-        description="Ly8gR2VuZXJhdGVkIGJ5IFFJQk8gMC4xLjEwCk9QRU5RQVNNIDIuMDsKaW5jbHVkZSAicWVsaWIxLmluYyI7CnFyZWcgcVsxXTsKY3JlZyByZWdpc3RlcjBbMV07CmggcVswXTsKbWVhc3VyZSBxWzBdIC0-IHJlZ2lzdGVyMFswXTs=",
+        description="Ly8gR2VuZXJhdGVkIGJ5IFFJQk8gMC4xLjEyLmRldjAKT1BFTlFBU00gMi4wOwppbmNsdWRlICJxZWxpYjEuaW5jIjsKcXJlZyBxWzFdOwpjcmVnIHJlZ2lzdGVyMFsxXTsKaCBxWzBdOwptZWFzdXJlIHFbMF0gLT4gcmVnaXN0ZXIwWzBdOw==",
         number_shots=10,
         job_type=JobType.CIRCUIT,
     )
     assert isinstance(job, Job)
     assert job.job_request == expected_job_request
```

### Comparing `qiboconnection-0.7.2/tests/test_job_result.py` & `qiboconnection-0.8.0/tests/test_job_result.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_live_plots.py` & `qiboconnection-0.8.0/tests/test_live_plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """ Tests methods for LivePlots """
 
+import asyncio
+from unittest.mock import MagicMock, patch
+
 import pytest
+import websockets
 
 from qiboconnection.live_plot import LivePlot
 from qiboconnection.live_plots import LivePlots
 from qiboconnection.typings.live_plot import (
     LivePlotAxis,
     LivePlotLabels,
     LivePlotPacket,
     LivePlotType,
 )
 
+from .utils import get_current_event_loop_or_create
+
 
 def ok_method(*args, **kwargs):
     """returns `'ok'`"""
     return "OK"
 
 
 @pytest.fixture(name="live_plot_type")
@@ -37,35 +43,90 @@
 
 def test_live_plots_constructor():
     """test live plot creation"""
     live_plots = LivePlots()
     assert isinstance(live_plots, LivePlots)
 
 
+@patch("websockets.connect", autospec=True)
 def test_live_plots_add_plot(
-    live_plot_type: LivePlotType, live_plot_labels: LivePlotLabels, live_plot_axis: LivePlotAxis
+    mocked_websockets_connect: MagicMock,
+    live_plot_type: LivePlotType,
+    live_plot_labels: LivePlotLabels,
+    live_plot_axis: LivePlotAxis,
 ):
     """test live plot `create_live_plot`"""
+    """Tests LivePlots add plot functionality"""
+
+    loop = get_current_event_loop_or_create()
+
+    mocked_connection_future = loop.create_future()
+    mocked_connection_future.set_result(MagicMock())
+    mocked_websockets_connect.return_value = mocked_connection_future
+
     live_plots = LivePlots()
     expected_live_plot = LivePlot(
         plot_id=1,
         plot_type=live_plot_type,
         websocket_url="server/demo-url",
         labels=live_plot_labels,
         axis=live_plot_axis,
     )
-    live_plots.create_live_plot(
-        plot_id=1,
-        plot_type=live_plot_type,
-        websocket_url="server/demo-url",
-        labels=live_plot_labels,
-        axis=live_plot_axis,
+    asyncio.run(expected_live_plot.start_up())
+
+    asyncio.run(
+        live_plots.create_live_plot(
+            plot_id=1,
+            plot_type=live_plot_type,
+            websocket_url="server/demo-url",
+            labels=live_plot_labels,
+            axis=live_plot_axis,
+        )
+    )
+    created_live_plot = live_plots._get_live_plot(plot_id=1)
+
+    mocked_websockets_connect.assert_called_with("server/demo-url")
+    assert expected_live_plot == created_live_plot
+
+
+@patch("qiboconnection.live_plot.LivePlot.send_data", autospec=True)
+@patch("qiboconnection.live_plot.websockets.connect", autospec=True)
+def test_live_plots_send_data(
+    mocked_websockets_connect: MagicMock,
+    live_plot_send_data: MagicMock,
+    live_plot_type: LivePlotType,
+    live_plot_labels: LivePlotLabels,
+    live_plot_axis: LivePlotAxis,
+):
+    """Tests the LivePlots send_data functionality, mocking the inferior LivePlot layer."""
+
+    loop = get_current_event_loop_or_create()
+
+    mocked_connection_future = loop.create_future()
+    mocked_connection_future.set_result(MagicMock())
+    mocked_websockets_connect.return_value = mocked_connection_future
+
+    live_plots = LivePlots()
+    asyncio.run(
+        live_plots.create_live_plot(
+            plot_id=1,
+            plot_type=live_plot_type,
+            websocket_url="server/demo-url",
+            labels=live_plot_labels,
+            axis=live_plot_axis,
+        )
+    )
+
+    asyncio.run(live_plots.send_data(plot_id=1, x=1, y=1, z=None))
+
+    expected_sent_data_packet = LivePlotPacket.build_packet(
+        plot_id=1, plot_type=live_plot_type, x=1, y=1, z=None, labels=live_plot_labels, axis=live_plot_axis
     )
 
-    assert expected_live_plot.__dict__ == live_plots._get_live_plot(plot_id=1).__dict__
+    live_plot_send_data.assert_called_with(self=live_plots._get_live_plot(plot_id=1), data=expected_sent_data_packet)
 
 
 def test_check_data_and_plot_type_compatibility_with_ok_case(
     live_plot_type: LivePlotType, live_plot_labels: LivePlotLabels, live_plot_axis: LivePlotAxis
 ):
     """test live plot `CheckDataAndPlotTypeCompatibility` works with base case"""
     live_plot = LivePlot(
```

### Comparing `qiboconnection-0.7.2/tests/test_runcard.py` & `qiboconnection-0.8.0/tests/test_runcard.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_runcard_typings.py` & `qiboconnection-0.8.0/tests/test_runcard_typings.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_saved_experiment.py` & `qiboconnection-0.8.0/tests/test_saved_experiment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_saved_experiment_listing.py` & `qiboconnection-0.8.0/tests/test_saved_experiment_listing.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_saved_experiment_typings.py` & `qiboconnection-0.8.0/tests/test_saved_experiment_typings.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.7.2/tests/test_util.py` & `qiboconnection-0.8.0/tests/test_util.py`

 * *Files identical despite different names*

