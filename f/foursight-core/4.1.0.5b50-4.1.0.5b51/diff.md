# Comparing `tmp/foursight_core-4.1.0.5b50.tar.gz` & `tmp/foursight_core-4.1.0.5b51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.0.5b50.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.5b51.tar", max compression
```

## Comparing `foursight_core-4.1.0.5b50.tar` & `foursight_core-4.1.0.5b51.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-04-26 11:12:56.893741 foursight_core-4.1.0.5b50/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-04-26 11:12:56.897741 foursight_core-4.1.0.5b50/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-26 11:12:56.897741 foursight_core-4.1.0.5b50/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-04-26 11:12:56.897741 foursight_core-4.1.0.5b50/foursight_core/app.py
--rw-r--r--   0        0        0   105730 2023-04-26 11:12:56.897741 foursight_core-4.1.0.5b50/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/package.py
--rw-r--r--   0        0        0    17014 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     7709 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    23203 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20652 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3459 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     5745 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4878 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3257 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     4621 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    77887 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11353 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    32676 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4861 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-04-26 11:12:56.901741 foursight_core-4.1.0.5b50/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1927369 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1609 2023-04-26 11:12:56.913741 foursight_core-4.1.0.5b50/pyproject.toml
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b50/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-26 14:15:59.652887 foursight_core-4.1.0.5b51/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/app.py
+-rw-r--r--   0        0        0   105729 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/package.py
+-rw-r--r--   0        0        0    17191 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     7608 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    23203 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6315 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28316 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20652 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3456 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4876 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3257 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9524 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5200 2023-04-26 14:15:59.660887 foursight_core-4.1.0.5b51/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    78139 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11353 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    32676 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4861 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-04-26 14:15:59.664887 foursight_core-4.1.0.5b51/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1927239 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-04-26 14:15:59.672887 foursight_core-4.1.0.5b51/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1609 2023-04-26 14:15:59.676888 foursight_core-4.1.0.5b51/pyproject.toml
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b51/PKG-INFO
```

### Comparing `foursight_core-4.1.0.5b50/LICENSE.txt` & `foursight_core-4.1.0.5b51/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.5b51/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/app_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/app_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,21 +273,21 @@
         user_record["error"] = error
         user_record["exception"] = exception
 
     def get_portal_url(self, env_name: str, raise_exception: bool = False) -> Optional[str]:
         portal_url = self._cached_portal_url.get(env_name)
         if not portal_url:
             try:
-                environment_and_bucket_info = \
-                    self.environment.get_environment_and_bucket_info(env_name, self.stage.get_stage())
+                environment_and_bucket_info = (
+                    self.environment.get_environment_and_bucket_info(env_name, self.stage.get_stage()))
                 portal_url = environment_and_bucket_info.get("fourfront")
                 self._cached_portal_url[env_name] = portal_url
             except Exception as e:
                 if raise_exception:
-                    raise e
+                    raise
                 message = f"Error getting portal URL: {get_error_message(e)}"
                 logger.error(message)
                 return None
         return self._cached_portal_url[env_name]
 
     def get_auth0_client_id(self, env_name: str) -> str:
         auth0_client_id = os.environ.get("CLIENT_ID")
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/buckets.py` & `foursight_core-4.1.0.5b51/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/check_schema.py` & `foursight_core-4.1.0.5b51/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/check_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.5b51/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/decorators.py` & `foursight_core-4.1.0.5b51/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/deploy.py` & `foursight_core-4.1.0.5b51/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/environment.py` & `foursight_core-4.1.0.5b51/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/es_connection.py` & `foursight_core-4.1.0.5b51/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/exceptions.py` & `foursight_core-4.1.0.5b51/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/fs_connection.py` & `foursight_core-4.1.0.5b51/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/identity.py` & `foursight_core-4.1.0.5b51/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/mapping.json` & `foursight_core-4.1.0.5b51/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/package.py` & `foursight_core-4.1.0.5b51/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,18 +153,20 @@
             authenticator = authenticator.casefold()
             if "google" in authenticator:
                 authenticator = "google"
             elif "github" in authenticator:
                 authenticator = "github"
         try:
             if request:
+                # Note that these "test_mode_xyz" cookies are for testing only
+                # and if used must be manually set, e.g. via Chrome Developer Tools.
                 test_mode_access_key_simulate_error = read_cookie_bool(request, "test_mode_access_key_simulate_error")
                 if test_mode_access_key_simulate_error:
                     # For testing only, we simulate a portal access key error (e.g. due to expiration),
