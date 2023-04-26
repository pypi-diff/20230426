# Comparing `tmp/scc_pyteam_template_tools-0.2.4.tar.gz` & `tmp/scc_pyteam_template_tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scc_pyteam_template_tools-0.2.4.tar", max compression
+gzip compressed data, was "scc_pyteam_template_tools-0.2.5.tar", max compression
```

## Comparing `scc_pyteam_template_tools-0.2.4.tar` & `scc_pyteam_template_tools-0.2.5.tar`

### file list

```diff
@@ -1,169 +1,168 @@
--rw-r--r--   0        0        0      411 2023-04-25 15:23:05.019135 scc_pyteam_template_tools-0.2.4/README.md
--rw-r--r--   0        0        0     1376 2023-04-25 15:24:34.706244 scc_pyteam_template_tools-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      737 2023-04-25 15:23:05.019376 scc_pyteam_template_tools-0.2.4/scc_pyteam/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 17:23:04.697458 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/__init__.py
--rw-r--r--   0        0        0      581 2023-04-25 15:23:05.019894 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-20 15:46:56.580855 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/setup.py
--rw-r--r--   0        0        0      298 2023-04-20 15:46:56.581875 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0      199 2023-04-20 16:50:02.293193 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      104 2023-04-20 16:50:02.268288 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     6071 2023-04-20 15:46:56.583687 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2013 2023-04-20 15:46:56.584571 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      126 2023-04-20 16:50:02.293312 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.vscode/settings.json
--rw-r--r--   0        0        0     1270 2023-04-20 15:46:56.586337 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile
--rw-r--r--   0        0        0     1926 2023-04-24 10:25:04.350056 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0     1007 2023-04-25 15:23:05.020331 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-04-20 15:46:56.588241 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/__init__.py
--rw-r--r--   0        0        0     3314 2023-04-24 10:25:04.350832 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
--rw-r--r--   0        0        0       77 2023-04-20 15:46:56.588964 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/uvicorn.py
--rw-r--r--   0        0        0       73 2023-04-20 16:50:02.294981 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/postgres/.gitignore
--rw-r--r--   0        0        0       73 2023-04-20 16:50:02.259726 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/redis/.gitignore
--rw-r--r--   0        0        0      491 2023-04-20 15:46:56.591179 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0        0 2023-04-20 15:46:56.591426 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/tutorials.md
--rw-r--r--   0        0        0       98 2023-04-20 16:50:02.284253 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/.gitignore
--rw-r--r--   0        0        0      968 2023-04-24 10:25:04.351280 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env
--rwxr-xr-x   0        0        0     1119 2023-04-23 15:41:51.956622 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py
--rw-r--r--   0        0        0     1288 2023-04-20 15:46:56.592691 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0      718 2023-04-24 10:25:04.351448 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      359 2023-04-20 16:50:03.790426 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/run.py
--rw-r--r--   0        0        0       71 2023-04-23 15:39:13.773443 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:03:45.083735 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:03:45.087654 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/__init__.py
--rw-r--r--   0        0        0       44 2023-04-20 16:50:02.187899 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/admin/__init__.py
--rw-r--r--   0        0        0      276 2023-04-24 10:25:04.351632 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/__init__.py
--rw-r--r--   0        0        0     1191 2023-04-24 10:25:04.351744 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py
--rw-r--r--   0        0        0       24 2023-04-24 10:25:04.351921 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/schemas/__init__.py
--rw-r--r--   0        0        0       24 2023-04-24 10:25:04.352074 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/utils/__init__.py
--rw-r--r--   0        0        0      179 2023-04-20 16:50:02.295318 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/apps.py
--rw-r--r--   0        0        0     7720 2023-04-20 16:50:03.883631 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py
--rw-r--r--   0        0        0        0 2023-04-20 16:03:45.102373 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/migrations/__init__.py
--rw-r--r--   0        0        0       44 2023-04-20 16:50:02.195695 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:23:29.024761 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/serializers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:03:45.107687 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tasks.py
--rw-r--r--   0        0        0       84 2023-04-20 16:50:02.212945 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tests.py
--rw-r--r--   0        0        0      158 2023-04-24 10:25:04.352237 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/urls.py
--rw-r--r--   0        0        0        0 2023-04-20 16:24:34.287655 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/utils.py
--rw-r--r--   0        0        0        0 2023-04-20 16:03:45.113131 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/views/__init__.py
--rw-r--r--   0        0        0       54 2023-04-24 06:55:51.453643 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/__init__.py
--rw-r--r--   0        0        0      115 2023-04-23 15:25:27.839383 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/logger.py
--rw-r--r--   0        0        0      597 2023-04-20 16:50:03.473182 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py
--rw-r--r--   0        0        0      208 2023-04-20 16:03:45.122818 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/__init__.py
--rw-r--r--   0        0        0      394 2023-04-20 16:50:03.420204 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/api_router.py
--rw-r--r--   0        0        0      914 2023-04-24 06:55:51.691382 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py
--rw-r--r--   0        0        0     8484 2023-04-24 10:25:04.352654 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py
--rw-r--r--   0        0        0      883 2023-04-20 16:50:03.391964 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-20 16:50:03.883927 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py
--rw-r--r--   0        0        0     2418 2023-04-20 16:50:03.879584 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py
--rw-r--r--   0        0        0      605 2023-04-20 16:18:13.439388 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py
--rw-r--r--   0        0        0     3108 2023-04-24 10:25:04.353496 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py
--rw-r--r--   0        0        0      377 2023-04-20 16:50:03.853031 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/elk_settings.py
--rw-r--r--   0        0        0      543 2023-04-20 16:18:13.441777 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py
--rw-r--r--   0        0        0      935 2023-04-20 16:50:02.352078 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py
--rw-r--r--   0        0        0     1288 2023-04-20 16:50:02.372221 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py
--rw-r--r--   0        0        0      570 2023-04-20 16:50:03.859709 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py
--rw-r--r--   0        0        0      773 2023-04-20 16:18:13.443896 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py
--rw-r--r--   0        0        0     1044 2023-04-20 16:50:03.883070 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py
--rw-r--r--   0        0        0     1096 2023-04-24 10:25:04.353673 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py
--rw-r--r--   0        0        0      126 2023-04-20 16:18:13.445434 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/security_settings.py
--rw-r--r--   0        0        0     1265 2023-04-25 15:23:05.020808 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py
--rw-r--r--   0        0        0      755 2023-04-25 15:23:05.021014 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py
--rw-r--r--   0        0        0      882 2023-04-20 16:50:02.359988 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py
--rw-r--r--   0        0        0     1556 2023-04-24 10:25:04.353834 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py
--rw-r--r--   0        0        0     1754 2023-04-24 10:25:04.353986 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py
--rw-r--r--   0        0        0        0 2023-04-20 16:03:45.124224 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/schema/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:03:45.124500 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/staticfiles/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-20 15:46:56.615335 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/static/.gitkeep
--rw-r--r--   0        0        0       37 2023-04-20 15:46:56.615737 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0      708 2023-04-20 16:50:02.020530 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-18 17:38:22.400176 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/setup.py
--rw-r--r--   0        0        0      298 2023-04-19 17:03:48.251032 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0      199 2023-04-20 16:50:02.305533 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      103 2023-04-19 17:03:48.251289 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     6071 2023-04-19 17:03:48.251414 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2013 2023-04-19 17:03:48.251508 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      125 2023-04-19 17:03:48.251642 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.vscode/settings.json
--rw-r--r--   0        0        0     1270 2023-04-20 09:52:59.439761 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile
--rw-r--r--   0        0        0     1389 2023-04-25 15:23:05.021337 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0     1007 2023-04-25 15:23:05.021602 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-04-19 17:03:48.251826 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/__init__.py
--rw-r--r--   0        0        0      216 2023-04-19 17:03:48.251974 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
--rw-r--r--   0        0        0       77 2023-04-19 17:03:48.252079 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/uvicorn.py
--rw-r--r--   0        0        0       74 2023-04-20 08:25:37.251439 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/mongo/.gitignore
--rw-r--r--   0        0        0       74 2023-04-20 08:25:37.251631 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/redis/.gitignore
--rw-r--r--   0        0        0      491 2023-04-19 17:03:48.252214 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0        0 2023-04-19 17:03:48.252252 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/tutorials.md
--rw-r--r--   0        0        0       98 2023-04-20 16:50:02.268445 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/.gitignore
--rw-r--r--   0        0        0      761 2023-04-20 15:05:07.117927 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env
--rw-r--r--   0        0        0     1288 2023-04-19 17:03:48.252522 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0      640 2023-04-20 10:12:40.163865 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      359 2023-04-20 08:25:37.252094 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/run.py
--rw-r--r--   0        0        0        8 2023-04-18 17:38:21.752557 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/README.md
--rw-r--r--   0        0        0        0 2023-04-20 09:47:46.675844 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/__init__.py
--rw-r--r--   0        0        0      550 2023-04-20 16:50:03.402726 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py
--rw-r--r--   0        0        0       34 2023-04-19 17:03:48.253167 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/__init__.py
--rw-r--r--   0        0        0      115 2023-04-19 17:03:48.253271 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/logger.py
--rw-r--r--   0        0        0        0 2023-04-19 17:03:48.253341 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/__init__.py
--rw-r--r--   0        0        0      743 2023-04-20 08:25:37.252363 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py
--rw-r--r--   0        0        0     4172 2023-04-20 08:25:37.252645 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py
--rw-r--r--   0        0        0      178 2023-04-19 17:03:48.253802 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/__init__.py
--rw-r--r--   0        0        0      463 2023-04-19 17:03:48.253901 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/shutdown.py
--rw-r--r--   0        0        0      797 2023-04-20 08:25:37.252889 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py
--rw-r--r--   0        0        0      448 2023-04-24 06:55:51.713060 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/__init__.py
--rw-r--r--   0        0        0      644 2023-04-20 16:50:03.896480 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py
--rw-r--r--   0        0        0      638 2023-04-20 16:50:03.903051 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py
--rw-r--r--   0        0        0       75 2023-04-20 16:50:02.289033 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/__init__.py
--rw-r--r--   0        0        0      703 2023-04-20 16:50:03.896723 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py
--rw-r--r--   0        0        0     3613 2023-04-20 16:50:03.918712 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py
--rw-r--r--   0        0        0     1952 2023-04-19 17:03:48.254305 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 17:13:02.112539 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/models/__init__.py
--rw-r--r--   0        0        0      241 2023-04-20 16:50:03.407563 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/__init__.py
--rw-r--r--   0        0        0      325 2023-04-20 16:50:03.894872 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/__init__.py
--rw-r--r--   0        0        0       61 2023-04-20 16:50:02.295235 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/__init__.py
--rw-r--r--   0        0        0      131 2023-04-20 16:50:02.204627 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/get_info.py
--rw-r--r--   0        0        0       70 2023-04-20 16:50:02.295113 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/__init__.py
--rw-r--r--   0        0        0      107 2023-04-20 16:50:02.293451 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/get_info.py
--rw-r--r--   0        0        0        0 2023-04-18 17:13:03.836332 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/schemas/__init__.py
--rw-r--r--   0        0        0       64 2023-04-19 17:03:48.254558 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/__init__.py
--rw-r--r--   0        0        0      581 2023-04-19 17:03:48.254674 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py
--rw-r--r--   0        0        0     1032 2023-04-19 17:03:48.254795 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-20 16:50:03.921923 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py
--rw-r--r--   0        0        0     2467 2023-04-19 17:03:48.255004 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py
--rw-r--r--   0        0        0      605 2023-04-20 08:38:02.684338 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py
--rw-r--r--   0        0        0     4228 2023-04-19 17:03:48.255198 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py
--rw-r--r--   0        0        0      378 2023-04-19 17:03:48.255288 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/elk_settings.py
--rw-r--r--   0        0        0      543 2023-04-20 08:25:37.253394 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py
--rw-r--r--   0        0        0      935 2023-04-19 17:03:48.255491 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py
--rw-r--r--   0        0        0     1288 2023-04-19 17:03:48.255592 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py
--rw-r--r--   0        0        0      575 2023-04-19 17:03:48.255697 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py
--rw-r--r--   0        0        0      773 2023-04-19 17:03:48.255815 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py
--rw-r--r--   0        0        0     1078 2023-04-19 17:03:48.255913 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py
--rw-r--r--   0        0        0      825 2023-04-20 16:50:02.376263 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py
--rw-r--r--   0        0        0      126 2023-04-19 17:03:48.256089 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/security_settings.py
--rw-r--r--   0        0        0     1758 2023-04-20 16:50:02.359308 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py
--rw-r--r--   0        0        0      814 2023-04-19 17:03:48.256287 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py
--rw-r--r--   0        0        0      882 2023-04-20 08:25:37.253631 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py
--rw-r--r--   0        0        0        0 2023-04-19 17:03:48.256467 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0      435 2023-04-20 16:50:03.905138 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/api_response.py
--rw-r--r--   0        0        0     6722 2023-04-19 17:03:48.256610 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py
--rw-r--r--   0        0        0      659 2023-04-20 16:50:02.369099 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py
--rw-r--r--   0        0        0      977 2023-04-19 17:03:48.256710 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py
--rw-r--r--   0        0        0      579 2023-04-20 16:50:03.427852 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py
--rw-r--r--   0        0        0      417 2023-04-19 17:03:48.257076 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/__init__.py
--rw-r--r--   0        0        0      114 2023-04-19 17:03:48.257171 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/client_events.py
--rw-r--r--   0        0        0      114 2023-04-19 17:03:48.257265 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/server_events.py
--rw-r--r--   0        0        0        0 2023-04-20 08:25:37.253966 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/static/.gitkeep
--rw-r--r--   0        0        0       37 2023-04-19 17:03:48.257371 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0      270 2023-04-18 17:06:57.867927 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-18 17:38:22.403558 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-18 17:38:21.752501 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-18 17:29:28.725210 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      270 2023-04-18 17:06:53.025075 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-18 17:38:22.404118 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-18 17:38:21.745563 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-18 17:29:37.188720 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      270 2023-04-18 17:07:00.132336 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-18 17:38:22.400783 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-18 17:38:21.752755 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-18 17:29:46.489100 scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0     7821 1970-01-01 00:00:00.000000 scc_pyteam_template_tools-0.2.4/setup.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 scc_pyteam_template_tools-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      441 2023-04-25 15:32:59.973258 scc_pyteam_template_tools-0.2.5/README.md
+-rw-r--r--   0        0        0     1376 2023-04-25 15:32:59.973258 scc_pyteam_template_tools-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-04-25 15:32:59.973258 scc_pyteam_template_tools-0.2.5/scc_pyteam/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.973258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/__init__.py
+-rw-r--r--   0        0        0      581 2023-04-25 15:32:59.973258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 15:32:59.973258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/setup.py
+-rw-r--r--   0        0        0      298 2023-04-25 15:32:59.973258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0      199 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      104 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     6071 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2013 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      126 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     1270 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile
+-rw-r--r--   0        0        0     1926 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0     1007 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/__init__.py
+-rw-r--r--   0        0        0     3314 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
+-rw-r--r--   0        0        0       77 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/uvicorn.py
+-rw-r--r--   0        0        0       73 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/postgres/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/redis/.gitignore
+-rw-r--r--   0        0        0      491 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/tutorials.md
+-rw-r--r--   0        0        0       98 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/.gitignore
+-rw-r--r--   0        0        0      968 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env
+-rwxr-xr-x   0        0        0     1119 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py
+-rw-r--r--   0        0        0     1288 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0      718 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      359 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/run.py
+-rw-r--r--   0        0        0       71 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/admin/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/__init__.py
+-rw-r--r--   0        0        0     1191 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py
+-rw-r--r--   0        0        0       24 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/schemas/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/utils/__init__.py
+-rw-r--r--   0        0        0      179 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/apps.py
+-rw-r--r--   0        0        0     7720 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/migrations/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/serializers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tasks.py
+-rw-r--r--   0        0        0       84 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tests.py
+-rw-r--r--   0        0        0      158 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/urls.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/views/__init__.py
+-rw-r--r--   0        0        0       54 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/logger.py
+-rw-r--r--   0        0        0      597 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py
+-rw-r--r--   0        0        0      208 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/__init__.py
+-rw-r--r--   0        0        0      394 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/api_router.py
+-rw-r--r--   0        0        0      914 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py
+-rw-r--r--   0        0        0     8484 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py
+-rw-r--r--   0        0        0      883 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py
+-rw-r--r--   0        0        0     2418 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py
+-rw-r--r--   0        0        0      605 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py
+-rw-r--r--   0        0        0     3108 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py
+-rw-r--r--   0        0        0      377 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/elk_settings.py
+-rw-r--r--   0        0        0      543 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py
+-rw-r--r--   0        0        0      935 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py
+-rw-r--r--   0        0        0     1288 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py
+-rw-r--r--   0        0        0      570 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py
+-rw-r--r--   0        0        0      773 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py
+-rw-r--r--   0        0        0     1044 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py
+-rw-r--r--   0        0        0     1096 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py
+-rw-r--r--   0        0        0      126 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/security_settings.py
+-rw-r--r--   0        0        0     1265 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py
+-rw-r--r--   0        0        0      755 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py
+-rw-r--r--   0        0        0      882 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py
+-rw-r--r--   0        0        0     1556 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py
+-rw-r--r--   0        0        0     1754 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.977258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/schema/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/staticfiles/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/static/.gitkeep
+-rw-r--r--   0        0        0       37 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0      708 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/setup.py
+-rw-r--r--   0        0        0      298 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0      199 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      103 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     6071 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2013 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      125 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     1270 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile
+-rw-r--r--   0        0        0     1389 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0     1007 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
+-rw-r--r--   0        0        0       77 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/uvicorn.py
+-rw-r--r--   0        0        0       74 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/mongo/.gitignore
+-rw-r--r--   0        0        0       74 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/redis/.gitignore
+-rw-r--r--   0        0        0      491 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/tutorials.md
+-rw-r--r--   0        0        0       98 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/.gitignore
+-rw-r--r--   0        0        0      761 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env
+-rw-r--r--   0        0        0     1288 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0      640 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      359 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/run.py
+-rw-r--r--   0        0        0        8 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/__init__.py
+-rw-r--r--   0        0        0      550 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py
+-rw-r--r--   0        0        0       34 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/logger.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py
+-rw-r--r--   0        0        0     4172 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py
+-rw-r--r--   0        0        0      178 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/__init__.py
+-rw-r--r--   0        0        0      463 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/shutdown.py
+-rw-r--r--   0        0        0      797 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py
+-rw-r--r--   0        0        0      448 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py
+-rw-r--r--   0        0        0      638 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py
+-rw-r--r--   0        0        0       75 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/__init__.py
+-rw-r--r--   0        0        0      703 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py
+-rw-r--r--   0        0        0     3613 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py
+-rw-r--r--   0        0        0     1952 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/models/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/get_info.py
+-rw-r--r--   0        0        0       70 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/get_info.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/schemas/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/__init__.py
+-rw-r--r--   0        0        0      581 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py
+-rw-r--r--   0        0        0     1032 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py
+-rw-r--r--   0        0        0     2467 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py
+-rw-r--r--   0        0        0      605 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py
+-rw-r--r--   0        0        0     4228 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py
+-rw-r--r--   0        0        0      378 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/elk_settings.py
+-rw-r--r--   0        0        0      543 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py
+-rw-r--r--   0        0        0      935 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py
+-rw-r--r--   0        0        0     1288 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py
+-rw-r--r--   0        0        0      575 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py
+-rw-r--r--   0        0        0      773 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py
+-rw-r--r--   0        0        0     1078 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py
+-rw-r--r--   0        0        0      825 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py
+-rw-r--r--   0        0        0      126 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/security_settings.py
+-rw-r--r--   0        0        0     1758 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py
+-rw-r--r--   0        0        0      814 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py
+-rw-r--r--   0        0        0      882 2023-04-25 15:32:59.981258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0      435 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/api_response.py
+-rw-r--r--   0        0        0     6722 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py
+-rw-r--r--   0        0        0      659 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py
+-rw-r--r--   0        0        0      977 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py
+-rw-r--r--   0        0        0      579 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py
+-rw-r--r--   0        0        0      417 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/client_events.py
+-rw-r--r--   0        0        0      114 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/server_events.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/static/.gitkeep
+-rw-r--r--   0        0        0       37 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      270 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      270 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-25 15:32:59.985258 scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 scc_pyteam_template_tools-0.2.5/PKG-INFO
```

### Comparing `scc_pyteam_template_tools-0.2.4/pyproject.toml` & `scc_pyteam_template_tools-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scc-pyteam-template-tools"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["NhanDD <hp.duongducnhan@gmail.com>"]
 readme = "README.md"
 packages = [{include = "scc_pyteam"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/__init__.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Entry point of my coca tools
 """
 import os
 
 from cookiecutter.main import cookiecutter
 
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 BASE_PATH = os.path.dirname(os.path.abspath(__file__))
 TEMPLATE_PATH = os.path.join(BASE_PATH, 'cookiecutter_templates')
 
 
 def welcome():
     """Say welcome to users"""
     print('welcome to coca tools')
```

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/cookiecutter.json` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/cookiecutter.json` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py` & `scc_pyteam_template_tools-0.2.5/scc_pyteam/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py`

 * *Files identical despite different names*

### Comparing `scc_pyteam_template_tools-0.2.4/PKG-INFO` & `scc_pyteam_template_tools-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scc-pyteam-template-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: NhanDD
 Author-email: hp.duongducnhan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,19 +30,19 @@
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Description-Content-Type: text/markdown
 
 # Installation
 - Require python >= 3.10
 - using pip
     ```
-    $ pip install coca-tools
+    $ pip install scc-pyteam-template-tools
     ```
 - using poetry
     ```
-    $ poetry add coca-tools
+    $ poetry add scc-pyteam-template-tools
     ```
 
 
 # Guide
 - Require: using in global environment
 - create fastapi template with command then fill the questions
     ```
```

