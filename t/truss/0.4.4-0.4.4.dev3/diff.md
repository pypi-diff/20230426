# Comparing `tmp/truss-0.4.4.tar.gz` & `tmp/truss-0.4.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.4.tar", max compression
+gzip compressed data, was "truss-0.4.4.dev3.tar", max compression
```

## Comparing `truss-0.4.4.tar` & `truss-0.4.4.dev3.tar`

### file list

```diff
@@ -1,167 +1,164 @@
--rw-r--r--   0        0        0     5483 2023-04-26 11:28:59.394814 truss-0.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-04-26 11:28:59.394814 truss-0.4.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-04-26 11:28:59.394814 truss-0.4.4/LICENSE
--rw-r--r--   0        0        0     5958 2023-04-26 11:28:59.394814 truss-0.4.4/README.md
--rw-r--r--   0        0        0     3316 2023-04-26 11:28:59.394814 truss-0.4.4/ROADMAP.md
--rw-r--r--   0        0        0      465 2023-04-26 11:28:59.394814 truss-0.4.4/context_builder.Dockerfile
--rw-r--r--   0        0        0     2205 2023-04-26 11:28:59.470813 truss-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-26 11:28:59.470813 truss-0.4.4/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-04-26 11:28:59.470813 truss-0.4.4/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-04-26 11:28:59.470813 truss-0.4.4/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-04-26 11:28:59.470813 truss-0.4.4/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-04-26 11:28:59.470813 truss-0.4.4/truss/build.py
--rw-r--r--   0        0        0    10452 2023-04-26 11:28:59.470813 truss-0.4.4/truss/cli.py
--rw-r--r--   0        0        0     2742 2023-04-26 11:28:59.470813 truss-0.4.4/truss/constants.py
--rw-r--r--   0        0        0     1237 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     5130 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4511 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1976 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     1686 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-04-26 11:28:59.470813 truss-0.4.4/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-04-26 11:28:59.470813 truss-0.4.4/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-04-26 11:28:59.470813 truss-0.4.4/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-04-26 11:28:59.470813 truss-0.4.4/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-04-26 11:28:59.470813 truss-0.4.4/truss/errors.py
--rw-r--r--   0        0        0      824 2023-04-26 11:28:59.470813 truss-0.4.4/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-04-26 11:28:59.470813 truss-0.4.4/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6565 2023-04-26 11:28:59.470813 truss-0.4.4/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-04-26 11:28:59.470813 truss-0.4.4/truss/notebook.py
--rw-r--r--   0        0        0    11065 2023-04-26 11:28:59.470813 truss-0.4.4/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-04-26 11:28:59.470813 truss-0.4.4/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2388 2023-04-26 11:28:59.470813 truss-0.4.4/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-04-26 11:28:59.470813 truss-0.4.4/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-04-26 11:28:59.470813 truss-0.4.4/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-04-26 11:28:59.470813 truss-0.4.4/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-04-26 11:28:59.470813 truss-0.4.4/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/__init__.py
--rw-r--r--   0        0        0     1409 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1849 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       82 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      979 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0     2616 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/docs/README.md
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     2272 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1696 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0     1196 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      875 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1708 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0      237 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1892 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/common/external_data_resolver.py
--rw-r--r--   0        0        0     1352 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0      593 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     3318 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      733 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     5674 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      162 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     1054 2023-04-26 11:28:59.470813 truss-0.4.4/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1666 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1898 2023-04-26 11:28:59.474813 truss-0.4.4/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0      216 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0      669 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0     1006 2023-04-26 11:28:59.474813 truss-0.4.4/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/__init__.py
--rw-r--r--   0        0        0    20835 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/conftest.py
--rw-r--r--   0        0        0      783 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    11109 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6937 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2157 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/server/common/test_external_resolver.py
--rw-r--r--   0        0        0     2038 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2252 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_build.py
--rw-r--r--   0        0        0     2359 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_docker.py
--rw-r--r--   0        0        0     2605 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    31937 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-04-26 11:28:59.474813 truss-0.4.4/truss/tests/test_validation.py
--rw-r--r--   0        0        0    12070 2023-04-26 11:28:59.474813 truss-0.4.4/truss/truss_config.py
--rw-r--r--   0        0        0     2845 2023-04-26 11:28:59.474813 truss-0.4.4/truss/truss_gatherer.py
--rw-r--r--   0        0        0    40806 2023-04-26 11:28:59.474813 truss-0.4.4/truss/truss_handle.py
--rw-r--r--   0        0        0     5331 2023-04-26 11:28:59.474813 truss-0.4.4/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-04-26 11:28:59.474813 truss-0.4.4/truss/types.py
--rw-r--r--   0        0        0      227 2023-04-26 11:28:59.474813 truss-0.4.4/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-04-26 11:28:59.474813 truss-0.4.4/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-04-26 11:28:59.474813 truss-0.4.4/truss/util/jinja.py
--rw-r--r--   0        0        0     2018 2023-04-26 11:28:59.474813 truss-0.4.4/truss/util/path.py
--rw-r--r--   0        0        0     2317 2023-04-26 11:28:59.474813 truss-0.4.4/truss/validation.py
--rw-r--r--   0        0        0     7297 1970-01-01 00:00:00.000000 truss-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/LICENSE
+-rw-r--r--   0        0        0     5958 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/README.md
+-rw-r--r--   0        0        0     3316 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/ROADMAP.md
+-rw-r--r--   0        0        0      465 2023-04-21 04:27:43.131092 truss-0.4.4.dev3/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2209 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/cli.py
+-rw-r--r--   0        0        0     2742 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/constants.py
+-rw-r--r--   0        0        0     1237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     5130 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4511 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1976 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     1686 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6565 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/notebook.py
+-rw-r--r--   0        0        0    10874 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2388 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1409 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1849 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       82 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      979 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0     2616 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/docs/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0     1173 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0     1196 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1708 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1892 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/external_data_resolver.py
+-rw-r--r--   0        0        0     1352 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     3318 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     5511 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      416 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      733 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     5384 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      162 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     1054 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1666 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1898 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0      216 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0      669 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0     1006 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/__init__.py
+-rw-r--r--   0        0        0    19997 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/conftest.py
+-rw-r--r--   0        0        0      783 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    10483 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6937 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2157 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/server/common/test_external_resolver.py
+-rw-r--r--   0        0        0     1910 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_build.py
+-rw-r--r--   0        0        0     2359 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     2605 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    31937 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    12070 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_config.py
+-rw-r--r--   0        0        0     2845 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    40806 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_handle.py
+-rw-r--r--   0        0        0     5331 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/types.py
+-rw-r--r--   0        0        0      227 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/jinja.py
+-rw-r--r--   0        0        0     2018 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/path.py
+-rw-r--r--   0        0        0     2317 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/validation.py
+-rw-r--r--   0        0        0     7302 1970-01-01 00:00:00.000000 truss-0.4.4.dev3/PKG-INFO
```

### Comparing `truss-0.4.4/CODE_OF_CONDUCT.md` & `truss-0.4.4.dev3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/CONTRIBUTING.md` & `truss-0.4.4.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/LICENSE` & `truss-0.4.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/README.md` & `truss-0.4.4.dev3/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/ROADMAP.md` & `truss-0.4.4.dev3/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/pyproject.toml` & `truss-0.4.4.dev3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.4"
+version = "0.4.4dev3"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.4/truss/blob/blob_backend_registry.py` & `truss-0.4.4.dev3/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/blob/http_public_blob_backend.py` & `truss-0.4.4.dev3/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/build.py` & `truss-0.4.4.dev3/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/cli.py` & `truss-0.4.4.dev3/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/constants.py` & `truss-0.4.4.dev3/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/image_builder/image_builder.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/image_builder/util.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/local_loader/train_local.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/contexts/local_loader/utils.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/docker.py` & `truss-0.4.4.dev3/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/environment_inference/requirements_inference.py` & `truss-0.4.4.dev3/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/errors.py` & `truss-0.4.4.dev3/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/local/local_config.py` & `truss-0.4.4.dev3/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/local/local_config_handler.py` & `truss-0.4.4.dev3/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_framework.py` & `truss-0.4.4.dev3/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/__init__.py` & `truss-0.4.4.dev3/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.4.dev3/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/keras.py` & `truss-0.4.4.dev3/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/lightgbm.py` & `truss-0.4.4.dev3/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/mlflow.py` & `truss-0.4.4.dev3/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/pytorch.py` & `truss-0.4.4.dev3/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/sklearn.py` & `truss-0.4.4.dev3/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_frameworks/xgboost.py` & `truss-0.4.4.dev3/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/model_inference.py` & `truss-0.4.4.dev3/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/patch/calc_patch.py` & `truss-0.4.4.dev3/truss/patch/calc_patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,30 +130,22 @@
     root: Path,
     previous_root_path_content_hashes: Dict[str, str],
     ignore_patterns: Optional[List[str]],
 ) -> Dict[str, List[str]]:
     """
     TODO(pankaj) add support for directory creation in patch
     """
