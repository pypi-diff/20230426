# Comparing `tmp/gvm_tools-23.3.0.tar.gz` & `tmp/gvm_tools-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvm_tools-23.3.0.tar", max compression
+gzip compressed data, was "gvm_tools-23.4.0.tar", max compression
```

## Comparing `gvm_tools-23.3.0.tar` & `gvm_tools-23.4.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0    35141 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/LICENSE
--rw-r--r--   0        0        0     6665 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/README.md
--rw-r--r--   0        0        0     1134 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/__init__.py
--rw-r--r--   0        0        0      103 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/__version__.py
--rw-r--r--   0        0        0     4334 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/cli.py
--rw-r--r--   0        0        0     2796 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/config.py
--rw-r--r--   0        0        0     6271 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/helper.py
--rw-r--r--   0        0        0    10623 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/parser.py
--rw-r--r--   0        0        0     5325 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/pyshell.py
--rw-r--r--   0        0        0     3576 2023-03-22 11:57:56.752462 gvm_tools-23.3.0/gvmtools/script.py
--rw-r--r--   0        0        0     2192 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/pyproject.toml
--rw-r--r--   0        0        0    14437 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/.pylintrc
--rw-r--r--   0        0        0    11534 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/README.md
--rw-r--r--   0        0        0     2064 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/application-detection.gmp.py
--rw-r--r--   0        0        0     2680 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/bulk-modify-schedules.gmp.py
--rw-r--r--   0        0        0     3418 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/cfg-gen-for-certs.gmp.py
--rw-r--r--   0        0        0    42608 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/check-gmp.gmp.py
--rw-r--r--   0        0        0     3012 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/clean-sensor.gmp.py
--rw-r--r--   0        0        0     4075 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/combine-reports.gmp.py
--rwxr-xr-x   0        0        0    11544 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/create-consolidated-report.gmp.py
--rw-r--r--   0        0        0    19339 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/create-cve-report-from-json.gmp.py
--rw-r--r--   0        0        0     2854 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/create-dummy-data.gmp.py
--rw-r--r--   0        0        0     4769 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/create-targets-from-host-list.gmp.py
--rw-r--r--   0        0        0    28306 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/default_report_data.json
--rw-r--r--   0        0        0     1981 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/delete-overrides-by-filter.gmp.py
--rw-r--r--   0        0        0     2784 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/export-pdf-report.gmp.py
--rw-r--r--   0        0        0    15103 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/generate-random-reports.gmp.py
--rw-r--r--   0        0        0     2359 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/generate-random-targets.gmp.py
--rw-r--r--   0        0        0     1398 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/list-tasks.gmp.py
--rw-r--r--   0        0        0     3681 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/monthly-report-gos4.gmp.py
--rw-r--r--   0        0        0     4294 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/monthly-report.gmp.py
--rw-r--r--   0        0        0     3686 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/nvt-scan.gmp.py
--rw-r--r--   0        0        0      111 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/requirements.txt
--rw-r--r--   0        0        0     3205 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/scan-new-system.gmp.py
--rw-r--r--   0        0        0     7586 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/send-delta-emails.gmp.py
--rw-r--r--   0        0        0     2449 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/send-schedules.gmp.py
--rw-r--r--   0        0        0     4459 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/send-targets.gmp.py
--rw-r--r--   0        0        0     5899 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/send-tasks.gmp.py
--rw-r--r--   0        0        0    11403 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/start-alert-scan.gmp.py
--rw-r--r--   0        0        0     8859 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/start-multiple-alerts-scan.gmp.py
--rw-r--r--   0        0        0     5589 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/start-nvt-scan.gmp.py
--rw-r--r--   0        0        0     2423 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/sync-hosts.gmp.py
--rw-r--r--   0        0        0     4952 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/scripts/update-task-target.gmp.py
--rw-r--r--   0        0        0     1639 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1236 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/root_help.3.10.snap
--rw-r--r--   0        0        0     1247 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/root_help.snap
--rw-r--r--   0        0        0     2103 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/__init__.py
--rw-r--r--   0        0        0     7637 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/example_schedules.xml
--rw-r--r--   0        0        0     9980 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/example_target.xml
--rw-r--r--   0        0        0     5830 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/example_task.xml
--rw-r--r--   0        0        0     2869 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/get_alerts.xml
--rw-r--r--   0        0        0     4325 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/get_scan_configs.xml
--rw-r--r--   0        0        0      921 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/invalid_xml.xml
--rw-r--r--   0        0        0     7411 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/test_combine_reports.py
--rw-r--r--   0        0        0    16064 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/test_create_consolidated_report.py
--rw-r--r--   0        0        0     2390 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/test_send_schedules.py
--rw-r--r--   0        0        0     3687 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/test_send_targets.py
--rw-r--r--   0        0        0     3397 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/test_send_tasks.py
--rw-r--r--   0        0        0     7095 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/scripts/test_start_alert_scan.py
--rw-r--r--   0        0        0      361 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/socket_help.3.10.snap
--rw-r--r--   0        0        0      372 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/socket_help.snap
--rw-r--r--   0        0        0      522 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/ssh_help.3.10.snap
--rw-r--r--   0        0        0      533 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/ssh_help.snap
--rw-r--r--   0        0        0      214 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/test.cfg
--rw-r--r--   0        0        0       41 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/test_auth.cfg
--rw-r--r--   0        0        0     3446 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/test_config.py
--rw-r--r--   0        0        0     8732 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/test_helper.py
--rw-r--r--   0        0        0    17368 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/test_parser.py
--rw-r--r--   0        0        0      776 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/tls_help.3.10.snap
--rw-r--r--   0        0        0      787 2023-03-22 11:57:56.756462 gvm_tools-23.3.0/tests/tls_help.snap
--rw-r--r--   0        0        0     8121 1970-01-01 00:00:00.000000 gvm_tools-23.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/LICENSE
+-rw-r--r--   0        0        0     6665 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/README.md
+-rw-r--r--   0        0        0     1134 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/__version__.py
+-rw-r--r--   0        0        0     4334 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/cli.py
+-rw-r--r--   0        0        0     2796 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/config.py
+-rw-r--r--   0        0        0     6305 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/helper.py
+-rw-r--r--   0        0        0    10948 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/parser.py
+-rw-r--r--   0        0        0     5325 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/pyshell.py
+-rw-r--r--   0        0        0     3576 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/gvmtools/script.py
+-rw-r--r--   0        0        0     2192 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0    14437 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/.pylintrc
+-rw-r--r--   0        0        0    11534 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/README.md
+-rw-r--r--   0        0        0     2064 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/application-detection.gmp.py
+-rw-r--r--   0        0        0     2680 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/bulk-modify-schedules.gmp.py
+-rw-r--r--   0        0        0     3418 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/cfg-gen-for-certs.gmp.py
+-rw-r--r--   0        0        0    42608 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/check-gmp.gmp.py
+-rw-r--r--   0        0        0     3012 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/clean-sensor.gmp.py
+-rw-r--r--   0        0        0     4075 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/combine-reports.gmp.py
+-rwxr-xr-x   0        0        0    11544 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/create-consolidated-report.gmp.py
+-rw-r--r--   0        0        0    19339 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/create-cve-report-from-json.gmp.py
+-rw-r--r--   0        0        0     2854 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/create-dummy-data.gmp.py
+-rw-r--r--   0        0        0     4769 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/create-targets-from-host-list.gmp.py
+-rw-r--r--   0        0        0    28306 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/default_report_data.json
+-rw-r--r--   0        0        0     1981 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/delete-overrides-by-filter.gmp.py
+-rw-r--r--   0        0        0     2784 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/export-pdf-report.gmp.py
+-rw-r--r--   0        0        0    15103 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/generate-random-reports.gmp.py
+-rw-r--r--   0        0        0     2359 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/generate-random-targets.gmp.py
+-rw-r--r--   0        0        0     1398 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/list-tasks.gmp.py
+-rw-r--r--   0        0        0     3681 2023-04-26 13:21:29.413986 gvm_tools-23.4.0/scripts/monthly-report-gos4.gmp.py
+-rw-r--r--   0        0        0     4294 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/monthly-report.gmp.py
+-rw-r--r--   0        0        0     3686 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/nvt-scan.gmp.py
+-rw-r--r--   0        0        0      111 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/requirements.txt
+-rw-r--r--   0        0        0     3205 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/scan-new-system.gmp.py
+-rw-r--r--   0        0        0     7586 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/send-delta-emails.gmp.py
+-rw-r--r--   0        0        0     2449 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/send-schedules.gmp.py
+-rw-r--r--   0        0        0     4459 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/send-targets.gmp.py
+-rw-r--r--   0        0        0     5899 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/send-tasks.gmp.py
+-rw-r--r--   0        0        0    11403 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/start-alert-scan.gmp.py
+-rw-r--r--   0        0        0     8859 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/start-multiple-alerts-scan.gmp.py
+-rw-r--r--   0        0        0     5589 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/start-nvt-scan.gmp.py
+-rw-r--r--   0        0        0     2423 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/sync-hosts.gmp.py
+-rw-r--r--   0        0        0     4952 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/scripts/update-task-target.gmp.py
+-rw-r--r--   0        0        0     1639 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1236 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/root_help.3.10.snap
+-rw-r--r--   0        0        0     1247 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/root_help.snap
+-rw-r--r--   0        0        0     2103 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     7637 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/example_schedules.xml
+-rw-r--r--   0        0        0     9980 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/example_target.xml
+-rw-r--r--   0        0        0     5830 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/example_task.xml
+-rw-r--r--   0        0        0     2869 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/get_alerts.xml
+-rw-r--r--   0        0        0     4325 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/get_scan_configs.xml
+-rw-r--r--   0        0        0      921 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/invalid_xml.xml
+-rw-r--r--   0        0        0     7411 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/test_combine_reports.py
+-rw-r--r--   0        0        0    16064 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/test_create_consolidated_report.py
+-rw-r--r--   0        0        0     2390 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/test_send_schedules.py
+-rw-r--r--   0        0        0     3687 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/test_send_targets.py
+-rw-r--r--   0        0        0     3397 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/test_send_tasks.py
+-rw-r--r--   0        0        0     7095 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/scripts/test_start_alert_scan.py
+-rw-r--r--   0        0        0      361 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/socket_help.3.10.snap
+-rw-r--r--   0        0        0      372 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/socket_help.snap
+-rw-r--r--   0        0        0      656 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/ssh_help.3.10.snap
+-rw-r--r--   0        0        0      667 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/ssh_help.snap
+-rw-r--r--   0        0        0      214 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/test.cfg
+-rw-r--r--   0        0        0       41 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/test_auth.cfg
+-rw-r--r--   0        0        0     3446 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/test_config.py
+-rw-r--r--   0        0        0     8732 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/test_helper.py
+-rw-r--r--   0        0        0    17368 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/test_parser.py
+-rw-r--r--   0        0        0      776 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/tls_help.3.10.snap
+-rw-r--r--   0        0        0      787 2023-04-26 13:21:29.417986 gvm_tools-23.4.0/tests/tls_help.snap
+-rw-r--r--   0        0        0     8121 1970-01-01 00:00:00.000000 gvm_tools-23.4.0/PKG-INFO
```

### Comparing `gvm_tools-23.3.0/LICENSE` & `gvm_tools-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/README.md` & `gvm_tools-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/gvmtools/__init__.py` & `gvm_tools-23.4.0/gvmtools/__init__.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/gvmtools/cli.py` & `gvm_tools-23.4.0/gvmtools/cli.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/gvmtools/config.py` & `gvm_tools-23.4.0/gvmtools/config.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/gvmtools/helper.py` & `gvm_tools-23.4.0/gvmtools/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,30 +85,30 @@
                 row_columns.append(self._create_column(column, column_size))
 
             row_strings.append(self._create_row(row_columns))
 
         return "\n".join(row_strings)
 
 
