# Comparing `tmp/fastapi_template-4.1.2.tar.gz` & `tmp/fastapi_template-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_template-4.1.2.tar", max compression
+gzip compressed data, was "fastapi_template-4.1.3.tar", max compression
```

## Comparing `fastapi_template-4.1.2.tar` & `fastapi_template-4.1.3.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0     1069 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/LICENSE
--rw-r--r--   0        0        0     4288 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/__init__.py
--rw-r--r--   0        0        0     1170 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/__main__.py
--rw-r--r--   0        0        0    20614 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/cli.py
--rw-r--r--   0        0        0     7913 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/input_model.py
--rw-r--r--   0        0        0     1194 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/hooks/__init__.py
--rw-r--r--   0        0        0     2583 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/hooks/post_gen_project.py
--rw-r--r--   0        0        0       28 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/hooks/pre_gen_project.py
--rw-r--r--   0        0        0     2086 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      463 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.editorconfig
--rw-r--r--   0        0        0      272 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.env
--rw-r--r--   0        0        0     2386 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     5369 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml
--rw-r--r--   0        0        0     2070 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     3206 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml
--rw-r--r--   0        0        0     1743 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7207 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      960 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini
--rw-r--r--   0        0        0     8623 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json
--rw-r--r--   0        0        0      918 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile
--rw-r--r--   0        0        0      543 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml
--rw-r--r--   0        0        0      565 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml
--rw-r--r--   0        0        0     8135 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml
--rw-r--r--   0        0        0     2718 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml
--rw-r--r--   0        0        0     3002 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml
--rw-r--r--   0        0        0       87 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/namespace.yml
--rw-r--r--   0        0        0     1242 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml
--rw-r--r--   0        0        0     1022 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml
--rw-r--r--   0        0        0      509 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/otel-collector-config.yml
--rw-r--r--   0        0        0     6563 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      305 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/replaceable_files.json
--rw-r--r--   0        0        0       45 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0     1659 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py
--rw-r--r--   0        0        0    13920 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py
--rw-r--r--   0        0        0      255 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/base.py
--rw-r--r--   0        0        0      135 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/config.py
--rw-r--r--   0        0        0       19 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/__init__.py
--rw-r--r--   0        0        0     1119 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py
--rw-r--r--   0        0        0       46 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/meta.py
--rw-r--r--   0        0        0       26 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/__init__.py
--rw-r--r--   0        0        0     2310 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py
--rw-r--r--   0        0        0      510 2023-04-23 16:19:38.515960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/script.py.mako
--rw-r--r--   0        0        0      302 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
--rw-r--r--   0        0        0      800 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py
--rw-r--r--   0        0        0        0 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/__init__.py
--rw-r--r--   0        0        0      421 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/__init__.py
--rw-r--r--   0        0        0      309 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/dummy_model.py
--rw-r--r--   0        0        0     2790 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py
--rw-r--r--   0        0        0      533 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py
--rw-r--r--   0        0        0       42 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/__init__.py
--rw-r--r--   0        0        0     1113 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py
--rw-r--r--   0        0        0     1068 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py
--rw-r--r--   0        0        0        0 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/__init__.py
--rw-r--r--   0        0        0       44 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/__init__.py
--rw-r--r--   0        0        0      177 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/dummy_model.py
--rw-r--r--   0        0        0     2693 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py
--rw-r--r--   0        0        0      490 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dependencies.py
--rw-r--r--   0        0        0      124 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/models/dummy_model.py
--rw-r--r--   0        0        0      184 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/base.py
--rw-r--r--   0        0        0       19 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/__init__.py
--rw-r--r--   0        0        0     1562 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py
--rw-r--r--   0        0        0      687 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py
--rw-r--r--   0        0        0       46 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/meta.py
--rw-r--r--   0        0        0       26 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/__init__.py
--rw-r--r--   0        0        0     2487 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py
--rw-r--r--   0        0        0      510 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/script.py.mako
--rw-r--r--   0        0        0      302 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
--rw-r--r--   0        0        0      819 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py
--rw-r--r--   0        0        0        0 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/__init__.py
--rw-r--r--   0        0        0      421 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/__init__.py
--rw-r--r--   0        0        0      392 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/dummy_model.py
--rw-r--r--   0        0        0     3018 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py
--rw-r--r--   0        0        0      567 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py
--rw-r--r--   0        0        0       19 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/__init__.py
--rw-r--r--   0        0        0     1081 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py
--rw-r--r--   0        0        0      261 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_mysql.sql
--rw-r--r--   0        0        0      228 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_pg.sql
--rw-r--r--   0        0        0      242 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_sqlite.sql
--rw-r--r--   0        0        0      239 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_mysql.sql
--rw-r--r--   0        0        0      231 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_pg.sql
--rw-r--r--   0        0        0      216 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_sqlite.sql
--rw-r--r--   0        0        0       48 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/__init__.py
--rw-r--r--   0        0        0      255 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/dummy_model.py
--rw-r--r--   0        0        0     3497 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py
--rw-r--r--   0        0        0      676 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py
--rw-r--r--   0        0        0       50 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/__init__.py
--rw-r--r--   0        0        0       21 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/__init__.py
--rw-r--r--   0        0        0      491 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/dependencies.py
--rw-r--r--   0        0        0      962 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py
--rw-r--r--   0        0        0       24 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/__init__.py
--rw-r--r--   0        0        0      506 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/dependencies.py
--rw-r--r--   0        0        0     1657 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py
--rw-r--r--   0        0        0       21 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/__init__.py
--rw-r--r--   0        0        0      897 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py
--rw-r--r--   0        0        0      583 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py
--rw-r--r--   0        0        0     5098 2023-04-23 16:19:38.519960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py
--rw-r--r--   0        0        0  1034247 2023-04-23 16:19:38.527960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js
--rw-r--r--   0        0        0  1039995 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js
--rw-r--r--   0        0        0   144654 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css
--rw-r--r--   0        0        0       47 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0     3260 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py
--rw-r--r--   0        0        0     1231 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py
--rw-r--r--   0        0        0     1707 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py
--rw-r--r--   0        0        0     3291 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py
--rw-r--r--   0        0        0     3084 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py
--rw-r--r--   0        0        0      478 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_{{cookiecutter.project_name}}.py
--rw-r--r--   0        0        0     1116 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py
--rw-r--r--   0        0        0       49 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/__init__.py
--rw-r--r--   0        0        0       49 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/__init__.py
--rw-r--r--   0        0        0      127 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/__init__.py
--rw-r--r--   0        0        0     1401 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py
--rw-r--r--   0        0        0      114 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/__init__.py
--rw-r--r--   0        0        0      334 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/schema.py
--rw-r--r--   0        0        0     1254 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py
--rw-r--r--   0        0        0      106 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/__init__.py
--rw-r--r--   0        0        0      109 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/schema.py
--rw-r--r--   0        0        0      406 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/views.py
--rw-r--r--   0        0        0      125 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/__init__.py
--rw-r--r--   0        0        0      131 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/schema.py
--rw-r--r--   0        0        0      663 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py
--rw-r--r--   0        0        0      135 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/__init__.py
--rw-r--r--   0        0        0      203 2023-04-23 16:19:38.531960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/views.py
--rw-r--r--   0        0        0      129 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/__init__.py
--rw-r--r--   0        0        0      177 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/schema.py
--rw-r--r--   0        0        0     1039 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py
--rw-r--r--   0        0        0      108 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/__init__.py
--rw-r--r--   0        0        0      181 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/schema.py
--rw-r--r--   0        0        0     1273 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py
--rw-r--r--   0        0        0     1736 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py
--rw-r--r--   0        0        0     3691 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py
--rw-r--r--   0        0        0       49 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/__init__.py
--rw-r--r--   0        0        0     2530 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py
--rw-r--r--   0        0        0      207 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/__init__.py
--rw-r--r--   0        0        0     1131 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py
--rw-r--r--   0        0        0     1389 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py
--rw-r--r--   0        0        0      186 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/schema.py
--rw-r--r--   0        0        0      189 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/__init__.py
--rw-r--r--   0        0        0      350 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/mutation.py
--rw-r--r--   0        0        0      341 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/query.py
--rw-r--r--   0        0        0      136 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/__init__.py
--rw-r--r--   0        0        0      736 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py
--rw-r--r--   0        0        0      135 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/schema.py
--rw-r--r--   0        0        0      140 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/__init__.py
--rw-r--r--   0        0        0     1134 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py
--rw-r--r--   0        0        0      166 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/schema.py
--rw-r--r--   0        0        0      192 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/__init__.py
--rw-r--r--   0        0        0      870 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py
--rw-r--r--   0        0        0      867 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py
--rw-r--r--   0        0        0      273 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/schema.py
--rw-r--r--   0        0        0     1692 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py
--rw-r--r--   0        0        0    10788 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py
--rw-r--r--   0        0        0     2607 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/tests/conftest.py
--rw-r--r--   0        0        0     4293 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/tests/test_generator.py
--rw-r--r--   0        0        0     1257 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/fastapi_template/tests/utils.py
--rw-r--r--   0        0        0     1222 2023-04-23 16:19:38.535960 fastapi_template-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 fastapi_template-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/LICENSE
+-rw-r--r--   0        0        0     4288 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/__init__.py
+-rw-r--r--   0        0        0     1170 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/__main__.py
+-rw-r--r--   0        0        0    20614 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/cli.py
+-rw-r--r--   0        0        0     7913 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/input_model.py
+-rw-r--r--   0        0        0     1194 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/hooks/__init__.py
+-rw-r--r--   0        0        0     2583 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/hooks/post_gen_project.py
+-rw-r--r--   0        0        0       28 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0     2086 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      463 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.editorconfig
+-rw-r--r--   0        0        0      272 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.env
+-rw-r--r--   0        0        0     2386 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     5369 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2070 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     3206 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1743 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7289 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      960 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini
+-rw-r--r--   0        0        0     8623 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json
+-rw-r--r--   0        0        0      988 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile
+-rw-r--r--   0        0        0      569 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml
+-rw-r--r--   0        0        0      565 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml
+-rw-r--r--   0        0        0     8154 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml
+-rw-r--r--   0        0        0     2718 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml
+-rw-r--r--   0        0        0     3002 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml
+-rw-r--r--   0        0        0       87 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/namespace.yml
+-rw-r--r--   0        0        0     1242 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml
+-rw-r--r--   0        0        0     1022 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml
+-rw-r--r--   0        0        0      509 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/otel-collector-config.yml
+-rw-r--r--   0        0        0     6563 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/replaceable_files.json
+-rw-r--r--   0        0        0       45 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0     1659 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py
+-rw-r--r--   0        0        0    13920 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py
+-rw-r--r--   0        0        0      255 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/base.py
+-rw-r--r--   0        0        0      135 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/config.py
+-rw-r--r--   0        0        0       19 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/__init__.py
+-rw-r--r--   0        0        0     1119 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py
+-rw-r--r--   0        0        0       46 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/meta.py
+-rw-r--r--   0        0        0       26 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/__init__.py
+-rw-r--r--   0        0        0     2310 2023-04-25 22:27:12.806448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/script.py.mako
+-rw-r--r--   0        0        0      302 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
+-rw-r--r--   0        0        0      800 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/__init__.py
+-rw-r--r--   0        0        0      421 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/dummy_model.py
+-rw-r--r--   0        0        0     2790 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py
+-rw-r--r--   0        0        0      533 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py
+-rw-r--r--   0        0        0       42 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/__init__.py
+-rw-r--r--   0        0        0     1113 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py
+-rw-r--r--   0        0        0     1068 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/dummy_model.py
+-rw-r--r--   0        0        0     2693 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py
+-rw-r--r--   0        0        0      490 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dependencies.py
+-rw-r--r--   0        0        0      124 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/models/dummy_model.py
+-rw-r--r--   0        0        0      184 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/base.py
+-rw-r--r--   0        0        0       19 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/__init__.py
+-rw-r--r--   0        0        0     1562 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py
+-rw-r--r--   0        0        0      687 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py
+-rw-r--r--   0        0        0       46 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/meta.py
+-rw-r--r--   0        0        0       26 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/__init__.py
+-rw-r--r--   0        0        0     2487 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/script.py.mako
+-rw-r--r--   0        0        0      302 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
+-rw-r--r--   0        0        0      819 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/__init__.py
+-rw-r--r--   0        0        0      421 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/__init__.py
+-rw-r--r--   0        0        0      392 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/dummy_model.py
+-rw-r--r--   0        0        0     3018 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py
+-rw-r--r--   0        0        0      567 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py
+-rw-r--r--   0        0        0       19 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/__init__.py
+-rw-r--r--   0        0        0     1081 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py
+-rw-r--r--   0        0        0      261 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_mysql.sql
+-rw-r--r--   0        0        0      228 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_pg.sql
+-rw-r--r--   0        0        0      242 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_sqlite.sql
+-rw-r--r--   0        0        0      239 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_mysql.sql
+-rw-r--r--   0        0        0      231 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_pg.sql
+-rw-r--r--   0        0        0      216 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_sqlite.sql
+-rw-r--r--   0        0        0       48 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/__init__.py
+-rw-r--r--   0        0        0      255 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/dummy_model.py
+-rw-r--r--   0        0        0     3497 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py
+-rw-r--r--   0        0        0      676 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py
+-rw-r--r--   0        0        0       50 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/__init__.py
+-rw-r--r--   0        0        0      491 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/dependencies.py
+-rw-r--r--   0        0        0      962 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py
+-rw-r--r--   0        0        0       24 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/__init__.py
+-rw-r--r--   0        0        0      506 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/dependencies.py
+-rw-r--r--   0        0        0     1657 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py
+-rw-r--r--   0        0        0       21 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py
+-rw-r--r--   0        0        0      583 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py
+-rw-r--r--   0        0        0     5098 2023-04-25 22:27:12.810448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py
+-rw-r--r--   0        0        0  1034247 2023-04-25 22:27:12.814448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js
+-rw-r--r--   0        0        0  1039995 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   144654 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css
+-rw-r--r--   0        0        0       47 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0     3260 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py
+-rw-r--r--   0        0        0     1231 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py
+-rw-r--r--   0        0        0     1707 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py
+-rw-r--r--   0        0        0     3291 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py
+-rw-r--r--   0        0        0     3084 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py
+-rw-r--r--   0        0        0      478 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_{{cookiecutter.project_name}}.py
+-rw-r--r--   0        0        0     1116 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py
+-rw-r--r--   0        0        0       49 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/__init__.py
+-rw-r--r--   0        0        0      127 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/__init__.py
+-rw-r--r--   0        0        0     1401 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py
+-rw-r--r--   0        0        0      114 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/schema.py
+-rw-r--r--   0        0        0     1254 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py
+-rw-r--r--   0        0        0      106 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/schema.py
+-rw-r--r--   0        0        0      406 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/views.py
+-rw-r--r--   0        0        0      125 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/schema.py
+-rw-r--r--   0        0        0      663 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py
+-rw-r--r--   0        0        0      135 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/views.py
+-rw-r--r--   0        0        0      129 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/schema.py
+-rw-r--r--   0        0        0     1039 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py
+-rw-r--r--   0        0        0      108 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/__init__.py
+-rw-r--r--   0        0        0      181 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/schema.py
+-rw-r--r--   0        0        0     1273 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py
+-rw-r--r--   0        0        0     1736 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py
+-rw-r--r--   0        0        0     3691 2023-04-25 22:27:12.822448 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py
+-rw-r--r--   0        0        0       49 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/__init__.py
+-rw-r--r--   0        0        0     2530 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py
+-rw-r--r--   0        0        0      207 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/__init__.py
+-rw-r--r--   0        0        0     1131 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py
+-rw-r--r--   0        0        0     1389 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py
+-rw-r--r--   0        0        0      186 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/schema.py
+-rw-r--r--   0        0        0      189 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/__init__.py
+-rw-r--r--   0        0        0      350 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/mutation.py
+-rw-r--r--   0        0        0      341 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/query.py
+-rw-r--r--   0        0        0      136 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py
+-rw-r--r--   0        0        0      135 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/schema.py
+-rw-r--r--   0        0        0      140 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/__init__.py
+-rw-r--r--   0        0        0     1134 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py
+-rw-r--r--   0        0        0      166 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/schema.py
+-rw-r--r--   0        0        0      192 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/__init__.py
+-rw-r--r--   0        0        0      870 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py
+-rw-r--r--   0        0        0      867 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py
+-rw-r--r--   0        0        0      273 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/schema.py
+-rw-r--r--   0        0        0     1692 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py
+-rw-r--r--   0        0        0    10788 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py
+-rw-r--r--   0        0        0     2607 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/tests/conftest.py
+-rw-r--r--   0        0        0     4293 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/tests/test_generator.py
+-rw-r--r--   0        0        0     1629 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/fastapi_template/tests/utils.py
+-rw-r--r--   0        0        0     1222 2023-04-25 22:27:12.826449 fastapi_template-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 fastapi_template-4.1.3/PKG-INFO
```

### Comparing `fastapi_template-4.1.2/LICENSE` & `fastapi_template-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/README.md` & `fastapi_template-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/__main__.py` & `fastapi_template-4.1.3/fastapi_template/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/cli.py` & `fastapi_template-4.1.3/fastapi_template/cli.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/input_model.py` & `fastapi_template-4.1.3/fastapi_template/input_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/cookiecutter.json` & `fastapi_template-4.1.3/fastapi_template/template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/hooks/post_gen_project.py` & `fastapi_template-4.1.3/fastapi_template/template/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.flake8` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.flake8`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   image: python:3.9.6-slim-buster
   tags:
     - kubernetes-runner
     - docker-runner
   except:
     - tags
   before_script:
-    - pip install poetry==1.2.2
+    - pip install poetry==1.4.2
     - poetry config virtualenvs.create false
     - poetry install
 
 black:
   extends:
     - .test-template
   script:
```

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/README.md` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 docker-compose -f deploy/docker-compose.yml --project-directory . up --build
 ```
 
 If you want to develop in docker with autoreload add `-f deploy/docker-compose.dev.yml` to your docker command.
 Like this:
 
 ```bash
-docker-compose -f deploy/docker-compose.yml -f deploy/docker-compose.dev.yml --project-directory . up
+docker-compose -f deploy/docker-compose.yml -f deploy/docker-compose.dev.yml --project-directory . up --build
 ```
 
 This command exposes the web application on port 8000, mounts current directory and enables autoreload.
 
 But you have to rebuild image every time you modify `poetry.lock` or `pyproject.toml` with this command:
 
 ```bash
@@ -206,16 +206,16 @@
 
 
 ## Running tests
 
 If you want to run it in docker, simply run:
 
 ```bash
-docker-compose -f deploy/docker-compose.yml --project-directory . run --rm api pytest -vv .
-docker-compose -f deploy/docker-compose.yml --project-directory . down
+docker-compose -f deploy/docker-compose.yml -f deploy/docker-compose.dev.yml --project-directory . run --build --rm api pytest -vv .
+docker-compose -f deploy/docker-compose.yml -f deploy/docker-compose.dev.yml --project-directory . down
 ```
 
 For running tests on your local machine.
 
 {%- if cookiecutter.db_info.name != "none" %}
 {%- if cookiecutter.db_info.name != "sqlite" %}
 1. you need to start a database.
