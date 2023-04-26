# Comparing `tmp/flytekit-1.6.0a1.tar.gz` & `tmp/flytekit-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.0a1.tar", last modified: Wed Apr 26 20:37:15 2023, max compression
+gzip compressed data, was "flytekit-1.6.0b0.tar", last modified: Wed Apr 19 20:54:19 2023, max compression
```

## Comparing `flytekit-1.6.0a1.tar` & `flytekit-1.6.0b0.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.077343 flytekit-1.6.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-26 20:37:15.077343 flytekit-1.6.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.029343 flytekit-1.6.0a1/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-26 20:37:08.000000 flytekit-1.6.0a1/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.029343 flytekit-1.6.0a1/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.033343 flytekit-1.6.0a1/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.033343 flytekit-1.6.0a1/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.033343 flytekit-1.6.0a1/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.033343 flytekit-1.6.0a1/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.033343 flytekit-1.6.0a1/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.037343 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.037343 flytekit-1.6.0a1/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    35938 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.049343 flytekit-1.6.0a1/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    75423 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.049343 flytekit-1.6.0a1/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.049343 flytekit-1.6.0a1/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.049343 flytekit-1.6.0a1/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.053343 flytekit-1.6.0a1/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.053343 flytekit-1.6.0a1/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.053343 flytekit-1.6.0a1/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.053343 flytekit-1.6.0a1/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.053343 flytekit-1.6.0a1/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.053343 flytekit-1.6.0a1/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.057343 flytekit-1.6.0a1/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.057343 flytekit-1.6.0a1/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.057343 flytekit-1.6.0a1/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.057343 flytekit-1.6.0a1/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.057343 flytekit-1.6.0a1/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/interfaces/stats/taggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.065343 flytekit-1.6.0a1/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.065343 flytekit-1.6.0a1/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.069343 flytekit-1.6.0a1/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.069343 flytekit-1.6.0a1/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.069343 flytekit-1.6.0a1/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.073343 flytekit-1.6.0a1/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.073343 flytekit-1.6.0a1/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.073343 flytekit-1.6.0a1/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.073343 flytekit-1.6.0a1/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.073343 flytekit-1.6.0a1/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.073343 flytekit-1.6.0a1/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.073343 flytekit-1.6.0a1/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.077343 flytekit-1.6.0a1/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.029343 flytekit-1.6.0a1/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-26 20:37:14.000000 flytekit-1.6.0a1/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-26 20:37:14.000000 flytekit-1.6.0a1/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:37:14.000000 flytekit-1.6.0a1/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-26 20:37:14.000000 flytekit-1.6.0a1/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-26 20:37:14.000000 flytekit-1.6.0a1/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 20:37:14.000000 flytekit-1.6.0a1/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:15.077343 flytekit-1.6.0a1/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-26 20:36:40.000000 flytekit-1.6.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 20:37:15.077343 flytekit-1.6.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-26 20:37:08.000000 flytekit-1.6.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-19 20:54:16.000000 flytekit-1.6.0b0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.370920 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.370920 flytekit-1.6.0b0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    35808 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75336 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-19 20:54:16.000000 flytekit-1.6.0b0/setup.py
```

### Comparing `flytekit-1.6.0a1/LICENSE` & `flytekit-1.6.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/MANIFEST.in` & `flytekit-1.6.0b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/PKG-INFO` & `flytekit-1.6.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0a1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0a1/README.md` & `flytekit-1.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/__init__.py` & `flytekit-1.6.0b0/flytekit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,14 @@
 from flytekit.core.resources import Resources
 from flytekit.core.schedule import CronSchedule, FixedRate
 from flytekit.core.task import Secret, reference_task, task
 from flytekit.core.workflow import ImperativeWorkflow as Workflow
 from flytekit.core.workflow import WorkflowFailurePolicy, reference_workflow, workflow
 from flytekit.deck import Deck
 from flytekit.extras import pytorch, sklearn, tensorflow
