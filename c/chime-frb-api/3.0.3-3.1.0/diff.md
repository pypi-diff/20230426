# Comparing `tmp/chime_frb_api-3.0.3.tar.gz` & `tmp/chime_frb_api-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chime_frb_api-3.0.3.tar", max compression
+gzip compressed data, was "chime_frb_api-3.1.0.tar", max compression
```

## Comparing `chime_frb_api-3.0.3.tar` & `chime_frb_api-3.1.0.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0     1080 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/LICENSE
--rw-r--r--   0        0        0     1386 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/README.md
--rw-r--r--   0        0        0      277 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/backends/__init__.py
--rw-r--r--   0        0        0      352 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/backends/bucket.py
--rw-r--r--   0        0        0      392 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/backends/distributor.py
--rw-r--r--   0        0        0     1932 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/backends/frb_master.py
--rw-r--r--   0        0        0      784 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/cli.py
--rw-r--r--   0        0        0      328 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/configs/__init__.py
--rw-r--r--   0        0        0      136 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/configs/test_workflow.yaml
--rw-r--r--   0        0        0      917 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/configs/workflow.yaml
--rw-r--r--   0        0        0       48 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/core/__init__.py
--rw-r--r--   0        0        0    18785 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/core/core.py
--rw-r--r--   0        0        0      289 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/core/exceptions.py
--rw-r--r--   0        0        0      144 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/core/json_type.py
--rw-r--r--   0        0        0     2569 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/core/logger.py
--rw-r--r--   0        0        0      265 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/bucket.py
--rw-r--r--   0        0        0     8351 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/buckets.py
--rw-r--r--   0        0        0     4548 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/calibration.py
--rw-r--r--   0        0        0      570 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/candidates.py
--rw-r--r--   0        0        0      810 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/catalog.py
--rw-r--r--   0        0        0     4839 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/distributor.py
--rw-r--r--   0        0        0    11217 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/events.py
--rw-r--r--   0        0        0     5521 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/metrics.py
--rw-r--r--   0        0        0     2013 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/mimic.py
--rw-r--r--   0        0        0     4000 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/parameters.py
--rw-r--r--   0        0        0     4882 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/results.py
--rw-r--r--   0        0        0     1875 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/sources.py
--rw-r--r--   0        0        0    11581 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/swarm.py
--rw-r--r--   0        0        0    12551 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/tns.py
--rw-r--r--   0        0        0     1879 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/verification.py
--rw-r--r--   0        0        0    12214 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/voe.py
--rw-r--r--   0        0        0     4234 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/modules/voe_subscribers.py
--rw-r--r--   0        0        0        0 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/stations/__init__.py
--rw-r--r--   0        0        0       22 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/stations/aro.py
--rw-r--r--   0        0        0      706 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/stations/drao.py
--rw-r--r--   0        0        0       22 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/stations/gbo.py
--rw-r--r--   0        0        0     2876 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/tests/docker-compose.yml
--rw-r--r--   0        0        0     9065 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/tests/test_archive.py
--rw-r--r--   0        0        0     3423 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/tests/test_audit_daemon.py
--rw-r--r--   0        0        0     1830 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/tests/test_bucket.py
--rw-r--r--   0        0        0     4282 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/tests/test_buckets.py
--rw-r--r--   0        0        0     1764 2023-04-03 19:43:25.314650 chime_frb_api-3.0.3/chime_frb_api/tests/test_calibration.py
--rw-r--r--   0        0        0      262 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_candidates.py
--rw-r--r--   0        0        0      610 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_catalog.py
--rw-r--r--   0        0        0     3413 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_core.py
--rw-r--r--   0        0        0     2066 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_distributor.py
--rw-r--r--   0        0        0     5823 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_events.py
--rw-r--r--   0        0        0     3335 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_metrics.py
--rw-r--r--   0        0        0      960 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_mimic.py
--rw-r--r--   0        0        0      849 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_parameters.py
--rw-r--r--   0        0        0     2143 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_results.py
--rw-r--r--   0        0        0      384 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_sources.py
--rw-r--r--   0        0        0      256 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_stations.py
--rw-r--r--   0        0        0     1454 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_swarm.py
--rw-r--r--   0        0        0     7035 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_tns.py
--rw-r--r--   0        0        0     5367 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_transfer_daemon.py
--rw-r--r--   0        0        0      467 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_verification.py
--rw-r--r--   0        0        0     8503 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_voe.py
--rw-r--r--   0        0        0     2780 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_voe_subscribers.py
--rw-r--r--   0        0        0     5167 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_work.py
--rw-r--r--   0        0        0     1208 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_work_http_operations.py
--rw-r--r--   0        0        0     6497 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/utils/__init__.py
--rw-r--r--   0        0        0     2642 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/utils/copy.py
--rw-r--r--   0        0        0      859 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/utils/github.py
--rw-r--r--   0        0        0     1220 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/utils/loki.py
--rw-r--r--   0        0        0     2642 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/utils/move.py
--rw-r--r--   0        0        0       76 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/cli/__init__.py
--rw-r--r--   0        0        0     3951 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/cli/buckets.py
--rw-r--r--   0        0        0     5239 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/cli/pipelines.py
--rw-r--r--   0        0        0     7771 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/cli/run.py
--rw-r--r--   0        0        0      789 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/cli/sample.py
--rw-r--r--   0        0        0      671 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/cli/sample.yaml
--rw-r--r--   0        0        0        0 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/daemons/__init__.py
--rw-r--r--   0        0        0      980 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/daemons/audit.py
--rw-r--r--   0        0        0     6709 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/daemons/transfer.py
--rw-r--r--   0        0        0       32 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/__init__.py
--rw-r--r--   0        0        0     5101 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/archive.py
--rw-r--r--   0        0        0       33 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/attempt.py
--rw-r--r--   0        0        0     4136 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/execute.py
--rw-r--r--   0        0        0     1418 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/validate.py
--rwxr-xr-x   0        0        0      408 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/runner.py
--rw-r--r--   0        0        0    18166 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/chime_frb_api/workflow/work.py
--rw-r--r--   0        0        0     1776 2023-04-03 19:43:25.318651 chime_frb_api-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 chime_frb_api-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1386 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/README.md
+-rw-r--r--   0        0        0      277 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/backends/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/backends/bucket.py
+-rw-r--r--   0        0        0      392 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/backends/distributor.py
+-rw-r--r--   0        0        0     1932 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/backends/frb_master.py
+-rw-r--r--   0        0        0      784 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/cli.py
+-rw-r--r--   0        0        0      368 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/configs/__init__.py
+-rw-r--r--   0        0        0      136 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/configs/test_workflow.yaml
+-rw-r--r--   0        0        0     1185 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/configs/workflow.yaml
+-rw-r--r--   0        0        0       48 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/core/__init__.py
+-rw-r--r--   0        0        0    18785 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/core/core.py
+-rw-r--r--   0        0        0      289 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/core/exceptions.py
+-rw-r--r--   0        0        0      144 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/core/json_type.py
+-rw-r--r--   0        0        0     2569 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/core/logger.py
+-rw-r--r--   0        0        0      265 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/modules/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-25 18:26:50.575637 chime_frb_api-3.1.0/chime_frb_api/modules/bucket.py
+-rw-r--r--   0        0        0     8351 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/buckets.py
+-rw-r--r--   0        0        0     4548 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/calibration.py
+-rw-r--r--   0        0        0      570 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/candidates.py
+-rw-r--r--   0        0        0      810 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/catalog.py
+-rw-r--r--   0        0        0     4839 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/distributor.py
+-rw-r--r--   0        0        0    11217 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/events.py
+-rw-r--r--   0        0        0     5521 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/metrics.py
+-rw-r--r--   0        0        0     2013 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/mimic.py
+-rw-r--r--   0        0        0     4000 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/parameters.py
+-rw-r--r--   0        0        0     4882 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/results.py
+-rw-r--r--   0        0        0     1875 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/sources.py
+-rw-r--r--   0        0        0    11581 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/swarm.py
+-rw-r--r--   0        0        0    12551 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/tns.py
+-rw-r--r--   0        0        0     1879 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/verification.py
+-rw-r--r--   0        0        0    12214 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/voe.py
+-rw-r--r--   0        0        0     4234 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/modules/voe_subscribers.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/stations/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/stations/aro.py
+-rw-r--r--   0        0        0      706 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/stations/drao.py
+-rw-r--r--   0        0        0       22 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/stations/gbo.py
+-rw-r--r--   0        0        0     2876 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/docker-compose.yml
+-rw-r--r--   0        0        0     9065 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_archive.py
+-rw-r--r--   0        0        0     3423 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_audit_daemon.py
+-rw-r--r--   0        0        0     1830 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_bucket.py
+-rw-r--r--   0        0        0     4282 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_buckets.py
+-rw-r--r--   0        0        0     1764 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_calibration.py
+-rw-r--r--   0        0        0      262 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_candidates.py
+-rw-r--r--   0        0        0      610 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_catalog.py
+-rw-r--r--   0        0        0     3413 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_core.py
+-rw-r--r--   0        0        0     2066 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_distributor.py
+-rw-r--r--   0        0        0     5823 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_events.py
+-rw-r--r--   0        0        0     3335 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_metrics.py
+-rw-r--r--   0        0        0      960 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_mimic.py
+-rw-r--r--   0        0        0      849 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_parameters.py
+-rw-r--r--   0        0        0     2134 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_results.py
+-rw-r--r--   0        0        0      384 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_sources.py
+-rw-r--r--   0        0        0      256 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_stations.py
+-rw-r--r--   0        0        0     1454 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_swarm.py
+-rw-r--r--   0        0        0     7035 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_tns.py
+-rw-r--r--   0        0        0     5367 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_transfer_daemon.py
+-rw-r--r--   0        0        0      467 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_verification.py
+-rw-r--r--   0        0        0     8503 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_voe.py
+-rw-r--r--   0        0        0     2780 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_voe_subscribers.py
+-rw-r--r--   0        0        0     5167 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_work.py
+-rw-r--r--   0        0        0     1208 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_work_http_operations.py
+-rw-r--r--   0        0        0     6650 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/utils/__init__.py
+-rw-r--r--   0        0        0     2642 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/utils/copy.py
+-rw-r--r--   0        0        0      859 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/utils/github.py
+-rw-r--r--   0        0        0     1263 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/utils/loki.py
+-rw-r--r--   0        0        0     2642 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/utils/move.py
+-rw-r--r--   0        0        0       76 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/cli/__init__.py
+-rw-r--r--   0        0        0     3951 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/cli/buckets.py
+-rw-r--r--   0        0        0     5239 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/cli/pipelines.py
+-rw-r--r--   0        0        0     9107 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/cli/run.py
+-rw-r--r--   0        0        0      789 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/cli/sample.py
+-rw-r--r--   0        0        0      671 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/cli/sample.yaml
+-rw-r--r--   0        0        0        0 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/daemons/__init__.py
+-rw-r--r--   0        0        0      980 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/daemons/audit.py
+-rw-r--r--   0        0        0     6787 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/daemons/transfer.py
+-rw-r--r--   0        0        0       32 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/__init__.py
+-rw-r--r--   0        0        0     5101 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/archive.py
+-rw-r--r--   0        0        0       33 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/attempt.py
+-rw-r--r--   0        0        0      523 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/container.py
+-rw-r--r--   0        0        0     4323 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/execute.py
+-rw-r--r--   0        0        0     1418 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/validate.py
+-rwxr-xr-x   0        0        0      408 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/runner.py
+-rw-r--r--   0        0        0    18166 2023-04-25 18:26:50.579637 chime_frb_api-3.1.0/chime_frb_api/workflow/work.py
+-rw-r--r--   0        0        0     1798 2023-04-25 18:26:50.599637 chime_frb_api-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 chime_frb_api-3.1.0/PKG-INFO
```

### Comparing `chime_frb_api-3.0.3/LICENSE` & `chime_frb_api-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/README.md` & `chime_frb_api-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/backends/frb_master.py` & `chime_frb_api-3.1.0/chime_frb_api/backends/frb_master.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/cli.py` & `chime_frb_api-3.1.0/chime_frb_api/cli.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/core/core.py` & `chime_frb_api-3.1.0/chime_frb_api/core/core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/core/logger.py` & `chime_frb_api-3.1.0/chime_frb_api/core/logger.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/bucket.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/buckets.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/calibration.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/candidates.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/candidates.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/catalog.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/distributor.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/events.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/events.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/metrics.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/mimic.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/parameters.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/results.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/results.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/sources.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/sources.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/swarm.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/tns.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/verification.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/verification.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/voe.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/modules/voe_subscribers.py` & `chime_frb_api-3.1.0/chime_frb_api/modules/voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/stations/drao.py` & `chime_frb_api-3.1.0/chime_frb_api/stations/drao.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/docker-compose.yml` & `chime_frb_api-3.1.0/chime_frb_api/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_archive.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_audit_daemon.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_audit_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_bucket.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_buckets.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_calibration.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_catalog.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_core.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_distributor.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_events.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_metrics.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_mimic.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_parameters.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_results.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,30 @@
         results.deposit([work.payload])
 
 
 def test_deposit_results(results, work):
     """Test deposit results."""
     work.status = "success"
     status = results.deposit([work.payload])
