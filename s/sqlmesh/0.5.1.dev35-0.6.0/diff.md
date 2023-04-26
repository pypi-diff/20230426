# Comparing `tmp/sqlmesh-0.5.1.dev35.tar.gz` & `tmp/sqlmesh-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.5.1.dev35.tar", last modified: Tue Apr 25 23:11:16 2023, max compression
+gzip compressed data, was "sqlmesh-0.6.0.tar", last modified: Wed Apr 26 17:24:35 2023, max compression
```

## Comparing `sqlmesh-0.5.1.dev35.tar` & `sqlmesh-0.6.0.tar`

### file list

```diff
@@ -1,734 +1,751 @@
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.050864 sqlmesh-0.5.1.dev35/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.950943 sqlmesh-0.5.1.dev35/.circleci/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1872 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/.circleci/config.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)     4414 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/.circleci/continue_config.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       66 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/.dockerignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     2152 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     1900 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/.pre-commit-config.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      234 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev35/.readthedocs.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      135 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev35/Dockerfile.api
--rw-r--r--   0 izeigerman   (501) staff       (20)      383 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/Dockerfile.app
--rw-r--r--   0 izeigerman   (501) staff       (20)    11346 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/LICENSE
--rw-r--r--   0 izeigerman   (501) staff       (20)     1855 2023-04-25 20:51:56.000000 sqlmesh-0.5.1.dev35/Makefile
--rw-r--r--   0 izeigerman   (501) staff       (20)     2037 2023-04-25 23:11:16.050962 sqlmesh-0.5.1.dev35/PKG-INFO
--rw-r--r--   0 izeigerman   (501) staff       (20)     1250 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/README.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1008 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/docker-compose.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.953289 sqlmesh-0.5.1.dev35/docs/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.935535 sqlmesh-0.5.1.dev35/docs/_readthedocs/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.953555 sqlmesh-0.5.1.dev35/docs/_readthedocs/html/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev35/docs/_readthedocs/html/.keep
--rw-r--r--   0 izeigerman   (501) staff       (20)     9965 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/comparisons.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.955154 sqlmesh-0.5.1.dev35/docs/concepts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.955660 sqlmesh-0.5.1.dev35/docs/concepts/architecture/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1334 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/architecture/serialization.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1113 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     6689 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/concepts/audits.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/environments.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5952 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/concepts/glossary.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       13 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/hooks.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     3027 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/macros.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.956479 sqlmesh-0.5.1.dev35/docs/concepts/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     9934 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/docs/concepts/models/model_kinds.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7859 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev35/docs/concepts/models/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/models/python_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     4938 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/models/seed_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5356 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/concepts/models/sql_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     6637 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/concepts/overview.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.956638 sqlmesh-0.5.1.dev35/docs/concepts/plans/
--rw-r--r--   0 izeigerman   (501) staff       (20)    43124 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 izeigerman   (501) staff       (20)     8973 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/concepts/plans.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5699 2023-02-27 20:36:43.000000 sqlmesh-0.5.1.dev35/docs/concepts/tests.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      607 2023-04-09 02:39:18.000000 sqlmesh-0.5.1.dev35/docs/development.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.958444 sqlmesh-0.5.1.dev35/docs/guides/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1943 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/docs/guides/connections.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1309 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/guides/migrations.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    10756 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/docs/guides/models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     6133 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/docs/guides/multi_repo.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     2142 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/guides/projects.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.959928 sqlmesh-0.5.1.dev35/docs/guides/scheduling/
--rw-r--r--   0 izeigerman   (501) staff       (20)   740917 2023-02-24 17:54:11.000000 sqlmesh-0.5.1.dev35/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   379880 2023-02-24 17:54:11.000000 sqlmesh-0.5.1.dev35/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 izeigerman   (501) staff       (20)     5648 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/guides/scheduling.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1854 2023-02-27 20:36:43.000000 sqlmesh-0.5.1.dev35/docs/guides/testing.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5517 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/index.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      297 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/installation.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.962358 sqlmesh-0.5.1.dev35/docs/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2905 2023-04-03 17:47:07.000000 sqlmesh-0.5.1.dev35/docs/integrations/airflow.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7801 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/docs/integrations/dbt.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    24125 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev35/docs/integrations/engines.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      925 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/integrations/github.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      217 2023-03-25 06:07:32.000000 sqlmesh-0.5.1.dev35/docs/integrations/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      665 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev35/docs/prerequisites.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    10781 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/docs/quick_start.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.963822 sqlmesh-0.5.1.dev35/docs/reference/
--rw-r--r--   0 izeigerman   (501) staff       (20)     6093 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/docs/reference/cli.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    13607 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev35/docs/reference/configuration.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     4579 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/docs/reference/notebook.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1127 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/reference/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       14 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/reference/python.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       16 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/docs/release_notes.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      122 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev35/docs/requirements.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)     3249 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/docs/sqlmesh.png
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.964059 sqlmesh-0.5.1.dev35/examples/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.965290 sqlmesh-0.5.1.dev35/examples/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1713 2023-04-09 02:39:12.000000 sqlmesh-0.5.1.dev35/examples/airflow/Dockerfile.template
--rw-r--r--   0 izeigerman   (501) staff       (20)     2164 2023-04-09 02:39:18.000000 sqlmesh-0.5.1.dev35/examples/airflow/Makefile
--rw-r--r--   0 izeigerman   (501) staff       (20)      942 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev35/examples/airflow/README.md
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.5.1.dev35/examples/airflow/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.965542 sqlmesh-0.5.1.dev35/examples/airflow/dags/
--rw-r--r--   0 izeigerman   (501) staff       (20)      263 2023-03-09 17:15:39.000000 sqlmesh-0.5.1.dev35/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3515 2023-04-09 02:39:12.000000 sqlmesh-0.5.1.dev35/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev35/examples/airflow/requirements.txt
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.965860 sqlmesh-0.5.1.dev35/examples/airflow/spark_conf/
--rw-r--r--   0 izeigerman   (501) staff       (20)      872 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev35/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 izeigerman   (501) staff       (20)      151 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev35/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.936830 sqlmesh-0.5.1.dev35/examples/multi/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.966040 sqlmesh-0.5.1.dev35/examples/multi/repo_1/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.966178 sqlmesh-0.5.1.dev35/examples/multi/repo_1/audits/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/audits/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      108 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/config.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.966380 sqlmesh-0.5.1.dev35/examples/multi/repo_1/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/macros/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/macros/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.966916 sqlmesh-0.5.1.dev35/examples/multi/repo_1/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/models/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)       63 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/models/a.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       53 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/models/b.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.967169 sqlmesh-0.5.1.dev35/examples/multi/repo_1/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_1/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.967292 sqlmesh-0.5.1.dev35/examples/multi/repo_2/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.967444 sqlmesh-0.5.1.dev35/examples/multi/repo_2/audits/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/audits/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      113 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/config.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.967692 sqlmesh-0.5.1.dev35/examples/multi/repo_2/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/macros/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/macros/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.968084 sqlmesh-0.5.1.dev35/examples/multi/repo_2/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/models/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)       64 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/models/c.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       53 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/models/d.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.968283 sqlmesh-0.5.1.dev35/examples/multi/repo_2/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/examples/multi/repo_2/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.968660 sqlmesh-0.5.1.dev35/examples/sushi/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.968953 sqlmesh-0.5.1.dev35/examples/sushi/audits/
--rw-r--r--   0 izeigerman   (501) staff       (20)      105 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/audits/items.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      119 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/audits/order_items.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      829 2023-04-21 21:07:50.000000 sqlmesh-0.5.1.dev35/examples/sushi/config.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.969080 sqlmesh-0.5.1.dev35/examples/sushi/data/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-24 21:30:36.000000 sqlmesh-0.5.1.dev35/examples/sushi/data/.keep
--rw-r--r--   0 izeigerman   (501) staff       (20)      551 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/helper.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.969287 sqlmesh-0.5.1.dev35/examples/sushi/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/hooks/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.969511 sqlmesh-0.5.1.dev35/examples/sushi/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/macros/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      702 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/macros/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.971722 sqlmesh-0.5.1.dev35/examples/sushi/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)      916 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      204 2023-03-03 17:17:44.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     1910 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/items.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1911 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/order_items.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1642 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/orders.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      346 2023-03-25 04:59:10.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      465 2023-04-24 18:34:50.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      123 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      691 2023-04-24 21:41:10.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      197 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.972017 sqlmesh-0.5.1.dev35/examples/sushi/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-03-24 20:49:46.000000 sqlmesh-0.5.1.dev35/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.972174 sqlmesh-0.5.1.dev35/examples/sushi/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1459 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev35/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.973287 sqlmesh-0.5.1.dev35/examples/sushi_dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)       15 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/.user.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.973420 sqlmesh-0.5.1.dev35/examples/sushi_dbt/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-14 18:30:53.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      507 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.973676 sqlmesh-0.5.1.dev35/examples/sushi_dbt/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-03-03 23:53:25.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-02-28 16:05:24.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.974733 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1125 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      182 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      309 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-01-31 01:13:15.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      752 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      186 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.938143 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.974892 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.975246 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.975674 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.975845 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.975981 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.976130 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.976275 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      783 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.977045 sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)       97 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-01-31 01:13:15.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.977232 sqlmesh-0.5.1.dev35/examples/sushi_dbt/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.977343 sqlmesh-0.5.1.dev35/examples/sushi_dbt/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev35/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.977546 sqlmesh-0.5.1.dev35/examples/wursthall/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.938930 sqlmesh-0.5.1.dev35/examples/wursthall/audits/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.977836 sqlmesh-0.5.1.dev35/examples/wursthall/audits/db/
--rw-r--r--   0 izeigerman   (501) staff       (20)      141 2023-01-31 01:13:15.000000 sqlmesh-0.5.1.dev35/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       66 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/config.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.978296 sqlmesh-0.5.1.dev35/examples/wursthall/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/macros/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      618 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.978466 sqlmesh-0.5.1.dev35/examples/wursthall/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.979457 sqlmesh-0.5.1.dev35/examples/wursthall/models/db/
--rw-r--r--   0 izeigerman   (501) staff       (20)      433 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      256 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     3161 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      542 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.980430 sqlmesh-0.5.1.dev35/examples/wursthall/models/src/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1672 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      120 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     3434 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      892 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.939314 sqlmesh-0.5.1.dev35/examples/wursthall/seeds/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.980598 sqlmesh-0.5.1.dev35/examples/wursthall/seeds/src/
--rw-r--r--   0 izeigerman   (501) staff       (20)     7416 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev35/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.981383 sqlmesh-0.5.1.dev35/examples/wursthall/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-02-20 22:54:27.000000 sqlmesh-0.5.1.dev35/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      955 2023-02-20 22:54:27.000000 sqlmesh-0.5.1.dev35/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)     2113 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/mkdocs.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.981615 sqlmesh-0.5.1.dev35/pdoc/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)     1153 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev35/pdoc/cli.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.981880 sqlmesh-0.5.1.dev35/pdoc/templates/
--rw-r--r--   0 izeigerman   (501) staff       (20)      131 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.982159 sqlmesh-0.5.1.dev35/posts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.985555 sqlmesh-0.5.1.dev35/posts/virtual_data_environments/
--rw-r--r--   0 izeigerman   (501) staff       (20)   318753 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/posts/virtual_data_environments/change_categorization.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   274526 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/posts/virtual_data_environments/isolated_rigid_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   163619 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/posts/virtual_data_environments/partial_breaking.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   298971 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/posts/virtual_data_environments/stateful_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   366545 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/posts/virtual_data_environments/virtual_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)  1344487 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/posts/virtual_data_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 izeigerman   (501) staff       (20)    18696 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/posts/virtual_data_environments.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      734 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/pytest.ini
--rw-r--r--   0 izeigerman   (501) staff       (20)     1393 2023-04-25 23:11:16.051526 sqlmesh-0.5.1.dev35/setup.cfg
--rw-r--r--   0 izeigerman   (501) staff       (20)     3158 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/setup.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.987817 sqlmesh-0.5.1.dev35/sqlmesh/
--rw-r--r--   0 izeigerman   (501) staff       (20)        3 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/.airflowignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     3950 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev35/sqlmesh/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      175 2023-04-25 23:11:15.000000 sqlmesh-0.5.1.dev35/sqlmesh/_version.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.988995 sqlmesh-0.5.1.dev35/sqlmesh/cli/
--rw-r--r--   0 izeigerman   (501) staff       (20)      898 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev35/sqlmesh/cli/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4314 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/cli/example_project.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9641 2023-04-23 13:55:51.000000 sqlmesh-0.5.1.dev35/sqlmesh/cli/main.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1433 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/sqlmesh/cli/options.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.991434 sqlmesh-0.5.1.dev35/sqlmesh/core/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      586 2023-01-20 19:19:17.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/_typing.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.992063 sqlmesh-0.5.1.dev35/sqlmesh/core/audit/
--rw-r--r--   0 izeigerman   (501) staff       (20)      449 2023-01-27 03:51:22.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1071 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8136 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.993730 sqlmesh-0.5.1.dev35/sqlmesh/core/config/
--rw-r--r--   0 izeigerman   (501) staff       (20)      668 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1001 2023-02-22 17:05:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      940 2023-02-08 20:28:46.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    21184 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/connection.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3351 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1655 2023-02-08 20:28:46.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5611 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/root.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8421 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    29390 2023-04-25 23:02:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/console.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      735 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/constants.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    36030 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8849 2023-04-25 21:37:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/context_diff.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    17626 2023-03-24 20:30:06.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/dialect.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.995720 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2626 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      762 2023-01-18 00:01:51.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    29021 2023-04-22 00:09:12.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4191 2023-04-22 00:43:39.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/base_postgres.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4238 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15694 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      402 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1939 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1971 2023-03-01 20:53:43.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2149 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6650 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1181 2023-03-01 20:53:43.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2658 2023-03-01 00:12:50.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4131 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1815 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/environment.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      742 2023-02-09 01:00:20.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/hooks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12521 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18920 2023-03-24 20:30:06.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.996782 sqlmesh-0.5.1.dev35/sqlmesh/core/model/
--rw-r--r--   0 izeigerman   (501) staff       (20)      594 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1746 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/cache.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1300 2023-04-18 21:05:17.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2417 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/decorator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    47685 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8168 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/kind.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13034 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/meta.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2017 2023-03-15 19:25:00.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/model/seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2314 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.997173 sqlmesh-0.5.1.dev35/sqlmesh/core/plan/
--rw-r--r--   0 izeigerman   (501) staff       (20)      191 2022-12-27 15:59:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    22476 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/plan/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8075 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12623 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/renderer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15386 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    20418 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.997666 sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/
--rw-r--r--   0 izeigerman   (501) staff       (20)      527 2023-02-13 20:33:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    33750 2023-04-25 23:01:42.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    19248 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.998195 sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/
--rw-r--r--   0 izeigerman   (501) staff       (20)      692 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13080 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12222 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    20698 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10834 2023-04-19 16:43:48.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/test.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1412 2022-12-24 00:00:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/core/user.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.000782 sqlmesh-0.5.1.dev35/sqlmesh/dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)       79 2023-03-13 19:40:14.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    16407 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    11231 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/builtin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1762 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/column.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4771 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5087 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8044 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9807 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13257 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/package.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3701 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/profile.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4772 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/project.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      928 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3137 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/source.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13503 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/target.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-02 18:36:40.000000 sqlmesh-0.5.1.dev35/sqlmesh/dbt/util.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.001037 sqlmesh-0.5.1.dev35/sqlmesh/engines/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/engines/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4437 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/engines/commands.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.001295 sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3414 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.001708 sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      148 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2571 2023-02-14 21:38:26.000000 sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.002017 sqlmesh-0.5.1.dev35/sqlmesh/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.002670 sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2210 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1726 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1829 2023-01-18 20:54:37.000000 sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13754 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev35/sqlmesh/magics.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.003253 sqlmesh-0.5.1.dev35/sqlmesh/migrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/migrations/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1749 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      103 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/migrations/v0002_remove_identify.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1183 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/sqlmesh/migrations/v0003_move_batch_size.py
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/py.typed
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.003390 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.004657 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-04 00:12:26.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4020 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3830 2023-03-09 17:15:48.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18799 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.005042 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-16 21:08:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2132 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      868 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8508 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.006396 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1444 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6307 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2549 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      877 2023-01-31 17:31:24.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1322 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/postgres.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1211 2023-01-20 19:19:17.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1340 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5222 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    11104 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4400 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1292 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4139 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5213 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.008707 sqlmesh-0.5.1.dev35/sqlmesh/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4378 2023-04-21 19:57:49.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3593 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/cache.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/concurrency.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7530 2023-02-14 22:10:01.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      410 2022-12-30 16:25:50.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/conversions.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4329 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/dag.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7549 2023-04-18 02:34:51.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/date.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1244 2023-02-04 22:32:08.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/errors.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    16084 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/jinja.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15093 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-03-07 23:18:33.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/pandas.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1609 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/pydantic.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1534 2023-01-25 18:09:57.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/rich.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6487 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1419 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.988535 sqlmesh-0.5.1.dev35/sqlmesh.egg-info/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2037 2023-04-25 23:11:15.000000 sqlmesh-0.5.1.dev35/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 izeigerman   (501) staff       (20)    21315 2023-04-25 23:11:15.000000 sqlmesh-0.5.1.dev35/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)        1 2023-04-25 23:11:15.000000 sqlmesh-0.5.1.dev35/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)      142 2023-04-25 23:11:15.000000 sqlmesh-0.5.1.dev35/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)      838 2023-04-25 23:11:15.000000 sqlmesh-0.5.1.dev35/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-04-25 23:11:15.000000 sqlmesh-0.5.1.dev35/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)    21020 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/sqlmesh.svg
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.009128 sqlmesh-0.5.1.dev35/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      285 2023-02-07 17:58:48.000000 sqlmesh-0.5.1.dev35/tests/common_fixtures.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3741 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/tests/conftest.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.012172 sqlmesh-0.5.1.dev35/tests/core/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/core/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.013747 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    27881 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2114 2023-04-22 00:43:39.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_base_postgres.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1270 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-07 23:18:33.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1253 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2613 2023-02-14 20:17:36.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1569 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_postgres.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8036 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3191 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7073 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/tests/core/test_audit.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6611 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/tests/core/test_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      850 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/core/test_connection_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10197 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/tests/core/test_context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2749 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev35/tests/core/test_dialect.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      464 2022-12-28 17:42:44.000000 sqlmesh-0.5.1.dev35/tests/core/test_environment.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    26685 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/core/test_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5880 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/tests/core/test_macros.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    25301 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev35/tests/core/test_model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15741 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/core/test_plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3862 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/core/test_plan_evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4647 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/core/test_scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    32235 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/core/test_schema_diff.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      857 2023-01-06 17:16:27.000000 sqlmesh-0.5.1.dev35/tests/core/test_seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    28498 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/core/test_snapshot.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10299 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    22681 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/core/test_state_sync.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.014366 sqlmesh-0.5.1.dev35/tests/dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-16 16:43:18.000000 sqlmesh-0.5.1.dev35/tests/dbt/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      636 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/tests/dbt/conftest.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2537 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/tests/dbt/test_adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13195 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/tests/dbt/test_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    17098 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev35/tests/dbt/test_transformation.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.014511 sqlmesh-0.5.1.dev35/tests/engines/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/engines/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.014852 sqlmesh-0.5.1.dev35/tests/engines/spark/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/engines/spark/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      357 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/engines/spark/conftest.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1503 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.943414 sqlmesh-0.5.1.dev35/tests/fixtures/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.942143 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.015904 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.016043 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.942278 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1055 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.016174 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 izeigerman   (501) staff       (20)    10264 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.016439 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.017112 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      334 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      863 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      196 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.942652 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.017240 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.017367 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.017613 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.017990 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1155 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      108 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      193 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.018118 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.018248 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.018389 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      540 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)     1250 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.018633 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)       42 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.018788 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.019189 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.019338 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.019602 sqlmesh-0.5.1.dev35/tests/fixtures/migrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)     9823 2023-04-24 22:27:34.000000 sqlmesh-0.5.1.dev35/tests/fixtures/migrations/environments.json
--rw-r--r--   0 izeigerman   (501) staff       (20)    25229 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev35/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.019755 sqlmesh-0.5.1.dev35/tests/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/integrations/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.019965 sqlmesh-0.5.1.dev35/tests/integrations/github/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/integrations/github/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.020094 sqlmesh-0.5.1.dev35/tests/integrations/github/fixtures/
--rw-r--r--   0 izeigerman   (501) staff       (20)      816 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 izeigerman   (501) staff       (20)      477 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.020388 sqlmesh-0.5.1.dev35/tests/schedulers/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/schedulers/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.021253 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1414 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.021751 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/operators/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4442 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4392 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9857 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1345 2023-04-21 23:58:46.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6092 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5944 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.023467 sqlmesh-0.5.1.dev35/tests/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/utils/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1118 2023-04-24 13:57:39.000000 sqlmesh-0.5.1.dev35/tests/utils/test_cache.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3580 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/tests/utils/test_concurrency.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6430 2023-02-14 21:38:26.000000 sqlmesh-0.5.1.dev35/tests/utils/test_connection_pool.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1381 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev35/tests/utils/test_dag.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1818 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/utils/test_date.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      551 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/utils/test_filesystem.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5516 2023-03-07 20:10:54.000000 sqlmesh-0.5.1.dev35/tests/utils/test_jinja.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5790 2023-03-03 23:53:25.000000 sqlmesh-0.5.1.dev35/tests/utils/test_metaprogramming.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2501 2023-03-07 23:18:33.000000 sqlmesh-0.5.1.dev35/tests/utils/test_pandas.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      518 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev35/tests/utils/test_pydantic.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2911 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/tests/utils/test_transactional_file.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1194 2023-03-13 19:40:14.000000 sqlmesh-0.5.1.dev35/tests/utils/test_yaml.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.023695 sqlmesh-0.5.1.dev35/tests/web/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev35/tests/web/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    16198 2023-04-25 21:35:53.000000 sqlmesh-0.5.1.dev35/tests/web/test_main.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.023830 sqlmesh-0.5.1.dev35/web/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev35/web/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.025839 sqlmesh-0.5.1.dev35/web/client/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1104 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/.eslintrc.js
--rw-r--r--   0 izeigerman   (501) staff       (20)       94 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)      129 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/.prettierignore
--rw-r--r--   0 izeigerman   (501) staff       (20)      403 2023-02-14 21:38:26.000000 sqlmesh-0.5.1.dev35/web/client/.prettierrc.js
--rw-r--r--   0 izeigerman   (501) staff       (20)     1076 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/web/client/index.html
--rw-r--r--   0 izeigerman   (501) staff       (20)    37689 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/openapi.json
--rw-r--r--   0 izeigerman   (501) staff       (20)      330 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/orval.config.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)   408504 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev35/web/client/package-lock.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     2389 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/package.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     1642 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/web/client/playwright.config.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)       82 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev35/web/client/postcss.config.js
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.944175 sqlmesh-0.5.1.dev35/web/client/public/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.025967 sqlmesh-0.5.1.dev35/web/client/public/favicons/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2473 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.026471 sqlmesh-0.5.1.dev35/web/client/src/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.026848 sqlmesh-0.5.1.dev35/web/client/src/api/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1236 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/api/channels.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5243 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/api/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3247 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/api/instance.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.944438 sqlmesh-0.5.1.dev35/web/client/src/assets/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.944554 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.029781 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74500 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74524 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74368 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    73964 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    68940 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    67284 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74116 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    73916 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.036028 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    55004 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56384 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57104 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    62320 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56652 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    61688 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57680 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    53148 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57060 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56836 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    61460 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    52820 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    59176 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    63876 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    60768 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    81732 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    60992 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    64792 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.037090 sqlmesh-0.5.1.dev35/web/client/src/context/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4126 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/context/context.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5719 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/context/editor.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      923 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/context/fileTree.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1129 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/context/lineage.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     2661 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/context/plan.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1562 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/context/theme.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.037383 sqlmesh-0.5.1.dev35/web/client/src/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)      308 2023-03-02 00:19:27.000000 sqlmesh-0.5.1.dev35/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      817 2023-02-27 20:28:04.000000 sqlmesh-0.5.1.dev35/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     9363 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/index.css
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.944813 sqlmesh-0.5.1.dev35/web/client/src/library/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:15.946210 sqlmesh-0.5.1.dev35/web/client/src/library/components/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.037537 sqlmesh-0.5.1.dev35/web/client/src/library/components/banner/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1705 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.037691 sqlmesh-0.5.1.dev35/web/client/src/library/components/button/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4517 2023-03-25 06:07:32.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.037859 sqlmesh-0.5.1.dev35/web/client/src/library/components/button/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)     3516 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.038030 sqlmesh-0.5.1.dev35/web/client/src/library/components/divider/
--rw-r--r--   0 izeigerman   (501) staff       (20)      856 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.038180 sqlmesh-0.5.1.dev35/web/client/src/library/components/divider/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      632 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.039418 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1388 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 izeigerman   (501) staff       (20)     5397 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8015 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     2718 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     9819 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    11303 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3527 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.039722 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 izeigerman   (501) staff       (20)     5880 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3987 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1538 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.040305 sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/
--rw-r--r--   0 izeigerman   (501) staff       (20)    10852 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6045 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     2997 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      562 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.040559 sqlmesh-0.5.1.dev35/web/client/src/library/components/graph/
--rw-r--r--   0 izeigerman   (501) staff       (20)    14478 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6392 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.041018 sqlmesh-0.5.1.dev35/web/client/src/library/components/ide/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4342 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     4870 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    22356 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.041323 sqlmesh-0.5.1.dev35/web/client/src/library/components/input/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2087 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.041476 sqlmesh-0.5.1.dev35/web/client/src/library/components/loading/
--rw-r--r--   0 izeigerman   (501) staff       (20)      486 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/loading/Loading.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.041888 sqlmesh-0.5.1.dev35/web/client/src/library/components/logo/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2292 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     4637 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8042 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.042265 sqlmesh-0.5.1.dev35/web/client/src/library/components/modal/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1560 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1447 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.043901 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/
--rw-r--r--   0 izeigerman   (501) staff       (20)     9269 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6775 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1312 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    10448 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     4920 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    15855 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     9926 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    12528 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3444 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2155 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2599 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.044078 sqlmesh-0.5.1.dev35/web/client/src/library/components/progress/
--rw-r--r--   0 izeigerman   (501) staff       (20)      713 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.044238 sqlmesh-0.5.1.dev35/web/client/src/library/components/report/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1047 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/report/ReportTestsErrors.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.044826 sqlmesh-0.5.1.dev35/web/client/src/library/components/root/
--rw-r--r--   0 izeigerman   (501) staff       (20)      526 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1921 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      443 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.045073 sqlmesh-0.5.1.dev35/web/client/src/library/components/splitPane/
--rw-r--r--   0 izeigerman   (501) staff       (20)      788 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.045224 sqlmesh-0.5.1.dev35/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 izeigerman   (501) staff       (20)    11713 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.045354 sqlmesh-0.5.1.dev35/web/client/src/library/components/toggle/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1453 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1197 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/main.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.046108 sqlmesh-0.5.1.dev35/web/client/src/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1647 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev35/web/client/src/models/artifact.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3472 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/models/directory.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     4190 2023-03-16 22:35:40.000000 sqlmesh-0.5.1.dev35/web/client/src/models/environment.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1760 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/web/client/src/models/file.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      173 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev35/web/client/src/models/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      766 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev35/web/client/src/models/initial.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      200 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev35/web/client/src/routes.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.046411 sqlmesh-0.5.1.dev35/web/client/src/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)       35 2023-01-20 18:11:03.000000 sqlmesh-0.5.1.dev35/web/client/src/tests/setup.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.5.1.dev35/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.046732 sqlmesh-0.5.1.dev35/web/client/src/types/
--rw-r--r--   0 izeigerman   (501) staff       (20)      467 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/types/enum.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      137 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/types/index.d.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.047045 sqlmesh-0.5.1.dev35/web/client/src/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4102 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev35/web/client/src/utils/index.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5245 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/utils/index.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.047167 sqlmesh-0.5.1.dev35/web/client/src/workers/
--rw-r--r--   0 izeigerman   (501) staff       (20)      113 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/workers/index.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.047484 sqlmesh-0.5.1.dev35/web/client/src/workers/sqlglot/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1105 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1578 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5842 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/web/client/tailwind.config.js
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.047649 sqlmesh-0.5.1.dev35/web/client/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      170 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/tests/initial.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1141 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/client/tsconfig.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     1297 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev35/web/client/vite.config.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.048928 sqlmesh-0.5.1.dev35/web/server/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev35/web/server/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.049075 sqlmesh-0.5.1.dev35/web/server/api/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev35/web/server/api/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-25 23:11:16.050709 sqlmesh-0.5.1.dev35/web/server/api/endpoints/
--rw-r--r--   0 izeigerman   (501) staff       (20)      784 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4564 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/commands.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      819 2023-02-27 20:28:04.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1858 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/directories.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      721 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/environments.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      637 2023-02-15 19:33:57.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/events.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5229 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/files.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3283 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/lineage.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      962 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/models.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3628 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev35/web/server/api/endpoints/plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3775 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev35/web/server/console.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1374 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/server/main.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5777 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev35/web/server/models.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      260 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev35/web/server/openapi.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2421 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/web/server/settings.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2114 2023-02-04 22:32:08.000000 sqlmesh-0.5.1.dev35/web/server/sse.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2461 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev35/web/server/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.787782 sqlmesh-0.6.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.683781 sqlmesh-0.6.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4414 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/.circleci/continue_config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1900 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/Dockerfile.api
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/Dockerfile.app
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11346 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1936 2023-04-26 17:24:35.787782 sqlmesh-0.6.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.683781 sqlmesh-0.6.0/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.663780 sqlmesh-0.6.0/docs/_readthedocs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.683781 sqlmesh-0.6.0/docs/_readthedocs/html/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/_readthedocs/html/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9965 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/comparisons.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.683781 sqlmesh-0.6.0/docs/concepts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.683781 sqlmesh-0.6.0/docs/concepts/architecture/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6689 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/audits.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5952 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/glossary.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/hooks.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/macros.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.687780 sqlmesh-0.6.0/docs/concepts/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7859 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/models/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/models/python_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4938 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/models/seed_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/models/sql_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/overview.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.687780 sqlmesh-0.6.0/docs/concepts/plans/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43124 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8973 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/plans.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5699 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/concepts/tests.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/development.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.687780 sqlmesh-0.6.0/docs/guides/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1943 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/connections.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/migrations.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/multi_repo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/projects.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.687780 sqlmesh-0.6.0/docs/guides/scheduling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   740917 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   379880 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5648 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/scheduling.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1854 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/guides/testing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5459 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/installation.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.687780 sqlmesh-0.6.0/docs/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/integrations/airflow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7801 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/integrations/dbt.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24057 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/integrations/engines.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/integrations/github.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/integrations/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/prerequisites.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10723 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/quick_start.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/docs/reference/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/reference/cli.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13607 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/reference/configuration.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/reference/notebook.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/reference/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/reference/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/release_notes.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3249 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/docs/sqlmesh.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/Dockerfile.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      942 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/airflow/dags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3515 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/airflow/spark_conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.667780 sqlmesh-0.6.0/examples/multi/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/multi/repo_1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/multi/repo_1/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/multi/repo_1/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/multi/repo_1/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/multi/repo_1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.691781 sqlmesh-0.6.0/examples/multi/repo_2/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/multi/repo_2/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/multi/repo_2/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/multi/repo_2/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/multi/repo_2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/sushi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/sushi/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/audits/items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/sushi/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/data/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/sushi/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/sushi/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      702 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/sushi/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      916 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1910 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/order_items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/orders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      197 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.695781 sqlmesh-0.6.0/examples/sushi/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      752 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.667780 sqlmesh-0.6.0/examples/sushi_dbt/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.699781 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      783 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/sushi_dbt/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/sushi_dbt/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.667780 sqlmesh-0.6.0/examples/wursthall/audits/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/audits/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/models/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3161 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      542 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/models/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1672 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3434 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.671780 sqlmesh-0.6.0/examples/wursthall/seeds/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/seeds/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/examples/wursthall/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/mkdocs.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/pdoc/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1153 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/pdoc/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/pdoc/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.703781 sqlmesh-0.6.0/posts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.707781 sqlmesh-0.6.0/posts/virtual_data_environments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   318753 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   274526 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163619 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   298971 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   366545 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1344487 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18638 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/posts/virtual_data_environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-04-26 17:24:35.787782 sqlmesh-0.6.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3158 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.707781 sqlmesh-0.6.0/sqlmesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/.airflowignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-04-26 17:24:35.000000 sqlmesh-0.6.0/sqlmesh/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.711781 sqlmesh-0.6.0/sqlmesh/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4314 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/cli/example_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9641 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/cli/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/cli/options.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.711781 sqlmesh-0.6.0/sqlmesh/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/_typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.711781 sqlmesh-0.6.0/sqlmesh/core/audit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8136 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.715781 sqlmesh-0.6.0/sqlmesh/core/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      668 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21184 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/connection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3351 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/root.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8421 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29390 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36016 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8904 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/context_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17626 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/dialect.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.715781 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2626 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29021 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4191 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15694 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1939 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6650 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4131 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12673 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18920 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.719781 sqlmesh-0.6.0/sqlmesh/core/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1746 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2417 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47685 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8168 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/kind.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13034 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2017 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/model/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2314 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.719781 sqlmesh-0.6.0/sqlmesh/core/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22476 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8125 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12623 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/renderer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15386 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20418 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.719781 sqlmesh-0.6.0/sqlmesh/core/snapshot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33750 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19248 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.719781 sqlmesh-0.6.0/sqlmesh/core/state_sync/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13382 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13144 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20810 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10834 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/core/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9390 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16407 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11231 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1762 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4771 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5087 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8044 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9807 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13257 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/package.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3701 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4772 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13503 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/dbt/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/engines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4437 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/engines/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2210 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13754 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/magics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/migrations/v0003_move_batch_size.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.723781 sqlmesh-0.6.0/sqlmesh/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.727781 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4020 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3830 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18819 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.727781 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2132 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8508 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.727781 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6307 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1340 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5222 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11104 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4400 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1292 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4139 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5213 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.731781 sqlmesh-0.6.0/sqlmesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4378 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7530 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4329 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7549 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16084 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/rich.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.711781 sqlmesh-0.6.0/sqlmesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1936 2023-04-26 17:24:35.000000 sqlmesh-0.6.0/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21936 2023-04-26 17:24:35.000000 sqlmesh-0.6.0/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-26 17:24:35.000000 sqlmesh-0.6.0/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-04-26 17:24:35.000000 sqlmesh-0.6.0/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2023-04-26 17:24:35.000000 sqlmesh-0.6.0/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-26 17:24:35.000000 sqlmesh-0.6.0/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21020 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/sqlmesh.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.731781 sqlmesh-0.6.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/common_fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4037 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.735781 sqlmesh-0.6.0/tests/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27881 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1270 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8036 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7073 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_audit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6611 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_connection_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10197 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_dialect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26685 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5880 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25301 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15741 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3862 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4647 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32235 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_schema_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28498 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_snapshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10299 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23620 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/core/test_state_sync.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/dbt/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/dbt/test_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13195 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/dbt/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17098 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/dbt/test_transformation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/engines/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/engines/spark/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.675780 sqlmesh-0.6.0/tests/fixtures/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.671780 sqlmesh-0.6.0/tests/fixtures/dbt/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.671780 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1055 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10264 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.739781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.675780 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.743781 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.747781 sqlmesh-0.6.0/tests/fixtures/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25229 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.747781 sqlmesh-0.6.0/tests/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.747781 sqlmesh-0.6.0/tests/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/integrations/github/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.747781 sqlmesh-0.6.0/tests/integrations/github/fixtures/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.747781 sqlmesh-0.6.0/tests/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.747781 sqlmesh-0.6.0/tests/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1414 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.747781 sqlmesh-0.6.0/tests/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4442 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4392 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9857 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6222 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5944 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.751781 sqlmesh-0.6.0/tests/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3580 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1818 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_filesystem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5516 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2501 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2911 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/utils/test_yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.751781 sqlmesh-0.6.0/tests/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/web/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16232 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/tests/web/test_main.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.751781 sqlmesh-0.6.0/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.755781 sqlmesh-0.6.0/web/client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/.eslintrc.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/.prettierignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/.prettierrc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.755781 sqlmesh-0.6.0/web/client/dist/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.759781 sqlmesh-0.6.0/web/client/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74500 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/CircularStd-Black-52659624.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74368 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74116 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24788 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/Plan-2de6d040.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55004 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57104 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/Publico-Bold-c79acd56.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    56836 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/Publico-Medium-01b4a891.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43005 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/index-5ca623f3.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2636569 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/index-64d94ea3.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/assets/worker-e891d118.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.759781 sqlmesh-0.6.0/web/client/dist/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-04-26 17:24:17.000000 sqlmesh-0.6.0/web/client/dist/favicons/favicon.ico
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-04-26 17:24:19.000000 sqlmesh-0.6.0/web/client/dist/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37689 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/openapi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      330 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/orval.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   408504 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/playwright.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/postcss.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.675780 sqlmesh-0.6.0/web/client/public/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.759781 sqlmesh-0.6.0/web/client/public/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.759781 sqlmesh-0.6.0/web/client/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.759781 sqlmesh-0.6.0/web/client/src/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/api/channels.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5243 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/api/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3247 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/api/instance.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.675780 sqlmesh-0.6.0/web/client/src/assets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.675780 sqlmesh-0.6.0/web/client/src/assets/fonts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.763781 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74500 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74524 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74368 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73964 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    68940 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    67284 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74116 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73916 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.767781 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    55004 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56384 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57104 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    62320 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56652 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61688 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57680 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    53148 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57060 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56836 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61460 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    52820 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    59176 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    63876 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60768 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    81732 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60992 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    64792 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.767781 sqlmesh-0.6.0/web/client/src/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4126 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/context/context.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5719 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/context/editor.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/context/fileTree.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2284 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/context/lineage.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2661 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/context/plan.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/context/theme.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.767781 sqlmesh-0.6.0/web/client/src/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9555 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/index.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.675780 sqlmesh-0.6.0/web/client/src/library/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.679781 sqlmesh-0.6.0/web/client/src/library/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.767781 sqlmesh-0.6.0/web/client/src/library/components/banner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1705 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.767781 sqlmesh-0.6.0/web/client/src/library/components/button/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4517 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.767781 sqlmesh-0.6.0/web/client/src/library/components/button/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.771781 sqlmesh-0.6.0/web/client/src/library/components/divider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.771781 sqlmesh-0.6.0/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.771781 sqlmesh-0.6.0/web/client/src/library/components/editor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1992 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5437 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8518 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9819 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11419 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3796 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.771781 sqlmesh-0.6.0/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5820 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5744 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.771781 sqlmesh-0.6.0/web/client/src/library/components/fileTree/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10852 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.771781 sqlmesh-0.6.0/web/client/src/library/components/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15931 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7045 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.771781 sqlmesh-0.6.0/web/client/src/library/components/ide/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4933 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22356 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.775781 sqlmesh-0.6.0/web/client/src/library/components/input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2087 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.775781 sqlmesh-0.6.0/web/client/src/library/components/loading/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/loading/Loading.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.775781 sqlmesh-0.6.0/web/client/src/library/components/logo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4637 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.775781 sqlmesh-0.6.0/web/client/src/library/components/modal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/library/components/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10448 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4920 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15855 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9926 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12528 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3444 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2155 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/library/components/progress/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/library/components/report/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/report/ReportTestsErrors.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/library/components/root/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1921 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/library/components/splitPane/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11713 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/library/components/toggle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1453 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1197 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/main.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1647 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/models/artifact.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3472 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/models/directory.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4190 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/models/environment.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/models/file.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/models/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/models/initial.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/routes.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/tests/setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.779781 sqlmesh-0.6.0/web/client/src/types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/types/enum.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/types/index.d.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.783782 sqlmesh-0.6.0/web/client/src/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5245 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/utils/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.783782 sqlmesh-0.6.0/web/client/src/workers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/workers/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.783782 sqlmesh-0.6.0/web/client/src/workers/sqlglot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5879 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/tailwind.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.783782 sqlmesh-0.6.0/web/client/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/tests/initial.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/tsconfig.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1297 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/client/vite.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.783782 sqlmesh-0.6.0/web/server/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.783782 sqlmesh-0.6.0/web/server/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 17:24:35.787782 sqlmesh-0.6.0/web/server/api/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4564 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      819 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/directories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/environments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/files.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/api/endpoints/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5777 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/openapi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2421 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/sse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2461 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      790 2023-04-26 17:24:29.000000 sqlmesh-0.6.0/web/server/watcher.py
```

### Comparing `sqlmesh-0.5.1.dev35/.circleci/config.yml` & `sqlmesh-0.6.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/.circleci/continue_config.yml` & `sqlmesh-0.6.0/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/.gitignore` & `sqlmesh-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/.pre-commit-config.yaml` & `sqlmesh-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/LICENSE` & `sqlmesh-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/Makefile` & `sqlmesh-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/PKG-INFO` & `sqlmesh-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.5.1.dev35
-Summary: UNKNOWN
+Version: 0.6.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -36,15 +34,13 @@
 ```pip install sqlmesh```
 
 Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
 
 ## Join our community
 We'd love to join you on your data journey. Connect with us in the following ways:
 
-* Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
 * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
 * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
 
 ## Contribution
 Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-
-
```

### Comparing `sqlmesh-0.5.1.dev35/README.md` & `sqlmesh-0.6.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 ```pip install sqlmesh```
 
 Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
 
 ## Join our community
 We'd love to join you on your data journey. Connect with us in the following ways:
 
-* Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
 * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
 * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
 
 ## Contribution
 Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
```

### Comparing `sqlmesh-0.5.1.dev35/docker-compose.yml` & `sqlmesh-0.6.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/comparisons.md` & `sqlmesh-0.6.0/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/architecture/serialization.md` & `sqlmesh-0.6.0/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.6.0/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/audits.md` & `sqlmesh-0.6.0/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/environments.md` & `sqlmesh-0.6.0/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/glossary.md` & `sqlmesh-0.6.0/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/macros.md` & `sqlmesh-0.6.0/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/models/model_kinds.md` & `sqlmesh-0.6.0/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/models/overview.md` & `sqlmesh-0.6.0/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/models/python_models.md` & `sqlmesh-0.6.0/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/models/seed_models.md` & `sqlmesh-0.6.0/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/models/sql_models.md` & `sqlmesh-0.6.0/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/overview.md` & `sqlmesh-0.6.0/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.6.0/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/plans.md` & `sqlmesh-0.6.0/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/concepts/tests.md` & `sqlmesh-0.6.0/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/development.md` & `sqlmesh-0.6.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/connections.md` & `sqlmesh-0.6.0/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/migrations.md` & `sqlmesh-0.6.0/docs/guides/migrations.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/models.md` & `sqlmesh-0.6.0/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/multi_repo.md` & `sqlmesh-0.6.0/docs/guides/multi_repo.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/projects.md` & `sqlmesh-0.6.0/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.6.0/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.6.0/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/scheduling.md` & `sqlmesh-0.6.0/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/guides/testing.md` & `sqlmesh-0.6.0/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/index.md` & `sqlmesh-0.6.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 
 * Table/Column level lineage visualizations (in development)
     * Quickly understand the full lineage and sequence of transformation of any column.
 
 ## Next steps
 * [Jump right in with the quickstart](quick_start.md)
 * [Learn more about SQLMesh concepts](concepts/overview.md)
