# Comparing `tmp/linktest-2.0.2.tar.gz` & `tmp/linktest-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.0.2.tar", last modified: Tue Apr 25 14:35:17 2023, max compression
+gzip compressed data, was "dist/linktest-2.0.3.tar", last modified: Wed Apr 26 06:31:52 2023, max compression
```

## Comparing `linktest-2.0.2.tar` & `linktest-2.0.3.tar`

### file list

```diff
@@ -1,88 +1,86 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-25 14:35:17.179132 linktest-2.0.2/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-04-25 14:35:17.178339 linktest-2.0.2/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-25 14:35:17.082212 linktest-2.0.2/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 14:32:28.000000 linktest-2.0.2/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.2/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/auto_generate_test_suite.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17746 2023-04-25 07:00:45.000000 linktest-2.0.2/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/auto_organize_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10936 2023-04-25 07:00:46.000000 linktest-2.0.2/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7063 2023-04-25 07:00:45.000000 linktest-2.0.2/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.2/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.2/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31804 2023-04-25 07:00:46.000000 linktest-2.0.2/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.2/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   110989 2023-04-25 14:28:53.000000 linktest-2.0.2/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.2/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      422 2023-04-25 14:32:22.000000 linktest-2.0.2/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.2/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.2/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3600 2023-04-25 07:00:45.000000 linktest-2.0.2/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-25 14:35:17.089117 linktest-2.0.2/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-04-25 14:35:16.000000 linktest-2.0.2/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2262 2023-04-25 14:35:16.000000 linktest-2.0.2/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-04-25 14:35:16.000000 linktest-2.0.2/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-04-25 14:35:16.000000 linktest-2.0.2/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-04-25 14:35:16.000000 linktest-2.0.2/linktest.egg-info/top_level.txt
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-25 14:35:17.176409 linktest-2.0.2/lintest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/auto_generate_test_suite.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/auto_organize_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/lintest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.2/lintest/xml_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-04-25 14:35:17.179368 linktest-2.0.2/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-04-25 14:35:11.000000 linktest-2.0.2/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:52.000000 linktest-2.0.3/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      192 2023-04-26 06:31:52.000000 linktest-2.0.3/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:52.000000 linktest-2.0.3/lintest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/xml_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_generate_test_suite.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/lintest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_organize_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/testcase_order.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.3/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.3/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.3/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.3/linktest/xml_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.3/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.3/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.3/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.3/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-26 05:35:06.000000 linktest-2.0.3/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      422 2023-04-26 06:29:54.000000 linktest-2.0.3/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.3/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.3/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.3/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.3/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100509 2023-04-26 03:25:21.000000 linktest-2.0.3/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.3/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.3/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.3/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.3/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-04-26 06:31:40.000000 linktest-2.0.3/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-04-26 06:31:52.000000 linktest-2.0.3/setup.cfg
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      192 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `linktest-2.0.2/linktest/appium_utils.py` & `linktest-2.0.3/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/auto_generate_test_suite.py` & `linktest-2.0.3/lintest/auto_generate_test_suite.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/auto_generate_testcase_list.py` & `linktest-2.0.3/lintest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.3/lintest/auto_generate_testcase_list_from_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 self.logger.info("start run_test()...")
                 login(self, username, password, channel)
 
       -----> 如果正确运行后，框架会根据 testLogin.csv & testLogin.py 自动生成符合框架运行标准的 auto_generated_by_csv.py文件（testLogin_case_list_auto_generated_by_csv.py）
         注意：和__init__.py文件类似，每次执行，都会根据相应的 .csv & .py文件自动生成最新的 auto_generated_by_csv.py文件
       testLogin_case_list_auto_generated_by_csv.py 内容如下：
 
-        from linktest.api_testcase import APITestCase
+        from lintest.api_testcase import APITestCase
         from tests.api.csv_dataset import testLoginDataSet
 
 
         class testLoginDataSet_1(APITestCase):
             tag = "testLoginDataSet"
 
             def run_test(self):
@@ -129,15 +129,15 @@
                         self.logger.info("start run_test()...") 
                         login(self, username, password, channel)
                         
               -----> 如果正确运行后，框架会根据 testLogin.csv & testLogin.py 自动生成符合框架运行标准的 auto_generated_by_csv.py文件（testLogin_case_list_auto_generated_by_csv.py）
                 注意：和__init__.py文件类似，每次执行，都会根据相应的 .csv & .py文件自动生成最新的 auto_generated_by_csv.py文件
               testLogin_case_list_auto_generated_by_csv.py 内容如下：
               
-                from linktest.api_testcase import APITestCase
+                from lintest.api_testcase import APITestCase
                 from tests.api.csv_dataset import testLoginDataSet
                 
                 
                 class testLoginDataSet_1(APITestCase):
                     tag = "testLoginDataSet"
                 
                     def run_test(self):
@@ -280,15 +280,15 @@
                 self.logger.info("start run_test()...")
                 login(self, username, password, channel)
 
       -----> 如果正确运行后，框架会根据 testLogin.csv & testLogin.py 自动生成符合框架运行标准的 auto_generated_by_csv.py文件（testLogin_case_list_auto_generated_by_csv.py）
         注意：和__init__.py文件类似，每次执行，都会根据相应的 .csv & .py文件自动生成最新的 auto_generated_by_csv.py文件
       testLogin_case_list_auto_generated_by_csv.py 内容如下：
 
-        from linktest.api_testcase import APITestCase
+        from lintest.api_testcase import APITestCase
         from tests.api.csv_dataset import testLoginDataSet
 
 
         class testLoginDataSet_1(APITestCase):
             tag = "testLoginDataSet"
 
             def run_test(self):
@@ -357,23 +357,23 @@
                         for line in py_file_obj.readlines():
                             if line.replace(" ", "").startswith("self.browser."):
                                 is_ui_testcase = True
                                 # 导入 UTTestCase
                                 with open(PROJECT_INFO.project_path + os.sep + directory_path + os.sep +
                                           file_name.split(".")[
                                               0] + "_case_list_auto_generated_by_csv.py", "a") as f:
-                                    f.write("from linktest.ui_testcase import UITestCase")
+                                    f.write("from lintest.ui_testcase import UITestCase")
                                 break
 
                     if not is_ui_testcase:
                         # 导入 UTTestCase
                         with open(PROJECT_INFO.project_path + os.sep + directory_path + os.sep +
                                   file_name.split(".")[
                                       0] + "_case_list_auto_generated_by_csv.py", "a") as f:
-                            f.write("from linktest.api_testcase import APITestCase")
+                            f.write("from lintest.api_testcase import APITestCase")
 
                     csv_file_full_path = PROJECT_INFO.project_path + os.sep + directory_path + os.sep + \
                                          file_name.split('.')[0] + ".csv"
 
 
                     # 解析 py 文件, 判断文件中是否有 tag = "tagName" 有则说明需要 为自动生成的testcase 同时设置用户自定义的 tagName
                     tag_name = ''
```

### Comparing `linktest-2.0.2/linktest/auto_organize_testcase.py` & `linktest-2.0.3/lintest/auto_organize_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/base_testcase.py` & `linktest-2.0.3/lintest/base_testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         # # todo: 此处用于 构建多线程时 每个线程独立的 TestEngineCaseInput(线程id作为key)
         # print("===================+++++++++++++==========threading.currentThread().ident")
         # print(threading.currentThread().ident)
 
         # self.CaseData 用于记录 case执行过程中产生的数据（多数情况用于 某个 testcase chain中, 某个Testcase中有调用了 另外一个Testcase.run_test() 则此case 被定义一个 TestcaseChain）
         # eg:
-        # from linktest.api_testcase import APITestCase
+        # from lintest.api_testcase import APITestCase
         # from tests.api.testcase_demo.testcase1 import Testcase1
         # from tests.api.testcase_demo.testcase2 import Testcase2
         #
         # class Testcase3(APITestCase):
         #     tag = 'case3'
         #
         #     def run_test(self):
@@ -177,24 +177,24 @@
             self.logger.info("assert_is_not_none(%s)  -- Failed" % (actual_val))
             raise
 
     def compare_json_and_return_diff(self, expected_json, actual_json, rules=None):
         """
         此方法 比较两个 json 时会忽略结构体内item的顺序,即如下 json1 & json2 会被认为是相同的
         json1 = {
-            "name": "linktest",
+            "name": "lintest",
             "Company": {
                 "name": "IKEA",
                 "No": 1
             },
             "version": "1.0"
         }
         json2 = {
             "version": "1.0",
-            "name": "linktest",
+            "name": "lintest",
             "Company": {
                 "name": "IKEA",
                 "No": 1
             }
         }
         """
 
@@ -217,15 +217,15 @@
 
     def compare_json_and_assert_equal(self, expected_json, actual_json, rules=None):
         diff = self.compare_json_and_return_diff(expected_json, actual_json, rules)
         self.pprint(diff)
         assert diff == {}
 
     def compare_json_with_strict_mode(self, expected_json, actual_json):