-                    # which would manifest itselft, most importantly, here, on login.
+                    # which would manifest itself, primarily and most importantly, here, on login.
                     raise Exception("test_mode_access_key_simulate_error")
             allowed_envs, first_name, last_name = self._envs.get_user_auth_info(email, raise_exception=True)
             user_exception = False
         except Exception as e:
             #
             # Here there was a problem getting the user info via Portal (e.g. due to expired or otherwise bad
             # Portal acesss key); this will NOT prevent the user from being logged in BUT it WILL prevent the
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/auth0_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,15 @@
         "scope": "openid email",
         "prompt": "select_account",
         "connections": ["github", "google-oauth2"]
     }
 
     def __init__(self, portal_url: str) -> None:
         if not portal_url:
-            portal_url = ""
-            logger.error("Portal URL required for Auth0Config usage.")
-            # raise ValueError("Portal URL required for Auth0Config usage.")
+            raise ValueError("Portal URL required for Auth0Config usage.")
         self._portal_url = portal_url
         self._config_url = f"{portal_url}{'/' if not portal_url.endswith('/') else ''}auth0_config?format=json"
         self._config_data = {}
         self._config_raw_data = {}
 
     def get_portal_url(self) -> str:
         return self._portal_url
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/cookie_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,25 @@
     return cookie_morsel.value if cookie_morsel else None
 
 
 def read_cookie_bool(request: dict, cookie_name: str) -> bool:
     return str_to_bool(read_cookie(request, cookie_name))
 
 
-def read_cookie_int(request: dict, cookie_name: str, fallback: int = 0) -> int:
+def read_cookie_int(request: dict, cookie_name: str, default: int = 0) -> int:
     value = read_cookie(request, cookie_name)
     if not value:
-        return fallback
+        return default
     if value.startswith("-"):
         value = value[1:]
         multiplier = -1
     else:
         multiplier = 1
     if not value.isdigit():
-        return fallback
+        return default
     return int(value) * multiplier
 
 
 def _read_cookies(request: dict) -> Optional[SimpleCookie]:
     """
     Returns the cookies from the given request as a SimpleCookie object.
     """
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/datetime_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,14 +63,26 @@
 def convert_time_t_to_useastern_datetime_string(time_t: int) -> Optional[str]:
     """
     Same as convert_time_t_to_datetime_string (above) but specifically for US/Eastern timezone.
     """
     return convert_time_t_to_datetime_string(time_t, TIMEZONE_USEASTERN)
 
 
+def convert_iso_datetime_string_to_datetime(value: str) -> Optional[datetime.datetime]:
+    """
+    Returns a datetime object, in the UTC timezone, for the given (assumed)
+    ISO 8601 conforming datetime string; if an error occurs (e.g. if the
+    given value is not ISO 8601 conforming) then returns None.
+    """
+    try:
+        return datetime.datetime.fromisoformat(value).astimezone(pytz.utc)
+    except Exception:
+        return None
+
+
 def convert_time_t_to_datetime(time_t: int) -> datetime.datetime:
     """
     Converts the given "epoch" time (seconds since 1970-01-01T00:00:00Z)
     to a datetime and returns its value.
     """
     return datetime.datetime.fromtimestamp(time_t, tz=pytz.UTC)
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/envs.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                     # from the last env in the loop; doesn't really matter, just pick one set; this is just for
                     # informational/display purposes in the UI.
                     first_name = user.get("first_name")
                     last_name = user.get("last_name")
                     allowed_envs.append(known_env["full_name"])
             except Exception as e:
                 if raise_exception:
-                    raise e
+                    raise
                 logger.warning(f"Exception getting allowed envs for {email}: {e}")
         return allowed_envs, first_name, last_name
 
     @staticmethod
     def _is_user_allowed_access(user: Optional[dict]) -> bool:
         return user and Envs._is_user_in_one_or_more_groups(user, ["admin", "foursight"])
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/portal_access_key_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from datetime import datetime, timedelta
 import pytz
 from dcicutils import ff_utils
+from dcicutils.misc_utils import future_datetime
 from typing import Optional, Tuple
 from ...app import app
+from .datetime_utils import convert_iso_datetime_string_to_datetime
 
 
 _PORTAL_ACCESS_KEY_NAME = "access_key_foursight"
 _PORTAL_ACCESS_KEY_USER_EMAIL = "foursight.app@gmail.com"
 _PORTAL_ACCESS_KEY_EXPIRES_SOON_WARNING_DAYS = 10
 
 
 def get_portal_access_key_info(env: str,
-                               obfuscate: bool = False,
+                               logged_in: bool = False,
                                test_mode_access_key_simulate_error: bool = False,
                                test_mode_access_key_expiration_warning_days: int = 0) -> dict:
     try:
         now = datetime.now(pytz.utc)
         connection = app.core.init_connection(env)
         connection_keys = connection.ff_keys
         key = connection_keys.get("key")
