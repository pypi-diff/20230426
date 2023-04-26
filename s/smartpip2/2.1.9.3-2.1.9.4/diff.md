# Comparing `tmp/smartpip2-2.1.9.3.tar.gz` & `tmp/smartpip2-2.1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smartpip2-2.1.9.3.tar", last modified: Mon Oct 24 09:44:10 2022, max compression
+gzip compressed data, was "dist/smartpip2-2.1.9.4.tar", last modified: Wed Apr 26 09:55:12 2023, max compression
```

## Comparing `smartpip2-2.1.9.3.tar` & `smartpip2-2.1.9.4.tar`

### file list

```diff
@@ -1,1118 +1,1118 @@
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/
--rw-rw-r--   0 johnyan    (501) staff       (20)   274732 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/CHANGELOG.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)    13444 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/LICENSE
--rw-rw-r--   0 johnyan    (501) staff       (20)     1433 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/MANIFEST.in
--rw-rw-r--   0 johnyan    (501) staff       (20)      404 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/NOTICE
--rw-r--r--   0 johnyan    (501) staff       (20)    26641 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/PKG-INFO
--rw-rw-r--   0 johnyan    (501) staff       (20)    20139 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/README.md
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/
--rw-r--r--   0 johnyan    (501) staff       (20)     2751 2022-07-19 14:54:13.000000 smartpip2-2.1.9.3/airflow/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1368 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/__main__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/_vendor/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/
--rw-r--r--   0 johnyan    (501) staff       (20)     1430 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)       95 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/__main__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/
--rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18192 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/abstract.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14270 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/aiohttp_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12812 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/flask_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2222 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/flask_utils.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/
--rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10764 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/abstract.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/aiohttp_app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5023 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/flask_app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/cli.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1842 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/coroutine_wrappers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1441 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/decorator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1752 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/metrics.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/parameter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/produces.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/response.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9853 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/security.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11690 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/uri_parsing.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15533 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/validation.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/exceptions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2692 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/handlers.py
--rw-r--r--   0 johnyan    (501) staff       (20)      212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/http_facts.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4050 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/json_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/jsonifier.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/lifecycle.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/mock.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/
--rw-r--r--   0 johnyan    (501) staff       (20)      294 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15461 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/abstract.py
--rw-r--r--   0 johnyan    (501) staff       (20)      127 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/compat.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14505 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/openapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6782 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/secure.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/swagger2.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4444 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/options.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1926 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/problem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6810 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/resolver.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3408 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/setup.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/spec.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6515 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/_vendor/connexion/utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2320 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/alembic.ini
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api/
--rw-r--r--   0 johnyan    (501) staff       (20)     1550 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api/auth/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/auth/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api/auth/backend/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/auth/backend/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2258 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/auth/backend/basic_auth.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1342 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/auth/backend/default.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/auth/backend/deny_all.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5563 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/auth/backend/kerberos_auth.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1500 2022-07-04 11:00:25.000000 smartpip2-2.1.9.3/airflow/api/auth/backend/smart_auth.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api/client/
--rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/client/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2465 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/client/api_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/client/json_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2223 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/client/local_client.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api/common/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/
--rw-r--r--   0 johnyan    (501) staff       (20)     2045 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/delete_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)      329 2020-10-10 01:23:08.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/gen_dag_file.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1426 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/get_code.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1381 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/get_dag_run_state.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1982 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/get_dag_runs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1886 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/get_lineage.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/get_task.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1628 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/get_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14243 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/mark_tasks.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2833 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/pool.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4413 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api/common/experimental/trigger_dag.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api_connexion/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3303 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/config_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5383 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/connection_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dag_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8558 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dag_run_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2044 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dag_source_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5487 2022-07-05 00:33:48.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dagsetup_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2517 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/event_log_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/extra_link_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1732 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/health_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2618 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/import_error_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3649 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/log_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1560 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/plugin_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5506 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/pool_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/provider_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6330 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/role_and_permission_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2401 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/task_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11479 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/task_instance_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2509 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/user_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4008 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/variable_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1363 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/version_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3848 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/endpoints/xcom_endpoint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5017 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/exceptions.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api_connexion/openapi/
--rw-r--r--   0 johnyan    (501) staff       (20)   107667 2022-07-05 06:13:09.000000 smartpip2-2.1.9.3/airflow/api_connexion/openapi/v1.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     3655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/parameters.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/common_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/config_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1995 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/connection_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/dag_run_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/dag_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)      971 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/dag_source_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1349 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/enum_schemas.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1738 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/error_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/event_log_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/health_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/log_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1754 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/plugin_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2370 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/pool_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1452 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/provider_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2531 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/role_and_permission_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1327 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/sla_miss_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6966 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/task_instance_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2992 2021-08-06 13:05:03.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/task_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2331 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/user_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/variable_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/version_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1769 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/schemas/xcom_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/api_connexion/security.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/cli/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    59796 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/cli_parser.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/cli/commands/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6551 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/celery_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2366 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/cheat_sheet_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/config_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/connection_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13203 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/dag_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3345 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/db_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/info_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/jobs_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1740 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/kerberos_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/kubernetes_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1999 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/legacy_commands.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/plugins_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/pool_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3862 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/provider_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1582 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/role_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1379 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/rotate_fernet_key_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/scheduler_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/sync_perm_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/task_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8359 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/user_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3968 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/variable_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)      929 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/version_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)    20747 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/commands/webserver_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5290 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/cli/simple_table.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/common/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2022-07-03 02:40:42.000000 smartpip2-2.1.9.3/airflow/common/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9162 2022-07-03 03:12:30.000000 smartpip2-2.1.9.3/airflow/common/datax.py
--rw-r--r--   0 johnyan    (501) staff       (20)    56372 2022-10-24 08:23:55.000000 smartpip2-2.1.9.3/airflow/common/smartpip.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/compat/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/compat/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/compat/functools.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/config_templates/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/config_templates/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11726 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/config_templates/airflow_local_settings.py
--rw-r--r--   0 johnyan    (501) staff       (20)    75766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/config_templates/config.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1629 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/config_templates/config.yml.schema.json
--rw-r--r--   0 johnyan    (501) staff       (20)    44296 2022-08-26 06:07:49.000000 smartpip2-2.1.9.3/airflow/config_templates/default_airflow.cfg
--rw-r--r--   0 johnyan    (501) staff       (20)     4094 2022-08-01 06:06:39.000000 smartpip2-2.1.9.3/airflow/config_templates/default_celery.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2028 2022-07-03 06:20:29.000000 smartpip2-2.1.9.3/airflow/config_templates/default_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3770 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/config_templates/default_test.cfg
--rw-r--r--   0 johnyan    (501) staff       (20)     4700 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/config_templates/default_webserver_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)    44793 2022-07-22 10:03:34.000000 smartpip2-2.1.9.3/airflow/configuration.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/contrib/
--rw-r--r--   0 johnyan    (501) staff       (20)      821 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/contrib/dagsetup/
--rw-r--r--   0 johnyan    (501) staff       (20)       86 2020-10-10 01:23:08.000000 smartpip2-2.1.9.3/airflow/contrib/dagsetup/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7588 2022-09-27 06:26:39.000000 smartpip2-2.1.9.3/airflow/contrib/dagsetup/config_dagfile.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2586 2021-11-22 09:21:52.000000 smartpip2-2.1.9.3/airflow/contrib/dagsetup/dagfile_test.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17314 2022-09-27 06:26:39.000000 smartpip2-2.1.9.3/airflow/contrib/dagsetup/gen_airflow_dagfile.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/
--rw-r--r--   0 johnyan    (501) staff       (20)     1053 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_athena_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_datasync_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_dynamodb_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_firehose_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_glue_catalog_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1597 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_lambda_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_logs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1114 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_sns_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/aws_sqs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/azure_container_instance_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1220 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/azure_container_registry_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/azure_container_volume_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1162 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/azure_cosmos_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/azure_data_lake_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/azure_fileshare_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/bigquery_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/cassandra_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/cloudant_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1395 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/databricks_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/datadog_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/datastore_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/dingding_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/discord_webhook_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/emr_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/fs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1099 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/ftp_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1625 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_api_base_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_bigtable_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_cloud_build_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_compute_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_container_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_dataflow_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1593 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_dataproc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_dlp_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_function_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1543 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_kms_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_mlengine_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_natural_language_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_pubsub_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1424 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_spanner_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_speech_to_text_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_sql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_tasks_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_text_to_speech_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1804 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_transfer_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_translate_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_video_intelligence_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_vision_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gcs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1130 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/gdrive_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/grpc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/imap_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/jenkins_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/jira_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/mongo_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/openfaas_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/opsgenie_alert_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/pagerduty_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/pinot_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/qubole_check_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/qubole_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/redis_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/redshift_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/sagemaker_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/salesforce_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/segment_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/sftp_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/slack_webhook_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/snowflake_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1143 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/spark_jdbc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1139 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/spark_sql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1151 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/spark_submit_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/sqoop_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1089 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/ssh_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/vertica_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/wasb_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/hooks/winrm_hook.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/contrib/operators/
--rw-r--r--   0 johnyan    (501) staff       (20)      890 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/adls_list_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/adls_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/aws_athena_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/aws_sqs_publish_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2504 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/awsbatch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1239 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/azure_container_instances_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/azure_cosmos_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_get_data.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_table_delete_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_to_bigquery.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1701 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_to_mysql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/cassandra_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1202 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/databricks_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2883 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/dataflow_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8275 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/dataproc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1737 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/datastore_export_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1736 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/datastore_import_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/dingding_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/discord_webhook_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/docker_swarm_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/druid_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/dynamodb_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/ecs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/emr_add_steps_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/emr_create_job_flow_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/emr_terminate_job_flow_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1728 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/file_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/file_to_wasb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4792 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_bigtable_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_cloud_build_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4827 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_compute_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_container_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4405 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_dlp_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2348 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_function_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3958 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_natural_language_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3976 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_spanner_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1808 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_speech_to_text_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5195 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_sql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1566 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_tasks_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_text_to_speech_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_transfer_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_translate_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1757 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_translate_speech_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1337 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_video_intelligence_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7931 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcp_vision_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2296 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_acl_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_delete_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_download_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1645 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_list_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1657 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1695 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_bq.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1672 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_gdrive_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1636 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/grpc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/hive_to_dynamodb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/imap_attachment_to_s3_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/jenkins_job_trigger_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/jira_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/kubernetes_pod_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3494 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/mlengine_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/mongo_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/mssql_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/mysql_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1163 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/opsgenie_alert_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/oracle_to_oracle_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1707 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/postgres_to_gcs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3949 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/pubsub_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1188 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/qubole_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/qubole_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/redis_publish_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/s3_copy_object_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1182 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/s3_delete_objects_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/s3_list_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/s3_to_gcs_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1264 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/s3_to_gcs_transfer_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/s3_to_sftp_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_base_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_endpoint_config_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_endpoint_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_model_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1185 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_training_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1189 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_transform_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_tuning_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/segment_track_event_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sftp_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sftp_to_s3_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/slack_webhook_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/snowflake_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sns_publish_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/spark_jdbc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/spark_sql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/spark_submit_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sql_to_gcs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/sqoop_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/ssh_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/vertica_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1702 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/vertica_to_hive.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/vertica_to_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1193 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/wasb_delete_blob_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/operators/winrm_operator.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/contrib/secrets/
--rw-r--r--   0 johnyan    (501) staff       (20)      884 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/secrets/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/secrets/aws_secrets_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/secrets/aws_systems_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/secrets/azure_key_vault.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1699 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/secrets/gcp_secrets_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/secrets/hashicorp_vault.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/
--rw-r--r--   0 johnyan    (501) staff       (20)     1059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/aws_athena_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/aws_redshift_cluster_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/aws_sqs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/azure_cosmos_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/bash_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/bigquery_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1158 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/cassandra_record_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/cassandra_table_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/celery_queue_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/datadog_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/emr_base_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/emr_job_flow_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/emr_step_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1068 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/file_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1109 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/ftp_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/gcp_transfer_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/gcs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/hdfs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/imap_attachment_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1123 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/jira_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/mongo_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/pubsub_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/python_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/qubole_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/redis_key_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/redis_pub_sub_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_base_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_endpoint_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1205 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_training_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_transform_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_tuning_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/sftp_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/wasb_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/sensors/weekday_sensor.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/contrib/task_runner/
--rw-r--r--   0 johnyan    (501) staff       (20)      860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/task_runner/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/task_runner/cgroup_task_runner.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/contrib/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)      973 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1206 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/gcp_field_sanitizer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/gcp_field_validator.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/contrib/utils/log/
--rw-r--r--   0 johnyan    (501) staff       (20)      979 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/log/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/log/task_handler_with_custom_formatter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/mlengine_operator_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/mlengine_prediction_summary.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1369 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/sendgrid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/contrib/utils/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)      735 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/customized_form_field_behaviours.schema.json
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/decorators/
--rw-r--r--   0 johnyan    (501) staff       (20)     7051 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/decorators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8901 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/decorators/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3297 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/decorators/python.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3658 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/decorators/python_virtualenv.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/decorators/task_group.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/example_dags/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2357 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_bash_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2828 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_branch_datetime_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1767 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_branch_day_of_week_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_branch_labels.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2040 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_branch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2121 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_branch_python_dop_operator_3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7964 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_complex.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2336 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_dag_decorator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_external_task_marker_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3398 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_kubernetes_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6683 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_kubernetes_executor_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1313 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_latest_only.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1632 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_latest_only_with_trigger.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_nested_branch_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2943 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_passing_params_via_test_command.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3122 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_python_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1705 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_short_circuit_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2211 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_skip_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_subdag_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2329 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_task_group.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1988 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_task_group_decorator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1631 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_trigger_controller_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_trigger_target_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2662 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_xcom.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2118 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/example_dags/example_xcomargs.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/example_dags/libs/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/libs/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)      832 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/libs/helper.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/example_dags/subdags/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/subdags/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1733 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/subdags/subdag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/test_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/tutorial.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4311 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/tutorial_etl_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3302 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/tutorial_taskflow_api_etl.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3481 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6925 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/exceptions.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/executors/
--rw-r--r--   0 johnyan    (501) staff       (20)      802 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11695 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/base_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    25085 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/celery_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/celery_kubernetes_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4430 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/dask_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5674 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/debug_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/executor_constants.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4985 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/executor_loader.py
--rw-r--r--   0 johnyan    (501) staff       (20)    32831 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/kubernetes_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13912 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/local_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/executors/sequential_executor.py
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2022-10-24 03:38:18.000000 smartpip2-2.1.9.3/airflow/git_version
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/hooks/
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/S3_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)      800 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6597 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/base_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/dbapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/dbapi_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/docker_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/druid_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1527 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/filesystem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/hdfs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/hive_hooks.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/http_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1108 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/jdbc_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/mssql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/mysql_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/oracle_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/pig_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/postgres_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/presto_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/samba_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/slack_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/sqlite_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3589 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/subprocess.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/webhdfs_hook.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/hooks/zendesk_hook.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/jobs/
--rw-r--r--   0 johnyan    (501) staff       (20)      928 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/jobs/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    38099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/jobs/backfill_job.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9737 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/jobs/base_job.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/jobs/local_task_job.py
--rw-r--r--   0 johnyan    (501) staff       (20)    81963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/jobs/scheduler_job.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/kubernetes/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/k8s_model.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5528 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/kube_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/kube_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/kubernetes_helper_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1215 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/pod.py
--rw-r--r--   0 johnyan    (501) staff       (20)    20148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/pod_generator.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13034 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0 johnyan    (501) staff       (20)      996 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/pod_launcher.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/pod_launcher_deprecated.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/pod_runtime_info_env.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4555 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/refresh_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5242 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/secret.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/volume.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/kubernetes/volume_mount.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/lineage/
--rw-r--r--   0 johnyan    (501) staff       (20)     6456 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/lineage/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1730 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/lineage/backend.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2197 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/lineage/entities.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4442 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/logging_config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/macros/
--rw-r--r--   0 johnyan    (501) staff       (20)     2574 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/macros/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4884 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/macros/hive.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/migrations/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/env.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/migrations/versions/
--rw-r--r--   0 johnyan    (501) staff       (20)     1739 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/05f30312d566_merge_heads.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15150 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/13eb55f81627_for_compatibility.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1726 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/211e584da130_add_ti_state_index.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16341 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1475 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/2e541a1dcfed_task_duration.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2315 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1360 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3490 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/40e67319e3a9_dagrun_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1372 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/4446e08588_dagrun_start_end.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1689 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1230 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/502898887f84_adding_extra_to_log.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2605 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1257 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/52d714495f0_job_id_indices.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1952 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2512 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4511 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16875 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2634 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5447 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1323 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2958 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3222 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7211 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/92c57b58940d_add_fab_tables.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1920 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2874 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1301 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/9635ae0956e7_index_faskfail.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4170 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6567 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1278 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1600 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1839 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1204 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/b0125267960b_merge_heads.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1479 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1706 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1332 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1284 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1965 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3520 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1367 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5115 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1488 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3199 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1477 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1216 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1503 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1534 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3522 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11190 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/e3a246e0dc1_current_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1536 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/models/
--rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)    66313 2021-08-06 14:28:15.000000 smartpip2-2.1.9.3/airflow/models/baseoperator.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13786 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/connection.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2771 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/crypto.py
--rw-r--r--   0 johnyan    (501) staff       (20)    96020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)    27766 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/dagbag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/dagcode.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/dagparam.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1914 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/dagpickle.py
--rw-r--r--   0 johnyan    (501) staff       (20)    30854 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/dagrun.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/errors.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2239 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/log.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/pool.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/renderedtifields.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6417 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/sensorinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/serialized_dag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6652 2021-09-30 12:06:57.000000 smartpip2-2.1.9.3/airflow/models/skipmixin.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/slamiss.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/taskfail.py
--rw-r--r--   0 johnyan    (501) staff       (20)    82807 2022-08-01 13:38:00.000000 smartpip2-2.1.9.3/airflow/models/taskinstance.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/taskmixin.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/taskreschedule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7485 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/variable.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9883 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/xcom.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/models/xcom_arg.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/mypy/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/mypy/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/mypy/plugin/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/mypy/plugin/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2866 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/mypy/plugin/decorators.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/operators/
--rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6978 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/bash.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/bash_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2120 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/branch.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1070 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/branch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2897 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/dagrun_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/datetime.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/docker_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/druid_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/dummy.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/dummy_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/email.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/email_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/gcs_to_s3.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/generic_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/google_api_to_s3_transfer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/hive_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1166 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/hive_stats_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/hive_to_druid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1663 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/hive_to_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/hive_to_samba_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1118 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/http_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/jdbc_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2696 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/latest_only.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/latest_only_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/mssql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1668 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/mssql_to_hive.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/mysql_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/mysql_to_hive.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/oracle_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/papermill_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/pig_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/postgres_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/presto_check_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1658 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/presto_to_mysql.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18378 2021-08-07 01:46:07.000000 smartpip2-2.1.9.3/airflow/operators/python.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/python_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1680 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/redshift_to_s3_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/s3_file_transform_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1622 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/s3_to_hive_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/s3_to_redshift_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/slack_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)    20630 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/sql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1476 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/sql_branch_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/sqlite_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8631 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/subdag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1098 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/subdag_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6935 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/trigger_dagrun.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/operators/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)    14314 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/plugins_manager.py
--rw-r--r--   0 johnyan    (501) staff       (20)      882 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/provider_info.schema.json
--rw-r--r--   0 johnyan    (501) staff       (20)    17989 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/providers_manager.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/secrets/
--rw-r--r--   0 johnyan    (501) staff       (20)     1267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/secrets/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3321 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/secrets/base_secrets.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1601 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/secrets/environment_variables.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12137 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/secrets/local_filesystem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/secrets/metastore.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/security/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/security/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/security/kerberos.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2582 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/security/permissions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2880 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/security/utils.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/sensors/
--rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/base_sensor_operator.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3334 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/bash.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2851 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/date_time.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/date_time_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13029 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/external_task.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2380 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/filesystem.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/hdfs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/hive_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/http_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/metastore_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/named_hive_partition_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2864 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/python.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/s3_key_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/s3_prefix_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)    30370 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/smart_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4769 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/sql.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/sql_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/time_delta.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/time_delta_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1406 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/time_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/web_hdfs_sensor.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/sensors/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/sentry.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/serialization/
--rw-r--r--   0 johnyan    (501) staff       (20)      813 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/serialization/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/serialization/enums.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/serialization/helpers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2313 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/serialization/json_schema.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8061 2021-08-06 13:03:21.000000 smartpip2-2.1.9.3/airflow/serialization/schema.json
--rw-r--r--   0 johnyan    (501) staff       (20)    35709 2021-08-06 14:28:15.000000 smartpip2-2.1.9.3/airflow/serialization/serialized_objects.py
--rw-r--r--   0 johnyan    (501) staff       (20)    19657 2022-07-03 03:38:58.000000 smartpip2-2.1.9.3/airflow/settings.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/smart_sensor_dags/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/smart_sensor_dags/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2086 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/smart_sensor_dags/smart_sensor_group.py
--rw-r--r--   0 johnyan    (501) staff       (20)    13906 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/stats.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/task/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/task/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/task/task_runner/
--rw-r--r--   0 johnyan    (501) staff       (20)     2443 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/task/task_runner/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/task/task_runner/base_task_runner.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/task/task_runner/cgroup_task_runner.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4618 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/task/task_runner/standard_task_runner.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/templates.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/ti_deps/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4779 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/dep_context.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/dependencies_deps.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1504 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/dependencies_states.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/
--rw-r--r--   0 johnyan    (501) staff       (20)      844 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5905 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/base_ti_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1449 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/dag_ti_slots_available_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/dag_unpaused_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2245 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/dagrun_exists_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/dagrun_id_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/exec_date_after_start_date_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2132 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/not_in_retry_period_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3232 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/not_previously_skipped_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2871 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/pool_slots_available_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/prev_dagrun_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/ready_to_reschedule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2275 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/runnable_exec_date_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1639 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/task_concurrency_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/task_not_running_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/trigger_rule_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/ti_deps/deps/valid_state_dep.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:51.000000 smartpip2-2.1.9.3/airflow/typing_compat.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3672 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/callback_requests.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/cli.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3847 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/cli_action_loggers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/code_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1579 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/compression.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1409 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/configuration.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2413 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/dag_cycle_tester.py
--rw-r--r--   0 johnyan    (501) staff       (20)    49403 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/dag_processing.py
--rw-r--r--   0 johnyan    (501) staff       (20)    10420 2021-08-09 11:44:27.000000 smartpip2-2.1.9.3/airflow/utils/dates.py
--rw-r--r--   0 johnyan    (501) staff       (20)    21208 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/db.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1859 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/decorators.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1312 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/docs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6061 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/dot_renderer.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/edgemodifier.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12238 2022-07-03 05:03:18.000000 smartpip2-2.1.9.3/airflow/utils/email.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1521 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/entry_points.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1489 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/event_scheduler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8221 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/file.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7066 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/helpers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2457 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/json.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/utils/log/
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/cloudwatch_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/colored_log.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/es_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/file_processor_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11716 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/file_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/gcs_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/json_formatter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/log_reader.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/logging_mixin.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/s3_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8849 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/secrets_masker.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/stackdriver_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2178 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/task_handler_with_custom_formatter.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/log/wasb_task_handler.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/mixins.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1414 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/module_loading.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/net.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/operator_helpers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/operator_resources.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/orm_event_handlers.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2704 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/platform.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/process_utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/python_virtualenv.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1892 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/python_virtualenv_script.jinja2
--rw-r--r--   0 johnyan    (501) staff       (20)     3817 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/retries.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2975 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/serve_logs.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2420 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/session.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9571 2021-08-09 11:25:35.000000 smartpip2-2.1.9.3/airflow/utils/sqlalchemy.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/state.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/strings.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15018 2021-08-06 13:06:23.000000 smartpip2-2.1.9.3/airflow/utils/task_group.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/timeout.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5244 2021-08-09 11:25:54.000000 smartpip2-2.1.9.3/airflow/utils/timezone.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/trigger_rule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/types.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1640 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/weekday.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/weight_rule.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2412 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/utils/yaml.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1196 2022-10-13 03:18:37.000000 smartpip2-2.1.9.3/airflow/version.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/
--rw-r--r--   0 johnyan    (501) staff       (20)       87 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/.eslintignore
--rw-r--r--   0 johnyan    (501) staff       (20)       84 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/.eslintrc
--rw-r--r--   0 johnyan    (501) staff       (20)       26 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/.stylelintignore
--rw-r--r--   0 johnyan    (501) staff       (20)       45 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/.stylelintrc
--rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/api/
--rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/api/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/api/experimental/
--rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/api/experimental/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15690 2021-08-05 08:41:16.000000 smartpip2-2.1.9.3/airflow/www/api/experimental/endpoints.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5616 2021-08-09 08:25:04.000000 smartpip2-2.1.9.3/airflow/www/app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4186 2021-08-06 17:29:43.000000 smartpip2-2.1.9.3/airflow/www/auth.py
--rw-r--r--   0 johnyan    (501) staff       (20)      984 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/blueprints.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3152 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/decorators.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/extensions/
--rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_appbuilder.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-09-15 03:14:39.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_appbuilder_links.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_dagbag.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_jinja_globals.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2102 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_manifest_files.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2041 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_security.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1683 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_session.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8001 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_views.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/extensions/init_wsgi_middlewares.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8227 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/forms.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/gunicorn_config.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2755 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    30652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/security.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/static/
--rw-r--r--   0 johnyan    (501) staff       (20)   622963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/airflow.gif
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/static/css/
--rw-r--r--   0 johnyan    (501) staff       (20)   127184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/bootstrap-theme.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1209 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/calendar.css
--rw-r--r--   0 johnyan    (501) staff       (20)     3047 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/dags.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1392 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/flash.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1325 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/gantt.css
--rw-r--r--   0 johnyan    (501) staff       (20)     3240 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/graph.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1385 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/loading-dots.css
--rw-r--r--   0 johnyan    (501) staff       (20)     9964 2022-10-13 06:28:22.000000 smartpip2-2.1.9.3/airflow/www/static/css/main.css
--rw-r--r--   0 johnyan    (501) staff       (20)   112025 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/material-icons.css
--rw-r--r--   0 johnyan    (501) staff       (20)     2416 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/switch.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/css/tree.css
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/static/dist/
--rw-r--r--   0 johnyan    (501) staff       (20)   104074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js
--rw-r--r--   0 johnyan    (501) staff       (20)     7718 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/bootstrap-datetimepicker.min.css
--rw-r--r--   0 johnyan    (501) staff       (20)    37970 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/bootstrap-datetimepicker.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)    10289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/bootstrap3-typeahead.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1087 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css
--rw-r--r--   0 johnyan    (501) staff       (20)    15940 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js
--rw-r--r--   0 johnyan    (501) staff       (20)   346026 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/circles.995e0afd45c3641109e1.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5931 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/codemirror.css
--rw-r--r--   0 johnyan    (501) staff       (20)   398753 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/codemirror.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1466 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/coffeescript-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8981 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1310 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/css-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)    29780 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/d3-shape.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)     9207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/d3-tip.js
--rw-r--r--   0 johnyan    (501) staff       (20)   151725 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/d3.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)    14075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js
--rw-r--r--   0 johnyan    (501) staff       (20)     6495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js
--rw-r--r--   0 johnyan    (501) staff       (20)     9796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js
--rw-r--r--   0 johnyan    (501) staff       (20)    28194 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.core.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)    26948 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.core.min.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)   725181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)   668783 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.min.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)     2612 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css
--rw-r--r--   0 johnyan    (501) staff       (20)    16899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js
--rw-r--r--   0 johnyan    (501) staff       (20)     4226 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dataTables.bootstrap.min.css
--rw-r--r--   0 johnyan    (501) staff       (20)     1979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/dataTables.bootstrap.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5203 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/flash.d205b61edc54ed448412.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/flash.d205b61edc54ed448412.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css
--rw-r--r--   0 johnyan    (501) staff       (20)    40502 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css
--rw-r--r--   0 johnyan    (501) staff       (20)    53822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1989 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/html-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)    16827 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/ie.e458fc4544c628f16e02.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2159 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/javascript-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)    38837 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/javascript.js
--rw-r--r--   0 johnyan    (501) staff       (20)    83565 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/jquery.dataTables.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)  1283507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/jshint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1333 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/json-lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/lint.css
--rw-r--r--   0 johnyan    (501) staff       (20)     9125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/lint.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4229 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js
--rw-r--r--   0 johnyan    (501) staff       (20)     7313 2022-10-13 06:28:22.000000 smartpip2-2.1.9.3/airflow/www/static/dist/main.e52cf607b64cdcd15089.css
--rw-r--r--   0 johnyan    (501) staff       (20)    15979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/main.e52cf607b64cdcd15089.js
--rw-r--r--   0 johnyan    (501) staff       (20)     3327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/manifest.json
--rw-r--r--   0 johnyan    (501) staff       (20)   111620 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js
--rw-r--r--   0 johnyan    (501) staff       (20)   385945 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/moment.c1933ee062e9650051f7.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8329 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.css
--rw-r--r--   0 johnyan    (501) staff       (20)     3677 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.css.map
--rw-r--r--   0 johnyan    (501) staff       (20)   253352 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.js
--rw-r--r--   0 johnyan    (501) staff       (20)  1954533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)   993008 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/redoc.standalone.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2816 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0 johnyan    (501) staff       (20)  3389627 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/redoc.standalone.js.map
--rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/sum.md5
--rw-r--r--   0 johnyan    (501) staff       (20)     2091 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/switch.e97750fdb7423f33656a.css
--rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/switch.e97750fdb7423f33656a.js
--rw-r--r--   0 johnyan    (501) staff       (20)     9898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js
--rw-r--r--   0 johnyan    (501) staff       (20)    31314 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js
--rw-r--r--   0 johnyan    (501) staff       (20)    23111 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/tree.412f55814f4c1710d907.css
--rw-r--r--   0 johnyan    (501) staff       (20)    46722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/tree.412f55814f4c1710d907.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5116 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5055 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1255 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/dist/yaml-lint.js
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/static/js/
--rw-r--r--   0 johnyan    (501) staff       (20)    11183 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/calendar.js
--rw-r--r--   0 johnyan    (501) staff       (20)     3436 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/circles.js
--rw-r--r--   0 johnyan    (501) staff       (20)     4994 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/connection_form.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8057 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/dag.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1010 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/dag_code.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5997 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/dag_dependencies.js
--rw-r--r--   0 johnyan    (501) staff       (20)    11004 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/dags.js
--rw-r--r--   0 johnyan    (501) staff       (20)     3593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/datetime_utils.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/duration_chart.js
--rw-r--r--   0 johnyan    (501) staff       (20)     8882 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/gantt.js
--rw-r--r--   0 johnyan    (501) staff       (20)    21515 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/graph.js
--rw-r--r--   0 johnyan    (501) staff       (20)      887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/ie.js
--rw-r--r--   0 johnyan    (501) staff       (20)     6355 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/main.js
--rw-r--r--   0 johnyan    (501) staff       (20)      995 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/meta_value.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1107 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/task_instance.js
--rw-r--r--   0 johnyan    (501) staff       (20)     4274 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/task_instances.js
--rw-r--r--   0 johnyan    (501) staff       (20)     5599 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/ti_log.js
--rw-r--r--   0 johnyan    (501) staff       (20)    15167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/tree.js
--rw-r--r--   0 johnyan    (501) staff       (20)     1020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/trigger.js
--rw-r--r--   0 johnyan    (501) staff       (20)      957 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/js/variable_edit.js
--rw-r--r--   0 johnyan    (501) staff       (20)    16671 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/loading.gif
--rw-r--r--   0 johnyan    (501) staff       (20)     3184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/pin.svg
--rw-r--r--   0 johnyan    (501) staff       (20)     7501 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/pin_100.png
--rw-r--r--   0 johnyan    (501) staff       (20)     1547 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/pin_25.png
--rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/pin_32.png
--rw-r--r--   0 johnyan    (501) staff       (20)     2306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/pin_35.png
--rw-r--r--   0 johnyan    (501) staff       (20)     2685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/pin_40.png
--rw-r--r--   0 johnyan    (501) staff       (20)    24922 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/pin_large.png
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/static/screenshots/
--rw-r--r--   0 johnyan    (501) staff       (20)    31140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/screenshots/gantt.png
--rw-r--r--   0 johnyan    (501) staff       (20)    38282 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/screenshots/graph.png
--rw-r--r--   0 johnyan    (501) staff       (20)    35259 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/screenshots/tree.png
--rw-r--r--   0 johnyan    (501) staff       (20)      160 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/sort_asc.png
--rw-r--r--   0 johnyan    (501) staff       (20)      201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/sort_both.png
--rw-r--r--   0 johnyan    (501) staff       (20)      158 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/static/sort_desc.png
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/airflow/www/templates/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/
--rw-r--r--   0 johnyan    (501) staff       (20)     1877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/calendar.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2581 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/chart.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1345 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/circles.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/code.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1894 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/config.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/confirm.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1038 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/conn_create.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1049 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/conn_edit.html
--rw-r--r--   0 johnyan    (501) staff       (20)    21916 2021-09-21 03:40:31.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/dag.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/dag_code.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/dag_dependencies.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3424 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/dag_details.html
--rw-r--r--   0 johnyan    (501) staff       (20)    16490 2021-09-21 04:00:33.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/dags.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2900 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/duration_chart.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/gantt.html
--rw-r--r--   0 johnyan    (501) staff       (20)     5609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/graph.html
--rw-r--r--   0 johnyan    (501) staff       (20)     4035 2021-08-09 08:31:54.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/main.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3173 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/model_list.html
--rw-r--r--   0 johnyan    (501) staff       (20)      950 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/noaccess.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/plugin.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/redoc.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2213 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/task.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/task_instance.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1044 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/ti_code.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2929 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/ti_log.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1431 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/traceback.html
--rw-r--r--   0 johnyan    (501) staff       (20)     4480 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/tree.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/trigger.html
--rw-r--r--   0 johnyan    (501) staff       (20)      999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/variable_edit.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/variable_list.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1231 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/airflow/xcom.html
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/templates/analytics/
--rw-r--r--   0 johnyan    (501) staff       (20)     1195 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/analytics/google_analytics.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1807 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/analytics/metarouter.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1810 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/analytics/segment.html
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/
--rw-r--r--   0 johnyan    (501) staff       (20)     4446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/custom_icons.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/dag_docs.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3000 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/flash.html
--rw-r--r--   0 johnyan    (501) staff       (20)      809 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/index.html
--rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/loading_dots.html
--rw-r--r--   0 johnyan    (501) staff       (20)     4388 2022-10-13 06:34:20.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/navbar.html
--rw-r--r--   0 johnyan    (501) staff       (20)     2001 2022-10-13 08:38:39.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/navbar_menu.html
--rw-r--r--   0 johnyan    (501) staff       (20)     3486 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/templates/appbuilder/navbar_right.html
--rw-r--r--   0 johnyan    (501) staff       (20)    16328 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/utils.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2615 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/validators.py
--rw-r--r--   0 johnyan    (501) staff       (20)   149695 2021-11-22 06:20:23.000000 smartpip2-2.1.9.3/airflow/www/views.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6792 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/webpack.config.js
--rw-r--r--   0 johnyan    (501) staff       (20)     2549 2021-08-04 09:43:52.000000 smartpip2-2.1.9.3/airflow/www/widgets.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/licenses/
--rw-rw-r--   0 johnyan    (501) staff       (20)     1131 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-bootstrap.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)      984 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-bootstrap3-typeahead.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)      556 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-connexion.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-d3-shape.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1079 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-d3-tip.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-d3js.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1062 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-dagre-d3.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1076 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-datatables.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1081 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-elasticmock.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1301 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-flask-kerberos.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)    11349 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-hue.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)    11357 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-jqclock.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1605 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-jquery.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1077 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-moment-strftime.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1075 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-moment.txt
--rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/licenses/LICENSE-normalize.txt
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/scripts/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/scripts/systemd/
--rw-rw-r--   0 johnyan    (501) staff       (20)      678 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/README
--rw-rw-r--   0 johnyan    (501) staff       (20)      968 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/airflow
--rw-rw-r--   0 johnyan    (501) staff       (20)     1195 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/airflow-flower.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1200 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/airflow-kerberos.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1190 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/airflow-scheduler.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1243 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/airflow-webserver.service
--rw-rw-r--   0 johnyan    (501) staff       (20)     1203 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/airflow-worker.service
--rw-rw-r--   0 johnyan    (501) staff       (20)      824 2021-08-03 16:23:18.000000 smartpip2-2.1.9.3/scripts/systemd/airflow.conf
--rw-rw-r--   0 johnyan    (501) staff       (20)     4042 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/setup.cfg
--rw-rw-r--   0 johnyan    (501) staff       (20)    33517 2022-10-24 09:43:56.000000 smartpip2-2.1.9.3/setup.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2022-10-24 09:44:10.000000 smartpip2-2.1.9.3/smartpip2.egg-info/
--rw-r--r--   0 johnyan    (501) staff       (20)    26641 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/smartpip2.egg-info/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)    44222 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/smartpip2.egg-info/SOURCES.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/smartpip2.egg-info/dependency_links.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/smartpip2.egg-info/entry_points.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2021-08-07 01:38:26.000000 smartpip2-2.1.9.3/smartpip2.egg-info/not-zip-safe
--rw-r--r--   0 johnyan    (501) staff       (20)    29803 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/smartpip2.egg-info/requires.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        8 2022-10-24 09:44:09.000000 smartpip2-2.1.9.3/smartpip2.egg-info/top_level.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/
+-rw-rw-r--   0 johnyan    (501) staff       (20)   274732 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/CHANGELOG.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)    13444 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/LICENSE
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1433 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/MANIFEST.in
+-rw-rw-r--   0 johnyan    (501) staff       (20)      404 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/NOTICE
+-rw-r--r--   0 johnyan    (501) staff       (20)    26641 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/PKG-INFO
+-rw-rw-r--   0 johnyan    (501) staff       (20)    20139 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/README.md
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2751 2022-07-19 14:54:13.000000 smartpip2-2.1.9.4/airflow/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1368 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/__main__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1430 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)       95 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/__main__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/
+-rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18192 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/abstract.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14270 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/aiohttp_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12812 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2222 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_utils.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/
+-rw-r--r--   0 johnyan    (501) staff       (20)       42 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10764 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/abstract.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/aiohttp_app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5023 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/flask_app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/cli.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1842 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/coroutine_wrappers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1441 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/decorator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1752 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/metrics.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/parameter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/produces.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/response.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9853 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/security.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11690 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/uri_parsing.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15533 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/validation.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/exceptions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2692 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/handlers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/http_facts.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4050 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/json_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/jsonifier.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/lifecycle.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/mock.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/
+-rw-r--r--   0 johnyan    (501) staff       (20)      294 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15461 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/abstract.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      127 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/compat.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14505 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/openapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6782 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/secure.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/swagger2.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4444 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/options.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1926 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/problem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6810 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/resolver.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3408 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/setup.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/spec.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6515 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/_vendor/connexion/utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2320 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/alembic.ini
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1550 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/auth/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2258 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/basic_auth.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1342 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/default.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/deny_all.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5563 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/kerberos_auth.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1500 2022-07-04 11:00:25.000000 smartpip2-2.1.9.4/airflow/api/auth/backend/smart_auth.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/client/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2465 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/api_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/json_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2223 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/client/local_client.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/common/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2045 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/delete_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      329 2020-10-10 01:23:08.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/gen_dag_file.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1426 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_code.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1381 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_run_state.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1982 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_runs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1886 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_lineage.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_task.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1628 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/get_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14243 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/mark_tasks.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2833 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/pool.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4413 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api/common/experimental/trigger_dag.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3303 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/config_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5383 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/connection_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8558 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_run_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2044 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_source_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5487 2022-07-05 00:33:48.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dagsetup_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2517 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/event_log_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2449 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/extra_link_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1732 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/health_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2618 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/import_error_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3649 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/log_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1560 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/plugin_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5506 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/pool_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/provider_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6330 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/role_and_permission_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2401 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11479 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_instance_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2509 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/user_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4008 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/variable_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1363 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/version_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3848 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/endpoints/xcom_endpoint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5017 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/exceptions.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/openapi/
+-rw-r--r--   0 johnyan    (501) staff       (20)   107667 2022-07-05 06:13:09.000000 smartpip2-2.1.9.4/airflow/api_connexion/openapi/v1.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     3655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/parameters.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/common_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/config_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1995 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/connection_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4184 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_run_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      971 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_source_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1349 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/enum_schemas.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1738 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/error_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/event_log_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/health_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/log_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1754 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/plugin_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2370 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/pool_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1452 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/provider_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2531 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/role_and_permission_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1327 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/sla_miss_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6966 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_instance_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2992 2021-08-06 13:05:03.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2331 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/user_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/variable_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/version_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1769 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/schemas/xcom_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/api_connexion/security.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/cli/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    59796 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/cli_parser.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/cli/commands/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6551 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/celery_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2366 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/cheat_sheet_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/config_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/connection_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13203 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/dag_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3345 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/db_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13283 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/info_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2070 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/jobs_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1740 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/kerberos_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/kubernetes_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1999 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/legacy_commands.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/plugins_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/pool_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3862 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/provider_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1582 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/role_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1379 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/rotate_fernet_key_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/scheduler_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1416 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/sync_perm_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/task_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8359 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/user_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3968 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/variable_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      929 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/version_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    20747 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/commands/webserver_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5290 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/cli/simple_table.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/common/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2022-07-03 02:40:42.000000 smartpip2-2.1.9.4/airflow/common/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9162 2022-07-03 03:12:30.000000 smartpip2-2.1.9.4/airflow/common/datax.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    58815 2023-04-26 09:55:02.000000 smartpip2-2.1.9.4/airflow/common/smartpip.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/compat/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/compat/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/compat/functools.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/config_templates/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11726 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/airflow_local_settings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    75766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/config.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1629 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/config.yml.schema.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    44296 2022-08-26 06:07:49.000000 smartpip2-2.1.9.4/airflow/config_templates/default_airflow.cfg
+-rw-r--r--   0 johnyan    (501) staff       (20)     4094 2022-08-01 06:06:39.000000 smartpip2-2.1.9.4/airflow/config_templates/default_celery.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2028 2022-07-03 06:20:29.000000 smartpip2-2.1.9.4/airflow/config_templates/default_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3770 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/default_test.cfg
+-rw-r--r--   0 johnyan    (501) staff       (20)     4700 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/config_templates/default_webserver_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    44793 2022-07-22 10:03:34.000000 smartpip2-2.1.9.4/airflow/configuration.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/
+-rw-r--r--   0 johnyan    (501) staff       (20)      821 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/
+-rw-r--r--   0 johnyan    (501) staff       (20)       86 2020-10-10 01:23:08.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7650 2023-04-26 08:41:20.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/config_dagfile.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2586 2021-11-22 09:21:52.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/dagfile_test.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17582 2023-04-26 07:37:37.000000 smartpip2-2.1.9.4/airflow/contrib/dagsetup/gen_airflow_dagfile.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1053 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_athena_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_datasync_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_dynamodb_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_firehose_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_glue_catalog_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1597 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_lambda_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_logs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1114 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sns_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sqs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_instance_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1220 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_registry_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_volume_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1162 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_cosmos_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_data_lake_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/azure_fileshare_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/bigquery_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/cassandra_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/cloudant_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1395 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/databricks_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/datadog_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/datastore_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/dingding_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/discord_webhook_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/emr_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/fs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1099 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/ftp_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1625 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_api_base_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_bigtable_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_cloud_build_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_compute_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1574 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_container_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1598 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataflow_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1593 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataproc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dlp_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_function_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1543 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_kms_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_mlengine_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_natural_language_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_pubsub_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1424 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_spanner_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_speech_to_text_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_sql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_tasks_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1664 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_text_to_speech_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1804 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_transfer_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_translate_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_video_intelligence_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_vision_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gcs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1130 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/gdrive_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/grpc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/imap_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/jenkins_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/jira_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/mongo_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/openfaas_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/opsgenie_alert_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/pagerduty_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/pinot_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_check_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/redis_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/redshift_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1261 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/sagemaker_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/salesforce_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/segment_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/sftp_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/slack_webhook_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/snowflake_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1143 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/spark_jdbc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1139 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/spark_sql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1151 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/spark_submit_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/sqoop_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1089 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/ssh_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1117 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/vertica_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/wasb_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/hooks/winrm_hook.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/operators/
+-rw-r--r--   0 johnyan    (501) staff       (20)      890 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/adls_list_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1667 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/adls_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1142 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/aws_athena_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1132 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/aws_sqs_publish_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2504 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/awsbatch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1239 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/azure_container_instances_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/azure_cosmos_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_get_data.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_table_delete_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_bigquery.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1701 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_mysql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/cassandra_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1202 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/databricks_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2883 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dataflow_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8275 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dataproc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1737 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/datastore_export_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1736 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/datastore_import_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dingding_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/discord_webhook_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/docker_swarm_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/druid_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/dynamodb_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/ecs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/emr_add_steps_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/emr_create_job_flow_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/emr_terminate_job_flow_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1728 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/file_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/file_to_wasb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4792 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_bigtable_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_cloud_build_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4827 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_compute_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2785 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_container_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4405 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_dlp_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2348 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_function_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3958 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_natural_language_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3976 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_spanner_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1808 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_speech_to_text_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5195 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_sql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1566 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_tasks_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1766 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_text_to_speech_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7980 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_transfer_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1757 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_speech_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1337 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_video_intelligence_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7931 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcp_vision_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2296 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_acl_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1655 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_delete_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_download_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1645 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_list_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1657 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1695 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_bq.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1672 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gdrive_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1636 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/grpc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/hive_to_dynamodb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/imap_attachment_to_s3_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/jenkins_job_trigger_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/jira_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/kubernetes_pod_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3494 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mlengine_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mongo_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mssql_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/mysql_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1163 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/opsgenie_alert_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1687 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_oracle_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1707 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/postgres_to_gcs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3949 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/pubsub_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1188 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/qubole_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/qubole_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/redis_publish_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_copy_object_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1182 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_delete_objects_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_list_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1264 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_transfer_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_sftp_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_base_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1225 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_config_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_model_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1185 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_training_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1189 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_transform_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_tuning_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1179 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/segment_track_event_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sftp_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sftp_to_s3_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1150 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/slack_webhook_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/snowflake_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sns_publish_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/spark_jdbc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/spark_sql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/spark_submit_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1677 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sql_to_gcs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/sqoop_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1105 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/ssh_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/vertica_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1702 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_hive.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1682 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1193 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/wasb_delete_blob_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/operators/winrm_operator.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/
+-rw-r--r--   0 johnyan    (501) staff       (20)      884 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/aws_secrets_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/aws_systems_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/azure_key_vault.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1699 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/gcp_secrets_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/secrets/hashicorp_vault.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1059 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1131 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_athena_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1197 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_redshift_cluster_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/aws_sqs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/azure_cosmos_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1097 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/bash_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/bigquery_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1158 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_record_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1154 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_table_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/celery_queue_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/datadog_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/emr_base_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1152 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/emr_job_flow_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1137 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/emr_step_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1068 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/file_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1109 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/ftp_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1830 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/gcp_transfer_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3356 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/gcs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/hdfs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/imap_attachment_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1123 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/jira_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1111 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/mongo_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/pubsub_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/python_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1176 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/qubole_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/redis_key_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/redis_pub_sub_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1161 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_base_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_endpoint_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1205 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_training_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_transform_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1169 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_tuning_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/sftp_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1159 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/wasb_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/sensors/weekday_sensor.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/task_runner/
+-rw-r--r--   0 johnyan    (501) staff       (20)      860 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/task_runner/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1134 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/task_runner/cgroup_task_runner.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)      973 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1206 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_sanitizer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_validator.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/contrib/utils/log/
+-rw-r--r--   0 johnyan    (501) staff       (20)      979 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/log/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1173 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/log/task_handler_with_custom_formatter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1190 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_operator_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1212 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_prediction_summary.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1369 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/sendgrid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1047 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/contrib/utils/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      735 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/customized_form_field_behaviours.schema.json
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/decorators/
+-rw-r--r--   0 johnyan    (501) staff       (20)     7051 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8901 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3297 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/python.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3658 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/python_virtualenv.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2784 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/decorators/task_group.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/example_dags/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2357 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_bash_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2828 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_datetime_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1767 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_day_of_week_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1611 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_labels.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2040 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2121 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_branch_python_dop_operator_3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7964 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_complex.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2336 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_dag_decorator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3112 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_external_task_marker_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3398 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6683 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1313 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_latest_only.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1632 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_latest_only_with_trigger.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2034 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_nested_branch_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2943 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_passing_params_via_test_command.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3122 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_python_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1705 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_short_circuit_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2211 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_skip_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_subdag_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2329 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_task_group.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1988 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_task_group_decorator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1631 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_trigger_controller_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_trigger_target_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2662 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_xcom.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2118 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/example_dags/example_xcomargs.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/example_dags/libs/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/libs/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      832 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/libs/helper.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/example_dags/subdags/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/subdags/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1733 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/subdags/subdag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1172 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/test_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4311 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial_etl_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3302 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3481 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6925 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/exceptions.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/executors/
+-rw-r--r--   0 johnyan    (501) staff       (20)      802 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11695 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/base_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    25085 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/celery_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/celery_kubernetes_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4430 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/dask_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5674 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/debug_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/executor_constants.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4985 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/executor_loader.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    32831 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/kubernetes_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13912 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/local_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/executors/sequential_executor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2022-10-24 03:38:18.000000 smartpip2-2.1.9.4/airflow/git_version
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/hooks/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/S3_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      800 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6597 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/base_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/dbapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/dbapi_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/docker_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/druid_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1527 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/filesystem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/hdfs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1200 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/hive_hooks.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1096 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/http_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1108 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/jdbc_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/mssql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/mysql_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/oracle_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/pig_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1124 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/postgres_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/presto_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/samba_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/slack_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/sqlite_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3589 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/subprocess.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/webhdfs_hook.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/hooks/zendesk_hook.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/jobs/
+-rw-r--r--   0 johnyan    (501) staff       (20)      928 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    38099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/backfill_job.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9737 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/base_job.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/local_task_job.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    81963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/jobs/scheduler_job.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/kubernetes/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2113 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/k8s_model.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5528 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/kube_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/kube_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/kubernetes_helper_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1215 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    20148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_generator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13034 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      996 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher_deprecated.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/pod_runtime_info_env.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4555 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/refresh_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5242 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/secret.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1156 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/volume.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/kubernetes/volume_mount.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/lineage/
+-rw-r--r--   0 johnyan    (501) staff       (20)     6456 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/lineage/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1730 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/lineage/backend.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2197 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/lineage/entities.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4442 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/logging_config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/macros/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2574 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/macros/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4884 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/macros/hive.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/migrations/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/env.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/migrations/versions/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1739 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/05f30312d566_merge_heads.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3109 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15150 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/13eb55f81627_for_compatibility.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1726 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/211e584da130_add_ti_state_index.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16341 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1475 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2e541a1dcfed_task_duration.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1174 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2315 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1360 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3490 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/40e67319e3a9_dagrun_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1246 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1372 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/4446e08588_dagrun_start_end.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1689 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6279 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1230 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/502898887f84_adding_extra_to_log.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2605 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1257 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/52d714495f0_job_id_indices.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1952 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2512 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4511 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16875 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2634 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5447 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1323 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2958 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3222 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1927 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7211 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/92c57b58940d_add_fab_tables.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1920 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2874 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1301 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/9635ae0956e7_index_faskfail.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4170 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6567 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1278 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1600 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1839 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1204 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b0125267960b_merge_heads.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1479 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1706 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1332 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1284 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1965 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3520 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1367 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5115 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1488 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3199 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1477 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1216 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1503 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1534 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3522 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11190 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e3a246e0dc1_current_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1536 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1991 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/models/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1781 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    66313 2021-08-06 14:28:15.000000 smartpip2-2.1.9.4/airflow/models/baseoperator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13786 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/connection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2771 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/crypto.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    96020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    27766 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagbag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagcode.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagparam.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1914 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagpickle.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    30854 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/dagrun.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/errors.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2239 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/log.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/pool.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7099 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/renderedtifields.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6417 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/sensorinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/serialized_dag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6652 2021-09-30 12:06:57.000000 smartpip2-2.1.9.4/airflow/models/skipmixin.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/slamiss.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2036 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/taskfail.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    82807 2022-08-01 13:38:00.000000 smartpip2-2.1.9.4/airflow/models/taskinstance.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/taskmixin.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4110 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/taskreschedule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7485 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/variable.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9883 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/xcom.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5237 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/models/xcom_arg.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/mypy/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/mypy/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/mypy/plugin/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/mypy/plugin/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2866 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/mypy/plugin/decorators.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/operators/
+-rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6978 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/bash.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/bash_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2120 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/branch.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1070 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/branch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2897 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/dagrun_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/datetime.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/docker_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/druid_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1238 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/dummy.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/dummy_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/email.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1062 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/email_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1148 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/gcs_to_s3.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/generic_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/google_api_to_s3_transfer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1133 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1166 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_stats_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_to_druid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1663 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_to_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/hive_to_samba_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1118 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/http_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1112 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/jdbc_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2696 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/latest_only.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1083 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/latest_only_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mssql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1668 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mssql_to_hive.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1119 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mysql_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/mysql_to_hive.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/oracle_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1147 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/papermill_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/pig_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1149 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/postgres_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2469 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/presto_check_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1658 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/presto_to_mysql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18378 2021-08-07 01:46:07.000000 smartpip2-2.1.9.4/airflow/operators/python.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1157 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/python_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1680 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/redshift_to_s3_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/s3_file_transform_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1622 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/s3_to_hive_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1673 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/s3_to_redshift_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1144 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/slack_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    20630 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/sql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1476 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/sql_branch_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/sqlite_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8631 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/subdag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1098 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/subdag_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6935 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/trigger_dagrun.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/operators/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    14314 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/plugins_manager.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      882 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/provider_info.schema.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    17989 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/providers_manager.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/secrets/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1267 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3321 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/base_secrets.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1601 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/environment_variables.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12137 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/local_filesystem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/secrets/metastore.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/security/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/kerberos.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2582 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/permissions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2880 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/security/utils.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/sensors/
+-rw-r--r--   0 johnyan    (501) staff       (20)      804 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1058 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/base_sensor_operator.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3334 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/bash.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2851 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/date_time.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/date_time_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13029 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/external_task.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2380 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/filesystem.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1126 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/hdfs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1164 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/hive_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1104 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/http_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1186 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/metastore_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/named_hive_partition_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2864 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/python.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1129 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/s3_key_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1141 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/s3_prefix_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    30370 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/smart_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4769 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/sql.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1046 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/sql_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1719 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/time_delta.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1073 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/time_delta_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1406 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/time_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/web_hdfs_sensor.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/sensors/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6613 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/sentry.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/serialization/
+-rw-r--r--   0 johnyan    (501) staff       (20)      813 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/enums.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/helpers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2313 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/serialization/json_schema.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8061 2021-08-06 13:03:21.000000 smartpip2-2.1.9.4/airflow/serialization/schema.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    35709 2021-08-06 14:28:15.000000 smartpip2-2.1.9.4/airflow/serialization/serialized_objects.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    19657 2022-07-03 03:38:58.000000 smartpip2-2.1.9.4/airflow/settings.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/smart_sensor_dags/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/smart_sensor_dags/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2086 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/smart_sensor_dags/smart_sensor_group.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    13906 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/stats.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/task/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/task/task_runner/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2443 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6791 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/base_task_runner.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/cgroup_task_runner.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4618 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/task/task_runner/standard_task_runner.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1346 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/templates.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/ti_deps/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4779 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/dep_context.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3709 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/dependencies_deps.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1504 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/dependencies_states.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/
+-rw-r--r--   0 johnyan    (501) staff       (20)      844 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5905 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/base_ti_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1449 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_ti_slots_available_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1249 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_unpaused_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2245 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_exists_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2260 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_id_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1841 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/exec_date_after_start_date_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2132 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/not_in_retry_period_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3232 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/not_previously_skipped_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2871 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/pool_slots_available_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/prev_dagrun_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/ready_to_reschedule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2275 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/runnable_exec_date_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1639 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/task_concurrency_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1559 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/task_not_running_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/trigger_rule_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2365 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/ti_deps/deps/valid_state_dep.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:51.000000 smartpip2-2.1.9.4/airflow/typing_compat.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3672 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/callback_requests.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/cli.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3847 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/cli_action_loggers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/code_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1579 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/compression.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1409 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/configuration.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2413 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/dag_cycle_tester.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    49403 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/dag_processing.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    10420 2021-08-09 11:44:27.000000 smartpip2-2.1.9.4/airflow/utils/dates.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    21208 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/db.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1859 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/decorators.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1312 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/docs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6061 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/dot_renderer.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5069 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/edgemodifier.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12238 2022-07-03 05:03:18.000000 smartpip2-2.1.9.4/airflow/utils/email.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1521 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/entry_points.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1489 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/event_scheduler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8221 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/file.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7066 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/helpers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2457 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/json.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/utils/log/
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1177 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/cloudwatch_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/colored_log.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/es_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/file_processor_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11716 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/file_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1155 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/gcs_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2165 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/json_formatter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4890 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/log_reader.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5425 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/logging_mixin.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1145 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/s3_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8849 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/secrets_masker.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/stackdriver_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2178 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/task_handler_with_custom_formatter.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/log/wasb_task_handler.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1472 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/mixins.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1414 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/module_loading.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1180 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/net.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/operator_helpers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4161 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/operator_resources.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3532 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/orm_event_handlers.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2704 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/platform.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9500 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/process_utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/python_virtualenv.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1892 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/python_virtualenv_script.jinja2
+-rw-r--r--   0 johnyan    (501) staff       (20)     3817 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/retries.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2975 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/serve_logs.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2420 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/session.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9571 2021-08-09 11:25:35.000000 smartpip2-2.1.9.4/airflow/utils/sqlalchemy.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4006 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/state.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1171 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/strings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15018 2021-08-06 13:06:23.000000 smartpip2-2.1.9.4/airflow/utils/task_group.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1960 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/timeout.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5244 2021-08-09 11:25:54.000000 smartpip2-2.1.9.4/airflow/utils/timezone.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/trigger_rule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1551 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/types.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1640 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/weekday.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/weight_rule.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2412 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/utils/yaml.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1196 2022-10-13 03:18:37.000000 smartpip2-2.1.9.4/airflow/version.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/
+-rw-r--r--   0 johnyan    (501) staff       (20)       87 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.eslintignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       84 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.eslintrc
+-rw-r--r--   0 johnyan    (501) staff       (20)       26 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.stylelintignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       45 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/.stylelintrc
+-rw-r--r--   0 johnyan    (501) staff       (20)      787 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/api/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/api/experimental/
+-rw-r--r--   0 johnyan    (501) staff       (20)      789 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/api/experimental/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15690 2021-08-05 08:41:16.000000 smartpip2-2.1.9.4/airflow/www/api/experimental/endpoints.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5616 2021-08-09 08:25:04.000000 smartpip2-2.1.9.4/airflow/www/app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4186 2021-08-06 17:29:43.000000 smartpip2-2.1.9.4/airflow/www/auth.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      984 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/blueprints.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3152 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/decorators.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/extensions/
+-rw-r--r--   0 johnyan    (501) staff       (20)      785 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2123 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2021-09-15 03:14:39.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder_links.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_dagbag.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_jinja_globals.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2102 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_manifest_files.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2041 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_security.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1683 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_session.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8001 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_views.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2136 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/extensions/init_wsgi_middlewares.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8227 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/forms.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1146 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/gunicorn_config.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2755 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    30652 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/security.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/static/
+-rw-r--r--   0 johnyan    (501) staff       (20)   622963 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/airflow.gif
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/static/css/
+-rw-r--r--   0 johnyan    (501) staff       (20)   127184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/bootstrap-theme.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1209 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/calendar.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     3047 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/dags.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1392 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/flash.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1325 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/gantt.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     3240 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/graph.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1385 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/loading-dots.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     9964 2022-10-13 06:28:22.000000 smartpip2-2.1.9.4/airflow/www/static/css/main.css
+-rw-r--r--   0 johnyan    (501) staff       (20)   112025 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/material-icons.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     2416 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/switch.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/css/tree.css
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/static/dist/
+-rw-r--r--   0 johnyan    (501) staff       (20)   104074 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4243 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     7718 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    37970 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    10289 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap3-typeahead.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1087 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    15940 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   346026 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/circles.995e0afd45c3641109e1.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5931 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.css
+-rw-r--r--   0 johnyan    (501) staff       (20)   398753 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1466 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/coffeescript-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8981 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1310 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/css-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    29780 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/d3-shape.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     9207 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/d3-tip.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   151725 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/d3.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    14075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     6495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     9796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    28194 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    26948 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)   725181 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   668783 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)     2612 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    16899 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     4226 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     1979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5203 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1075 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1128 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    40502 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2744 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    53822 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1989 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/html-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    16827 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/ie.e458fc4544c628f16e02.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2159 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/javascript-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    38837 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/javascript.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    83565 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/jquery.dataTables.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)  1283507 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/jshint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1333 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/json-lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2607 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/lint.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     9125 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/lint.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1244 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4229 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     7313 2022-10-13 06:28:22.000000 smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    15979 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     3327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/manifest.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   111620 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4233 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js
+-rw-r--r--   0 johnyan    (501) staff       (20)   385945 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/moment.c1933ee062e9650051f7.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8329 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     3677 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css.map
+-rw-r--r--   0 johnyan    (501) staff       (20)   253352 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js
+-rw-r--r--   0 johnyan    (501) staff       (20)  1954533 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)   993008 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2816 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)  3389627 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.map
+-rw-r--r--   0 johnyan    (501) staff       (20)     1855 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/sum.md5
+-rw-r--r--   0 johnyan    (501) staff       (20)     2091 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.css
+-rw-r--r--   0 johnyan    (501) staff       (20)     4219 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     9898 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    31314 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    23111 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1616 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.css
+-rw-r--r--   0 johnyan    (501) staff       (20)    46722 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5116 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5055 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1255 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/dist/yaml-lint.js
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/static/js/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11183 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/calendar.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     3436 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/circles.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     4994 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/connection_form.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8057 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dag.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1010 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dag_code.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5997 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dag_dependencies.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    11004 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/dags.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     3593 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/datetime_utils.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1103 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/duration_chart.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     8882 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/gantt.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    21515 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/graph.js
+-rw-r--r--   0 johnyan    (501) staff       (20)      887 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/ie.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     6355 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/main.js
+-rw-r--r--   0 johnyan    (501) staff       (20)      995 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/meta_value.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1107 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/task_instance.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     4274 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/task_instances.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     5599 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/ti_log.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    15167 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/tree.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     1020 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/trigger.js
+-rw-r--r--   0 johnyan    (501) staff       (20)      957 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/js/variable_edit.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    16671 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/loading.gif
+-rw-r--r--   0 johnyan    (501) staff       (20)     3184 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin.svg
+-rw-r--r--   0 johnyan    (501) staff       (20)     7501 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_100.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     1547 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_25.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     1201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_32.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     2306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_35.png
+-rw-r--r--   0 johnyan    (501) staff       (20)     2685 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_40.png
+-rw-r--r--   0 johnyan    (501) staff       (20)    24922 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/pin_large.png
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/
+-rw-r--r--   0 johnyan    (501) staff       (20)    31140 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/gantt.png
+-rw-r--r--   0 johnyan    (501) staff       (20)    38282 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/graph.png
+-rw-r--r--   0 johnyan    (501) staff       (20)    35259 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/screenshots/tree.png
+-rw-r--r--   0 johnyan    (501) staff       (20)      160 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/sort_asc.png
+-rw-r--r--   0 johnyan    (501) staff       (20)      201 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/sort_both.png
+-rw-r--r--   0 johnyan    (501) staff       (20)      158 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/static/sort_desc.png
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/airflow/www/templates/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1877 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/calendar.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2581 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/chart.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1345 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/circles.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1217 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/code.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1894 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/config.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/confirm.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1038 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_create.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1049 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_edit.html
+-rw-r--r--   0 johnyan    (501) staff       (20)    21916 2021-09-21 03:40:31.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1306 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_code.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2526 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_dependencies.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3424 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_details.html
+-rw-r--r--   0 johnyan    (501) staff       (20)    16490 2021-09-21 04:00:33.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/dags.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2900 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/duration_chart.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3268 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/gantt.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     5609 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/graph.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     4035 2021-08-09 08:31:54.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/main.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3173 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/model_list.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      950 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/noaccess.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1495 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/plugin.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/redoc.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2213 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/task.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2387 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/task_instance.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1044 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_code.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2929 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_log.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1431 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/traceback.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     4480 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/tree.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2327 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/trigger.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      999 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_edit.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1468 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_list.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1231 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/airflow/xcom.html
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1195 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/google_analytics.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1807 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/metarouter.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1810 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/analytics/segment.html
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/
+-rw-r--r--   0 johnyan    (501) staff       (20)     4446 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/custom_icons.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1796 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/dag_docs.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3000 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/flash.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      809 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/index.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     1060 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/loading_dots.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     4388 2022-10-13 06:34:20.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     2001 2022-10-13 08:38:39.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_menu.html
+-rw-r--r--   0 johnyan    (501) staff       (20)     3486 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_right.html
+-rw-r--r--   0 johnyan    (501) staff       (20)    16328 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/utils.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2615 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/validators.py
+-rw-r--r--   0 johnyan    (501) staff       (20)   149695 2021-11-22 06:20:23.000000 smartpip2-2.1.9.4/airflow/www/views.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6792 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/webpack.config.js
+-rw-r--r--   0 johnyan    (501) staff       (20)     2549 2021-08-04 09:43:52.000000 smartpip2-2.1.9.4/airflow/www/widgets.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/licenses/
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1131 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-bootstrap.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)      984 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-bootstrap3-typeahead.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)      556 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-connexion.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-d3-shape.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1079 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-d3-tip.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1475 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-d3js.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1062 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-dagre-d3.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1076 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-datatables.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1081 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-elasticmock.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1301 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-flask-kerberos.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)    11349 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-hue.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)    11357 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-jqclock.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1605 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-jquery.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1077 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-moment-strftime.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1075 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-moment.txt
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1096 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/licenses/LICENSE-normalize.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:11.000000 smartpip2-2.1.9.4/scripts/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/scripts/systemd/
+-rw-rw-r--   0 johnyan    (501) staff       (20)      678 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/README
+-rw-rw-r--   0 johnyan    (501) staff       (20)      968 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1195 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-flower.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1200 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-kerberos.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1190 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-scheduler.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1243 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-webserver.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)     1203 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow-worker.service
+-rw-rw-r--   0 johnyan    (501) staff       (20)      824 2021-08-03 16:23:18.000000 smartpip2-2.1.9.4/scripts/systemd/airflow.conf
+-rw-rw-r--   0 johnyan    (501) staff       (20)     4042 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/setup.cfg
+-rw-rw-r--   0 johnyan    (501) staff       (20)    33517 2023-04-26 09:55:02.000000 smartpip2-2.1.9.4/setup.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-04-26 09:55:12.000000 smartpip2-2.1.9.4/smartpip2.egg-info/
+-rw-r--r--   0 johnyan    (501) staff       (20)    26641 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)    44222 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/SOURCES.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/dependency_links.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/entry_points.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2021-08-07 01:38:26.000000 smartpip2-2.1.9.4/smartpip2.egg-info/not-zip-safe
+-rw-r--r--   0 johnyan    (501) staff       (20)    29803 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/requires.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        8 2023-04-26 09:55:10.000000 smartpip2-2.1.9.4/smartpip2.egg-info/top_level.txt
```

### Comparing `smartpip2-2.1.9.3/CHANGELOG.txt` & `smartpip2-2.1.9.4/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/LICENSE` & `smartpip2-2.1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/MANIFEST.in` & `smartpip2-2.1.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/PKG-INFO` & `smartpip2-2.1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: smartpip2
-Version: 2.1.9.3
+Version: 2.1.9.4
 Summary: Programmatically author, schedule and monitor data pipelines
 Home-page: https://www.smartchart.cn/
 Author: Apache Software Foundation
 Author-email: 84345999@qq.com
 License: Apache License 2.0
-Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.3
+Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.4
 Project-URL: Documentation, https://airflow.apache.org/docs/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Description: <!--
          Licensed to the Apache Software Foundation (ASF) under one
          or more contributor license agreements.  See the NOTICE file
          distributed with this work for additional information
@@ -357,116 +357,116 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: apache.webhdfs
-Provides-Extra: apache.hive
 Provides-Extra: jdbc
-Provides-Extra: openfaas
-Provides-Extra: segment
-Provides-Extra: apache.pinot
-Provides-Extra: trino
-Provides-Extra: ftp
-Provides-Extra: samba
-Provides-Extra: grpc
-Provides-Extra: sentry
-Provides-Extra: mongo
-Provides-Extra: celery
-Provides-Extra: tableau
-Provides-Extra: virtualenv
-Provides-Extra: jenkins
-Provides-Extra: presto
-Provides-Extra: pagerduty
-Provides-Extra: zendesk
-Provides-Extra: devel
-Provides-Extra: salesforce
+Provides-Extra: statsd
+Provides-Extra: s3
+Provides-Extra: async
+Provides-Extra: cgroups
+Provides-Extra: all
 Provides-Extra: rabbitmq
-Provides-Extra: apache.drill
-Provides-Extra: cloudant
-Provides-Extra: spark
-Provides-Extra: vertica
-Provides-Extra: mssql
-Provides-Extra: devel_ci
+Provides-Extra: docker
 Provides-Extra: microsoft.winrm