-        """不会忽略json体内Item的顺序, 即: { "name": "linktest", "version": 1.0 } 和 {"version": 1.0, "name": "linktest" } 是不同的, 本质上就是当做字符串来比较"""
+        """不会忽略json体内Item的顺序, 即: { "name": "lintest", "version": 1.0 } 和 {"version": 1.0, "name": "lintest" } 是不同的, 本质上就是当做字符串来比较"""
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> compare_json_with_strict_mode: ")
         v1 = json.dumps(expected_json, sort_keys=False)
         v2 = json.dumps(actual_json, sort_keys=False)
 
         self.logger.info("------ expected_json: ")
         self.logger.info(self.pformat(v1))
@@ -237,15 +237,15 @@
         self.pprint(v1)
         print("------ actual_json: ")
         self.pprint(v2)
 
         assert v1 == v2
 
     # def compare_json_with_strict_mode(self, expected_json, actual_json):
-    #     """不会忽略json体内Item的顺序, 即: { "name": "linktest", "version": 1.0 } 和 {"version": 1.0, "name": "linktest" } 是不同的"""
+    #     """不会忽略json体内Item的顺序, 即: { "name": "lintest", "version": 1.0 } 和 {"version": 1.0, "name": "lintest" } 是不同的"""
     #
     #     self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> compare_json_with_strict_mode: ")
     #     self.logger.info("------ expected_json: ")
     #     self.logger.info(self.pformat(expected_json))
     #     self.logger.info("------ actual_json: ")
     #     self.logger.info(self.pformat(actual_json))
     #
```

### Comparing `linktest-2.0.2/linktest/clean_data.py` & `linktest-2.0.3/lintest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/conver_xml_into_db.py` & `linktest-2.0.3/lintest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/database_helper.py` & `linktest-2.0.3/lintest/database_helper.py`

 * *Files identical despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-database_helper.py is used to save the linktest's execution's logs
+database_helper.py is used to save the lintest's execution's logs
 
 @author: Wang Lin
 """
 import os
 import socket
 import traceback
 import pymysql
```

### Comparing `linktest-2.0.2/linktest/date_utilities.py` & `linktest-2.0.3/lintest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/doctor.py` & `linktest-2.0.3/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/framework_log.py` & `linktest-2.0.3/lintest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/get_adb_devices.py` & `linktest-2.0.3/lintest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/get_ios_devices_list.py` & `linktest-2.0.3/lintest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/get_platform_info.py` & `linktest-2.0.3/lintest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/get_project_info.py` & `linktest-2.0.3/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/html_report.py` & `linktest-2.0.3/linktest/html_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                             </tr>
                             <tr>
                                 <th>Execution Host OS</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
                                 <th>Test Framework</th>