-from flytekit.image_spec import ImageSpec
 from flytekit.loggers import logger
 from flytekit.models.common import Annotations, AuthRole, Labels
 from flytekit.models.core.execution import WorkflowExecutionPhase
 from flytekit.models.core.types import BlobType
 from flytekit.models.documentation import Description, Documentation, SourceCode
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
@@ -237,15 +236,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.0a1"
+__version__ = "1.6.0b0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.0a1/flytekit/bin/entrypoint.py` & `flytekit-1.6.0b0/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.0b0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.0b0/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/auth/keyring.py` & `flytekit-1.6.0b0/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/auth/token_client.py` & `flytekit-1.6.0b0/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/auth_helper.py` & `flytekit-1.6.0b0/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/friendly.py` & `flytekit-1.6.0b0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.0b0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.0b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/helpers.py` & `flytekit-1.6.0b0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clients/raw.py` & `flytekit-1.6.0b0/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.0b0/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clis/helpers.py` & `flytekit-1.6.0b0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing
 from datetime import datetime, timedelta
 
-import rich_click as click
+import click
 
 from flytekit.clis.sdk_in_container.helpers import get_and_save_remote_with_click_context
 from flytekit.clis.sdk_in_container.run import DateTimeType, DurationParamType
 
 _backfill_help = """
 The backfill command generates and registers a new workflow based on the input launchplan to run an
 automated backfill. The workflow can be managed using the Flyte UI and can be canceled, relaunched, and recovered.
 
-    - ``launchplan`` refers to the name of the Launchplan
-    - ``launchplan_version`` is optional and should be a valid version for a Launchplan version.
+- ``launchplan`` refers to the name of the Launchplan
+- ``launchplan_version`` is optional and should be a valid version for a Launchplan version.
 """
 
 
 def resolve_backfill_window(
     from_date: datetime = None,
     to_date: datetime = None,
     backfill_window: timedelta = None,
@@ -164,16 +164,15 @@
             launchplan_version=launchplan_version,
             execution_name=execution_name,
             version=version,
             dry_run=dry_run,
             execute=execute,
             parallel=parallel,
         )
-        if dry_run:
-            return
-        console_url = remote.generate_console_url(entity)
-        if execute:
-            click.secho(f"\n Execution launched {console_url} to see execution in the console.", fg="green")
-            return
-        click.secho(f"\n Workflow registered at {console_url}", fg="green")
+        if entity:
+            console_url = remote.generate_console_url(entity)
+            if execute:
+                click.secho(f"\n Execution launched {console_url} to see execution in the console.", fg="green")
+                return
+            click.secho(f"\n Workflow registered at {console_url}", fg="green")
     except StopIteration as e:
         click.secho(f"{e.value}", fg="red")
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import pathlib
 import typing
 
-import rich_click as click
+import click
 from typing_extensions import OrderedDict
 
 from flytekit.clis.sdk_in_container.constants import CTX_MODULE, CTX_PROJECT_ROOT
 from flytekit.clis.sdk_in_container.run import RUN_LEVEL_PARAMS_KEY, get_entities_in_file, load_naive_entity
 from flytekit.configuration import ImageConfig, SerializationSettings
 from flytekit.core.base_task import PythonTask
 from flytekit.core.workflow import PythonFunctionWorkflow
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import rich_click as _click
+import click as _click
 
 CTX_PROJECT = "project"
 CTX_DOMAIN = "domain"
 CTX_VERSION = "version"
 CTX_TEST = "test"
 CTX_PACKAGES = "pkgs"
 CTX_NOTIFICATIONS = "notifications"
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import replace
 from typing import Optional
 