```

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.9.6-slim-buster
+FROM python:3.9.6-slim-buster as prod
 
 {%- if cookiecutter.db_info.name == "mysql" %}
 RUN apt-get update && apt-get install -y \
   default-libmysqlclient-dev \
   gcc \
   && rm -rf /var/lib/apt/lists/*
 {%- endif %}
@@ -11,31 +11,35 @@
 {%- if cookiecutter.db_info.name == "postgresql" %}
 RUN apt-get update && apt-get install -y \
   gcc \
   && rm -rf /var/lib/apt/lists/*
 {%- endif %}
 
 
-RUN pip install poetry==1.2.2
+RUN pip install poetry==1.4.2
 
 # Configuring poetry
 RUN poetry config virtualenvs.create false
 
 # Copying requirements of a project
 COPY pyproject.toml poetry.lock /app/src/
 WORKDIR /app/src
 
 # Installing requirements
-RUN poetry install
+RUN poetry install --only main
 
 {%- if cookiecutter.db_info.name == "mysql" or cookiecutter.db_info.name == "postgresql" %}
 # Removing gcc
 RUN apt-get purge -y \
   gcc \
   && rm -rf /var/lib/apt/lists/*
 {%- endif %}
 
 # Copying actuall application
 COPY . /app/src/
-RUN poetry install
+RUN poetry install --only main
 
 CMD ["/usr/local/bin/python", "-m", "{{cookiecutter.project_name}}"]
+
+FROM prod as dev
+
+RUN poetry install
```

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 version: '3.9'
 
 services:
   api:
     ports:
       # Exposes application port.
     - "8000:8000"
