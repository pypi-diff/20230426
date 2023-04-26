# Comparing `tmp/django-simple-deploy-0.5.8.tar.gz` & `tmp/django-simple-deploy-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-deploy-0.5.8.tar", last modified: Sun Nov 13 04:06:19 2022, max compression
+gzip compressed data, was "django-simple-deploy-0.5.9.tar", last modified: Sun Nov 13 08:51:02 2022, max compression
```

## Comparing `django-simple-deploy-0.5.8.tar` & `django-simple-deploy-0.5.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.028594 django-simple-deploy-0.5.8/
--rw-r--r--   0 eric       (501) staff       (20)     1484 2021-10-22 19:44:16.000000 django-simple-deploy-0.5.8/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      121 2022-07-13 05:56:21.000000 django-simple-deploy-0.5.8/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)     2626 2022-11-13 04:06:19.028715 django-simple-deploy-0.5.8/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1338 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.004168 django-simple-deploy-0.5.8/django_simple_deploy.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     2626 2022-11-13 04:06:18.000000 django-simple-deploy-0.5.8/django_simple_deploy.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1807 2022-11-13 04:06:18.000000 django-simple-deploy-0.5.8/django_simple_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-11-13 04:06:18.000000 django-simple-deploy-0.5.8/django_simple_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       12 2022-11-13 04:06:18.000000 django-simple-deploy-0.5.8/django_simple_deploy.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)      137 2022-11-13 04:06:18.000000 django-simple-deploy-0.5.8/django_simple_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.005447 django-simple-deploy-0.5.8/docs/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.008950 django-simple-deploy-0.5.8/docs/contributing/
--rw-r--r--   0 eric       (501) staff       (20)    10555 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/contributing/development_environment.md
--rw-r--r--   0 eric       (501) staff       (20)     3474 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/contributing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     3392 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/contributing/own_account.md
--rw-r--r--   0 eric       (501) staff       (20)     6806 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/contributing/test_run.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.011926 django-simple-deploy-0.5.8/docs/design_docs/
--rw-r--r--   0 eric       (501) staff       (20)     2728 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.8/docs/design_docs/rationale.md
--rw-r--r--   0 eric       (501) staff       (20)     5165 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.8/docs/design_docs/strengths_limitations.md
--rw-r--r--   0 eric       (501) staff       (20)     3588 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.8/docs/design_docs/use_cases.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.012743 django-simple-deploy-0.5.8/docs/general_documentation/
--rw-r--r--   0 eric       (501) staff       (20)     7900 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.8/docs/general_documentation/choosing_platform.md
--rw-r--r--   0 eric       (501) staff       (20)     1505 2022-10-28 01:36:02.000000 django-simple-deploy-0.5.8/docs/index.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.015259 django-simple-deploy-0.5.8/docs/maintaining/
--rw-r--r--   0 eric       (501) staff       (20)     1048 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.8/docs/maintaining/index.md
--rw-r--r--   0 eric       (501) staff       (20)     1372 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.8/docs/maintaining/managing_releases.md
--rw-r--r--   0 eric       (501) staff       (20)     1381 2022-10-25 00:54:24.000000 django-simple-deploy-0.5.8/docs/maintaining/merging_prs.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.017559 django-simple-deploy-0.5.8/docs/quick_starts/
--rw-r--r--   0 eric       (501) staff       (20)      202 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/quick_starts/index.md
--rw-r--r--   0 eric       (501) staff       (20)     3785 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/quick_starts/quick_start_flyio.md
--rw-r--r--   0 eric       (501) staff       (20)     3598 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/quick_starts/quick_start_heroku.md
--rw-r--r--   0 eric       (501) staff       (20)     3765 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.8/docs/quick_starts/quick_start_platformsh.md
--rw-r--r--   0 eric       (501) staff       (20)       17 2022-09-23 21:19:15.000000 django-simple-deploy-0.5.8/docs/requirements.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.019238 django-simple-deploy-0.5.8/docs/unit_tests/
--rw-r--r--   0 eric       (501) staff       (20)      369 2022-11-10 06:37:53.000000 django-simple-deploy-0.5.8/docs/unit_tests/index.md
--rw-r--r--   0 eric       (501) staff       (20)     2808 2022-11-11 00:44:13.000000 django-simple-deploy-0.5.8/docs/unit_tests/running_unit_tests.md
--rw-r--r--   0 eric       (501) staff       (20)    24387 2022-11-11 00:44:13.000000 django-simple-deploy-0.5.8/docs/unit_tests/understanding_unit_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      100 2021-10-27 16:26:42.000000 django-simple-deploy-0.5.8/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)     1394 2022-11-13 04:06:19.029340 django-simple-deploy-0.5.8/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)       38 2021-10-22 19:53:08.000000 django-simple-deploy-0.5.8/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.021149 django-simple-deploy-0.5.8/simple_deploy/
--rw-r--r--   0 eric       (501) staff       (20)        0 2021-10-20 01:41:21.000000 django-simple-deploy-0.5.8/simple_deploy/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      157 2021-10-20 01:41:21.000000 django-simple-deploy-0.5.8/simple_deploy/apps.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:18.999535 django-simple-deploy-0.5.8/simple_deploy/management/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.021445 django-simple-deploy-0.5.8/simple_deploy/management/commands/
--rw-r--r--   0 eric       (501) staff       (20)    32607 2022-11-11 07:49:12.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/simple_deploy.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.025405 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/
--rw-r--r--   0 eric       (501) staff       (20)        0 2021-11-05 00:29:53.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    22040 2022-10-18 03:28:03.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_flyio.py
--rw-r--r--   0 eric       (501) staff       (20)    20062 2022-11-13 04:04:20.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_heroku.py
--rw-r--r--   0 eric       (501) staff       (20)     2941 2022-09-03 03:16:29.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages.py
--rw-r--r--   0 eric       (501) staff       (20)     5302 2022-10-24 16:45:49.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages_flyio.py
--rw-r--r--   0 eric       (501) staff       (20)     3712 2022-09-03 03:16:29.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages_heroku.py
--rw-r--r--   0 eric       (501) staff       (20)     7157 2022-11-04 05:13:02.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages_platformsh.py
--rw-r--r--   0 eric       (501) staff       (20)    19333 2022-10-29 03:51:54.000000 django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_platformsh.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 04:06:19.028334 django-simple-deploy-0.5.8/simple_deploy/templates/
--rw-r--r--   0 eric       (501) staff       (20)      604 2022-10-12 21:10:51.000000 django-simple-deploy-0.5.8/simple_deploy/templates/dockerfile_flyio
--rw-r--r--   0 eric       (501) staff       (20)      777 2022-10-12 21:10:51.000000 django-simple-deploy-0.5.8/simple_deploy/templates/fly.toml
--rw-r--r--   0 eric       (501) staff       (20)      809 2022-10-25 17:32:11.000000 django-simple-deploy-0.5.8/simple_deploy/templates/flyio_settings.py
--rw-r--r--   0 eric       (501) staff       (20)     2118 2022-10-24 20:41:27.000000 django-simple-deploy-0.5.8/simple_deploy/templates/platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1042 2022-09-03 03:16:29.000000 django-simple-deploy-0.5.8/simple_deploy/templates/platformsh_settings.py
--rw-r--r--   0 eric       (501) staff       (20)      249 2022-05-24 02:01:59.000000 django-simple-deploy-0.5.8/simple_deploy/templates/services.yaml
--rw-r--r--   0 eric       (501) staff       (20)       60 2021-10-20 01:41:21.000000 django-simple-deploy-0.5.8/simple_deploy/tests.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.804362 django-simple-deploy-0.5.9/
+-rw-r--r--   0 eric       (501) staff       (20)     1484 2021-10-22 19:44:16.000000 django-simple-deploy-0.5.9/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      121 2022-07-13 05:56:21.000000 django-simple-deploy-0.5.9/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)     2626 2022-11-13 08:51:02.804489 django-simple-deploy-0.5.9/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1338 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.779703 django-simple-deploy-0.5.9/django_simple_deploy.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     2626 2022-11-13 08:51:02.000000 django-simple-deploy-0.5.9/django_simple_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1807 2022-11-13 08:51:02.000000 django-simple-deploy-0.5.9/django_simple_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2022-11-13 08:51:02.000000 django-simple-deploy-0.5.9/django_simple_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       12 2022-11-13 08:51:02.000000 django-simple-deploy-0.5.9/django_simple_deploy.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)      137 2022-11-13 08:51:02.000000 django-simple-deploy-0.5.9/django_simple_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.781019 django-simple-deploy-0.5.9/docs/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.784566 django-simple-deploy-0.5.9/docs/contributing/
+-rw-r--r--   0 eric       (501) staff       (20)    10555 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/contributing/development_environment.md
+-rw-r--r--   0 eric       (501) staff       (20)     3474 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/contributing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3392 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/contributing/own_account.md
+-rw-r--r--   0 eric       (501) staff       (20)     6806 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/contributing/test_run.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.787441 django-simple-deploy-0.5.9/docs/design_docs/
+-rw-r--r--   0 eric       (501) staff       (20)     2728 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.9/docs/design_docs/rationale.md
+-rw-r--r--   0 eric       (501) staff       (20)     5165 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.9/docs/design_docs/strengths_limitations.md
+-rw-r--r--   0 eric       (501) staff       (20)     3588 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.9/docs/design_docs/use_cases.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.788352 django-simple-deploy-0.5.9/docs/general_documentation/
+-rw-r--r--   0 eric       (501) staff       (20)     7900 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.9/docs/general_documentation/choosing_platform.md
+-rw-r--r--   0 eric       (501) staff       (20)     1505 2022-10-28 01:36:02.000000 django-simple-deploy-0.5.9/docs/index.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.790912 django-simple-deploy-0.5.9/docs/maintaining/
+-rw-r--r--   0 eric       (501) staff       (20)     1048 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.9/docs/maintaining/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     1372 2022-10-21 17:07:34.000000 django-simple-deploy-0.5.9/docs/maintaining/managing_releases.md
+-rw-r--r--   0 eric       (501) staff       (20)     1381 2022-10-25 00:54:24.000000 django-simple-deploy-0.5.9/docs/maintaining/merging_prs.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.793353 django-simple-deploy-0.5.9/docs/quick_starts/
+-rw-r--r--   0 eric       (501) staff       (20)      202 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/quick_starts/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3785 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/quick_starts/quick_start_flyio.md
+-rw-r--r--   0 eric       (501) staff       (20)     3598 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/quick_starts/quick_start_heroku.md
+-rw-r--r--   0 eric       (501) staff       (20)     3765 2022-10-27 18:54:57.000000 django-simple-deploy-0.5.9/docs/quick_starts/quick_start_platformsh.md
+-rw-r--r--   0 eric       (501) staff       (20)       17 2022-09-23 21:19:15.000000 django-simple-deploy-0.5.9/docs/requirements.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.795247 django-simple-deploy-0.5.9/docs/unit_tests/
+-rw-r--r--   0 eric       (501) staff       (20)      369 2022-11-10 06:37:53.000000 django-simple-deploy-0.5.9/docs/unit_tests/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     2808 2022-11-11 00:44:13.000000 django-simple-deploy-0.5.9/docs/unit_tests/running_unit_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)    24387 2022-11-11 00:44:13.000000 django-simple-deploy-0.5.9/docs/unit_tests/understanding_unit_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      100 2021-10-27 16:26:42.000000 django-simple-deploy-0.5.9/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1394 2022-11-13 08:51:02.805088 django-simple-deploy-0.5.9/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)       38 2021-10-22 19:53:08.000000 django-simple-deploy-0.5.9/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.797227 django-simple-deploy-0.5.9/simple_deploy/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2021-10-20 01:41:21.000000 django-simple-deploy-0.5.9/simple_deploy/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      157 2021-10-20 01:41:21.000000 django-simple-deploy-0.5.9/simple_deploy/apps.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.775645 django-simple-deploy-0.5.9/simple_deploy/management/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.797614 django-simple-deploy-0.5.9/simple_deploy/management/commands/
+-rw-r--r--   0 eric       (501) staff       (20)    32607 2022-11-11 07:49:12.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/simple_deploy.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.801220 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2021-11-05 00:29:53.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    22388 2022-11-13 08:49:09.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_flyio.py
+-rw-r--r--   0 eric       (501) staff       (20)    20062 2022-11-13 04:04:20.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_heroku.py
+-rw-r--r--   0 eric       (501) staff       (20)     2941 2022-09-03 03:16:29.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages.py
+-rw-r--r--   0 eric       (501) staff       (20)     5302 2022-10-24 16:45:49.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages_flyio.py
+-rw-r--r--   0 eric       (501) staff       (20)     3712 2022-09-03 03:16:29.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages_heroku.py
+-rw-r--r--   0 eric       (501) staff       (20)     7157 2022-11-04 05:13:02.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages_platformsh.py
+-rw-r--r--   0 eric       (501) staff       (20)    19333 2022-10-29 03:51:54.000000 django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_platformsh.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-11-13 08:51:02.804111 django-simple-deploy-0.5.9/simple_deploy/templates/
+-rw-r--r--   0 eric       (501) staff       (20)      507 2022-11-13 08:49:09.000000 django-simple-deploy-0.5.9/simple_deploy/templates/dockerfile_flyio
+-rw-r--r--   0 eric       (501) staff       (20)      777 2022-10-12 21:10:51.000000 django-simple-deploy-0.5.9/simple_deploy/templates/fly.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1433 2022-11-13 08:49:09.000000 django-simple-deploy-0.5.9/simple_deploy/templates/flyio_settings.py
+-rw-r--r--   0 eric       (501) staff       (20)     2118 2022-10-24 20:41:27.000000 django-simple-deploy-0.5.9/simple_deploy/templates/platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1042 2022-09-03 03:16:29.000000 django-simple-deploy-0.5.9/simple_deploy/templates/platformsh_settings.py
+-rw-r--r--   0 eric       (501) staff       (20)      249 2022-05-24 02:01:59.000000 django-simple-deploy-0.5.9/simple_deploy/templates/services.yaml
+-rw-r--r--   0 eric       (501) staff       (20)       60 2021-10-20 01:41:21.000000 django-simple-deploy-0.5.9/simple_deploy/tests.py
```

### Comparing `django-simple-deploy-0.5.8/LICENSE` & `django-simple-deploy-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/PKG-INFO` & `django-simple-deploy-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.5.8
+Version: 0.5.9
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django-simple-deploy-0.5.8/README.md` & `django-simple-deploy-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/django_simple_deploy.egg-info/PKG-INFO` & `django-simple-deploy-0.5.9/django_simple_deploy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.5.8
+Version: 0.5.9
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django-simple-deploy-0.5.8/django_simple_deploy.egg-info/SOURCES.txt` & `django-simple-deploy-0.5.9/django_simple_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/contributing/development_environment.md` & `django-simple-deploy-0.5.9/docs/contributing/development_environment.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/contributing/index.md` & `django-simple-deploy-0.5.9/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/contributing/own_account.md` & `django-simple-deploy-0.5.9/docs/contributing/own_account.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/contributing/test_run.md` & `django-simple-deploy-0.5.9/docs/contributing/test_run.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/design_docs/rationale.md` & `django-simple-deploy-0.5.9/docs/design_docs/rationale.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/design_docs/strengths_limitations.md` & `django-simple-deploy-0.5.9/docs/design_docs/strengths_limitations.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/design_docs/use_cases.md` & `django-simple-deploy-0.5.9/docs/design_docs/use_cases.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/general_documentation/choosing_platform.md` & `django-simple-deploy-0.5.9/docs/general_documentation/choosing_platform.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/index.md` & `django-simple-deploy-0.5.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/maintaining/index.md` & `django-simple-deploy-0.5.9/docs/maintaining/index.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/maintaining/managing_releases.md` & `django-simple-deploy-0.5.9/docs/maintaining/managing_releases.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/maintaining/merging_prs.md` & `django-simple-deploy-0.5.9/docs/maintaining/merging_prs.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/quick_starts/quick_start_flyio.md` & `django-simple-deploy-0.5.9/docs/quick_starts/quick_start_flyio.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/quick_starts/quick_start_heroku.md` & `django-simple-deploy-0.5.9/docs/quick_starts/quick_start_heroku.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/quick_starts/quick_start_platformsh.md` & `django-simple-deploy-0.5.9/docs/quick_starts/quick_start_platformsh.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/unit_tests/running_unit_tests.md` & `django-simple-deploy-0.5.9/docs/unit_tests/running_unit_tests.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/docs/unit_tests/understanding_unit_tests.md` & `django-simple-deploy-0.5.9/docs/unit_tests/understanding_unit_tests.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/setup.cfg` & `django-simple-deploy-0.5.9/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-simple-deploy
-version = 0.5.8
+version = 0.5.9
 description = A management command that auto-configures a Django project for deployment.
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Documentation = https://django-simple-deploy.readthedocs.io/en/latest/
 	GitHub = https://github.com/ehmatthes/django-simple-deploy
 	Changelog = https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/simple_deploy.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/simple_deploy.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_flyio.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_flyio.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         self._add_dockerignore()
         self._add_flytoml_file()
         self._modify_settings()
 
         self._add_gunicorn()
         self._add_psycopg2_binary()
         self._add_dj_database_url()