-import rich_click as click
+import click
 
 from flytekit.clis.sdk_in_container.constants import CTX_CONFIG_FILE
 from flytekit.configuration import Config, ImageConfig, get_config_file
 from flytekit.loggers import cli_logger
 from flytekit.remote.remote import FlyteRemote
 
 FLYTE_REMOTE_INSTANCE_KEY = "flyte_remote"
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import rich_click as click
+import click
 from cookiecutter.main import cookiecutter
 
 
 @click.command("init")
 @click.option(
     "--template",
     default="simple-example",
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import rich_click as click
+import click
 
 from flytekit.clis.sdk_in_container.helpers import get_and_save_remote_with_click_context
 from flytekit.models.launch_plan import LaunchPlanState
 
 _launchplan_help = """
 The launchplan command activates or deactivates a specified or the latest version of the launchplan.
 If ``--activate`` is chosen then the previous version of the launchplan will be deactivated.
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-import rich_click as click
+import click
 
 from flytekit.clis.helpers import display_help_with_error
 from flytekit.clis.sdk_in_container import constants
 from flytekit.configuration import (
     DEFAULT_RUNTIME_PYTHON_INTERPRETER,
     FastSerializationSettings,
     ImageConfig,
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
+import click
 import grpc
-import rich_click as click
 from google.protobuf.json_format import MessageToJson
 
 from flytekit import configuration
 from flytekit.clis.sdk_in_container.backfill import backfill
 from flytekit.clis.sdk_in_container.build import build
 from flytekit.clis.sdk_in_container.constants import CTX_CONFIG_FILE, CTX_PACKAGES, CTX_VERBOSE
 from flytekit.clis.sdk_in_container.init import init
@@ -70,15 +70,15 @@
     if isinstance(e, grpc.RpcError):
         pretty_print_grpc_error(e)
         return
 
     click.secho(f"Failed with Unknown Exception {type(e)} Reason: {e}", fg="red")  # noqa
 
 
-class ErrorHandlingCommand(click.RichGroup):
+class ErrorHandlingCommand(click.Group):
     def invoke(self, ctx: click.Context) -> typing.Any:
         try:
             return super().invoke(ctx)
         except Exception as e:
             if CTX_VERBOSE in ctx.obj and ctx.obj[CTX_VERBOSE]:
                 print("Verbose mode on")
                 raise e
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import typing
 
-import rich_click as click
+import click
 
 from flytekit.clis.helpers import display_help_with_error
 from flytekit.clis.sdk_in_container import constants
 from flytekit.clis.sdk_in_container.helpers import get_and_save_remote_with_click_context, patch_image_config
 from flytekit.configuration import ImageConfig
 from flytekit.configuration.default_images import DefaultImages
 from flytekit.loggers import cli_logger
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import os
 import pathlib
 import typing
 from dataclasses import dataclass
 from typing import cast
 
-import rich_click as click
+import click
 from dataclasses_json import DataClassJsonMixin
 from pytimeparse import parse
 from typing_extensions import get_args
 
 from flytekit import BlobType, Literal, Scalar
 from flytekit.clis.sdk_in_container.constants import (
     CTX_CONFIG_FILE,
@@ -606,15 +606,15 @@
 
         if run_level_params.get("dump_snippet"):
             dump_flyte_remote_snippet(execution, project, domain)
 
     return _run
 
 
-class WorkflowCommand(click.RichGroup):
+class WorkflowCommand(click.MultiCommand):
     """
     click multicommand at the python file layer, subcommands should be all the workflows in the file.
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._filename = pathlib.Path(filename).resolve()
@@ -674,15 +674,15 @@
             params=params,
             callback=run_command(ctx, entity),
             help=f"Run {module}.{exe_entity} in script mode",
         )
         return cmd
 
 
-class RunCommand(click.RichGroup):
+class RunCommand(click.MultiCommand):
     """
     A click command group for registering and executing flyte workflows & tasks in a file.
     """
 
     def __init__(self, *args, **kwargs):
         params = get_workflow_command_base_params()
         super().__init__(*args, params=params, **kwargs)
```

### Comparing `flytekit-1.6.0a1/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import typing
 from enum import Enum as _Enum
 
