# Comparing `tmp/evolved5g-1.0.2.tar.gz` & `tmp/evolved5g-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evolved5g-1.0.2.tar", last modified: Thu Mar  9 15:32:49 2023, max compression
+gzip compressed data, was "evolved5g-1.0.3.tar", last modified: Wed Apr 26 07:38:20 2023, max compression
```

## Comparing `evolved5g-1.0.2.tar` & `evolved5g-1.0.3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.689331 evolved5g-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-03-09 15:32:17.000000 evolved5g-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-03-09 15:32:17.000000 evolved5g-1.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-09 15:32:17.000000 evolved5g-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-09 15:32:17.000000 evolved5g-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-03-09 15:32:49.689331 evolved5g-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-09 15:32:17.000000 evolved5g-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.673330 evolved5g-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.677330 evolved5g-1.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.677330 evolved5g-1.0.2/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/dummy_html_example.png
--rw-r--r--   0 runner    (1001) docker     (123)   416176 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/generate.gif
--rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/generate_execution.png
--rw-r--r--   0 runner    (1001) docker     (123)    31097 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/repo_creation.png
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/repo_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/ssh_gpg.png
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/ssh_key.png
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/ssh_key_button.png
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/token1.png
--rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/token2.png
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/images/token3.png
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/information.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/libraries.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-03-09 15:32:17.000000 evolved5g-1.0.2/docs/source/pre_requisites.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.677330 evolved5g-1.0.2/evolved5g/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/cli_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    79623 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.681330 evolved5g-1.0.2/evolved5g/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.681330 evolved5g-1.0.2/evolved5g/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/cells_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/g_n_bs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/location_frontend_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/login_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/monitoring_event_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/paths_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/qo_s_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/u_es_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/ui_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api/utils_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.689331 evolved5g-1.0.2/evolved5g/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/accumulated_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_u_es_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_ue_create_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_ue_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_ue_update_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/cell_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/cell_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/gnb_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/gnb_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/location_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_report_received.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/path_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/path_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/qo_s_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/qos_monitoring_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/reporting_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/snssai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/u_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/ue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/ue_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/ue_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/usage_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/user_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/user_plane_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/user_plane_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/user_plane_notification_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/user_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-09 15:32:17.000000 evolved5g-1.0.2/evolved5g/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:32:49.681330 evolved5g-1.0.2/evolved5g.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-03-09 15:32:49.000000 evolved5g-1.0.2/evolved5g.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-03-09 15:32:49.000000 evolved5g-1.0.2/evolved5g.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:32:49.000000 evolved5g-1.0.2/evolved5g.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-09 15:32:49.000000 evolved5g-1.0.2/evolved5g.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:32:46.000000 evolved5g-1.0.2/evolved5g.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-09 15:32:49.000000 evolved5g-1.0.2/evolved5g.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-09 15:32:49.000000 evolved5g-1.0.2/evolved5g.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-09 15:32:17.000000 evolved5g-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-09 15:32:49.689331 evolved5g-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-09 15:32:17.000000 evolved5g-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.074720 evolved5g-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-26 07:37:46.000000 evolved5g-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-26 07:37:46.000000 evolved5g-1.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 07:37:46.000000 evolved5g-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-26 07:37:46.000000 evolved5g-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-04-26 07:38:20.074720 evolved5g-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-26 07:37:46.000000 evolved5g-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.062720 evolved5g-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.062720 evolved5g-1.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.062720 evolved5g-1.0.3/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/dummy_html_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   416176 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/generate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/generate_execution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31097 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/repo_creation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/repo_structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/ssh_gpg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/ssh_key.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/ssh_key_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/token1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/token2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/images/token3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/information.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/libraries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-26 07:37:46.000000 evolved5g-1.0.3/docs/source/pre_requisites.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.066720 evolved5g-1.0.3/evolved5g/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/cli_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88851 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.066720 evolved5g-1.0.3/evolved5g/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.066720 evolved5g-1.0.3/evolved5g/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/cells_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/g_n_bs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/location_frontend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/login_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/monitoring_event_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/paths_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/qo_s_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/u_es_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/ui_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api/utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.074720 evolved5g-1.0.3/evolved5g/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/accumulated_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_u_es_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_ue_create_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_ue_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_ue_update_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/cell_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/cell_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/gnb_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/gnb_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/location_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_report_received.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/path_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/path_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/qo_s_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/qos_monitoring_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/reporting_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/snssai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/u_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/ue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/ue_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/ue_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/usage_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/user_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/user_plane_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/user_plane_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/user_plane_notification_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/user_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-26 07:37:46.000000 evolved5g-1.0.3/evolved5g/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:20.066720 evolved5g-1.0.3/evolved5g.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-04-26 07:38:20.000000 evolved5g-1.0.3/evolved5g.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-26 07:38:20.000000 evolved5g-1.0.3/evolved5g.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:38:20.000000 evolved5g-1.0.3/evolved5g.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 07:38:20.000000 evolved5g-1.0.3/evolved5g.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:38:16.000000 evolved5g-1.0.3/evolved5g.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 07:38:20.000000 evolved5g-1.0.3/evolved5g.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 07:38:20.000000 evolved5g-1.0.3/evolved5g.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 07:37:46.000000 evolved5g-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 07:38:20.074720 evolved5g-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-26 07:37:46.000000 evolved5g-1.0.3/setup.py
```

### Comparing `evolved5g-1.0.2/CONTRIBUTING.rst` & `evolved5g-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/HISTORY.rst` & `evolved5g-1.0.3/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 =======
 History
 =======
 
 -------------------
+1.0.3 (2023-04-25)
+-------------------
+* New SDK Class CAPIFLogger, that allows a provider (like NEF Emulator) to save Log information, for example capture incoming requests and responses
+* New SDK Class CAPIFAuditor, that allows a provider (like NEF Emulator) to query the Log, for example filter all the Log information for a given Network APP
+* Added examples of usage for CAPIFLogger and CAPIFAuditor class in examples/nef_logger_and_audit_example.py
+* At CAPIFProviderConnector class when using the publish_services() method, a copy of the published to CAPIF api is saved to the local certificates folder. This is useful if you want to retrieve the relevant CAPIF ids for this service like aef_id or api_id.
+
+-------------------
 1.0.2 (2023-03-09)
 -------------------
-* Bug fix on minimum python version. Change it from 3.6 to 3.7. Installing the SDK in older ubuntu distribution raises an error at runtime requiring higher python version coming from Cookiecutter. 
+* Update TSN Manager class, apply security improvements.  Now each request to the TSN API uses JWT Bearer authentication. Access tokens are retrieved via CAPIF.
+* Bug fix on minimum python version. Change it from 3.6 to 3.7. Installing the SDK in older ubuntu distribution raises an error at runtime requiring higher python version coming from Cookiecutter.
 
 -------------------
 1.0.1 (2023-03-03)
 -------------------
 * Bug fix on CAPIFProviderConnector: If you run it twice (for example for testing purposes) the .pem certificate should be overriden.
 
 -------------------
```

### Comparing `evolved5g-1.0.2/LICENSE` & `evolved5g-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/PKG-INFO` & `evolved5g-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.2
+Version: 1.0.3
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,17 +54,26 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.3 (2023-04-25)
+        -------------------
+        * New SDK Class CAPIFLogger, that allows a provider (like NEF Emulator) to save Log information, for example capture incoming requests and responses
+        * New SDK Class CAPIFAuditor, that allows a provider (like NEF Emulator) to query the Log, for example filter all the Log information for a given Network APP
+        * Added examples of usage for CAPIFLogger and CAPIFAuditor class in examples/nef_logger_and_audit_example.py
+        * At CAPIFProviderConnector class when using the publish_services() method, a copy of the published to CAPIF api is saved to the local certificates folder. This is useful if you want to retrieve the relevant CAPIF ids for this service like aef_id or api_id.
+        
+        -------------------
         1.0.2 (2023-03-09)
         -------------------
-        * Bug fix on minimum python version. Change it from 3.6 to 3.7. Installing the SDK in older ubuntu distribution raises an error at runtime requiring higher python version coming from Cookiecutter. 
+        * Update TSN Manager class, apply security improvements.  Now each request to the TSN API uses JWT Bearer authentication. Access tokens are retrieved via CAPIF.
+        * Bug fix on minimum python version. Change it from 3.6 to 3.7. Installing the SDK in older ubuntu distribution raises an error at runtime requiring higher python version coming from Cookiecutter.
         
         -------------------
         1.0.1 (2023-03-03)
         -------------------
         * Bug fix on CAPIFProviderConnector: If you run it twice (for example for testing purposes) the .pem certificate should be overriden.
         
         -------------------