-* [Join our Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg)
+* [Join our Slack community](https://tobikodata.com/slack)
```

### Comparing `sqlmesh-0.5.1.dev35/docs/integrations/airflow.md` & `sqlmesh-0.6.0/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/integrations/dbt.md` & `sqlmesh-0.6.0/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/integrations/engines.md` & `sqlmesh-0.6.0/docs/integrations/engines.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 | `priority`                      | The priority of the underlying job. (Default: `INTERACTIVE`)                                  | string |    N     |
 | `maximum_bytes_billed`          | The maximum number of bytes to be billed for the underlying job.                              |  int   |    N     |
 
 
 ## BigQuery - Airflow Scheduler
 **Engine Name:** `bigquery`
 
-In order to share a common implementation across local and Airflow, SQLMesh BigQuery implements its own hook and operator. 
+In order to share a common implementation across local and Airflow, SQLMesh BigQuery implements its own hook and operator.
 
 To enable support for this operator, the Airflow BigQuery provider package should be installed on the target Airflow cluster along with SQLMesh with the BigQuery extra:
 ```
 pip install "apache-airflow-providers-google"
 pip install "sqlmesh[bigquery]"
 ```
 
@@ -43,29 +43,29 @@
         "sqlmesh_gcp_conn_id": "<Connection ID>"
     },
 )
 ```
 
 # Databricks
 ## Databricks - Local/Built-in Scheduler
-If your project contains Python models that use PySpark DataFrames AND you are using the built-in scheduler, then you must run plan/apply on a Databricks cluster. 
+If your project contains Python models that use PySpark DataFrames AND you are using the built-in scheduler, then you must run plan/apply on a Databricks cluster.
 This can be done using the [Notebook magic](../reference/notebook.md) or by using the [CLI](../reference/cli.md).
-This is something we are looking into improving &mdash; please leave us feedback in [our Slack channel](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) if this impacts you.
+This is something we are looking into improving &mdash; please leave us feedback in [our Slack channel](https://tobikodata.com/slack) if this impacts you.
 A potential workaround until this support is added is to use [Databricks Connect](https://docs.databricks.com/dev-tools/databricks-connect.html). This will make it look like you are running on a cluster, and should theoretically work.
 
 Databricks has a few options for connection types to choose from:
 ### Type: databricks (Recommended)
-This type will automatically detect if you are running in an environment that already has a SparkSession defined. 
-If it detects a SparkSession, then it assumes this is a Databricks SparkSession and uses that. 
+This type will automatically detect if you are running in an environment that already has a SparkSession defined.
+If it detects a SparkSession, then it assumes this is a Databricks SparkSession and uses that.
 If it doesn't detect a SparkSession, then it will use the connection configuration to connect to Databricks over
-the [Databricks SQL Connector](https://docs.databricks.com/dev-tools/python-sql-connector.html). 
+the [Databricks SQL Connector](https://docs.databricks.com/dev-tools/python-sql-connector.html).
 See [databricks_sql configuration](#type--databrickssql) for the connection configuration.
 
 ### Type: databricks_spark_session
-This connection type assumes that wherever you are running you have access to a Databricks SparkSession. 
+This connection type assumes that wherever you are running you have access to a Databricks SparkSession.
 This will simplify the required configuration to run since you will not need to provide connection configuration.
 
 ### Type: databricks_sql
 This connection type assumes you only need to run SQL queries against Databricks.
 If all of your models are SQL models or if Python doesn't use PySpark DataFrame, then this can be used.
 Below is the connection configuration for this type:
 
@@ -82,24 +82,24 @@
 
 Databricks has multiple operators to help differentiate running a SQL query vs. running a Python script.
 
 ### Engine: `databricks` (Recommended)
 
 When evaluating models, the SQLMesh Databricks integration implements the [DatabricksSubmitRunOperator](https://airflow.apache.org/docs/apache-airflow-providers-databricks/1.0.0/operators.html). This is needed to be able to run either SQL or Python scripts on the Databricks cluster.
 
-When performing environment management operations, the SQLMesh Databricks integration is similar to the [DatabricksSqlOperator](https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/operators/sql.html#databrickssqloperator), and relies on the same [DatabricksSqlHook](https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/_api/airflow/providers/databricks/hooks/databricks_sql/index.html#airflow.providers.databricks.hooks.databricks_sql.DatabricksSqlHook) implementation. 
+When performing environment management operations, the SQLMesh Databricks integration is similar to the [DatabricksSqlOperator](https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/operators/sql.html#databrickssqloperator), and relies on the same [DatabricksSqlHook](https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/_api/airflow/providers/databricks/hooks/databricks_sql/index.html#airflow.providers.databricks.hooks.databricks_sql.DatabricksSqlHook) implementation.
 All environment management operations are SQL-based, and the overhead of submitting jobs can be avoided.
 
 ### Engine: `databricks-submit`
 
 Whether evaluating models or performing environment management operations, the SQLMesh Databricks integration implements the [DatabricksSubmitRunOperator](https://airflow.apache.org/docs/apache-airflow-providers-databricks/1.0.0/operators.html).
 
 ### Engine: `databricks-sql`
 
-Forces the SQLMesh Databricks integration to use the operator based on the [DatabricksSqlOperator](https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/operators/sql.html#databrickssqloperator) for all operations. If your project is pure SQL operations, then this is an option. 
+Forces the SQLMesh Databricks integration to use the operator based on the [DatabricksSqlOperator](https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/operators/sql.html#databrickssqloperator) for all operations. If your project is pure SQL operations, then this is an option.
 
 To enable support for this operator, the Airflow Databricks provider package should be installed on the target Airflow cluster along with the SQLMesh package with databricks extra as follows:
 ```
 pip install apache-airflow-providers-databricks
 sqlmesh[databricks]
 ```
 
@@ -142,15 +142,15 @@
 # DuckDB
 ## DuckDB - Local/Built-in Scheduler
 | Option     | Description                                                                  |  Type  | Required |
 |------------|------------------------------------------------------------------------------|:------:|:--------:|
 | `database` | The optional database name. If not specified, the in-memory database is used | string |    N     |
 
 ## DuckDB - Airflow
-DuckDB only works when running locally; therefore it does not support Airflow. 
+DuckDB only works when running locally; therefore it does not support Airflow.
 
 # Postgres
 ## Postgres - Local/Built-in Scheduler
 | Option            | Description                                                                     |  Type  | Required |
 |-------------------|---------------------------------------------------------------------------------|:------:|:--------:|
 | `host`            | The hostname of the Postgres server                                             | string |    Y     |
 | `user`            | The username to use for authentication with the Postgres server                 | string |    Y     |
@@ -208,15 +208,15 @@
 | `is_serverless`         | If the Amazon Redshift cluster is serverless (Default: `False`)                                             |  bool  |    N     |
 | `serverless_acct_id`    | The account ID of the serverless cluster                                                                    | string |    N     |
 | `serverless_work_group` | The name of work group for serverless end point                                                             | string |    N     |
 
 ## Redshift - Airflow Scheduler
 **Engine Name:** `redshift`
 
-In order to share a common implementation across local and Airflow, SQLMesh Bigquery implements its own hook and operator. 
+In order to share a common implementation across local and Airflow, SQLMesh Bigquery implements its own hook and operator.
 
 To enable support for this operator, the Airflow BigQuery provider package should be installed on the target Airflow cluster along with SQLMesh with the Redshift extra:
 ```
 pip install "apache-airflow-providers-amazon"
 pip install "sqlmesh[redshift]"
 ```
```