-    root_relative_new_paths = set(
-        (str(path.relative_to(root)) for path in root.glob("**/*"))
-    )
-    unignored_new_paths = _calc_unignored_paths(
-        root, root_relative_new_paths, ignore_patterns
-    )
+    unignored_paths = _calc_unignored_paths(root, ignore_patterns)
     previous_root_relative_paths = set(previous_root_path_content_hashes.keys())
-    unignored_prev_paths = _calc_unignored_paths(
-        root, previous_root_relative_paths, ignore_patterns
-    )
 
-    added_paths = unignored_new_paths - unignored_prev_paths
-    removed_paths = unignored_prev_paths - unignored_new_paths
+    added_paths = unignored_paths - previous_root_relative_paths
+    removed_paths = previous_root_relative_paths - unignored_paths
 
     updated_paths = set()
-    common_paths = unignored_new_paths.intersection(unignored_prev_paths)
+    common_paths = unignored_paths.intersection(previous_root_relative_paths)
     for path in common_paths:
         full_path: Path = root / path
         if full_path.is_file():
             content_hash = file_content_hash_str(full_path)
             previous_content_hash = previous_root_path_content_hashes[path]
             if content_hash != previous_content_hash:
                 updated_paths.add(path)
@@ -162,26 +154,27 @@
         "added": list(added_paths),
         "updated": list(updated_paths),
         "removed": list(removed_paths),
     }
 
 
 def _calc_unignored_paths(
-    root: Path,
-    root_relative_paths: Set[str],
-    ignore_patterns: Optional[List[str]] = None,
+    root: Path, ignore_patterns: Optional[List[str]] = None
 ) -> Set[str]:
     root_relative_ignored_paths = set()
     if ignore_patterns is not None:
         for ignore_pattern in ignore_patterns:
             ignored_paths_for_pattern = set(
                 (str(path.relative_to(root)) for path in root.glob(ignore_pattern))
             )
             root_relative_ignored_paths.update(ignored_paths_for_pattern)
 