+    build:
+      target: dev
     volumes:
       # Adds current directory as volume.
     - .:/app/src/
     environment:
       # Enables autoreload.
       {{cookiecutter.project_name | upper}}_RELOAD: "True"
 
@@ -17,10 +19,10 @@
   taskiq-worker:
     volumes:
       # Adds current directory as volume.
       - .:/app/src/
     command:
       - taskiq
       - worker
-      - {{cookiecutter.project_name}}.taskiq:broker
+      - {{cookiecutter.project_name}}.tkq:broker
       - --reload
   {%- endif %}
```

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 version: '3.9'
 
 services:
   api: &main_app
     build:
       context: .
       dockerfile: ./deploy/Dockerfile
+      target: prod
     image: {{cookiecutter.project_name}}:{{"${" }}{{cookiecutter.project_name | upper }}_VERSION:-latest{{"}"}}
     restart: always
     env_file:
       - .env
     {%- if cookiecutter.traefik_labels == "True" %}
     labels:
       # Enables traefik for this container.
```

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py` & `fastapi_template-4.1.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/tests/conftest.py` & `fastapi_template-4.1.3/fastapi_template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/tests/test_generator.py` & `fastapi_template-4.1.3/fastapi_template/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-4.1.2/fastapi_template/tests/utils.py` & `fastapi_template-4.1.3/fastapi_template/tests/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 import shlex
 import subprocess
 from typing import Optional
 from fastapi_template.input_model import BuilderContext
 from fastapi_template.__main__ import generate_project
 
 