-    assert status[work.pipeline] is True
+    assert status[work.pipeline] == 1
 
     response = results.view(
         pipeline=work.pipeline,
         query={"status": "success"},
         projection={"id": 1},
     )
     assert len(response) == 1
     assert response[0]["id"] == work.id
 
 
 def test_update_results(results, work):
     """Test update results."""
     work.status = "failure"
     status = results.update([work.payload])
-    assert status[work.pipeline] is True
+    assert status[work.pipeline] == 1
 
     response = results.view(
         pipeline=work.pipeline,
         query={"status": "failure"},
         projection={"id": 1, "status": 1},
     )
 
@@ -73,15 +73,15 @@
     response = results.status()
     assert response == {work.pipeline: 1}
 
 
 def test_delete_results(results, work):
     """Test delete results."""
     status = results.delete_ids(work.pipeline, [work.id])
-    assert status[work.pipeline] is True
+    assert status[work.pipeline] == 1
 
     response = results.view(
         pipeline=work.pipeline,
         query={},
         projection={"id": 1},
     )
```

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_swarm.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_tns.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_transfer_daemon.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_transfer_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_voe.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_voe_subscribers.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_work.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_work.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_work_http_operations.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_work_http_operations.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/tests/test_workflow.py` & `chime_frb_api-3.1.0/chime_frb_api/tests/test_workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             "run",
             "workflow-tests",
             "chime_frb_api.tests.test_workflow." + func_name,
             "--lifetime=%i" % lifetime,
             "--base-url=http://localhost:8000",
             "--site=local",
             "--sleep-time=1",
-            "--log-level=DEBUG",
+            "--loki-url=http://not-working-loki-url",
+            "--log-level=INFO",
         ],
     )
 
 
 def invoke_dynamic_run(lifetime: int = 1):
     """Invoke the run command with the given arguments."""
     return CliRunner().invoke(
@@ -85,15 +86,16 @@
         [
             "run",
             "workflow-tests",
             "--lifetime=%i" % lifetime,
             "--base-url=http://localhost:8000",
             "--site=local",
             "--sleep-time=1",
-            "--log-level=DEBUG",
+            "--loki-url=http://not-working-loki-url",
+            "--log-level=INFO",
         ],
     )
 
 
 def test_success(buckets, work):
     """Test that a successful task is marked as such."""
     assert work.deposit(**BUCKETS_KWARGS)
@@ -196,15 +198,16 @@
             "run",
             "workflow-tests",
             "chime_frb_api.tests.test_workflow.sleep_func",
             "--lifetime=1",
             "--base-url=http://localhost:9000",
             "--site=local",
             "--sleep-time=1",
-            "--log-level=DEBUG",
+            "--loki-url=http://not-a-real-url",
+            "--log-level=INFO",
         ],
     )
     assert result.exit_code == 1
 
 
 def sleep_func(**kwargs):
     """Sleep for a given number of seconds."""
```