+        self._add_whitenoise()
 
         self._conclude_automate_all()
 
         self._show_success_message()
 
 
     def _set_on_flyio(self):
@@ -267,14 +268,23 @@
         self.sd.write_output("\n  Looking for dj-database-url...")
 
         if self.sd.using_req_txt:
             self.sd.add_req_txt_pkg('dj-database-url')
         elif self.sd.using_pipenv:
             self.sd.add_pipenv_pkg('dj-database-url')
 
+    def _add_whitenoise(self):
+        """Add whitenoise to project requirements."""
+        self.sd.write_output("\n  Looking for whitenoise...")
+
+        if self.sd.using_req_txt:
+            self.sd.add_req_txt_pkg('whitenoise')
+        elif self.sd.using_pipenv:
+            self.sd.add_pipenv_pkg('whitenoise')
+
 
     def _conclude_automate_all(self):
         """Finish automating the push to Fly.io.
         - Commit all changes.
         - Call `fly deploy`.
         - Call `fly open`, and grab URL.
         """
```

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_heroku.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_heroku.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages_flyio.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages_flyio.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages_heroku.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages_heroku.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_messages_platformsh.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_messages_platformsh.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/management/commands/utils/deploy_platformsh.py` & `django-simple-deploy-0.5.9/simple_deploy/management/commands/utils/deploy_platformsh.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/templates/fly.toml` & `django-simple-deploy-0.5.9/simple_deploy/templates/fly.toml`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/templates/platform.app.yaml` & `django-simple-deploy-0.5.9/simple_deploy/templates/platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.5.8/simple_deploy/templates/platformsh_settings.py` & `django-simple-deploy-0.5.9/simple_deploy/templates/platformsh_settings.py`

 * *Files identical despite different names*