### Comparing `sqlmesh-0.5.1.dev35/docs/integrations/github.md` & `sqlmesh-0.6.0/docs/integrations/github.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GitHub Actions
 
 SQLMesh's Github Actions integration will allow you to add a SQLMesh CI/CD bot to any Github project using [Github Actions](https://github.com/features/actions). The bot will automatically run [plan/apply](../concepts/plans.md) to an [environment](../concepts/environments.md) based on the code in a pull request.
 
-This will be done without copying or rebuilding data using SQLMesh's [Virtual Data Environments](../concepts/glossary.md#virtual-environments). 
+This will be done without copying or rebuilding data using SQLMesh's [Virtual Data Environments](../concepts/glossary.md#virtual-environments).
 Once approved, the CI/CD bot will automatically run [plan/apply](../concepts/plans.md) to the production environment and merge the PR upon completion.
 This allows you to always have your main branch and prod environments in sync.
 
-We will be launching this CI/CD bot soon &mdash; in the meantime, please leave any feedback or questions in [our Slack channel](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg)!
+We will be launching this CI/CD bot soon &mdash; in the meantime, please leave any feedback or questions in [our Slack channel](https://tobikodata.com/slack)!
```

### Comparing `sqlmesh-0.5.1.dev35/docs/prerequisites.md` & `sqlmesh-0.6.0/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/quick_start.md` & `sqlmesh-0.6.0/docs/quick_start.md`

 * *Files 1% similar despite different names*

```diff
@@ -248,8 +248,8 @@
 ```
 
 ## 5. Next steps
 
 Congratulations, you've now conquered the basics of using SQLMesh!
 
 * [Learn more about SQLMesh concepts](concepts/overview.md)
-* [Join our Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg)
+* [Join our Slack community](https://tobikodata.com/slack)
```

### Comparing `sqlmesh-0.5.1.dev35/docs/reference/cli.md` & `sqlmesh-0.6.0/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/reference/configuration.md` & `sqlmesh-0.6.0/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/reference/notebook.md` & `sqlmesh-0.6.0/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/reference/overview.md` & `sqlmesh-0.6.0/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/docs/sqlmesh.png` & `sqlmesh-0.6.0/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/airflow/Dockerfile.template` & `sqlmesh-0.6.0/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/airflow/Makefile` & `sqlmesh-0.6.0/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/airflow/README.md` & `sqlmesh-0.6.0/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.6.0/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.6.0/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/config.py` & `sqlmesh-0.6.0/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/helper.py` & `sqlmesh-0.6.0/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/macros/macros.py` & `sqlmesh-0.6.0/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.0/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/models/items.py` & `sqlmesh-0.6.0/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/models/order_items.py` & `sqlmesh-0.6.0/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/models/orders.py` & `sqlmesh-0.6.0/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.0/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.6.0/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.6.0/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.0/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.6.0/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.6.0/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.6.0/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.6.0/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.6.0/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/macros/macros.py` & `sqlmesh-0.6.0/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.6.0/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.6.0/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.6.0/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.6.0/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/models/src/shared.py` & `sqlmesh-0.6.0/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.6.0/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.6.0/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.6.0/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/mkdocs.yml` & `sqlmesh-0.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/pdoc/cli.py` & `sqlmesh-0.6.0/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/posts/virtual_data_environments/change_categorization.png` & `sqlmesh-0.6.0/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/posts/virtual_data_environments/isolated_rigid_envs.png` & `sqlmesh-0.6.0/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/posts/virtual_data_environments/partial_breaking.png` & `sqlmesh-0.6.0/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/posts/virtual_data_environments/stateful_envs.png` & `sqlmesh-0.6.0/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/posts/virtual_data_environments/virtual_envs.png` & `sqlmesh-0.6.0/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/posts/virtual_data_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.6.0/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/posts/virtual_data_environments.md` & `sqlmesh-0.6.0/posts/virtual_data_environments.md`

 * *Files 0% similar despite different names*

```diff
@@ -154,8 +154,8 @@
 - Data is immediately available in new environments thanks to the separation between **virtual** and **physical** layers.
 - Changes and their downstream impacts are categorized automatically to achieve both efficiency and correctness.
 - Rolling back a change happens almost instantaneously since no data movement is involved and only views that are part of the **virtual layer** get updated.
 - Deploying changes to production is a **virtual layer** operation, which ensures that results observed during development are exactly the same in production and that data and code are always in sync.
 
 To streamline deploying changes to production, our team is about to release the SQLMesh [CI/CD bot](https://github.com/TobikoData/sqlmesh/blob/main/docs/integrations/github.md), which will help automate this process.
 
-Don't miss out - join our [Slack channel](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) and stay tuned!
+Don't miss out - join our [Slack channel](https://tobikodata.com/slack) and stay tuned!
```

### Comparing `sqlmesh-0.5.1.dev35/pytest.ini` & `sqlmesh-0.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/setup.cfg` & `sqlmesh-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/setup.py` & `sqlmesh-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             "redshift_connector",
         ],
         "snowflake": [
             "snowflake-connector-python[pandas]",
         ],
         "web": [
             "fastapi==0.95.0",
-            "hyperscript==0.0.1",
+            "watchfiles==0.19.0",
             "pyarrow==11.0.0",
             "uvicorn==0.21.1",
         ],
     },
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/__init__.py` & `sqlmesh-0.6.0/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/cli/__init__.py` & `sqlmesh-0.6.0/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/cli/example_project.py` & `sqlmesh-0.6.0/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/cli/main.py` & `sqlmesh-0.6.0/sqlmesh/cli/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/cli/options.py` & `sqlmesh-0.6.0/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/_typing.py` & `sqlmesh-0.6.0/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.6.0/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/audit/definition.py` & `sqlmesh-0.6.0/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/__init__.py` & `sqlmesh-0.6.0/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/base.py` & `sqlmesh-0.6.0/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.6.0/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/common.py` & `sqlmesh-0.6.0/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/connection.py` & `sqlmesh-0.6.0/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/loader.py` & `sqlmesh-0.6.0/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/model.py` & `sqlmesh-0.6.0/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/root.py` & `sqlmesh-0.6.0/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.6.0/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/console.py` & `sqlmesh-0.6.0/sqlmesh/core/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/constants.py` & `sqlmesh-0.6.0/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/context.py` & `sqlmesh-0.6.0/sqlmesh/core/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -888,15 +888,15 @@
             if snapshot.version
             else snapshot.qualified_view_name.for_environment(c.PROD)
             for name, snapshot in self.snapshots.items()
         }
 
     def _context_diff(
         self,
-        environment: str | Environment,
+        environment: str,
         snapshots: t.Optional[t.Dict[str, Snapshot]] = None,
         create_from: t.Optional[str] = None,
     ) -> ContextDiff:
         environment = Environment.normalize_name(environment)
         return ContextDiff.create(
             environment,
             snapshots=snapshots or self.snapshots,
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/context_diff.py` & `sqlmesh-0.6.0/sqlmesh/core/context_diff.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 When creating a ContextDiff object, SQLMesh will compare the snapshots from one environment with those of
 another remote environment and determine if models have been added, removed, or modified.
 """
 from __future__ import annotations
 
 import typing as t
 
-from sqlmesh.core.environment import Environment
 from sqlmesh.core.snapshot import (
     Snapshot,
     SnapshotChangeCategory,
     SnapshotDataVersion,
     SnapshotId,
 )
 from sqlmesh.utils.errors import SQLMeshError
@@ -34,14 +33,16 @@
     environments.
     """
 
     environment: str
     """The environment to diff."""
     is_new_environment: bool
     """Whether the target environment is new."""
+    is_unfinalized_environment: bool
+    """Whether the currently stored environment record is in unfinalized state."""
     create_from: str
     """The name of the environment the target environment will be created from if new."""
     added: t.Set[str]
     """New models."""
     removed: t.Set[str]
     """Deleted models."""
     modified_snapshots: t.Dict[str, t.Tuple[Snapshot, Snapshot]]
@@ -52,15 +53,15 @@
     """New snapshots."""
     previous_plan_id: t.Optional[str]
     """Previous plan id."""
 
     @classmethod
     def create(
         cls,
-        environment: str | Environment,
+        environment: str,
         snapshots: t.Dict[str, Snapshot],
         create_from: str,
         state_reader: StateReader,
     ) -> ContextDiff:
         """Create a ContextDiff object.
 
         Args:
@@ -69,20 +70,16 @@
             create_from: The environment to create the target environment from if it
                 doesn't exist.
             state_reader: StateReader to access the remote environment to diff.
 
         Returns:
             The ContextDiff object.
         """
-        if isinstance(environment, str):
-            environment = environment.lower()
-            env = state_reader.get_environment(environment)
-        else:
-            env = environment
-            environment = env.name.lower()
+        environment = environment.lower()
+        env = state_reader.get_environment(environment)
 
         if env is None:
             env = state_reader.get_environment(create_from.lower())
             is_new_environment = True
         else:
             is_new_environment = False
 
@@ -147,26 +144,29 @@
                     snapshot.change_category = remote_head.change_category
                 else:
                     snapshot.categorize_as(SnapshotChangeCategory.BREAKING)
 
         return ContextDiff(
             environment=environment,
             is_new_environment=is_new_environment,
+            is_unfinalized_environment=bool(env and not env.finalized_ts),
             create_from=create_from,
             added=added,
             removed=removed,
             modified_snapshots=modified_snapshots,
             snapshots=merged_snapshots,
             new_snapshots=new_snapshots,
             previous_plan_id=env.plan_id if env and not is_new_environment else None,
         )
 
     @property
     def has_changes(self) -> bool:
-        return self.has_snapshot_changes or self.is_new_environment
+        return (
+            self.has_snapshot_changes or self.is_new_environment or self.is_unfinalized_environment
+        )
 
     @property
     def has_snapshot_changes(self) -> bool:
         return bool(self.added or self.removed or self.modified_snapshots)
 
     def directly_modified(self, model_name: str) -> bool:
         """Returns whether or not a model was directly modified in this context.
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/dialect.py` & `sqlmesh-0.6.0/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/base_postgres.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.6.0/sqlmesh/core/engine_adapter/spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/environment.py` & `sqlmesh-0.6.0/sqlmesh/core/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     name: str
     snapshots: t.List[SnapshotTableInfo]
     start_at: TimeLike
     end_at: t.Optional[TimeLike]
     plan_id: str
     previous_plan_id: t.Optional[str]
     expiration_ts: t.Optional[int]
+    finalized_ts: t.Optional[int]
 
     @validator("snapshots", pre=True)
     @classmethod
     def _convert_snapshots(cls, v: str | t.List[SnapshotTableInfo]) -> t.List[SnapshotTableInfo]:
         if isinstance(v, str):
             return [SnapshotTableInfo.parse_obj(obj) for obj in json.loads(v)]
         return v
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/hooks.py` & `sqlmesh-0.6.0/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/loader.py` & `sqlmesh-0.6.0/sqlmesh/core/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,17 @@
     ) -> UniqueKeyDict[str, Model]:
         """Loads the sql models into a Dict"""
         models: UniqueKeyDict = UniqueKeyDict("models")
         for context_path, config in self._context.configs.items():
             cache = SqlMeshLoader._Cache(self, context_path)
 
             for path in self._glob_paths(context_path / c.MODELS, config=config, extension=".sql"):
+                if not os.path.getsize(path):
+                    continue
+
                 self._track_file(path)
 
                 def _load() -> Model:
                     with open(path, "r", encoding="utf-8") as file:
                         try:
                             expressions = parse(
                                 file.read(), default_dialect=config.model_defaults.dialect
@@ -230,14 +233,17 @@
         models: UniqueKeyDict = UniqueKeyDict("models")
         registry = model_registry.registry()
         registry.clear()
         registered: t.Set[str] = set()
 
         for context_path, config in self._context.configs.items():
             for path in self._glob_paths(context_path / c.MODELS, config=config, extension=".py"):
+                if not os.path.getsize(path):
+                    continue
+
                 self._track_file(path)
                 self._import_python_file(path, context_path)
                 new = registry.keys() - registered
                 registered |= new
                 for name in new:
                     model = registry[name].model(
                         path=path,
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/macros.py` & `sqlmesh-0.6.0/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/__init__.py` & `sqlmesh-0.6.0/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/cache.py` & `sqlmesh-0.6.0/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/common.py` & `sqlmesh-0.6.0/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/decorator.py` & `sqlmesh-0.6.0/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/definition.py` & `sqlmesh-0.6.0/sqlmesh/core/model/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/kind.py` & `sqlmesh-0.6.0/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/meta.py` & `sqlmesh-0.6.0/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/model/seed.py` & `sqlmesh-0.6.0/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/notification_target.py` & `sqlmesh-0.6.0/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/plan/definition.py` & `sqlmesh-0.6.0/sqlmesh/core/plan/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.6.0/sqlmesh/core/plan/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
                 on_complete=on_complete,
             )
             self.snapshot_evaluator.demote(
                 removed,
                 environment=environment.name,
                 on_complete=on_complete,
             )
+            self.state_sync.finalize(environment)
             completed = True
         finally:
             self.console.stop_promotion_progress(success=completed)
 
     def _restate(self, plan: Plan) -> None:
         all_snapshots = (
             [s for s in plan.snapshots if s.name in plan.restatements]
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/renderer.py` & `sqlmesh-0.6.0/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/scheduler.py` & `sqlmesh-0.6.0/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/schema_diff.py` & `sqlmesh-0.6.0/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.6.0/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.6.0/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.6.0/sqlmesh/core/snapshot/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.6.0/sqlmesh/core/snapshot/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.6.0/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.6.0/sqlmesh/core/state_sync/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,14 +334,23 @@
                 snapshots for same models.
 
         Returns:
            A tuple of (added snapshot table infos, removed snapshot table infos)
         """
 
     @abc.abstractmethod
+    def finalize(self, environment: Environment) -> None:
+        """Finalize the target environment, indicating that this environment has been
+        fully promoted and is ready for use.
+
+        Args:
+            environment: The target environment to finalize.
+        """
+
+    @abc.abstractmethod
     def delete_expired_environments(self) -> t.List[Environment]:
         """Removes expired environments.
 
         Expired environments are environments that have exceeded their time-to-live value.
 
         Returns:
             The list of removed environments.
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.6.0/sqlmesh/core/state_sync/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     SnapshotId,
     SnapshotIdLike,
     SnapshotInfoLike,
     SnapshotNameVersionLike,
     SnapshotTableInfo,
 )
 from sqlmesh.core.state_sync.base import StateSync
-from sqlmesh.utils.date import TimeLike, now, to_datetime
+from sqlmesh.utils.date import TimeLike, now, now_timestamp, to_datetime
 from sqlmesh.utils.errors import SQLMeshError
 
 logger = logging.getLogger(__name__)
 
 
 def transactional(
     transaction_type: TransactionType = TransactionType.DML,
@@ -126,14 +126,34 @@
                     )
 
         table_infos = [s.table_info for s in snapshots]
         self._update_environment(environment)
         return table_infos, [existing_table_infos[name] for name in missing_models]
 
     @transactional()
+    def finalize(self, environment: Environment) -> None:
+        """Finalize the target environment, indicating that this environment has been
+        fully promoted and is ready for use.
+
+        Args:
+            environment: The target environment to finalize.
+        """
+        logger.info("Finalizing environment '%s'", environment)
+
+        stored_environment = self._get_environment(environment.name, lock_for_update=True)
+        if stored_environment and stored_environment.plan_id != environment.plan_id:
+            raise SQLMeshError(
+                f"Plan '{environment.plan_id}' is no longer valid for the target environment '{environment.name}'. "
+                f"Stored plan ID: '{stored_environment.plan_id}'. Please recreate the plan and try again"
+            )
+
+        environment.finalized_ts = now_timestamp()
+        self._update_environment(environment)
+
+    @transactional()
     def delete_expired_snapshots(self) -> t.List[Snapshot]:
         current_time = now()
 
         snapshots_by_version = defaultdict(list)
         for s in self._get_snapshots().values():
             snapshots_by_version[(s.name, s.version)].append(s)
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.6.0/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
             "name": exp.DataType.build("text"),
             "snapshots": exp.DataType.build("text"),
             "start_at": exp.DataType.build("text"),
             "end_at": exp.DataType.build("text"),
             "plan_id": exp.DataType.build("text"),
             "previous_plan_id": exp.DataType.build("text"),
             "expiration_ts": exp.DataType.build("bigint"),
+            "finalized_ts": exp.DataType.build("bigint"),
         }
 
     @property
     def version_columns_to_types(self) -> t.Dict[str, exp.DataType]:
         return {
             "schema_version": exp.DataType.build("int"),
             "sqlglot_version": exp.DataType.build("text"),
@@ -232,14 +233,15 @@
                             environment.name,
                             json.dumps([snapshot.dict() for snapshot in environment.snapshots]),
                             environment.start_at,
                             environment.end_at,
                             environment.plan_id,
                             environment.previous_plan_id,
                             environment.expiration_ts,
+                            environment.finalized_ts,
                         )
                     ],
                     columns_to_types=self.environment_columns_to_types,
                 )
             ),
             columns_to_types=self.environment_columns_to_types,
             contains_json=True,
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/test.py` & `sqlmesh-0.6.0/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/core/user.py` & `sqlmesh-0.6.0/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/adapter.py` & `sqlmesh-0.6.0/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.6.0/sqlmesh/dbt/basemodel.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/builtin.py` & `sqlmesh-0.6.0/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/column.py` & `sqlmesh-0.6.0/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/common.py` & `sqlmesh-0.6.0/sqlmesh/dbt/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/context.py` & `sqlmesh-0.6.0/sqlmesh/dbt/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/loader.py` & `sqlmesh-0.6.0/sqlmesh/dbt/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/model.py` & `sqlmesh-0.6.0/sqlmesh/dbt/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/package.py` & `sqlmesh-0.6.0/sqlmesh/dbt/package.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/profile.py` & `sqlmesh-0.6.0/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/project.py` & `sqlmesh-0.6.0/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/seed.py` & `sqlmesh-0.6.0/sqlmesh/dbt/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/source.py` & `sqlmesh-0.6.0/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/dbt/target.py` & `sqlmesh-0.6.0/sqlmesh/dbt/target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/engines/commands.py` & `sqlmesh-0.6.0/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/app.py` & `sqlmesh-0.6.0/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.6.0/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.6.0/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.6.0/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.6.0/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/magics.py` & `sqlmesh-0.6.0/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.6.0/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/migrations/v0003_move_batch_size.py` & `sqlmesh-0.6.0/sqlmesh/migrations/v0003_move_batch_size.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,41 +238,52 @@
 
     def _create_promotion_demotion_tasks(
         self, request: common.PlanDagSpec
     ) -> t.Tuple[BaseOperator, BaseOperator]:
         start_task = EmptyOperator(task_id="snapshot_promotion_start")
         end_task = EmptyOperator(task_id="snapshot_promotion_end")
 
+        environment = Environment(
+            name=request.environment_name,
+            snapshots=request.promoted_snapshots,
+            start_at=request.start,
+            end_at=request.end,
+            plan_id=request.plan_id,
+            previous_plan_id=request.previous_plan_id,
+            expiration_ts=request.environment_expiration_ts,
+        )
+
         update_state_task = PythonOperator(
             task_id="snapshot_promotion__update_state",
             python_callable=promotion_update_state_task,
             op_kwargs={
-                "snapshots": request.promoted_snapshots,
-                "environment_name": request.environment_name,
-                "start": request.start,
-                "end": request.end,
+                "environment": environment,
                 "unpaused_dt": request.unpaused_dt,
                 "no_gaps": request.no_gaps,
-                "plan_id": request.plan_id,
-                "previous_plan_id": request.previous_plan_id,
-                "environment_expiration_ts": request.environment_expiration_ts,
             },
         )
 
+        finalize_task = PythonOperator(
+            task_id="snapshot_promotion__finalize",
+            python_callable=promotion_finalize_task,
+            op_kwargs={"environment": environment},
+        )
+
         start_task >> update_state_task
+        finalize_task >> end_task
 
         if request.promoted_snapshots:
             create_views_task = self._create_snapshot_promotion_operator(
                 request.promoted_snapshots,
                 request.environment_name,
                 request.ddl_concurrent_tasks,
                 request.is_dev,
                 "snapshot_promotion__create_views",
             )
-            create_views_task >> end_task
+            create_views_task >> finalize_task
 
             if not request.is_dev and request.unpaused_dt:
                 migrate_tables_task = self._create_snapshot_migrate_tables_operator(
                     request.promoted_snapshots,
                     request.ddl_concurrent_tasks,
                     "snapshot_promotion__migrate_tables",
                 )
@@ -285,18 +296,18 @@
             delete_views_task = self._create_snapshot_demotion_operator(
                 request.demoted_snapshots,
                 request.environment_name,
                 request.ddl_concurrent_tasks,
                 "snapshot_promotion__delete_views",
             )
             update_state_task >> delete_views_task
-            delete_views_task >> end_task
+            delete_views_task >> finalize_task
 
         if not request.promoted_snapshots and not request.demoted_snapshots:
-            update_state_task >> end_task
+            update_state_task >> finalize_task
 
         return (start_task, end_task)
 
     def _create_backfill_tasks(
         self,
         backfill_intervals: t.List[common.BackfillIntervalsPerSnapshot],
         snapshots: t.Dict[SnapshotId, Snapshot],
@@ -475,30 +486,20 @@
 
 def creation_update_state_task(new_snapshots: t.Iterable[Snapshot]) -> None:
     with util.scoped_state_sync() as state_sync:
         state_sync.push_snapshots(new_snapshots)
 
 
 def promotion_update_state_task(
-    snapshots: t.List[SnapshotTableInfo],
-    environment_name: str,
-    start: TimeLike,
-    end: t.Optional[TimeLike],
+    environment: Environment,
     unpaused_dt: t.Optional[TimeLike],
     no_gaps: bool,
-    plan_id: str,
-    previous_plan_id: t.Optional[str],
-    environment_expiration_ts: t.Optional[int],
 ) -> None:
-    environment = Environment(
-        name=environment_name,
-        snapshots=snapshots,
-        start_at=start,
-        end_at=end,
-        plan_id=plan_id,
-        previous_plan_id=previous_plan_id,
-        expiration_ts=environment_expiration_ts,
-    )
     with util.scoped_state_sync() as state_sync:
         state_sync.promote(environment, no_gaps=no_gaps)
-        if snapshots and not end and unpaused_dt:
-            state_sync.unpause_snapshots(snapshots, unpaused_dt)
+        if environment.snapshots and not environment.end_at and unpaused_dt:
+            state_sync.unpause_snapshots(environment.snapshots, unpaused_dt)
+
+
+def promotion_finalize_task(environment: Environment) -> None:
+    with util.scoped_state_sync() as state_sync:
+        state_sync.finalize(environment)
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/postgres.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.6.0/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/__init__.py` & `sqlmesh-0.6.0/sqlmesh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/cache.py` & `sqlmesh-0.6.0/sqlmesh/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/concurrency.py` & `sqlmesh-0.6.0/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.6.0/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/dag.py` & `sqlmesh-0.6.0/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/date.py` & `sqlmesh-0.6.0/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/errors.py` & `sqlmesh-0.6.0/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/jinja.py` & `sqlmesh-0.6.0/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.6.0/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/pandas.py` & `sqlmesh-0.6.0/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/pydantic.py` & `sqlmesh-0.6.0/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/rich.py` & `sqlmesh-0.6.0/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.6.0/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh/utils/yaml.py` & `sqlmesh-0.6.0/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.6.0/sqlmesh.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.5.1.dev35
-Summary: UNKNOWN
+Version: 0.6.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -36,15 +34,13 @@
 ```pip install sqlmesh```
 
 Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
 
 ## Join our community
 We'd love to join you on your data journey. Connect with us in the following ways:
 
-* Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
 * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
 * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
 
 ## Contribution
 Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-
-
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.6.0/sqlmesh.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -271,14 +271,15 @@
 sqlmesh/integrations/github/notification_operator_provider.py
 sqlmesh/integrations/github/notification_target.py
 sqlmesh/integrations/github/shared.py
 sqlmesh/migrations/__init__.py
 sqlmesh/migrations/v0001_init.py
 sqlmesh/migrations/v0002_remove_identify.py
 sqlmesh/migrations/v0003_move_batch_size.py
+sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
 sqlmesh/schedulers/__init__.py
 sqlmesh/schedulers/airflow/__init__.py
 sqlmesh/schedulers/airflow/api.py
 sqlmesh/schedulers/airflow/client.py
 sqlmesh/schedulers/airflow/common.py
 sqlmesh/schedulers/airflow/dag_generator.py
 sqlmesh/schedulers/airflow/integration.py
@@ -429,14 +430,26 @@
 web/client/package-lock.json
 web/client/package.json
 web/client/playwright.config.ts
 web/client/postcss.config.js
 web/client/tailwind.config.js
 web/client/tsconfig.json
 web/client/vite.config.ts
+web/client/dist/index.html
+web/client/dist/assets/CircularStd-Black-52659624.otf
+web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+web/client/dist/assets/Plan-2de6d040.js
+web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+web/client/dist/assets/Publico-Bold-c79acd56.otf
+web/client/dist/assets/Publico-Medium-01b4a891.otf
+web/client/dist/assets/index-5ca623f3.css
+web/client/dist/assets/index-64d94ea3.js
+web/client/dist/assets/worker-e891d118.js
+web/client/dist/favicons/favicon.ico
 web/client/public/favicons/favicon.ico
 web/client/src/index.css
 web/client/src/main.tsx
 web/client/src/routes.tsx
 web/client/src/api/channels.ts
 web/client/src/api/index.ts
 web/client/src/api/instance.ts
@@ -549,14 +562,15 @@
 web/server/console.py
 web/server/main.py
 web/server/models.py
 web/server/openapi.py
 web/server/settings.py
 web/server/sse.py
 web/server/utils.py
+web/server/watcher.py
 web/server/api/__init__.py
 web/server/api/endpoints/__init__.py
 web/server/api/endpoints/commands.py
 web/server/api/endpoints/context.py
 web/server/api/endpoints/directories.py
 web/server/api/endpoints/environments.py
 web/server/api/endpoints/events.py
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.6.0/sqlmesh.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,10 +60,10 @@
 redshift_connector
 
 [snowflake]
 snowflake-connector-python[pandas]
 
 [web]
 fastapi==0.95.0
-hyperscript==0.0.1
+watchfiles==0.19.0
 pyarrow==11.0.0
 uvicorn==0.21.1
```

### Comparing `sqlmesh-0.5.1.dev35/sqlmesh.svg` & `sqlmesh-0.6.0/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/conftest.py` & `sqlmesh-0.6.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import typing as t
+from shutil import rmtree
 
 import duckdb
 import pytest
 from pytest_mock.plugin import MockerFixture
 from sqlglot import exp, maybe_parse
+from sqlglot.helper import ensure_list
 
 from sqlmesh.core.context import Context
 from sqlmesh.core.model import Model
 from sqlmesh.core.plan import BuiltInPlanEvaluator, Plan
 from sqlmesh.core.snapshot import Snapshot
 from sqlmesh.utils import random_id
 from sqlmesh.utils.date import TimeLike
@@ -79,14 +81,15 @@
     context.apply(plan)
     return context
 
 
 def init_and_plan_context(
     paths: str | t.List[str], mocker: MockerFixture, start: TimeLike = "1 week ago"
 ) -> t.Tuple[Context, Plan]:
+    delete_cache(paths)
     sushi_context = Context(paths=paths, config="test_config")
     confirm = mocker.patch("sqlmesh.core.console.Confirm")
     confirm.ask.return_value = False
 
     plan = sushi_context.plan("prod")
     plan.set_start(start)
 
@@ -127,7 +130,15 @@
 
     return _make_function
 
 
 @pytest.fixture
 def random_name() -> t.Callable:
     return lambda: f"generated_{random_id()}"
+
+
+def delete_cache(project_paths: str | t.List[str]) -> None:
+    for path in ensure_list(project_paths):
+        try:
+            rmtree(path + "/.cache")
+        except FileNotFoundError:
+            pass
```

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_base_postgres.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_postgres.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.6.0/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_audit.py` & `sqlmesh-0.6.0/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_config.py` & `sqlmesh-0.6.0/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_connection_config.py` & `sqlmesh-0.6.0/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_context.py` & `sqlmesh-0.6.0/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_dialect.py` & `sqlmesh-0.6.0/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_integration.py` & `sqlmesh-0.6.0/tests/core/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_macros.py` & `sqlmesh-0.6.0/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_model.py` & `sqlmesh-0.6.0/tests/core/test_model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_plan.py` & `sqlmesh-0.6.0/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_plan_evaluator.py` & `sqlmesh-0.6.0/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_scheduler.py` & `sqlmesh-0.6.0/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_schema_diff.py` & `sqlmesh-0.6.0/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_seed.py` & `sqlmesh-0.6.0/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_snapshot.py` & `sqlmesh-0.6.0/tests/core/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.6.0/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/core/test_state_sync.py` & `sqlmesh-0.6.0/tests/core/test_state_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typing as t
 
+import duckdb
 import pandas as pd
 import pytest
 from pytest_mock.plugin import MockerFixture
 from sqlglot import exp, parse_one
 
 from sqlmesh.core.context import Context
 from sqlmesh.core.engine_adapter import create_engine_adapter
@@ -441,14 +442,42 @@
         update={"data_hash": "new_snapshot_same_interval"}
     )
     new_snapshot_same_interval.add_interval("2022-01-01", "2022-01-03")
     state_sync.push_snapshots([new_snapshot_same_interval])
     promote_snapshots(state_sync, [new_snapshot_same_interval], "prod", no_gaps=True)
 
 
+def test_finalize(state_sync: EngineAdapterStateSync, make_snapshot: t.Callable):
+    snapshot_a = make_snapshot(
+        SqlModel(
+            name="a",
+            query=parse_one("select 1, ds"),
+        ),
+    )
+    snapshot_a.categorize_as(SnapshotChangeCategory.BREAKING)
+
+    state_sync.push_snapshots([snapshot_a])
+    promote_snapshots(state_sync, [snapshot_a], "prod")
+
+    env = state_sync.get_environment("prod")
+    assert env
+    state_sync.finalize(env)
+
+    env = state_sync.get_environment("prod")
+    assert env
+    assert env.finalized_ts is not None
+
+    env.plan_id = "different_plan_id"
+    with pytest.raises(
+        SQLMeshError,
+        match=r"Plan 'different_plan_id' is no longer valid for the target environment 'prod'.*",
+    ):
+        state_sync.finalize(env)
+
+
 def test_start_date_gap(state_sync: EngineAdapterStateSync, make_snapshot: t.Callable):
     model = SqlModel(
         name="a",
         query=parse_one("select 1, ds"),
         start="2022-01-01",
         kind=IncrementalByTimeRangeKind(time_column="ds"),
         cron="@daily",
@@ -565,16 +594,16 @@
 
 def test_get_version(state_sync: EngineAdapterStateSync) -> None:
     # fresh install should not raise
     assert state_sync.get_versions() == Versions(
         schema_version=SCHEMA_VERSION, sqlglot_version=SQLGLOT_VERSION
     )
 
-    # old install does not have this table / row
-    delete_versions(state_sync)
+    # Start with a clean slate.
+    state_sync = EngineAdapterStateSync(create_engine_adapter(duckdb.connect, "duckdb"))
 
     with pytest.raises(
         SQLMeshError,
         match=rf"SQLMesh \(local\) is using version '{SCHEMA_VERSION}' which is ahead of '0'",
     ):
         state_sync.get_versions()
 
@@ -622,15 +651,17 @@
 
 
 def test_migrate(state_sync: EngineAdapterStateSync, mocker: MockerFixture) -> None:
     mock = mocker.patch("sqlmesh.core.state_sync.EngineAdapterStateSync._migrate_rows")
     state_sync.migrate()
     mock.assert_not_called()
 
-    delete_versions(state_sync)
+    # Start with a clean slate.
+    state_sync = EngineAdapterStateSync(create_engine_adapter(duckdb.connect, "duckdb"))
+
     state_sync.migrate()
     mock.assert_called_once()
     assert state_sync.get_versions() == Versions(
         schema_version=SCHEMA_VERSION, sqlglot_version=SQLGLOT_VERSION
     )
```

### Comparing `sqlmesh-0.5.1.dev35/tests/dbt/conftest.py` & `sqlmesh-0.6.0/tests/dbt/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from pathlib import Path
 
 import pytest
 from pytest_mock.plugin import MockerFixture
 
 from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.project import Project
+from tests.conftest import delete_cache
 
 
 @pytest.fixture()
 def sushi_test_project(mocker: MockerFixture) -> Project:
-    project = Project.load(DbtContext(project_root=Path("tests/fixtures/dbt/sushi_test")))
+    project_root = "tests/fixtures/dbt/sushi_test"
+    delete_cache(project_root)
+    project = Project.load(DbtContext(project_root=Path(project_root)))
     for package_name, package in project.packages.items():
         project.context.jinja_macros.add_macros(
             package.macro_infos,
             package=package_name if package_name != project.context.project_name else None,
         )
     return project
```

### Comparing `sqlmesh-0.5.1.dev35/tests/dbt/test_adapter.py` & `sqlmesh-0.6.0/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/dbt/test_config.py` & `sqlmesh-0.6.0/tests/dbt/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/dbt/test_transformation.py` & `sqlmesh-0.6.0/tests/dbt/test_transformation.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/engines/spark/test_db_api.py` & `sqlmesh-0.6.0/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.6.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/migrations/environments.json` & `sqlmesh-0.6.0/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.6.0/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.6.0/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.6.0/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.6.0/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.6.0/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.6.0/tests/schedulers/airflow/test_client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.6.0/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.6.0/tests/schedulers/airflow/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
 @pytest.mark.integration
 @pytest.mark.airflow_integration
 def test_mult_snapshots_same_version(airflow_client: AirflowClient, make_snapshot, random_name):
     model_name = random_name()
 
     snapshot = make_snapshot(_create_model(model_name), version="1")
+    snapshot.change_category = SnapshotChangeCategory.BREAKING
     # Presetting the interval here to avoid backfill.
     snapshot.add_interval("2022-01-01", "2022-01-01")
     snapshot.set_unpaused_ts(now())
 
     original_fingerprint = snapshot.fingerprint
 
     environment_name = _random_environment_name()
@@ -89,14 +90,15 @@
 
     dag = _get_snapshot_dag(airflow_client, model_name, snapshot.version)
     assert dag["is_active"]
 
     new_fingerprint = original_fingerprint.copy(update={"data_hash": "new_snapshot"})
 
     snapshot.fingerprint = new_fingerprint
+    snapshot.change_category = SnapshotChangeCategory.FORWARD_ONLY
     environment.previous_plan_id = environment.plan_id
     environment.plan_id = "new_plan_id"
     _apply_plan_and_block(airflow_client, [snapshot], environment)
 
     _validate_snapshot_identifiers_for_version(
         airflow_client,
         snapshot,
```

### Comparing `sqlmesh-0.5.1.dev35/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.6.0/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_cache.py` & `sqlmesh-0.6.0/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_concurrency.py` & `sqlmesh-0.6.0/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_connection_pool.py` & `sqlmesh-0.6.0/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_dag.py` & `sqlmesh-0.6.0/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_date.py` & `sqlmesh-0.6.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_filesystem.py` & `sqlmesh-0.6.0/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_jinja.py` & `sqlmesh-0.6.0/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_metaprogramming.py` & `sqlmesh-0.6.0/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_pandas.py` & `sqlmesh-0.6.0/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_pydantic.py` & `sqlmesh-0.6.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_transactional_file.py` & `sqlmesh-0.6.0/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/utils/test_yaml.py` & `sqlmesh-0.6.0/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/tests/web/test_main.py` & `sqlmesh-0.6.0/tests/web/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,14 +484,15 @@
             "name": "prod",
             "snapshots": [],
             "start_at": 0,
             "end_at": None,
             "plan_id": "",
             "previous_plan_id": None,
             "expiration_ts": None,
+            "finalized_ts": None,
         }
     }
 
 
 def test_get_lineage(web_sushi_context: Context) -> None:
     response = client.get("/api/lineage/sushi.waiters/ds")
     assert response.status_code == 200
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/.eslintrc.js` & `sqlmesh-0.6.0/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/index.html` & `sqlmesh-0.6.0/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/openapi.json` & `sqlmesh-0.6.0/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/package-lock.json` & `sqlmesh-0.6.0/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/package.json` & `sqlmesh-0.6.0/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/playwright.config.ts` & `sqlmesh-0.6.0/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/public/favicons/favicon.ico` & `sqlmesh-0.6.0/web/client/dist/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/api/channels.ts` & `sqlmesh-0.6.0/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/api/index.ts` & `sqlmesh-0.6.0/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/api/instance.ts` & `sqlmesh-0.6.0/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.6.0/web/client/dist/assets/CircularStd-Black-52659624.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.6.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.6.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.6.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.6.0/web/client/dist/assets/Publico-Bold-c79acd56.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.6.0/web/client/dist/assets/Publico-Medium-01b4a891.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.6.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/context/context.ts` & `sqlmesh-0.6.0/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/context/editor.ts` & `sqlmesh-0.6.0/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/context/fileTree.ts` & `sqlmesh-0.6.0/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/context/plan.ts` & `sqlmesh-0.6.0/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/context/theme.tsx` & `sqlmesh-0.6.0/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.6.0/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/index.css` & `sqlmesh-0.6.0/web/client/src/index.css`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     --color-accent: hsla(264, 100%, 60%, 1);
     --color-success: hsla(111, 66%, 55%, 1);
     --color-warning: hsla(30, 94%, 62%, 1);
     --color-danger: hsla(1, 100%, 64%, 1);
     --color-neutral: hsla(0, 0%, 50%, 1);
 
     /* Brand */
+    --color-brand-10: hsla(24, 100%, 60%, 0.1);
+    --color-brand-20: hsla(24, 100%, 60%, 0.2);
+    --color-brand-30: hsla(24, 100%, 60%, 0.3);
+    --color-brand-40: hsla(24, 100%, 60%, 0.4);
     --color-brand-100: hsla(37, 100%, 92%, 1);
     --color-brand-200: hsla(34, 100%, 84%, 1);
     --color-brand-300: hsla(31, 100%, 76%, 1);
     --color-brand-400: hsla(27, 100%, 70%, 1);
     --color-brand-500: var(--color-brand);
     --color-brand-600: hsla(20, 72%, 50%, 1);
     --color-brand-700: hsla(16, 76%, 41%, 1);
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.6.0/web/client/src/library/components/editor/Editor.css`

 * *Files 26% similar despite different names*

```diff
@@ -41,25 +41,48 @@
 }
 
 .cm-editor .cm-scroller::-webkit-scrollbar-thumb {
   background: var(--color-brand);
   border-radius: 1rem;
 }
 
-.sqlmesh-model {
+.cm-tooltip {
+  border: none !important;
+  outline: none !important;
+  background: var(--color-theme) !important;
+}
+
+.sqlmesh-model,
+.sqlmesh-model > span {
+  display: inline-block;
   color: var(--color-primary-500);
   background: var(--color-primary-10);
   box-shadow: inset 0 -2px 0 0 var(--color-primary-300);
-  display: inline-block;
   cursor: pointer;
   font-weight: bold;
 }
 
-.cm-tooltip {
-  border: none !important;
-  outline: none !important;
-  background: var(--color-theme) !important;
-}
-
 .sqlmesh-model:hover {
   opacity: 0.8;
 }
+
+.sqlmesh-model.--is-active-model,
+.sqlmesh-model.--is-active-model:hover,
+.sqlmesh-model.--is-active-model > span,
+.sqlmesh-model.--is-active-model:hover > span {
+  box-shadow: none;
+  cursor: default;
+  opacity: 1;
+}
+
+.sqlmesh-model__column.--is-original,
+.sqlmesh-model__column.--is-original > span {
+  display: inline-block;
+  color: var(--color-accent-300);
+}
+
+.sqlmesh-model__column.--is-active-model.--is-derived,
+.sqlmesh-model__column.--is-active-model.--is-derived > span {
+  display: inline-block;
+  color: var(--color-brand-300);
+  background: var(--color-brand-10);
+}
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/editor/Editor.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -40,23 +40,31 @@
     }
 
     if (e.data.topic === 'dialects') {
       setDialects(e.data.payload.dialects ?? [])
     }
   }, [])
 
-  const sizesCodeEditorAndInspector = useMemo(
-    () => getSizesCodeEditorAndInspector(),
-    [tab],
-  )
-
-  const sizesCodeEditorAndPreview = useMemo(
-    () => getSizesCodeEditorAndPreview(),
-    [tab, previewConsole, previewTable],
-  )
+  const sizesCodeEditorAndInspector = useMemo(() => {
+    const showInspector =
+      tab != null &&
+      (tab.file.isSQLMeshModel || tab.file.isLocal) &&
+      isFalse(isStringEmptyOrNil(tab.file.content))
+
+    return showInspector ? [75, 25] : [100, 0]
+  }, [tab])
+
+  const sizesCodeEditorAndPreview = useMemo(() => {
+    const showPreview =
+      tab != null &&
+      ((tab.file.isLocal && [previewTable, previewConsole].some(Boolean)) ||
+        tab.file.isSQLMeshModel)
+
+    return showPreview ? [70, 30] : [100, 0]
+  }, [tab, previewConsole, previewTable])
 
   useEffect(() => {
     engine.postMessage({
       topic: 'dialects',
     })
 
     engine.addEventListener('message', handleEngineWorkerMessage)
@@ -82,31 +90,14 @@
 
   useEffect(() => {
     if (selectedFile == null || tab?.file === selectedFile) return
 
     selectTab(createTab(selectedFile))
   }, [selectedFile])
 
-  function getSizesCodeEditorAndPreview(): [number, number] {
-    const showPreview =
-      tab != null &&
-      ((tab.file.isLocal && [previewTable, previewConsole].some(Boolean)) ||
-        tab.file.isSQLMeshModel)
-    return showPreview ? [80, 20] : [100, 0]
-  }
-
-  function getSizesCodeEditorAndInspector(): [number, number] {
-    const showInspector =
-      tab != null &&
-      (tab.file.isSQLMeshModel || tab.file.isLocal) &&
-      isFalse(isStringEmptyOrNil(tab.file.content))
-
-    return showInspector ? [75, 25] : [100, 0]
-  }
-
   function toggleDirection(): void {
     setDirection(direction =>
       direction === 'vertical' ? 'horizontal' : 'vertical',
     )
   }
 
   return (
@@ -127,15 +118,20 @@
             direction === 'vertical' ? 'flex flex-col' : 'flex',
           )}
           sizes={sizesCodeEditorAndPreview}
           direction={direction}
           minSize={0}
           snapOffset={0}
         >
-          <div className="flex flex-col h-full overflow-hidden">
+          <div
+            className={clsx(
+              'flex flex-col overflow-hidden',
+              direction === 'vertical' ? 'w-full ' : 'h-full',
+            )}
+          >
             {isReadyEngine && (
               <>
                 <div className="flex flex-col h-full overflow-hidden">
                   <SplitPane
                     className="flex h-full"
                     sizes={sizesCodeEditorAndInspector}
                     minSize={0}
@@ -152,17 +148,22 @@
                 <Divider />
                 <div className="px-2 flex justify-between items-center min-h-[2rem]">
                   <EditorFooter tab={tab} />
                 </div>
               </>
             )}
           </div>
-          <div className="w-full">
+          <div
+            className={clsx(
+              direction === 'vertical' ? 'flex flex-col' : 'flex',
+            )}
+          >
             {tab != null && (
               <EditorPreview
+                key={tab.file.id}
                 tab={tab}
                 toggleDirection={toggleDirection}
               />
             )}
           </div>
         </SplitPane>
       )}
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,25 @@
   debounceSync,
   isFalse,
   isStringEmptyOrNil,
 } from '~/utils'
 import { isCancelledError, useQueryClient } from '@tanstack/react-query'
 import { useStoreContext } from '~/context/context'
 import { type EditorTab, useStoreEditor } from '~/context/editor'
+import { EnumFileExtensions } from '@models/file'
 
 export default function CodeEditor({ tab }: { tab: EditorTab }): JSX.Element {
   const { mode } = useColorScheme()
   const [SqlMeshDialect, SqlMeshDialectCleanUp] = useSqlMeshExtension()
 
   const models = useStoreContext(s => s.models)
-
   const files = useStoreFileTree(s => s.files)
   const selectFile = useStoreFileTree(s => s.selectFile)
 
+  const previewLineage = useStoreEditor(s => s.previewLineage)
   const tabs = useStoreEditor(s => s.tabs)
   const dialects = useStoreEditor(s => s.dialects)
   const engine = useStoreEditor(s => s.engine)
   const refreshTab = useStoreEditor(s => s.refreshTab)
   const closeTab = useStoreEditor(s => s.closeTab)
   const selectTab = useStoreEditor(s => s.selectTab)
   const createTab = useStoreEditor(s => s.createTab)
@@ -69,26 +70,43 @@
 
   const dialectsTitles = useMemo(
     () => dialects.map(d => d.dialect_title),
     [dialects],
   )
 
   const extensions = useMemo(() => {
+    const model = models.get(tab.file.path)
+    const columns = new Set(
+      Object.keys(previewLineage ?? {})
+        .map(modelName => models.get(modelName)?.columns.map(c => c.name))
+        .flat()
+        .filter(Boolean) as string[],
+    )
+
     return [
       mode === EnumColorScheme.Dark ? dracula : tomorrow,
       HoverTooltip(models),
       events(models, files, selectFile),
-      SqlMeshModel(models),
-      tab.file.extension === '.py' && python(),
-      tab.file.extension === '.yaml' && StreamLanguage.define(yaml),
-      tab.file.extension === '.sql' &&
+      model != null && SqlMeshModel(models, model, columns),
+      tab.file.extension === EnumFileExtensions.Python && python(),
+      tab.file.extension === EnumFileExtensions.YAML &&
+        StreamLanguage.define(yaml),
+      tab.file.extension === EnumFileExtensions.SQL &&
         tab.dialectOptions != null &&
         SqlMeshDialect(models, tab.file, tab.dialectOptions, dialectsTitles),
     ].filter(Boolean) as Extension[]
-  }, [tab.file, tab.dialectOptions, models, mode, files, dialectsTitles])
+  }, [
+    tab.file,
+    tab.dialectOptions,
+    models,
+    mode,
+    files,
+    dialectsTitles,
+    previewLineage,
+  ])
 
   const keymaps = useMemo(
     () => [
       {
         key: 'Mod-Alt-[',
         preventDefault: true,
         run() {
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 } from '@tanstack/react-table'
 import { debounceAsync, isNil, isTrue } from '~/utils'
 import { type EditorTab, useStoreEditor, type Lineage } from '~/context/editor'
 import { ViewColumnsIcon } from '@heroicons/react/24/solid'
 import { Button } from '@components/button/Button'
 import { EnumVariant } from '~/types/enum'
 import { useStoreContext } from '@context/context'
-import { apiCancelLineage, useApiModelLineage } from '@api/index'
-import Graph from '@components/graph/Graph'
-import { useQueryClient } from '@tanstack/react-query'
+import { useApiModelLineage } from '@api/index'
 import Loading from '@components/loading/Loading'
+import Graph from '@components/graph/Graph'
 
 export const EnumEditorPreviewTabs = {
   Query: 'Query',
   Table: 'Table',
   Console: 'Console',
   Lineage: 'Lineage',
 } as const
@@ -36,14 +35,15 @@
   const models = useStoreContext(s => s.models)
 
   const previewQuery = useStoreEditor(s => s.previewQuery)
   const previewConsole = useStoreEditor(s => s.previewConsole)
   const previewTable = useStoreEditor(s => s.previewTable)
 
   const [activeTabIndex, setActiveTabIndex] = useState(-1)
+  const [modelName, setModelName] = useState<string | undefined>()
 
   const tabs = useMemo(() => {
     if (tab.file.isLocal)
       return [
         EnumEditorPreviewTabs.Table,
         EnumEditorPreviewTabs.Query,
         EnumEditorPreviewTabs.Console,
@@ -54,14 +54,15 @@
         EnumEditorPreviewTabs.Query,
         EnumEditorPreviewTabs.Console,
         EnumEditorPreviewTabs.Lineage,
       ]
 
     return [EnumEditorPreviewTabs.Console]
   }, [tab])
+
   const [headers, data] = useMemo(
     () =>
       previewTable == null
         ? [[], []]
         : [previewTable[0] ?? [], previewTable[1] ?? []],
     [previewTable],
   )
@@ -84,14 +85,18 @@
     [previewTable, previewQuery, previewConsole],
   )
 
   useEffect(() => {
     setActiveTabIndex(tab.file.isSQLMeshModel ? 3 : -1)
   }, [previewTable, previewQuery, previewConsole, tab])
 
+  useEffect(() => {
+    setModelName(models.get(tab.file.path)?.name)
+  }, [models, tab.file])
+
   const table = useReactTable({
     data,
     columns,
     getCoreRowModel: getCoreRowModel(),
   })
 
   function isDisabledPreviewTable(tabName: string): boolean {
@@ -102,16 +107,14 @@
     return tabName === EnumEditorPreviewTabs.Console && isNil(previewConsole)
   }
 
   function isDisabledPreviewQuery(tabName: string): boolean {
     return tabName === EnumEditorPreviewTabs.Query && isNil(previewQuery)
   }
 
-  const model = models.get(tab.file.path)
-
   return (
     <div
       className={clsx(
         'w-full h-full flex flex-col text-prose overflow-auto scrollbar scrollbar--vertical',
       )}
     >
       <Tab.Group
@@ -258,72 +261,72 @@
             </pre>
           </Tab.Panel>
           <Tab.Panel
             className={clsx(
               'w-full h-full ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2 p-2',
             )}
           >
-            {model == null ? (
+            {modelName == null ? (
               <div>Model Does Not Exist</div>
             ) : (
               <EditorPreviewLineage
-                key={model.name}
-                model={model.name}
+                key={modelName}
+                model={modelName}
+                tab={tab}
               />
             )}
           </Tab.Panel>
         </Tab.Panels>
       </Tab.Group>
     </div>
   )
 }
 
-function EditorPreviewLineage({ model }: { model: string }): JSX.Element {
-  const client = useQueryClient()
-
-  const { data: dag, refetch: getModelLineage } = useApiModelLineage(model)
+function EditorPreviewLineage({
+  model,
+  tab,
+}: {
+  model: string
+  tab: EditorTab
+}): JSX.Element {
+  const { data: lineage, refetch: getModelLineage } = useApiModelLineage(model)
 
   const previewLineage = useStoreEditor(s => s.previewLineage)
   const setPreviewLineage = useStoreEditor(s => s.setPreviewLineage)
 
   const debouncedGetModelLineage = useCallback(
     debounceAsync(getModelLineage, 1000, true),
-    [model],
+    [model, tab.file.path, tab.file.fingerprint],
   )
 
   useEffect(() => {
     void debouncedGetModelLineage()
-
-    return () => {
-      debouncedGetModelLineage.cancel()
-
-      apiCancelLineage(client)
-    }
-  }, [model])
+  }, [debouncedGetModelLineage])
 
   useEffect(() => {
-    if (dag == null) {
+    if (lineage == null) {
       setPreviewLineage(undefined)
     } else {
       setPreviewLineage(
-        Object.keys(dag).reduce((acc: Record<string, Lineage>, key) => {
+        Object.keys(lineage).reduce((acc: Record<string, Lineage>, key) => {
           acc[key] = {
-            models: dag[key] ?? [],
+            models: lineage[key] ?? [],
+            columns: previewLineage?.[key]?.columns ?? undefined,
           }
 
           return acc
         }, {}),
       )
     }
-  }, [dag])
+  }, [lineage])
 
   return previewLineage == null ? (
     <div className="w-full h-full flex items-center justify-center bg-primary-10">
       <Loading hasSpinner>Loading Lineage...</Loading>
     </div>
   ) : (
     <Graph
-      graph={previewLineage}
+      lineage={previewLineage}
       highlightedNodes={[model]}
     />
   )
 }
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import { useMemo, type MouseEvent } from 'react'
 import { PlusIcon, XCircleIcon } from '@heroicons/react/24/solid'
 import { EnumSize, EnumVariant } from '~/types/enum'
 import { Button } from '../button/Button'
 import clsx from 'clsx'
 import { type EditorTab, useStoreEditor } from '~/context/editor'
+import { useStoreLineage, useStoreReactFlow } from '@context/lineage'
 
 export default function EditorTabs(): JSX.Element {
   const tabs = useStoreEditor(s => s.tabs)
   const selectTab = useStoreEditor(s => s.selectTab)
   const createTab = useStoreEditor(s => s.createTab)
 
   const [tabsLocal, tabsRemote] = useMemo(() => {
@@ -66,26 +67,31 @@
 }
 
 function Tab({ tab, title }: { tab: EditorTab; title: string }): JSX.Element {
   const activeTab = useStoreEditor(s => s.tab)
   const selectTab = useStoreEditor(s => s.selectTab)
   const closeTab = useStoreEditor(s => s.closeTab)
 
+  const clearActiveEdges = useStoreLineage(s => s.clearActiveEdges)
+  const clearNodesAndEdges = useStoreReactFlow(s => s.clearNodesAndEdges)
+
   function closeEditorTab(tab: EditorTab): void {
     closeTab(tab.file)
   }
 
   return (
     <li
       className={clsx(
         'inline-block py-1 pr-2 last-child:pr-0 overflow-hidden text-center overflow-ellipsis cursor-pointer',
       )}
       onClick={(e: MouseEvent) => {
         e.stopPropagation()
 
+        clearActiveEdges()
+        clearNodesAndEdges()
         selectTab(tab)
       }}
     >
       <span
         className={clsx(
           'flex border-2 justify-between items-center pl-2 pr-1 py-[0.125rem] min-w-[8rem] rounded-md group border-transparent border-r border-r-theme-darker dark:border-r-theme-lighter',
           tab.file.id === activeTab?.file.id
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.6.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files 3% similar despite different names*

```diff
@@ -124,22 +124,21 @@
 
             return await completeFromList(suggestions)(ctx)
           },
         }),
       ])
     }
 
-  const SqlMeshDialectCleanUp: ExtensionCleanUp =
-    function SqlMeshDialectCleanUp(): void {
-      const handler = cache.get('message')
+  function SqlMeshDialectCleanUp(): void {
+    const handler = cache.get('message')
 
-      if (handler == null) return
+    if (handler == null) return
 
-      sqlglotWorker.removeEventListener('message', handler)
-    }
+    sqlglotWorker.removeEventListener('message', handler)
+  }
 
   return [SqlMeshDialectExtension, SqlMeshDialectCleanUp]
 }
 
 function SQLMeshModelKeywords(
   dialects: string[] = [],
 ): Map<string, Completion[]> {
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.6.0/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.6.0/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.6.0/web/client/src/library/components/graph/help.ts`

 * *Files 16% similar despite different names*

```diff
@@ -2,64 +2,71 @@
 import { isArrayNotEmpty, isFalse, isNil, isObjectEmpty } from '../../../utils'
 import { type Model } from '@api/client'
 import { Position, type Edge, type Node, type XYPosition } from 'reactflow'
 import { type Lineage } from '@context/editor'
 
 export interface GraphNodeData {
   label: string
-  isHighlighted: boolean
-  isInteractive: boolean
+  isHighlighted?: boolean
+  isInteractive?: boolean
   [key: string]: any
 }
 
 const elk = new ELK()
 
 const NODE_WIDTH = 172
 const NODE_HEIGHT = 32
 
 export function getNodesAndEdges({
   lineage,
   highlightedNodes,
   models,
   nodes = [],
+  edges = [],
 }: {
   lineage: Record<string, Lineage>
   highlightedNodes: string[]
   models: Map<string, Model>
-  nodes: Node[]
+  nodes?: Node[]
+  edges?: Edge[]
 }): {
   nodesMap: Record<string, Node>
   edges: Edge[]
   nodes: Node[]
   columns: Record<string, { ins: string[]; outs: string[] }>
 } {
+  const currentEdges = edges.reduce(
+    (acc: Record<string, Edge>, edge) =>
+      Object.assign(acc, { [edge.id]: edge }),
+    {},
+  )
   const targets = new Set(
     Object.values(lineage)
       .map(l => l.models)
       .flat(),
   )
   const modelNames = Object.keys(lineage)
   const nodesMap = getNodeMap(
     modelNames,
     lineage,
     highlightedNodes,
     models,
     targets,
     nodes,
   )
-  const edges: Edge[] = []
+  const outputEdges: Edge[] = []
   const columns: Record<string, { ins: string[]; outs: string[] }> = {}
 
   for (const modelSource of modelNames) {
     const modelLineage = lineage[modelSource]
 
     if (modelLineage == null) continue
 
     modelLineage.models.forEach(modelTarget => {
-      edges.push(createGraphEdge(modelSource, modelTarget))
+      outputEdges.push(createGraphEdge(modelSource, modelTarget))
     })
 
     if (modelLineage.columns == null || isObjectEmpty(modelLineage.columns))
       continue
 
     for (const columnSource in modelLineage.columns) {
       const sourceId = toNodeOrEdgeId(modelSource, columnSource)
@@ -88,36 +95,55 @@
               outs: [],
             }
           }
 
           columns[sourceId]?.ins.push(targetId)
           columns[targetId]?.outs.push(sourceId)
 
-          edges.push(
-            createGraphEdge(
-              modelSource,
-              modelTarget,
-              toNodeOrEdgeId('source', modelSource, columnSource),
-              toNodeOrEdgeId('target', modelTarget, columnTarget),
-              false,
-              {
-                target: modelTarget,
-                source: modelSource,
-                columnSource,
-                columnTarget,
-              },
-            ),
+          const sourceHandle = toNodeOrEdgeId(
+            'source',
+            modelSource,
+            columnSource,
+          )
+          const targetHandle = toNodeOrEdgeId(
+            'target',
+            modelTarget,
+            columnTarget,
+          )
+          const edgeId = toNodeOrEdgeId(
+            modelSource,
+            modelTarget,
+            sourceHandle,
+            targetHandle,
+          )
+          const currentEdge = currentEdges[edgeId]
+
+          outputEdges.push(
+            currentEdge ??
+              createGraphEdge(
+                modelSource,
+                modelTarget,
+                sourceHandle,
+                targetHandle,
+                false,
+                {
+                  target: modelTarget,
+                  source: modelSource,
+                  columnSource,
+                  columnTarget,
+                },
+              ),
           )
         }
       }
     }
   }
 
   return {
-    edges,
+    edges: outputEdges,
     nodes: Object.values(nodesMap),
     nodesMap,
     columns,
   }
 }
 
 export async function createGraphLayout({
@@ -165,22 +191,23 @@
   )
 
   return modelNames.reduce((acc: Record<string, Node>, label: string) => {
     const node =
       current[label] ??
       createGraphNode({
         label,
-        isHighlighted: highlightedNodes.includes(label),
-        isInteractive:
-          isArrayNotEmpty(highlightedNodes) &&
-          isFalse(highlightedNodes.includes(label)),
         width: NODE_WIDTH,
         height: NODE_HEIGHT + 32 * (models.get(label)?.columns?.length ?? 0),
       })
 
+    node.data.isHighlighted = highlightedNodes.includes(label)
+    node.data.isInteractive =
+      isArrayNotEmpty(highlightedNodes) &&
+      isFalse(highlightedNodes.includes(label))
+
     if (isArrayNotEmpty(lineage[node.id]?.models)) {
       node.sourcePosition = Position.Left
     }
 
     if (targets.has(node.id)) {
       node.targetPosition = Position.Right
     }
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/ide/IDE.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
   ])
   const debouncedGetModels = useCallback(debounceAsync(getModels, 1000, true), [
     getModels,
   ])
 
   useEffect(() => {
     const unsubscribeTasks = subscribe('tasks', updateTasks)
+    const unsubscribeModels = subscribe('models', setModels)
 
     void debouncedGetEnvironemnts()
     void debouncedGetFiles()
     void debouncedGetModels()
 
     return () => {
       debouncedGetEnvironemnts.cancel()
@@ -73,14 +74,15 @@
       debouncedGetModels.cancel()
 
       apiCancelModels(client)
       apiCancelFiles(client)
       apiCancelGetEnvironments(client)
 
       unsubscribeTasks?.()
+      unsubscribeModels?.()
     }
   }, [])
 
   useEffect(() => {
     if (
       contextEnvironemnts == null ||
       isArrayEmpty(Object.keys(contextEnvironemnts))
@@ -117,15 +119,14 @@
         </div>
       </div>
       <Divider />
       {environment != null && (
         <SplitPane
           sizes={[20, 80]}
           minSize={[160]}
-          maxSize={[320]}
           snapOffset={0}
           className="flex w-full h-full overflow-hidden"
         >
           <FileTree project={project} />
           <Editor />
         </SplitPane>
       )}
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.6.0/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.6.0/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.6.0/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/report/ReportTestsErrors.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/report/ReportTestsErrors.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.6.0/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.6.0/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/main.tsx` & `sqlmesh-0.6.0/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/models/artifact.ts` & `sqlmesh-0.6.0/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/models/directory.ts` & `sqlmesh-0.6.0/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/models/environment.ts` & `sqlmesh-0.6.0/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/models/file.ts` & `sqlmesh-0.6.0/web/client/src/models/file.ts`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import { type File, FileType } from '../api/client'
 import { type ModelDirectory } from './directory'
 import { type InitialArtifact, ModelArtifact } from './artifact'
 import { isStringEmptyOrNil } from '@utils/index'
 
+export const EnumFileExtensions = {
+  SQL: '.sql',
+  Python: '.py',
+  CSV: '.csv',
+  YAML: '.yaml',
+} as const
+
 export interface InitialFile extends InitialArtifact, File {
   content: string
   extension: string
   is_supported: boolean
 }
 
 export class ModelFile extends ModelArtifact<InitialFile> {
@@ -19,15 +26,15 @@
 
   constructor(initial?: File | ModelFile, parent?: ModelDirectory) {
     super(
       (initial as ModelFile)?.isModel
         ? (initial as ModelFile).initial
         : {
             ...(initial as File),
-            extension: initial?.extension ?? '.sql',
+            extension: initial?.extension ?? EnumFileExtensions.SQL,
             is_supported: initial?.is_supported ?? true,
             content: initial?.content ?? '',
           },
       parent,
     )
 
     this.extension = initial?.extension ?? this.initial.extension
@@ -48,14 +55,26 @@
     return this.content !== this._content
   }
 
   get isSQLMeshModel(): boolean {
     return this.type === 'model'
   }
 
+  get fingerprint(): string {
+    return this._content
+  }
+
+  get isSQLMeshModelPython(): boolean {
+    return this.isSQLMeshModel && this.extension === EnumFileExtensions.Python
+  }
+
+  get isSQLMeshModelSQL(): boolean {
+    return this.isSQLMeshModel && this.extension === EnumFileExtensions.SQL
+  }
+
   updateContent(newContent: string = ''): void {
     this._content = newContent
     this.content = newContent
   }
 }
 
 function getFileType(path?: string): FileType | undefined {
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/models/initial.ts` & `sqlmesh-0.6.0/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/tests/utils.tsx` & `sqlmesh-0.6.0/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/utils/index.spec.ts` & `sqlmesh-0.6.0/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/utils/index.ts` & `sqlmesh-0.6.0/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.6.0/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.6.0/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/tailwind.config.js` & `sqlmesh-0.6.0/web/client/tailwind.config.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -39,14 +39,15 @@
                 darker: 'var(--color-theme-darker)',
                 lighter: 'var(--color-theme-lighter)',
             },
             divider: {
                 DEFAULT: 'var(--color-divider)',
             },
             brand: {
+                10: 'var(--color-brand-10)',
                 100: 'var(--color-brand-100)',
                 200: 'var(--color-brand-200)',
                 300: 'var(--color-brand-300)',
                 400: 'var(--color-brand-400)',
                 500: 'var(--color-brand-500)',
                 600: 'var(--color-brand-600)',
                 700: 'var(--color-brand-700)',
```

### Comparing `sqlmesh-0.5.1.dev35/web/client/tsconfig.json` & `sqlmesh-0.6.0/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/client/vite.config.ts` & `sqlmesh-0.6.0/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/__init__.py` & `sqlmesh-0.6.0/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/commands.py` & `sqlmesh-0.6.0/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/context.py` & `sqlmesh-0.6.0/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/directories.py` & `sqlmesh-0.6.0/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/environments.py` & `sqlmesh-0.6.0/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/events.py` & `sqlmesh-0.6.0/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/files.py` & `sqlmesh-0.6.0/web/server/api/endpoints/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,46 +83,50 @@
     )
 
 
 @router.get("/{path:path}", response_model=models.File)
 def get_file(
     path: str = Depends(validate_path),
     settings: Settings = Depends(get_settings),
-    path_mapping: t.Dict[str, t.Any] = Depends(get_path_mapping),
+    path_mapping: t.Dict[Path, models.FileType] = Depends(get_path_mapping),
 ) -> models.File:
     """Get a file, including its contents."""
     try:
         with open(settings.project_path / path) as f:
             content = f.read()
     except FileNotFoundError:
         raise HTTPException(status_code=HTTP_404_NOT_FOUND)
     return models.File(
-        name=os.path.basename(path), path=path, content=content, type=path_mapping.get(path)
+        name=os.path.basename(path), path=path, content=content, type=path_mapping.get(Path(path))
     )
 
 
 @router.post("/{path:path}", response_model=models.File)
 async def write_file(
     content: str = Body("", embed=True),
     new_path: t.Optional[str] = Body(None, embed=True),
     path: str = Depends(validate_path),
     settings: Settings = Depends(get_settings),
     context: Context = Depends(get_context),
+    path_mapping: t.Dict[Path, models.FileType] = Depends(get_path_mapping),
 ) -> models.File:
     """Create, update, or rename a file."""
     path_or_new_path = path
     if new_path:
         path_or_new_path = validate_path(new_path, context)
         replace_file(settings.project_path / path, settings.project_path / path_or_new_path)
     else:
         (settings.project_path / path_or_new_path).write_text(content, encoding="utf-8")
 
     content = (settings.project_path / path_or_new_path).read_text()
     return models.File(
-        name=os.path.basename(path_or_new_path), path=path_or_new_path, content=content
+        name=os.path.basename(path_or_new_path),
+        path=path_or_new_path,
+        content=content,
+        type=path_mapping.get(Path(path)),
     )
 
 
 @router.delete("/{path:path}")
 async def delete_file(
     response: Response,
     path: str = Depends(validate_path),
```

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/lineage.py` & `sqlmesh-0.6.0/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/models.py` & `sqlmesh-0.6.0/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/api/endpoints/plan.py` & `sqlmesh-0.6.0/web/server/api/endpoints/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 ].qualified_view_name.for_environment(plan.environment.name)
                 if interval.snapshot_name in plan.context_diff.snapshots
                 else interval.snapshot_name,
                 interval=[
                     [to_ds(t) for t in make_inclusive(start, end)]
                     for start, end in interval.merged_intervals
                 ][0],
-                batches=tasks[interval.snapshot_name],
+                batches=tasks.get(interval.snapshot_name, 0),
             )
             for interval in plan.missing_intervals
         ]
 
         payload.changes = models.ContextEnvironmentChanges(
             removed=plan.context_diff.removed,
             added=plan.context_diff.added,
```

### Comparing `sqlmesh-0.5.1.dev35/web/server/console.py` & `sqlmesh-0.6.0/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/main.py` & `sqlmesh-0.6.0/web/server/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from fastapi import FastAPI
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 
 from web.server.api.endpoints import api_router
 from web.server.console import ApiConsole
+from web.server.watcher import watch_project
 
 app = FastAPI()
 api_console = ApiConsole()
 
 app.include_router(api_router, prefix="/api")
 WEB_DIRECTORY = pathlib.Path(__file__).parent.parent
 
@@ -22,19 +23,21 @@
             item = await api_console.queue.get()
             for listener in app.state.console_listeners:
                 await listener.put(item)
             api_console.queue.task_done()
 
     app.state.console_listeners = []
     app.state.dispatch_task = asyncio.create_task(dispatch())
+    app.state.watch_task = asyncio.create_task(watch_project(api_console.queue))
 
 
 @app.on_event("shutdown")
 def shutdown_event() -> None:
     app.state.dispatch_task.cancel()
+    app.state.watch_task.cancel()
 
 
 @app.get("/health")
 def health() -> str:
     return "ok"
```

### Comparing `sqlmesh-0.5.1.dev35/web/server/models.py` & `sqlmesh-0.6.0/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/settings.py` & `sqlmesh-0.6.0/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/sse.py` & `sqlmesh-0.6.0/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev35/web/server/utils.py` & `sqlmesh-0.6.0/web/server/utils.py`

 * *Files identical despite different names*

