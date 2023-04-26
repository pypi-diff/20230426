# Comparing `tmp/nua_orchestrator-0.5.13.tar.gz` & `tmp/nua_orchestrator-0.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_orchestrator-0.5.13.tar", max compression
+gzip compressed data, was "nua_orchestrator-0.5.14.tar", max compression
```

## Comparing `nua_orchestrator-0.5.13.tar` & `nua_orchestrator-0.5.14.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     3789 2023-04-24 21:25:56.870296 nua_orchestrator-0.5.13/README.md
--rw-r--r--   0        0        0     2721 2023-04-24 21:28:00.790633 nua_orchestrator-0.5.13/pyproject.toml
--rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.13/src/nua/orchestrator/__init__.py
--rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.13/src/nua/orchestrator/__main__.py
--rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.13/src/nua/orchestrator/admin_local.py
--rw-r--r--   0        0        0    42885 2023-04-24 21:25:56.872804 nua_orchestrator-0.5.13/src/nua/orchestrator/app_deployment.py
--rw-r--r--   0        0        0    12313 2023-04-11 14:23:48.025954 nua_orchestrator-0.5.13/src/nua/orchestrator/app_instance.py
--rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.13/src/nua/orchestrator/app_management.py
--rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/__init__.py
--rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/db_utils.py
--rw-r--r--   0        0        0     3205 2023-04-04 11:21:10.875934 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/engine.py
--rw-r--r--   0        0        0     6378 2023-04-16 15:02:45.960265 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/evaluators.py
--rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/__init__.py
--rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_engine.py
--rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_functions.py
--rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_report.py
--rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.13/src/nua/orchestrator/bootstrap/__init__.py
--rw-r--r--   0        0        0     7132 2023-04-24 21:25:56.873313 nua_orchestrator-0.5.13/src/nua/orchestrator/bootstrap/bootstrap.py
--rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/__init__.py
--rw-r--r--   0        0        0     2546 2023-04-21 16:49:16.834079 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/certbot.py
--rw-r--r--   0        0        0     4666 2023-04-24 21:25:56.873579 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/commands.py
--rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/__init__.py
--rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/cli.ini
--rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
--rw-r--r--   0        0        0     2507 2023-04-24 21:25:56.873772 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/installer.py
--rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/api.py
--rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/backup.py
--rw-r--r--   0        0        0     1887 2023-04-14 13:33:56.045871 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/deploy_remove.py
--rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/restore.py
--rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/start_stop.py
--rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/status.py
--rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/configuration.py
--rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/debug.py
--rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/init.py
--rw-r--r--   0        0        0     6483 2023-04-16 08:46:30.714460 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/main.py
--rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.13/src/nua/orchestrator/config.py
--rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.13/src/nua/orchestrator/constants.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.13/src/nua/orchestrator/db/__init__.py
--rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.13/src/nua/orchestrator/db/create.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/__init__.py
--rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/auth.py
--rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/base.py
--rw-r--r--   0        0        0     2073 2023-04-18 09:50:17.612727 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/deployconfig.py
--rw-r--r--   0        0        0      856 2023-04-18 09:50:17.612881 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/host.py
--rw-r--r--   0        0        0     1033 2023-04-18 09:50:17.613199 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/image.py
--rw-r--r--   0        0        0     4153 2023-04-18 09:50:17.613726 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/instance.py
--rw-r--r--   0        0        0     1602 2023-04-18 09:50:17.613874 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/setting.py
--rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/user_count.py
--rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.13/src/nua/orchestrator/db/session.py
--rw-r--r--   0        0        0    16381 2023-04-12 10:07:58.740008 nua_orchestrator-0.5.13/src/nua/orchestrator/db/store.py
--rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/__init__.py
--rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/migrations.py
--rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/tools.py
--rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/__init__.py
--rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.json
--rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.py
--rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mongo.json
--rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mongo.py
--rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.json
--rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.py
--rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/redis-cache.json
--rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/redis-cache.py
--rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/__init__.py
--rw-r--r--   0        0        0     7074 2023-04-24 21:25:56.874060 nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/mariadb_utils.py
--rw-r--r--   0        0        0     8130 2023-04-24 21:25:56.874228 nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/postgres_utils.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.13/src/nua/orchestrator/default_conf/__init__.py
--rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.13/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
--rw-r--r--   0        0        0    12007 2023-04-24 21:25:56.874494 nua_orchestrator-0.5.13/src/nua/orchestrator/deploy_utils.py
--rw-r--r--   0        0        0    18027 2023-04-24 21:25:56.874767 nua_orchestrator-0.5.13/src/nua/orchestrator/docker_utils.py
--rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.13/src/nua/orchestrator/domain_split.py
--rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.13/src/nua/orchestrator/healthcheck.py
--rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.13/src/nua/orchestrator/higher_package.py
--rw-r--r--   0        0        0     1417 2023-04-08 16:30:35.183610 nua_orchestrator-0.5.13/src/nua/orchestrator/internal_secrets.py
--rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.13/src/nua/orchestrator/net_utils/__init__.py
--rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.13/src/nua/orchestrator/net_utils/external_ip.py
--rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.13/src/nua/orchestrator/net_utils/ports.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/__init__.py
--rw-r--r--   0        0        0     1622 2023-04-24 21:25:56.874974 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/cmd.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/css/__init__.py
--rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/css/style.css
--rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/index.html
--rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/installer.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/__init__.py
--rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/default_site
--rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_located.j2
--rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_not_located.j2
--rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_located.j2
--rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located.j2
--rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
--rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/nginx.conf
--rw-r--r--   0        0        0     4895 2023-04-24 21:25:56.875166 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/utils.py
--rw-r--r--   0        0        0     4620 2023-04-24 21:08:40.326542 nua_orchestrator-0.5.13/src/nua/orchestrator/nua_db_setup.py
--rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.13/src/nua/orchestrator/nua_env.py
--rw-r--r--   0        0        0     1078 2023-04-05 05:50:21.473685 nua_orchestrator-0.5.13/src/nua/orchestrator/persistent.py
--rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.13/src/nua/orchestrator/port_normalization.py
--rw-r--r--   0        0        0     3351 2023-04-24 21:25:56.875342 nua_orchestrator-0.5.13/src/nua/orchestrator/register_plugins.py
--rw-r--r--   0        0        0     2848 2023-01-08 20:45:01.446656 nua_orchestrator-0.5.13/src/nua/orchestrator/registry.py
--rw-r--r--   0        0        0    15807 2023-04-24 21:25:56.875604 nua_orchestrator-0.5.13/src/nua/orchestrator/resource.py
--rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.13/src/nua/orchestrator/resource_deps.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/__init__.py
--rw-r--r--   0        0        0      307 2023-02-06 17:21:30.505291 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/deactivate_all_instances.py
--rw-r--r--   0        0        0      263 2023-01-19 17:57:22.674122 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/docker_list_all.py
--rw-r--r--   0        0        0     1211 2023-04-17 20:53:06.739901 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/docker_remove_all.py
--rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/list_instances.py
--rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/mariadb_restore.py
--rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_instances.py
--rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_mounted_volumes.py
--rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_used_ports.py
--rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/set_pg_pwd.py
--rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.13/src/nua/orchestrator/search_cmd.py
--rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.13/src/nua/orchestrator/services/__init__.py
--rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.13/src/nua/orchestrator/services/mariadb.py
--rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.13/src/nua/orchestrator/services/postgres.py
--rw-r--r--   0        0        0     1127 2023-01-30 14:35:45.686645 nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_base.py
--rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_loader.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.13/src/nua/orchestrator/util/__init__.py
--rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.13/src/nua/orchestrator/util/deep_access_dict.py
--rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.13/src/nua/orchestrator/util/deep_update.py
--rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.13/src/nua/orchestrator/utils.py
--rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.13/src/nua/orchestrator/version.py
--rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.13/src/nua/orchestrator/volume.py
--rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.13/PKG-INFO
+-rw-r--r--   0        0        0     3789 2023-04-24 21:25:56.870296 nua_orchestrator-0.5.14/README.md
+-rw-r--r--   0        0        0     2721 2023-04-26 06:46:56.050490 nua_orchestrator-0.5.14/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.14/src/nua/orchestrator/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.14/src/nua/orchestrator/__main__.py
+-rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.14/src/nua/orchestrator/admin_local.py
+-rw-r--r--   0        0        0    50949 2023-04-26 06:41:08.609843 nua_orchestrator-0.5.14/src/nua/orchestrator/app_deployment.py
+-rw-r--r--   0        0        0    12482 2023-04-26 06:41:08.610306 nua_orchestrator-0.5.14/src/nua/orchestrator/app_instance.py
+-rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.14/src/nua/orchestrator/app_management.py
+-rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/db_utils.py
+-rw-r--r--   0        0        0     3205 2023-04-04 11:21:10.875934 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/engine.py
+-rw-r--r--   0        0        0     6378 2023-04-16 15:02:45.960265 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/evaluators.py
+-rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/__init__.py
+-rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_engine.py
+-rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_functions.py
+-rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_report.py
+-rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.14/src/nua/orchestrator/bootstrap/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-24 21:25:56.873313 nua_orchestrator-0.5.14/src/nua/orchestrator/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/__init__.py
+-rw-r--r--   0        0        0     2546 2023-04-21 16:49:16.834079 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/certbot.py
+-rw-r--r--   0        0        0     4666 2023-04-24 21:25:56.873579 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/commands.py
+-rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/__init__.py
+-rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/cli.ini
+-rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
+-rw-r--r--   0        0        0     2507 2023-04-24 21:25:56.873772 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/installer.py
+-rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/api.py
+-rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/backup.py
+-rw-r--r--   0        0        0     1898 2023-04-26 06:41:08.610568 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/deploy_remove.py
+-rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/restore.py
+-rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/start_stop.py
+-rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/status.py
+-rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/configuration.py
+-rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/debug.py
+-rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/init.py
+-rw-r--r--   0        0        0     6483 2023-04-16 08:46:30.714460 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/main.py
+-rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.14/src/nua/orchestrator/config.py
+-rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.14/src/nua/orchestrator/constants.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.14/src/nua/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.14/src/nua/orchestrator/db/create.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/__init__.py
+-rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/auth.py
+-rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/base.py
+-rw-r--r--   0        0        0     2073 2023-04-18 09:50:17.612727 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/deployconfig.py
+-rw-r--r--   0        0        0      856 2023-04-18 09:50:17.612881 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/host.py
+-rw-r--r--   0        0        0     1033 2023-04-18 09:50:17.613199 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/image.py
+-rw-r--r--   0        0        0     4253 2023-04-26 06:41:08.610731 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/instance.py
+-rw-r--r--   0        0        0     1602 2023-04-18 09:50:17.613874 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/setting.py
+-rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/user_count.py
+-rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.14/src/nua/orchestrator/db/session.py
+-rw-r--r--   0        0        0    16464 2023-04-26 06:41:08.610982 nua_orchestrator-0.5.14/src/nua/orchestrator/db/store.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/migrations.py
+-rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/tools.py
+-rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/__init__.py
+-rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.json
+-rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.py
+-rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mongo.json
+-rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mongo.py
+-rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.json
+-rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.py
+-rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/redis-cache.json
+-rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/redis-cache.py
+-rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/__init__.py
+-rw-r--r--   0        0        0     7074 2023-04-24 21:25:56.874060 nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/mariadb_utils.py
+-rw-r--r--   0        0        0     8130 2023-04-24 21:25:56.874228 nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/postgres_utils.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.14/src/nua/orchestrator/default_conf/__init__.py
+-rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.14/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
+-rw-r--r--   0        0        0    12004 2023-04-26 06:41:08.611177 nua_orchestrator-0.5.14/src/nua/orchestrator/deploy_utils.py
+-rw-r--r--   0        0        0    18027 2023-04-24 21:25:56.874767 nua_orchestrator-0.5.14/src/nua/orchestrator/docker_utils.py
+-rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.14/src/nua/orchestrator/domain_split.py
+-rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.14/src/nua/orchestrator/healthcheck.py
+-rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.14/src/nua/orchestrator/higher_package.py
+-rw-r--r--   0        0        0     1417 2023-04-08 16:30:35.183610 nua_orchestrator-0.5.14/src/nua/orchestrator/internal_secrets.py
+-rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.14/src/nua/orchestrator/net_utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.14/src/nua/orchestrator/net_utils/external_ip.py
+-rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.14/src/nua/orchestrator/net_utils/ports.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/__init__.py
+-rw-r--r--   0        0        0     1622 2023-04-24 21:25:56.874974 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/cmd.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/css/__init__.py
+-rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/css/style.css
+-rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/index.html
+-rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/installer.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/__init__.py
+-rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/default_site
+-rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_located.j2
+-rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_not_located.j2
+-rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_located.j2
+-rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located.j2
+-rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
+-rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/nginx.conf
+-rw-r--r--   0        0        0     4895 2023-04-24 21:25:56.875166 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/utils.py
+-rw-r--r--   0        0        0     4621 2023-04-26 06:41:08.611435 nua_orchestrator-0.5.14/src/nua/orchestrator/nua_db_setup.py
+-rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.14/src/nua/orchestrator/nua_env.py
+-rw-r--r--   0        0        0     1078 2023-04-05 05:50:21.473685 nua_orchestrator-0.5.14/src/nua/orchestrator/persistent.py
+-rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.14/src/nua/orchestrator/port_normalization.py
+-rw-r--r--   0        0        0     3351 2023-04-24 21:25:56.875342 nua_orchestrator-0.5.14/src/nua/orchestrator/register_plugins.py
+-rw-r--r--   0        0        0     2848 2023-01-08 20:45:01.446656 nua_orchestrator-0.5.14/src/nua/orchestrator/registry.py
+-rw-r--r--   0        0        0    15807 2023-04-24 21:25:56.875604 nua_orchestrator-0.5.14/src/nua/orchestrator/resource.py
+-rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.14/src/nua/orchestrator/resource_deps.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/__init__.py
+-rw-r--r--   0        0        0      307 2023-02-06 17:21:30.505291 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/deactivate_all_instances.py
+-rw-r--r--   0        0        0      263 2023-01-19 17:57:22.674122 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/docker_list_all.py
+-rw-r--r--   0        0        0     1211 2023-04-17 20:53:06.739901 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/docker_remove_all.py
+-rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/list_instances.py
+-rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/mariadb_restore.py
+-rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_instances.py
+-rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_mounted_volumes.py
+-rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_used_ports.py
+-rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/set_pg_pwd.py
+-rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.14/src/nua/orchestrator/search_cmd.py
+-rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.14/src/nua/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.14/src/nua/orchestrator/services/mariadb.py
+-rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.14/src/nua/orchestrator/services/postgres.py
+-rw-r--r--   0        0        0     1127 2023-01-30 14:35:45.686645 nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_base.py
+-rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_loader.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.14/src/nua/orchestrator/util/__init__.py
+-rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.14/src/nua/orchestrator/util/deep_access_dict.py
+-rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.14/src/nua/orchestrator/util/deep_update.py
+-rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.14/src/nua/orchestrator/utils.py
+-rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.14/src/nua/orchestrator/version.py
+-rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.14/src/nua/orchestrator/volume.py
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.14/PKG-INFO
```

### Comparing `nua_orchestrator-0.5.13/README.md` & `nua_orchestrator-0.5.14/README.md`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/pyproject.toml` & `nua_orchestrator-0.5.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-orchestrator"
-version = "0.5.13"
+version = "0.5.14"
 description = "Nua orchestrator - local implementation"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -28,18 +28,18 @@
 nua-deactivate-all = "nua.orchestrator.scripts.deactivate_all_instances:main"
 nua-docker-list-all = "nua.orchestrator.scripts.docker_list_all:main"
 nua-docker-rm-all = "nua.orchestrator.scripts.docker_remove_all:main"
 nua_test_services = "nua.orchestrator.service:test"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.13"
-nua-agent = "=0.5.13"
-nua-build = "=0.5.13"
-nua-autobuild = "=0.5.13"
+nua-lib = "=0.5.14"
+nua-agent = "=0.5.14"
+nua-build = "=0.5.14"
+nua-autobuild = "=0.5.14"
 SQLAlchemy-serializer = "^1.4.1"
 SQLAlchemy = "^1.4.36"
 psycopg2-binary = "^2.9.3"
 setuptools = "*"
 wheel = "*"
 tomli = "^2"
 paramiko = "^2.11.0"
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/admin_local.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/admin_local.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/app_deployment.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/app_deployment.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 import time
 from collections.abc import Callable
 from copy import deepcopy
 from pathlib import Path
 from pprint import pformat
 from typing import Any
 
-from nua.lib.console import print_green, print_red
 from nua.lib.panic import (
     Abort,
     bold_debug,
     debug,
     important,
     info,
+    red_line,
     show,
-    vprint,
     warning,
 )
 from nua.lib.tool.state import verbosity
 
 from . import config
 from .app_instance import AppInstance
 from .assign.engine import instance_key_evaluator
@@ -94,14 +93,16 @@
 
     def __init__(self):
         self.loaded_config = {}
         self.apps = []
         self.apps_per_domain = []
         self.deployed_domains = []
         self.already_deployed_domains = set()
+        self.deployed_labels = []
+        self.already_deployed_labels = set()
         self.required_services = set()
         self.available_services = {}
         self.orig_mounted_volumes = []
         self.previous_config_id = 0
         self._mounted_before_removing = []  # internal use when removing app instance
         # self.future_config_id = 0
 
@@ -179,16 +180,17 @@
         config_path = Path(deploy_config).expanduser().resolve()
         with verbosity(1):
             info(f"Deploy apps from: {config_path}")
         self.loaded_config = parse_any_format(config_path)
         self.parse_deploy_apps()
         self.sort_apps_per_name_domain()
         self.deployed_domains = sorted(
-            {apps_dom["hostname"] for apps_dom in self.apps_per_domain}
+            {apps["hostname"] for apps in self.apps_per_domain}
         )
+        self.deployed_labels = sorted(app.label_id for app in self.apps)
         with verbosity(3):
             self.print_host_list()
 
     def load_deployed_configuration(self):
         previous_config = self.previous_success_deployment_record()
         if not previous_config:
             with verbosity(2):
@@ -204,46 +206,240 @@
         ]
         self.sort_apps_per_name_domain()
         self.deployed_domains = sorted(
             {apps_dom["hostname"] for apps_dom in self.apps_per_domain}
         )
 
     def merge(self, additional: AppDeployment, option: str = "add"):
-        """Merge a deployment configuration into the current one.
+        """Merge a deployment configuration into the current deployed configuration.
 
         WIP:
             - first step: 'add', strict, no conflict allowed
             - next: add and replace if needed (merge)
         """
         with verbosity(3):
-            print(f"Deployment merge option: {option}")
+            debug(f"Deployment merge option: {option}")
         if option == "add":
             return self.merge_add(additional)
         raise RuntimeError("Merge option not implemented")
 
+    def merge_sequential(self, additional: AppDeployment):
+        """Merge a deployment configuration sequentially."""
+        with verbosity(3):
+            debug("Deployment merge sequentially")
+        for app in additional.apps:
+            deploy_strategy = self.evaluate_deploy_strategy(app)
+            method = getattr(self, deploy_strategy)
+            method(app)
+
+    def evaluate_deploy_strategy(self, merged_app: AppInstance) -> str:
+        same_label_app = next(
+            (app for app in self.apps if app.label_id == merged_app.label_id), None
+        )
+        same_domain_app = next(
+            (app for app in self.apps if app.domain == merged_app.domain), None
+        )
+        if same_label_app:
+            return self._deploy_same_label_strategy(
+                merged_app,
+                same_label_app,
+                same_domain_app,
+            )
+        else:
+            if same_domain_app:
+                raise Abort(
+                    f"Domain '{merged_app.domain}' already in use "
+                    f"for another label: {same_domain_app.label}"
+                )
+            # new label on new domain
+            return "deploy_new_app"
+
+    def _deploy_same_label_strategy(
+        self,
+        merged_app: AppInstance,
+        same_label_app: AppInstance,
+        same_domain_app: AppInstance,
+    ) -> str:
+        if same_label_app.domain == merged_app.domain:
+            if same_label_app.app_id == merged_app.app_id:
+                # same app on on same domain
+                return "deploy_update_app"
+            else:
+                # another app on same domain
+                return "deploy_replace_app"
+        else:
+            if merged_app.domain in self.deployed_domains:
+                # but not our domain
+                raise Abort(
+                    f"Domain '{merged_app.domain}' already in use "
+                    f"for another label: {same_domain_app.label}"
+                )
+            else:
+                if same_label_app.app_id == merged_app.app_id:
+                    # same app on another domain
+                    return "deploy_move_domain"
+                else:
+                    # another app on another domain
+                    return "deploy_reuse_label"
+
+    def deploy_new_app(self, app: AppInstance):
+        """Deploy new label and app on new domain"""
+        important(f"Deploy '{app.label}': a new {app.app_id} on '{app.domain}'")
+        self._deploy_new_app(app, load_persistent=False)
+
+    def _deploy_new_app(
+        self,
+        app: AppInstance,
+        load_persistent: bool = False,
+    ):
+        """Deploy an app."""
+        # step 1:
+        app.set_network_name()
+        app.set_resources_names()
+        app.merge_instance_to_resources()
+        for resource in app.resources:
+            resource.configure_db()
+        app.set_volumes_names()
+        for service in app.local_services:
+            if service not in self.available_services:
+                raise Abort(f"Required service '{service}' is not available")
+        if load_persistent:
+            # if really new app, not persistent for now, but some persitent data if
+            # same reusing label
+            self.retrieve_persistent(app)
+        self.evaluate_dynamic_values(app)
+
+        # step 2: ports
+        start_ports = config.read("nua", "ports", "start") or 8100
+        end_ports = config.read("nua", "ports", "end") or 9000
+        allocated_ports = self.configured_ports()
+        ports_instances_domains = store.ports_instances_domains()
+        allocated_ports.update(ports_instances_domains)
+        allocator = port_allocator(start_ports, end_ports, allocated_ports)
+        app.allocate_auto_ports(allocator)
+        for resource in app.resources:
+            resource.allocate_auto_ports(allocator)
+
+        # step 3
+        app.parse_healthcheck()
+        for service in app.local_services:
+            handler = self.available_services[service]
+            if not handler.check_site_configuration(app):
+                raise Abort(
+                    f"Required service '{service}' not configured for "
+                    f"app {app.domain}"
+                )
+        self.store_initial_deployment_state()
+        self.already_deployed_domains = set(self.deployed_domains)
+        self.already_deployed_labels = set(self.deployed_labels)
+        self.apps.append(app)
+        self.sort_apps_per_name_domain()
+        self.deployed_domains = sorted(
+            {apps_dom["hostname"] for apps_dom in self.apps_per_domain}
+        )
+        self.deployed_labels = sorted(a.label_id for a in self.apps)
+        self.merge_nginx_configuration()
+        self.merge_start_apps([app])
+
+    def deploy_update_app(self, app: AppInstance):
+        """Deploy same app on on same domain."""
+        important(f"Deploy '{app.label}': update {app.app_id} on '{app.domain}'")
+        self._deploy_remove_label_domain(app, remove_volumes=False)
+        self.load_deployed_configuration()
+        self._deploy_new_app(app, load_persistent=True)
+
+    def deploy_replace_app(self, merged_app: AppInstance):
+        """Deploy another app on same domain."""
+        same_label_app = next(
+            (app for app in self.apps if app.label_id == merged_app.label_id), None
+        )
+        important(
+            f"Deploy '{merged_app.label}': replace {same_label_app.app_id} "
+            f"by {merged_app.app_id} on '{merged_app.domain}'"
+        )
+        self._deploy_remove_label_domain(merged_app, remove_volumes=True)
+        self.load_deployed_configuration()
+        self._deploy_new_app(merged_app, load_persistent=False)
+
+    def deploy_move_domain(self, merged_app: AppInstance):
+        """Deploy same app on another domain."""
+        same_domain_app = next(
+            (app for app in self.apps if app.domain == merged_app.domain), None
+        )
+        important(
+            f"Deploy '{merged_app.label}': move {merged_app.app_id} "
+            f"from '{same_domain_app.domain}' to '{merged_app.domain}'"
+        )
+        self._deploy_remove_label_domain(same_domain_app, remove_volumes=False)
+        self.load_deployed_configuration()
+        self._deploy_new_app(merged_app, load_persistent=True)
+
+    def deploy_reuse_label(self, merged_app: AppInstance):
+        """Deploy another app on another domain."""
+        same_label_app = next(
+            (app for app in self.apps if app.label_id == merged_app.label_id), None
+        )
+        important(
+            f"Deploy '{merged_app.label}': remove {same_label_app.app_id} and"
+            f"from '{same_label_app.domain}' and\n"
+            f"install {merged_app.app_id} to '{merged_app.domain}'"
+        )
+        # do not keep data:
+        self._deploy_remove_label_domain(same_label_app, remove_volumes=True)
+        self.load_deployed_configuration()
+        self._deploy_new_app(merged_app, load_persistent=True)
+
+    def _deploy_remove_label_domain(
+        self,
+        merged_app: AppInstance,
+        remove_volumes: bool = False,
+    ):
+        # deployed_app = next(
+        #     (a for a in self.apps if a.label_id == merged_app.label_id), None
+        # )
+        domain = merged_app.domain
+        stopping_apps = self.instances_of_domain(domain)
+        self.remove_nginx_configuration(domain)
+        self.stop_deployed_apps(domain, stopping_apps)
+        self.remove_container_and_network(domain, stopping_apps)
+        if remove_volumes:
+            self.remove_managed_volumes(stopping_apps)
+        if verbosity(3):
+            debug("remove_deployed_instance:")
+            debug(" ".join([a.domain for a in stopping_apps]))
+        self.remove_deployed_instance(domain, stopping_apps)
+
     def merge_add(self, additional: AppDeployment):
         """Merge by simple addtion of new domain to list."""
         with verbosity(3):
-            print(f"self.deployed_domains       {self.deployed_domains}")
-            print(f"additional.deployed_domains {additional.deployed_domains}")
+            debug(f"self.deployed_domains       {self.deployed_domains}")
+            debug(f"additional.deployed_domains {additional.deployed_domains}")
         conflict = known_strings(self.deployed_domains, additional.deployed_domains)
         if conflict:
             raise Abort(
                 f"Some required domains are already deployed: {', '.join(conflict)}\n"
                 "Merge with strict add do not allow domain conflicts"
             )
+        conflict = known_strings(self.deployed_labels, additional.deployed_labels)
+        if conflict:
+            raise Abort(
+                f"Some required labels are already deployed: {', '.join(conflict)}\n"
+                "Merge with strict add do not allow label conflicts (for now)"
+            )
         # Note: additional should read from DB the already allocated ports:
         additional.configure_apps()
         self.store_initial_deployment_state()
         self.already_deployed_domains = set(self.deployed_domains)
+        self.already_deployed_labels = set(self.deployed_labels)
         self.apps.extend(additional.apps)
         self.sort_apps_per_name_domain()
         self.deployed_domains = sorted(
             {apps_dom["hostname"] for apps_dom in self.apps_per_domain}
         )
+        self.deployed_labels = sorted(app.label_id for app in self.apps)
         self.merge_nginx_configuration()
         self.merge_start_apps(additional.apps)
 
     def instances_of_domain(self, domain: str) -> list[AppInstance]:
         """Select deployed instances of domain."""
         self.load_deployed_configuration()
         for apps_dom in self.apps_per_domain:
@@ -377,41 +573,41 @@
     def merge_start_apps(self, new_apps: list[AppInstance]):
         """Start new deployed apps."""
         if not self.already_deployed_domains:
             # easy, either first deployment or all apps removed, start from zero:
             return self.start_apps()
         # restarting local services:
         self.restart_local_services()
-        for site in new_apps:
-            deactivate_app(site)
-            self.start_network(site)
-            self.evaluate_container_params(site)
-            self.start_resources_containers(site)
-            self.setup_resources_db(site)
-            self.merge_volume_only_resources(site)
-            self.start_main_app_container(site)
-            site.running_status = RUNNING
-            self.store_container_instance(site)
+        for app in new_apps:
+            deactivate_app(app)
+            self.start_network(app)
+            self.evaluate_container_params(app)
+            self.start_resources_containers(app)
+            self.setup_resources_db(app)
+            self.merge_volume_only_resources(app)
+            self.start_main_app_container(app)
+            app.running_status = RUNNING
+            self.store_container_instance(app)
         chown_r_nua_nginx()
         nginx_reload()
 
     def start_apps(self):
         """Start all apps to deploy."""
         # restarting local services:
         self.restart_local_services()
-        for site in self.apps:
-            deactivate_app(site)
-            self.start_network(site)
-            self.evaluate_container_params(site)
-            self.start_resources_containers(site)
-            self.setup_resources_db(site)
-            self.merge_volume_only_resources(site)
-            self.start_main_app_container(site)
-            site.running_status = RUNNING
-            self.store_container_instance(site)
+        for app in self.apps:
+            deactivate_app(app)
+            self.start_network(app)
+            self.evaluate_container_params(app)
+            self.start_resources_containers(app)
+            self.setup_resources_db(app)
+            self.merge_volume_only_resources(app)
+            self.start_main_app_container(app)
+            app.running_status = RUNNING
+            self.store_container_instance(app)
         chown_r_nua_nginx()
         nginx_restart()
 
     def start_deployed_apps(self, domain: str, apps: list[AppInstance]):
         """Start deployed instances previously stopped."""
         with verbosity(1):
             info(f"Start instance of domain '{domain}'.")
@@ -495,63 +691,62 @@
         before = self._local_volumes_dict(self._mounted_before_removing)
         for source in before:
             remove_volume_by_source(source)
 
     def remove_deployed_instance(self, domain: str, apps: list[AppInstance]):
         """Remove data of stopped app: local managed volumes."""
         with verbosity(1):
-            info(f"Remove app instance of domain '{domain}'.")
-        for site in apps:
-            self.remove_app_instance(site)
+            info(f"Remove app instance of domain '{domain}' from DB.")
+        for app in apps:
+            self.remove_app_instance(app)
 
     def parse_deploy_apps(self):
-        """Make the list of AppInstances.
+        """Make the list of AppInstances to be deployed/merged.
 
         Check config syntax, replace missing information by defaults.
         """
         apps = []
         for site_dict in self.loaded_config["site"]:
             if not isinstance(site_dict, dict):
                 raise Abort(
                     "AppInstance configuration must be a dict",
                     explanation=f"{pformat(site_dict)}",
                 )
 
             app_instance = AppInstance(site_dict)
             app_instance.check_valid()
-            # site.set_ports_as_dict()
             apps.append(app_instance)
         self.apps = apps
 
     def sort_apps_per_name_domain(self):
         """Classify the apps per domain, filtering out miss declared apps.
 
         The apps per domain are available in self.apps_per_domain
         """
-        self._filter_duplicate_instance_names()
+        self._filter_duplicate_labels()
         self._make_apps_per_domain()
         self._filter_miss_located_apps()
         self._update_apps_list()
 
-    def _filter_duplicate_instance_names(self) -> None:
-        """Warn about duplicate instance_name and remove the duplicate.
+    def _filter_duplicate_labels(self) -> None:
+        """Warn about duplicate label and remove the duplicate.
 
         Note:
             - It's a basic feature for consistency, not a security feature
               about currently deployed instances.
         """
         filtered = []
-        known_names = set()
-        for site in self.apps:
-            name = site.instance_name_internal
-            if name in known_names:
-                warning(f"Duplicate instance name '{name}'. Skipped.")
+        known_labels = set()
+        for app in self.apps:
+            label_id = app.label_id
+            if label_id in known_labels:
+                warning(f"Duplicate label '{label_id}'. Skipped.")
                 continue
-            filtered.append(site)
-            known_names.add(name)
+            filtered.append(app)
+            known_labels.add(label_id)
         self.apps = filtered
 
     def _make_apps_per_domain(self) -> None:
         """Convert dict(hostname:[apps,..]) to list({hostname, apps}).
 
         ouput format:
         [{'hostname': 'test.example.com',
@@ -642,24 +837,24 @@
         # first: check that all Nua images are available:
         if not self.find_all_apps_images():
             raise Abort("Missing Nua images")
 
         self.install_images()
 
     def find_all_apps_images(self) -> bool:
-        for site in self.apps:
-            if not site.find_registry_path():
-                print_red(f"No image found for '{site.image}'")
+        for app in self.apps:
+            if not app.find_registry_path():
+                show(f"No image found for '{app.image}'")
                 return False
         with verbosity(1):
             seen = set()
-            for site in self.apps:
-                if site.image not in seen:
-                    seen.add(site.image)
-                    info(f"Image found: '{site.image}'")
+            for app in self.apps:
+                if app.image not in seen:
+                    seen.add(app.image)
+                    info(f"Image found: '{app.image}'")
         return True
 
     def install_images(self):
         start_container_engine()
         installed = {}
         for site in self.apps:
             if not site.find_registry_path(cached=True):
@@ -688,22 +883,22 @@
 
     def _pull_resource(self, resource: Resource) -> bool:
         if resource.type == "local":
             # will check later in the process
             return True
         if resource.is_docker_type():
             with verbosity(4):
-                vprint("pull docker resource:", resource)
+                debug("pull docker resource:", resource)
             return pull_resource_container(resource)
         return True
 
     def apps_check_local_service_available(self):
         self.required_services = {s for site in self.apps for s in site.local_services}
         with verbosity(3):
-            vprint("required services:", self.required_services)
+            debug("required services:", self.required_services)
         available_services = set(self.available_services.keys())
         for service in self.required_services:
             if service not in available_services:
                 raise Abort(f"Required service '{service}' is not available")
 
     def apps_check_host_services_configuration(self):
         for site in self.apps:
@@ -712,55 +907,55 @@
                 if not handler.check_site_configuration(site):
                     raise Abort(
                         f"Required service '{service}' not configured for "
                         f"site {site.domain}"
                     )
 
     def apps_parse_resources(self):
-        for site in self.apps:
-            site.parse_resources()
+        for app in self.apps:
+            app.parse_resources()
 
     def apps_parse_healthcheck(self):
-        for site in self.apps:
-            site.parse_healthcheck()
+        for app in self.apps:
+            app.parse_healthcheck()
         with verbosity(3):
-            info("apps_parse_healthcheck() done")
+            debug("apps_parse_healthcheck() done")
 
     def apps_set_network_name(self):
-        for site in self.apps:
-            site.set_network_name()
+        for app in self.apps:
+            app.set_network_name()
         with verbosity(3):
-            info("apps_set_network_name() done")
+            debug("apps_set_network_name() done")
 
     def apps_set_resources_names(self):
-        for site in self.apps:
-            site.set_resources_names()
+        for app in self.apps:
+            app.set_resources_names()
         with verbosity(3):
-            info("apps_set_resources_names() done")
+            debug("apps_set_resources_names() done")
 
     def apps_merge_app_instances_to_resources(self):
         """Merge configuration declared in the AppInstance config to original
         nua-config declarations."""
-        for site in self.apps:
-            site.merge_instance_to_resources()
+        for app in self.apps:
+            app.merge_instance_to_resources()
         with verbosity(3):
-            info("apps_merge_instances_to_resources() done")
+            debug("apps_merge_instances_to_resources() done")
 
     def apps_configure_requested_db(self):
-        for site in self.apps:
-            for resource in site.resources:
+        for app in self.apps:
+            for resource in app.resources:
                 resource.configure_db()
         with verbosity(3):
-            info("apps_configure_requested_db() done")
+            debug("apps_configure_requested_db() done")
 
     def apps_set_volumes_names(self):
-        for site in self.apps:
-            site.set_volumes_names()
+        for app in self.apps:
+            app.set_volumes_names()
         with verbosity(3):
-            info("apps_set_volumes_names() done")
+            debug("apps_set_volumes_names() done")
 
     def restart_local_services(self):
         with verbosity(2):
             if self.required_services:
                 show("Services to restart:", pformat(self.required_services))
             else:
                 info("Services to restart: None")
@@ -785,169 +980,169 @@
         nginx_reload()
 
     def apps_generate_ports(self):
         start_ports = config.read("nua", "ports", "start") or 8100
         end_ports = config.read("nua", "ports", "end") or 9000
         allocated_ports = self.configured_ports()
         with verbosity(4):
-            vprint(f"apps_generate_ports(): {allocated_ports=}")
+            debug(f"apps_generate_ports(): {allocated_ports=}")
         # list of ports used for domains / apps, trying to keep them unchanged
         ports_instances_domains = store.ports_instances_domains()
         with verbosity(4):
-            vprint(f"apps_generate_ports(): {ports_instances_domains=}")
+            debug(f"apps_generate_ports(): {ports_instances_domains=}")
         allocated_ports.update(ports_instances_domains)
         with verbosity(3):
-            vprint(f"apps_generate_ports() used ports:\n {allocated_ports=}")
+            debug(f"apps_generate_ports() used ports:\n {allocated_ports=}")
         self.apps_allocate_ports(
             port_allocator(start_ports, end_ports, allocated_ports)
         )
         with verbosity(3):
-            vprint("apps_generate_ports() done")
+            debug("apps_generate_ports() done")
 
     def configured_ports(self) -> set[int]:
         """Return set of required host ports (aka non auto ports) from
         site_list.
 
         Returns: set of integers
         """
         used = set()
-        for site in self.apps:
-            used.update(site.used_ports())
+        for app in self.apps:
+            used.update(app.used_ports())
         return used
 
     def apps_allocate_ports(self, allocator: Callable):
         """Update site dict with auto generated ports."""
-        for site in self.apps:
-            site.allocate_auto_ports(allocator)
-            for resource in site.resources:
+        for app in self.apps:
+            app.allocate_auto_ports(allocator)
+            for resource in app.resources:
                 resource.allocate_auto_ports(allocator)
 
-    def evaluate_container_params(self, site: AppInstance):
+    def evaluate_container_params(self, app: AppInstance):
         """Compute site run environment parameters except those requiring late
         evaluation (i.e. host names of started containers)."""
-        self.generate_app_container_run_parameters(site)
-        for resource in site.resources:
+        self.generate_app_container_run_parameters(app)
+        for resource in app.resources:
             self.generate_resource_container_run_parameters(resource)
 
     def apps_retrieve_persistent(self):
-        for site in self.apps:
-            self.retrieve_persistent(site)
+        for app in self.apps:
+            self.retrieve_persistent(app)
 
-    def retrieve_persistent(self, site: AppInstance):
-        previous = store.instance_persistent(site.domain, site.app_id)
-        # previous = store.instance_persistent(site.instance_name_internal)
+    def retrieve_persistent(self, app: AppInstance):
+        previous = store.instance_persistent(app.label_id)
         with verbosity(4):
-            vprint(f"persistent previous: {previous=}")
-        previous.update(site.persistent_full_dict())
-        site.set_persistent_full_dict(previous)
+            debug(f"persistent previous: {previous=}")
+        previous.update(app.persistent_full_dict())
+        app.set_persistent_full_dict(previous)
 
     def apps_evaluate_dynamic_values(self):
-        for site in self.apps:
-            self.evaluate_dynamic_values(site)
+        for app in self.apps:
+            self.evaluate_dynamic_values(app)
 
-    def evaluate_dynamic_values(self, site: AppInstance):
-        ordered_resources = site.order_resources_dependencies()
+    def evaluate_dynamic_values(self, app: AppInstance):
+        ordered_resources = app.order_resources_dependencies()
         for resource in ordered_resources:
-            if resource == site:
-                self.generate_app_env_port_values(site)
+            if resource == app:
+                self.generate_app_env_port_values(app)
             else:
-                self.generate_resource_env_port_values(site, resource)
+                self.generate_resource_env_port_values(app, resource=resource)
 
-    def generate_app_env_port_values(self, site: AppInstance):
-        run_env = deepcopy(site.env)
-        run_env.update(instance_key_evaluator(site, late_evaluation=False))
-        site.env = run_env
+    def generate_app_env_port_values(self, app: AppInstance):
+        run_env = deepcopy(app.env)
+        run_env.update(instance_key_evaluator(app, late_evaluation=False))
+        app.env = run_env
         new_port_list = []
-        for port in site.port_list:
+        for port in app.port_list:
             new_port = deepcopy(port)
             new_port.update(
                 instance_key_evaluator(
-                    site,
+                    app,
                     port=port,
                     late_evaluation=False,
                 )
             )
             new_port_list.append(new_port)
-        site.port_list = new_port_list
+        app.port_list = new_port_list
 
-    def generate_resource_env_port_values(self, site: AppInstance, resource: Resource):
+    def generate_resource_env_port_values(self, app: AppInstance, resource: Resource):
         run_env = deepcopy(resource.env)
         run_env.update(
-            instance_key_evaluator(site, resource=resource, late_evaluation=False)
+            instance_key_evaluator(app, resource=resource, late_evaluation=False)
         )
         resource.env = run_env
 
-    def start_network(self, site: AppInstance):
-        if site.network_name:
-            create_container_private_network(site.network_name)
+    def start_network(self, app: AppInstance):
+        if app.network_name:
+            create_container_private_network(app.network_name)
 
-    def start_resources_containers(self, site: AppInstance):
-        for resource in site.resources:
+    def start_resources_containers(self, app: AppInstance):
+        for resource in app.resources:
             if resource.is_docker_type():
                 mounted_volumes = mount_resource_volumes(resource)
                 start_one_container(resource, mounted_volumes)
                 # until we check startup of container or set value in parameters...
                 time.sleep(2)
 
-    def setup_resources_db(self, site: AppInstance):
-        for resource in site.resources:
+    def setup_resources_db(self, app: AppInstance):
+        for resource in app.resources:
             resource.setup_db()
 
-    def merge_volume_only_resources(self, site: AppInstance):
-        for resource in site.resources:
+    def merge_volume_only_resources(self, app: AppInstance):
+        for resource in app.resources:
             if resource.volume_declaration:
-                site.volume = site.volume + resource.volume_declaration
+                app.volume = app.volume + resource.volume_declaration
 
-    def start_main_app_container(self, site: AppInstance):
+    def start_main_app_container(self, app: AppInstance):
         # volumes need to be mounted before beeing passed as arguments to
         # docker.run()
-        mounted_volumes = mount_resource_volumes(site)
-        start_one_container(site, mounted_volumes)
+        mounted_volumes = mount_resource_volumes(app)
+        start_one_container(app, mounted_volumes)
 
-    def store_container_instance(self, site: AppInstance):
+    def store_container_instance(self, app: AppInstance):
         with verbosity(3):
             bold_debug("Saving AppInstance configuration in Nua DB")
         store.store_instance(
-            app_id=site.app_id,
-            nua_tag=site.nua_tag,
-            domain=site.domain,
-            container=site.container_name,
-            image=site.image,
-            state=site.running_status,
-            site_config=dict(site),
+            app_id=app.app_id,
+            label_id=app.label_id,
+            nua_tag=app.nua_tag,
+            domain=app.domain,
+            container=app.container_name,
+            image=app.image,
+            state=app.running_status,
+            site_config=dict(app),
         )
 
-    def generate_app_container_run_parameters(self, site: AppInstance):
+    def generate_app_container_run_parameters(self, app: AppInstance):
         """Return suitable parameters for the docker.run() command.
 
         Does not include the internal_secrets, that are passed only at
         docker.run() execution, thus secrets not stored in instance
         data.
         """
         # base defaults hardcoded and from nua orchestrator configuration
         run_params = deepcopy(RUN_BASE)
         nua_docker_default_run = config.read("nua", "docker_default_run") or {}
         run_params.update(nua_docker_default_run)
         # run parameters defined in the image configuration, without the "env"
         # sections:
-        nua_conf_docker = deepcopy(site.image_nua_config.get("docker", {}))
+        nua_conf_docker = deepcopy(app.image_nua_config.get("docker", {}))
         if "env" in nua_conf_docker:
             del nua_conf_docker["env"]
         run_params.update(nua_conf_docker)
         # update with parameters that could be added to AppInstance configuration :
-        run_params.update(site.get("docker", {}))
+        run_params.update(app.get("docker", {}))
         # Add the hostname/IP of local Docker hub (Docker feature) :
         self.add_host_gateway_to_extra_hosts(run_params)
-        run_params["name"] = site.container_name
-        run_params["ports"] = site.ports_as_docker_params()
-        run_params["environment"] = site.env
-        if site.healthcheck:
-            run_params["healthcheck"] = HealthCheck(site.healthcheck).as_docker_params()
+        run_params["name"] = app.container_name
+        run_params["ports"] = app.ports_as_docker_params()
+        run_params["environment"] = app.env
+        if app.healthcheck:
+            run_params["healthcheck"] = HealthCheck(app.healthcheck).as_docker_params()
         self.sanitize_run_params(run_params)
-        site.run_params = run_params
+        app.run_params = run_params
 
     def generate_resource_container_run_parameters(
         self,
         resource: Resource,
     ):
         """Return suitable parameters for the docker.run() command (for
         Resource)."""
@@ -972,25 +1167,25 @@
 
     @staticmethod
     def sanitize_run_params(run_params: dict):
         """Docker constraint: 2 docker options not compatible."""
         if "restart_policy" in run_params:
             run_params["auto_remove"] = False
 
-    def services_environment(self, site: AppInstance) -> dict:
+    def services_environment(self, app: AppInstance) -> dict:
         run_env = {}
-        for service in site.local_services:
+        for service in app.local_services:
             handler = self.available_services[service]
             # function may need or not site param:
-            run_env.update(handler.environment(site))
+            run_env.update(handler.environment(app))
         return run_env
 
-    def resources_environment(self, site: AppInstance) -> dict:
+    def resources_environment(self, app: AppInstance) -> dict:
         run_env = {}
-        for resource in site.resources:
+        for resource in app.resources:
             run_env.update(resource.environment_ports())
         return run_env
 
     def post_deployment(self):
         self.store_deploy_configs_after_swap()
         self.display_deployment_status()
 
@@ -1009,27 +1204,27 @@
     def display_deployed_apps(self):
         if not self.apps:
             show("No app deployed.")
             return
 
         show("Deployed apps:")
         protocol = protocol_prefix()
-        for site in self.apps:
-            msg = f"Instance name: {site.instance_name_internal}"
+        for app in self.apps:
+            msg = f"Label: {app.label_id}"
             info(msg)
-            msg = f"Image '{site.image}' deployed as {protocol}{site.domain}"
+            msg = f"Image '{app.image}' deployed as {protocol}{app.domain}"
             info(msg)
-            msg = f"Deployment status: {site.running_status}"
+            msg = f"Deployment status: {app.running_status}"
             info(msg)
-            self.display_persistent_data(site)
+            self.display_persistent_data(app)
         print()
 
-    def display_persistent_data(self, site: AppInstance):
+    def display_persistent_data(self, app: AppInstance):
         with verbosity(3):
-            content = site.persistent_full_dict()
+            content = app.persistent_full_dict()
             if content:
                 bold_debug("Persistent generated variables:")
                 debug(pformat(content))
 
     def display_used_volumes(self):
         with verbosity(1):
             current_mounted = store.list_instances_container_active_volumes()
@@ -1040,22 +1235,24 @@
                 show(Volume.string(volume))
 
     def display_unused_volumes(self):
         with verbosity(1):
             unused = unused_volumes(self.orig_mounted_volumes)
             if not unused:
                 return
-            print_green(
+            important(
                 "Some volumes are mounted but not used by current Nua configuration:"
             )
             for volume in unused:
-                vprint(Volume.string(volume))
+                show(Volume.string(volume))
 
     def print_host_list(self):
-        vprint("apps per domain:\n", pformat(self.apps_per_domain))
+        # used with verbosity 3
+        bold_debug("apps per domain:\n")
+        debug(pformat(self.apps_per_domain))
 
 
 def _verify_located(host: dict):
     """host format:
 
      {'hostname': 'test.example.com',
       'apps': [{'domain': 'test.example.com/instance1',
@@ -1125,11 +1322,11 @@
     else:
         hostname = host["hostname"]
         warning(f"too many apps for {hostname=}, site discarded:")
         site = host["apps"].pop(0)
         valid_apps = [site]
         for site in host["apps"]:
             image = site.image
-            print_red(f"    {image=} / {site['domain']}")
+            red_line(f"    {image=} / {site['domain']}")
 
     host["apps"] = valid_apps
     host["located"] = False
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/app_instance.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/app_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 from copy import deepcopy
 from pathlib import Path
 from pprint import pformat
 
 from nua.agent.nua_config import hyphen_get
 from nua.agent.nua_tag import nua_tag_string
-from nua.lib.panic import Abort, info, vprint, warning
+from nua.lib.panic import Abort, debug, info, warning
 from nua.lib.tool.state import verbosity
 
 from .db.model.instance import STOPPED
 from .domain_split import DomainSplit
 from .persistent import Persistent
 from .port_normalization import (
     normalize_ports_list,
     ports_as_list,
     rebase_ports_on_defaults,
 )
 from .resource import Resource
 from .resource_deps import ResourceDeps
 from .search_cmd import search_nua
-from .utils import sanitized_name
 from .volume import Volume
 
 
 class AppInstance(Resource):
     MANDATORY_KEYS = ("image", "domain")
 
     def __init__(self, app_instance_dict: dict):
@@ -46,15 +45,15 @@
         return app_instance
 
     def check_valid(self):
         self._check_mandatory()
         self._nomalize_env_values()
         self._normalize_ports()
         self._normalize_domain()
-        self._set_instance_name()
+        self._set_label_id()
 
     @property
     def resources(self) -> list:
         """List of sub resources of the AppInstance object.
 
         Warning: only AppInstance class has an actual use of 'resources'.
         The subclass Resource will always provide an *empty* list
@@ -70,20 +69,20 @@
         return self["image_nua_config"]
 
     @image_nua_config.setter
     def image_nua_config(self, image_nua_config: dict):
         self["image_nua_config"] = image_nua_config
 
     @property
-    def instance_name_internal(self) -> str:
-        return self["instance_name_internal"]
+    def label_id(self) -> str:
+        return self["label_id"]
 
     @property
-    def instance_name_user(self) -> str:
-        return self["instance_name_user"]
+    def label(self) -> str:
+        return self["label"]
 
     @property
     def top_domain(self) -> str:
         return self["top_domain"]
 
     @top_domain.setter
     def top_domain(self, top_domain: str):
@@ -125,18 +124,19 @@
     @property
     def nua_dash_name(self) -> str:
         return self.nua_tag.replace(":", "-")
 
     @property
     def container_name(self) -> str:
         # override the method of Resource
-        suffix = DomainSplit(self.domain).container_suffix()
-        name = sanitized_name(f"{self.nua_dash_name}-{suffix}")
-        self["container_name"] = name
-        return name
+        # suffix = DomainSplit(self.domain).container_suffix()
+        # name = sanitized_name(f"{self.nua_dash_name}-{suffix}")
+        # self["container_name"] = name
+        # return name
+        return f"{self.label_id}-{self.app_id}"
 
     @property
     def running_status(self) -> str:
         return self.get("running_status", STOPPED)
 
     @running_status.setter
     def running_status(self, status: str):
@@ -165,15 +165,21 @@
     def set_persistent_full_dict(self, persist_dict: dict):
         self["persistent"] = persist_dict
 
     def parse_healthcheck(self):
         self._parse_healthcheck(self.image_nua_config.get("healthcheck", {}))
 
     def set_volumes_names(self):
-        suffix = DomainSplit(self.domain).container_suffix()
+        # suffix = DomainSplit(self.domain).container_suffix()
+        # self.volume = [Volume.update_name_dict(v, suffix) for v in self.volume]
+        # for resource in self.resources:
+        #     resource.volume = [
+        #         Volume.update_name_dict(v, suffix) for v in resource.volume
+        #     ]
+        suffix = self.label_id
         self.volume = [Volume.update_name_dict(v, suffix) for v in self.volume]
         for resource in self.resources:
             resource.volume = [
                 Volume.update_name_dict(v, suffix) for v in resource.volume
             ]
 
     @property
@@ -191,15 +197,15 @@
         """
         self.network_name = ""
         if any(resource.requires_network() for resource in self.resources):
             self.network_name = self.container_name
             for resource in self.resources:
                 resource.network_name = self.network_name
             with verbosity(4):
-                vprint("detect_required_network() network_name =", self.network_name)
+                debug("detect_required_network() network_name =", self.network_name)
 
     def resource_per_name(self, name: str) -> Resource | None:
         for resource in self.resources:
             if resource.resource_name == name:
                 return resource
         return None
 
@@ -258,15 +264,15 @@
     def parse_resources(self):
         resources = [
             self._parse_resource(resource_declaration)
             for resource_declaration in self.image_nua_config.get("resource", [])
         ]
         resources = [res for res in resources if res]
         with verbosity(3):
-            vprint(f"Image resources: {pformat(resources)}")
+            debug(f"Image resources: {pformat(resources)}")
         self.resources = resources
 
     def _parse_resource(self, declaration: dict) -> Resource | None:
         for required_key in ("name", "type"):
             value = declaration.get(required_key)
             if not value or not isinstance(value, str):
                 warning(
@@ -280,41 +286,49 @@
         return resource
 
     def _normalize_domain(self):
         dom = DomainSplit(self.domain)
         self.domain = dom.full_path()
         self.top_domain = dom.top_domain()
 
-    def _set_instance_name(self):
-        name = hyphen_get(self, "instance-name") or ""
-        if not "_".join(name.split()):
-            name = self.default_instance_name()
+    def _set_label_id(self):
+        label = hyphen_get(self, "label") or ""
+        if not "_".join(label.split()):
+            label = self.default_label()
             with verbosity(0):
-                info(f"Instance name not provided, using default: '{name}'")
-        self.set_instance_name(name)
+                info(f"Label not provided, using default: '{label}'")
+        self.set_instance_label(label)
 
-    def set_instance_name(self, name: str):
-        name_internal = "_".join(name.split())
-        if not name_internal:
-            raise ValueError("Empty name instance is not allowed")
-        self["instance_name_internal"] = name_internal
-        self["instance_name_user"] = name.strip()
+    def default_label(self):
+        """Return a label based on app id and domain.
+
+        To use when the user does not provide an app label or as default
+        value.
+        """
+        return f"{self.image_short}-{self.domain}"
+
+    def set_instance_label(self, label: str):
+        label_id = "_".join(label.split())
+        if not label_id:
+            raise ValueError("Empty label is not allowed")
+        self["label_id"] = label_id
+        self["label"] = label.strip()
 
     def rebase_volumes_upon_nua_conf(self):
         self.volume = self.rebased_volumes_upon_package_conf(self.image_nua_config)
 
     def rebase_ports_upon_nua_config(self):
         nua_config_ports = deepcopy(self.image_nua_config.get("port", {}))
         if not isinstance(nua_config_ports, dict):
             raise Abort("nua_config['port'] must be a dict")
 
         base_ports = normalize_ports_list(ports_as_list(nua_config_ports))
         self.port_list = rebase_ports_on_defaults(base_ports, self.port_list)
         with verbosity(4):
-            vprint(f"rebase_ports_upon_nua_config(): ports={pformat(self.port_list)}")
+            debug(f"rebase_ports_upon_nua_config(): ports={pformat(self.port_list)}")
 
     def find_registry_path(self, cached: bool = False) -> bool:
         # list of images sorted by version:
         if cached and self.registry_path:
             return True
         results = self._search_nua_registry()
         if results:
@@ -338,15 +352,7 @@
         for resource in self.resources:
             if resource.is_docker_type():
                 name = f"{self.container_name}-{resource.base_name}"
                 resource.container_name = name
                 # docker resources are only visible from bridge network, so use
                 # the container name as hostname
                 resource.hostname = name
-
-    def default_instance_name(self):
-        """Return a name based on app id and domain.
-
-        To use when the user does not provide an app name or as default
-        value.
-        """
-        return f"{self.image_short}-{self.domain}"
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/app_management.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/app_management.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/assign/engine.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/assign/engine.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/assign/evaluators.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/assign/evaluators.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_engine.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_engine.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_functions.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_functions.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_report.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_report.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/bootstrap/bootstrap.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/certbot.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/certbot.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/commands.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/commands.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf` & `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/installer.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/installer.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/api.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/deploy_remove.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/deploy_remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,9 +45,9 @@
     deployer = AppDeployment()
     deployer.local_services_inventory()
     deployer.load_deployed_configuration()
     additional = AppDeployment()
     additional.local_services_inventory()
     additional.load_deploy_config(merge_config)
     additional.gather_requirements()
-    deployer.merge(additional)
+    deployer.merge_sequential(additional)
     deployer.post_deployment()
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/restore.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/start_stop.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/start_stop.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/status.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/configuration.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/debug.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/debug.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/init.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/init.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/main.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/auth.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/auth.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/deployconfig.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/deployconfig.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/host.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/host.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/image.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/image.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/instance.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,22 @@
     There can be only one app per domain.
     """
 
     __tablename__ = "instance"
 
     id = Column(Integer, primary_key=True)
     app_id = Column(String(80))
+    label_id = Column(String(80))
     nua_tag = Column(String(160))
     domain = Column(String(160))
     container = Column(String(160), default="")
     image = Column(String(160), default="")
     state = Column(String(16), default=STOPPED)
     created = Column(String(40))
     site_config = Column(JSON)
     #  broken for sqlite: instance = index_property("data", "instance", default="")
 
     def __repr__(self) -> str:
-        return f"Instance(app_id={self.app_id}, container='{self.container}', tag={self.nua_tag})"
+        return (
+            f"Instance(label_id={self.label_id}, app_id={self.app_id}, "
+            f"container='{self.container}', tag={self.nua_tag})"
+        )
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/setting.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/setting.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db/store.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,38 +214,40 @@
         user = session.query(User).filter(User.username == username).first()
         if not user:
             return None
         return deepcopy(user.data)
 
 
 def store_instance(
-    app_id="",
-    nua_tag="",
-    domain="",
-    container="",
-    image="",
-    state=STOPPED,
-    site_config=None,
-):
+    app_id: str = "",
+    label_id: str = "",
+    nua_tag: str = "",
+    domain: str = "",
+    container: str = "",
+    image: str = "",
+    state: str = STOPPED,
+    site_config: dict | None = None,
+) -> None:
     """Store a Nua instance in the local DB (table 'instance')."""
 
     new_instance = Instance(
         app_id=app_id,
+        label_id=label_id,
         nua_tag=nua_tag,
         domain=domain,
         container=container,
         image=image,
         state=state,
         created=now_iso(),
         site_config=site_config or {},
     )
     with Session() as session:
         # Image:
         # enforce unicity
-        existing = session.query(Instance).filter_by(domain=domain).first()
+        existing = session.query(Instance).filter_by(label_id=label_id).first()
         if existing:
             session.delete(existing)
         session.flush()
         session.add(new_instance)
         session.commit()
 
 
@@ -418,23 +420,22 @@
     with Session() as session:
         existing = session.query(Instance).filter_by(domain=domain).first()
         if existing:
             existing.state = state
             session.commit()
 
 
-def instance_persistent(domain: str, app_id: str) -> dict:
-    """Return the persistent dictionary if (or an empty dict if not found)"""
+def instance_persistent(label_id: str) -> dict:
+    """Return the persistent dictionary if (or an empty dict if not found)."""
     persistent = {}
     with Session() as session:
         existing = (
             session.query(Instance)
             .filter_by(
-                domain=domain,
-                app_id=app_id,
+                label_id=label_id,
             )
             .first()
         )
         if existing:
             site_config = existing.site_config
             persistent = site_config.get("persistent", {})
     return persistent
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/tools.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/tools.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.json` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mongo.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mongo.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.json` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/redis-cache.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/redis-cache.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/sqlite.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/sqlite.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/mariadb_utils.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/mariadb_utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/postgres_utils.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/default_conf/nua_defaults_settings.toml` & `nua_orchestrator-0.5.14/src/nua/orchestrator/default_conf/nua_defaults_settings.toml`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/deploy_utils.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/deploy_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,19 +257,19 @@
     for name in container_names:
         if not name:
             continue
         docker_remove_container_previous(name, show_warning)
         store.instance_delete_by_container(name)
 
 