-                                <td align='center'><a target="_blank" href="https://plugins.jetbrains.com/plugin/19712-linktest/versions">linktest %s</a></td>
+                                <td align='center'><a target="_blank" href="https://plugins.jetbrains.com/plugin/19712-lintest/versions">linktest %s</a></td>
                             </tr>
                         </table>
                     </td>
                 </tr>
             </table>
             """ % (
                 start_time.strftime("%Y-%m-%d %H:%M:%S %p"),
```

### Comparing `linktest-2.0.2/linktest/logged_requests.py` & `linktest-2.0.3/lintest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/main.py` & `linktest-2.0.3/linktest/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -608,15 +608,14 @@
                     TestCaseExecutor.executing_ios_testcase_flag = True
 
             if issubclass(testcase, android_testcase.AndroidTestCase):
                 device_name = TestCaseExecutor.get_device_name(testcase)
 
                 if getattr(TestCaseExecutor, device_name) is True:
                     TestCaseExecutor.testcase_queue.appendleft(testcase)
-                    # TestCaseExecutor.testcase_queue.append(testcase)
                     print(
                         "------ already one android testcase executing on device: %s" % device_name)
                     time.sleep(DEFAULT_SLEEP_TIME_FOR_MOBILE_TESTCASE)
                     continue
                 else:
                     setattr(TestCaseExecutor, device_name, True)
 
@@ -768,26 +767,21 @@
                         app_path = testcase.ios_desired_capabilities["app"]
                         if app_path.startswith("/"):
                             # if the app_path starts_with "/", then it means user set the absolute path, just pass it.
                             pass
                         else:
                             if app_path.startswith("app/"):
                                 testcase.ios_desired_capabilities["app"] = project_info.project_path + "/" + app_path
-                            else:
-                                # use the package (e.g: app: "com.ikea")
-                                pass
 
                     executing_testcase.ios_driver = mobiledriver.Remote(
                         'http://%s:%s/wd/hub' % (testcase.appium_server_ip, testcase.appium_server_port),
                         desired_capabilities=testcase.ios_desired_capabilities)
                     executing_testcase.logger.info(
                         '---------- IOS Driver Info: %s' % executing_testcase.ios_driver.__dict__ + os.linesep)
 
-                    # log_memory_usage("after create ios driver", executing_testcase)
-
                     if hasattr(settings, "ios_implicitly_wait"):
                         if type(settings.ios_implicitly_wait) == int or type(settings.ios_implicitly_wait) == float:
                             executing_testcase.ios_driver.implicitly_wait(getattr(settings, "ios_implicitly_wait"))
                             executing_testcase.logger.info("set ios_implicitly_wait:%s" % settings.ios_implicitly_wait)
                         else:
                             # if the type of settings.ios_implicitly_wait is not correct, here set a default value: 60
                             executing_testcase.ios_driver.implicitly_wait(60)
@@ -835,16 +829,14 @@
                             "there are no android_implicitly_wait found in settings, then set a default value: 60")
                         executing_testcase.logger.warning(
                             "there are no android_implicitly_wait found in settings, then set a default value: 60")
 
                     executing_testcase.logger.info(
                         '---------- Android Driver Info: %s' % executing_testcase.android_driver.__dict__ + os.linesep)
 
-                    # log_memory_usage("after create android driver", executing_testcase)
-
                 # Backend testcases will not need to create browser & close browser
                 if issubclass(testcase, ui_testcase.UITestCase):
                     try:
                         executing_testcase.create_browser_driver()
                         testcase.browser = executing_testcase.browser
                         testcase.browserName = executing_testcase.browser.name
                         executing_testcase.logger.info(
@@ -909,17 +901,15 @@
                     executing_testcase.logger.info("------ run_test() Start")
 
                     # For DEBUG_RUN mode,will not set timeout for each testcase
                     executing_testcase.run_test()
 
             except BaseException:
                 executing_testcase.ExecutionStatusSetByFramework = "failed"
-                # log_memory_usage("catch exception", executing_testcase)
                 traceback.print_exc()
-                # print(testcase.__dict__)
                 traceback_info = traceback.format_exc()
 
                 if issubclass(testcase, ui_testcase.UITestCase):
 
                     try:
                         # save the current URL and all the browser's related information when got error.
                         executing_testcase.logger.error(
@@ -949,15 +939,14 @@
                             # remove the html tag in execption_info
                             exception_info = re.sub(r'</?\w+[^>]*>', '', exception_info)
                             break
 
                 executing_testcase.exception_info = exception_info
                 executing_testcase.exception_info_for_xml_report = re.sub(r'</?\w+[^>]*>', '', traceback_info_str)
                 executing_testcase.error_message_for_db = executing_testcase.exception_info_for_xml_report
-                # testcase.exception_info_for_xml_report = traceback_info_str
                 executing_testcase.traceback_info = traceback_info
 
                 TestCaseExecutor.failed_testcases.append(executing_testcase)
 
                 if TestCaseExecutor.rerun_testcase_queue is not None:
                     if executing_testcase.rerun_tag == 0:
                         TestCaseExecutor.rerun_testcase_queue.append(testcase)
@@ -1000,32 +989,14 @@
                         }
 
 
                         res = executing_testcase.requests.post(
                             "%s/case/exec/complete" % settings.TestEngineCallBackAPI,
                             data=json.dumps(callback_post_data),
                             headers=headers)
-
-                        # if res.status_code == 200:
-                        #     log_file_content = ""
-                        #     with open(executing_testcase.logfile_full_name, "r") as case_log_file:
-                        #         # log_file_content = case_log_file.read()
-                        #         log_path = project_info.project_name + executing_testcase.logfile_full_name.split(
-                        #             project_info.project_name + os.sep + "output")[-1]
-                        #         print(log_path)
-                        #         # todo: remove
-                        #         # change to save the log_path instead of log content
-                        #         log_file_content = log_path
-                        #
-                        #     executing_testcase.requests.post("%s/chainData/uploadLog?chainDataId=%s&currentCaseIndex=%s" %(
-                        #         settings.TestEngineCallBackAPI,
-                        #         executing_testcase.TestEngineCaseInput["execution_id"], executing_testcase.TestEngineCaseInput["case_index"]),
-                        #                                 data=log_file_content.encode(),
-                        #                                 headers=headers)
-
                 except BaseException:
                     traceback.print_exc()
                     executing_testcase.logger.error(traceback.format_exc())
                     pass
             else:
                 # TestCaseExecutor.passed_testcases.append(testcase)
                 TestCaseExecutor.passed_testcases.append(executing_testcase)
@@ -1072,56 +1043,25 @@
                             "testExecutionStatus": "PASSED"
                         }
 
                         res = executing_testcase.requests.post(
                             "%s/case/exec/complete" % settings.TestEngineCallBackAPI,
                             data=json.dumps(callback_post_data),
                             headers=headers)
-
-                        # if res.status_code == 200:
-                        #     log_file_content = ""
-                        #     with open(executing_testcase.logfile_full_name, "r") as case_log_file:
-                        #         # log_file_content = case_log_file.read()
-                        #         log_path = project_info.project_name + executing_testcase.logfile_full_name.split(
-                        #             project_info.project_name + os.sep + "output")[-1]
-                        #         print(log_path)
-                        #
-                        #         # change to save the log_path instead of log content
-                        #         log_file_content = log_path
-                        #
-                        #     executing_testcase.requests.post(
-                        #         "%s/chainData/uploadLog?chainDataId=%s&currentCaseIndex=%s" % (
-                        #             settings.TestEngineCallBackAPI,
-                        #             executing_testcase.TestEngineCaseInput["execution_id"],
-                        #             executing_testcase.TestEngineCaseInput["case_index"]),
-                        #         data=log_file_content.encode(),
-                        #         headers=headers)
                 except BaseException:
                     traceback.print_exc()
                     executing_testcase.logger.error("\n\n")
                     executing_testcase.logger.error("******************************** Invoke TestEngine Callback ******")
                     executing_testcase.logger.error("********************************  Error  *************************")
                     executing_testcase.logger.error(traceback.format_exc())
                     pass
             finally:
                 # 如果case中 有调用： self.GlobalDataList.append("XXX") 则推荐 settings中设置 ReRun_flag = False
                 executing_testcase.GlobalExecutedCaseList.append(executing_testcase)
 
-                # try:
-                #     print(
-                #         "TestCase: %s ------ Done (Passed:%s | Failed:%s | Remaining:%s | Total:%s)" % (
-                #             testcase.__name__,
-                #             len(TestCaseExecutor.passed_testcases),
-                #             len(TestCaseExecutor.failed_testcases),
-                #             len(TestCaseExecutor.testcase_queue),
-                #             self.total_testcases_count))
-                #
-                # except BaseException:
-                #     pass
-
                 try:
                     if hasattr(executing_testcase, "teardown"):
                         executing_testcase.logger.info("------ execute teardown() Start")
                         executing_testcase.teardown()
                         executing_testcase.logger.info("------ execute teardown() End")
                 except BaseException as e:
                     executing_testcase.logger.error(e)
@@ -1186,40 +1126,14 @@
                                         project_info.output_folder, ".") \
                                                                     + os.sep + browser + "_" + \
                                                                     executing_testcase.screenshot_name
                                 elif executing_testcase.rerun_tag == 1:
                                     executing_testcase.rerun_screenshot = testcase_full_folder.replace(
                                         project_info.output_folder,
                                         ".") + os.sep + "_" + executing_testcase.screenshot_name
-                                # if executing_testcase.ExecutionStatusSetByFramework == "failed":
-                                #     webdriver.save_screenshot(
-                                #         testcase_full_folder + os.sep + webdriver.name + "_" + browser + "_" +
-                                #         executing_testcase.screenshot_name)
-                                #     executing_testcase.screenshot_path_list_for_db.append(
-                                #         testcase_full_folder + os.sep + webdriver.name + "_" + browser + "_" +
-                                #         executing_testcase.screenshot_name)
-                                # elif hasattr(settings, "SaveScreenshotForPassedTestCaseFlag"):
-                                #     if settings.SaveScreenshotForPassedTestCaseFlag is True:
-                                #         webdriver.save_screenshot(
-                                #             testcase_full_folder + os.sep + webdriver.name + "_" + browser + "_" +
-                                #             executing_testcase.screenshot_name)
-                                #         executing_testcase.screenshot_path_list_for_db.append(
-                                #             testcase_full_folder + os.sep + webdriver.name + "_" + browser + "_" +
-                                #             executing_testcase.screenshot_name)
-                                #
-                                # if executing_testcase.rerun_tag == 0:
-                                #     executing_testcase.screenshot = testcase_full_folder.replace(
-                                #         project_info.output_folder, ".") \
-                                #                                     + os.sep + webdriver.name + "_" + browser + "_" + \
-                                #                                     executing_testcase.screenshot_name
-                                # elif executing_testcase.rerun_tag == 1:
-                                #     executing_testcase.rerun_screenshot = testcase_full_folder.replace(
-                                #         project_info.output_folder,
-                                #         ".") + os.sep + webdriver.name + "_" + browser + "_" + \
-                                #                                           executing_testcase.screenshot_name
                             except BaseException:
                                 traceback.print_exc()
                             finally:
                                 try:
                                     is_appium_installed = True
                                     try:
                                         import appium
@@ -1291,45 +1205,14 @@
                             len(TestCaseExecutor.passed_testcases),
                             len(TestCaseExecutor.failed_testcases),
                             len(TestCaseExecutor.testcase_queue),
                             self.total_testcases_count))
 
                 except BaseException:
                     pass
-                # #log_memory_usage("start to generate html report", executing_testcase)
-                # # if settings.DEBUG_RUN is True then will not generate report.html after each testcase execution done
-                # # and will get a better performance because no "report_lock".
-                # if settings.DEBUG_RUN is False:
-                #     # if settings.DEBUG_RUN is False and
-                #     #   1. testcase got passed   or
-                #     #   2. testcase got failed but rerun_tag == 1 and settings.RERUN_FLAG is True   or
-                #     #   3. testcase got failed and settings.RERUN_FLAG is False
-                #     # then: generate the html report after each testcase execution done!
-                #     if testcase in TestCaseExecutor.passed_testcases or \
-                #             (settings.RERUN_FLAG is True and
-                #              testcase in TestCaseExecutor.failed_testcases and testcase.rerun_tag == 1) \
-                #             or \
-                #             (settings.RERUN_FLAG is False and testcase in TestCaseExecutor.failed_testcases):
-                #         pass
-                #
-                #         # with TestCaseExecutor.report_lock:
-                #         #     try:
-                #         #         # print(self.begin_time)
-                #         #         html_report.Reporter(self.output_folder,
-                #         #                              TestCaseExecutor.passed_testcases,
-                #         #                              TestCaseExecutor.failed_testcases,
-                #         #                              TestCaseExecutor.error_testcases,
-                #         #                              self.begin_time,
-                #         #                              PLATFORM_INFO,
-                #         #                              True)
-                #         #     except BaseException:
-                #         #         traceback.print_exc()
-                #         #         print(traceback.format_exc())
-                #
-                # #log_memory_usage("after generate the html report", executing_testcase)
 
 
 def kill_process_by_name(process_name):
     for i in range(5):
         try:
             if platform.system() == "Windows":
                 subprocess.check_output("taskkill /f /im %s" % process_name, shell=True, stderr=subprocess.STDOUT)
@@ -1379,41 +1262,32 @@
 
     Note:
         the argv must be like "key=val key2=val2", each argv split by white-space and the key is case-insensitive
 
     @author: Wang Lin
     """
 
-    import sys
     import os
 
-    # from linktest.get_project_info import get_project_info
     from .get_project_info import get_project_info
 
-    # os.environ["LINK_TEST_PROJECT_PATH"] = os.path.dirname(os.path.abspath(__file__))
-    # sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
-
     project_info = get_project_info()
-
-    # todo: self.project_path = project_info.project_path
     settings_file_path = project_info.project_path + os.sep + "settings" + os.sep + "__init__.py"
 
-    # argv_list = sys.argv[1:]
     argv_list = []
 
     for item in args.split("&"):
         item = item.lstrip().rstrip()
         if item.find("=") != -1:
             argv_list.append(item)
 
     if len(argv_list) > 0:
         for argv in argv_list:
             if "=" not in argv:
                 print("the argv must like: key=val")
-                # raise BaseException("the argv must like: key=val")
 
         argv_dict = {}
         updated_argv = []
 
         for argv in argv_list:
             if (argv.find("=") != -1):
                 argv_dict[argv.split("=")[0].lstrip().rstrip()] = argv.split("=")[1].lstrip().rstrip()
@@ -1444,25 +1318,18 @@
             for argv in argv_dict.keys():
                 if argv not in updated_argv:
                     argv_list_not_found.append(argv)
 
             print("***************** WARNING: below argv not found in settings/__init__.py *****************")
             print(argv_list_not_found)
 
-        # with open(settings_file_path, "r") as settings_file:
-
         try:
             importlib.reload(settings)
         except BaseException:
             traceback.print_exc()
-        # else:
-        #     try:
-        #         exec("from %s import %s as testcase_list_for_package" % (package_name, testcase_list_string))
-        #     except BaseException:
-        #         traceback.format_exc()
 
 
 def run_with(args=None):
     """
     the args for func run_with(args=None) support below 3 types:
         1. None
             e.g: main.run_with()
@@ -1489,15 +1356,14 @@
     """
     print("====== init args:")
     print(args)
 
     if args is None:
         args = []
     elif isinstance(args, str):