```

### Comparing `evolved5g-1.0.2/README.rst` & `evolved5g-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/Makefile` & `evolved5g-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/make.bat` & `evolved5g-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/cli.rst` & `evolved5g-1.0.3/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/conf.py` & `evolved5g-1.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/dummy_html_example.png` & `evolved5g-1.0.3/docs/source/images/dummy_html_example.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/generate.gif` & `evolved5g-1.0.3/docs/source/images/generate.gif`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/generate_execution.png` & `evolved5g-1.0.3/docs/source/images/generate_execution.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/repo_creation.png` & `evolved5g-1.0.3/docs/source/images/repo_creation.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/repo_structure.png` & `evolved5g-1.0.3/docs/source/images/repo_structure.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/ssh_gpg.png` & `evolved5g-1.0.3/docs/source/images/ssh_gpg.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/ssh_key.png` & `evolved5g-1.0.3/docs/source/images/ssh_key.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/ssh_key_button.png` & `evolved5g-1.0.3/docs/source/images/ssh_key_button.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/token1.png` & `evolved5g-1.0.3/docs/source/images/token1.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/token2.png` & `evolved5g-1.0.3/docs/source/images/token2.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/images/token3.png` & `evolved5g-1.0.3/docs/source/images/token3.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/index.rst` & `evolved5g-1.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/information.rst` & `evolved5g-1.0.3/docs/source/information.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/installation.rst` & `evolved5g-1.0.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/libraries.rst` & `evolved5g-1.0.3/docs/source/libraries.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 
 At the current release the SDK contains six classes
 
 * **LocationSubscriber**: allows you to track devices and retrieve updates about their location.You can use LocationSubscriber to create subscriptions, where each one of them can be used to track a device.
 * **QosAwareness**: allows you to request QoS from a set of standardized values for better service experience (Ex. TCP_BASED / LIVE Streaming / CONVERSATIONAL_VOICE etc). You can create subscriptions where each one of them has specific QoS parameters. A notification is sent back to the net-app if the QoS targets can no longer be full-filled.
 * **ConnectionMonitor**: allows you to monitor devices in the 5G Network. You can use this class to retrieve notifications by the 5G Network for individual devices when connection is lost (for example the user device has not been connected to the 5G network for the past 10 seconds) or when connection is alive.
-* **TSNManager** allows NetApp developers to apply Time-Sensitive Networking (TSN) standards to time-sensitive NetApps. Allows the configuration of certain parameters in the underlying TSN infrastructure of the testbed.
+* **TSNManager** allows Network App developers to apply Time-Sensitive Networking (TSN) standards to time-sensitive NetApps. Allows the configuration of certain parameters in the underlying TSN infrastructure of the testbed.
 * **CAPIFInvokerConnector** a low level class, that is used by the evolved-5G CLI in order to register NetApps to CAPIF
-* **ServiceDiscoverer** allows NetApp developers to connect to CAPIF in order to discover services. It's also used internally within the SDK in order to get access token from CAPIF before interacting with services like NEF or CAPIF.
+* **ServiceDiscoverer** allows Network App developers to connect to CAPIF in order to discover services. It's also used internally within the SDK in order to get access token from CAPIF before interacting with services like NEF or CAPIF.
 * **CAPIFProviderConnector** a low level class, that allows an Exposer (like the NEF emulator or the TSN emulator) to register to CAPIF
+* **CAPIFLogger**, that allows an API provider (like NEF Emulator) to save Log information, for example capture incoming requests and responses
+* **CAPIFAuditor**, that allows an API provider (like NEF Emulator) to query the Log, for example filter all the Log information for a given Network APP
 
 
 
 Examples of usage /Have a look at the code
 ------------------------------------------
 Have a look at the examples folder for code samples on how to use the SDK Library.
 
@@ -22,20 +24,25 @@
 
 * `QosAwareness example <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/qos_awereness_examples.py>`_
 
 * `ConnectionMonitor example <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/connection_monitor_examples.py>`_
 
 * `CAPIFInvokerConnector example <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/netapp_capif_connector_examples.py>`_
 
-* `CAPIFProviderConnector example at <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/nef_capif_connector_examples.py> and <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/tsn_capif_connector_examples.py>`_
+* `CAPIFProviderConnector example for NEF <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/nef_capif_connector_examples.py>`_
+* `CAPIFProviderConnector example for TSN <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/tsn_capif_connector_examples.py>`_
 
 * `ServiceDiscoverer example <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/netapp_service_discovery_examples.py>`_
 
 * `TSNManager example <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/tsn_manager_examples.py>`_
 
+* `CAPIFLogger example <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/nef_logger_and_audit_example.py>`_
+
+* `CAPIFAuditor  example <https://github.com/EVOLVED-5G/SDK-CLI/blob/master/examples/nef_logger_and_audit_example.py>`_
+
 
 Prerequisites / How to start
 ----------------------------
 
 Install the requirements_dev.txt
 
 .. code-block:: console
@@ -45,15 +52,15 @@
 Make sure you have initiated the CAPIF server  (See  `here <https://github.com/EVOLVED-5G/CAPIF_API_Services>`_ for instructions).
 
 Make sure you have initiated the TSN server  (See  `here <https://github.com/EVOLVED-5G/TSN_AF>`_ for instructions).
 
 Make sure you have initiated the NEF_EMULATOR at url :py:func:`http://localhost:8888` (See  `here <https://github.com/EVOLVED-5G/NEF_emulator>`_  for instructions),
 you have logged in to the interface, clicked on the map and have started the simulation.
 
-Make sure that your NetApp has been registered and onboarded to CAPIF. If this process is completed, then in the specified folder the following files should be present
+Make sure that your Network App has been registered and onboarded to CAPIF. If this process is completed, then in the specified folder the following files should be present
 
     - ca.crt
     - capif_api_details.json
     - private.key
     - your_common_name_you_specified.crt
 
 Then run a webserver in order to capture the callback post requests from NEF EMULATOR: On the terminal run the following commands to initialize the webserver.
@@ -84,15 +91,15 @@
 (you should be able to retrieve notifications when user devices connect or disconnect to the netowrk,  printed in the terminal that runs the FLASK webserver)
 
 ConnectionMonitor Library
 ----------------------------
 
 Overview
 ###################
-ConnectionMonitor library supports two events as described briefly above. The first event is the loss of connectivity event where the network detects that a UE is no longer reachable for either signalling or user plane communication. The NetApp may provide a Maximum Detection Time, which indicates the maximum period of time without any communication with the UE (after the UE is considered to be unreachable by the network). The respective monitoring type enumeration and the maximum detection time parameter are shown below:
+ConnectionMonitor library supports two events as described briefly above. The first event is the loss of connectivity event where the network detects that a UE is no longer reachable for either signalling or user plane communication. The Network App may provide a Maximum Detection Time, which indicates the maximum period of time without any communication with the UE (after the UE is considered to be unreachable by the network). The respective monitoring type enumeration and the maximum detection time parameter are shown below:
 
 .. code-block:: console
 
    monitoring_type= ConnectionMonitor.MonitoringType.INFORM_WHEN_NOT_CONNECTED
    wait_time_before_sending_notification_in_seconds=5
 
 The second event is the ue reachability event where the network detects when the UE becomes reachable (for sending downlink data or SMS to the UE). The monitoring type enumeration is shown below:
@@ -100,14 +107,14 @@
 .. code-block:: console
 
    monitoring_type= ConnectionMonitor.MonitoringType.INFORM_WHEN_CONNECTED
 
 Prerequisite
 ###################
 
-❗An important prerequisite for the loss of connectivity event (INFORM_WHEN_NOT_CONNECTED) is that while a NetApp successfully receives the callback notification from the NEF Emulator, subsequently NEF expects an ``HTTP Response`` with the ``JSON`` content shown below:
+❗An important prerequisite for the loss of connectivity event (INFORM_WHEN_NOT_CONNECTED) is that while a Network App successfully receives the callback notification from the NEF Emulator, subsequently NEF expects an ``HTTP Response`` with the ``JSON`` content shown below:
 
 .. code-block:: console
 
    {"ack" : "TRUE"}
 
-As a result, the developer should ensure that in the endpoint that is responsible for receiving the callback notifications (HTTP POST requests) from NEF, NetApp always returns the aforementioned acknowledgement, in ``JSON`` format.
+As a result, the developer should ensure that in the endpoint that is responsible for receiving the callback notifications (HTTP POST requests) from NEF, Network App always returns the aforementioned acknowledgement, in ``JSON`` format.
```

### Comparing `evolved5g-1.0.2/docs/source/pipelines.rst` & `evolved5g-1.0.3/docs/source/pipelines.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/docs/source/pre_requisites.rst` & `evolved5g-1.0.3/docs/source/pre_requisites.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/cli.py` & `evolved5g-1.0.3/evolved5g/cli.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/cli_helper.py` & `evolved5g-1.0.3/evolved5g/cli_helper.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/sdk.py` & `evolved5g-1.0.3/evolved5g/sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """SDK module"""
 import os
 from typing import List
 
 from evolved5g import swagger_client
 from abc import ABC, abstractmethod
 from enum import Enum