-def deactivate_app(site: AppInstance):
+def deactivate_app(app: AppInstance):
     """Deactive containers of AppInstance and all sub Resources (updating
     orchestrator DB)."""
-    container_names = [res.container_name for res in site.resources]
-    container_names.append(site.container_name)
+    container_names = [res.container_name for res in app.resources]
+    container_names.append(app.container_name)
     deactivate_containers(container_names, show_warning=False)
 
 
 def deactivate_all_instances():
     """Find all instances in DB.
 
     - remove container if it exists
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/docker_utils.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/docker_utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/domain_split.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/domain_split.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/healthcheck.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/healthcheck.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/higher_package.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/higher_package.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/internal_secrets.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/internal_secrets.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/cmd.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/cmd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/css/style.css` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/css/style.css`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/index.html` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/index.html`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/installer.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/installer.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/default_site` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/default_site`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_located.j2` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_not_located.j2` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_located.j2` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located.j2` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/nginx.conf` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/utils.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nua_db_setup.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nua_db_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 def setup_first_launch():
     settings = store.installed_nua_settings()
     if not settings:
         print_green(
             f"First launch: set Nua defaults in '{config.read('nua', 'db', 'url')}'"
         )
         return set_default_settings()
+
     installed_version = settings.get("version", "")
     if installed_version == __version__:
         return set_db_url_in_settings(settings)
     else:
         print_red(
             f"Updating Nua settings from version {settings['version']} "
             f"by version {__version__} defaults"
```

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/nua_env.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/nua_env.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/persistent.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/persistent.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/port_normalization.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/port_normalization.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/register_plugins.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/register_plugins.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/registry.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/registry.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/resource.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/resource.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/resource_deps.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/resource_deps.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/docker_remove_all.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/docker_remove_all.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/mariadb_restore.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/mariadb_restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_instances.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_instances.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/set_pg_pwd.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/set_pg_pwd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/search_cmd.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/search_cmd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/services/postgres.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/services/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_base.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_base.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_loader.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_loader.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/util/deep_access_dict.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/util/deep_access_dict.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/utils.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/src/nua/orchestrator/volume.py` & `nua_orchestrator-0.5.14/src/nua/orchestrator/volume.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.13/PKG-INFO` & `nua_orchestrator-0.5.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nua-orchestrator
-Version: 0.5.13
+Version: 0.5.14
 Summary: Nua orchestrator - local implementation
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=1.4.36,<2.0.0)
 Requires-Dist: SQLAlchemy-serializer (>=1.4.1,<2.0.0)
 Requires-Dist: docker (>=6,<7)
-Requires-Dist: nua-agent (==0.5.13)
-Requires-Dist: nua-autobuild (==0.5.13)
-Requires-Dist: nua-build (==0.5.13)
-Requires-Dist: nua-lib (==0.5.13)
+Requires-Dist: nua-agent (==0.5.14)
+Requires-Dist: nua-autobuild (==0.5.14)
+Requires-Dist: nua-build (==0.5.14)
+Requires-Dist: nua-lib (==0.5.14)
 Requires-Dist: paramiko (>=2.11.0,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21,<0.22)
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2,<3)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
```