-def yes_or_no(question):
+def yes_or_no(question: str) -> bool:
     """Asks the user to proceed or not in a gvmtools script
 
     Arguments:
         question (str): The condition the user should answer
     """
     reply = str(input(question + " (y/n): ")).lower().strip()
     if reply[0] == ("y"):
         return True
     if reply[0] == ("n"):
         return False
     else:
         return yes_or_no("Please enter 'y' or 'n'")
 
 
-def error_and_exit(msg):
+def error_and_exit(msg: str) -> None:
     """Prints an error message and quits the gvmtools script
 
     Arguments:
         msg (str): The error message, that will be printed
     """
     print(f"\nError: {msg}\n", file=sys.stderr)
     sys.exit(1)
@@ -196,15 +196,15 @@
         gmp.authenticate(username, password)
         return (username, password)
     except GvmError as e:
         print("Could not authenticate. Please check your credentials.")
         raise e
 
 
-def run_script(path, global_vars):
+def run_script(path, global_vars) -> None:
     """Loads and executes a file as a python script
 
     Arguments:
         path (str): Path to the script file
         vars (dict): Variables passed as globals to the script
     """
     try:
```

### Comparing `gvm_tools-23.3.0/gvmtools/parser.py` & `gvm_tools-23.4.0/gvmtools/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 """Command Line Interface Parser
 """
 
 import argparse
 import logging
 from pathlib import Path