-import rich_click as click
+import click
 
 from flytekit.clis.sdk_in_container import constants
 from flytekit.clis.sdk_in_container.constants import CTX_PACKAGES
 from flytekit.configuration import FastSerializationSettings, ImageConfig, SerializationSettings
 from flytekit.exceptions.scopes import system_entry_point
 from flytekit.tools.fast_registration import fast_package
 from flytekit.tools.repo import serialize_to_folder
@@ -65,15 +65,15 @@
         flytekit_virtualenv_root=flytekit_virtualenv_root,
         python_interpreter=python_interpreter,
     )
 
     serialize_to_folder(pkgs, serialization_settings, local_source_root, folder)
 
 
-@click.group("serialize", cls=click.RichGroup)
+@click.group("serialize")
 @click.option(
     "--image",
     required=False,
     default=lambda: os.environ.get("FLYTE_INTERNAL_IMAGE", ""),
     help="Text tag, for example ``somedocker.com/myimage:someversion123``",
 )
 @click.option(
@@ -120,15 +120,15 @@
         import flytekit
 
         flytekit_install_loc = os.path.abspath(flytekit.__file__)
         ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT] = os.path.dirname(flytekit_install_loc)
         ctx.obj[CTX_PYTHON_INTERPRETER] = sys.executable
 
 
-@click.command("workflows", cls=click.RichCommand)
+@click.command("workflows")
 # For now let's just assume that the directory needs to exist. If you're docker run -v'ing, docker will create the
 # directory for you so it shouldn't be a problem.
 @click.option("-f", "--folder", type=click.Path(exists=True))
 @click.pass_context
 def workflows(ctx, folder=None):
 
     if folder:
@@ -144,21 +144,21 @@
         image=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
-@click.group("fast", cls=click.RichGroup)
+@click.group("fast")
 @click.pass_context
 def fast(ctx):
     pass
 
 
-@click.command("workflows", cls=click.RichCommand)
+@click.command("workflows")
 @click.option(
     "--deref-symlinks",
     default=False,
     is_flag=True,
     help="Enables symlink dereferencing when packaging files in fast registration",
 )
 @click.option("-f", "--folder", type=click.Path(exists=True))
```

### Comparing `flytekit-1.6.0a1/flytekit/configuration/__init__.py` & `flytekit-1.6.0b0/flytekit/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,15 +791,14 @@
             version=self.version,
             image_config=self.image_config,
             env=self.env.copy() if self.env else None,
             git_repo=self.git_repo,
             flytekit_virtualenv_root=self.flytekit_virtualenv_root,
             python_interpreter=self.python_interpreter,
             fast_serialization_settings=self.fast_serialization_settings,
-            source_root=self.source_root,
         )
 
     def should_fast_serialize(self) -> bool:
         """
         Whether or not the serialization settings specify that entities should be serialized for fast registration.
         """
         return self.fast_serialization_settings is not None and self.fast_serialization_settings.enabled
@@ -842,15 +841,14 @@
         version: str
         image_config: ImageConfig
         env: Optional[Dict[str, str]] = None
         git_repo: Optional[str] = None
         flytekit_virtualenv_root: Optional[str] = None
         python_interpreter: Optional[str] = None
         fast_serialization_settings: Optional[FastSerializationSettings] = None
-        source_root: Optional[str] = None
 
         def with_fast_serialization_settings(self, fss: fast_serialization_settings) -> SerializationSettings.Builder:
             self.fast_serialization_settings = fss
             return self
 
         def build(self) -> SerializationSettings:
             return SerializationSettings(
@@ -859,9 +857,8 @@
                 version=self.version,
                 image_config=self.image_config,
                 env=self.env,
                 git_repo=self.git_repo,
                 flytekit_virtualenv_root=self.flytekit_virtualenv_root,
                 python_interpreter=self.python_interpreter,
                 fast_serialization_settings=self.fast_serialization_settings,
-                source_root=self.source_root,
             )