-        if key and obfuscate:
+        if key and not logged_in:
+            # This logged_in flag is passed from caller (react_api.reactapi_portal_access_key)
+            # and is False iff the user is NOT logged in; so if logged in then we do NOT obfuscate
+            # the access key (ID) but if we ARE not logged in we just see the first letter of it.
+            # And of course we do not return a value for any part of the secret at all, ever.
             key = key[0] + "*******"
-        secret = connection_keys.get("secret")
-        if secret:
-            secret = "********" if obfuscate else secret[1] + "*******"
         server = connection_keys.get("server")
-        access_key_info = {"key": key, "secret": secret, "server": server}
+        access_key_info = {"key": key, "secret": "********", "server": server, "logged_in": logged_in}
         access_key_create_date, access_key_expires_date, access_key_expires_exception = \
             _get_portal_access_key_expires_date(connection_keys)
         if access_key_expires_date:
             access_key_info["created_at"] = access_key_create_date.strftime("%Y-%m-%d %H:%M:%S")
             if access_key_expires_date == datetime.max:
                 access_key_info["expires_at"] = None
                 access_key_info["expired"] = False
                 access_key_info["invalid"] = False
                 access_key_info["expires_soon"] = False
             else:
                 access_key_info["expires_at"] = access_key_expires_date.strftime("%Y-%m-%d %H:%M:%S")
                 access_key_info["expired"] = now >= access_key_expires_date
                 access_key_info["invalid"] = access_key_info["expired"]
+                # Note that these "test_mode_xyz" variables are for testing only and are set
+                # via cookies and if used must be manually set, e.g. via Chrome Developer Tools.
                 if test_mode_access_key_expiration_warning_days > 0:
                     expires_soon_days = test_mode_access_key_expiration_warning_days
                 else:
                     expires_soon_days = _PORTAL_ACCESS_KEY_EXPIRES_SOON_WARNING_DAYS
                 access_key_info["expires_soon"] = _is_datetime_within_future_ndays(access_key_expires_date,
                                                                                    ndays=expires_soon_days,
                                                                                    now=now)
@@ -62,29 +67,29 @@
         return {}
 
 
 def _get_portal_access_key_expires_date(keys: dict) -> Tuple[datetime, Optional[datetime], Optional[Exception]]:
     try:
         query = f"/search/?type=AccessKey&description={_PORTAL_ACCESS_KEY_NAME}&sort=-date_created"
         access_key = ff_utils.search_metadata(query, key=keys)[0]
-        access_key_create_date = datetime.fromisoformat(access_key["date_created"]).astimezone(pytz.utc)
+        access_key_create_date = convert_iso_datetime_string_to_datetime(access_key["date_created"])
         access_key_expires_date = access_key.get("expiration_date")
         if access_key_expires_date:
-            access_key_expires_date = datetime.fromisoformat(access_key_expires_date).astimezone(pytz.utc)
+            access_key_expires_date = convert_iso_datetime_string_to_datetime(access_key_expires_date)
         else:
             # There may or may not be an expiration date (e.g. for fourfront);
-            # if not then make it the max date which is 9999-12-31.
+            # if not then make it the max date which is 9999-12-31 23:59:59.999999.
             access_key_expires_date = datetime.max
         return (access_key_create_date, access_key_expires_date, None)
     except Exception as e:
         return (None, None, e)
 
 
 def _is_datetime_within_future_ndays(d: datetime, ndays: int, now: Optional[datetime] = None) -> bool:
     """
     Returns True iff the given datatime is within ndays IN THE FUTURE of the CURRENT
     datetime. I.e. if the current datetime plus ndays is greater-than-or-equal to
     the given datetime the returns True; otherwise returns False.
     """
     if not now:
         now = datetime.now(pytz.utc)
-    return (d - now) <= timedelta(days=ndays) if d >= now else False
+    return d <= future_datetime(now=now, days=ndays)
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/react_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,59 +278,63 @@
         data["auth"] = auth
         # 2022-10-18
         # No longer sharing known-envs widely; send only if authenticated;
         # if not authenticated then act as-if the default-env is the only known-env;
         # in this case also include (as an FYI for the UI) the real number of known-envs.
         if auth["authenticated"]:
             data["auth"]["known_envs"] = self._envs.get_known_envs_with_gac_names()
