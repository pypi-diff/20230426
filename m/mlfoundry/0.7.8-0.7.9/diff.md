# Comparing `tmp/mlfoundry-0.7.8.tar.gz` & `tmp/mlfoundry-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.7.8.tar", max compression
+gzip compressed data, was "mlfoundry-0.7.9.tar", max compression
```

## Comparing `mlfoundry-0.7.8.tar` & `mlfoundry-0.7.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     3158 2023-04-24 10:51:50.367933 mlfoundry-0.7.8/README.md
--rw-r--r--   0        0        0      991 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0     9414 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0      731 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      739 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2724 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/constants.py
--rw-r--r--   0        0        0      103 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/__init__.py
--rw-r--r--   0        0        0     7854 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/dataset.py
--rw-r--r--   0        0        0     2255 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/schema.py
--rw-r--r--   0        0        0    13138 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/serde.py
--rw-r--r--   0        0        0     2028 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/serde_utils.py
--rw-r--r--   0        0        0     2078 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/stats.py
--rw-r--r--   0        0        0     1903 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/types.py
--rw-r--r--   0        0        0     2588 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/validation.py
--rw-r--r--   0        0        0       69 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/whylogs_types/__init__.py
--rw-r--r--   0        0        0     4025 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/whylogs_types/summary.py
--rw-r--r--   0        0        0     1358 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/enums.py
--rw-r--r--   0        0        0      325 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     1906 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      724 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15215 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22189 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      571 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     7521 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     2871 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    14349 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0     1281 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/dataset_artifact.py
--rw-r--r--   0        0        0      222 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/dataset_schema.py
--rw-r--r--   0        0        0      318 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/dataset_stats.py
--rw-r--r--   0        0        0       50 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    30890 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    46245 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4304 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/run_utils.py
--rw-r--r--   0        0        0      492 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/schema.py
--rw-r--r--   0        0        0     9979 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3549 2023-04-24 10:52:05.396042 mlfoundry-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-04-26 11:54:04.850183 mlfoundry-0.7.9/README.md
+-rw-r--r--   0        0        0      991 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0     7069 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0      731 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      739 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2724 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/constants.py
+-rw-r--r--   0        0        0      103 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/__init__.py
+-rw-r--r--   0        0        0     7854 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/dataset.py
+-rw-r--r--   0        0        0     2255 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/schema.py
+-rw-r--r--   0        0        0    13138 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/serde.py
+-rw-r--r--   0        0        0     2028 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/serde_utils.py
+-rw-r--r--   0        0        0     2078 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/stats.py
+-rw-r--r--   0        0        0     1903 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/types.py
+-rw-r--r--   0        0        0     2588 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/validation.py
+-rw-r--r--   0        0        0       69 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/whylogs_types/__init__.py
+-rw-r--r--   0        0        0     4025 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/whylogs_types/summary.py
+-rw-r--r--   0        0        0     1358 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/enums.py
+-rw-r--r--   0        0        0      325 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     1906 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      724 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15215 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22189 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      571 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     7521 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     2871 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    14349 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5983 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0     1281 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/dataset_artifact.py
+-rw-r--r--   0        0        0      222 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/dataset_schema.py
+-rw-r--r--   0        0        0      318 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/dataset_stats.py
+-rw-r--r--   0        0        0       50 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    30890 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    46245 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4304 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0      492 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/schema.py
+-rw-r--r--   0        0        0     9979 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3549 2023-04-26 11:54:16.574302 mlfoundry-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.7.9/PKG-INFO
```

### Comparing `mlfoundry-0.7.8/README.md` & `mlfoundry-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/__init__.py` & `mlfoundry-0.7.9/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/__main__.py` & `mlfoundry-0.7.9/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/amplitude.py` & `mlfoundry-0.7.9/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.7.9/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import os
 import posixpath
-import signal
-import sys
 import typing
 import uuid