+from dataclasses import dataclass
 from evolved5g.swagger_client import (
     MonitoringEventAPIApi,
     MonitoringEventSubscriptionCreate,
     MonitoringEventSubscription,
     SessionWithQoSAPIApi,
     AsSessionWithQoSSubscriptionCreate,
     Snssai,
@@ -37,47 +38,54 @@
 import json
 from uuid import uuid4
 import warnings
 
 
 class MonitoringSubscriber(ABC):
     def __init__(
-        self,
-        host: str,
-        nef_bearer_access_token: str,
-        folder_path_for_certificates_and_capif_api_key: str,
-        capif_host: str,
-        capif_https_port: int,
+            self,
+            host: str,
+            nef_bearer_access_token: str,
+            folder_path_for_certificates_and_capif_api_key: str,
+            capif_host: str,
+            capif_https_port: int,
     ):
         configuration = swagger_client.Configuration()
         configuration.verify_ssl = False
         configuration.host = host
-        service_discoverer = ServiceDiscoverer(folder_path_for_certificates_and_capif_api_key, capif_host, capif_https_port)
+        service_discoverer = ServiceDiscoverer(folder_path_for_certificates_and_capif_api_key, capif_host,
+                                               capif_https_port)
         api_name = "/nef/api/v1/3gpp-monitoring-event/"
         configuration.available_endpoints = {
             "MONITORING_SUBSCRIPTIONS": service_discoverer.retrieve_specific_resource_name(api_name,
                                                                                            "MONITORING_SUBSCRIPTIONS"),
             "MONITORING_SUBSCRIPTION_SINGLE": service_discoverer.retrieve_specific_resource_name(api_name,
                                                                                                  "MONITORING_SUBSCRIPTION_SINGLE"),
         }
         api_resource_description = service_discoverer.retrieve_api_description_by_name(api_name)
-        configuration.access_token = nef_bearer_access_token + "," + service_discoverer.get_access_token(api_name,api_resource_description["apiId"],api_resource_description["aefProfiles"][0]["aefId"])
+        configuration.access_token = nef_bearer_access_token + "," + service_discoverer.get_access_token(api_name,
+                                                                                                         api_resource_description[
+                                                                                                             "apiId"],
+                                                                                                         api_resource_description[
+                                                                                                             "aefProfiles"][
+                                                                                                             0][
+                                                                                                             "aefId"])
         api_client = swagger_client.ApiClient(configuration=configuration)
         self.monitoring_event_api = MonitoringEventAPIApi(api_client)
         self.cell_api = CellsApi(api_client)
 
     def create_subscription_request(
-        self,
-        monitoring_type,
-        external_id,
-        notification_destination,
-        maximum_number_of_reports,
-        monitor_expire_time,
-        maximum_detection_time,
-        reachability_type,
+            self,
+            monitoring_type,
+            external_id,
+            notification_destination,
+            maximum_number_of_reports,
+            monitor_expire_time,
+            maximum_detection_time,
+            reachability_type,
     ) -> MonitoringEventSubscriptionCreate:
         return MonitoringEventSubscriptionCreate(
             external_id,
             notification_destination,
             monitoring_type,
             maximum_number_of_reports,
             monitor_expire_time,
@@ -95,15 +103,15 @@
         """
 
         return self.monitoring_event_api.read_active_subscriptions_api_v13gpp_monitoring_event_v1_scs_as_id_subscriptions_get(
             netapp_id, skip=skip, limit=limit
         )
 
     def get_subscription(
-        self, netapp_id: str, subscription_id: str
+            self, netapp_id: str, subscription_id: str
     ) -> MonitoringEventSubscription:
         """
         Gets subscription by id
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str subscription_id: string (Identifier of the subscription resource)
         """
@@ -121,20 +129,20 @@
         return self.monitoring_event_api.delete_subscription_api_v13gpp_monitoring_event_v1_scs_as_id_subscriptions_subscription_id_delete(
             netapp_id, subscription_id
         )
 
 
 class LocationSubscriber(MonitoringSubscriber):
     def __init__(
-        self,
-        nef_url: str,
-        nef_bearer_access_token: str,
-        folder_path_for_certificates_and_capif_api_key: str,
-        capif_host: str,
-        capif_https_port: int,
+            self,
+            nef_url: str,
+            nef_bearer_access_token: str,
+            folder_path_for_certificates_and_capif_api_key: str,
+            capif_host: str,
+            capif_https_port: int,
     ):
         """
         Initializes class LocationSubscriber.
         This SKD class allows you to track devices and retrieve updates about their location.
         You can create subscriptions where each one of them can be used to track a device.
         A notification is sent to a callback url you will provide, everytime the user device changes Cell
 
@@ -148,27 +156,27 @@
             capif_https_port,
         )
 
     def __get_monitoring_type(self):
         return "LOCATION_REPORTING"
 
     def get_location_information(
-        self, netapp_id: str, external_id
+            self, netapp_id: str, external_id
     ) -> MonitoringEventReport:
         """
         Returns the location of a specific device.
         This is equivalent to creating a subscription with maximum_number_of_reports = 1
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str external_id: Globally unique identifier containing a Domain Identifier and a Local Identifier. <Local Identifier>@<Domain Identifier>
         """
 
         # create a dummy expiration time. Since we are requesting for only 1 report, we will get the location information back instantly
         monitor_expire_time = (
-            datetime.datetime.utcnow() + datetime.timedelta(minutes=1)
-        ).isoformat() + "Z"
+                                      datetime.datetime.utcnow() + datetime.timedelta(minutes=1)
+                              ).isoformat() + "Z"
         body = self.create_subscription_request(
             self.__get_monitoring_type(),
             external_id,
             None,
             maximum_number_of_reports=1,
             monitor_expire_time=monitor_expire_time,
             maximum_detection_time=None,
@@ -186,20 +194,20 @@
         Returns information about a specific cell
 
         :param str cell_id: string (The ID of the cell)
         """
         return self.cell_api.read_cell_api_v1_cells_cell_id_get(cell_id)
 
     def create_subscription(
-        self,
-        netapp_id: str,
-        external_id,
-        notification_destination,
-        maximum_number_of_reports,
-        monitor_expire_time,
+            self,
+            netapp_id: str,
+            external_id,
+            notification_destination,
+            maximum_number_of_reports,
+            monitor_expire_time,
     ) -> MonitoringEventSubscription:
         """
         Creates a subscription that will be used to retrieve Location information about a device.
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str external_id: Globally unique identifier containing a Domain Identifier and a Local Identifier. <Local Identifier>@<Domain Identifier>
         :param notification_destination: The url that you will notifications about the location of the user
@@ -219,21 +227,21 @@
         # a monitoring event report
         response = self.monitoring_event_api.create_subscription_api_v13gpp_monitoring_event_v1_scs_as_id_subscriptions_post(
             body, netapp_id
         )
         return response
 
     def update_subscription(
-        self,
-        netapp_id: str,
-        subscription_id: str,
-        external_id,
-        notification_destination,
-        maximum_number_of_reports,
-        monitor_expire_time,
+            self,
+            netapp_id: str,
+            subscription_id: str,
+            external_id,
+            notification_destination,
+            maximum_number_of_reports,
+            monitor_expire_time,
     ) -> MonitoringEventSubscription:
         """
         Creates a subscription that will be used to retrieve Location information about a device.
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str subscription_id: string (Identifier of the subscription resource)
         :param str external_id: Globally unique identifier containing a Domain Identifier and a Local Identifier. <Local Identifier>@<Domain Identifier>
@@ -264,20 +272,20 @@
         If INFORM_WHEN_NOT_CONNECTED is selected then the 5G API will send you a notification is the device has not been connected to the 5G Network for the past X seconds
         """
 
         INFORM_WHEN_CONNECTED = 1
         INFORM_WHEN_NOT_CONNECTED = 2
 
     def __init__(
-        self,
-        nef_url: str,
-        nef_bearer_access_token:str,
-        folder_path_for_certificates_and_capif_api_key: str,
-        capif_host: str,
-        capif_https_port: int,
+            self,
+            nef_url: str,
+            nef_bearer_access_token: str,
+            folder_path_for_certificates_and_capif_api_key: str,
+            capif_host: str,
+            capif_https_port: int,
     ):
         """
         Initializes class ConnectionMonitor.
         Consider a scenario where a NetApp wants to monitor 100 devices in the 5G Network.
         The netapp wants to track, at any given time how many NetApps are connected to the 5G Network and how many netApps are disconnected.
 
         Using ConnectionMonitor the NetApp can retrieve notifications by the 5G Network for individual devices when
@@ -301,22 +309,22 @@
     def __get_monitoring_type(self, monitoring_type: MonitoringType):
         if monitoring_type == self.MonitoringType.INFORM_WHEN_CONNECTED:
             return "UE_REACHABILITY"
         else:
             return "LOSS_OF_CONNECTIVITY"
 
     def create_subscription(
-        self,
-        netapp_id: str,
-        external_id,
-        notification_destination,
-        monitoring_type: MonitoringType,
-        wait_time_before_sending_notification_in_seconds: int,
-        maximum_number_of_reports,
-        monitor_expire_time,
+            self,
+            netapp_id: str,
+            external_id,
+            notification_destination,
+            monitoring_type: MonitoringType,
+            wait_time_before_sending_notification_in_seconds: int,
+            maximum_number_of_reports,
+            monitor_expire_time,
     ) -> MonitoringEventSubscription:
         """
         Creates a subscription that will be used to track the Network Connectivity about a device.
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str external_id: Globally unique identifier containing a Domain Identifier and a Local Identifier. <Local Identifier>@<Domain Identifier>
         :param notification_destination: The url that you will retrieve notifications when a device is connected or not connected for the past X seconds
@@ -345,23 +353,23 @@
         # a monitoring event report
         response = self.monitoring_event_api.create_subscription_api_v13gpp_monitoring_event_v1_scs_as_id_subscriptions_post(
             body, netapp_id
         )
         return response
 
     def update_subscription(
-        self,
-        netapp_id: str,
-        subscription_id: str,
-        external_id,
-        notification_destination,
-        monitoring_type: MonitoringType,
-        wait_time_before_sending_notification_in_seconds: int,
-        maximum_number_of_reports,
-        monitor_expire_time,
+            self,
+            netapp_id: str,
+            subscription_id: str,
+            external_id,
+            notification_destination,
+            monitoring_type: MonitoringType,
+            wait_time_before_sending_notification_in_seconds: int,
+            maximum_number_of_reports,
+            monitor_expire_time,
     ) -> MonitoringEventSubscription:
         """
         Creates a subscription that will be used to retrieve Location information about a device.
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str subscription_id: string (Identifier of the subscription resource)
         :param str external_id: Globally unique identifier containing a Domain Identifier and a Local Identifier. <Local Identifier>@<Domain Identifier>
@@ -493,20 +501,20 @@
         def get_reporting_mode(self):
             return ReportingFrequency.PERIODIC
 
         def get_reporting_configuration(self):
             return self.repetition_period_in_seconds
 
     def __init__(
-        self,
-        nef_url: str,
-        nef_bearer_access_token: str,
-        folder_path_for_certificates_and_capif_api_key: str,
-        capif_host: str,
-        capif_https_port: int,
+            self,
+            nef_url: str,
+            nef_bearer_access_token: str,
+            folder_path_for_certificates_and_capif_api_key: str,
+            capif_host: str,
+            capif_https_port: int,
     ):
         """
         Initializes class QosAwareness.
         This SKD class allows you to request QoS from a set of standardized values for better service experience.
 
         You can create subscriptions where each one of them has specific QoS parameters.
         A notification is sent to a callback url you will provide, informing you in case the QoS targets can no
@@ -533,27 +541,33 @@
                 api_name, "QOS_SUBSCRIPTIONS"
             ),
             "QOS_SUBSCRIPTION_SINGLE": service_discoverer.retrieve_specific_resource_name(
                 api_name, "QOS_SUBSCRIPTION_SINGLE"
             ),
         }
         api_resource_description = service_discoverer.retrieve_api_description_by_name(api_name)