-            is_logged_in = True
+            logged_in = True
         else:
-            is_logged_in = False
+            logged_in = False
             known_envs_default = self._envs.find_known_env(self._envs.get_default_env())
             known_envs_actual_count = self._envs.get_known_envs_count()
             data["auth"]["known_envs"] = [known_envs_default]
             data["auth"]["known_envs_actual_count"] = known_envs_actual_count
         data["auth"]["default_env"] = self._envs.get_default_env()
+        # Note that these "test_mode_xyz" cookies are for testing only
+        # and if used must be manually set, e.g. via Chrome Developer Tools.
         test_mode_certificate_simulate_error = read_cookie_bool(request, "test_mode_certificate_simulate_error")
         if test_mode_certificate_simulate_error:
             data["portal"]["url"] = None
+        # Note that we know that data["portal"]["url"] is explicitly set via _reactapi_header_nocache.
         if not data["portal"]["url"]:
             # Here we did not get a Portal URL from the to app.core.get_portal_url (via _reactapi_header_nocache).
             # That call ends up ultimately calling the Portal health endpoint (via s3Utils.get_synthetic_env_config
             # via environment.get_environment_and_bucket_info). So there may have been a problem with the Portal,
             # e.g. bad SSL certificate; we will get the Portal URL by other means, and from get get its SSL
             # certificate to help diagnose any problem with that. C4-1017 (April 2023).
             try:
                 if test_mode_certificate_simulate_error:
                     raise Exception("test_mode_certificate_simulate_error")
                 portal_url = app.core.get_portal_url(env or default_env, raise_exception=True)
                 data["portal"]["url"] = portal_url
             except Exception as e:
                 e = str(e)
-                data["portal"]["exception"] = e
+                data_portal = data["portal"]
+                data_portal["exception"] = e
                 if "certifi" in e.lower():
-                    data["portal"]["ssl_certificate_error"] = True
+                    data_portal["ssl_certificate_error"] = True
                 portal_url = env_utils_get_portal_url(env)
-                data["portal"]["url"] = portal_url
-                data["portal"]["ssl_certificate"] = get_ssl_certificate_info(portal_url)
-                if data["portal"]["ssl_certificate"]:
-                    data["portal"]["ssl_certificate"]["name"] = "Portal"
-                    data["portal"]["ssl_certificate"]["exception"] = e
+                data_portal["url"] = portal_url
+                data_portal["ssl_certificate"] = get_ssl_certificate_info(portal_url)
+                if data_portal["ssl_certificate"]:
+                    data_portal["ssl_certificate"]["name"] = "Portal"
+                    data_portal["ssl_certificate"]["exception"] = e
         data["timestamp"] = convert_utc_datetime_to_useastern_datetime_string(datetime.datetime.utcnow())
         test_mode_access_key_simulate_error = read_cookie_bool(request, "test_mode_access_key_simulate_error")
         if auth.get("user_exception"): # or test_mode_access_key_simulate_error:
             # Since this call to get the Portal access key info can be relatively expensive, we don't want to
             # do it on every /header API call; so we only call it if, according to the user's authtoken cookie,
             # an exception was experienced when trying to authorize the user (via envs.get_user_auth_info) on
             # login, which if so, would indicate that the is likely a problem with the Portal access key.
             test_mode_access_key_expiration_warning_days = \
                 read_cookie_int(request, "test_mode_access_key_expiration_warning_days")
             data["portal_access_key"] = get_portal_access_key_info(
                 env,
-                obfuscate=not is_logged_in,
+                logged_in=logged_in,
                 test_mode_access_key_simulate_error=test_mode_access_key_simulate_error,
                 test_mode_access_key_expiration_warning_days=test_mode_access_key_expiration_warning_days)
             if data["portal_access_key"].get("invalid"):
                 data["portal_access_key_error"] = True
         return self.create_success_response(data)
 
     def _reactapi_header_nocache(self, request: dict, env: str) -> dict:
@@ -402,21 +406,21 @@
                 portal_ssl_certificate_info["name"] = "Portal"
                 response.append(portal_ssl_certificate_info)
         return self.create_success_response(response)
 
     def reactapi_portal_access_key(self, request: dict, args: Optional[dict] = None) -> Response:
         env = self._envs.get_default_env()
         auth = self._auth.authorize(request, env)