-Provides-Extra: pinot
-Provides-Extra: leveldb
-Provides-Extra: password
+Provides-Extra: pagerduty
+Provides-Extra: druid
+Provides-Extra: snowflake
+Provides-Extra: plexus
+Provides-Extra: discord
+Provides-Extra: slack
+Provides-Extra: apache.livy
+Provides-Extra: celery
+Provides-Extra: databricks
+Provides-Extra: devel
+Provides-Extra: webhdfs
+Provides-Extra: kerberos
 Provides-Extra: jira
+Provides-Extra: devel_hadoop
 Provides-Extra: cncf.kubernetes
-Provides-Extra: singularity
-Provides-Extra: ssh
-Provides-Extra: docker
+Provides-Extra: crypto
+Provides-Extra: microsoft.azure
+Provides-Extra: spark
+Provides-Extra: tableau
+Provides-Extra: cloudant
+Provides-Extra: google
+Provides-Extra: apache.hive
+Provides-Extra: mongo
+Provides-Extra: deprecated_api
+Provides-Extra: openfaas
+Provides-Extra: hdfs
+Provides-Extra: hive
+Provides-Extra: amazon
 Provides-Extra: ldap
-Provides-Extra: papermill
-Provides-Extra: postgres
+Provides-Extra: presto
+Provides-Extra: qubole
+Provides-Extra: telegram
+Provides-Extra: airbyte
+Provides-Extra: gcp_api
+Provides-Extra: ftp
+Provides-Extra: pinot
+Provides-Extra: mysql
+Provides-Extra: odbc
+Provides-Extra: salesforce
+Provides-Extra: neo4j
+Provides-Extra: dingding
+Provides-Extra: devel_ci
 Provides-Extra: apache.atlas