### Comparing `chime_frb_api-3.0.3/chime_frb_api/utils/copy.py` & `chime_frb_api-3.1.0/chime_frb_api/utils/copy.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/utils/github.py` & `chime_frb_api-3.1.0/chime_frb_api/utils/github.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/utils/loki.py` & `chime_frb_api-3.1.0/chime_frb_api/utils/loki.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         if loki_sc == 200:
             loki_handler = LokiHandler(
                 url=loki_url, tags={"site": site, "pipeline": pipeline}, version="1"
             )
             loki_handler.setFormatter(
                 Formatter("%(levelname)s %(tag)s %(name)s %(message)s")
             )
+            loki_handler.setLevel("ERROR")
             logger.root.addHandler(loki_handler)
             logger.debug(f"Loki URL: {loki_url}")
             status = True
         else:
             raise AttributeError("Loki not ready.")
     except Exception as error:
         logger.debug(error)
```

### Comparing `chime_frb_api-3.0.3/chime_frb_api/utils/move.py` & `chime_frb_api-3.1.0/chime_frb_api/utils/move.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/cli/buckets.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/cli/buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/cli/pipelines.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/cli/run.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/cli/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Fetch and process Work using any method compatible with Tasks API."""
 
 
+import platform
 import signal
 import time
 from threading import Event
 from typing import Any, Callable, Dict, List, Optional
 
 import click
 import requests
 from rich.console import Console
 
 from chime_frb_api import get_logger
-from chime_frb_api.configs import LOKI_URLS, WORKFLOW_URLS
+from chime_frb_api.configs import LOKI_URLS, PRODUCTS_URLS, WORKFLOW_URLS
 from chime_frb_api.core.logger import set_tag, unset_tag
 from chime_frb_api.utils import loki
 from chime_frb_api.workflow import Work
-from chime_frb_api.workflow.lifecycle import archive, execute, validate
+from chime_frb_api.workflow.lifecycle import archive, container, execute, validate
 
 logger = get_logger("workflow")
 
 
 @click.command("run", short_help="Perform work.")
 @click.argument("bucket", type=str, required=True)
 @click.argument(
@@ -75,14 +76,22 @@
     type=click.STRING,
     default=None,
     required=False,
     show_default=True,
     help="url for loki logging server.",
 )
 @click.option(
+    "--products-url",
+    type=click.STRING,
+    default=None,
+    required=False,
+    show_default=True,
+    help="url for products and plotsj.",
+)
+@click.option(
     "--log-level",
     type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
     default="INFO",
     show_default=True,
     help="logging level.",
 )
 def run(
@@ -90,39 +99,51 @@
     function: str,
     command: str,
     lifetime: int,
     sleep_time: int,
     base_url: Optional[str],
     site: str,
     loki_url: Optional[str],
+    products_url: Optional[str],
     log_level: str,
 ):
     """Perform work retrieved from the workflow buckets."""
     # Set logging level
     logger.root.setLevel(log_level)
     logger.root.handlers[0].setLevel(log_level)
     if not base_url:
         base_url = str(WORKFLOW_URLS[site])
     if not loki_url:
         loki_url = str(LOKI_URLS[site])
+    if not products_url:
+        products_url = str(PRODUCTS_URLS[site])
     # Setup and connect to the workflow backend
     logger.info("[bold]Workflow Run CLI[/bold]", extra=dict(markup=True, color="green"))
     logger.info(f"Bucket   : {bucket}")
     logger.info(f"Function : {function}")
     logger.info(f"Command  : {command}")
     logger.info(f"Mode     : {'Static' if (function or command) else 'Dynamic'}")
     # Print inifinity symbol if lifetime is -1, otherwise print lifetime
     logger.info(f"Lifetime : {'infinite' if lifetime == -1 else lifetime}")
     logger.info(f"Sleep    : {sleep_time}s")
     logger.info(f"Work Site: {site}")
     logger.info(f"Log Level: {log_level}")
     logger.info(f"Base URL : {base_url}")
     logger.info(f"Loki URL : {loki_url}")
+    logger.info(f"Prod URL : {products_url}")
+    logger.info(
+        "[bold]Execution Environment [/bold]",
+        extra=dict(markup=True, color="green"),
+    )
+    logger.info(f"Operating System: {platform.system()}")
+    logger.info(f"Python Version  : {platform.python_version()}")
+    logger.info(f"Python Compiler : {platform.python_compiler()}")
+    logger.info(f"Virtualization  : {container.virtualization()}")
     logger.info(
-        "[bold]Workflow Configuration Checks [/bold]",
+        "[bold]Configuration Checks [/bold]",
         extra=dict(markup=True, color="green"),
     )
     loki_status = loki.add_handler(logger, site, bucket, loki_url)
     logger.info(f"Loki Logs: {'✅' if loki_status else '❌'}")
 
     try:
         requests.get(base_url).headers
@@ -138,19 +159,24 @@
         logger.info("Function : ✅")
 
     try:
         logger.info(
             "[bold]Starting Workflow Lifecycle[/bold]",
             extra=dict(markup=True, color="green"),
         )
+        slowdown: float = 1.0
+        if container.virtualization():
+            slowdown = 1000.0
         console = Console(force_terminal=True, tab_size=4)
         with console.status(
-            status="Running...",
-            spinner="arc",
+            status="",
+            spinner="toggle2",
             spinner_style="bold green",
+            refresh_per_second=1,
+            speed=1 / slowdown,
         ):
             lifecycle(bucket, function, lifetime, sleep_time, site, base_url)
     except Exception as error:
         logger.exception(error)
     finally:
         logger.info(
             "[bold]Workflow Lifecycle Complete[/bold]",
@@ -247,14 +273,23 @@
             archive.run(work)
             status = True
     except Exception as error:
         logger.exception(error)
         work.status = "failure"  # type: ignore
     finally:
         if work:
+            if any(work.notify.slack.dict().values()) and work.products:
+                work.products = [
+                    f"<{str(PRODUCTS_URLS[site])}{product}|{product}>"
+                    for product in work.products
+                ]
+            if any(work.notify.slack.dict().values()) and work.plots:
+                work.plots = [
+                    f"<{str(PRODUCTS_URLS[site])}{plot}|{plot}>" for plot in work.plots
+                ]
             work.update(**kwargs)  # type: ignore
             logger.info("work completed: ✅")
         unset_tag()
         return status
 
 
 if __name__ == "__main__":
```

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/cli/sample.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/cli/sample.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/cli/sample.yaml` & `chime_frb_api-3.1.0/chime_frb_api/workflow/cli/sample.yaml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/daemons/audit.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/daemons/audit.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/daemons/transfer.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/daemons/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,29 @@
 
     Returns:
         transfer_status (bool): Number of works deposited to results.
     """
     try:
         transfer_status = False
         results_deposit_status = results.deposit(works)