-from concurrent.futures import ProcessPoolExecutor, as_completed
-from multiprocessing import active_children
 
 from mlflow.entities import FileInfo, SignedURL
 from mlflow.store.artifact.artifact_repo import ArtifactRepository
 from mlflow.tracking import MlflowClient
 from mlflow.utils.file_utils import (
     download_file_using_http_uri,
     relative_path_to_artifact_path,
@@ -17,38 +13,14 @@
 from mlflow.utils.rest_utils import cloud_storage_http_request
 
 from mlfoundry.exceptions import MlFoundryException
 from mlfoundry.tracking.entities import ArtifactCredential
 from mlfoundry.tracking.truefoundry_rest_store import TruefoundryRestStore
 
 
-def sigterm_handler(sig, frame):
-    print("Handling SIGTERM...")
-    try:
-        active = active_children()
-        # terminate all active children
-        for child in active:
-            child.terminate()
-    finally:
-        # terminate the process
-        sys.exit(0)
-
-
-def sighup_handler(sig, frame):
-    print("Handling SIGHUP...")
-    try:
-        active = active_children()
-        # terminate all active children
-        for child in active:
-            child.terminate()
-    finally:
-        # terminate the process
-        sys.exit(0)
-
-
 class TruefoundryArtifactRepository(ArtifactRepository):
     def __init__(
         self,
         artifact_uri,
         rest_store: TruefoundryRestStore,
         credentials=None,
         storage_integration_id=None,
@@ -121,107 +93,61 @@
             run_id=self._extract_run_id(self.artifact_uri), path=remote_file_path
         )
         download_file_using_http_uri(
             http_uri=artifact_credential.signed_uri, download_path=local_path
         )
 
 
-def _signed_uri_upload_file(signed_url: SignedURL, local_file: str):
-    if os.stat(local_file).st_size == 0:
-        with cloud_storage_http_request("put", signed_url.url, data="") as response:
-            response.raise_for_status()
-    else:
-        with open(local_file, "rb") as file:
-            with cloud_storage_http_request(
-                "put", signed_url.url, data=file
-            ) as response:
-                response.raise_for_status()
-
-
 class MlFoundryArtifactsRepository(ArtifactRepository):
     def __init__(self, version_id: uuid.UUID, mlflow_client: MlflowClient):
         self.version_id = version_id
         self._tracking_client = mlflow_client
         super().__init__(artifact_uri=None)
 
     # these methods should be named list_files, log_directory, log_file, etc
 
     def list_artifacts(self, path=None) -> typing.List[FileInfo]:
         return self._tracking_client.list_files_for_artifact_version(
             version_id=self.version_id, path=path
         )
 
-    def get_write_signed_url(self, local_file, artifact_path=None) -> str:
-        dest_path = artifact_path or ""
-        dest_path = dest_path.lstrip(posixpath.sep)
-        dest_path = posixpath.join(dest_path, os.path.basename(local_file))
-
-        return self._tracking_client.get_signed_urls_for_artifact_version_write(
-            version_id=self.version_id, paths=[dest_path]
-        )[0]
-
     def _signed_uri_upload_file(self, signed_url: SignedURL, local_file: str):
-        _signed_uri_upload_file(signed_url=signed_url, local_file=local_file)
+        if os.stat(local_file).st_size == 0:
+            with cloud_storage_http_request("put", signed_url.url, data="") as response:
+                response.raise_for_status()
+        else:
+            with open(local_file, "rb") as file:
+                with cloud_storage_http_request(
+                    "put", signed_url.url, data=file
+                ) as response:
+                    response.raise_for_status()
 
     def log_artifacts(self, local_dir, artifact_path=None):
         dest_path = artifact_path or ""
         dest_path = dest_path.lstrip(posixpath.sep)
-        files = []
-
         for (root, _, file_names) in os.walk(local_dir):
             upload_path = dest_path
             if root != local_dir:
                 rel_path = os.path.relpath(root, local_dir)
                 rel_path = relative_path_to_artifact_path(rel_path)
                 upload_path = posixpath.join(dest_path, rel_path)
             for file_name in file_names:
                 local_file = os.path.join(root, file_name)
-                files.append((upload_path, local_file))
-
-        files.sort(
-            key=lambda x: os.stat(x[1]).st_size
-        )  # sort on the basis of file size
-
-        # finally block doesn't execute when SIGTERM, SIGHUP, SIGKILL are received
-        # Handle SIGTERM, SIGHUP signals to avoid zombie processes
-        signal.signal(signal.SIGTERM, sigterm_handler)
-        signal.signal(signal.SIGHUP, sighup_handler)
-
-        # Log artifacts in parallel using ProcessPoolExecutor
-        with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
-            futures = []
-
-            for upload_path, local_file in files:
-                signed_url = self.get_write_signed_url(
-                    local_file=local_file, artifact_path=upload_path
-                )
-                future = executor.submit(
-                    _signed_uri_upload_file, signed_url, local_file
-                )
-                futures.append(future)
-
-            try:
-                for future in as_completed(futures):
-                    future.result()
-            except Exception as e:
-                raise e
-            finally:
-                [f.cancel() for f in futures]
-                # Accessing protected member of a class here (could fail in future versions)
-                for pid, proc in executor._processes.items():
-                    if proc.is_alive():
-                        proc.terminate()
+                self.log_artifact(local_file=local_file, artifact_path=upload_path)
 
     def log_artifact(self, local_file, artifact_path=None):
+        dest_path = artifact_path or ""
+        dest_path = dest_path.lstrip(posixpath.sep)
+        dest_path = posixpath.join(dest_path, os.path.basename(local_file))
         # TODO (chiragjn): Re-implement log_artifacts to take advantage of getting multiple signed urls at once
         #                  However care also needs to be taken to expose and pass in proper expiry because the user
         #                  user might be on slow connections or downloading many files sequentially might eat up time
-        signed_url = self.get_write_signed_url(
-            local_file=local_file, artifact_path=artifact_path
-        )
+        signed_url = self._tracking_client.get_signed_urls_for_artifact_version_write(
+            version_id=self.version_id, paths=[dest_path]
+        )[0]
         self._signed_uri_upload_file(signed_url, local_file)
 
     def _download_file(self, remote_file_path: str, local_path: str):
         if not remote_file_path:
             raise MlFoundryException(
                 f"remote_file_path cannot be None or empty str {remote_file_path}"
             )
```

### Comparing `mlfoundry-0.7.8/mlfoundry/background/interface.py` & `mlfoundry-0.7.9/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/background/sender.py` & `mlfoundry-0.7.9/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/background/system_metrics.py` & `mlfoundry-0.7.9/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/background/utils.py` & `mlfoundry-0.7.9/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.7.9/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/cli/commands/download.py` & `mlfoundry-0.7.9/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/cli/commands/login.py` & `mlfoundry-0.7.9/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/constants.py` & `mlfoundry-0.7.9/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/dataset.py` & `mlfoundry-0.7.9/mlfoundry/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/schema.py` & `mlfoundry-0.7.9/mlfoundry/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/serde.py` & `mlfoundry-0.7.9/mlfoundry/dataset/serde.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/serde_utils.py` & `mlfoundry-0.7.9/mlfoundry/dataset/serde_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/stats.py` & `mlfoundry-0.7.9/mlfoundry/dataset/stats.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/types.py` & `mlfoundry-0.7.9/mlfoundry/dataset/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/validation.py` & `mlfoundry-0.7.9/mlfoundry/dataset/validation.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/dataset/whylogs_types/summary.py` & `mlfoundry-0.7.9/mlfoundry/dataset/whylogs_types/summary.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/enums.py` & `mlfoundry-0.7.9/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.7.9/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/git_info.py` & `mlfoundry-0.7.9/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/integrations/lightning.py` & `mlfoundry-0.7.9/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/integrations/transformers.py` & `mlfoundry-0.7.9/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/internal_namespace.py` & `mlfoundry-0.7.9/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/__init__.py` & `mlfoundry-0.7.9/mlfoundry/log_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/dataset_artifact.py` & `mlfoundry-0.7.9/mlfoundry/log_types/dataset_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/image/image.py` & `mlfoundry-0.7.9/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.7.9/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/image/types.py` & `mlfoundry-0.7.9/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/plot.py` & `mlfoundry-0.7.9/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.7.9/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/log_types/utils.py` & `mlfoundry-0.7.9/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/login.py` & `mlfoundry-0.7.9/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.7.9/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.7.9/mlfoundry/mlfoundry_api.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.7.9/mlfoundry/mlfoundry_run.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/monitoring/entities.py` & `mlfoundry-0.7.9/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.7.9/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.7.9/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/run_utils.py` & `mlfoundry-0.7.9/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/session.py` & `mlfoundry-0.7.9/mlfoundry/session.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.7.9/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/tracking/entities.py` & `mlfoundry-0.7.9/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.7.9/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.7.9/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.7.9/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.8/pyproject.toml` & `mlfoundry-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.7.8" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.7.9" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
```

### Comparing `mlfoundry-0.7.8/PKG-INFO` & `mlfoundry-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.7.8
+Version: 0.7.9
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