+    root_relative_paths = set(
+        (str(path.relative_to(root)) for path in root.glob("**/*"))
+    )
     return root_relative_paths - root_relative_ignored_paths
 
 
 def _calc_config_patches(
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> Optional[List[Patch]]:
     """Calculate patch based on changes to config.
```

### Comparing `truss-0.4.4/truss/patch/dir_signature.py` & `truss-0.4.4.dev3/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/patch/hash.py` & `truss-0.4.4.dev3/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/patch/types.py` & `truss-0.4.4.dev3/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/readme_generator.py` & `truss-0.4.4.dev3/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/README.md.jinja` & `truss-0.4.4.dev3/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/base.Dockerfile.jinja` & `truss-0.4.4.dev3/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/application.py` & `truss-0.4.4.dev3/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/endpoints.py` & `truss-0.4.4.dev3/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/helpers/errors.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/helpers/types.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/control/control/server.py` & `truss-0.4.4.dev3/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/custom/model/model.py` & `truss-0.4.4.dev3/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/docs/README.md` & `truss-0.4.4.dev3/truss/templates/docs/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/keras/model/model.py` & `truss-0.4.4.dev3/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/lightgbm/model/model.py` & `truss-0.4.4.dev3/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/mlflow/model/model.py` & `truss-0.4.4.dev3/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/pipeline/model/model.py` & `truss-0.4.4.dev3/truss/templates/pipeline/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/pytorch/model/model.py` & `truss-0.4.4.dev3/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/server/common/external_data_resolver.py` & `truss-0.4.4.dev3/truss/templates/server/common/external_data_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/server/common/logging.py` & `truss-0.4.4.dev3/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/server/common/serialization.py` & `truss-0.4.4.dev3/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/server/common/truss_server.py` & `truss-0.4.4.dev3/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/server/inference_server.py` & `truss-0.4.4.dev3/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/server/model_wrapper.py` & `truss-0.4.4.dev3/truss/templates/server/model_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import importlib
 import inspect
 import logging
-import os
 import sys
 import time
 import traceback
 from enum import Enum
 from pathlib import Path
 from threading import Lock, Thread
 from typing import Dict, Optional, Union
 
 import kserve
 from cloudevents.http import CloudEvent
 from common.external_data_resolver import download_external_data  # noqa: E402
-from common.retry import retry
 from kserve.grpc.grpc_predict_v2_pb2 import ModelInferRequest, ModelInferResponse
 from shared.secrets_resolver import SecretsResolver
 
 MODEL_BASENAME = "model"
 
-NUM_LOAD_RETRIES = int(os.environ.get("NUM_LOAD_RETRIES_TRUSS", "3"))
-
 
 class ModelWrapper(kserve.Model):
     class Status(Enum):
         NOT_READY = 0
         LOADING = 1
         READY = 2
         FAILED = 3
@@ -111,21 +107,15 @@
         if _signature_accepts_keyword_arg(model_class_signature, "data_dir"):
             model_init_params["data_dir"] = data_dir
         if _signature_accepts_keyword_arg(model_class_signature, "secrets"):
             model_init_params["secrets"] = SecretsResolver.get_secrets(self._config)
         self._model = model_class(**model_init_params)
 
         if hasattr(self._model, "load"):
-            retry(
-                self._model.load,
-                NUM_LOAD_RETRIES,
-                self.logger.warn,
-                "Failed to load model.",
-                gap_seconds=1.0,
-            )
+            self._model.load()
 
     def preprocess(
         self,
         payload: Union[Dict, CloudEvent, ModelInferRequest],
         headers: Optional[Dict[str, str]] = None,
     ) -> Union[Dict, ModelInferRequest]:
         if not hasattr(self._model, "preprocess"):
```

### Comparing `truss-0.4.4/truss/templates/server.Dockerfile.jinja` & `truss-0.4.4.dev3/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/shared/secrets_resolver.py` & `truss-0.4.4.dev3/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/sklearn/model/model.py` & `truss-0.4.4.dev3/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/training/job.py` & `truss-0.4.4.dev3/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/templates/xgboost/model/model.py` & `truss-0.4.4.dev3/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/auto-mpg.data` & `truss-0.4.4.dev3/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/happy.ipynb` & `truss-0.4.4.dev3/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.4.dev3/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.4.dev3/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/readme_int_example.md` & `truss-0.4.4.dev3/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/readme_no_example.md` & `truss-0.4.4.dev3/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/readme_str_example.md` & `truss-0.4.4.dev3/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/test_truss/config.yaml` & `truss-0.4.4.dev3/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/test_data/test_truss/model/model.py` & `truss-0.4.4.dev3/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/conftest.py` & `truss-0.4.4.dev3/truss/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -771,44 +771,7 @@
 ) -> Path:
     dir_path = where_dir / truss_name
     handle = init(str(dir_path))
     if handle_ops is not None:
         handle_ops(handle)
     handle.spec.model_class_filepath.write_text(model_code)
     return dir_path
-
-
-class Helpers:
-    @staticmethod
-    @contextlib.contextmanager
-    def file_content(file_path: Path, content: str):
-        orig_content = file_path.read_text()
-        try:
-            file_path.write_text(content)
-            yield
-        finally:
-            file_path.write_text(orig_content)
-
-    @staticmethod
-    @contextlib.contextmanager
-    def sys_path(path: Path):
-        try:
-            sys.path.append(str(path))
-            yield
-        finally:
-            sys.path.pop()
-
-    @staticmethod
-    @contextlib.contextmanager
-    def env_var(var: str, value: str):
-        orig_environ = os.environ.copy()
-        try:
-            os.environ[var] = value
-            yield
-        finally:
-            os.environ.clear()
-            os.environ.update(orig_environ)
-
-
-@pytest.fixture
-def helpers():
-    return Helpers()
```

### Comparing `truss-0.4.4/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.4.dev3/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/local/test_local_config_handler.py` & `truss-0.4.4.dev3/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/patch/test_calc_patch.py` & `truss-0.4.4.dev3/truss/tests/patch/test_calc_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,31 +115,14 @@
     patches = calc_truss_patch(
         custom_model_truss_dir,
         prev_sign,
     )
     assert len(patches) == 0
 
 
-def test_calc_truss_ignore_pycache_existing(custom_model_truss_dir: Path):
-    # If __pycache__ existed before and there are no changes, there should be no
-    # patches.
-    top_pycache_path = custom_model_truss_dir / "__pycache__"
-    top_pycache_path.mkdir()
-    (top_pycache_path / "bla.pyc").touch()
-    model_pycache_path = custom_model_truss_dir / "model" / "__pycache__"
-    model_pycache_path.mkdir()
-    (model_pycache_path / "foo.pyo").touch()
-    sign = calc_truss_signature(custom_model_truss_dir)
-    patches = calc_truss_patch(
-        custom_model_truss_dir,
-        sign,
-    )
-    assert len(patches) == 0
-
-
 def test_calc_truss_ignore_changes_outside_patch_relevant_dirs(
     custom_model_truss_dir: Path,
 ):
     prev_sign = calc_truss_signature(custom_model_truss_dir)
     top_pycache_path = custom_model_truss_dir / "__pycache__"
     top_pycache_path.mkdir()
     (top_pycache_path / "README.md").touch()
```

### Comparing `truss-0.4.4/truss/tests/patch/test_hash.py` & `truss-0.4.4.dev3/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/samples.py` & `truss-0.4.4.dev3/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/templates/control/control/test_server.py` & `truss-0.4.4.dev3/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.4.dev3/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.4.dev3/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/templates/server/common/test_external_resolver.py` & `truss-0.4.4.dev3/truss/tests/templates/server/common/test_external_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_backward.py` & `truss-0.4.4.dev3/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_build.py` & `truss-0.4.4.dev3/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_config.py` & `truss-0.4.4.dev3/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_context_builder_image.py` & `truss-0.4.4.dev3/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_docker.py` & `truss-0.4.4.dev3/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_model_inference.py` & `truss-0.4.4.dev3/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_notebooks.py` & `truss-0.4.4.dev3/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.4.dev3/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_truss_gatherer.py` & `truss-0.4.4.dev3/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_truss_handle.py` & `truss-0.4.4.dev3/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/tests/test_validation.py` & `truss-0.4.4.dev3/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/truss_config.py` & `truss-0.4.4.dev3/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/truss_gatherer.py` & `truss-0.4.4.dev3/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/truss_handle.py` & `truss-0.4.4.dev3/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/truss_spec.py` & `truss-0.4.4.dev3/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/types.py` & `truss-0.4.4.dev3/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/util/gpu.py` & `truss-0.4.4.dev3/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/util/path.py` & `truss-0.4.4.dev3/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/truss/validation.py` & `truss-0.4.4.dev3/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4/PKG-INFO` & `truss-0.4.4.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.4
+Version: 0.4.4.dev3
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.11
```

