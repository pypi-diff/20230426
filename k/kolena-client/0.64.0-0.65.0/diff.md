# Comparing `tmp/kolena_client-0.64.0.tar.gz` & `tmp/kolena_client-0.65.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.64.0.tar", max compression
+gzip compressed data, was "kolena_client-0.65.0.tar", max compression
```

## Comparing `kolena_client-0.64.0.tar` & `kolena_client-0.65.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0    11346 2023-04-18 22:03:41.350605 kolena_client-0.64.0/LICENSE
--rw-r--r--   0        0        0      556 2023-04-18 22:03:41.350605 kolena_client-0.64.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1492 2023-04-18 22:03:41.350605 kolena_client-0.64.0/README.md
--rw-r--r--   0        0        0     1356 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1725 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     7578 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7480 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5507 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      690 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/samples.py
--rw-r--r--   0        0        0      833 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0      784 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/_consts.py
--rw-r--r--   0        0        0     1604 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     6883 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      579 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     2774 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1260 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/futures.py
--rw-r--r--   0        0        0     1183 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2646 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4161 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/log.py
--rw-r--r--   0        0        0      997 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     4768 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     6672 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/stratification.py
--rw-r--r--   0        0        0     1942 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-04-18 22:03:41.350605 kolena_client-0.64.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3005 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    14006 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3578 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     2541 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4138 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8415 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13650 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    12938 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     4707 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0      689 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/_consts.py
--rw-r--r--   0        0        0    20512 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9248 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14560 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12177 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    17008 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15219 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     4134 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/initialize.py
--rw-r--r--   0        0        0     4454 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6052 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     6423 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    14664 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0     9312 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3359 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3433 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      625 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     2738 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7436 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13248 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22814 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     8817 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    11379 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9293 2023-04-18 22:03:41.354605 kolena_client-0.64.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     1927 2023-04-18 22:03:53.818579 kolena_client-0.64.0/pyproject.toml
--rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 kolena_client-0.64.0/setup.py
--rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 kolena_client-0.64.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-25 23:03:30.123107 kolena_client-0.65.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-04-25 23:03:30.123107 kolena_client-0.65.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1405 2023-04-25 23:03:30.123107 kolena_client-0.65.0/README.md
+-rw-r--r--   0        0        0     1356 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1725 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     7578 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7480 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5507 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      690 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/samples.py
+-rw-r--r--   0        0        0      833 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0      784 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/_consts.py
+-rw-r--r--   0        0        0     1604 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     6883 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      579 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     2774 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1260 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/futures.py
+-rw-r--r--   0        0        0     1183 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2646 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4161 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0      997 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     4768 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     6672 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/stratification.py
+-rw-r--r--   0        0        0     1942 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3005 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    14006 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3578 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     2541 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4138 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-04-25 23:03:30.123107 kolena_client-0.65.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8415 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13650 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    12938 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     4707 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0      689 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/_consts.py
+-rw-r--r--   0        0        0    20512 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9248 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14560 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12177 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    17008 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15219 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     4134 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4454 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6052 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     6423 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    14664 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0     9312 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3359 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3433 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      625 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     2738 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7436 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13248 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22814 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     8817 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    11379 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9293 2023-04-25 23:03:30.127107 kolena_client-0.65.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     1927 2023-04-25 23:03:41.467385 kolena_client-0.65.0/pyproject.toml
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 kolena_client-0.65.0/setup.py
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 kolena_client-0.65.0/PKG-INFO
```

### Comparing `kolena_client-0.64.0/LICENSE` & `kolena_client-0.65.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/LICENSE_HEADER` & `kolena_client-0.65.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/README.md` & `kolena_client-0.65.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 <p align="center">
-  <img src="./docs/source/_static/wordmark-purple.svg#gh-light-mode-only" width="400" alt="Kolena" />
-  <img src="./docs/source/_static/wordmark-white.svg#gh-dark-mode-only" width="400" alt="Kolena" />
+  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />
 </p>
 
 <p align='center'>
   <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>
   <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>
   <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>
   <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-                               [Kolena] [Kolena]