-        configuration.access_token =nef_bearer_access_token + "," + service_discoverer.get_access_token(api_name,api_resource_description["apiId"],api_resource_description["aefProfiles"][0]["aefId"])
+        configuration.access_token = nef_bearer_access_token + "," + service_discoverer.get_access_token(api_name,
+                                                                                                         api_resource_description[
+                                                                                                             "apiId"],
+                                                                                                         api_resource_description[
+                                                                                                             "aefProfiles"][
+                                                                                                             0][
+                                                                                                             "aefId"])
         api_client = swagger_client.ApiClient(configuration=configuration)
         self.qos_api = SessionWithQoSAPIApi(api_client)
 
     def create_subscription_request(
-        self,
-        equipment_network_identifier: str,
-        network_identifier: NetworkIdentifier,
-        notification_destination: str,
-        qos_reference: int,
-        alt_qo_s_references,
-        usage_threshold: UsageThreshold,
-        qos_mon_info,
+            self,
+            equipment_network_identifier: str,
+            network_identifier: NetworkIdentifier,
+            notification_destination: str,
+            qos_reference: int,
+            alt_qo_s_references,
+            usage_threshold: UsageThreshold,
+            qos_mon_info,
     ) -> AsSessionWithQoSSubscriptionCreate:
         ip4_address_value = (
             equipment_network_identifier
             if network_identifier == QosAwareness.NetworkIdentifier.IP_V4_ADDRESS
             else None
         )
         ip6_address_value = (
@@ -584,21 +598,21 @@
             qos_reference=qos_reference,
             alt_qo_s_references=alt_qo_s_references,
             usage_threshold=usage_threshold,
             qos_mon_info=qos_mon_info,
         )
 
     def create_non_guaranteed_bit_rate_subscription(
-        self,
-        netapp_id,
-        equipment_network_identifier: str,
-        network_identifier: NetworkIdentifier,
-        notification_destination: str,
-        non_gbr_qos_reference: NonGBRQosReference,
-        usage_threshold: UsageThreshold,
+            self,
+            netapp_id,
+            equipment_network_identifier: str,
+            network_identifier: NetworkIdentifier,
+            notification_destination: str,
+            non_gbr_qos_reference: NonGBRQosReference,
+            usage_threshold: UsageThreshold,
     ) -> AsSessionWithQoSSubscription:
         """
         Initializes a Non Guaranteed Bit Rate (NGBR) Quality of Service (QoS) subscription.
         This is useful for TCP based or Live Streaming scenarios.
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param equipment_network_identifier: The IP 4 address or IP 6 address or Mac address of the user device / equiment.
@@ -624,22 +638,22 @@
 
         response = self.qos_api.create_subscription_api_v13gpp_as_session_with_qos_v1_scs_as_id_subscriptions_post(
             body, netapp_id
         )
         return response
 
     def update_non_guaranteed_bit_rate_subscription(
-        self,
-        netapp_id: str,
-        subscription_id: str,
-        equipment_network_identifier: str,
-        network_identifier: NetworkIdentifier,
-        notification_destination: str,
-        non_gbr_qos_reference: NonGBRQosReference,
-        usage_threshold: UsageThreshold,
+            self,
+            netapp_id: str,
+            subscription_id: str,
+            equipment_network_identifier: str,
+            network_identifier: NetworkIdentifier,
+            notification_destination: str,
+            non_gbr_qos_reference: NonGBRQosReference,
+            usage_threshold: UsageThreshold,
     ) -> AsSessionWithQoSSubscription:
         """
         Updates a given subscription.
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str subscription_id: string (Identifier of the subscription resource)
         :param equipment_network_identifier: The IP 4 address or IP 6 address or Mac address of the user device / equiment.
@@ -664,24 +678,24 @@
         )
 
         return self.qos_api.update_subscription_api_v13gpp_as_session_with_qos_v1_scs_as_id_subscriptions_subscription_id_put(
             body, netapp_id, subscription_id
         )
 
     def create_guaranteed_bit_rate_subscription(
-        self,
-        netapp_id,
-        equipment_network_identifier,
-        network_identifier,
-        notification_destination: str,
-        gbr_qos_reference: GBRQosReference,
-        usage_threshold: UsageThreshold,
-        qos_monitoring_parameter: QosMonitoringParameter,
-        threshold: int,
-        reporting_mode: GuaranteedBitRateReportingMode,
+            self,
+            netapp_id,
+            equipment_network_identifier,
+            network_identifier,
+            notification_destination: str,
+            gbr_qos_reference: GBRQosReference,
+            usage_threshold: UsageThreshold,
+            qos_monitoring_parameter: QosMonitoringParameter,
+            threshold: int,
+            reporting_mode: GuaranteedBitRateReportingMode,
     ) -> AsSessionWithQoSSubscription:
 
         """
         Initializes a Guaranteed Bit Rate (NGBR) Quality of Service (QoS) subscription.
         This is useful for Conversational Voice / Video or Discrete automation scenarios.
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
@@ -719,19 +733,19 @@
 
         response = self.qos_api.create_subscription_api_v13gpp_as_session_with_qos_v1_scs_as_id_subscriptions_post(
             body, netapp_id
         )
         return response
 
     def __create_gbr_request_qo_parameters(
-        self,
-        gbr_qos_reference,
-        qos_monitoring_parameter,
-        threshold,
-        reporting_mode: GuaranteedBitRateReportingMode,
+            self,
+            gbr_qos_reference,
+            qos_monitoring_parameter,
+            threshold,
+            reporting_mode: GuaranteedBitRateReportingMode,
     ):
         # Contains the remaining Guaranted Qos references, as fallback
         alt_qo_s_references = []
         for qos_reference in QosAwareness.GBRQosReference:
             if qos_reference != gbr_qos_reference:
                 alt_qo_s_references.append(qos_reference.value)
         # User has to specify
@@ -752,15 +766,15 @@
         )
 
         reporting_freqs = [reporting_mode.get_reporting_mode()]
         wait_time = None
         rep_period = None
 
         if isinstance(
-            reporting_mode, QosAwareness.EventTriggeredReportingConfiguration
+                reporting_mode, QosAwareness.EventTriggeredReportingConfiguration
         ):
             wait_time = reporting_mode.get_reporting_configuration()
         else:
             rep_period = reporting_mode.get_reporting_configuration()
 
         qos_monitoring_info = QosMonitoringInformation(
             req_qos_mon_params=[qos_monitoring_parameter.value],
@@ -770,25 +784,25 @@
             lat_thresh_rp=lat_thresh_rp,
             wait_time=wait_time,
             rep_period=rep_period,
         )
         return alt_qo_s_references, qos_monitoring_info
 
     def update_guaranteed_bit_rate_subscription(
-        self,
-        netapp_id: str,
-        subscription_id: str,
-        equipment_network_identifier: str,
-        network_identifier: NetworkIdentifier,
-        notification_destination: str,
-        gbr_qos_reference: GBRQosReference,
-        usage_threshold: UsageThreshold,
-        qos_monitoring_parameter: QosMonitoringParameter,
-        threshold: int,
-        reporting_mode: GuaranteedBitRateReportingMode,
+            self,
+            netapp_id: str,
+            subscription_id: str,
+            equipment_network_identifier: str,
+            network_identifier: NetworkIdentifier,
+            notification_destination: str,
+            gbr_qos_reference: GBRQosReference,
+            usage_threshold: UsageThreshold,
+            qos_monitoring_parameter: QosMonitoringParameter,
+            threshold: int,
+            reporting_mode: GuaranteedBitRateReportingMode,
     ) -> AsSessionWithQoSSubscription:
         """
         Updates a given subscription.
 
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         :param str subscription_id: string (Identifier of the subscription resource)
@@ -824,28 +838,28 @@
             qos_mon_info=qos_monitoring_info,
         )
         return self.qos_api.update_subscription_api_v13gpp_as_session_with_qos_v1_scs_as_id_subscriptions_subscription_id_put(
             body, netapp_id, subscription_id
         )
 
     def get_all_subscriptions(
-        self, netapp_id: str
+            self, netapp_id: str
     ) -> List[AsSessionWithQoSSubscription]:
         """
         Reads all active subscriptions
 
         :param str netapp_id: string (The ID of the Netapp that creates a subscription)
         """
 
         return self.qos_api.read_active_subscriptions_api_v13gpp_as_session_with_qos_v1_scs_as_id_subscriptions_get(
             netapp_id
         )
 
     def get_subscription(
-        self, netapp_id: str, subscription_id: str
+            self, netapp_id: str, subscription_id: str
     ) -> AsSessionWithQoSSubscription:
         """
 
         :param netapp_id:
         :param subscription_id:
         :return:
         """