-Provides-Extra: async
-Provides-Extra: snowflake
-Provides-Extra: opsgenie
-Provides-Extra: microsoft.azure
+Provides-Extra: hashicorp
+Provides-Extra: apache.hdfs
+Provides-Extra: mssql
+Provides-Extra: yandex
+Provides-Extra: dask
+Provides-Extra: samba
+Provides-Extra: gcp
+Provides-Extra: imap
+Provides-Extra: jenkins
+Provides-Extra: virtualenv
+Provides-Extra: github_enterprise
+Provides-Extra: segment
+Provides-Extra: devel_all
+Provides-Extra: apache.drill
+Provides-Extra: singularity
 Provides-Extra: aws
+Provides-Extra: postgres
+Provides-Extra: papermill
+Provides-Extra: sendgrid
 Provides-Extra: apache.kylin
-Provides-Extra: qubole
-Provides-Extra: qds
-Provides-Extra: apache.livy
-Provides-Extra: mysql
-Provides-Extra: devel_hadoop
-Provides-Extra: sqlite
-Provides-Extra: apache.beam
-Provides-Extra: apache.druid
+Provides-Extra: opsgenie
+Provides-Extra: asana
+Provides-Extra: oracle
+Provides-Extra: apache.pinot
 Provides-Extra: exasol
-Provides-Extra: all
-Provides-Extra: webhdfs
-Provides-Extra: statsd
+Provides-Extra: apache.cassandra
+Provides-Extra: doc
+Provides-Extra: microsoft.mssql
 Provides-Extra: atlas
+Provides-Extra: kubernetes
+Provides-Extra: apache.beam
+Provides-Extra: elasticsearch
+Provides-Extra: redis
+Provides-Extra: vertica
+Provides-Extra: google_auth
+Provides-Extra: sentry
+Provides-Extra: zendesk
+Provides-Extra: apache.sqoop
+Provides-Extra: http
+Provides-Extra: leveldb
 Provides-Extra: apache.pig
-Provides-Extra: hashicorp
-Provides-Extra: sendgrid
 Provides-Extra: facebook
-Provides-Extra: crypto
-Provides-Extra: azure
-Provides-Extra: slack
-Provides-Extra: apache.hdfs
-Provides-Extra: imap
-Provides-Extra: hive
-Provides-Extra: google_auth
+Provides-Extra: apache.webhdfs
+Provides-Extra: apache.druid
+Provides-Extra: trino
+Provides-Extra: all_dbs
 Provides-Extra: sftp
-Provides-Extra: doc
-Provides-Extra: apache.cassandra
-Provides-Extra: dingding
-Provides-Extra: gcp_api
-Provides-Extra: cassandra
-Provides-Extra: hdfs
 Provides-Extra: winrm
-Provides-Extra: devel_all
-Provides-Extra: gcp
-Provides-Extra: redis
+Provides-Extra: azure
+Provides-Extra: grpc
+Provides-Extra: sqlite
+Provides-Extra: password
 Provides-Extra: apache.spark
-Provides-Extra: odbc
-Provides-Extra: all_dbs
-Provides-Extra: telegram
-Provides-Extra: oracle
-Provides-Extra: dask
-Provides-Extra: neo4j
-Provides-Extra: asana
-Provides-Extra: amazon
-Provides-Extra: apache.sqoop
-Provides-Extra: druid
-Provides-Extra: elasticsearch
-Provides-Extra: s3
-Provides-Extra: cgroups
-Provides-Extra: kubernetes
-Provides-Extra: databricks
-Provides-Extra: deprecated_api
-Provides-Extra: plexus
-Provides-Extra: discord
-Provides-Extra: github_enterprise
-Provides-Extra: google
-Provides-Extra: microsoft.mssql
+Provides-Extra: cassandra
+Provides-Extra: qds
 Provides-Extra: datadog
-Provides-Extra: yandex
-Provides-Extra: kerberos
-Provides-Extra: airbyte
-Provides-Extra: http
+Provides-Extra: ssh
```

### Comparing `smartpip2-2.1.9.3/README.md` & `smartpip2-2.1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/__init__.py` & `smartpip2-2.1.9.4/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/__main__.py` & `smartpip2-2.1.9.4/airflow/__main__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/__init__.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/abstract.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/abstract.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/aiohttp_api.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/aiohttp_api.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/flask_api.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_api.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/apis/flask_utils.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/apis/flask_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/abstract.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/abstract.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/aiohttp_app.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/aiohttp_app.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/apps/flask_app.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/apps/flask_app.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/cli.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/cli.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/coroutine_wrappers.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/coroutine_wrappers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/decorator.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/metrics.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/metrics.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/parameter.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/parameter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/produces.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/produces.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/response.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/response.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/security.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/uri_parsing.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/decorators/validation.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/decorators/validation.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/exceptions.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/handlers.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/handlers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/json_schema.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/json_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/jsonifier.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/jsonifier.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/lifecycle.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/lifecycle.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/mock.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/mock.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/abstract.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/abstract.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/openapi.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/openapi.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/secure.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/secure.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/operations/swagger2.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/operations/swagger2.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/options.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/options.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/problem.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/problem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/resolver.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/resolver.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/setup.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/setup.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/spec.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/spec.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/_vendor/connexion/utils.py` & `smartpip2-2.1.9.4/airflow/_vendor/connexion/utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/alembic.ini` & `smartpip2-2.1.9.4/airflow/alembic.ini`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/__init__.py` & `smartpip2-2.1.9.4/airflow/api/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/auth/__init__.py` & `smartpip2-2.1.9.4/airflow/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/auth/backend/__init__.py` & `smartpip2-2.1.9.4/airflow/api/auth/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/auth/backend/basic_auth.py` & `smartpip2-2.1.9.4/airflow/api/auth/backend/basic_auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/auth/backend/default.py` & `smartpip2-2.1.9.4/airflow/api/auth/backend/default.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/auth/backend/deny_all.py` & `smartpip2-2.1.9.4/airflow/api/auth/backend/deny_all.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/auth/backend/kerberos_auth.py` & `smartpip2-2.1.9.4/airflow/api/auth/backend/kerberos_auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/auth/backend/smart_auth.py` & `smartpip2-2.1.9.4/airflow/api/auth/backend/smart_auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/client/__init__.py` & `smartpip2-2.1.9.4/airflow/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/client/api_client.py` & `smartpip2-2.1.9.4/airflow/api/client/api_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/client/json_client.py` & `smartpip2-2.1.9.4/airflow/api/client/json_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/client/local_client.py` & `smartpip2-2.1.9.4/airflow/api/client/local_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/__init__.py` & `smartpip2-2.1.9.4/airflow/api/common/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/__init__.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/delete_dag.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/delete_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/get_code.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/get_code.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/get_dag_run_state.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/get_dag_runs.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/get_dag_runs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/get_lineage.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/get_lineage.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/get_task.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/get_task.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/get_task_instance.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/get_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/mark_tasks.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/mark_tasks.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/pool.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/pool.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api/common/experimental/trigger_dag.py` & `smartpip2-2.1.9.4/airflow/api/common/experimental/trigger_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/__init__.py` & `smartpip2-2.1.9.4/airflow/api_connexion/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/__init__.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/config_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/config_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/connection_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/connection_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dag_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dag_run_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_run_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dag_source_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dag_source_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/dagsetup_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/dagsetup_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/event_log_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/event_log_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/extra_link_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/extra_link_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/health_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/health_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/import_error_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/import_error_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/log_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/log_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/plugin_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/plugin_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/pool_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/pool_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/provider_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/provider_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/role_and_permission_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/role_and_permission_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/task_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/task_instance_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/task_instance_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/user_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/user_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/variable_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/variable_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/version_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/version_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/endpoints/xcom_endpoint.py` & `smartpip2-2.1.9.4/airflow/api_connexion/endpoints/xcom_endpoint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/exceptions.py` & `smartpip2-2.1.9.4/airflow/api_connexion/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/openapi/v1.yaml` & `smartpip2-2.1.9.4/airflow/api_connexion/openapi/v1.yaml`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/parameters.py` & `smartpip2-2.1.9.4/airflow/api_connexion/parameters.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/__init__.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/common_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/common_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/config_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/config_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/connection_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/connection_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/dag_run_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_run_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/dag_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/dag_source_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/dag_source_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/enum_schemas.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/enum_schemas.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/error_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/error_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/event_log_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/event_log_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/health_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/health_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/log_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/log_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/plugin_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/plugin_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/pool_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/pool_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/provider_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/provider_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/role_and_permission_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/role_and_permission_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/sla_miss_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/sla_miss_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/task_instance_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_instance_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/task_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/task_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/user_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/user_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/variable_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/variable_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/version_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/version_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/schemas/xcom_schema.py` & `smartpip2-2.1.9.4/airflow/api_connexion/schemas/xcom_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/api_connexion/security.py` & `smartpip2-2.1.9.4/airflow/api_connexion/security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/__init__.py` & `smartpip2-2.1.9.4/airflow/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/cli_parser.py` & `smartpip2-2.1.9.4/airflow/cli/cli_parser.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/__init__.py` & `smartpip2-2.1.9.4/airflow/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/celery_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/celery_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/cheat_sheet_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/cheat_sheet_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/config_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/config_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/connection_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/connection_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/dag_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/dag_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/db_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/db_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/info_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/jobs_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/jobs_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/kerberos_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/kerberos_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/kubernetes_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/kubernetes_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/legacy_commands.py` & `smartpip2-2.1.9.4/airflow/cli/commands/legacy_commands.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/plugins_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/plugins_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/pool_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/pool_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/provider_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/provider_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/role_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/role_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/rotate_fernet_key_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/rotate_fernet_key_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/scheduler_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/scheduler_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/sync_perm_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/sync_perm_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/task_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/task_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/user_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/user_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/variable_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/variable_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/version_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/version_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/commands/webserver_command.py` & `smartpip2-2.1.9.4/airflow/cli/commands/webserver_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/cli/simple_table.py` & `smartpip2-2.1.9.4/airflow/cli/simple_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/common/datax.py` & `smartpip2-2.1.9.4/airflow/common/datax.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/common/smartpip.py` & `smartpip2-2.1.9.4/airflow/common/smartpip.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,38 +21,41 @@
     def __init__ (OO0000O0O0OOOO0O0 ,err ='SmartPip Error'):#line:29
         Exception .__init__ (OO0000O0O0OOOO0O0 ,err )#line:30
 def smart_upload (OO00OOO00O00O00O0 ):#line:34
     OOO00000OOO00O0O0 ,O00O00OOO0OO0O00O =os .path .split (OO00OOO00O00O00O0 )#line:35
     O00O00OOO0OO0O00O =O00O00OOO0OO0O00O .split ('.')[0 ]#line:36
     O00OO0OOO0OOO0O0O ={"title":O00O00OOO0OO0O00O ,"token":DATASET_TOKEN ,"visitor":"Airflow"}#line:41
     O00O0O00OO0O00000 ={'file':open (OO00OOO00O00O00O0 ,'rb')}#line:42
-    OOO000000000OOOO0 =f'''{P_URL}/echart/dataset_api/?type=506&visitor=Airflow&token={DATASET_TOKEN}&param={{"uptime":"{time.time()}","filename":"{O00O00OOO0OO0O00O}"}}'''#line:43
+    OOO000000000OOOO0 =f'''{P_URL}/echart/dataset_api/?type=uploadlog&visitor=Airflow&token={DATASET_TOKEN}&param={{"uptime":"{time.time()}","filename":"{O00O00OOO0OO0O00O}"}}'''#line:43
     O0OO0O000O00O00O0 =60 #line:44