```

### Comparing `flytekit-1.6.0a1/flytekit/configuration/default_images.py` & `flytekit-1.6.0b0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/configuration/feature_flags.py` & `flytekit-1.6.0b0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/configuration/file.py` & `flytekit-1.6.0b0/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/configuration/internal.py` & `flytekit-1.6.0b0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/annotation.py` & `flytekit-1.6.0b0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/base_sql_task.py` & `flytekit-1.6.0b0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/base_task.py` & `flytekit-1.6.0b0/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/checkpointer.py` & `flytekit-1.6.0b0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/class_based_resolver.py` & `flytekit-1.6.0b0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/condition.py` & `flytekit-1.6.0b0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/constants.py` & `flytekit-1.6.0b0/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/container_task.py` & `flytekit-1.6.0b0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/context_manager.py` & `flytekit-1.6.0b0/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/data_persistence.py` & `flytekit-1.6.0b0/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/docstring.py` & `flytekit-1.6.0b0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.0b0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/gate.py` & `flytekit-1.6.0b0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/interface.py` & `flytekit-1.6.0b0/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/launch_plan.py` & `flytekit-1.6.0b0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/local_cache.py` & `flytekit-1.6.0b0/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/map_task.py` & `flytekit-1.6.0b0/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/mock_stats.py` & `flytekit-1.6.0b0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/node.py` & `flytekit-1.6.0b0/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/node_creation.py` & `flytekit-1.6.0b0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/notification.py` & `flytekit-1.6.0b0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/pod_template.py` & `flytekit-1.6.0b0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/promise.py` & `flytekit-1.6.0b0/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/python_auto_container.py` & `flytekit-1.6.0b0/flytekit/core/python_auto_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,17 +177,16 @@
             return self._get_container(settings)
 
     def _get_container(self, settings: SerializationSettings) -> _task_model.Container:
         env = {}
         for elem in (settings.env, self.environment):
             if elem:
                 env.update(elem)
-        if settings.fast_serialization_settings is None or not settings.fast_serialization_settings.enabled:
-            if isinstance(self.container_image, ImageSpec):
-                self.container_image.source_root = settings.source_root
+        if isinstance(self.container_image, ImageSpec):
+            self.container_image.source_root = settings.source_root
         return _get_container_definition(
             image=get_registerable_container_image(self.container_image, settings.image_config),
             command=[],
             args=self.get_command(settings=settings),
             data_loading_config=None,
             environment=env,
             storage_request=self.resources.requests.storage,
```

### Comparing `flytekit-1.6.0a1/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.0b0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/python_function_task.py` & `flytekit-1.6.0b0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/reference.py` & `flytekit-1.6.0b0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/reference_entity.py` & `flytekit-1.6.0b0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/resources.py` & `flytekit-1.6.0b0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/schedule.py` & `flytekit-1.6.0b0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/shim_task.py` & `flytekit-1.6.0b0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/task.py` & `flytekit-1.6.0b0/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/testing.py` & `flytekit-1.6.0b0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/tracker.py` & `flytekit-1.6.0b0/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/type_engine.py` & `flytekit-1.6.0b0/flytekit/core/type_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -995,25 +995,22 @@
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
         if type(python_val) != list:
             raise TypeTransformerFailedError("Expected a list")
 
         if ListTransformer.is_batchable(python_type):
             from flytekit.types.pickle.pickle import BatchSize, FlytePickle
 
-            batch_size = len(python_val)  # default batch size
+            batchSize = len(python_val)  # default batch size
             # parse annotated to get the number of items saved in a pickle file.
             if get_origin(python_type) is Annotated:
                 for annotation in get_args(python_type)[1:]:
                     if isinstance(annotation, BatchSize):
-                        batch_size = annotation.val
+                        batchSize = annotation.val
                         break
-            if batch_size > 0:
-                lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batch_size], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batch_size)]  # type: ignore
-            else:
-                lit_list = []
+            lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batchSize], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batchSize)]  # type: ignore
         else:
             t = self.get_sub_type(python_type)
             lit_list = [TypeEngine.to_literal(ctx, x, t, expected.collection_type) for x in python_val]  # type: ignore
         return Literal(collection=LiteralCollection(literals=lit_list))
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> typing.List[typing.Any]:  # type: ignore
         try:
```

### Comparing `flytekit-1.6.0a1/flytekit/core/type_helpers.py` & `flytekit-1.6.0b0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/utils.py` & `flytekit-1.6.0b0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/core/workflow.py` & `flytekit-1.6.0b0/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/deck/deck.py` & `flytekit-1.6.0b0/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/deck/html/template.html` & `flytekit-1.6.0b0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/deck/renderer.py` & `flytekit-1.6.0b0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/exceptions/scopes.py` & `flytekit-1.6.0b0/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/exceptions/system.py` & `flytekit-1.6.0b0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/exceptions/user.py` & `flytekit-1.6.0b0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extend/__init__.py` & `flytekit-1.6.0b0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.0b0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.0b0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.0b0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/pytorch/native.py` & `flytekit-1.6.0b0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.0b0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/sklearn/native.py` & `flytekit-1.6.0b0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.0b0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/tasks/shell.py` & `flytekit-1.6.0b0/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.0b0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.0b0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.0b0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/image_spec/image_spec.py` & `flytekit-1.6.0b0/flytekit/image_spec/image_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import base64
 import hashlib
 import os
 import sys
 import typing
 from abc import abstractmethod
-from copy import copy
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import List, Optional
 
 import click
 import docker
-import requests
 from dataclasses_json import dataclass_json
 from docker.errors import APIError, ImageNotFound
 
 
 @dataclass_json
 @dataclass
 class ImageSpec:
@@ -54,39 +52,30 @@
             container_image = f"{self.registry}/{container_image}"
         return container_image
 
     def exist(self) -> bool:
         """
         Check if the image exists in the registry.
         """
+        client = docker.from_env()
         try:
-            client = docker.from_env()
             if self.registry:
                 client.images.get_registry_data(self.image_name())
             else:
                 client.images.get(self.image_name())
             return True
         except APIError as e:
             if e.response.status_code == 404:
                 return False
+            if e.response.status_code == 403:
+                click.secho("Permission denied. Please login you docker registry first.", fg="red")
+                raise e
+            return False
         except ImageNotFound:
             return False
-        except Exception as e:
-            tag = calculate_hash_from_image_spec(self)
-            # if docker engine is not running locally
-            response = requests.get(f"https://hub.docker.com/v2/repositories/{self.registry}/{self.name}/tags/{tag}")
-            if response.status_code == 200:
-                return True
-            response = requests.get(f"https://ghcr.io/v2/{self.registry}/{self.name}/manifests/{tag}")
-            if response.status_code == 200:
-                return True
-
-            click.secho(f"Failed to check if the image exists with error : {e}", fg="red")
-            click.secho("Flytekit assumes that the image already exists.", fg="blue")
-            return True
 
     def __hash__(self):
         return hash(self.to_json())
 
 
 class ImageSpecBuilder:
     @abstractmethod
@@ -123,18 +112,18 @@
 
 
 @lru_cache(maxsize=None)
 def calculate_hash_from_image_spec(image_spec: ImageSpec):
     """
     Calculate the hash from the image spec.
     """
-    spec = copy(image_spec)
-    spec.source_root = hash_directory(image_spec.source_root) if image_spec.source_root else b""
     image_spec_bytes = bytes(image_spec.to_json(), "utf-8")