@@ -867,30 +881,30 @@
 
 class CAPIFInvokerConnector:
     """
     Τhis class is responsbile for onboarding an Invoker (ex. a NetApp) to CAPIF
     """
 
     def __init__(
-        self,
-        folder_to_store_certificates: str,
-        capif_host: str,
-        capif_http_port: str,
-        capif_https_port: str,
-        capif_netapp_username,
-        capif_netapp_password: str,
-        capif_callback_url: str,
-        description: str,
-        csr_common_name: str,
-        csr_organizational_unit: str,
-        csr_organization: str,
-        crs_locality: str,
-        csr_state_or_province_name,
-        csr_country_name,
-        csr_email_address,
+            self,
+            folder_to_store_certificates: str,
+            capif_host: str,
+            capif_http_port: str,
+            capif_https_port: str,
+            capif_netapp_username,
+            capif_netapp_password: str,
+            capif_callback_url: str,
+            description: str,
+            csr_common_name: str,
+            csr_organizational_unit: str,
+            csr_organization: str,
+            crs_locality: str,
+            csr_state_or_province_name,
+            csr_country_name,
+            csr_email_address,
     ):
         """
 
         :param folder_to_store_certificates: The folder where certificates will be stores. Your own certificate,
          along with the certificate root that will be retrieved by the CAPIF server
         :param capif_host: The host of the CAPIF Server. It can be an ip or a domain name (Ex. localhost)
         :param capif_http_port: The port of http port (if None is specified port 80 will be used)
@@ -914,23 +928,21 @@
         # make sure the parameters are str
         capif_http_port = str(capif_http_port)
         capif_https_port = str(capif_https_port)
         if len(capif_http_port) == 0 or int(capif_http_port) == 80:
             self.capif_http_url = "http://" + capif_host.strip() + "/"
         else:
             self.capif_http_url = (
-                "http://" + capif_host.strip() + ":" + capif_http_port.strip() + "/"
+                    "http://" + capif_host.strip() + ":" + capif_http_port.strip() + "/"
             )
 
         if len(capif_https_port) == 0 or int(capif_https_port) == 443:
             self.capif_https_url = "https://" + capif_host.strip() + "/"
         else:
-            self.capif_https_url = (
-                "https://" + capif_host.strip() + ":" + capif_https_port.strip() + "/"
-            )
+            self.capif_https_url = "https://" + capif_host.strip() + ":" + capif_https_port.strip() + "/"
 
         self.capif_callback_url = self.__add_trailing_slash_to_url_if_missing(
             capif_callback_url.strip()
         )
         self.capif_netapp_username = capif_netapp_username
         self.capif_netapp_password = capif_netapp_password
         self.description = description
@@ -1043,15 +1055,15 @@
         response.raise_for_status()
         response_payload = json.loads(response.text)
         ca_root_file = open(self.folder_to_store_certificates + "ca.crt", "wb+")
         ca_root_file.write(bytes(response_payload["ca_root"], "utf-8"))
         return response_payload["access_token"]
 
     def __onboard_netapp_to_capif_and_create_the_signed_certificate(
-        self, public_key, capif_onboarding_url, capif_access_token
+            self, public_key, capif_onboarding_url, capif_access_token
     ):
         url = self.capif_https_url + capif_onboarding_url
         payload_dict = {
             "notificationDestination": self.capif_callback_url,
             "supportedFeatures": "fffffff",
             # TODO: This works fine.  But what about CapifProviderConnector class where we onboard a Provider/Exposer. On onboarding there we dont pass the username. Is this a mistake in the flow? Or a different flow is implemented there
             "apiInvokerInformation": self.csr_common_name,
@@ -1086,15 +1098,15 @@
             )
         )
         certification_file.close()
         return response_payload["apiInvokerId"]
 
     def __write_to_file(self, csr_common_name, api_invoker_id, discover_services_url):
         with open(
-            self.folder_to_store_certificates + "capif_api_details.json", "w"
+                self.folder_to_store_certificates + "capif_api_details.json", "w"
         ) as outfile:
             json.dump(
                 {
                     "csr_common_name": csr_common_name,
                     "api_invoker_id": api_invoker_id,
                     "discover_services_url": discover_services_url,
                 },
@@ -1104,29 +1116,29 @@
 
 class CAPIFProviderConnector:
     """
     Τhis class is responsible for onboarding an exposer (eg. NEF emulator) to CAPIF
     """
 
     def __init__(
-        self,
-        certificates_folder: str,
-        description: str,
-        capif_host: str,
-        capif_http_port: str,
-        capif_https_port: str,
-        capif_netapp_username,
-        capif_netapp_password: str,
-        csr_common_name: str,
-        csr_organizational_unit: str,
-        csr_organization: str,
-        crs_locality: str,
-        csr_state_or_province_name,
-        csr_country_name,
-        csr_email_address,
+            self,
+            certificates_folder: str,
+            description: str,
+            capif_host: str,
+            capif_http_port: str,
+            capif_https_port: str,
+            capif_netapp_username,
+            capif_netapp_password: str,
+            csr_common_name: str,
+            csr_organizational_unit: str,
+            csr_organization: str,
+            crs_locality: str,
+            csr_state_or_province_name,
+            csr_country_name,
+            csr_email_address,
     ):
         """
         :param certificates_folder: The folder where certificates will be created and stored.
         :param description: A short description of the Provider
         :param capif_host:
         :param capif_http_port:
         :param capif_https_port:
@@ -1148,22 +1160,22 @@
         # make sure the parameters are str
         capif_http_port = str(capif_http_port)
         capif_https_port = str(capif_https_port)
         if len(capif_http_port) == 0 or int(capif_http_port) == 80:
             self.capif_http_url = "http://" + capif_host.strip() + "/"
         else:
             self.capif_http_url = (
-                "http://" + capif_host.strip() + ":" + capif_http_port.strip() + "/"
+                    "http://" + capif_host.strip() + ":" + capif_http_port.strip() + "/"
             )
 
         if len(capif_https_port) == 0 or int(capif_https_port) == 443:
             self.capif_https_url = "https://" + capif_host.strip() + "/"
         else:
             self.capif_https_url = (
-                "https://" + capif_host.strip() + ":" + capif_https_port.strip() + "/"
+                    "https://" + capif_host.strip() + ":" + capif_https_port.strip() + "/"
             )
 
         self.capif_host = capif_host.strip()
         self.capif_netapp_username = capif_netapp_username
         self.capif_netapp_password = capif_netapp_password
 
         self.csr_common_name = csr_common_name
@@ -1197,15 +1209,15 @@
 
     def __create_private_and_public_keys(self, api_prov_func_role) -> bytes:
         """
         Creates 2 keys in folder folder_to_store_certificates. An api_prov_func_role_private.key and a api_prov_func_role_private.public.csr key"
         :return: The contents of the public key
         """
         private_key_path = (
-            self.certificates_folder + api_prov_func_role + "_private_key.key"
+                self.certificates_folder + api_prov_func_role + "_private_key.key"
         )
         csr_file_path = self.certificates_folder + api_prov_func_role + "_public.csr"
 
         # create public/private key
         key = PKey()
         key.generate_key(TYPE_RSA, 2048)
 
@@ -1283,15 +1295,14 @@
 
         url = self.capif_http_url + "register"
         payload = dict()
         payload["username"] = self.capif_netapp_username
         payload["password"] = self.capif_netapp_password
         payload["role"] = role
         payload["description"] = self.description