-        # args = ags.split()
         args = args.replace("{ ", "{").replace(" }", "}").replace(": ", ":").replace(" :", ":").replace(", ", ",").replace(" ,", ",").split()
     elif isinstance(args, list):
         for argv in args:
             if not isinstance(argv, str):
                 raise TypeError(run_with.func_doc)
     else:
         raise TypeError(run_with.func_doc)
@@ -1550,16 +1416,14 @@
                 project_id = value.lstrip().rstrip()
             elif item == 'CALLBACK_API' or item == 'CALLBACKAPI':
                 callback_api = value.lstrip().rstrip()
             elif item == 'CASEID' or item == "CASE_ID" or item == "TESTCASE_ID" or item == "TESTCASEID":
                 case_id = value.lstrip().rstrip()
             elif item == 'CASEINDEX' or item == "CASE_INDEX":
                 case_index = value.lstrip().rstrip()
-            # elif item == 'PROJECTID' or item == "PROJECT_ID":
-            #     project_id = value.lstrip().rstrip()
             elif item == 'PRIORITY':
                 priority = value.lstrip().rstrip()
                 priority = int(priority)
             else:
                 update_config_str += "%s=%s &" % (item.lstrip().rstrip(), value)
 
     print("type(execution_id):", type(execution_id))
@@ -1628,15 +1492,14 @@
             for arg in args_init:
                 if arg.find("=") == -1:
                     args.append(arg)
         else:
             #说明命令行中有传入priority=XXX参数，则走根据 priority 执行的流程
             args.append("tests") #此处直接把所有的tests加入参数中，后面再根据priority过滤
 
-
     print(" ======== final args:")
     print(args)
 
     if len(args) < 1:
         usage()
         return
 
@@ -1758,67 +1621,67 @@
                 tag_name = None
 
                 if argument == "quick_run":
                     continue  # todo: break? then quick_run can be the first argument, if break here, quick_run must be the last argument
 
                 try:
                     if argument.__contains__("."):
-                        print("****** Warning: there are '.' in tag {tag}, here replace '.' as '_' ".format(tag=argument))
-                        tag_name = argument.replace(".", "_").lower()
+                        print("Warning: there are '.' in tag {tag}, here replace '.' as '_' ".format(tag=argument))
+                        tag_name = argument.replace(".", "_")
                     else:
-                        tag_name = argument.lower()
+                        tag_name = argument
 
                     # first try to find the argument as a tag name
                     if isinstance(testcase_dict_for_tags[tag_name], list):
                         for testcase_for_tag in testcase_dict_for_tags[tag_name]:
                             testcase_list.append(testcase_for_tag)
 
                     elif issubclass(testcase_dict_for_tags[tag_name], base_testcase.BaseTestCase):
                         testcase_list.append(testcase_dict_for_tags[tag_name])
 
-                    print("------ Found TAG: %s" % tag_name)
+                    print("******** Found TAG: %s" % tag_name)
 
                 except KeyError:
                     # it no tag name found from testcases then try to search it as a TestcaseClassName
                     try:
-                        testcase_list.append(testcase_dict_for_classname[argument.lower()])
+                        testcase_list.append(testcase_dict_for_classname[argument])
 
-                        print("------ Found TestcaseClassName: %s" % argument)
+                        print("******** Found TestcaseClassName: %s" % argument)
 
                     except KeyError:
                         # if no TestcaseClassName found from testcases then try to search it as a TestcaseList
                         try:
-                            if isinstance(testcase_dict_for_package[argument.lower()], list):
+                            if isinstance(testcase_dict_for_package[argument], list):
 
-                                for testcase_for_package in testcase_dict_for_package[argument.lower()]:
+                                for testcase_for_package in testcase_dict_for_package[argument]:
                                     testcase_list.append(testcase_for_package)
 
-                            print("------ Found TestcaseList: %s" % argument)
+                            print("******** Found TestcaseList: %s" % argument)
 
                         except KeyError:
                             try:
-                                if argument.lower().__contains__("."):
-                                    package_name = argument.lower().replace(".", "_") + "_testcases"
+                                if argument.__contains__("."):
+                                    package_name = argument.replace(".", "_") + "_testcases"
 
                                     if isinstance(testcase_dict_for_package[package_name], list):
 
                                         for testcase_for_package in testcase_dict_for_package[package_name]:
                                             testcase_list.append(testcase_for_package)
 
-                                    print("------ Found Package: %s" % argument)
+                                    print("******** Found Package: %s" % argument)
 
                                 elif argument == "tests":
                                     package_name = argument + "_testcases"
 
                                     if isinstance(testcase_dict_for_package[package_name], list):
 
                                         for testcase_for_package in testcase_dict_for_package[package_name]:
                                             testcase_list.append(testcase_for_package)
 
-                                    print("------ Found Package: %s" % argument)
+                                    print("******** Found Package: %s" % argument)
                                 else:
                                     print('''
 ****** ERROR: NO Tag/TestcaseClassName/TestcaseList/Package: '%s' Found in testcases!
 Tips:
     If you are sure that there are no spelling errors, there are two possible reasons for not finding the corresponding case:
     1. The tag in the testcase script contains "ignore"
     2. run_test() is not implemented in the testcase script''' % argument)
@@ -1967,17 +1830,14 @@
 
         if total_testcases_count == 0:
             print("\n\n\n++++++++++++++++++++++++++++ No testcases will be executed! ++++++++++++++++++++++++++++\n"
                                      "Please execute CMD 'python3 run.py --help' for more info :) ")
             return
 
         if non_backend_testcase_count > 0:
-            # if non_backend_testcase_count <= thread_pool_size:
-            #     thread_pool_size = non_backend_testcase_count
-
             import multiprocessing
             if thread_pool_size > multiprocessing.cpu_count() * 2:
                 thread_pool_size = multiprocessing.cpu_count() * 2
                 print("So many Non_Backend testcases concurrently run, here set the thread_pool_size = (2 * cpu_count:%s = %s)" % (
                         multiprocessing.cpu_count(), 2 * multiprocessing.cpu_count()))
 
         if total_testcases_count < thread_pool_size:
@@ -2075,15 +1935,14 @@
                         execution_time = end_time - begin_time
 
                         database_helper.insert_execution_summary_log(
                             execution_id=output_folder.split(os.sep + "output" + os.sep)[1],
                             environment=settings.ENVIRONMENT,
                             os=PLATFORM_INFO,
                             automation_framework_version=linktest.__version__,
-                            # total_execution_time=convert_to_seconds(execution_time),
                             total_execution_time=execution_time,
                             jenkins_job_name=None,
                             project_name=project_info.project_name,
                             total_testcases_count=total_testcases_count,
                             pass_testcases_count=len(TestCaseExecutor.passed_testcases),
                             fail_testcases_count=total_testcases_count - len(TestCaseExecutor.passed_testcases),
                             rerun_flag=1 if settings.RERUN_FLAG else 0
@@ -2091,21 +1950,14 @@
             except BaseException:
                 traceback.print_exc()
             finally:
                 pass
 
         print(os.linesep + "=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
 
-        # try:
-        #     import webbrowser
-        #     # webbrowser.open_new("file:///" + output_folder + os.sep + "report.html")
-        #     # webbrowser.open_new("http://127.0.0.1:5000/")
-        # except BaseException:
-        #     traceback.print_exc()
-
         if hasattr(settings, "COPY_REPORT_TO_SPECIFIED_PATH"):
             if settings.COPY_REPORT_TO_SPECIFIED_PATH is True:
                 if not hasattr(settings, "SPECIFIED_REPORT_PATH") or not hasattr(settings, "SPECIFIED_REPORT_HOST_IP") \
                         or not hasattr(settings, "SPECIFIED_REPORT_HOST_PORT") or not hasattr(settings,
                                                                                               "SPECIFIED_REPORT_HOST_USERNAME") \
                         or not hasattr(settings, "SPECIFIED_REPORT_HOST_PASSWORD"):
                     raise Exception("如果 COPY_REPORT_TO_SPECIFIED_PATH = True, 则必须设置：SPECIFIED_REPORT_PATH & "
@@ -2128,31 +1980,14 @@
                 #     else:
                 #         print("文件上传成功" + output_folder)
                 #     finally:
                 #         ssh_client.close()
 
                 # scp_report_to_specified_path(output_folder)
 
-        # print("====++++++++++======")
-        # print(len(BaseTestCase.GlobalExecutedCaseList))
-        # print(BaseTestCase.GlobalExecutedCaseList)
-        # print(BaseTestCase.GlobalExecutedCaseList[-1])
-        # print(BaseTestCase.GlobalExecutedCaseList[-1].logfile_full_name)
-
-        # 如下这段被注释的逻辑需要再enhance一下， 比如：如果 logContent本身就包含了'[' or ']'
-        # last_done_case_log_time = "2015"
-        # last_done_case = None
-        # for executed_case in BaseTestCase.GlobalExecutedCaseList[-10:]:
-        #     last_time = executed_case.execution_log.split("]")[0].split("[")[1]
-        #     if last_time > last_done_case_log_time:
-        #         last_done_case_log_time = last_time
-        #         last_done_case_path = executed_case.logfile_full_name
-        #         last_done_case = executed_case
-        #
-
         # 如果最后执行完所有的testcase 并且GlobalDataList 不为空，则自动保存GlobalDataList
         if len(BaseTestCase.GlobalDataList) > 0:
             try:
                 with open(output_folder + os.sep + "global_data_list.txt", "w") as f:
                     f.write(str(BaseTestCase.GlobalDataList))
 
                 with open(output_folder + os.sep + "global_data_list.py", "w") as f:
```

### Comparing `linktest-2.0.2/linktest/memory_usage.py` & `linktest-2.0.3/lintest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/run.py` & `linktest-2.0.3/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/run_testcase_thread.py` & `linktest-2.0.3/lintest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/scp_report_to_specified_path.py` & `linktest-2.0.3/lintest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/selenium_helper.py` & `linktest-2.0.3/lintest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/timeout_thread.py` & `linktest-2.0.3/lintest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/ui_testcase.py` & `linktest-2.0.3/lintest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/update_config.py` & `linktest-2.0.3/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/linktest/xml_report.py` & `linktest-2.0.3/lintest/xml_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import socket
 import datetime
 import traceback
 
 try:
-    import linktest
+    import lintest
 except ImportError:
     traceback.print_exc()
 
 
 def convert_to_seconds(t):
     try:
         s_time = str(t)
@@ -33,17 +33,17 @@
     execution_time = end_time - begin_time
 
     with open(output_folder + os.sep + "xunitresults.xml", "w", encoding='utf-8') as xml_file:
         pass_count = len(passed_testcases)
         fail_count = len(failed_testcases)
 
         xml_file.write(
-            "<testsuite failures='%s' tests='%s' name='Automation Run' hostname='%s' time='%s' timestamp='%s' type='linktest_%s'>\n" % (
+            "<testsuite failures='%s' tests='%s' name='Automation Run' hostname='%s' time='%s' timestamp='%s' type='lintest_%s'>\n" % (
                 fail_count, pass_count + fail_count, socket.getfqdn(), execution_time, begin_time,
-                linktest.__version__))
+                lintest.__version__))
 
         for failed_testcase in failed_testcases:
             xml_file.write("    <testcase classname='%s' name='%s' time='%s' status='fail'>\n" % (
                 failed_testcase.__module__, failed_testcase.__class__.__name__,
                 failed_testcase.execution_time))
 
             # the value of xml's attribute must not contains the "<" or ">" character, here replace "<" to "&lt;" and
```

### Comparing `linktest-2.0.2/linktest.egg-info/SOURCES.txt` & `linktest-2.0.3/linktest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 setup.py
 linktest/__init__.py
 linktest/android_testcase.py
 linktest/api_testcase.py
 linktest/appium_utils.py
-linktest/auto_generate_test_suite.py
 linktest/auto_generate_testcase_list.py
 linktest/auto_generate_testcase_list_from_csv.py
-linktest/auto_organize_testcase.py
 linktest/base_testcase.py
 linktest/clean_data.py
 linktest/conver_xml_into_db.py
 linktest/database_helper.py
 linktest/date_utilities.py
 linktest/doctor.py
 linktest/framework_log.py
```

### Comparing `linktest-2.0.2/lintest/appium_utils.py` & `linktest-2.0.3/lintest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/auto_generate_testcase_list.py` & `linktest-2.0.3/linktest/auto_generate_testcase_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
-This module is used to:
- 1. generate the testcase list in init.py files under tests package according what testcases the package include
- 2. generate the testcase list by tag names under settings/tag_testcases
-
-Created on Aug. 5, 2018
+This module serves to:
+1. Generate the test case list in init.py files within the 'tests' package, based on the included test cases.
+2. Create the test case list by tag names under the 'settings/tag_testcases' directory.
 
 @author: Wang Lin
 """
 
 import os
 import time
 import shutil
@@ -23,20 +21,17 @@
 import importlib
 
 from collections import OrderedDict
 from . import get_project_info
 from . import android_testcase
 from .get_adb_devices import get_adb_devices
 from .clean_data import clear_init_file, remove_android_temp
-from .doctor import doctor_check
 from .android_testcase import AndroidTestCase
 from .base_testcase import BaseTestCase
 
-from .memory_usage import log_memory_usage
-
 ANDROID_TESTCASE_PACKAGE_NAME = "android"
 ANDROID_TESTCASE_TEMP_PACKAGE_NAME = "android_temp"
 REAL_DEVICE = android_testcase.AndroidTestCase.REAL_DEVICE
 VIRTUAL_DEVICE = android_testcase.AndroidTestCase.VIRTUAL_DEVICE
 APPIUM_SERVER_PORT = int(getattr(settings, 'APPIUM_SERVER_DEFAULT_PORT', 4723))
 
 PROJECT_INFO = get_project_info.get_project_info()
@@ -48,16 +43,16 @@
 clear_init_file()
 
 try:
     exec("from tests.ignore_testcases_list import IgnoreTestCases")
 except BaseException:
     print("\nWARNING: No IgnoreTestcases list found from your project\n")
 
-    # if the IgnoreTestCases doesn't exists. here define a new list to store all the testcases which has "ignore"
-    # tag, will ignore these "ignored" testcases when auto generate the testcases list in __init__.py files .
+    # If IgnoreTestCases doesn't exist, define a new list to store all test cases with the "ignore" tag.
+    # These "ignored" test cases will be excluded when auto-generating the test case list in __init__.py files.
     IgnoreTestCases = []
 
 
 def generate_testcase_list(testcase_dict):
     if os.path.exists(TAG_TESTCASES_DIRECTORY):
         shutil.rmtree(TAG_TESTCASES_DIRECTORY)
 
@@ -98,25 +93,25 @@
     file_full_name = PROJECT_INFO.project_path + os.sep + file_full_name
     import_string_list = []
     class_name_list = []
     contains_run_test = False
     contains_tag_flag = False
 
     with open(file_full_name, "r", encoding='utf-8') as file_object:
-        # if there are no "tag" found in the file content, then will not add this testcase into testcase_dict_for_tags
+        # If no "tag" is found in the file content, the test case will not be added to the testcase_dict_for_tags.
         for line in file_object:
             if line.replace(" ", "").__contains__("tag="):
                 contains_tag_flag = True
                 break
 
     with open(file_full_name, "r", encoding='utf-8') as file_object:
-        # if there are no run_test() or runTest() method found in the file content, then this file not a TestCase file
+        # If neither the run_test() nor runTest() method is found in the file content, then this file is not considered a TestCase file.
         for line in file_object:
             if line.__contains__("def ") and (
-                        line.__contains__("run_test(") or line.__contains__("runTest(")) and line.__contains__(":") \
+                    line.__contains__("run_test(") or line.__contains__("runTest(")) and line.__contains__(":") \
                     and not line.strip().startswith("#"):
                 contains_run_test = True
                 break
 
     if contains_run_test is True:
         with open(file_full_name, "r", encoding='utf-8') as file_object:
 
@@ -143,19 +138,21 @@
                             import_base_class_flag = True
                             break
 
                     if import_base_class_flag is False:
                         break
 
                     namespace = {}
-                    exec(import_string,namespace)  # this line must be exits(TestcaseA extends from CheckoutTestcase which is subclass of FrontendTestCase
+
+                    # This line must exist: TestcaseA inherits from CheckoutTestcase, which is a subclass of UITestCase.
+                    exec(import_string, namespace)
                     exec("base_class_name = %s" % base_class_name_string, namespace)
                     base_class_name = namespace['base_class_name']
 
-                    # if base_class_name is not the subclass of BaseTestCase, then this class is not a TestCase Class
+                    # If base_class_name is not a subclass of BaseTestCase, then this class is not considered a TestCase class.
                     if not issubclass(base_class_name, BaseTestCase):
                         break
 
                     module_path_str = file_full_name.split(PROJECT_INFO.project_path)[1]
                     module_path_str = module_path_str.replace(os.sep, ".")
                     module_path_str = module_path_str.replace(".tests.", "tests.")
                     module_path_str = module_path_str.strip()
@@ -219,15 +216,15 @@
                             testcase_dict_for_tags["ignore"].append(testcase)
                     else:
                         class_name_list.append(class_name)
 
     return class_name_list
 
 
-def generate_andoid_testcase_temp_packages(android_testcases_package_list):
+def generate_android_testcase_temp_packages(android_testcases_package_list):
     for package_name in android_testcases_package_list:
         package_name = package_name.split(".android.")[1]
         name_list = package_name.split(".")
 
         new_package_path = TESTS_PACKAGE_PATH + os.sep + ANDROID_TESTCASE_TEMP_PACKAGE_NAME
 
         for name in name_list:
@@ -245,18 +242,18 @@
 
 def get_class_name_list(file_full_name):
     import_string_list = []
     class_name_list = []
     contains_run_test = False
 
     with open(file_full_name, "r", encoding='utf-8') as file_object:
-        # if there are no run_test() or runTest() method found in the file content, then this file not a TestCase file
+        # If neither the run_test() nor runTest() method is found in the file content, then this file is not considered a TestCase file.
         for line in file_object:
             if line.__contains__("def ") and (
-                        line.__contains__("run_test(") or line.__contains__("runTest(")) and line.__contains__(":") \
+                    line.__contains__("run_test(") or line.__contains__("runTest(")) and line.__contains__(":") \
                     and not line.strip().startswith("#"):
                 contains_run_test = True
                 break
 
     if contains_run_test is True:
         with open(file_full_name, "r", encoding='utf-8') as file_object:
 
@@ -269,15 +266,16 @@
                     class_name_string, base_class_name_string = line.split("(")
                     class_name = class_name_string.split(" ")[-1]
                     class_name_list.append(class_name)
 
     return class_name_list
 
 
-def generate_testcase_by_device(device_name, file_full_name, file_name, directory_path, d_device_account, appium_server_port):
+def generate_testcase_by_device(device_name, file_full_name, file_name, directory_path, d_device_account,
+                                appium_server_port):
     user_name = d_device_account[device_name][0]
     password = d_device_account[device_name][1]
 
     if device_name.__contains__("."):
         device_name_for_new_testcase = "virtual_device_%s" % device_name.replace(".", "_").replace(":", "_")
     else:
         device_name_for_new_testcase = "real_device_%s" % device_name
@@ -339,15 +337,14 @@
             i += 1
 
         with open(new_testcase_file_full_name, "w", encoding='utf-8') as new_testcase_file:
             new_testcase_file.writelines(contents)
 
 
 def auto_generate_testcase_list(call_by_doctor=False):
-    log_memory_usage("start to auto_generate_testcase_list")
     test_cases_dict = {PROJECT_INFO.testcase_package_name: []}
     testcase_dict_for_tags = {}
     testcase_dict_for_classname = {}
     testcase_package_name_list = []
     testcase_dict_for_package = {}
     android_testcases_path = TESTS_PACKAGE_PATH + os.sep + "android"
     new_android_testcases_package_list = []
@@ -411,15 +408,15 @@
                     new_directory_path = new_directory_path.replace(PROJECT_INFO.project_path + os.sep, "")
                     new_directory_path = new_directory_path.replace(os.sep, ".")
                     new_android_testcases_package_list.append(new_directory_path)
 
             with open(ANDROID_TEMP_PACKAGE_PATH + os.sep + "__init__.py", "w"):
                 pass
 
-            generate_andoid_testcase_temp_packages(new_android_testcases_package_list)
+            generate_android_testcase_temp_packages(new_android_testcases_package_list)
 
             for directory_path, directory_names, file_names in os.walk(android_testcases_path, topdown=True):
 
                 for file_name in file_names:
                     if file_name.endswith(".py") and file_name != "__init__.py":
                         file_full_name = os.path.join(directory_path, file_name)
                         class_name_list = get_class_name_list(file_full_name)
@@ -518,56 +515,53 @@
 
                 if class_names.index(class_name) < (len(class_names) - 1):
                     file_obj.write(",")
                     file_obj.write("\n")
 
             file_obj.write("\n]\n")
 
-            # py_compile.compile(init_file) # todo: can i remove this line ?
+            # py_compile.compile(init_file) # todo
 
     # generate testcase_list which group by tag name
     generate_testcase_list(testcase_dict_for_tags)
 
     for key in test_cases_dict.keys():
         if key == "tests.tag_testcases":
             continue
 
         testcase_package_name_list.append(key)
 
     for package_name in testcase_package_name_list:
         testcase_list_string = package_name.replace(".", "_") + "_testcases"
 
         try:
-            # print("-------- start reload: ", package_name)
-            # print(sys.modules)
-            # because the context in the tests/xxx/__init__.py files were auto generated, here must reload the tests_xxx_testcases
-            # note: must use reload, use import_module(package_name) will not work.
+            # Since the context in the tests/xxx/__init__.py files is auto-generated, tests_xxx_testcases must be reloaded.
+            # Note: Use 'reload' instead of 'import_module(package_name)', as the latter will not work.
             importlib.reload(sys.modules[package_name])
-            # importlib.import_module(package_name)
         except KeyError:
             print("Ignored file: %s" % package_name)
         else:
             try:
                 exec("from %s import %s as testcase_list_for_package" % (package_name, testcase_list_string))
                 exec("testcase_dict_for_package[testcase_list_string] = testcase_list_for_package")
             except BaseException:
                 traceback.format_exc()
 
     if len(device_list) > 0 and (call_by_doctor is False):
         if "tests.android" in testcase_package_name_list:
 
-            # "there are android testcases found, so here copy android_temp to android ..."
+            # "Android test cases have been found, so here we copy android_temp to android..."
             for package_name in testcase_package_name_list:
                 if package_name.__contains__(".android."):
                     new_package_name = package_name.replace(".android.", ".%s." % ANDROID_TESTCASE_TEMP_PACKAGE_NAME)
                     try:
                         testcase_dict_for_package[package_name.replace(".", "_") + "_testcases"] = \
                             testcase_dict_for_package[new_package_name.replace(".", "_") + "_testcases"]
                     except KeyError:
-                        # KeyError means that there are no testcase found under the package_name, just ignore it
+                        # A KeyError indicates that no test case was found under the package_name; it can be safely ignored.
                         pass
 
                 elif package_name == "tests.android":
                     testcase_dict_for_package["tests_android_testcases"] = testcase_dict_for_package[
                         "tests_android_temp_testcases"]
 
     if os.path.exists(ANDROID_TEMP_PACKAGE_PATH):
@@ -617,37 +611,8 @@
             init_file = TESTS_PACKAGE_PATH + os.sep + ANDROID_TESTCASE_TEMP_PACKAGE_NAME + os.sep + "__init__.py"
             py_compile.compile(init_file)
 
             importlib.reload(sys.modules["tests.%s" % ANDROID_TESTCASE_TEMP_PACKAGE_NAME])
             exec("from tests.%s import tests_android_temp_testcases" % ANDROID_TESTCASE_TEMP_PACKAGE_NAME)
             exec("testcase_dict_for_tags['full_matrix'] = tests_android_temp_testcases")
 
-    log_memory_usage("after execute auto_generate_testcase_list")
     return testcase_dict_for_tags, testcase_dict_for_classname, testcase_dict_for_package
-#
-# if __name__ == "__main__":
-#     # before generate the testcase list, call doctor_check() to check the necessary configuration files.
-#     doctor_check()
-#
-#     testcase_dict_for_tags, testcase_dict_for_classname, testcase_dict_for_package = auto_generate_testcase_list()
-#
-#     print("*" * 60)
-#     print("the testcase list which auto organized by tag name under: %s" % TAG_TESTCASES_DIRECTORY)
-#     print("*" * 60)
-#
-#     if len(testcase_dict_for_tags.keys()) > 0:
-#         print("\n---------------------- below is the testcase list group by tag name: ----------------------")
-#
-#         for key in testcase_dict_for_tags.keys():
-#             print("tag_name: %s," % key, " count:%s, " % len(testcase_dict_for_tags[key]), testcase_dict_for_tags[key])
-#
-#     if len(testcase_dict_for_classname) > 0:
-#         print("\n---------------------- below is the testcase list group by class name: ----------------------")
-#
-#         for key, val in testcase_dict_for_classname.items():
-#             print(key, ":", val)
-#
-#     if testcase_dict_for_package.items() > 0:
-#         print("\n---------------------- below is the testcase list group by package name: ----------------------")
-#
-#         for key, val in testcase_dict_for_package.items():
-#             print(key, ", count:%s " % len(val), val)
```

### Comparing `linktest-2.0.2/lintest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.3/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,87 +1,54 @@
 """
 This module is used to:
-  auto generate the testcase list by the .csv & related .py file
+  Auto-generate the test case list based on the .csv and corresponding .py files.
 
+If you need to use a dataSet (currently only supporting CSV format), please define it as follows:
+  1. Create a CSV file using a comma (",") as the separator.
+  2. In the same directory as the CSV file, create a .py file with the same name. This .py file must define a `run_test(self, param...)` method.
 
-如果需要使用 dataSet(目前只支持CSV格式）,请按照如下方式定义：
-    1. 定义一个 csv文件, 必须使用","作为分隔符
-    2. 在csv文件的同级目录下定义一个 和csv文件同名的.py文件，py文件中必须定义一个 run_test(self, param...)方法
-    参考如下：
-       1. testLogin.csv 文件如下：
-           channel,username,password
-            web,"admin1","admin1"
-            web,admin2,"admin2"
-            web,user1,user2
-            app,admin1,admin1
-            app,admin2,admin2
-
-       2. testLogin.py文件内容如下：
-            from common.test_login import login # 引入的具体业务逻辑处理方法
-
-            def run_my_test(self, username, password, channel): # 定义接受的参数（此处接收的参数都必须定义在csv中--列名）
-                self.logger.info("start run_test()...")
-                login(self, username, password, channel)
-
-      -----> 如果正确运行后，框架会根据 testLogin.csv & testLogin.py 自动生成符合框架运行标准的 auto_generated_by_csv.py文件（testLogin_case_list_auto_generated_by_csv.py）
-        注意：和__init__.py文件类似，每次执行，都会根据相应的 .csv & .py文件自动生成最新的 auto_generated_by_csv.py文件
-      testLogin_case_list_auto_generated_by_csv.py 内容如下：
-
-        from lintest.api_testcase import APITestCase
-        from tests.api.csv_dataset import testLoginDataSet
-
-
-        class testLoginDataSet_1(APITestCase):
-            tag = "testLoginDataSet"
-
-            def run_test(self):
-                username = 'admin1'
-                password = 'admin1'
+For example:
+  1. testLogin.csv file content:
+        username,password
+        user1,password1
+        user2,password2
 
-                testLoginDataSet.run_test(self, username, password)
-
-
-        class testLoginDataSet_2(APITestCase):
-            tag = "testLoginDataSet"
+  2. testLogin.py file content:
+        from common.test_login import login  # Import the specific business logic handling method
 
-            def run_test(self):
-                username = 'admin2'
-                password = 'admin2'
+        def run_my_test(self, username, password):  # Define the received parameters (parameters must be defined in the CSV columns)
+            self.logger.info("start run_test()...")
+            login(self, username, password)
 
-                testLoginDataSet.run_test(self, username, password)
-
-
-        class testLoginDataSet_3(APITestCase):
-            tag = "testLoginDataSet"
-
-            def run_test(self):
-                username = 'user1'
-                password = 'user2'
+  -----> If executed correctly, the framework will generate a file (testLogin_case_list_auto_generated_by_csv.py) that conforms to the framework's running standards based on testLogin.csv and testLogin.py.
 
-                testLoginDataSet.run_test(self, username, password)
+  Note: Similar to the __init__.py file, each time the script is executed, it will generate the latest auto_generated_by_csv.py file based on the corresponding .csv and .py files.
 
+  The content of testLogin_case_list_auto_generated_by_csv.py:
 
-        class testLoginDataSet_4(APITestCase):
-            tag = "testLoginDataSet"
+      from linktest.api_testcase import APITestCase
+      from tests.api.csv_dataset import testLoginDataSet
 
-            def run_test(self):
-                username = 'admin1'
-                password = 'admin1'
+      class testLoginDataSet_1(APITestCase):
+          tag = "testLoginDataSet"
 
-                testLoginDataSet.run_test(self, username, password)
+          def run_test(self):
+              username = 'user1'
+              password = 'password1'
 
+              testLoginDataSet.run_test(self, username, password)
 
-        class testLoginDataSet_5(APITestCase):
-            tag = "testLoginDataSet"
+      class testLoginDataSet_2(APITestCase):
+          tag = "testLoginDataSet"
 
-            def run_test(self):
-                username = 'admin2'
-                password = 'admin2'
+          def run_test(self):
+              username = 'user2'
+              password = 'password2'
 
-                testLoginDataSet.run_test(self, username, password)
+              testLoginDataSet.run_test(self, username, password)
 
 @author: Wang Lin
 """
 
 import os
 import csv
 import traceback
@@ -129,15 +96,15 @@
                         self.logger.info("start run_test()...") 
                         login(self, username, password, channel)
                         
               -----> 如果正确运行后，框架会根据 testLogin.csv & testLogin.py 自动生成符合框架运行标准的 auto_generated_by_csv.py文件（testLogin_case_list_auto_generated_by_csv.py）
                 注意：和__init__.py文件类似，每次执行，都会根据相应的 .csv & .py文件自动生成最新的 auto_generated_by_csv.py文件
               testLogin_case_list_auto_generated_by_csv.py 内容如下：
               
-                from lintest.api_testcase import APITestCase
+                from linktest.api_testcase import APITestCase
                 from tests.api.csv_dataset import testLoginDataSet
                 
                 
                 class testLoginDataSet_1(APITestCase):
                     tag = "testLoginDataSet"
                 
                     def run_test(self):
@@ -280,15 +247,15 @@
                 self.logger.info("start run_test()...")
                 login(self, username, password, channel)
 
       -----> 如果正确运行后，框架会根据 testLogin.csv & testLogin.py 自动生成符合框架运行标准的 auto_generated_by_csv.py文件（testLogin_case_list_auto_generated_by_csv.py）
         注意：和__init__.py文件类似，每次执行，都会根据相应的 .csv & .py文件自动生成最新的 auto_generated_by_csv.py文件
       testLogin_case_list_auto_generated_by_csv.py 内容如下：
 
-        from lintest.api_testcase import APITestCase
+        from linktest.api_testcase import APITestCase
         from tests.api.csv_dataset import testLoginDataSet
 
 
         class testLoginDataSet_1(APITestCase):
             tag = "testLoginDataSet"
 
             def run_test(self):
@@ -357,23 +324,23 @@
                         for line in py_file_obj.readlines():
                             if line.replace(" ", "").startswith("self.browser."):
                                 is_ui_testcase = True
                                 # 导入 UTTestCase
                                 with open(PROJECT_INFO.project_path + os.sep + directory_path + os.sep +
                                           file_name.split(".")[
                                               0] + "_case_list_auto_generated_by_csv.py", "a") as f:
-                                    f.write("from lintest.ui_testcase import UITestCase")
+                                    f.write("from linktest.ui_testcase import UITestCase")
                                 break
 
                     if not is_ui_testcase:
                         # 导入 UTTestCase
                         with open(PROJECT_INFO.project_path + os.sep + directory_path + os.sep +
                                   file_name.split(".")[
                                       0] + "_case_list_auto_generated_by_csv.py", "a") as f:
-                            f.write("from lintest.api_testcase import APITestCase")
+                            f.write("from linktest.api_testcase import APITestCase")
 
                     csv_file_full_path = PROJECT_INFO.project_path + os.sep + directory_path + os.sep + \
                                          file_name.split('.')[0] + ".csv"
 
 
                     # 解析 py 文件, 判断文件中是否有 tag = "tagName" 有则说明需要 为自动生成的testcase 同时设置用户自定义的 tagName
                     tag_name = ''
```

### Comparing `linktest-2.0.2/lintest/auto_organize_testcase.py` & `linktest-2.0.3/linktest/run_testcase_thread.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,47 @@
-"""
-This module is to organize all the testcases into different groups(such as: "smoke", "nightly", "ignore" and "regression")
-
-Testcase Demo: (below testcase will be added into smoke and nightly group)
-
-class TestBackend1(BackendTestCase):
-    execute_tag = "smoke, nightly"
-
-    def run_test(self):
-        self.test_case_id = "BackendTC-1"
-        self.logger.debug("start to run backend test case 1")
-
-@author: Wang Lin
-"""
-
-import os
+import threading
 import traceback
+import datetime
 
-try:
-    from tests import tests_testcases
-except ImportError:
-    traceback.print_exc()
-
-
-def generate_testcase_list(testcase_dict):
-    for key in testcase_dict.keys():
-        if key == "regression":
-            continue
-
-        values = testcase_dict.get(key)
-        with open((".." + os.path.sep + "tests" + os.path.sep + "%s.py") % key, "w") as file_obj:
-            file_obj.write("import tests")
-            file_obj.write(os.linesep)
-            file_obj.write(os.linesep)
-
-            file_obj.write("%s_run_testcase_list = [%s" % (key, os.linesep))
-
-            for value in values:
-                file_obj.write("    " + value.__module__ + "." + value.__name__)
-                file_obj.write("," + os.linesep)
-
-            file_obj.write("]")
-
-
-def auto_organize_testcase(testcase_list):
-    tag_list = []
-    testcase_dict = {}
-
-    for testcase in testcase_list:
-        if hasattr(testcase, "tag"):
-            tags = testcase.tag.lower().split(",")
-            for tag in tags:
-                if tag.strip() not in tag_list:
-                    tag_list.append(tag.strip())
-
-    for tag in tag_list:
-        testcase_dict[tag] = []
-
-    for testcase in testcase_list:
-        if hasattr(testcase, "tag"):
-            testcase_tags = testcase.tag.lower().split(",")
-            for tag in testcase_tags:
-                testcase_dict[tag.strip()].append(testcase)
-
-    generate_testcase_list(testcase_dict)
-
-    return testcase_dict
-
+from .base_testcase import BaseTestCase
 
-if __name__ == "__main__":
-    testcase_dict = auto_organize_testcase(tests_testcases)
 
-    for key in testcase_dict.keys():
-        if key != "regression":
-            print
-            key, " : ", testcase_dict[key]
+class StartTestcaseThread(threading.Thread):
+    """
+    StartTestcaseThread is used to call the testcase's runTest()/run_test() method,
+    and will set the testcases's done_flag as "True" after execution done without any exception.
+
+    @author: Wang Lin
+    """
+
+    def __init__(self, executing_testcase):
+        threading.Thread.__init__(self)
+        self.executing_testcase = executing_testcase
+
+    def run(self):
+        # 先执行 setup()， 再执行 run_test()
+
+        self.executing_testcase.testcase_start_time = datetime.datetime.now()
+
+        try:
+            # 执行 setup() 之前 先 log TestEngineCaseInput(如果是由 test-engine 发起的)
+            if BaseTestCase.TestEngineCaseInput:
+                self.executing_testcase.logger.info("------ TestEngineCaseInput:")
+                self.executing_testcase.logger.info(self.executing_testcase.TestEngineCaseInput)
+
+            if hasattr(self.executing_testcase, "setup"):
+                self.executing_testcase.logger.info("------ execute setup() Start")
+                self.executing_testcase.setup()
+                self.executing_testcase.logger.info("------ execute setup() End")
+
+            if hasattr(self.executing_testcase, "runTest"):
+                print("the method runTest() is deprecated, please re-name it as run_test()")
+                self.executing_testcase.logger.info("================== runTest() start:")
+                self.executing_testcase.runTest()
+            else:
+                self.executing_testcase.logger.info("================== run_test() start:")
+                self.executing_testcase.run_test()
+        except BaseException:
+            traceback.print_exc()
+            self.executing_testcase.exception_info = traceback.format_exc()
+        else:
+            self.executing_testcase.done_flag = True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linktest-2.0.2/lintest/base_testcase.py` & `linktest-2.0.3/linktest/base_testcase.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class BaseTestCase(object):
     """
 BaseTestCase is the superclass for all the backend(Non UI) and frontend(UI) Testcases and Mobile Testcases
 @author: Wang Lin
 """
 
-    # TestEngineCaseInput 即 TestEngineCaseInput from gitHub Action (test-engine目前只支持单线程)
+    # TestEngineCaseInput from gitHub Action (test-engine目前只支持单线程)
     TestEngineCaseInput = {}
 
     # GlobalObjData 是全局数据对象（各个不同的thread发起的不同的testcase直接共享该数据）
     GlobalObjData = {}
 
     # 框架提供的全局数据列表: GlobalDataList
     GlobalDataList = []
@@ -60,15 +60,15 @@
 
         # # todo: 此处用于 构建多线程时 每个线程独立的 TestEngineCaseInput(线程id作为key)
         # print("===================+++++++++++++==========threading.currentThread().ident")
         # print(threading.currentThread().ident)
 
         # self.CaseData 用于记录 case执行过程中产生的数据（多数情况用于 某个 testcase chain中, 某个Testcase中有调用了 另外一个Testcase.run_test() 则此case 被定义一个 TestcaseChain）
         # eg:
-        # from lintest.api_testcase import APITestCase
+        # from linktest.api_testcase import APITestCase
         # from tests.api.testcase_demo.testcase1 import Testcase1
         # from tests.api.testcase_demo.testcase2 import Testcase2
         #
         # class Testcase3(APITestCase):
         #     tag = 'case3'
         #
         #     def run_test(self):
@@ -177,24 +177,24 @@
             self.logger.info("assert_is_not_none(%s)  -- Failed" % (actual_val))
             raise
 
     def compare_json_and_return_diff(self, expected_json, actual_json, rules=None):
         """
         此方法 比较两个 json 时会忽略结构体内item的顺序,即如下 json1 & json2 会被认为是相同的
         json1 = {
-            "name": "lintest",
+            "name": "linktest",
             "Company": {
                 "name": "IKEA",
                 "No": 1
             },
             "version": "1.0"
         }
         json2 = {
             "version": "1.0",
-            "name": "lintest",
+            "name": "linktest",
             "Company": {
                 "name": "IKEA",
                 "No": 1
             }
         }
         """
 
@@ -217,15 +217,15 @@
 
     def compare_json_and_assert_equal(self, expected_json, actual_json, rules=None):
         diff = self.compare_json_and_return_diff(expected_json, actual_json, rules)
         self.pprint(diff)
         assert diff == {}
 
     def compare_json_with_strict_mode(self, expected_json, actual_json):
-        """不会忽略json体内Item的顺序, 即: { "name": "lintest", "version": 1.0 } 和 {"version": 1.0, "name": "lintest" } 是不同的, 本质上就是当做字符串来比较"""
+        """不会忽略json体内Item的顺序, 即: { "name": "linktest", "version": 1.0 } 和 {"version": 1.0, "name": "linktest" } 是不同的, 本质上就是当做字符串来比较"""
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> compare_json_with_strict_mode: ")
         v1 = json.dumps(expected_json, sort_keys=False)
         v2 = json.dumps(actual_json, sort_keys=False)
 
         self.logger.info("------ expected_json: ")
         self.logger.info(self.pformat(v1))
@@ -235,30 +235,7 @@
 
         print("------ expected_json: ")
         self.pprint(v1)
         print("------ actual_json: ")
         self.pprint(v2)
 
         assert v1 == v2
-
-    # def compare_json_with_strict_mode(self, expected_json, actual_json):
-    #     """不会忽略json体内Item的顺序, 即: { "name": "lintest", "version": 1.0 } 和 {"version": 1.0, "name": "lintest" } 是不同的"""
-    #
-    #     self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> compare_json_with_strict_mode: ")
-    #     self.logger.info("------ expected_json: ")
-    #     self.logger.info(self.pformat(expected_json))
-    #     self.logger.info("------ actual_json: ")
-    #     self.logger.info(self.pformat(actual_json))
-    #
-    #     # from collections import OrderedDict
-    #     # def sorting(item):
-    #     #     if isinstance(item, dict):
-    #     #         return sorted((key, sorting(values)) for key, values in item.items())
-    #     #     if isinstance(item, list):
-    #     #         return sorted(sorting(x) for x in item)
-    #     #     else:
-    #     #         return item
-    #     #
-    #
-    #     diff = self.compare_json_and_return_diff(json.loads(json.dumps(expected_json, sort_keys=False)),
-    #                                              json.loads(json.dumps(actual_json, sort_keys=False)))
-    #     assert diff == {}
```

### Comparing `linktest-2.0.2/lintest/clean_data.py` & `linktest-2.0.3/linktest/clean_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-module clean_data.py is used to:
-1. clear all the __init__.py file which under tests package
+The clean_data.py module is used to:
+1. Clear all the __init__.py files under the 'tests' package.
 2. remove all the .pyc files which under tests package
 
 @author: Wang Lin
 """
 import os
 import time
 import shutil
```

### Comparing `linktest-2.0.2/lintest/conver_xml_into_db.py` & `linktest-2.0.3/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/database_helper.py` & `linktest-2.0.3/linktest/database_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-database_helper.py is used to save the lintest's execution's logs
+The database_helper.py module is used to save the logs of test case script execution into the specified database.
 
 @author: Wang Lin
 """
 import os
 import socket
 import traceback
 import pymysql
```

### Comparing `linktest-2.0.2/lintest/date_utilities.py` & `linktest-2.0.3/linktest/date_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import calendar
 import datetime
 
 
 def add_months(date_time, month):
     """
-    according to the business logic, we need get the previous several months date.
+    get the previous several months date.
+
     @author: Wang Lin
     """
     if month <= 0:
         if abs(month) <= 12:
             if date_time.month < abs(month):
                 new_year = date_time.year - 1
                 if abs(month) > 12:
```

### Comparing `linktest-2.0.2/lintest/doctor.py` & `linktest-2.0.3/lintest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/get_adb_devices.py` & `linktest-2.0.3/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/get_ios_devices_list.py` & `linktest-2.0.3/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/get_platform_info.py` & `linktest-2.0.3/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/get_project_info.py` & `linktest-2.0.3/lintest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/html_report.py` & `linktest-2.0.3/lintest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/logged_requests.py` & `linktest-2.0.3/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/main.py` & `linktest-2.0.3/lintest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/memory_usage.py` & `linktest-2.0.3/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/run.py` & `linktest-2.0.3/lintest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/scp_report_to_specified_path.py` & `linktest-2.0.3/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/selenium_helper.py` & `linktest-2.0.3/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/timeout_thread.py` & `linktest-2.0.3/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/ui_testcase.py` & `linktest-2.0.3/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/update_config.py` & `linktest-2.0.3/lintest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.2/lintest/xml_report.py` & `linktest-2.0.3/linktest/xml_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 import socket
 import datetime
 import traceback
 
 try:
-    import lintest
+    import linktest
 except ImportError:
     traceback.print_exc()
 
 
 def convert_to_seconds(t):
     try:
         s_time = str(t)
-        # print("start to covert to seconds:" + s_time)
         if "." in s_time:
             s_time, ms = s_time.split(".")
             ms = "0." + ms
         else:
             ms = 0
         h, m, s = s_time.split(":")
         h, m, s = int(h), int(m), int(s)
@@ -33,17 +32,17 @@
     execution_time = end_time - begin_time
 
     with open(output_folder + os.sep + "xunitresults.xml", "w", encoding='utf-8') as xml_file:
         pass_count = len(passed_testcases)
         fail_count = len(failed_testcases)
 
         xml_file.write(
-            "<testsuite failures='%s' tests='%s' name='Automation Run' hostname='%s' time='%s' timestamp='%s' type='lintest_%s'>\n" % (
+            "<testsuite failures='%s' tests='%s' name='Automation Run' hostname='%s' time='%s' timestamp='%s' type='linktest_%s'>\n" % (
                 fail_count, pass_count + fail_count, socket.getfqdn(), execution_time, begin_time,
-                lintest.__version__))
+                linktest.__version__))
 
         for failed_testcase in failed_testcases:
             xml_file.write("    <testcase classname='%s' name='%s' time='%s' status='fail'>\n" % (
                 failed_testcase.__module__, failed_testcase.__class__.__name__,
                 failed_testcase.execution_time))
 
             # the value of xml's attribute must not contains the "<" or ">" character, here replace "<" to "&lt;" and
```

