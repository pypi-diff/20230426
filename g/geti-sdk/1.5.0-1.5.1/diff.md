# Comparing `tmp/geti-sdk-1.5.0.tar.gz` & `tmp/geti-sdk-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geti-sdk-1.5.0.tar", last modified: Mon Apr 24 09:21:41 2023, max compression
+gzip compressed data, was "geti-sdk-1.5.1.tar", last modified: Wed Apr 26 14:33:14 2023, max compression
```

## Comparing `geti-sdk-1.5.0.tar` & `geti-sdk-1.5.1.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/LICENSE
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/MANIFEST.in
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/README.md
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.412743 geti-sdk-1.5.0/geti_sdk/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/annotation_readers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/base_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/geti_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/algorithms.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/annotation_scene.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/annotations.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/code_deployment_info.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configuration.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configuration_identifiers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/data_models/containers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/containers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/containers/algorithm_list.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/containers/media_list.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/data_models/enums/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_kind.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/configuration_enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/deployment_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/domain.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/job_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/job_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/media_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/model_status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      943 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/optimization_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/prediction_mode.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/shape_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/task_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/job.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/label.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/media.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/media_identifiers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8433 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/model_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/performance.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/predictions.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/project.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/shapes.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6544 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/task.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/task_annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/demos/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/constants.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.412743 geti-sdk-1.5.0/geti_sdk/demos/data/
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/demos/data/example/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data/example/dogs.png
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6113 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/anomaly_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9051 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/coco_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5359 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/download_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1881 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/video_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/anomaly_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/coco_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/deployment/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/deployment/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/deployment/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/deployment/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/deployment/data_models/intermediate_inference_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/data_models/region_of_interest.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26525 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/deployed_model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/deployment.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/deployment/resources/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/resources/OVMS_README.md
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/resources/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/utils.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55063 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/geti.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/http_session/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/exception.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/geti_session.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/server_config.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6021 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/platform_versions.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/rest_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3575 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/configuration_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/dataset_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/deployment_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/image_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16827 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/media_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/video_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/model_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/prediction_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/project_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/task_templates.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/training_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_converters/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/configuration_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/job_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/media_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/model_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/project_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/status_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/utils/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/algorithm_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/credentials_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/dictionary_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/label_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/plot_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/serialization_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/workspace_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.412743 geti-sdk-1.5.0/geti_sdk.egg-info/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5718 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/requires.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/top_level.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/pyproject.toml
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/requirements/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements-dev.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements-docs.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements-notebooks.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/setup.cfg
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/setup.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/tests/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/conftest.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/tests/helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/constants.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/finalizers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/fixtures.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/plotting.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/project_service.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/training.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/vcr_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.282863 geti-sdk-1.5.1/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/LICENSE
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/MANIFEST.in
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-04-26 14:33:14.282863 geti-sdk-1.5.1/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/README.md
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.266863 geti-sdk-1.5.1/geti_sdk/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.266863 geti-sdk-1.5.1/geti_sdk/annotation_readers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/annotation_readers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/annotation_readers/base_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.266863 geti-sdk-1.5.1/geti_sdk/annotation_readers/datumaro_annotation_reader/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/annotation_readers/geti_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.270863 geti-sdk-1.5.1/geti_sdk/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/algorithms.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/annotation_scene.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/annotations.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/code_deployment_info.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/configurable_parameter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/configurable_parameter_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/configuration.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/configuration_identifiers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.270863 geti-sdk-1.5.1/geti_sdk/data_models/containers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/containers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/containers/algorithm_list.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/containers/media_list.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.270863 geti-sdk-1.5.1/geti_sdk/data_models/enums/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/annotation_kind.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/configuration_enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/deployment_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/domain.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/job_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/job_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/media_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/model_status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      943 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/optimization_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/prediction_mode.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/shape_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/enums/task_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/job.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/label.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/media.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/media_identifiers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8433 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/model_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/performance.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/predictions.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/project.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/shapes.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6544 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/task.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/task_annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/data_models/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.274863 geti-sdk-1.5.1/geti_sdk/demos/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/constants.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.262863 geti-sdk-1.5.1/geti_sdk/demos/data/
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.274863 geti-sdk-1.5.1/geti_sdk/demos/data/example/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/data/example/dogs.png
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.274863 geti-sdk-1.5.1/geti_sdk/demos/data_helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/data_helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/data_helpers/anomaly_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/data_helpers/coco_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5361 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/data_helpers/download_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/data_helpers/video_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.274863 geti-sdk-1.5.1/geti_sdk/demos/demo_projects/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/demo_projects/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/demo_projects/anomaly_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/demo_projects/coco_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/demos/demo_projects/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.274863 geti-sdk-1.5.1/geti_sdk/deployment/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.274863 geti-sdk-1.5.1/geti_sdk/deployment/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/data_models/intermediate_inference_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/data_models/region_of_interest.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26525 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/deployed_model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/deployment.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.274863 geti-sdk-1.5.1/geti_sdk/deployment/resources/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/resources/OVMS_README.md
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/resources/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/deployment/utils.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55063 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/geti.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/http_session/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/http_session/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/http_session/exception.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/http_session/geti_session.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/http_session/server_config.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6021 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/platform_versions.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/rest_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3575 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/rest_clients/annotation_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/annotation_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/annotation_clients/annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/configuration_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/dataset_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/deployment_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/image_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16827 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/media_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/video_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/model_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/prediction_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/rest_clients/project_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/project_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/project_client/project_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/project_client/task_templates.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_clients/training_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/rest_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/rest_converters/annotation_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/configuration_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/job_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/media_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/model_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.278863 geti-sdk-1.5.1/geti_sdk/rest_converters/prediction_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/project_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/rest_converters/status_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.282863 geti-sdk-1.5.1/geti_sdk/utils/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/algorithm_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/credentials_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/dictionary_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/label_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/plot_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/serialization_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/geti_sdk/utils/workspace_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.266863 geti-sdk-1.5.1/geti_sdk.egg-info/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-04-26 14:33:14.000000 geti-sdk-1.5.1/geti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5718 2023-04-26 14:33:14.000000 geti-sdk-1.5.1/geti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-04-26 14:33:14.000000 geti-sdk-1.5.1/geti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-26 14:33:14.000000 geti-sdk-1.5.1/geti_sdk.egg-info/requires.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-04-26 14:33:14.000000 geti-sdk-1.5.1/geti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/pyproject.toml
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.282863 geti-sdk-1.5.1/requirements/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/requirements/requirements-dev.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/requirements/requirements-docs.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/requirements/requirements-notebooks.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/requirements/requirements.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-04-26 14:33:14.282863 geti-sdk-1.5.1/setup.cfg
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/setup.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.282863 geti-sdk-1.5.1/tests/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/conftest.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-26 14:33:14.282863 geti-sdk-1.5.1/tests/helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/constants.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/finalizers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/fixtures.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/plotting.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/project_service.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/training.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-04-26 14:10:09.000000 geti-sdk-1.5.1/tests/helpers/vcr_helpers.py
```

### Comparing `geti-sdk-1.5.0/LICENSE` & `geti-sdk-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/PKG-INFO` & `geti-sdk-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.0
+Version: 1.5.1
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.0/README.md` & `geti-sdk-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/__init__.py` & `geti-sdk-1.5.1/geti_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
    .. automethod:: upload_and_predict_media_folder
 
 """
 
 from .geti import Geti
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 
 __all__ = ["Geti"]
```

### Comparing `geti-sdk-1.5.0/geti_sdk/annotation_readers/__init__.py` & `geti-sdk-1.5.1/geti_sdk/annotation_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/annotation_readers/base_annotation_reader.py` & `geti-sdk-1.5.1/geti_sdk/annotation_readers/base_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py` & `geti-sdk-1.5.1/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py` & `geti-sdk-1.5.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py` & `geti-sdk-1.5.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/annotation_readers/directory_tree_annotation_reader.py` & `geti-sdk-1.5.1/geti_sdk/annotation_readers/directory_tree_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/annotation_readers/geti_annotation_reader.py` & `geti-sdk-1.5.1/geti_sdk/annotation_readers/geti_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/__init__.py` & `geti-sdk-1.5.1/geti_sdk/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/algorithms.py` & `geti-sdk-1.5.1/geti_sdk/data_models/algorithms.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/annotation_scene.py` & `geti-sdk-1.5.1/geti_sdk/data_models/annotation_scene.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/annotations.py` & `geti-sdk-1.5.1/geti_sdk/data_models/annotations.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/code_deployment_info.py` & `geti-sdk-1.5.1/geti_sdk/data_models/code_deployment_info.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter.py` & `geti-sdk-1.5.1/geti_sdk/data_models/configurable_parameter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter_group.py` & `geti-sdk-1.5.1/geti_sdk/data_models/configurable_parameter_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/configuration.py` & `geti-sdk-1.5.1/geti_sdk/data_models/configuration.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/configuration_identifiers.py` & `geti-sdk-1.5.1/geti_sdk/data_models/configuration_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/containers/__init__.py` & `geti-sdk-1.5.1/geti_sdk/data_models/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/containers/algorithm_list.py` & `geti-sdk-1.5.1/geti_sdk/data_models/containers/algorithm_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/containers/media_list.py` & `geti-sdk-1.5.1/geti_sdk/data_models/containers/media_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/__init__.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_kind.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/annotation_kind.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_state.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/configuration_enums.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/configuration_enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/deployment_state.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/deployment_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/domain.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/domain.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/job_state.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/job_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/job_type.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/job_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/media_type.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/media_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/model_status.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/model_status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/optimization_type.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/optimization_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/prediction_mode.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/prediction_mode.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/shape_type.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/shape_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/enums/task_type.py` & `geti-sdk-1.5.1/geti_sdk/data_models/enums/task_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/job.py` & `geti-sdk-1.5.1/geti_sdk/data_models/job.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/label.py` & `geti-sdk-1.5.1/geti_sdk/data_models/label.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/media.py` & `geti-sdk-1.5.1/geti_sdk/data_models/media.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/media_identifiers.py` & `geti-sdk-1.5.1/geti_sdk/data_models/media_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/model.py` & `geti-sdk-1.5.1/geti_sdk/data_models/model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/model_group.py` & `geti-sdk-1.5.1/geti_sdk/data_models/model_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/performance.py` & `geti-sdk-1.5.1/geti_sdk/data_models/performance.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/predictions.py` & `geti-sdk-1.5.1/geti_sdk/data_models/predictions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/project.py` & `geti-sdk-1.5.1/geti_sdk/data_models/project.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/shapes.py` & `geti-sdk-1.5.1/geti_sdk/data_models/shapes.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/status.py` & `geti-sdk-1.5.1/geti_sdk/data_models/status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/task.py` & `geti-sdk-1.5.1/geti_sdk/data_models/task.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/task_annotation_state.py` & `geti-sdk-1.5.1/geti_sdk/data_models/task_annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/data_models/utils.py` & `geti-sdk-1.5.1/geti_sdk/data_models/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/__init__.py` & `geti-sdk-1.5.1/geti_sdk/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/constants.py` & `geti-sdk-1.5.1/geti_sdk/demos/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/data/example/dogs.png` & `geti-sdk-1.5.1/geti_sdk/demos/data/example/dogs.png`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/__init__.py` & `geti-sdk-1.5.1/geti_sdk/demos/data_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/anomaly_helpers.py` & `geti-sdk-1.5.1/geti_sdk/demos/data_helpers/anomaly_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     )
     archive_name = f"{dataset_name}.tar.xz"
     url = f"https://www.mydrive.ch/shares/38536/3830184030e49fe74747669442f0f282/download/420938166-1629953277/{archive_name}"
     download_file(url, target_folder=dataset_path, check_valid_archive=False)
     archive_path = os.path.join(dataset_path, archive_name)
     validate_hash(
         file_path=archive_path,
-        expected_hash="146b2166c35a1d0cf37ded091366ac01a50338b4ac704632f1239890eaca4449",
+        expected_hash="f9c14ab6c802e69899b529da8b9417b319fa39027a0602ec2beeaf2c3a51e5d527248dfdd3c977a0066fb0ed284c6cdb7236e9cc11d06e927e07072496408be3",
     )
 
     logging.info(f"Extracting the '{dataset_name}' dataset at path {archive_path}...")
     with tarfile.open(archive_path) as tar_file:
         tar_file.extractall(dataset_path)
 
     if not is_ad_dataset(transistor_dataset_path):
```

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/coco_helpers.py` & `geti-sdk-1.5.1/geti_sdk/demos/data_helpers/coco_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             `None`
 
         :return: Tuple holding the hash digests for the archives, structured like:
             (image_zip, annotation_zip).
         """
         if self == COCOSubset.VAL2017:
             return (
-                "4f7e2ccb2866ec5041993c9cf2a952bbed69647b115d0f74da7ce8f4bef82f05",
-                "113a836d90195ee1f884e704da6304dfaaecff1f023f49b6ca93c4aaae470268",
+                "9ea554bcf9e6f88876b1157ab38247eb7c1c57564c05c7345a06ac479c6e7a3b9c3825150c189d7d3f2e807c95fd0e07fe90161c563591038e697c846ac76007",
+                "3f00c90323ee745b37a9ac040d00f170d49695ed9ffc1d8e0fbd4c5e2d8e9c697fd822b2022df552da5f1892dbcaeb68788416a347b05a20035ed0686f0e1f66",
             )
         else:
             return None, None
 
 
 def directory_has_coco_subset(target_folder: str, coco_subset: COCOSubset) -> bool:
     """
```

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/download_helpers.py` & `geti-sdk-1.5.1/geti_sdk/demos/data_helpers/download_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     """
     Verify that hash matches the calculated hash of the file.
 
     :param file_path: Path to file.
     :param expected_hash: Expected hash of the file.
     """
     with open(file_path, "rb") as hash_file:
-        downloaded_hash = hashlib.sha256(hash_file.read()).hexdigest()
+        downloaded_hash = hashlib.sha3_512(hash_file.read()).hexdigest()
     if downloaded_hash != expected_hash:
         raise ValueError(
             f"Downloaded file {file_path} does not match the required hash."
         )
 
 
 def set_directory_permissions(
```

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/video_helpers.py` & `geti-sdk-1.5.1/geti_sdk/demos/data_helpers/video_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     else:
         video_file_path = download_file(
             url="https://storage.openvinotoolkit.org/data/test_data/videos/person-bicycle-car-detection.mp4",
             target_folder=os.path.dirname(video_path),
         )
 
     # Compare hashes
-    expected_hash = "452b11b7e0efbd019f1d9570d0c790e90416ad4ad29eec6003872d08443140ef"
+    expected_hash = "7eafb94b3491e7554d92637596ddaaf1c69fdb8421c3d49eb09df4b7d05788c76391cb791cc2c8197e66d352306328d09c8d72e42733b1f1a311cd1e35ee1cce"
     validate_hash(file_path=video_file_path, expected_hash=expected_hash)
     return video_file_path
```

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/__init__.py` & `geti-sdk-1.5.1/geti_sdk/demos/demo_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/anomaly_demos.py` & `geti-sdk-1.5.1/geti_sdk/demos/demo_projects/anomaly_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/coco_demos.py` & `geti-sdk-1.5.1/geti_sdk/demos/demo_projects/coco_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/utils.py` & `geti-sdk-1.5.1/geti_sdk/demos/demo_projects/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/__init__.py` & `geti-sdk-1.5.1/geti_sdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/data_models/__init__.py` & `geti-sdk-1.5.1/geti_sdk/deployment/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/data_models/intermediate_inference_result.py` & `geti-sdk-1.5.1/geti_sdk/deployment/data_models/intermediate_inference_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/data_models/region_of_interest.py` & `geti-sdk-1.5.1/geti_sdk/deployment/data_models/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/deployed_model.py` & `geti-sdk-1.5.1/geti_sdk/deployment/deployed_model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/deployment.py` & `geti-sdk-1.5.1/geti_sdk/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/resources/OVMS_README.md` & `geti-sdk-1.5.1/geti_sdk/deployment/resources/OVMS_README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/resources/__init__.py` & `geti-sdk-1.5.1/geti_sdk/deployment/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/deployment/utils.py` & `geti-sdk-1.5.1/geti_sdk/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/geti.py` & `geti-sdk-1.5.1/geti_sdk/geti.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/http_session/__init__.py` & `geti-sdk-1.5.1/geti_sdk/http_session/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/http_session/exception.py` & `geti-sdk-1.5.1/geti_sdk/http_session/exception.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/http_session/geti_session.py` & `geti-sdk-1.5.1/geti_sdk/http_session/geti_session.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/http_session/server_config.py` & `geti-sdk-1.5.1/geti_sdk/http_session/server_config.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/platform_versions.py` & `geti-sdk-1.5.1/geti_sdk/platform_versions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/__init__.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/__init__.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/annotation_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/annotation_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/annotation_clients/annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/configuration_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/configuration_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/dataset_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/deployment_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/deployment_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/__init__.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/image_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/image_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/media_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/media_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/video_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/media_client/video_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/model_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/model_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/prediction_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/prediction_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/__init__.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/project_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/project_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/project_client/project_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/task_templates.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/project_client/task_templates.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_clients/training_client.py` & `geti-sdk-1.5.1/geti_sdk/rest_clients/training_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/__init__.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/__init__.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/annotation_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/configuration_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/configuration_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/job_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/job_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/media_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/media_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/model_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/model_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/__init__.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/prediction_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/project_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/project_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/rest_converters/status_rest_converter.py` & `geti-sdk-1.5.1/geti_sdk/rest_converters/status_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/__init__.py` & `geti-sdk-1.5.1/geti_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/algorithm_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/algorithm_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/credentials_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/dictionary_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/dictionary_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/label_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/label_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/plot_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/project_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/serialization_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk/utils/workspace_helpers.py` & `geti-sdk-1.5.1/geti_sdk/utils/workspace_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk.egg-info/PKG-INFO` & `geti-sdk-1.5.1/geti_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.0
+Version: 1.5.1
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.0/geti_sdk.egg-info/SOURCES.txt` & `geti-sdk-1.5.1/geti_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/geti_sdk.egg-info/requires.txt` & `geti-sdk-1.5.1/geti_sdk.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 omegaconf==2.3.*
 opencv-python==4.5.*
 python-dotenv==1.0.*
 tqdm==4.65.*
 Pillow==9.5.*
 pathvalidate>=2.5.0
 simplejson==3.19.*
-ipython==8.11.*
-otx==1.1.2
+ipython==8.12.*
+otx==1.2.0
 openvino==2022.3.0
 openmodelzoo-modelapi==2022.3.*
 certifi>=2022.12.7
 joblib>=1.1.1
 protobuf>=3.20.2
 ovmsclient>=2022.3
 orjson==3.8.8
```

### Comparing `geti-sdk-1.5.0/setup.py` & `geti-sdk-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/__init__.py` & `geti-sdk-1.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/conftest.py` & `geti-sdk-1.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/__init__.py` & `geti-sdk-1.5.1/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/constants.py` & `geti-sdk-1.5.1/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/enums.py` & `geti-sdk-1.5.1/tests/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/finalizers.py` & `geti-sdk-1.5.1/tests/helpers/finalizers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/fixtures.py` & `geti-sdk-1.5.1/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/plotting.py` & `geti-sdk-1.5.1/tests/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/project_helpers.py` & `geti-sdk-1.5.1/tests/helpers/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/project_service.py` & `geti-sdk-1.5.1/tests/helpers/project_service.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/training.py` & `geti-sdk-1.5.1/tests/helpers/training.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.0/tests/helpers/vcr_helpers.py` & `geti-sdk-1.5.1/tests/helpers/vcr_helpers.py`

 * *Files identical despite different names*