-        is_logged_in = auth.get("authenticated")
+        logged_in = auth.get("authenticated")
         test_mode_access_key_simulate_error = read_cookie_bool(request, "test_mode_access_key_simulate_error")
         test_mode_access_key_expiration_warning_days = read_cookie_int(
                 request, "test_mode_access_key_expiration_warning_days")
         response = get_portal_access_key_info(
             env,
-            obfuscate=not is_logged_in,
+            logged_in=logged_in,
             test_mode_access_key_simulate_error=test_mode_access_key_simulate_error,
             test_mode_access_key_expiration_warning_days=test_mode_access_key_expiration_warning_days)
         return self.create_success_response(response)
 
     @memoize
     def _get_env_and_bucket_info(self, env: str, stage_name: str) -> dict:
         return sort_dictionary_by_case_insensitive_keys(
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.5b51/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.5b51/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.5b51/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.8b129b67.js.LICENSE.txt */
+/*! For license information please see main.faf78e31.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -49256,37 +49256,20 @@
                     children: (0, Kr.jsx)("table", {
                         width: "100%",
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Portal:"
-                                }), (0, Kr.jsx)("td", {
+                                }), (0, Kr.jsxs)("td", {
                                     style: i,
-                                    children: (0, Kr.jsx)("a", {
+                                    children: [(0, Kr.jsx)("a", {
                                         href: "".concat(r.server),
                                         target: "_blank",
                                         children: r.server
-                                    })
-                                })]
-                            }), (0, Kr.jsxs)("tr", {
-                                children: [(0, Kr.jsx)("td", {
-                                    style: s,
-                                    children: "Access Key:"
-                                }), (0, Kr.jsxs)("td", {
-                                    style: i,
-                                    children: [r.key, Br.IsLoggedIn(n) && (0, Kr.jsxs)(Kr.Fragment, {
-                                        children: ["\xa0\xa0", Fr.RightArrow, "\xa0\xa0", (0, Kr.jsx)("a", {
-                                            href: "".concat(r.server, "/access-keys/").concat(r.key, "/"),
-                                            style: {
-                                                color: o
-                                            },
-                                            target: "_blank",
-                                            children: "View"
-                                        })]
                                     }), (0, Kr.jsx)("small", {
                                         style: {
                                             float: "right",
                                             marginRight: "-10pt"
                                         },
                                         children: (0, Kr.jsx)("b", {
                                             children: f ? (0, Kr.jsx)(Kr.Fragment, {
@@ -49312,18 +49295,27 @@
                                             })
                                         })
                                     })]
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
-                                    children: "Access Key Secret:"
-                                }), (0, Kr.jsx)("td", {
+                                    children: "Access Key:"
+                                }), (0, Kr.jsxs)("td", {
                                     style: i,
-                                    children: r.secret
+                                    children: [r.key, Br.IsLoggedIn(n) && (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: ["\xa0\xa0", Fr.RightArrow, "\xa0\xa0", (0, Kr.jsx)("a", {
+                                            href: "".concat(r.server, "/access-keys/").concat(r.key, "/"),
+                                            style: {
+                                                color: o
+                                            },
+                                            target: "_blank",
+                                            children: "View"
+                                        })]
+                                    })]
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Creation Date:"
                                 }), (0, Kr.jsxs)("td", {
                                     style: i,
```

### Comparing `foursight_core-4.1.0.5b50/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.5b51/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/routes.py` & `foursight_core-4.1.0.5b51/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/run_result.py` & `foursight_core-4.1.0.5b51/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/s3_connection.py` & `foursight_core-4.1.0.5b51/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.5b51/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.5b51/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.5b51/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.5b51/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/stage.py` & `foursight_core-4.1.0.5b51/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/base.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/header.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/history.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/info.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/unused.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/user.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/users.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.5b51/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b50/pyproject.toml` & `foursight_core-4.1.0.5b51/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.0.5b50"
+version = "4.1.0.5b51"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
 click = "^7.1.2"
 cron-descriptor = "^1.2.31"
 cryptography = "39.0.2" # Required for AWS Cognito JWT decode (PyJWKClient)
-dcicutils = "7.3.0.1b21"
+dcicutils = "7.3.0.1b36"
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 geocoder = "1.38.1"
 gitpython = "^3.1.2"
 google = "^3.0.0"
 google-auth-oauthlib = "^0.7.0"
 google-api-python-client = "^1.12.5"
```

### Comparing `foursight_core-4.1.0.5b50/PKG-INFO` & `foursight_core-4.1.0.5b51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.0.5b50
+Version: 4.1.0.5b51
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
 Requires-Dist: cryptography (==39.0.2)
-Requires-Dist: dcicutils (==7.3.0.1b21)
+Requires-Dist: dcicutils (==7.3.0.1b36)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
```