+from typing import Optional
 
 from gvm import get_version as get_gvm_version
 from gvm.connections import (
     DEFAULT_TIMEOUT,
     SSHConnection,
     TLSConnection,
     UnixSocketConnection,
@@ -44,15 +45,15 @@
 PROTOCOL_OSP = "OSP"
 PROTOCOL_GMP = "GMP"
 DEFAULT_PROTOCOL = PROTOCOL_GMP
 
 
 class CliParser:
     def __init__(
-        self, description, logfilename, *, prog=None, ignore_config=False
+        self, description: str, logfilename, *, prog=None, ignore_config=False
     ):
         bootstrap_parser = argparse.ArgumentParser(
             prog=prog,
             description=description,
             formatter_class=argparse.RawTextHelpFormatter,
             # don't parse help initially. the args from parser wouldn't be shown
             add_help=False,
@@ -207,14 +208,20 @@
         )
         parser_ssh.add_argument(
             "--ssh-username", help="SSH username (default: %(default)r)"
         )
         parser_ssh.add_argument(
             "--ssh-password", help="SSH password (default: %(default)r)"
         )
+        parser_ssh.add_argument(
+            "-A",
+            "--auto-accept-host",
+            action="store_true",
+            help="When executed in e.g. CI, auto accept SSH host addition",
+        )
 
         parser_tls = self._subparsers.add_parser(
             "tls", help="Use TLS secured connection to connect to service"
         )
         parser_tls.add_argument(
             "--hostname", help="Hostname or IP address (default: %(default)s)"
         )
@@ -310,14 +317,15 @@
     hostname=None,
     port=None,
     certfile=None,
     keyfile=None,
     cafile=None,
     ssh_username=None,
     ssh_password=None,
+    auto_accept_host: Optional[bool] = None,
     **kwargs,  # pylint: disable=unused-argument
 ):
     if "socket" in connection_type:
         return UnixSocketConnection(timeout=timeout, path=socketpath)
 
     if "tls" in connection_type:
         return TLSConnection(
@@ -331,8 +339,9 @@
 
     return SSHConnection(
         timeout=timeout,
         hostname=hostname,
         port=port,
         username=ssh_username,
         password=ssh_password,
+        auto_accept_host=auto_accept_host,
     )
```

### Comparing `gvm_tools-23.3.0/gvmtools/pyshell.py` & `gvm_tools-23.4.0/gvmtools/pyshell.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/gvmtools/script.py` & `gvm_tools-23.4.0/gvmtools/script.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/pyproject.toml` & `gvm_tools-23.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "gvm-tools"
-version = "23.3.0"
+version = "23.4.0"
 authors = ["Greenbone AG <info@greenbone.net>"]
 description = "Tools to control a GSM/GVM over GMP or OSP"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/gvm-tools/"
 repository = "https://github.com/greenbone/gvm-tools/"
 documentation = "https://greenbone.github.io/gvm-tools/"
@@ -47,15 +47,15 @@
 autohooks-plugin-pylint = ">=22.8.1"
 autohooks-plugin-black = ">=22.8.1"
 autohooks-plugin-isort = ">=22.8.0"
 pontos = ">=22.8.1"
 sphinx = "^5.3.0"
 coverage = "^7.2"
 rope = "^1.7.0"
-furo = "^2022.12.7"
+furo = "^2023.3.27"
 
 [tool.black]
 line-length = 80
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 exclude = '''
 /(
     \.git
```

### Comparing `gvm_tools-23.3.0/scripts/.pylintrc` & `gvm_tools-23.4.0/scripts/.pylintrc`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/README.md` & `gvm_tools-23.4.0/scripts/README.md`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/application-detection.gmp.py` & `gvm_tools-23.4.0/scripts/application-detection.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/bulk-modify-schedules.gmp.py` & `gvm_tools-23.4.0/scripts/bulk-modify-schedules.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/cfg-gen-for-certs.gmp.py` & `gvm_tools-23.4.0/scripts/cfg-gen-for-certs.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/check-gmp.gmp.py` & `gvm_tools-23.4.0/scripts/check-gmp.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/clean-sensor.gmp.py` & `gvm_tools-23.4.0/scripts/clean-sensor.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/combine-reports.gmp.py` & `gvm_tools-23.4.0/scripts/combine-reports.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/create-consolidated-report.gmp.py` & `gvm_tools-23.4.0/scripts/create-consolidated-report.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/create-cve-report-from-json.gmp.py` & `gvm_tools-23.4.0/scripts/create-cve-report-from-json.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/create-dummy-data.gmp.py` & `gvm_tools-23.4.0/scripts/create-dummy-data.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/create-targets-from-host-list.gmp.py` & `gvm_tools-23.4.0/scripts/create-targets-from-host-list.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/default_report_data.json` & `gvm_tools-23.4.0/scripts/default_report_data.json`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/delete-overrides-by-filter.gmp.py` & `gvm_tools-23.4.0/scripts/delete-overrides-by-filter.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/export-pdf-report.gmp.py` & `gvm_tools-23.4.0/scripts/export-pdf-report.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/generate-random-reports.gmp.py` & `gvm_tools-23.4.0/scripts/generate-random-reports.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/generate-random-targets.gmp.py` & `gvm_tools-23.4.0/scripts/generate-random-targets.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/list-tasks.gmp.py` & `gvm_tools-23.4.0/scripts/list-tasks.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/monthly-report-gos4.gmp.py` & `gvm_tools-23.4.0/scripts/monthly-report-gos4.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/monthly-report.gmp.py` & `gvm_tools-23.4.0/scripts/monthly-report.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/nvt-scan.gmp.py` & `gvm_tools-23.4.0/scripts/nvt-scan.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/scan-new-system.gmp.py` & `gvm_tools-23.4.0/scripts/scan-new-system.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/send-delta-emails.gmp.py` & `gvm_tools-23.4.0/scripts/send-delta-emails.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/send-schedules.gmp.py` & `gvm_tools-23.4.0/scripts/send-schedules.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/send-targets.gmp.py` & `gvm_tools-23.4.0/scripts/send-targets.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/send-tasks.gmp.py` & `gvm_tools-23.4.0/scripts/send-tasks.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/start-alert-scan.gmp.py` & `gvm_tools-23.4.0/scripts/start-alert-scan.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/start-multiple-alerts-scan.gmp.py` & `gvm_tools-23.4.0/scripts/start-multiple-alerts-scan.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/start-nvt-scan.gmp.py` & `gvm_tools-23.4.0/scripts/start-nvt-scan.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/sync-hosts.gmp.py` & `gvm_tools-23.4.0/scripts/sync-hosts.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/scripts/update-task-target.gmp.py` & `gvm_tools-23.4.0/scripts/update-task-target.gmp.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/__init__.py` & `gvm_tools-23.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/root_help.3.10.snap` & `gvm_tools-23.4.0/tests/root_help.3.10.snap`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/root_help.snap` & `gvm_tools-23.4.0/tests/root_help.snap`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/__init__.py` & `gvm_tools-23.4.0/tests/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/example_schedules.xml` & `gvm_tools-23.4.0/tests/scripts/example_schedules.xml`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/example_target.xml` & `gvm_tools-23.4.0/tests/scripts/example_target.xml`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/example_task.xml` & `gvm_tools-23.4.0/tests/scripts/example_task.xml`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/get_alerts.xml` & `gvm_tools-23.4.0/tests/scripts/get_alerts.xml`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/get_scan_configs.xml` & `gvm_tools-23.4.0/tests/scripts/get_scan_configs.xml`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/invalid_xml.xml` & `gvm_tools-23.4.0/tests/scripts/invalid_xml.xml`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/test_combine_reports.py` & `gvm_tools-23.4.0/tests/scripts/test_combine_reports.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/test_create_consolidated_report.py` & `gvm_tools-23.4.0/tests/scripts/test_create_consolidated_report.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/test_send_schedules.py` & `gvm_tools-23.4.0/tests/scripts/test_send_schedules.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/test_send_targets.py` & `gvm_tools-23.4.0/tests/scripts/test_send_targets.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/test_send_tasks.py` & `gvm_tools-23.4.0/tests/scripts/test_send_tasks.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/scripts/test_start_alert_scan.py` & `gvm_tools-23.4.0/tests/scripts/test_start_alert_scan.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/ssh_help.3.10.snap` & `gvm_tools-23.4.0/tests/ssh_help.3.10.snap`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 usage: gvm-test-cli ssh [-h] [--hostname HOSTNAME] [--port PORT]
                         [--ssh-username SSH_USERNAME]
-                        [--ssh-password SSH_PASSWORD]
+                        [--ssh-password SSH_PASSWORD] [-A]
 
 options:
   -h, --help            show this help message and exit
   --hostname HOSTNAME   Hostname or IP address (default: 127.0.0.1)
   --port PORT           SSH port (default: 22)
   --ssh-username SSH_USERNAME
                         SSH username (default: 'gmp')
   --ssh-password SSH_PASSWORD
                         SSH password (default: 'gmp')
+  -A, --auto-accept-host
+                        When executed in e.g. CI, auto accept SSH host
+                        addition
```

### Comparing `gvm_tools-23.3.0/tests/ssh_help.snap` & `gvm_tools-23.4.0/tests/ssh_help.snap`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 usage: gvm-test-cli ssh [-h] [--hostname HOSTNAME] [--port PORT]
                         [--ssh-username SSH_USERNAME]
-                        [--ssh-password SSH_PASSWORD]
+                        [--ssh-password SSH_PASSWORD] [-A]
 
 optional arguments:
   -h, --help            show this help message and exit
   --hostname HOSTNAME   Hostname or IP address (default: 127.0.0.1)
   --port PORT           SSH port (default: 22)
   --ssh-username SSH_USERNAME
                         SSH username (default: 'gmp')
   --ssh-password SSH_PASSWORD
                         SSH password (default: 'gmp')
+  -A, --auto-accept-host
+                        When executed in e.g. CI, auto accept SSH host
+                        addition
```

### Comparing `gvm_tools-23.3.0/tests/test_config.py` & `gvm_tools-23.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/test_helper.py` & `gvm_tools-23.4.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/test_parser.py` & `gvm_tools-23.4.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/tls_help.3.10.snap` & `gvm_tools-23.4.0/tests/tls_help.3.10.snap`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/tests/tls_help.snap` & `gvm_tools-23.4.0/tests/tls_help.snap`

 * *Files identical despite different names*

### Comparing `gvm_tools-23.3.0/PKG-INFO` & `gvm_tools-23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvm-tools
-Version: 23.3.0
+Version: 23.4.0
 Summary: Tools to control a GSM/GVM over GMP or OSP
 Home-page: https://github.com/greenbone/gvm-tools/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