-        # TODO: ASK STAVROS. THIS INFORMATION IS STORED AT CAPIF users collection.  Is it used somewhere else at the capif? Notice it does not have postfixes "AEF/APF/AMF"
         payload["cn"] = self.csr_common_name
 
         response = requests.request(
             "POST",
             url,
             headers={"Content-Type": "application/json"},
             data=json.dumps(payload),
@@ -1323,26 +1334,26 @@
 
         return response_payload["access_token"]
 
     def __write_to_file(self, onboarding_response, capif_registration_id, publish_url):
 
         for func_provile in onboarding_response["apiProvFuncs"]:
             with open(
-                self.certificates_folder
-                + "dummy_"
-                + func_provile["apiProvFuncRole"].lower()
-                + ".crt",
-                "wb",
+                    self.certificates_folder
+                    + "dummy_"
+                    + func_provile["apiProvFuncRole"].lower()
+                    + ".crt",
+                    "wb",
             ) as certification_file:
                 certification_file.write(
                     bytes(func_provile["regInfo"]["apiProvCert"], "utf-8")
                 )
 
         with open(
-            self.certificates_folder + "capif_provider_details.json", "w"
+                self.certificates_folder + "capif_provider_details.json", "w"
         ) as outfile:
             data = {
                 "capif_registration_id": capif_registration_id,
                 "publish_url": publish_url,
             }
             for api_prov_func in onboarding_response["apiProvFuncs"]:
                 key = api_prov_func["apiProvFuncRole"] + "_api_prov_func_id"
@@ -1366,21 +1377,24 @@
         onboarding_response = self.__onboard_exposer_to_capif(
             access_token, capif_onboarding_url
         )
         self.__write_to_file(
             onboarding_response, capif_registration_id, ccf_publish_url
         )
 
-    def publish_services(self, service_api_description_json_full_path) -> None:
+    def publish_services(self, service_api_description_json_full_path) -> dict:
         """
-        :param service_api_description_json_full_path: The full path fo the service_api_description.json that contains
-        the endpoints that will be published
+            :param service_api_description_json_full_path: The full path fo the service_api_description.json that contains
+            the endpoints that will be published
+            :return: The published services dictionary that was saved in CAPIF
+
         """
+
         with open(
-            self.certificates_folder + "capif_provider_details.json", "r"
+                self.certificates_folder + "capif_provider_details.json", "r"
         ) as openfile:
             file = json.load(openfile)
             publish_url = file["publish_url"]
             AEF_api_prov_func_id = file["AEF_api_prov_func_id"]
             APF_api_prov_func_id = file["APF_api_prov_func_id"]
 
         url = self.capif_https_url + publish_url.replace(
@@ -1388,52 +1402,54 @@
         )
 
         with open(service_api_description_json_full_path, "rb") as service_file:
             data = json.load(service_file)
             for profile in data["aefProfiles"]:
                 profile["aefId"] = AEF_api_prov_func_id
 
-            response = requests.request(
-                "POST",
-                url,
-                headers={"Content-Type": "application/json"},
-                data=json.dumps(data),
-                cert=(
-                    # TODO:Ask Stavros should this be named like APF_dummy.crt  or like dummy_apf.crt? Does the naming matters? Also we are passing the APF and not the AMF or the AEF keys?
-                    # When should AMF or AEF be passed? At which scenarios?
-                    # Is it fine that we have hardcoded these?
-                    self.certificates_folder + "dummy_apf.crt",
-                    self.certificates_folder + "APF_private_key.key",
-                ),
-                verify=self.certificates_folder + "ca.crt",
-            )
-            response.raise_for_status()
-            response_payload = json.loads(response.text)
-            return response_payload["apiId"]
+        response = requests.request(
+            "POST",
+            url,
+            headers={"Content-Type": "application/json"},
+            data=json.dumps(data),
+            cert=(
+                self.certificates_folder + "dummy_apf.crt",
+                self.certificates_folder + "APF_private_key.key",
+            ),
+            verify=self.certificates_folder + "ca.crt",
+        )
+        response.raise_for_status()
+        capif_response = response.text
+
+        file_name = os.path.basename(service_api_description_json_full_path)
+        with open(self.certificates_folder + "CAPIF_" + file_name, "w") as outfile:
+            outfile.write(capif_response)
+
+        return json.loads(capif_response)
 
 
 class ServiceDiscoverer:
     class ServiceDiscovererException(Exception):
         pass
 
     def __init__(
-        self,
-        folder_path_for_certificates_and_api_key: str,
-        capif_host: str,
-        capif_https_port: int,
+            self,
+            folder_path_for_certificates_and_api_key: str,
+            capif_host: str,
+            capif_https_port: int,
     ):
         self.capif_host = capif_host
         self.capif_https_port = capif_https_port
         self.folder_to_store_certificates_and_api_key = os.path.join(
             folder_path_for_certificates_and_api_key.strip(), ""
         )
         self.capif_api_details = self.__load_netapp_api_details()
         self.signed_key_crt_path = (
                 self.folder_to_store_certificates_and_api_key
-                + self.capif_api_details["csr_common_name"]+ ".crt"
+                + self.capif_api_details["csr_common_name"] + ".crt"
         )
         self.private_key_path = self.folder_to_store_certificates_and_api_key + "private.key"
         self.ca_root_path = self.folder_to_store_certificates_and_api_key + "ca.crt"
 
     def get_api_invoker_id(self):
         return self.capif_api_details["api_invoker_id"]
 
@@ -1445,53 +1461,52 @@
             return json.load(openfile)
 
     def _add_trailing_slash_to_url_if_missing(self, url):
         if url[len(url) - 1] != "/":
             url = url + "/"
         return url
 
-    def get_access_token(self,api_name,api_id,aef_id):
+    def get_access_token(self, api_name, api_id, aef_id):
         """
         :param api_name: The api id name is returned by discover services
          :param api_id: The api id that is returned by discover services
         :param aef_id: The relevant aef_id that is returned by discover services
          :return: The access token (jwt)
         """
         if not self.__aef_id_already_registered(aef_id):
-            self.__register_security_service(api_id,aef_id)
+            self.__register_security_service(api_id, aef_id)
             self.__save_aef_id_to_already_registered_cached_list(aef_id)
 
-        token_dic = self.__get_security_token(api_name,aef_id)
+        token_dic = self.__get_security_token(api_name, aef_id)
         return token_dic["access_token"]
 
-    def __aef_id_already_registered(self,aef_id):
-       return "registered_aef_ids" in self.capif_api_details and \
+    def __aef_id_already_registered(self, aef_id):
+        return "registered_aef_ids" in self.capif_api_details and \
             aef_id in self.capif_api_details["registered_aef_ids"]
 
-    def __save_aef_id_to_already_registered_cached_list(self,aef_id):
+    def __save_aef_id_to_already_registered_cached_list(self, aef_id):
         if "registered_aef_ids" not in self.capif_api_details:
-            self.capif_api_details["registered_aef_ids"] =[]
+            self.capif_api_details["registered_aef_ids"] = []
 
         self.capif_api_details["registered_aef_ids"].append(aef_id)
         with open(
                 self.folder_to_store_certificates_and_api_key + "capif_api_details.json", "w"
         ) as outfile:
-            json.dump(self.capif_api_details,outfile)
+            json.dump(self.capif_api_details, outfile)
 
-    def __register_security_service(self,  api_id, aef_id):
+    def __register_security_service(self, api_id, aef_id):
         """
 
         :param api_id: The api id that is returned by discover services
         :param aef_id: The aef_id that is returned by discover services
         :return: None
         """
         url = "https://{}/capif-security/v1/trustedInvokers/{}".format(self.capif_host,
                                                                        self.capif_api_details["api_invoker_id"])
 
-
         payload = {
             "securityInfo": [
                 {
                     "prefSecurityMethods": ["Oauth"]
                 }
             ],
             "notificationDestination": "https://mynotificationdest.com",
@@ -1511,28 +1526,29 @@
                                 json=payload,
                                 cert=(self.signed_key_crt_path, self.private_key_path),
                                 verify=self.ca_root_path
                                 )
         response.raise_for_status()
         response_payload = response.json()
 
-    def __get_security_token(self,api_name,aef_id ):
+    def __get_security_token(self, api_name, aef_id):
         """
         :param api_name: The api id name is returned by discover services
         :param aef_id: The relevant aef_id that is returned by discover services
         :return: The access token (jwt)
         """
 
-        url = "https://{}/capif-security/v1/securities/{}/token".format(self.capif_host,self.capif_api_details["api_invoker_id"] )
+        url = "https://{}/capif-security/v1/securities/{}/token".format(self.capif_host,
+                                                                        self.capif_api_details["api_invoker_id"])
 
-        payload= {
+        payload = {
             "grant_type": "client_credentials",
             "client_id": self.capif_api_details["api_invoker_id"],
             "client_secret": "string",
-            "scope": "3gpp#"+aef_id+":"+api_name
+            "scope": "3gpp#" + aef_id + ":" + api_name
         }
         headers = {
             'Content-Type': 'application/x-www-form-urlencoded',
         }
 
         response = requests.post(url,
                                  headers=headers,
@@ -1548,29 +1564,28 @@
 
         url = "https://{}/{}{}".format(
             self.capif_host,
             self.capif_api_details["discover_services_url"],
             self.capif_api_details["api_invoker_id"],
         )
 
-
         response = requests.request(
             "GET",
             url,
             headers={"Content-Type": "application/json"},
             data={},
             files={},
             cert=(self.signed_key_crt_path, self.private_key_path),
             verify=self.ca_root_path
         )
         response.raise_for_status()
         response_payload = json.loads(response.text)
         return response_payload
 
-    def retrieve_api_description_by_name(self,api_name):
+    def retrieve_api_description_by_name(self, api_name):
         capif_apifs = self.discover_service_apis()
         endpoints = list(
             filter(lambda api: api["apiName"] == api_name, capif_apifs["serviceAPIDescriptions"])
         )
         if len(endpoints) == 0:
             raise ServiceDiscoverer.ServiceDiscovererException(
                 "Could not find available endpoints for api_name: "
@@ -1621,141 +1636,146 @@
     """
     Contains helper functions to apply Time-Sensitive Networking (TSN) standards to time-sensitive NetApps.
     Allows the configuration of certain parameters in the underlying TSN infrastructure of the testbed.
     These parameters indicate the expected QoS of the communication. Read more at https://github.com/EVOLVED-5G/TSN_AF
     """
 
     def __init__(
-        self,
-        folder_path_for_certificates_and_capif_api_key:str,
-        capif_host: str,
-        capif_https_port: int,
-        https: bool,
-        tsn_host: str,
-        tsn_port: int,
+            self,
+            folder_path_for_certificates_and_capif_api_key: str,
+            capif_host: str,
+            capif_https_port: int,
+            https: bool,
+            tsn_host: str,
+            tsn_port: int,
     ) -> None:
 
         self.folder_path_for_certificates_and_capif_api_key = os.path.join(
             folder_path_for_certificates_and_capif_api_key.strip(), ""
         )
         self.api_name = "/tsn/api/"
-        self.service_discoverer = ServiceDiscoverer(self.folder_path_for_certificates_and_capif_api_key,capif_host, capif_https_port)
+        self.service_discoverer = ServiceDiscoverer(self.folder_path_for_certificates_and_capif_api_key, capif_host,
+                                                    capif_https_port)
+        api_resource_description = self.service_discoverer.retrieve_api_description_by_name(self.api_name)
+        self.access_token = self.service_discoverer.get_access_token(self.api_name, api_resource_description["apiId"],
+                                                                     api_resource_description["aefProfiles"][0][
+                                                                         "aefId"])
+        self.headers_auth = {
+            "Accept": "application/json",
+            'Authorization': 'Bearer ' + self.access_token
+        }
         self.api_invoker_id = self.service_discoverer.get_api_invoker_id()
         self.url_prefix = "{protocol}://{host}:{port}".format(
-                                  protocol="https" if https else "http",
-                                  host=tsn_host,
-                                  port=tsn_port
-                            )
-
+            protocol="https" if https else "http",
+            host=tsn_host,
+            port=tsn_port
+        )
 
     class TSNNetappIdentifier:
         def __init__(self, netapp_name: str):
             self.netapp_name = netapp_name
             self.__identifier = self.__generate_random_identifier()
 
         def __generate_random_identifier(self):
-
-             return "{netapp_name}_{random_uuid}".format(
-                 netapp_name=self.netapp_name, random_uuid=uuid4().hex
-             )
+            return "{netapp_name}_{random_uuid}".format(
+                netapp_name=self.netapp_name, random_uuid=uuid4().hex
+            )
 
         @property
         def value(self):
             return self.__identifier
 
-
-
     class TSNProfile:
         def __init__(self, tsn_manager, profile_name):
             self.tsn_manager = tsn_manager
             self.name = profile_name
             self.configuration = self.get_configuration_for_tsn_profile()
 
         class TSNProfileConfiguration:
             def __init__(self, parameters_dict):
                 for (
-                    profile_parameter_name,
-                    profile_parameter_value,
+                        profile_parameter_name,
+                        profile_parameter_value,
                 ) in parameters_dict.items():
                     setattr(self, profile_parameter_name, profile_parameter_value)
 
             def get_profile_configuration_parameters(self):
                 return vars(self)
 
         def get_configuration_for_tsn_profile(
-            self,
+                self,
         ) -> TSNProfileConfiguration:
             """
             Returns the configuration parameters of the selected time-sensitive networking (TSN) profile.
 
             :return: the default TSN profile configuration
             """
 
-            url =self.tsn_manager.url_prefix +\
-                self.tsn_manager.service_discoverer.\
-                    retrieve_specific_resource_name(self.tsn_manager.api_name, "TSN_DETAIL_PROFILE").\
-                    format(profileName=self.name)
+            url = self.tsn_manager.url_prefix + \
+                  self.tsn_manager.service_discoverer. \
+                      retrieve_specific_resource_name(self.tsn_manager.api_name, "TSN_DETAIL_PROFILE"). \
+                      format(profileName=self.name)
 
-            response = requests.get(url=url, headers={"Accept": "application/json"})
+            response = requests.get(url=url, headers=self.tsn_manager.headers_auth)
             response.raise_for_status()
             parameters_dict = json.loads(response.text)[self.name]
             return self.TSNProfileConfiguration(parameters_dict)
 
     def get_tsn_profiles(self) -> [TSNProfile]:
         """
         Returns the names of supported time-sensitive networking (TSN) profiles.
 
         :return: a list of TSN profiles. Each TSN profile is a TSNProfile class.
 
         """
-        url =self.url_prefix+  self.service_discoverer.\
-            retrieve_specific_resource_name(self.api_name, "TSN_LIST_PROFILES").\
+        url = self.url_prefix + self.service_discoverer. \
+            retrieve_specific_resource_name(self.api_name, "TSN_LIST_PROFILES"). \
             format(scsAsId=self.api_invoker_id)
 
-        response = requests.get(url=url, headers={"Accept": "application/json"})
+        response = requests.get(url=url, headers=self.headers_auth)
         response.raise_for_status()
         response_dict = json.loads(response.text)
         return [
             self.TSNProfile(tsn_manager=self, profile_name=name)
             for name in response_dict["profiles"]
         ]
 
     def apply_tsn_profile_to_netapp(
-        self,
-        tsn_netapp_identifier: TSNNetappIdentifier,
-        profile: TSNProfile,
+            self,
+            tsn_netapp_identifier: TSNNetappIdentifier,
+            profile: TSNProfile,
     ) -> str:
         """
         Applies the time-sensitive networking (TSN) profile to the NetApp specified by <tsn_netapp_identifier>
 
         :param tsn_netapp_identifier: the TSN identifier class of the NetApp
         :param profile: the TSN profile whose configuration will be applied to the NetApp
         :return: token which can be used to clear the configuration from the NetApp
         """
 
         data = {
             "identifier": tsn_netapp_identifier.value,
             "profile": profile.name,
             "overrides": {},
         }
-        url = self.url_prefix+ self.service_discoverer.retrieve_specific_resource_name(self.api_name, "TSN_APPLY_CONFIGURATION")
-
+        url = self.url_prefix + self.service_discoverer.retrieve_specific_resource_name(self.api_name,
+                                                                                        "TSN_APPLY_CONFIGURATION")
 
         response = requests.post(
-                url=url, json=data, headers={"Content-type": "application/json"}
+            url=url, json=data, headers=self.headers_auth
         )
         response.raise_for_status()
         response = json.loads(response.text)
         return response["token"]
 
     def apply_profile_with_overriden_parameters_to_netapp(
-        self,
-        tsn_netapp_identifier: TSNNetappIdentifier,
-        base_profile: TSNProfile,
-        modified_params: dict,
+            self,
+            tsn_netapp_identifier: TSNNetappIdentifier,
+            base_profile: TSNProfile,
+            modified_params: dict,
     ) -> str:
         """
         Overrides the default parameters of the time-sensitive networking (TSN) profile, and applies it to the NetApp
         specified by <tsn_netapp_identifier>.
 
 
         :param tsn_netapp_identifier: the TSN identifier class of the NetApp
@@ -1765,57 +1785,234 @@
         """
         if not modified_params:
             return self.apply_tsn_profile_to_netapp(
                 tsn_netapp_identifier=tsn_netapp_identifier,
                 profile=base_profile,
             )
 
-
-        profile_base_params = (
-            base_profile.get_configuration_for_tsn_profile().get_profile_configuration_parameters()
-        )
-        for param_to_override, new_param_value in modified_params.items():
-            try:
-                _ = profile_base_params[param_to_override]
-            except KeyError:
-                warnings.warn(
-                    f'parameter value of "{param_to_override}" has no effect since it is not a configuration parameter '
-                    f'of the base profile "{base_profile.name}".\nOverridable parameters are '
-                    f'the following [{",".join(profile_base_params.keys())}]'
-                )
-
         data = {
             "identifier": tsn_netapp_identifier.value,
             "profile": base_profile.name,
             "overrides": modified_params,
         }
-        url = self.url_prefix+ self.service_discoverer.retrieve_specific_resource_name(self.api_name, "TSN_APPLY_CONFIGURATION")
+        url = self.url_prefix + self.service_discoverer.retrieve_specific_resource_name(self.api_name,
+                                                                                        "TSN_APPLY_CONFIGURATION")
 
         response = requests.post(
-            url=url, json=data, headers={"Content-type": "application/json"}
+            url=url,
+            json=data,
+            headers=self.headers_auth
         )
         response.raise_for_status()
         response = json.loads(response.text)
         return response["token"]
 
     def clear_profile_for_tsn_netapp_identifier(
-        self, tsn_netapp_identifier: TSNNetappIdentifier, clearance_token: str
+            self, tsn_netapp_identifier: TSNNetappIdentifier, clearance_token: str
     ) -> None:
         """
         Disables a previously applied configuration for the selected NetApp
 
 
         :param tsn_netapp_identifier: the TSN identifier class of the NetApp
         :param clearance_token: used to clear the applied TSN configuration from the NetApp
         """
 
-        url = self.url_prefix+ self.service_discoverer.retrieve_specific_resource_name(self.api_name, "TSN_CLEAR_CONFIGURATION")
+        url = self.url_prefix + self.service_discoverer.retrieve_specific_resource_name(self.api_name,
+                                                                                        "TSN_CLEAR_CONFIGURATION")
 
         data = {
             "identifier": tsn_netapp_identifier.value,
             "token": clearance_token,
         }
         response = requests.post(
-            url=url, json=data, headers={"Content-type": "application/json"}
+            url=url, json=data, headers=self.headers_auth
         )
         response.raise_for_status()
         assert "success" in json.loads(response.text)["message"]
+
+
+class CAPIFLogCommon(ABC):
+    def __init__(self,  certificates_folder,
+                 capif_host,
+                 capif_https_port):
+
+        self.certificates_folder = os.path.join(certificates_folder.strip(), "")
+        self.capif_https_url = ""
+        if len(capif_https_port) == 0 or int(capif_https_port) == 443:
+            self.capif_https_url = "https://" + capif_host.strip() + "/"
+        else:
+            self.capif_https_url = "https://" + capif_host.strip() + ":" + capif_https_port.strip() + "/"
+
+        with open(
+                self.certificates_folder + "capif_provider_details.json", "r"
+        ) as openfile:
+            self.capif_provider_details = json.load(openfile)
+            self.aef_id = self.capif_provider_details["AEF_api_prov_func_id"]
+
+    def get_capif_service_description(self, capif_service_api_description_json_full_path):
+        """
+        Use this method to read the api_id of  your service from the relevant file or other relevant information
+
+        :param capif_service_api_description_json_full_path:
+        This file  is generated when you register your Provider to CAPIF. It is stored inside your certificate folder.
+        :return: The service description json that is stored in CAPIF
+        """
+        with open(
+                capif_service_api_description_json_full_path, "r"
+        ) as openfile:
+            return json.load(openfile)
+
+class CAPIFLogger(CAPIFLogCommon):
+
+    def __init__(self,
+                 certificates_folder,
+                 capif_host,
+                 capif_https_port):
+
+        """
+          :param certificates_folder: The certificated folder you used during registration of the Provider to CAPIF
+          :param capif_host: The CAPIF host name
+          :param capif_https_port: The CAPIF https port
+        """
+        super().__init__(certificates_folder,capif_host,capif_https_port)
+        self.capif_logger_url = self.capif_https_url + "api-invocation-logs/v1/" + self.aef_id + "/logs"
+
+    @dataclass
+    class LogEntry:
+        """
+           A class representing a LogEntry that will be saved to CAPIF Invocation logs.
+
+      Attributes:
+            apiId (str): The ID of the API invoked.
+            apiVersion (str): The version of the API that was invoked.
+            apiName (str): The name of the API.
+            resourceName (str): The name of the resource being invoked
+            uri (str): Full URI  of the request.
+            protocol (str): The protocol used for the request (ex. HTTP_1_1)
+            invocationLatency (int): The time taken to process the request, in milliseconds.
+            invocationTime (datetime): Date on which the request was invoked.
+            operation (str): The HTTP operation being performed (Ex. GET,POST,PUT,DELETE)
+            result (int): The HTTP status code of the results (ex. 200)
+            inputParameters (dict): The input parameters for the request.
+            outputParameters (dict): The output / response parameters
+        """
+        apiId: str
+        apiVersion: str
+        apiName: str
+        resourceName: str
+        uri: str
+        protocol: str
+        invocationLatency: int
+        invocationTime: datetime
+        operation: str
+        result: int
+        inputParameters: dict
+        outputParameters: dict
+
+
+
+
+
+    def save_log(self, api_invoker_id, log_entries: List[LogEntry]):
+
+        payload = {
+            "aefId": self.aef_id,
+            "apiInvokerId": api_invoker_id,
+            "logs": list(map(lambda logentry: logentry.__dict__, log_entries)),
+            "supportedFeatures": "fffffff"
+        }
+
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", self.capif_logger_url,
+                                    headers=headers,
+                                    data=json.dumps(payload),
+                                    cert=(
+                                        self.certificates_folder + "dummy_aef.crt",
+                                        self.certificates_folder + "AEF_private_key.key",
+                                    ),
+                                    verify=self.certificates_folder + 'ca.crt')
+        response.raise_for_status()
+        response_payload = json.loads(response.text)
+
+        return response_payload
+
+
+
+
+class CAPIFAuditor(CAPIFLogCommon):
+
+    def __init__(self,
+                 certificates_folder,
+                 capif_host,
+                 capif_https_port):
+        """
+        :param certificates_folder: The certificated folder you used during registration of the Provider to CAPIF
+        :param capif_host: The CAPIF host name
+        :param capif_https_port: The CAPIF https port
+        """
+        super().__init__(certificates_folder,capif_host,capif_https_port)
+        self.capif_query_log_url = self.capif_https_url + "logs/v1/apiInvocationLogs"
+
+    def query_log(self, api_invoker_id=None, time_start=None, time_end=None, api_id=None,
+              api_name=None, api_version=None, result=None, resource_name=None, protocol=None,
+              operation=None):
+
+        """
+        :param api_invoker_id:
+        :param time_start:    # e.g. 2022-10-24T00:00:00.000Z
+        :param time_end:  # e.g. 2022-10-25T00:00:00.000Z
+        :param api_id:  # e.g. f7ba97e8f08a7f53365ba81be60a0c
+        :param api_name:   # e.g. dummy-aef
+        :param api_version:   # e.g. v1
+        :param result:   # e.g. 201
+        :param resource_name:   # e.g. MONITORING_SUBSCRIPTION_SINGLE
+        :param protocol:  # e.g. HTTP_1_1 or HTTP_2
+        :param operation:    # e.g. POST
+        :return: The Log entries found in the CAPIF database
+        """
+
+        params = dict()
+        params.update({'aef-id':self.aef_id})
+
+        if api_invoker_id is not None:
+            params.update({'api-invoker-id': api_invoker_id})
+
+        if time_start is not None:
+            params.update({'time-range-start': time_start})
+
+        if time_end is not None:
+            params.update({'time-range-end': time_end})
+
+        if api_id is not None:
+            params.update({'api-id': api_id})
+
+        if api_name is not None:
+            params.update({'api-name': api_name})
+
+        if api_version is not None:
+            params.update({'api-version': api_version})
+
+        if result is not None:
+            params.update({'result': result})
+
+        if resource_name is not None:
+            params.update({'resource-name': resource_name})
+
+        if protocol is not None:
+            params.update({'protocol': protocol})
+
+        if operation is not None:
+            params.update({'operation': operation})
+
+        response = requests.request("GET", self.capif_query_log_url, params=params,
+                                    cert=(
+                                        self.certificates_folder + "dummy_amf.crt",
+                                        self.certificates_folder + "AMF_private_key.key",
+                                    ),
+                                    verify=self.certificates_folder + 'ca.crt')
+        response.raise_for_status()
+        response_payload = json.loads(response.text)
+        return response_payload
```

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/__init__.py` & `evolved5g-1.0.3/evolved5g/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/__init__.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/cells_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/cells_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/default_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/g_n_bs_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/g_n_bs_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/location_frontend_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/location_frontend_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/login_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/login_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/monitoring_event_api_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/monitoring_event_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/paths_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/paths_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/qo_s_information_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/qo_s_information_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/session_with_qo_s_api_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/session_with_qo_s_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/u_es_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/u_es_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/ui_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/ui_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/users_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api/utils_api.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/api_client.py` & `evolved5g-1.0.3/evolved5g/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/configuration.py` & `evolved5g-1.0.3/evolved5g/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/__init__.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/accumulated_usage.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/accumulated_usage.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_u_es_speed.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_u_es_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_ue_create_speed.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_ue_create_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_ue_speed.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_ue_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_ue_update_speed.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_ue_update_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/cell.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/cell.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/cell_create.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/cell_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/cell_update.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/cell_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/gnb.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/gnb.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/gnb_create.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/gnb_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/gnb_update.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/gnb_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/http_validation_error.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/location_info.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/location_info.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_report.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_report_received.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_report_received.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_subscription.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_event_subscription_create.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_event_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_notification.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_notification.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/monitoring_type.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/monitoring_type.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/msg.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/msg.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/path.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/path.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/path_create.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/path_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/path_update.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/path_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/paths.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/paths.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/point.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/point.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/qo_s_monitoring_report.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/qo_s_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/qos_monitoring_information.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/qos_monitoring_information.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/reporting_frequency.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/reporting_frequency.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/snssai.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/snssai.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/speed.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/token.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/u_es.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/u_es.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/ue.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/ue.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/ue_create.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/ue_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/ue_update.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/ue_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/usage_threshold.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/usage_threshold.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/user.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/user_create.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/user_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/user_plane_event.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/user_plane_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/user_plane_event_report.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/user_plane_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/user_plane_notification_data.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/user_plane_notification_data.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/user_update.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/user_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/models/validation_error.py` & `evolved5g-1.0.3/evolved5g/swagger_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g/swagger_client/rest.py` & `evolved5g-1.0.3/evolved5g/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/evolved5g.egg-info/PKG-INFO` & `evolved5g-1.0.3/evolved5g.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.2
+Version: 1.0.3
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,17 +54,26 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.3 (2023-04-25)
+        -------------------
+        * New SDK Class CAPIFLogger, that allows a provider (like NEF Emulator) to save Log information, for example capture incoming requests and responses
+        * New SDK Class CAPIFAuditor, that allows a provider (like NEF Emulator) to query the Log, for example filter all the Log information for a given Network APP
+        * Added examples of usage for CAPIFLogger and CAPIFAuditor class in examples/nef_logger_and_audit_example.py
+        * At CAPIFProviderConnector class when using the publish_services() method, a copy of the published to CAPIF api is saved to the local certificates folder. This is useful if you want to retrieve the relevant CAPIF ids for this service like aef_id or api_id.
+        
+        -------------------
         1.0.2 (2023-03-09)
         -------------------
-        * Bug fix on minimum python version. Change it from 3.6 to 3.7. Installing the SDK in older ubuntu distribution raises an error at runtime requiring higher python version coming from Cookiecutter. 
+        * Update TSN Manager class, apply security improvements.  Now each request to the TSN API uses JWT Bearer authentication. Access tokens are retrieved via CAPIF.
+        * Bug fix on minimum python version. Change it from 3.6 to 3.7. Installing the SDK in older ubuntu distribution raises an error at runtime requiring higher python version coming from Cookiecutter.
         
         -------------------
         1.0.1 (2023-03-03)
         -------------------
         * Bug fix on CAPIFProviderConnector: If you run it twice (for example for testing purposes) the .pem certificate should be overriden.
         
         -------------------
```

### Comparing `evolved5g-1.0.2/evolved5g.egg-info/SOURCES.txt` & `evolved5g-1.0.3/evolved5g.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.2/setup.py` & `evolved5g-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords="evolved5g",
     name="evolved5g",
     packages=find_packages(include=["evolved5g", "evolved5g.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/EVOLVED-5G/SDK-CLI",
-    version="1.0.2",
+    version="1.0.3",
     zip_safe=False,
 )
```