+                                   [Kolena]
  [https://img.shields.io/pypi/v/kolena-client] [https://img.shields.io/pypi/l/
    kolena-client] [https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-
       6434c1] [https://img.shields.io/badge/docs-API%20Reference-6434c1]
 --- [Kolena](https://www.kolena.io) is a comprehensive machine learning testing
 and debugging platform to surface hidden model behaviors and take the mystery
 out of model development. Kolena helps you: - Perform high-resolution model
 evaluation - Understand and track behavioral improvements and regressions -
```

### Comparing `kolena_client-0.64.0/kolena/__init__.py` & `kolena_client-0.65.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/__init__.py` & `kolena_client-0.65.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/__init__.py` & `kolena_client-0.65.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.65.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/client_log.py` & `kolena_client-0.65.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/core.py` & `kolena_client-0.65.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/detection.py` & `kolena_client-0.65.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/fr.py` & `kolena_client-0.65.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/generic.py` & `kolena_client-0.65.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/repository.py` & `kolena_client-0.65.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/samples.py` & `kolena_client-0.65.0/kolena/_api/v1/samples.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/token.py` & `kolena_client-0.65.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_api/v1/workflow.py` & `kolena_client-0.65.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/__init__.py` & `kolena_client-0.65.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/_consts.py` & `kolena_client-0.65.0/kolena/_utils/_consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.65.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/batched_load.py` & `kolena_client-0.65.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/cli.py` & `kolena_client-0.65.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.65.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.65.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/datatypes.py` & `kolena_client-0.65.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/endpoints.py` & `kolena_client-0.65.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/frozen.py` & `kolena_client-0.65.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/futures.py` & `kolena_client-0.65.0/kolena/_utils/futures.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/geometry.py` & `kolena_client-0.65.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/inference_validators.py` & `kolena_client-0.65.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/instrumentation.py` & `kolena_client-0.65.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/krequests.py` & `kolena_client-0.65.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/log.py` & `kolena_client-0.65.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/repository.py` & `kolena_client-0.65.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/serde.py` & `kolena_client-0.65.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/serializable.py` & `kolena_client-0.65.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/state.py` & `kolena_client-0.65.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/stratification.py` & `kolena_client-0.65.0/kolena/_utils/stratification.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.65.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/_utils/validators.py` & `kolena_client-0.65.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/__init__.py` & `kolena_client-0.65.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/metadata.py` & `kolena_client-0.65.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/model.py` & `kolena_client-0.65.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.65.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.65.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.65.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.65.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.65.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/test_case.py` & `kolena_client-0.65.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/test_config.py` & `kolena_client-0.65.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/test_image.py` & `kolena_client-0.65.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/test_run.py` & `kolena_client-0.65.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/classification/test_suite.py` & `kolena_client-0.65.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/__init__.py` & `kolena_client-0.65.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_datatypes.py` & `kolena_client-0.65.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.65.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.65.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.65.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/inference.py` & `kolena_client-0.65.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.65.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/model.py` & `kolena_client-0.65.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.65.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.65.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.65.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.65.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.65.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/ground_truth.py` & `kolena_client-0.65.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/inference.py` & `kolena_client-0.65.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/metadata.py` & `kolena_client-0.65.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/model.py` & `kolena_client-0.65.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/test_case.py` & `kolena_client-0.65.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/test_config.py` & `kolena_client-0.65.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/test_image.py` & `kolena_client-0.65.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/test_run.py` & `kolena_client-0.65.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/detection/test_suite.py` & `kolena_client-0.65.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/errors.py` & `kolena_client-0.65.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/__init__.py` & `kolena_client-0.65.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/_consts.py` & `kolena_client-0.65.0/kolena/fr/_consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/datatypes.py` & `kolena_client-0.65.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/model.py` & `kolena_client-0.65.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/test_case.py` & `kolena_client-0.65.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/test_images.py` & `kolena_client-0.65.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/test_run.py` & `kolena_client-0.65.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/fr/test_suite.py` & `kolena_client-0.65.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/initialize.py` & `kolena_client-0.65.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/__init__.py` & `kolena_client-0.65.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/_datatypes.py` & `kolena_client-0.65.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/_helpers.py` & `kolena_client-0.65.0/kolena/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/_validators.py` & `kolena_client-0.65.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/annotation.py` & `kolena_client-0.65.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/asset.py` & `kolena_client-0.65.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/evaluator.py` & `kolena_client-0.65.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.65.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/ground_truth.py` & `kolena_client-0.65.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/inference.py` & `kolena_client-0.65.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.65.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.65.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/model.py` & `kolena_client-0.65.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/test_case.py` & `kolena_client-0.65.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/test_run.py` & `kolena_client-0.65.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/test_sample.py` & `kolena_client-0.65.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/test_suite.py` & `kolena_client-0.65.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/kolena/workflow/workflow.py` & `kolena_client-0.65.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.64.0/pyproject.toml` & `kolena_client-0.65.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.64.0"
+version = "0.65.0"
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena_client-0.64.0/setup.py` & `kolena_client-0.65.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,17 +40,17 @@
                              'typing-extensions>=4.5.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']}
 
 setup_kwargs = {
     'name': 'kolena-client',
-    'version': '0.64.0',
+    'version': '0.65.0',
     'description': "Client for Kolena's machine learning (ML) testing and debugging platform.",
-    'long_description': '<p align="center">\n  <img src="./docs/source/_static/wordmark-purple.svg#gh-light-mode-only" width="400" alt="Kolena" />\n  <img src="./docs/source/_static/wordmark-white.svg#gh-dark-mode-only" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>\n  <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\n`kolena-client` is the Python client library for programmatic interaction with Kolena.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena-client` typing and\nfunction documentation.\n',
+    'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>\n  <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\n`kolena-client` is the Python client library for programmatic interaction with Kolena.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena-client` typing and\nfunction documentation.\n',
     'author': 'Kolena Engineering',
     'author_email': 'eng@kolena.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kolena.io',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -7,17 +7,17 @@
 'click>=8.1.3,<9.0.0', 'dacite>=1.6', 'deprecation>=2.1.0,<3.0.0',
 'numpy>=1.19', 'pandas>=1.1,<1.6', 'pandera>=0.9.0', 'pyarrow>=8',
 'pydantic>=1.8', 'requests-toolbelt>=0.9.1,<0.10.0', 'requests>=2.20',
 'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0', 'tqdm>=4,<5']
 extras_require = \ {':python_version < "3.8"': ['importlib-metadata<5.0',
 'typing-extensions>=4.5.0,<5.0.0']} entry_points = \ {'console_scripts':
 ['kolena = kolena._utils.cli:run']} setup_kwargs = { 'name': 'kolena-client',
-'version': '0.64.0', 'description': "Client for Kolena's machine learning (ML)
+'version': '0.65.0', 'description': "Client for Kolena's machine learning (ML)
 testing and debugging platform.", 'long_description': '
-                           \n [Kolena]\n [Kolena]\n
+                                 \n [Kolena]\n
 \n\n
 \n [https://img.shields.io/pypi/v/kolena-client]\n [https://img.shields.io/
 pypi/l/kolena-client]\n [https://img.shields.io/badge/docs-
 Tutorial%20%26%20Usage-6434c1]\n [https://img.shields.io/badge/docs-
 API%20Reference-6434c1]\n
 \n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning
 testing and debugging platform to surface hidden\nmodel behaviors and take the
```

### Comparing `kolena_client-0.64.0/PKG-INFO` & `kolena_client-0.65.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.64.0
+Version: 0.65.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.11
@@ -40,16 +40,15 @@
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0); python_version < "3.8"
 Project-URL: Documentation, https://docs.kolena.io
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="./docs/source/_static/wordmark-purple.svg#gh-light-mode-only" width="400" alt="Kolena" />
-  <img src="./docs/source/_static/wordmark-white.svg#gh-dark-mode-only" width="400" alt="Kolena" />
+  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />
 </p>
 
 <p align='center'>
   <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>
   <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>
   <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>
   <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.64.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.65.0 Summary: Client for
 Kolena's machine learning (ML) testing and debugging platform. Home-page:
 https://kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author:
 Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.11
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
@@ -19,15 +19,15 @@
 numpy (>=1.19) Requires-Dist: pandas (>=1.1,<1.6) Requires-Dist: pandera
 (>=0.9.0) Requires-Dist: pyarrow (>=8) Requires-Dist: pydantic (>=1.8)
 Requires-Dist: requests (>=2.20) Requires-Dist: requests-toolbelt
 (>=0.9.1,<0.10.0) Requires-Dist: retrying (>=1.3.3,<2.0.0) Requires-Dist:
 termcolor (>=1.1.0,<2.0.0) Requires-Dist: tqdm (>=4,<5) Requires-Dist: typing-
 extensions (>=4.5.0,<5.0.0); python_version < "3.8" Project-URL: Documentation,
 https://docs.kolena.io Description-Content-Type: text/markdown
-                               [Kolena] [Kolena]
+                                   [Kolena]
  [https://img.shields.io/pypi/v/kolena-client] [https://img.shields.io/pypi/l/
    kolena-client] [https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-
       6434c1] [https://img.shields.io/badge/docs-API%20Reference-6434c1]
 --- [Kolena](https://www.kolena.io) is a comprehensive machine learning testing
 and debugging platform to surface hidden model behaviors and take the mystery
 out of model development. Kolena helps you: - Perform high-resolution model
 evaluation - Understand and track behavioral improvements and regressions -
```