-    OO000000O0O00O0OO =requests .post (f'{P_URL}/etl/api/upload_file_api/',files =O00O0O00OO0O00000 ,data =O00OO0OOO0OOO0O0O )#line:46
+    OO000000O0O00O0OO =requests .post (f'{P_URL}/etl/api/upload_file_api/',files =O00O0O00OO0O00000 ,data =O00OO0OOO0OOO0O0O, verify=False )#line:46
     print (OO000000O0O00O0OO .status_code )#line:47
     if OO000000O0O00O0OO .status_code ==200 :#line:48
         OO000000O0O00O0OO =OO000000O0O00O0OO .json ()#line:49
     elif OO000000O0O00O0OO .status_code ==504 :#line:50
         print ('timeout, try waiting...')#line:51
         OO000000O0O00O0OO ={"result":"error","data":"time out"}#line:52
         for O000O0OOOOOOOO00O in range (20 ):#line:53
-            O00O0OOOOO0O0O00O =requests .get (OOO000000000OOOO0 ).json ()#line:54
+            O00O0OOOOO0O0O00O =requests .get (OOO000000000OOOO0, verify=False).json ()#line:54
             print (O00O0OOOOO0O0O00O )#line:55
             O00OO0OOO0OOO0O0O =O00O0OOOOO0O0O00O ['data']#line:56
             if len (O00OO0OOO0OOO0O0O )>1 :#line:57
                 OO000000O0O00O0OO ={"result":"success","data":"uploaded"}#line:58
                 break #line:59
             time .sleep (O0OO0O000O00O00O0 )#line:60
     else :#line:61
         OO000000O0O00O0OO ={"result":"error","data":"some thing wrong"}#line:62
     print (OO000000O0O00O0OO )#line:63
     if OO000000O0O00O0OO ['result']=='error':#line:64
         raise SmartPipError ('Upload Error')#line:65
-def get_dataset (O0OOO000O00OO0OOO ):#line:68
+def get_dataset (O0OOO000O00OO0OOO, param=None ):#line:68
     ""#line:73
+    O0OOO000O00OO0OOO = _OOOOO00OO00O00OO0 +str (O0OOO000O00OO0OOO )
+    if param:
+        O0OOO000O00OO0OOO = f'{O0OOO000O00OO0OOO}&param={json.dumps(param)}'
     OO0O000OO000OO0OO =requests .get (_OOOOO00OO00O00OO0 +str (O0OOO000O00OO0OOO ),verify =False )#line:74
     OO0O000OO000OO0OO =OO0O000OO000OO0OO .json ()#line:75
     return OO0O000OO000OO0OO #line:76
 def dataset (OO00O0O000OOO0OO0 ,OOO0O0OO0O000O0OO ,OO0O0OO0O000OO000 ,tolist =None ):#line:79
     ""#line:86
     O0O0OO00O0O0OOO0O =60 *15 #line:87
     O00OO0000OO000OO0 =3600 *2 #line:88
@@ -101,23 +104,35 @@
             raise SmartPipError ('refresh_dash')#line:135
     except Exception as OOO0O0OO0O0O00OO0 :#line:136
         fun_email (f'{OOOO0OOO0O00O0000}-执行refresh出错',str (OOO0O0OO0O0O00OO0 .args ))#line:137
         raise SmartPipError (str (OOO0O0OO0O0O00OO0 .args ))#line:138
 def refresh_quality (OOO00O0OO0OO0000O ,OOOOOOO0000000O0O ,hours =1 ):#line:140
     ""#line:143
     try :#line:144
-        OO00OOO0OO0OO000O =requests .get (f'{_O0OO0OO00OO0OO00O}{OOOOOOO0000000O0O}&hours={hours}',verify =False )#line:145
+        OO00OOO0OO0OO000O =requests .get (f'{_O00OO00O000O0OOO0}{OOOOOOO0000000O0O}&hours={hours}',verify =False )#line:145
         OO00OOO0OO0OO000O =OO00OOO0OO0OO000O .json ()#line:146
         print (OO00OOO0OO0OO000O )#line:147
         OOO0OOO0O000OOOOO =OO00OOO0OO0OO000O ['status']#line:148
         if OOO0OOO0O000OOOOO !=200 :#line:149
             raise SmartPipError ('refresh_quality')#line:150
     except Exception as O0O0OO0O000000O00 :#line:151
         fun_email (f'{OOO00O0OO0OO0000O}-执行refresh_quality出错',str (O0O0OO0O000000O00 .args ))#line:152
         raise SmartPipError (str (O0O0OO0O000000O00 .args ))#line:153
+def dash_mail (O000000OOO00O0000 ,OOO000O00OOOO0000 ,O0O00OOOOOO000O0O ):#line:1
+    ""#line:5
+    if callable (OOO000O00OOOO0000 ):#line:6
+        O000OOO00O0O0OOO0 =OOO000O00OOOO0000 ()#line:7
+    else :#line:8
+        O000OOO00O0O0OOO0 =OOO000O00OOOO0000 #line:9
+    print (O000OOO00O0O0OOO0 )#line:10
+    if isinstance (O000OOO00O0O0OOO0 ,str ):#line:11
+        fun_email (O000000OOO00O0000 ,O000OOO00O0O0OOO0 ,O0O00OOOOOO000O0O )#line:12
+    else :#line:13
+        fun_email (O000OOO00O0O0OOO0 [0 ],O000OOO00O0O0OOO0 [1 ],O0O00OOOOOO000O0O )#line:14
+    print ('发送邮件成功!')
 def run_bash (O000OOOOOO0OOO0OO ):#line:157
     OOO0OO0O000O0000O =''#line:158
     O0OO00O0OO0OO0OOO =subprocess .Popen (O000OOOOOO0OOO0OO ,stdout =subprocess .PIPE ,stderr =subprocess .STDOUT ,shell =True ,cwd =ETL_FILE_PATH )#line:159
     print ('PID:',O0OO00O0OO0OO0OOO .pid )#line:160
     for OOO0OOOOO00O0OOO0 in iter (O0OO00O0OO0OO0OOO .stdout .readline ,b''):#line:161
         if O0OO00O0OO0OO0OOO .poll ()and OOO0OOOOO00O0OOO0 ==b'':#line:162
             break #line:163
@@ -181,14 +196,17 @@
         else :#line:230
             O00O0O00OO0O00OOO ['targetColumn']='["*"]'#line:231
         if OOO0OO00O00OO0O0O .endswith ('starrocks'):#line:233
             if '.'in O00O0O00OO0O00OOO ['targetTable']:#line:234
                 O00O0O00OO0O00OOO ['targetDB'],O00O0O00OO0O00OOO ['targetTable']=O00O0O00OO0O00OOO ['targetTable'].split ('.')#line:235
             else :#line:236
                 O00O0O00OO0O00OOO ['targetDB']='Test'#line:237
+        else:
+            if 'writeMode' not in O00O0OOOOOO0OO0OO:
+                O00O0OOOOOO0OO0OO['writeMode'] = 'insert'
     if 'preSql'in O00O0OOOOOO0OO0OO :#line:239
         O00O0O00OO0O00OOO ['preSql']=json .dumps (O00O0O00OO0O00OOO ['preSql'].strip ().split (';'))#line:240
     else :#line:241
         O00O0O00OO0O00OOO ['preSql']=''#line:242
     if 'postSql'in O00O0OOOOOO0OO0OO :#line:243
         O00O0O00OO0O00OOO ['postSql']=json .dumps (O00O0O00OO0O00OOO ['postSql'].strip ().split (';'))#line:244
     else :#line:245
@@ -219,20 +237,31 @@
         return 'file type error'#line:275
     with open (O0OO00OOO0OOOOO0O ,'r',encoding ='utf8')as OO0OO0O00OOOOOOO0 :#line:276
         OO0O0OOO000OOO00O =OO0OO0O00OOOOOOO0 .read ().strip ()#line:277
     O000OO0O0O0OOO00O =re .match (r"/\*(.*?)\*/(.+)",OO0O0OOO000OOO00O ,re .M |re .S )#line:278
     OOOO000O0000O00O0 =readSqlstr (O000OO0O0O0OOO00O .group (1 ).strip (),para_dict )#line:279
     O0OO0O00O0000O00O =O000OO0O0O0OOO00O .group (2 ).strip ()#line:280
     return OOOO000O0000O00O0 ,O0OO0O00O0000O00O #line:281
-def readSqlstr (OOO0OO000O0O0O00O ,para_dict =None ):#line:284
-    OOOO00O000OO0OOOO =re .sub (r"(\/\*(.|\n)*?\*\/)|--.*",'',OOO0OO000O0O0O00O .strip ())#line:285
-    if para_dict :#line:286
-        for OO000OO0OOO0OO0OO ,O00O0O00OO00OO000 in para_dict .items ():#line:287
-            OOOO00O000OO0OOOO =OOOO00O000OO0OOOO .replace ('$'+OO000OO0OOO0OO0OO ,str (O00O0O00OO00OO000 ))#line:288
-    return OOOO00O000OO0OOOO #line:289
+def readSqlstr (O00OO00OO00O00OOO ,para_dict =None ):#line:1
+    O0O000O0OOOOOO0O0 =re .sub (r"(\/\*(.|\n)*?\*\/)|--.*",'',O00OO00OO00O00OOO .strip ())#line:2
+    if para_dict :#line:3
+        for OO0OO000OO0OOOOOO ,O00OO000OO0OOO000 in para_dict .items ():#line:4
+            if OO0OO000OO0OOOOOO .isnumeric ():#line:5
+                OO00O0O0OOOO0OOO0 =get_dataset (O00OO000OO0OOO000 )['data']#line:6
+                print ('dataset:',OO00O0O0OOOO0OOO0 )#line:7
+                if len (OO00O0O0OOOO0OOO0 )>1 :#line:8
+                    for OOOOOOOO00O0OO0O0 ,O0O00OO0OOOO0O000 in zip (OO00O0O0OOOO0OOO0 [0 ],OO00O0O0OOOO0OOO0 [1 ]):#line:9
+                        O0O000O0OOOOOO0O0 =O0O000O0OOOOOO0O0 .replace ('$'+OOOOOOOO00O0OO0O0 ,str (O0O00OO0OOOO0O000 ))#line:10
+            elif callable (O00OO000OO0OOO000 ):#line:11
+                O000O0OOOOO000OO0 =O00OO000OO0OOO000 ()#line:12
+                for OOOOOOOO00O0OO0O0 ,O0O00OO0OOOO0O000 in O000O0OOOOO000OO0 .items ():#line:13
+                    O0O000O0OOOOOO0O0 =O0O000O0OOOOOO0O0 .replace ('$'+OOOOOOOO00O0OO0O0 ,str (O0O00OO0OOOO0O000 ))#line:14
+            else :#line:15
+                O0O000O0OOOOOO0O0 =O0O000O0OOOOOO0O0 .replace ('$'+OO0OO000OO0OOOOOO ,str (O00OO000OO0OOO000 ))#line:16
+    return O0O000O0OOOOOO0O0
 def run_sql_file (O00OO0OOOOOOOOOOO ,O00000000OOOOOO00 ,db_connect ='starrocks',para_dict =None ,dev =''):#line:292
     O0000O00O0OO0OO00 =O00OO0OOOOOOOOOOO .split ('/')#line:293
     try :#line:294
         OO0O000OO0OO00OO0 =readSqlFile (O00OO0OOOOOOOOOOO ,para_dict ).split (';')#line:295
         OO0O0000O0OOO000O =O00000000OOOOOO00 .get (db_connect )#line:296
         if dev :#line:297
             if f'{db_connect}{dev}'in O00000000OOOOOO00 .keys ():#line:298
@@ -253,14 +282,24 @@
                 OO0O0O00000OO0000 =OOOOO0OOO0O0O0O0O .get (f'{db_connect}{dev}')#line:315
         O0OOO00O000000OO0 =connect_db_execute ().execute_sql_list (O00O0000O00000O00 ,db_connect ,connect_dict =OO0O0O00000OO0000 )#line:316
         return O0OOO00O000000OO0 #line:317
     except Exception as O0OOO00000OOO00O0 :#line:318
         fun_email ('SQL执行出错',f'{O00O0000O00000O00}{O0OOO00000OOO00O0.args}')#line:319
         print (O0OOO00000OOO00O0 .args )#line:320
         raise SmartPipError ('Run SQL Error')#line:321
+def run_sp (O0OOOOOO00O00OOOO ,O0O00000OOO0OOOO0 ,db_connect ='oracle',sp_para =None ,dev =''):#line:1
+    try :#line:2
+        O0O0OOO0OO0OOOO0O =O0O00000OOO0OOOO0 .get (db_connect )#line:3
+        if dev :#line:4
+            if f'{db_connect}{dev}'in O0O00000OOO0OOOO0 .keys ():#line:5
+                O0O0OOO0OO0OOOO0O =O0O00000OOO0OOOO0 .get (f'{db_connect}{dev}')#line:6
+        connect_db_execute ().excute_proc (O0OOOOOO00O00OOOO ,O0O0OOO0OO0OOOO0O ,sp_para )#line:7
+    except Exception as O0000O00O0000OO00 :#line:8
+        fun_email ('{}执行出错'.format (O0OOOOOO00O00OOOO ),str (O0000O00O0000OO00 .args ))#line:9
+        raise O0000O00O0000OO00
 def run_kettle (O00000O00O0OOOO0O ,para_str ='',dev =False ):#line:325
     ""#line:332
     O0OOOO00000OOO0OO =O00000O00O0OOOO0O .split ('/')#line:333
     print ('kettle job start')#line:334
     if '.ktr'in O00000O00O0OOOO0O :#line:336
         OOO0000OO000OOO0O =f'{KETTLE_HOME}/pan.sh -level=Basic -file={O00000O00O0OOOO0O}{para_str}'#line:337
     else :#line:338
@@ -749,15 +788,15 @@
         ""#line:935
         if OO0O0O0OOOO00OO0O .offsets :#line:936
             if isinstance (OO0O0O0OOOO00OO0O .offsets ,int ):#line:937
                 return OO0O0O0OOOO00OO0O .offsets #line:938
             else :#line:939
                 O0O0O00OOO00OOOOO =OO0O0O0OOOO00OO0O .offsets .get (str (O0000OOOOOO0O0O0O ))#line:940
                 if O0O0O00OOO00OOOOO is not None :#line:941
-                    return O0O0O00OOO00OOOOO #line:942
+                    return int(O0O0O00OOO00OOOOO) #line:942
         O0O0O00OOO00OOOOO =0 #line:943
         try :#line:944
             OOO0O0000O0O000OO =f"{OO0O0O0OOOO00OO0O.current_dir}/kafka/{OO0O000OOOOO00O0O}_offset_{O0000OOOOOO0O0O0O}.txt"#line:945
             if os .path .exists (OOO0O0000O0O000OO ):#line:946
                 O000O0O0O000OOOO0 =open (OOO0O0000O0O000OO ).read ()#line:947
                 if O000O0O0O000OOOO0 :#line:948
                     O0O0O00OOO00OOOOO =int (O000O0O0O000OOOO0 )#line:949
```

### Comparing `smartpip2-2.1.9.3/airflow/compat/__init__.py` & `smartpip2-2.1.9.4/airflow/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/compat/functools.py` & `smartpip2-2.1.9.4/airflow/compat/functools.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/__init__.py` & `smartpip2-2.1.9.4/airflow/config_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/airflow_local_settings.py` & `smartpip2-2.1.9.4/airflow/config_templates/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/config.yml` & `smartpip2-2.1.9.4/airflow/config_templates/config.yml`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/config.yml.schema.json` & `smartpip2-2.1.9.4/airflow/config_templates/config.yml.schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/default_airflow.cfg` & `smartpip2-2.1.9.4/airflow/config_templates/default_airflow.cfg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/default_celery.py` & `smartpip2-2.1.9.4/airflow/config_templates/default_celery.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/default_functions.py` & `smartpip2-2.1.9.4/airflow/config_templates/default_functions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/default_test.cfg` & `smartpip2-2.1.9.4/airflow/config_templates/default_test.cfg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/config_templates/default_webserver_config.py` & `smartpip2-2.1.9.4/airflow/config_templates/default_webserver_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/configuration.py` & `smartpip2-2.1.9.4/airflow/configuration.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/dagsetup/config_dagfile.py` & `smartpip2-2.1.9.4/airflow/contrib/dagsetup/config_dagfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # -*- coding:utf-8 -*-
 import_format = '''# -*- coding:utf-8 -*-
 import os
 import sys
 import datetime
+import airflow
+from airflow.operators.python import PythonOperator, BranchPythonOperator
+from airflow.operators.trigger_dagrun import TriggerDagRunOperator
+from airflow.operators.bash import BashOperator
+from airflow import DAG
+from airflow.models import Variable
 pathname = os.path.dirname(os.path.abspath(__file__))
 sys.path.insert(0, pathname)
 sys.path.insert(0, os.path.abspath(os.path.join(pathname, '..')))
 
 from common{common_path}.functions import *
-from airflow.models import Variable
+
 dev=''
 retry_delay_minutes = 3
 '''
 
 param_format = '''
 # get your param from airflow web
 {param} = Variable.get('{param}')
@@ -116,15 +122,14 @@
 execute_sqlstr_format = '''
 # execute db sql script
 def S_{filename}():
     para_dict = dict(zip('{param}'.split(','),[{param}]))
     run_sql_str({remark},'{db}',para_dict,dev=dev)
 '''
 
-# 0 - sp name, 1 - para string
 execute_sp_format = '''
 # execute db procedure
 def S_{filename}():
     run_sp('{filename}',[{param}],dev=dev)
 '''
 
 execute_sqoop_format = '''
@@ -136,15 +141,15 @@
 '''
 
 execute_hdfsstarrocks_format = '''
 # execute starrocks script
 def S_{filename}():
     path = os.path.join(ETL_FILE_PATH , '{project_name}/{filename}.sql')
     para_dict = dict(zip('{param}'.split(','),[{param}]))
-    run_starrocks(path, para_dict)
+    hdfsStarrocks(path, para_dict)
 '''
 
 execute_sap_format = '''
 # execute sap rfc script
 def S_{filename}():
     path = os.path.join(ETL_FILE_PATH , '{project_name}/{filename}.json')
     para_dict = dict(zip('{param}'.split(','),[{param}]))
@@ -152,20 +157,14 @@
 '''
 
 param_str_format = ''' ' "-param:{item_param}={{}}"'.format({item_param}) '''
 
 dag_import_format = '''# -*- coding:utf-8 -*-
 import os
 import sys
-from airflow.operators.python import PythonOperator, BranchPythonOperator
-from airflow.operators.trigger_dagrun import TriggerDagRunOperator
-from airflow.operators.bash import BashOperator
-
-from airflow import DAG
-import airflow
 pathname = os.path.dirname(os.path.abspath(__file__))
 sys.path.insert(0, pathname)
 sys.path.insert(0, os.path.abspath(os.path.join(pathname, '..')))
 from etl_script.{project_name} import *
 '''
 
 dag_config_format = '''
@@ -214,18 +213,20 @@
     python_callable={funname},
     dag=dag
 )
 {filename}.ui_color = '{color}'
 {filename}.driver = '{driver}'
 '''
 
+
 dag_jobs_format_diy = '''
 {filename} = PythonOperator(
     task_id='{filename}',
     python_callable={funname},
+    provide_context = True,
     dag=dag
 )
 {filename}.ui_color = '{color}'
 {filename}.driver = '{driver}'
 '''
 
 dag_jobs_format_trigger = '''
@@ -262,30 +263,35 @@
 execute_dataset_format = '''
 # execute dataset script
 def S_{filename}():
     dataset('{filename}','{param}','{remark}',{tolist})
 '''
 # check starrocks routine job
 execute_routinestarrocks_format = '''
-# execute dataset script
 def S_{filename}():
     routineStarrocks('{label}','{flag}')
 '''
 
-# check dataset
+# refresh dashboard
 execute_dash_format = '''
-# execute dataset script
 def S_{filename}():
     refresh_dash('{filename}','{param}')
 '''
 
-execute_quality_format = '''
 # execute quality script
+execute_quality_format = '''
 def S_{filename}():
     refresh_quality('{filename}','{param}')
 '''
 
-refresh_tableau_format = '''
+
+# send mail
+execute_mail_format = '''
+def S_{filename}():
+    dash_mail('{filename}',{ds_fun},{tolist})
+'''
+
 # refresh tableau source script
+refresh_tableau_format = '''
 def S_{filename}():
     refreshTableauSource({sourceID})
 '''
```