-        if all(results_deposit_status.values()):
+        if all([val > 0 for val in results_deposit_status.values()]):
             buckets.delete_ids([work["id"] for work in works])
             transfer_status = True
         return transfer_status
     except Exception as error:
         print(f"Exception occurred: {error}")
         transfer_status = False
         work_to_deposit = [
             work for work in works if is_work_already_deposited(results, work) is False
         ]
         results_deposit_status = results.deposit(work_to_deposit)
-        if all(results_deposit_status.values()) or results_deposit_status == {}:
+        if (
+            all([val > 0 for val in results_deposit_status.values()])
+            or results_deposit_status == {}
+        ):
             buckets.delete_ids([work["id"] for work in works])
             transfer_status = True
         return transfer_status
 
 
 def is_work_already_deposited(results: Results, work: Dict[str, Any]) -> bool:
     """Check if a work has already been deposited to results.
```

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/archive.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/execute.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/execute.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Execute the work function or command."""
 import ast
 import subprocess
 import time
 from typing import Any, Callable, Dict, List, Optional
 
 import click
+from mergedeep import merge
 
 from chime_frb_api import get_logger
 from chime_frb_api.workflow import Work
 
 logger = get_logger("workflow")
 
 
@@ -45,17 +46,20 @@
     logger.info(f"executing: {user_func.__name__}(**{parameters})")
     start = time.time()
     try:
         results, products, plots = user_func(**parameters)
         logger.debug(f"results : {results}")
         logger.debug(f"products: {products}")
         logger.debug(f"plots   : {plots}")