@@ -35,14 +36,23 @@
             ]
         )
     return subprocess.run(docker_command)
 
 
 def run_default_check(context: BuilderContext, without_pytest=False):
     generate_project_and_chdir(context)
+    compose = Path("./deploy/docker-compose.yml")
+    compose_contents = compose.read_text()
+    new_compose_lines = []
+    for line in compose_contents.splitlines():
+        if line.strip().replace(" ", "") == "target:prod":
+            continue
+        new_compose_lines.append(line)
+    compose.write_text("\n".join(new_compose_lines) + "\n")
+
     assert run_pre_commit() == 0
 
     if without_pytest:
         return
 
     build = run_docker_compose_command("build")
     assert build.returncode == 0
```

### Comparing `fastapi_template-4.1.2/pyproject.toml` & `fastapi_template-4.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi_template"
-version = "4.1.2"
+version = "4.1.3"
 description = "Feature-rich robust FastAPI template"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 packages = [{ include = "fastapi_template" }]
 repository = "https://github.com/s3rius/FastAPI-template"
 homepage = "https://github.com/s3rius/FastAPI-template"
 readme = "README.md"
 keywords = ["FastAPI", "Cookiecutter", "Template"]
```

### Comparing `fastapi_template-4.1.2/PKG-INFO` & `fastapi_template-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-template
-Version: 4.1.2
+Version: 4.1.3
 Summary: Feature-rich robust FastAPI template
 Home-page: https://github.com/s3rius/FastAPI-template
 Keywords: FastAPI,Cookiecutter,Template
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-template Version: 4.1.2 Summary: Feature-
+Metadata-Version: 2.1 Name: fastapi-template Version: 4.1.3 Summary: Feature-
 rich robust FastAPI template Home-page: https://github.com/s3rius/FastAPI-
 template Keywords: FastAPI,Cookiecutter,Template Author: Pavel Kirilin Author-
 email: win10@list.ru Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: cookiecutter
```