### Comparing `smartpip2-2.1.9.3/airflow/contrib/dagsetup/dagfile_test.py` & `smartpip2-2.1.9.4/airflow/contrib/dagsetup/dagfile_test.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/dagsetup/gen_airflow_dagfile.py` & `smartpip2-2.1.9.4/airflow/contrib/dagsetup/gen_airflow_dagfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,25 @@
     'oracle_sql': {'color': '#74946e', 't': 'sql'},
     'mssql_sql': {'color': '#74946e', 't': 'sql'},
     'starrocks_sql': {'color': '#74946e', 't': 'sql'},
     'sqoop': {'color': '#665908', 't': 'sql'},
     'sap': {'color': '#f4a460', 't': 'json'},
     'trigger': {'color': '#9cbaba'},
     'branch': {'color': '#3d7373'},
-    'diy': {'color': '#c46c6c'},
+    'diy': {'color': '#c46c6c', 't': 'sql'},
     'hdfs': {'color': '#4675bf', 't': 'ktr'},
     'datax': {'color': '#4675cf', 't': 'sql'},
     'dataxx': {'color': '#4675df', 't': 'json'},
     'refresh_smc': {'color': '#6675df'},
     'refresh_quality': {'color': '#6875df'},
     'hdfsstarrocks': {'color': '#665998', 't': 'sql'},
     'kafkastarrocks': {'color': '#e8a6a6', 't': 'sql'},
     'apistarrocks': {'color': '#eea6a6', 't': 'sql'},
     'routinestarrocks': {'color': '#b4a7d6'},