-        work.results = results
-        work.products = products
-        work.plots = plots
+        if results:
+            work.results = merge(work.results or {}, results)  # type: ignore
+        if products:
+            work.products = (work.products or []) + products
+        if plots:
+            work.plots = (work.plots or []) + plots
         work.status = "success"
     except Exception as error:
         work.status = "failure"
         logger.exception(error)
     finally:
         end = time.time()
         work.stop = end
```

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/lifecycle/validate.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/lifecycle/validate.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/chime_frb_api/workflow/work.py` & `chime_frb_api-3.1.0/chime_frb_api/workflow/work.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.0.3/pyproject.toml` & `chime_frb_api-3.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chime-frb-api"
-version = "3.0.3"
+version = "3.1.0"
 description = "CHIME/FRB API"
 authors = ["Shiny Brar <charanjotbrar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CHIMEFRB/frb-api"
 documentation = "https://github.com/CHIMEFRB/frb-api"
 classifiers = [
@@ -30,14 +30,15 @@
 attrs = "^22.2.0"
 tenacity = "^8.1"
 rich = "^13.1"
 mkdocs-material = { version = ">=8", optional = true }
 pytkdocs = { version = ">=0.10", optional = true, extras = ["numpy-style"] }
 mkdocstrings-python = { version = "^0.8.3", optional = true }
 python-logging-loki = "^0.3.1"
+mergedeep = "^1.3.4"
 
 [tool.poetry.extras]
 docs = ["mkdocs-material", "mkdocstrings-python", "pytkdocs"]
 
 [tool.poetry.scripts]
 frb-api = "chime_frb_api.cli:cli"
 workflow = "chime_frb_api.workflow.runner:cli"
```

### Comparing `chime_frb_api-3.0.3/PKG-INFO` & `chime_frb_api-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chime-frb-api
-Version: 3.0.3
+Version: 3.1.0
 Summary: CHIME/FRB API
 Home-page: https://github.com/CHIMEFRB/frb-api
 License: MIT
 Author: Shiny Brar
 Author-email: charanjotbrar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: click (>=7)
+Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: mkdocs-material (>=8) ; extra == "docs"
 Requires-Dist: mkdocstrings-python (>=0.8.3,<0.9.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyjwt (>=2,<3)
 Requires-Dist: python-dateutil (>=2,<3)
 Requires-Dist: python-logging-loki (>=0.3.1,<0.4.0)
 Requires-Dist: pytkdocs[numpy-style] (>=0.10) ; extra == "docs"
```