-    tag = base64.urlsafe_b64encode(hashlib.md5(image_spec_bytes).digest()).decode("ascii")
+    source_root_bytes = hash_directory(image_spec.source_root) if image_spec.source_root else b""
+    h = hashlib.md5(image_spec_bytes + source_root_bytes)
+    tag = base64.urlsafe_b64encode(h.digest()).decode("ascii")
     # replace "=" with "." to make it a valid tag
     return tag.replace("=", ".")
 
 
 def hash_directory(path):
     """
     Return the SHA-256 hash of the directory at the given path.
```

### Comparing `flytekit-1.6.0a1/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.0b0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.0b0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/interfaces/random.py` & `flytekit-1.6.0b0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/interfaces/stats/client.py` & `flytekit-1.6.0b0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.0b0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/loggers.py` & `flytekit-1.6.0b0/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/admin/common.py` & `flytekit-1.6.0b0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/admin/task_execution.py` & `flytekit-1.6.0b0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/admin/workflow.py` & `flytekit-1.6.0b0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/annotation.py` & `flytekit-1.6.0b0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/array_job.py` & `flytekit-1.6.0b0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/common.py` & `flytekit-1.6.0b0/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/catalog.py` & `flytekit-1.6.0b0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/compiler.py` & `flytekit-1.6.0b0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/condition.py` & `flytekit-1.6.0b0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/errors.py` & `flytekit-1.6.0b0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/execution.py` & `flytekit-1.6.0b0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/identifier.py` & `flytekit-1.6.0b0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/types.py` & `flytekit-1.6.0b0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/core/workflow.py` & `flytekit-1.6.0b0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/documentation.py` & `flytekit-1.6.0b0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/dynamic_job.py` & `flytekit-1.6.0b0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/execution.py` & `flytekit-1.6.0b0/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/filters.py` & `flytekit-1.6.0b0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/interface.py` & `flytekit-1.6.0b0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/launch_plan.py` & `flytekit-1.6.0b0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/literals.py` & `flytekit-1.6.0b0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/matchable_resource.py` & `flytekit-1.6.0b0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/named_entity.py` & `flytekit-1.6.0b0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/node_execution.py` & `flytekit-1.6.0b0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/presto.py` & `flytekit-1.6.0b0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/project.py` & `flytekit-1.6.0b0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/qubole.py` & `flytekit-1.6.0b0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/schedule.py` & `flytekit-1.6.0b0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/security.py` & `flytekit-1.6.0b0/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/task.py` & `flytekit-1.6.0b0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/types.py` & `flytekit-1.6.0b0/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/models/workflow_closure.py` & `flytekit-1.6.0b0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/remote/__init__.py` & `flytekit-1.6.0b0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/remote/backfill.py` & `flytekit-1.6.0b0/flytekit/remote/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,31 +64,26 @@
     if schedule.cron_schedule is not None:
         cron_schedule = schedule.cron_schedule
     else:
         raise NotImplementedError("Currently backfilling only supports cron schedules.")
 
     logging.info(f"Generating backfill from {start_date} -> {end_date}. Parallel?[{parallel}]")
     wf = ImperativeWorkflow(name=f"backfill-{for_lp.name}")
-
-    input_name = schedule.kickoff_time_input_arg
     date_iter = croniter(cron_schedule.schedule, start_time=start_date, ret_type=datetime)
     prev_node = None
     actual_start = None
     actual_end = None
     while True:
         next_start_date = date_iter.get_next()
         if not actual_start:
             actual_start = next_start_date
         if next_start_date >= end_date:
             break
         actual_end = next_start_date
-        inputs = {}
-        if input_name:
-            inputs[input_name] = next_start_date
-        next_node = wf.add_launch_plan(for_lp, **inputs)
+        next_node = wf.add_launch_plan(for_lp, t=next_start_date)
         next_node = next_node.with_overrides(
             name=f"b-{next_start_date}", retries=per_node_retries, timeout=per_node_timeout
         )
         if not parallel:
             if prev_node:
                 prev_node.runs_before(next_node)
         prev_node = next_node
```

### Comparing `flytekit-1.6.0a1/flytekit/remote/entities.py` & `flytekit-1.6.0b0/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/remote/executions.py` & `flytekit-1.6.0b0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/remote/lazy_entity.py` & `flytekit-1.6.0b0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/remote/remote.py` & `flytekit-1.6.0b0/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/remote/remote_callable.py` & `flytekit-1.6.0b0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/testing/__init__.py` & `flytekit-1.6.0b0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/tools/fast_registration.py` & `flytekit-1.6.0b0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/tools/ignore.py` & `flytekit-1.6.0b0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/tools/module_loader.py` & `flytekit-1.6.0b0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/tools/repo.py` & `flytekit-1.6.0b0/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/tools/script_mode.py` & `flytekit-1.6.0b0/flytekit/tools/script_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import tarfile
 import tempfile
 import typing
 from pathlib import Path
 
 from flytekit import PythonFunctionTask
 from flytekit.core.tracker import get_full_module_path
-from flytekit.core.workflow import ImperativeWorkflow, WorkflowBase
+from flytekit.core.workflow import WorkflowBase
 
 
 def compress_scripts(source_path: str, destination: str, module_name: str):
     """
     Compresses the single script while maintaining the folder structure for that file.
 
     For example, given the follow file structure:
@@ -88,19 +88,15 @@
         script_file,
         script_file_destination,
     )
 
     # Try to copy other files to destination if tasks or workflows aren't in the same file
     for flyte_entity_name in mod.__dict__:
         flyte_entity = mod.__dict__[flyte_entity_name]
-        if (
-            isinstance(flyte_entity, (PythonFunctionTask, WorkflowBase))
-            and not isinstance(flyte_entity, ImperativeWorkflow)
-            and flyte_entity.instantiated_in
-        ):
+        if isinstance(flyte_entity, (PythonFunctionTask, WorkflowBase)) and flyte_entity.instantiated_in:
             copy_module_to_destination(
                 original_source_path, original_destination_path, flyte_entity.instantiated_in, visited
             )
 
 
 # Takes in a TarInfo and returns the modified TarInfo:
 # https://docs.python.org/3/library/tarfile.html#tarinfo-objects
```

### Comparing `flytekit-1.6.0a1/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.0b0/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/tools/subprocess.py` & `flytekit-1.6.0b0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/tools/translator.py` & `flytekit-1.6.0b0/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/directory/__init__.py` & `flytekit-1.6.0b0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/directory/types.py` & `flytekit-1.6.0b0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/file/__init__.py` & `flytekit-1.6.0b0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/file/file.py` & `flytekit-1.6.0b0/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.0b0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/pickle/pickle.py` & `flytekit-1.6.0b0/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/schema/types.py` & `flytekit-1.6.0b0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.0b0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/structured/__init__.py` & `flytekit-1.6.0b0/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.0b0/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/structured/bigquery.py` & `flytekit-1.6.0b0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.0b0/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.0b0/flytekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0a1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0a1/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.0b0/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/flytekit.egg-info/requires.txt` & `flytekit-1.6.0b0/flytekit.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -37,11 +37,10 @@
 diskcache>=5.2.1
 cloudpickle>=2.0.0
 cookiecutter>=1.7.3
 numpy
 gitpython
 kubernetes>=12.0.1
 rich
-rich_click
 
 [:python_version < "3.8.0"]
 singledispatchmethod
```

### Comparing `flytekit-1.6.0a1/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.0b0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0a1/setup.py` & `flytekit-1.6.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.0a1"
+__version__ = "1.6.0b0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -70,15 +70,14 @@
         "diskcache>=5.2.1",
         "cloudpickle>=2.0.0",
         "cookiecutter>=1.7.3",
         "numpy",
         "gitpython",
         "kubernetes>=12.0.1",
         "rich",
-        "rich_click",
     ],
     extras_require=extras_require,
     scripts=[
         "flytekit_scripts/flytekit_build_image.sh",
         "flytekit_scripts/flytekit_venv",
         "flytekit/bin/entrypoint.py",
     ],
```