+    'send_mail': {'color': 'green'},
 }
 
 
 def gen_airflow_dag(*args, **kwargs):
     """
     generate the airflow etl_script and dag file
     :param owner: 负责人
@@ -77,15 +78,15 @@
     if mail:
         extra_args = f"'email': '{mail}'"
     # -----------------transfer job str to job list---------------------
     user_define = ''
     if isinstance(job_list, str):
         items = job_list.split('#')
         # 第一行预留给写自定义参数或代码
-        user_define = items[0].strip()
+        user_define = items[0].strip().replace('--', '#')
         job_list = []
         # 过滤每一个
         for item in items[1:]:
             item = item.strip().split('--')[0]
             if item:
                 item_lst = item.split('|')
                 if len(item_lst) < 2:
@@ -212,14 +213,17 @@
             etl_str = etl_str + execute_dash_format.format(filename=item[1], param=item[2])
         elif driver == 'refresh_quality':
             etl_str = etl_str + execute_quality_format.format(filename=item[1], param=item[2])
         elif driver == 'dataset':
             if '@' in item[4]: item[4] = f'"{item[4]}"'
             etl_str = etl_str + execute_dataset_format.format(filename=item[1], param=item[2], remark=item[3],
                                                               tolist=item[4])
+        elif driver == 'send_mail':
+            if '@' in item[3]: item[3] = f'"{item[3]}"'
+            etl_str = etl_str + execute_mail_format.format(filename=item[1],ds_fun=item[2], tolist=item[3])
         dag_str = dag_str + item[1] + ' >> '
     # save the script py
     o_fileanme = AIRFLOW_HOME + '/etl_script/' + project_name + '.py'
     with open(o_fileanme, 'w', encoding='utf-8') as fo:
         fo.write(etl_str)
 
     # ----------------------gen dag file----------------------------------
```

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_athena_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_athena_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_datasync_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_datasync_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_dynamodb_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_dynamodb_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_firehose_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_firehose_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_glue_catalog_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_glue_catalog_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_lambda_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_lambda_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_logs_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_logs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_sns_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sns_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/aws_sqs_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/aws_sqs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/azure_container_instance_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_instance_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/azure_container_registry_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_registry_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/azure_container_volume_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_container_volume_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/azure_cosmos_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_cosmos_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/azure_data_lake_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_data_lake_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/azure_fileshare_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/azure_fileshare_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/bigquery_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/bigquery_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/cassandra_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/cassandra_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/cloudant_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/cloudant_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/databricks_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/databricks_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/datadog_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/datadog_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/datastore_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/datastore_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/dingding_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/dingding_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/discord_webhook_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/discord_webhook_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/emr_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/emr_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/fs_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/fs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/ftp_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/ftp_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_api_base_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_api_base_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_bigtable_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_bigtable_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_cloud_build_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_cloud_build_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_compute_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_compute_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_container_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_container_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_dataflow_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataflow_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_dataproc_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dataproc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_dlp_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_dlp_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_function_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_function_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_kms_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_kms_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_mlengine_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_mlengine_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_natural_language_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_natural_language_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_pubsub_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_pubsub_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_spanner_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_spanner_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_speech_to_text_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_speech_to_text_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_sql_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_sql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_tasks_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_tasks_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_text_to_speech_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_text_to_speech_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_transfer_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_transfer_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_translate_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_translate_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_video_intelligence_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_video_intelligence_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcp_vision_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcp_vision_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gcs_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gcs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/gdrive_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/gdrive_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/grpc_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/grpc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/imap_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/imap_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/jenkins_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/jenkins_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/jira_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/jira_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/mongo_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/mongo_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/openfaas_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/openfaas_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/opsgenie_alert_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/opsgenie_alert_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/pagerduty_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/pagerduty_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/pinot_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/pinot_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/qubole_check_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_check_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/qubole_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/qubole_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/redis_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/redis_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/redshift_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/redshift_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/sagemaker_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/sagemaker_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/salesforce_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/salesforce_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/segment_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/segment_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/sftp_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/sftp_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/slack_webhook_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/slack_webhook_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/snowflake_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/snowflake_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/spark_jdbc_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/spark_jdbc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/spark_sql_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/spark_sql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/spark_submit_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/spark_submit_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/sqoop_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/sqoop_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/ssh_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/ssh_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/vertica_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/vertica_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/wasb_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/wasb_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/hooks/winrm_hook.py` & `smartpip2-2.1.9.4/airflow/contrib/hooks/winrm_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/adls_list_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/adls_list_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/adls_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/adls_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/aws_athena_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/aws_athena_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/aws_sqs_publish_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/aws_sqs_publish_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/awsbatch_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/awsbatch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/azure_container_instances_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/azure_container_instances_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/azure_cosmos_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/azure_cosmos_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_check_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_get_data.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_get_data.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_table_delete_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_table_delete_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_to_bigquery.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/bigquery_to_mysql_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/bigquery_to_mysql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/cassandra_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/cassandra_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/databricks_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/databricks_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/dataflow_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/dataflow_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/dataproc_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/dataproc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/datastore_export_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/datastore_export_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/datastore_import_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/datastore_import_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/dingding_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/dingding_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/discord_webhook_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/discord_webhook_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/docker_swarm_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/docker_swarm_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/druid_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/druid_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/dynamodb_to_s3.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/ecs_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/ecs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/emr_add_steps_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/emr_add_steps_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/emr_create_job_flow_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/emr_create_job_flow_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/emr_terminate_job_flow_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/emr_terminate_job_flow_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/file_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/file_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/file_to_wasb.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/file_to_wasb.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_bigtable_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_bigtable_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_cloud_build_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_cloud_build_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_compute_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_compute_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_container_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_container_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_dlp_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_dlp_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_function_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_function_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_natural_language_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_natural_language_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_spanner_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_spanner_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_speech_to_text_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_speech_to_text_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_sql_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_sql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_tasks_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_tasks_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_text_to_speech_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_text_to_speech_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_transfer_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_transfer_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_translate_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_translate_speech_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_translate_speech_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_video_intelligence_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_video_intelligence_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcp_vision_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcp_vision_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_acl_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_acl_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_delete_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_delete_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_download_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_download_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_list_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_list_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_bq.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_bq.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gcs_transfer_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_gdrive_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_gdrive_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/gcs_to_s3.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/grpc_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/grpc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/hive_to_dynamodb.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/imap_attachment_to_s3_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/imap_attachment_to_s3_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/jenkins_job_trigger_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/jenkins_job_trigger_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/jira_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/jira_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/kubernetes_pod_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/kubernetes_pod_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/mlengine_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/mlengine_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/mongo_to_s3.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/mssql_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/mssql_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/mysql_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/mysql_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/opsgenie_alert_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/opsgenie_alert_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_azure_data_lake_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/oracle_to_oracle_transfer.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/oracle_to_oracle_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/postgres_to_gcs_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/postgres_to_gcs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/pubsub_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/pubsub_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/qubole_check_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/qubole_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/qubole_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/qubole_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/redis_publish_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/redis_publish_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/s3_copy_object_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/s3_copy_object_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/s3_delete_objects_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/s3_delete_objects_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/s3_list_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/s3_list_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/s3_to_gcs_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/s3_to_gcs_transfer_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_gcs_transfer_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/s3_to_sftp_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/s3_to_sftp_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_base_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_base_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_endpoint_config_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_config_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_endpoint_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_endpoint_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_model_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_model_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_training_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_training_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_transform_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_transform_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sagemaker_tuning_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sagemaker_tuning_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/segment_track_event_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/segment_track_event_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sftp_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sftp_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sftp_to_s3_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sftp_to_s3_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/slack_webhook_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/slack_webhook_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/snowflake_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/snowflake_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sns_publish_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sns_publish_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/spark_jdbc_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/spark_jdbc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/spark_sql_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/spark_sql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/spark_submit_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/spark_submit_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sql_to_gcs.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sql_to_gcs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/sqoop_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/sqoop_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/ssh_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/ssh_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/vertica_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/vertica_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/vertica_to_hive.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/vertica_to_mysql.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/wasb_delete_blob_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/wasb_delete_blob_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/operators/winrm_operator.py` & `smartpip2-2.1.9.4/airflow/contrib/operators/winrm_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/secrets/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/secrets/aws_secrets_manager.py` & `smartpip2-2.1.9.4/airflow/contrib/secrets/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/secrets/aws_systems_manager.py` & `smartpip2-2.1.9.4/airflow/contrib/secrets/aws_systems_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/secrets/azure_key_vault.py` & `smartpip2-2.1.9.4/airflow/contrib/secrets/azure_key_vault.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/secrets/gcp_secrets_manager.py` & `smartpip2-2.1.9.4/airflow/contrib/secrets/gcp_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/secrets/hashicorp_vault.py` & `smartpip2-2.1.9.4/airflow/contrib/secrets/hashicorp_vault.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/aws_athena_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_athena_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_glue_catalog_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/aws_redshift_cluster_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_redshift_cluster_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/aws_sqs_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/aws_sqs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/azure_cosmos_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/azure_cosmos_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/bash_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/bash_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/bigquery_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/bigquery_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/cassandra_record_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_record_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/cassandra_table_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/cassandra_table_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/celery_queue_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/celery_queue_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/datadog_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/datadog_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/emr_base_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/emr_base_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/emr_job_flow_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/emr_job_flow_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/emr_step_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/emr_step_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/file_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/file_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/ftp_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/ftp_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/gcp_transfer_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/gcp_transfer_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/gcs_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/gcs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/hdfs_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/hdfs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/imap_attachment_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/imap_attachment_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/jira_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/jira_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/mongo_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/mongo_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/pubsub_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/pubsub_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/python_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/python_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/qubole_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/qubole_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/redis_key_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/redis_key_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/redis_pub_sub_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/redis_pub_sub_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_base_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_base_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_endpoint_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_endpoint_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_training_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_training_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_transform_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_transform_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/sagemaker_tuning_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/sagemaker_tuning_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/sftp_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/sftp_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/wasb_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/wasb_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/sensors/weekday_sensor.py` & `smartpip2-2.1.9.4/airflow/contrib/sensors/weekday_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/task_runner/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/task_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/task_runner/cgroup_task_runner.py` & `smartpip2-2.1.9.4/airflow/contrib/task_runner/cgroup_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/gcp_field_sanitizer.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_sanitizer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/gcp_field_validator.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/gcp_field_validator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/log/__init__.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/log/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/log/task_handler_with_custom_formatter.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/log/task_handler_with_custom_formatter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/mlengine_operator_utils.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_operator_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/mlengine_prediction_summary.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/mlengine_prediction_summary.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/sendgrid.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/sendgrid.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/contrib/utils/weekday.py` & `smartpip2-2.1.9.4/airflow/contrib/utils/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/customized_form_field_behaviours.schema.json` & `smartpip2-2.1.9.4/airflow/customized_form_field_behaviours.schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/decorators/__init__.py` & `smartpip2-2.1.9.4/airflow/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/decorators/base.py` & `smartpip2-2.1.9.4/airflow/decorators/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/decorators/python.py` & `smartpip2-2.1.9.4/airflow/decorators/python.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/decorators/python_virtualenv.py` & `smartpip2-2.1.9.4/airflow/decorators/python_virtualenv.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/decorators/task_group.py` & `smartpip2-2.1.9.4/airflow/decorators/task_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/__init__.py` & `smartpip2-2.1.9.4/airflow/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_bash_operator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_bash_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_branch_datetime_operator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_branch_datetime_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_branch_day_of_week_operator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_branch_day_of_week_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_branch_labels.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_branch_labels.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_branch_operator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_branch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_branch_python_dop_operator_3.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_branch_python_dop_operator_3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_complex.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_complex.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_dag_decorator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_dag_decorator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_external_task_marker_dag.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_external_task_marker_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_kubernetes_executor.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_kubernetes_executor_config.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_kubernetes_executor_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_latest_only.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_latest_only.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_latest_only_with_trigger.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_latest_only_with_trigger.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_nested_branch_dag.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_nested_branch_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_passing_params_via_test_command.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_passing_params_via_test_command.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_python_operator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_python_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_short_circuit_operator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_short_circuit_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_skip_dag.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_skip_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_subdag_operator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_subdag_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_task_group.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_task_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_task_group_decorator.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_task_group_decorator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_trigger_controller_dag.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_trigger_controller_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_trigger_target_dag.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_trigger_target_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_xcom.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_xcom.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/example_xcomargs.py` & `smartpip2-2.1.9.4/airflow/example_dags/example_xcomargs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/libs/__init__.py` & `smartpip2-2.1.9.4/airflow/example_dags/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/libs/helper.py` & `smartpip2-2.1.9.4/airflow/example_dags/libs/helper.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/subdags/__init__.py` & `smartpip2-2.1.9.4/airflow/example_dags/subdags/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/subdags/subdag.py` & `smartpip2-2.1.9.4/airflow/example_dags/subdags/subdag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/test_utils.py` & `smartpip2-2.1.9.4/airflow/example_dags/test_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/tutorial.py` & `smartpip2-2.1.9.4/airflow/example_dags/tutorial.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/tutorial_etl_dag.py` & `smartpip2-2.1.9.4/airflow/example_dags/tutorial_etl_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/tutorial_taskflow_api_etl.py` & `smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py` & `smartpip2-2.1.9.4/airflow/example_dags/tutorial_taskflow_api_etl_virtualenv.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/exceptions.py` & `smartpip2-2.1.9.4/airflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/__init__.py` & `smartpip2-2.1.9.4/airflow/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/base_executor.py` & `smartpip2-2.1.9.4/airflow/executors/base_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/celery_executor.py` & `smartpip2-2.1.9.4/airflow/executors/celery_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/celery_kubernetes_executor.py` & `smartpip2-2.1.9.4/airflow/executors/celery_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/dask_executor.py` & `smartpip2-2.1.9.4/airflow/executors/dask_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/debug_executor.py` & `smartpip2-2.1.9.4/airflow/executors/debug_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/executor_constants.py` & `smartpip2-2.1.9.4/airflow/executors/executor_constants.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/executor_loader.py` & `smartpip2-2.1.9.4/airflow/executors/executor_loader.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/kubernetes_executor.py` & `smartpip2-2.1.9.4/airflow/executors/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/local_executor.py` & `smartpip2-2.1.9.4/airflow/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/executors/sequential_executor.py` & `smartpip2-2.1.9.4/airflow/executors/sequential_executor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/S3_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/S3_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/__init__.py` & `smartpip2-2.1.9.4/airflow/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/base.py` & `smartpip2-2.1.9.4/airflow/hooks/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/base_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/base_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/dbapi.py` & `smartpip2-2.1.9.4/airflow/hooks/dbapi.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/dbapi_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/dbapi_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/docker_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/docker_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/druid_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/druid_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/filesystem.py` & `smartpip2-2.1.9.4/airflow/hooks/filesystem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/hdfs_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/hdfs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/hive_hooks.py` & `smartpip2-2.1.9.4/airflow/hooks/hive_hooks.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/http_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/http_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/jdbc_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/jdbc_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/mssql_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/mssql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/mysql_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/mysql_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/oracle_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/oracle_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/pig_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/pig_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/postgres_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/postgres_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/presto_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/presto_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/samba_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/samba_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/slack_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/slack_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/sqlite_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/sqlite_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/subprocess.py` & `smartpip2-2.1.9.4/airflow/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/webhdfs_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/webhdfs_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/hooks/zendesk_hook.py` & `smartpip2-2.1.9.4/airflow/hooks/zendesk_hook.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/jobs/__init__.py` & `smartpip2-2.1.9.4/airflow/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/jobs/backfill_job.py` & `smartpip2-2.1.9.4/airflow/jobs/backfill_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/jobs/base_job.py` & `smartpip2-2.1.9.4/airflow/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/jobs/local_task_job.py` & `smartpip2-2.1.9.4/airflow/jobs/local_task_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/jobs/scheduler_job.py` & `smartpip2-2.1.9.4/airflow/jobs/scheduler_job.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/__init__.py` & `smartpip2-2.1.9.4/airflow/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/k8s_model.py` & `smartpip2-2.1.9.4/airflow/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/kube_client.py` & `smartpip2-2.1.9.4/airflow/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/kube_config.py` & `smartpip2-2.1.9.4/airflow/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/kubernetes_helper_functions.py` & `smartpip2-2.1.9.4/airflow/kubernetes/kubernetes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/pod.py` & `smartpip2-2.1.9.4/airflow/kubernetes/pod.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/pod_generator.py` & `smartpip2-2.1.9.4/airflow/kubernetes/pod_generator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/pod_generator_deprecated.py` & `smartpip2-2.1.9.4/airflow/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/pod_launcher.py` & `smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/pod_launcher_deprecated.py` & `smartpip2-2.1.9.4/airflow/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/pod_runtime_info_env.py` & `smartpip2-2.1.9.4/airflow/kubernetes/pod_runtime_info_env.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/refresh_config.py` & `smartpip2-2.1.9.4/airflow/kubernetes/refresh_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/secret.py` & `smartpip2-2.1.9.4/airflow/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/volume.py` & `smartpip2-2.1.9.4/airflow/kubernetes/volume.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/kubernetes/volume_mount.py` & `smartpip2-2.1.9.4/airflow/kubernetes/volume_mount.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/lineage/__init__.py` & `smartpip2-2.1.9.4/airflow/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/lineage/backend.py` & `smartpip2-2.1.9.4/airflow/lineage/backend.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/lineage/entities.py` & `smartpip2-2.1.9.4/airflow/lineage/entities.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/logging_config.py` & `smartpip2-2.1.9.4/airflow/logging_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/macros/__init__.py` & `smartpip2-2.1.9.4/airflow/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/macros/hive.py` & `smartpip2-2.1.9.4/airflow/macros/hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/__init__.py` & `smartpip2-2.1.9.4/airflow/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/env.py` & `smartpip2-2.1.9.4/airflow/migrations/env.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/004c1210f153_increase_queue_name_size_limit.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/03afc6b6f902_increase_length_of_fab_ab_view_menu_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/03bc53e68815_add_sm_dag_index.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/05f30312d566_merge_heads.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/05f30312d566_merge_heads.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/0a2a5b66e19d_add_task_reschedule_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/0e2a74e0fc9f_add_time_zone_awareness.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/127d2bf2dfa7_add_dag_id_state_index_on_dag_run_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/13eb55f81627_for_compatibility.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/13eb55f81627_for_compatibility.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/1507a7289a2f_create_is_encrypted.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/1968acfc09e3_add_is_encrypted_column_to_variable_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/1b38cef5b76e_add_dagrun.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/211e584da130_add_ti_state_index.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/211e584da130_add_ti_state_index.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/27c6a30d7c24_add_executor_config_to_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/2c6edca13270_resource_based_permissions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/2e42bb497a22_rename_last_scheduler_run_column.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/2e541a1dcfed_task_duration.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/2e541a1dcfed_task_duration.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/2e82aab8ef20_rename_user_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/338e90f54d61_more_logging_into_task_isntance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/33ae817a1ff4_add_kubernetes_resource_checkpointing.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/364159666cbd_add_job_id_to_dagrun_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/3c20cacc0044_add_dagrun_run_type.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/40e67319e3a9_dagrun_config.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/40e67319e3a9_dagrun_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/41f5f12752f8_add_superuser_field.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/4446e08588_dagrun_start_end.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/4446e08588_dagrun_start_end.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/449b4072c2da_increase_size_of_connection_extra_field_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/45ba3f1493b9_add_k8s_yaml_to_rendered_templates.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/4addfa1236f1_add_fractional_seconds_to_mysql_tables.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/502898887f84_adding_extra_to_log.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/502898887f84_adding_extra_to_log.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/52d53670a240_fix_mssql_exec_date_rendered_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/52d714495f0_job_id_indices.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/52d714495f0_job_id_indices.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/561833c1c74b_add_password_column_to_user.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/5e7d17757c7a_add_pid_field_to_taskinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/61ec73d9401f_add_description_field_to_connection.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/64a7d6477aae_fix_description_field_in_connection_to_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/64de9cddf6c9_add_task_fails_journal_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/6e96a59344a4_make_taskinstance_pool_not_nullable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/74effc47d867_change_datetime_to_datetime2_6_on_mssql_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/7939bcff74ba_add_dagtags_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/82b7c48c147f_remove_can_read_permission_on_config_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/849da589634d_prefix_dag_permissions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/8504051e801b_xcom_dag_task_indices.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/852ae6c715af_add_rendered_task_instance_fields_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/856955da8476_fix_sqlite_foreign_key.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/8646922c8a04_change_default_pool_slots_to_1.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/86770d1215c0_add_kubernetes_scheduler_uniqueness.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/8d48763f6d53_add_unique_constraint_to_conn_id.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/8f966b9c467a_set_conn_type_as_non_nullable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/90d1635d7b86_increase_pool_name_size_in_taskinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/92c57b58940d_add_fab_tables.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/92c57b58940d_add_fab_tables.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/939bb1e647c8_task_reschedule_fk_on_cascade_delete.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/947454bf1dff_add_ti_job_id_index.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/952da73b5eff_add_dag_code_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/9635ae0956e7_index_faskfail.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/9635ae0956e7_index_faskfail.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/98271e7606e2_add_scheduling_decision_to_dagrun_and_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/__init__.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/a13f7613ad25_resource_based_permissions_for_default_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/a4c2fd67d16b_add_pool_slots_field_to_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/a56c9515abdc_remove_dag_stat_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/a66efa278eea_add_precision_to_execution_date_in_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/b0125267960b_merge_heads.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/b0125267960b_merge_heads.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/b247b1e3d1ed_add_queued_by_job_id_to_ti.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/b25a55525161_increase_length_of_pool_name.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/b3b105409875_add_root_dag_id_to_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/bba5a7cfc896_add_a_column_to_track_the_encryption_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/bbc73705a13e_add_notification_sent_column_to_sla_miss.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/bbf4a7ad0465_remove_id_column_from_xcom.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/bdaa763e6c56_make_xcom_value_column_a_large_binary.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/bef4f3d11e8b_drop_kuberesourceversion_and_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/bf00311e1990_add_index_to_taskinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/c8ffec048a3b_add_fields_to_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/cc1e65623dc7_add_max_tries_column_to_task_instance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/cf5dc11e79ad_drop_user_and_chart.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/d2ae31099d61_increase_text_size_for_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/d38e04c12aa2_add_serialized_dag_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/da3f683c3a5a_add_dag_hash_column_to_serialized_dag_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/dd25f486b8ea_add_idx_log_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/dd4ecb8fbee3_add_schedule_interval_to_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/e165e7455d70_add_description_field_to_variable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/e1a11ece99cc_add_external_executor_id_to_ti.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/e38be357a868_update_schema_for_smart_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/e3a246e0dc1_current_schema.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/e3a246e0dc1_current_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/e959f08ac86c_change_field_in_dagcode_to_mediumtext_.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/f23433877c24_fix_mysql_not_null_constraint.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/f2ca10b85618_add_dag_stats_table.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py` & `smartpip2-2.1.9.4/airflow/migrations/versions/fe461863935f_increase_length_for_connection_password.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/__init__.py` & `smartpip2-2.1.9.4/airflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/base.py` & `smartpip2-2.1.9.4/airflow/models/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/baseoperator.py` & `smartpip2-2.1.9.4/airflow/models/baseoperator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/connection.py` & `smartpip2-2.1.9.4/airflow/models/connection.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/crypto.py` & `smartpip2-2.1.9.4/airflow/models/crypto.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/dag.py` & `smartpip2-2.1.9.4/airflow/models/dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/dagbag.py` & `smartpip2-2.1.9.4/airflow/models/dagbag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/dagcode.py` & `smartpip2-2.1.9.4/airflow/models/dagcode.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/dagparam.py` & `smartpip2-2.1.9.4/airflow/models/dagparam.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/dagpickle.py` & `smartpip2-2.1.9.4/airflow/models/dagpickle.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/dagrun.py` & `smartpip2-2.1.9.4/airflow/models/dagrun.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/errors.py` & `smartpip2-2.1.9.4/airflow/models/errors.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/log.py` & `smartpip2-2.1.9.4/airflow/models/log.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/pool.py` & `smartpip2-2.1.9.4/airflow/models/pool.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/renderedtifields.py` & `smartpip2-2.1.9.4/airflow/models/renderedtifields.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/sensorinstance.py` & `smartpip2-2.1.9.4/airflow/models/sensorinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/serialized_dag.py` & `smartpip2-2.1.9.4/airflow/models/serialized_dag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/skipmixin.py` & `smartpip2-2.1.9.4/airflow/models/skipmixin.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/slamiss.py` & `smartpip2-2.1.9.4/airflow/models/slamiss.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/taskfail.py` & `smartpip2-2.1.9.4/airflow/models/taskfail.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/taskinstance.py` & `smartpip2-2.1.9.4/airflow/models/taskinstance.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/taskmixin.py` & `smartpip2-2.1.9.4/airflow/models/taskmixin.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/taskreschedule.py` & `smartpip2-2.1.9.4/airflow/models/taskreschedule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/variable.py` & `smartpip2-2.1.9.4/airflow/models/variable.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/xcom.py` & `smartpip2-2.1.9.4/airflow/models/xcom.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/models/xcom_arg.py` & `smartpip2-2.1.9.4/airflow/models/xcom_arg.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/mypy/__init__.py` & `smartpip2-2.1.9.4/airflow/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/mypy/plugin/__init__.py` & `smartpip2-2.1.9.4/airflow/mypy/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/mypy/plugin/decorators.py` & `smartpip2-2.1.9.4/airflow/mypy/plugin/decorators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/__init__.py` & `smartpip2-2.1.9.4/airflow/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/bash.py` & `smartpip2-2.1.9.4/airflow/operators/bash.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/bash_operator.py` & `smartpip2-2.1.9.4/airflow/operators/bash_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/branch.py` & `smartpip2-2.1.9.4/airflow/operators/branch.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/branch_operator.py` & `smartpip2-2.1.9.4/airflow/operators/branch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/check_operator.py` & `smartpip2-2.1.9.4/airflow/operators/check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/dagrun_operator.py` & `smartpip2-2.1.9.4/airflow/operators/dagrun_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/datetime.py` & `smartpip2-2.1.9.4/airflow/operators/datetime.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/docker_operator.py` & `smartpip2-2.1.9.4/airflow/operators/docker_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/druid_check_operator.py` & `smartpip2-2.1.9.4/airflow/operators/druid_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/dummy.py` & `smartpip2-2.1.9.4/airflow/operators/dummy.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/dummy_operator.py` & `smartpip2-2.1.9.4/airflow/operators/dummy_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/email.py` & `smartpip2-2.1.9.4/airflow/operators/email.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/email_operator.py` & `smartpip2-2.1.9.4/airflow/operators/email_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/gcs_to_s3.py` & `smartpip2-2.1.9.4/airflow/operators/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/generic_transfer.py` & `smartpip2-2.1.9.4/airflow/operators/generic_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/google_api_to_s3_transfer.py` & `smartpip2-2.1.9.4/airflow/operators/google_api_to_s3_transfer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/hive_operator.py` & `smartpip2-2.1.9.4/airflow/operators/hive_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/hive_stats_operator.py` & `smartpip2-2.1.9.4/airflow/operators/hive_stats_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/hive_to_druid.py` & `smartpip2-2.1.9.4/airflow/operators/hive_to_druid.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/hive_to_mysql.py` & `smartpip2-2.1.9.4/airflow/operators/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/hive_to_samba_operator.py` & `smartpip2-2.1.9.4/airflow/operators/hive_to_samba_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/http_operator.py` & `smartpip2-2.1.9.4/airflow/operators/http_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/jdbc_operator.py` & `smartpip2-2.1.9.4/airflow/operators/jdbc_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/latest_only.py` & `smartpip2-2.1.9.4/airflow/operators/latest_only.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/latest_only_operator.py` & `smartpip2-2.1.9.4/airflow/operators/latest_only_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/mssql_operator.py` & `smartpip2-2.1.9.4/airflow/operators/mssql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/mssql_to_hive.py` & `smartpip2-2.1.9.4/airflow/operators/mssql_to_hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/mysql_operator.py` & `smartpip2-2.1.9.4/airflow/operators/mysql_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/mysql_to_hive.py` & `smartpip2-2.1.9.4/airflow/operators/mysql_to_hive.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/oracle_operator.py` & `smartpip2-2.1.9.4/airflow/operators/oracle_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/papermill_operator.py` & `smartpip2-2.1.9.4/airflow/operators/papermill_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/pig_operator.py` & `smartpip2-2.1.9.4/airflow/operators/pig_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/postgres_operator.py` & `smartpip2-2.1.9.4/airflow/operators/postgres_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/presto_check_operator.py` & `smartpip2-2.1.9.4/airflow/operators/presto_check_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/presto_to_mysql.py` & `smartpip2-2.1.9.4/airflow/operators/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/python.py` & `smartpip2-2.1.9.4/airflow/operators/python.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/python_operator.py` & `smartpip2-2.1.9.4/airflow/operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/redshift_to_s3_operator.py` & `smartpip2-2.1.9.4/airflow/operators/redshift_to_s3_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/s3_file_transform_operator.py` & `smartpip2-2.1.9.4/airflow/operators/s3_file_transform_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/s3_to_hive_operator.py` & `smartpip2-2.1.9.4/airflow/operators/s3_to_hive_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/s3_to_redshift_operator.py` & `smartpip2-2.1.9.4/airflow/operators/s3_to_redshift_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/slack_operator.py` & `smartpip2-2.1.9.4/airflow/operators/slack_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/sql.py` & `smartpip2-2.1.9.4/airflow/operators/sql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/sql_branch_operator.py` & `smartpip2-2.1.9.4/airflow/operators/sql_branch_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/sqlite_operator.py` & `smartpip2-2.1.9.4/airflow/operators/sqlite_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/subdag.py` & `smartpip2-2.1.9.4/airflow/operators/subdag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/subdag_operator.py` & `smartpip2-2.1.9.4/airflow/operators/subdag_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/trigger_dagrun.py` & `smartpip2-2.1.9.4/airflow/operators/trigger_dagrun.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/operators/weekday.py` & `smartpip2-2.1.9.4/airflow/operators/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/plugins_manager.py` & `smartpip2-2.1.9.4/airflow/plugins_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/provider_info.schema.json` & `smartpip2-2.1.9.4/airflow/provider_info.schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/providers_manager.py` & `smartpip2-2.1.9.4/airflow/providers_manager.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/secrets/__init__.py` & `smartpip2-2.1.9.4/airflow/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/secrets/base_secrets.py` & `smartpip2-2.1.9.4/airflow/secrets/base_secrets.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/secrets/environment_variables.py` & `smartpip2-2.1.9.4/airflow/secrets/environment_variables.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/secrets/local_filesystem.py` & `smartpip2-2.1.9.4/airflow/secrets/local_filesystem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/secrets/metastore.py` & `smartpip2-2.1.9.4/airflow/secrets/metastore.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/security/__init__.py` & `smartpip2-2.1.9.4/airflow/security/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/security/kerberos.py` & `smartpip2-2.1.9.4/airflow/security/kerberos.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/security/permissions.py` & `smartpip2-2.1.9.4/airflow/security/permissions.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/security/utils.py` & `smartpip2-2.1.9.4/airflow/security/utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/__init__.py` & `smartpip2-2.1.9.4/airflow/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/base.py` & `smartpip2-2.1.9.4/airflow/sensors/base.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/base_sensor_operator.py` & `smartpip2-2.1.9.4/airflow/sensors/base_sensor_operator.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/bash.py` & `smartpip2-2.1.9.4/airflow/sensors/bash.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/date_time.py` & `smartpip2-2.1.9.4/airflow/sensors/date_time.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/date_time_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/date_time_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/external_task.py` & `smartpip2-2.1.9.4/airflow/sensors/external_task.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/external_task_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/filesystem.py` & `smartpip2-2.1.9.4/airflow/sensors/filesystem.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/hdfs_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/hdfs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/hive_partition_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/hive_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/http_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/http_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/metastore_partition_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/metastore_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/named_hive_partition_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/named_hive_partition_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/python.py` & `smartpip2-2.1.9.4/airflow/sensors/python.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/s3_key_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/s3_key_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/s3_prefix_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/s3_prefix_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/smart_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/smart_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/sql.py` & `smartpip2-2.1.9.4/airflow/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/sql_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/sql_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/time_delta.py` & `smartpip2-2.1.9.4/airflow/sensors/time_delta.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/time_delta_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/time_delta_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/time_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/time_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/web_hdfs_sensor.py` & `smartpip2-2.1.9.4/airflow/sensors/web_hdfs_sensor.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sensors/weekday.py` & `smartpip2-2.1.9.4/airflow/sensors/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/sentry.py` & `smartpip2-2.1.9.4/airflow/sentry.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/serialization/__init__.py` & `smartpip2-2.1.9.4/airflow/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/serialization/enums.py` & `smartpip2-2.1.9.4/airflow/serialization/enums.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/serialization/helpers.py` & `smartpip2-2.1.9.4/airflow/serialization/helpers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/serialization/json_schema.py` & `smartpip2-2.1.9.4/airflow/serialization/json_schema.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/serialization/schema.json` & `smartpip2-2.1.9.4/airflow/serialization/schema.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/serialization/serialized_objects.py` & `smartpip2-2.1.9.4/airflow/serialization/serialized_objects.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/settings.py` & `smartpip2-2.1.9.4/airflow/settings.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/smart_sensor_dags/__init__.py` & `smartpip2-2.1.9.4/airflow/smart_sensor_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/smart_sensor_dags/smart_sensor_group.py` & `smartpip2-2.1.9.4/airflow/smart_sensor_dags/smart_sensor_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/stats.py` & `smartpip2-2.1.9.4/airflow/stats.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/task/__init__.py` & `smartpip2-2.1.9.4/airflow/task/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/task/task_runner/__init__.py` & `smartpip2-2.1.9.4/airflow/task/task_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/task/task_runner/base_task_runner.py` & `smartpip2-2.1.9.4/airflow/task/task_runner/base_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/task/task_runner/cgroup_task_runner.py` & `smartpip2-2.1.9.4/airflow/task/task_runner/cgroup_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/task/task_runner/standard_task_runner.py` & `smartpip2-2.1.9.4/airflow/task/task_runner/standard_task_runner.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/templates.py` & `smartpip2-2.1.9.4/airflow/templates.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/__init__.py` & `smartpip2-2.1.9.4/airflow/ti_deps/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/dep_context.py` & `smartpip2-2.1.9.4/airflow/ti_deps/dep_context.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/dependencies_deps.py` & `smartpip2-2.1.9.4/airflow/ti_deps/dependencies_deps.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/dependencies_states.py` & `smartpip2-2.1.9.4/airflow/ti_deps/dependencies_states.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/__init__.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/base_ti_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/base_ti_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/dag_ti_slots_available_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_ti_slots_available_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/dag_unpaused_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/dag_unpaused_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/dagrun_exists_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_exists_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/dagrun_id_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/dagrun_id_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/exec_date_after_start_date_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/exec_date_after_start_date_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/not_in_retry_period_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/not_in_retry_period_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/not_previously_skipped_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/not_previously_skipped_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/pool_slots_available_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/pool_slots_available_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/prev_dagrun_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/prev_dagrun_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/ready_to_reschedule.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/ready_to_reschedule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/runnable_exec_date_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/runnable_exec_date_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/task_concurrency_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/task_concurrency_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/task_not_running_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/task_not_running_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/trigger_rule_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/trigger_rule_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/ti_deps/deps/valid_state_dep.py` & `smartpip2-2.1.9.4/airflow/ti_deps/deps/valid_state_dep.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/typing_compat.py` & `smartpip2-2.1.9.4/airflow/typing_compat.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/__init__.py` & `smartpip2-2.1.9.4/airflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/callback_requests.py` & `smartpip2-2.1.9.4/airflow/utils/callback_requests.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/cli.py` & `smartpip2-2.1.9.4/airflow/utils/cli.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/cli_action_loggers.py` & `smartpip2-2.1.9.4/airflow/utils/cli_action_loggers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/code_utils.py` & `smartpip2-2.1.9.4/airflow/utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/compression.py` & `smartpip2-2.1.9.4/airflow/utils/compression.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/configuration.py` & `smartpip2-2.1.9.4/airflow/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/dag_cycle_tester.py` & `smartpip2-2.1.9.4/airflow/utils/dag_cycle_tester.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/dag_processing.py` & `smartpip2-2.1.9.4/airflow/utils/dag_processing.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/dates.py` & `smartpip2-2.1.9.4/airflow/utils/dates.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/db.py` & `smartpip2-2.1.9.4/airflow/utils/db.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/decorators.py` & `smartpip2-2.1.9.4/airflow/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/docs.py` & `smartpip2-2.1.9.4/airflow/utils/docs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/dot_renderer.py` & `smartpip2-2.1.9.4/airflow/utils/dot_renderer.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/edgemodifier.py` & `smartpip2-2.1.9.4/airflow/utils/edgemodifier.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/email.py` & `smartpip2-2.1.9.4/airflow/utils/email.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/entry_points.py` & `smartpip2-2.1.9.4/airflow/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/event_scheduler.py` & `smartpip2-2.1.9.4/airflow/utils/event_scheduler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/file.py` & `smartpip2-2.1.9.4/airflow/utils/file.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/helpers.py` & `smartpip2-2.1.9.4/airflow/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/json.py` & `smartpip2-2.1.9.4/airflow/utils/json.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/__init__.py` & `smartpip2-2.1.9.4/airflow/utils/log/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/cloudwatch_task_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/colored_log.py` & `smartpip2-2.1.9.4/airflow/utils/log/colored_log.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/es_task_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/es_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/file_processor_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/file_processor_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/file_task_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/file_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/gcs_task_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/gcs_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/json_formatter.py` & `smartpip2-2.1.9.4/airflow/utils/log/json_formatter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/log_reader.py` & `smartpip2-2.1.9.4/airflow/utils/log/log_reader.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/logging_mixin.py` & `smartpip2-2.1.9.4/airflow/utils/log/logging_mixin.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/s3_task_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/secrets_masker.py` & `smartpip2-2.1.9.4/airflow/utils/log/secrets_masker.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/stackdriver_task_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/stackdriver_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/task_handler_with_custom_formatter.py` & `smartpip2-2.1.9.4/airflow/utils/log/task_handler_with_custom_formatter.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/log/wasb_task_handler.py` & `smartpip2-2.1.9.4/airflow/utils/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/mixins.py` & `smartpip2-2.1.9.4/airflow/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/module_loading.py` & `smartpip2-2.1.9.4/airflow/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/net.py` & `smartpip2-2.1.9.4/airflow/utils/net.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/operator_helpers.py` & `smartpip2-2.1.9.4/airflow/utils/operator_helpers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/operator_resources.py` & `smartpip2-2.1.9.4/airflow/utils/operator_resources.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/orm_event_handlers.py` & `smartpip2-2.1.9.4/airflow/utils/orm_event_handlers.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/platform.py` & `smartpip2-2.1.9.4/airflow/utils/platform.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/process_utils.py` & `smartpip2-2.1.9.4/airflow/utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/python_virtualenv.py` & `smartpip2-2.1.9.4/airflow/utils/python_virtualenv.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/python_virtualenv_script.jinja2` & `smartpip2-2.1.9.4/airflow/utils/python_virtualenv_script.jinja2`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/retries.py` & `smartpip2-2.1.9.4/airflow/utils/retries.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/serve_logs.py` & `smartpip2-2.1.9.4/airflow/utils/serve_logs.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/session.py` & `smartpip2-2.1.9.4/airflow/utils/session.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/sqlalchemy.py` & `smartpip2-2.1.9.4/airflow/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/state.py` & `smartpip2-2.1.9.4/airflow/utils/state.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/strings.py` & `smartpip2-2.1.9.4/airflow/utils/strings.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/task_group.py` & `smartpip2-2.1.9.4/airflow/utils/task_group.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/timeout.py` & `smartpip2-2.1.9.4/airflow/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/timezone.py` & `smartpip2-2.1.9.4/airflow/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/trigger_rule.py` & `smartpip2-2.1.9.4/airflow/utils/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/types.py` & `smartpip2-2.1.9.4/airflow/utils/types.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/weekday.py` & `smartpip2-2.1.9.4/airflow/utils/weekday.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/weight_rule.py` & `smartpip2-2.1.9.4/airflow/utils/weight_rule.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/utils/yaml.py` & `smartpip2-2.1.9.4/airflow/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/version.py` & `smartpip2-2.1.9.4/airflow/version.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/__init__.py` & `smartpip2-2.1.9.4/airflow/www/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/api/__init__.py` & `smartpip2-2.1.9.4/airflow/www/api/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/api/experimental/__init__.py` & `smartpip2-2.1.9.4/airflow/www/api/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/api/experimental/endpoints.py` & `smartpip2-2.1.9.4/airflow/www/api/experimental/endpoints.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/app.py` & `smartpip2-2.1.9.4/airflow/www/app.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/auth.py` & `smartpip2-2.1.9.4/airflow/www/auth.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/blueprints.py` & `smartpip2-2.1.9.4/airflow/www/blueprints.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/decorators.py` & `smartpip2-2.1.9.4/airflow/www/decorators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/__init__.py` & `smartpip2-2.1.9.4/airflow/www/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_appbuilder.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_appbuilder_links.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_appbuilder_links.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_dagbag.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_dagbag.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_jinja_globals.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_jinja_globals.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_manifest_files.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_manifest_files.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_security.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_session.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_session.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_views.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_views.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/extensions/init_wsgi_middlewares.py` & `smartpip2-2.1.9.4/airflow/www/extensions/init_wsgi_middlewares.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/forms.py` & `smartpip2-2.1.9.4/airflow/www/forms.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/gunicorn_config.py` & `smartpip2-2.1.9.4/airflow/www/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/package.json` & `smartpip2-2.1.9.4/airflow/www/package.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/security.py` & `smartpip2-2.1.9.4/airflow/www/security.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/airflow.gif` & `smartpip2-2.1.9.4/airflow/www/static/airflow.gif`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/bootstrap-theme.css` & `smartpip2-2.1.9.4/airflow/www/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/calendar.css` & `smartpip2-2.1.9.4/airflow/www/static/css/calendar.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/dags.css` & `smartpip2-2.1.9.4/airflow/www/static/css/dags.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/flash.css` & `smartpip2-2.1.9.4/airflow/www/static/css/flash.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/gantt.css` & `smartpip2-2.1.9.4/airflow/www/static/css/gantt.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/graph.css` & `smartpip2-2.1.9.4/airflow/www/static/css/graph.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/loading-dots.css` & `smartpip2-2.1.9.4/airflow/www/static/css/loading-dots.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/main.css` & `smartpip2-2.1.9.4/airflow/www/static/css/main.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/material-icons.css` & `smartpip2-2.1.9.4/airflow/www/static/css/material-icons.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/switch.css` & `smartpip2-2.1.9.4/airflow/www/static/css/switch.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/css/tree.css` & `smartpip2-2.1.9.4/airflow/www/static/css/tree.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/airflowDefaultTheme.3e8bda71892b61b62f94.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/bootstrap-datetimepicker.min.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/bootstrap-datetimepicker.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/bootstrap3-typeahead.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/bootstrap3-typeahead.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/calendar.1400e6f5f65b22dd3d08.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/circles.995e0afd45c3641109e1.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/circles.995e0afd45c3641109e1.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/codemirror.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/codemirror.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/codemirror.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/coffeescript-lint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/coffeescript-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/connectionForm.e30c847e053269c52938.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/css-lint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/css-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/d3-shape.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/d3-shape.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/d3-tip.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/d3-tip.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/d3.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/d3.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/dag.88a0e9c8a0b51b2bad12.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/dagCode.2b1f14a241f16585fc99.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/dagDependencies.db5ffa947165467509de.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.core.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.core.min.js.map` & `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.core.min.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dagre-d3.min.js.map` & `smartpip2-2.1.9.4/airflow/www/static/dist/dagre-d3.min.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/dags.6c090f6b27d152c78e7a.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dataTables.bootstrap.min.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/dataTables.bootstrap.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/durationChart.6e8ade581fc7ebf52426.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/flash.d205b61edc54ed448412.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/flash.d205b61edc54ed448412.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/flash.d205b61edc54ed448412.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/gantt.eba97492f3cf3617f94d.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/graph.02535ab8a01e52e293f7.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/html-lint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/html-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/ie.e458fc4544c628f16e02.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/ie.e458fc4544c628f16e02.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/javascript-lint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/javascript-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/javascript.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/javascript.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/jquery.dataTables.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/jshint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/jshint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/json-lint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/json-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/lint.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/lint.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/lint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/loadingDots.4033edd9abf2750d6f8f.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/main.e52cf607b64cdcd15089.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/main.e52cf607b64cdcd15089.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/main.e52cf607b64cdcd15089.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/manifest.json` & `smartpip2-2.1.9.4/airflow/www/static/dist/manifest.json`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/materialIcons.3221294eb511f43d1b15.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/moment.c1933ee062e9650051f7.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/moment.c1933ee062e9650051f7.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.css.map` & `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.css.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/nv.d3.min.js.map` & `smartpip2-2.1.9.4/airflow/www/static/dist/nv.d3.min.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/redoc.standalone.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt` & `smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/redoc.standalone.js.map` & `smartpip2-2.1.9.4/airflow/www/static/dist/redoc.standalone.js.map`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/sum.md5` & `smartpip2-2.1.9.4/airflow/www/static/dist/sum.md5`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/switch.e97750fdb7423f33656a.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/switch.e97750fdb7423f33656a.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/switch.e97750fdb7423f33656a.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/taskInstance.185ec68feadbd2e343c1.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/taskInstances.9cabc2e44536cc6f488c.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/tiLog.1313b3d5fffe1fcd0a7d.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/tree.412f55814f4c1710d907.css` & `smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.css`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/tree.412f55814f4c1710d907.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/tree.412f55814f4c1710d907.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/trigger.37bd384c75c1a26ba764.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/variableEdit.2e42bd9c63244a3c7a07.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/dist/yaml-lint.js` & `smartpip2-2.1.9.4/airflow/www/static/dist/yaml-lint.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/calendar.js` & `smartpip2-2.1.9.4/airflow/www/static/js/calendar.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/circles.js` & `smartpip2-2.1.9.4/airflow/www/static/js/circles.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/connection_form.js` & `smartpip2-2.1.9.4/airflow/www/static/js/connection_form.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/dag.js` & `smartpip2-2.1.9.4/airflow/www/static/js/dag.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/dag_code.js` & `smartpip2-2.1.9.4/airflow/www/static/js/dag_code.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/dag_dependencies.js` & `smartpip2-2.1.9.4/airflow/www/static/js/dag_dependencies.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/dags.js` & `smartpip2-2.1.9.4/airflow/www/static/js/dags.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/datetime_utils.js` & `smartpip2-2.1.9.4/airflow/www/static/js/datetime_utils.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/duration_chart.js` & `smartpip2-2.1.9.4/airflow/www/static/js/duration_chart.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/gantt.js` & `smartpip2-2.1.9.4/airflow/www/static/js/gantt.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/graph.js` & `smartpip2-2.1.9.4/airflow/www/static/js/graph.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/ie.js` & `smartpip2-2.1.9.4/airflow/www/static/js/ie.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/main.js` & `smartpip2-2.1.9.4/airflow/www/static/js/main.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/meta_value.js` & `smartpip2-2.1.9.4/airflow/www/static/js/meta_value.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/task_instance.js` & `smartpip2-2.1.9.4/airflow/www/static/js/task_instance.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/task_instances.js` & `smartpip2-2.1.9.4/airflow/www/static/js/task_instances.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/ti_log.js` & `smartpip2-2.1.9.4/airflow/www/static/js/ti_log.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/tree.js` & `smartpip2-2.1.9.4/airflow/www/static/js/tree.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/trigger.js` & `smartpip2-2.1.9.4/airflow/www/static/js/trigger.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/js/variable_edit.js` & `smartpip2-2.1.9.4/airflow/www/static/js/variable_edit.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/loading.gif` & `smartpip2-2.1.9.4/airflow/www/static/loading.gif`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/pin.svg` & `smartpip2-2.1.9.4/airflow/www/static/pin.svg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/pin_100.png` & `smartpip2-2.1.9.4/airflow/www/static/pin_100.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/pin_25.png` & `smartpip2-2.1.9.4/airflow/www/static/pin_25.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/pin_32.png` & `smartpip2-2.1.9.4/airflow/www/static/pin_32.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/pin_35.png` & `smartpip2-2.1.9.4/airflow/www/static/pin_35.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/pin_40.png` & `smartpip2-2.1.9.4/airflow/www/static/pin_40.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/pin_large.png` & `smartpip2-2.1.9.4/airflow/www/static/pin_large.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/screenshots/gantt.png` & `smartpip2-2.1.9.4/airflow/www/static/screenshots/gantt.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/screenshots/graph.png` & `smartpip2-2.1.9.4/airflow/www/static/screenshots/graph.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/static/screenshots/tree.png` & `smartpip2-2.1.9.4/airflow/www/static/screenshots/tree.png`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/calendar.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/calendar.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/chart.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/chart.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/circles.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/circles.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/code.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/code.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/config.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/config.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/confirm.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/confirm.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/conn_create.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_create.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/conn_edit.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/conn_edit.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/dag.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/dag_code.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_code.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/dag_dependencies.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_dependencies.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/dag_details.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/dag_details.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/dags.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/dags.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/duration_chart.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/duration_chart.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/gantt.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/gantt.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/graph.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/graph.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/main.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/main.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/model_list.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/model_list.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/noaccess.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/noaccess.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/plugin.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/plugin.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/redoc.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/redoc.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/task.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/task.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/task_instance.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/task_instance.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/ti_code.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_code.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/ti_log.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/ti_log.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/traceback.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/traceback.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/tree.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/tree.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/trigger.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/trigger.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/variable_edit.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_edit.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/variable_list.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/variable_list.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/airflow/xcom.html` & `smartpip2-2.1.9.4/airflow/www/templates/airflow/xcom.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/analytics/google_analytics.html` & `smartpip2-2.1.9.4/airflow/www/templates/analytics/google_analytics.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/analytics/metarouter.html` & `smartpip2-2.1.9.4/airflow/www/templates/analytics/metarouter.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/analytics/segment.html` & `smartpip2-2.1.9.4/airflow/www/templates/analytics/segment.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/custom_icons.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/custom_icons.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/dag_docs.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/dag_docs.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/flash.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/flash.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/index.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/index.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/loading_dots.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/loading_dots.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/navbar.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/navbar_menu.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_menu.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/templates/appbuilder/navbar_right.html` & `smartpip2-2.1.9.4/airflow/www/templates/appbuilder/navbar_right.html`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/utils.py` & `smartpip2-2.1.9.4/airflow/www/utils.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/validators.py` & `smartpip2-2.1.9.4/airflow/www/validators.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/views.py` & `smartpip2-2.1.9.4/airflow/www/views.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/webpack.config.js` & `smartpip2-2.1.9.4/airflow/www/webpack.config.js`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/airflow/www/widgets.py` & `smartpip2-2.1.9.4/airflow/www/widgets.py`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-bootstrap.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-bootstrap.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-bootstrap3-typeahead.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-bootstrap3-typeahead.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-connexion.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-connexion.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-d3-shape.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-d3-shape.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-d3-tip.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-d3-tip.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-d3js.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-d3js.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-dagre-d3.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-dagre-d3.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-datatables.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-datatables.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-elasticmock.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-elasticmock.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-eonasdan-bootstrap-datetimepicker.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-flask-kerberos.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-flask-kerberos.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-hue.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-hue.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-jqclock.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-jqclock.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-jquery.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-jquery.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-moment-strftime.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-moment-strftime.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-moment.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-moment.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/licenses/LICENSE-normalize.txt` & `smartpip2-2.1.9.4/licenses/LICENSE-normalize.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/README` & `smartpip2-2.1.9.4/scripts/systemd/README`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/airflow` & `smartpip2-2.1.9.4/scripts/systemd/airflow`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/airflow-flower.service` & `smartpip2-2.1.9.4/scripts/systemd/airflow-flower.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/airflow-kerberos.service` & `smartpip2-2.1.9.4/scripts/systemd/airflow-kerberos.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/airflow-scheduler.service` & `smartpip2-2.1.9.4/scripts/systemd/airflow-scheduler.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/airflow-webserver.service` & `smartpip2-2.1.9.4/scripts/systemd/airflow-webserver.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/airflow-worker.service` & `smartpip2-2.1.9.4/scripts/systemd/airflow-worker.service`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/scripts/systemd/airflow.conf` & `smartpip2-2.1.9.4/scripts/systemd/airflow.conf`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/setup.cfg` & `smartpip2-2.1.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/setup.py` & `smartpip2-2.1.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # And it is particularly useful when you add a new provider and there is no
 # PyPI version to install the provider package from
 INSTALL_PROVIDERS_FROM_SOURCES = 'INSTALL_PROVIDERS_FROM_SOURCES'
 PY39 = sys.version_info >= (3, 9)
 
 logger = logging.getLogger(__name__)
 
-version = '2.1.9.3'
+version = '2.1.9.4'
 
 my_dir = dirname(__file__)
 
 
 def airflow_test_suite() -> unittest.TestSuite:
     """Test suite for Airflow tests"""
     test_loader = unittest.TestLoader()
```

### Comparing `smartpip2-2.1.9.3/smartpip2.egg-info/PKG-INFO` & `smartpip2-2.1.9.4/smartpip2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: smartpip2
-Version: 2.1.9.3
+Version: 2.1.9.4
 Summary: Programmatically author, schedule and monitor data pipelines
 Home-page: https://www.smartchart.cn/
 Author: Apache Software Foundation
 Author-email: 84345999@qq.com
 License: Apache License 2.0
-Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.3
+Download-URL: https://www.smartchart.cn/dist/airflow/2.1.9.4
 Project-URL: Documentation, https://airflow.apache.org/docs/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Description: <!--
          Licensed to the Apache Software Foundation (ASF) under one
          or more contributor license agreements.  See the NOTICE file
          distributed with this work for additional information
@@ -357,116 +357,116 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: apache.webhdfs
-Provides-Extra: apache.hive
 Provides-Extra: jdbc
-Provides-Extra: openfaas
-Provides-Extra: segment
-Provides-Extra: apache.pinot
-Provides-Extra: trino
-Provides-Extra: ftp
-Provides-Extra: samba
-Provides-Extra: grpc
-Provides-Extra: sentry
-Provides-Extra: mongo
-Provides-Extra: celery
-Provides-Extra: tableau
-Provides-Extra: virtualenv
-Provides-Extra: jenkins
-Provides-Extra: presto
-Provides-Extra: pagerduty
-Provides-Extra: zendesk
-Provides-Extra: devel
-Provides-Extra: salesforce
+Provides-Extra: statsd
+Provides-Extra: s3
+Provides-Extra: async
+Provides-Extra: cgroups
+Provides-Extra: all
 Provides-Extra: rabbitmq
-Provides-Extra: apache.drill
-Provides-Extra: cloudant
-Provides-Extra: spark
-Provides-Extra: vertica
-Provides-Extra: mssql
-Provides-Extra: devel_ci
+Provides-Extra: docker
 Provides-Extra: microsoft.winrm
-Provides-Extra: pinot
-Provides-Extra: leveldb
-Provides-Extra: password
+Provides-Extra: pagerduty
+Provides-Extra: druid
+Provides-Extra: snowflake
+Provides-Extra: plexus
+Provides-Extra: discord
+Provides-Extra: slack
+Provides-Extra: apache.livy
+Provides-Extra: celery
+Provides-Extra: databricks
+Provides-Extra: devel
+Provides-Extra: webhdfs
+Provides-Extra: kerberos
 Provides-Extra: jira
+Provides-Extra: devel_hadoop
 Provides-Extra: cncf.kubernetes
-Provides-Extra: singularity
-Provides-Extra: ssh
-Provides-Extra: docker
+Provides-Extra: crypto
+Provides-Extra: microsoft.azure
+Provides-Extra: spark
+Provides-Extra: tableau
+Provides-Extra: cloudant
+Provides-Extra: google
+Provides-Extra: apache.hive
+Provides-Extra: mongo
+Provides-Extra: deprecated_api
+Provides-Extra: openfaas
+Provides-Extra: hdfs
+Provides-Extra: hive
+Provides-Extra: amazon
 Provides-Extra: ldap
-Provides-Extra: papermill
-Provides-Extra: postgres
+Provides-Extra: presto
+Provides-Extra: qubole
+Provides-Extra: telegram
+Provides-Extra: airbyte
+Provides-Extra: gcp_api
+Provides-Extra: ftp
+Provides-Extra: pinot
+Provides-Extra: mysql
+Provides-Extra: odbc
+Provides-Extra: salesforce
+Provides-Extra: neo4j
+Provides-Extra: dingding
+Provides-Extra: devel_ci
 Provides-Extra: apache.atlas
-Provides-Extra: async
-Provides-Extra: snowflake
-Provides-Extra: opsgenie
-Provides-Extra: microsoft.azure
+Provides-Extra: hashicorp
+Provides-Extra: apache.hdfs
+Provides-Extra: mssql
+Provides-Extra: yandex
+Provides-Extra: dask
+Provides-Extra: samba
+Provides-Extra: gcp
+Provides-Extra: imap
+Provides-Extra: jenkins
+Provides-Extra: virtualenv
+Provides-Extra: github_enterprise
+Provides-Extra: segment
+Provides-Extra: devel_all
+Provides-Extra: apache.drill
+Provides-Extra: singularity
 Provides-Extra: aws
+Provides-Extra: postgres
+Provides-Extra: papermill
+Provides-Extra: sendgrid
 Provides-Extra: apache.kylin
-Provides-Extra: qubole
-Provides-Extra: qds
-Provides-Extra: apache.livy
-Provides-Extra: mysql
-Provides-Extra: devel_hadoop
-Provides-Extra: sqlite
-Provides-Extra: apache.beam
-Provides-Extra: apache.druid
+Provides-Extra: opsgenie
+Provides-Extra: asana
+Provides-Extra: oracle
+Provides-Extra: apache.pinot
 Provides-Extra: exasol
-Provides-Extra: all
-Provides-Extra: webhdfs
-Provides-Extra: statsd
+Provides-Extra: apache.cassandra
+Provides-Extra: doc
+Provides-Extra: microsoft.mssql
 Provides-Extra: atlas
+Provides-Extra: kubernetes
+Provides-Extra: apache.beam
+Provides-Extra: elasticsearch
+Provides-Extra: redis
+Provides-Extra: vertica
+Provides-Extra: google_auth
+Provides-Extra: sentry
+Provides-Extra: zendesk
+Provides-Extra: apache.sqoop
+Provides-Extra: http
+Provides-Extra: leveldb
 Provides-Extra: apache.pig
-Provides-Extra: hashicorp
-Provides-Extra: sendgrid
 Provides-Extra: facebook
-Provides-Extra: crypto
-Provides-Extra: azure
-Provides-Extra: slack
-Provides-Extra: apache.hdfs
-Provides-Extra: imap
-Provides-Extra: hive
-Provides-Extra: google_auth
+Provides-Extra: apache.webhdfs
+Provides-Extra: apache.druid
+Provides-Extra: trino
+Provides-Extra: all_dbs
 Provides-Extra: sftp
-Provides-Extra: doc
-Provides-Extra: apache.cassandra
-Provides-Extra: dingding
-Provides-Extra: gcp_api
-Provides-Extra: cassandra
-Provides-Extra: hdfs
 Provides-Extra: winrm
-Provides-Extra: devel_all
-Provides-Extra: gcp
-Provides-Extra: redis
+Provides-Extra: azure
+Provides-Extra: grpc
+Provides-Extra: sqlite
+Provides-Extra: password
 Provides-Extra: apache.spark
-Provides-Extra: odbc
-Provides-Extra: all_dbs
-Provides-Extra: telegram
-Provides-Extra: oracle
-Provides-Extra: dask
-Provides-Extra: neo4j
-Provides-Extra: asana
-Provides-Extra: amazon
-Provides-Extra: apache.sqoop
-Provides-Extra: druid
-Provides-Extra: elasticsearch
-Provides-Extra: s3
-Provides-Extra: cgroups
-Provides-Extra: kubernetes
-Provides-Extra: databricks
-Provides-Extra: deprecated_api
-Provides-Extra: plexus
-Provides-Extra: discord
-Provides-Extra: github_enterprise
-Provides-Extra: google
-Provides-Extra: microsoft.mssql
+Provides-Extra: cassandra
+Provides-Extra: qds
 Provides-Extra: datadog
-Provides-Extra: yandex
-Provides-Extra: kerberos
-Provides-Extra: airbyte
-Provides-Extra: http
+Provides-Extra: ssh
```

### Comparing `smartpip2-2.1.9.3/smartpip2.egg-info/SOURCES.txt` & `smartpip2-2.1.9.4/smartpip2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartpip2-2.1.9.3/smartpip2.egg-info/requires.txt` & `smartpip2-2.1.9.4/smartpip2.egg-info/requires.txt`

 * *Files identical despite different names*

