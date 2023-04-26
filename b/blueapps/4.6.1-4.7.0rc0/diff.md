# Comparing `tmp/blueapps-4.6.1.tar.gz` & `tmp/blueapps-4.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blueapps-4.6.1.tar", last modified: Mon Apr 24 12:02:16 2023, max compression
+gzip compressed data, was "dist/blueapps-4.7.0rc0.tar", last modified: Wed Apr 26 07:49:57 2023, max compression
```

## Comparing `blueapps-4.6.1.tar` & `blueapps-4.7.0rc0.tar`

### file list

```diff
@@ -1,220 +1,249 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/middleware/
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/request_provider.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/middleware/bkui/
--rw-r--r--   0 root         (0) root         (0)     1296 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/bkui/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/bkui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/middleware/xss/
--rw-r--r--   0 root         (0) root         (0)     2516 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/xss/decorators.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/xss/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/xss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7918 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/xss/pxfilter.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/middleware/xss/utils.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/utils/
--rw-r--r--   0 root         (0) root         (0)     4673 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/request_provider.py
--rw-r--r--   0 root         (0) root         (0)      884 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2887 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/jwt_client.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/esbclient.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/fancy_dict.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/unique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/utils/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/utils/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)     1432 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/utils/sites/open/
--rw-r--r--   0 root         (0) root         (0)     1337 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/sites/open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/utils/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)     1427 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/utils/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/opentelemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/opentelemetry/docs/
--rw-r--r--   0 root         (0) root         (0)     1420 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/docs/metric.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/opentelemetry/docs/assets/
--rw-r--r--   0 root         (0) root         (0)   169851 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/docs/assets/local_jaeger.png
--rw-r--r--   0 root         (0) root         (0)     3491 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/docs/trace.md
--rw-r--r--   0 root         (0) root         (0)     1859 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/opentelemetry/metrics/
--rw-r--r--   0 root         (0) root         (0)     2658 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/metrics/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/metrics/instrumentor.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/metrics/server.py
--rw-r--r--   0 root         (0) root         (0)     1109 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/metrics/celery.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4566 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/instrumentor.py
--rw-r--r--   0 root         (0) root         (0)     5064 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/setup.py
--rw-r--r--   0 root         (0) root         (0)      671 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/README.md
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/opentelemetry/instrument_app/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/instrument_app/apps.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/instrument_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/instrument_app/celery.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/opentelemetry/utils.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/core/
--rw-r--r--   0 root         (0) root         (0)     1409 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/core/exceptions/
--rw-r--r--   0 root         (0) root         (0)     3687 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/exceptions/base.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/exceptions/middleware.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/core/handler/
--rw-r--r--   0 root         (0) root         (0)     1593 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/handler/wsgi.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/handler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/core/celery/
--rw-r--r--   0 root         (0) root         (0)      835 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/celery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/celery/celery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/core/sites/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/sites/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/core/sites/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/conf/
--rw-r--r--   0 root         (0) root         (0)     5600 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/log.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/database.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/environ.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/validators.py
--rw-r--r--   0 root         (0) root         (0)     5362 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/default_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/conf/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/conf/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      942 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/conf/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/sites/open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/conf/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      986 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/conf/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/
--rw-r--r--   0 root         (0) root         (0)     5954 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/base.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/app.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/handlers/
--rw-r--r--   0 root         (0) root         (0)     6356 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/
--rw-r--r--   0 root         (0) root         (0)     2489 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/celerybeat.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/celery.py
--rw-r--r--   0 root         (0) root         (0)     7158 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/management/templates.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      833 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/bk_commands/test.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/dummy/
--rw-r--r--   0 root         (0) root         (0)     1005 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/dummy/dummy_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/dummy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/patch/
--rw-r--r--   0 root         (0) root         (0)     3773 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/patch/log.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/patch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/patch/settings_paas_services.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/patch/settings_open_saas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/
--rw-r--r--   0 root         (0) root         (0)     1046 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/decorators.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/management/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/management/commands/
--rw-r--r--   0 root         (0) root         (0)     1079 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/management/commands/apigw_clean_cache.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/apps.py
--rw-r--r--   0 root         (0) root         (0)     1287 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/utils/
--rw-r--r--   0 root         (0) root         (0)      940 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/utils/sms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/handlers/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6749 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/handlers/response.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/views.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/static/account/
--rw-r--r--   0 root         (0) root         (0)     2049 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/static/account/login.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/bk_token/
--rw-r--r--   0 root         (0) root         (0)     3176 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_token/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7830 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_token/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_token/models.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_token/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/null/
--rw-r--r--   0 root         (0) root         (0)      941 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/null/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/bk_ticket/
--rw-r--r--   0 root         (0) root         (0)     3634 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_ticket/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_ticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_ticket/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_ticket/models.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_ticket/forms.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/weixin/
--rw-r--r--   0 root         (0) root         (0)     4669 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/weixin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/weixin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/weixin/backends.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/weixin/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/rio/
--rw-r--r--   0 root         (0) root         (0)     3337 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/rio/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/rio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/rio/backends.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/rio/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/bk_jwt/
--rw-r--r--   0 root         (0) root         (0)     2307 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_jwt/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/bk_jwt/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/components/ptlogin/
--rw-r--r--   0 root         (0) root         (0)     3668 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/ptlogin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/ptlogin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/ptlogin/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/ptlogin/models.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/components/ptlogin/forms.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/templates/account/
--rw-r--r--   0 root         (0) root         (0)     1905 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/templates/account/login_page.html
--rw-r--r--   0 root         (0) root         (0)     1355 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/templates/account/login_success.html
--rw-r--r--   0 root         (0) root         (0)     1946 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/readme.md
--rw-r--r--   0 root         (0) root         (0)     1249 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/backends.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/conf.py
--rw-r--r--   0 root         (0) root         (0)     8875 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/models.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/migrations/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/migrations/0003_verifyinfo.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/migrations/0002_init_superuser.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/migrations/0004_create_cache_table.py
--rw-r--r--   0 root         (0) root         (0)     7369 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/migrations/0001_initial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/ieod/conf.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/open/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/open/conf.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/account/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/tencent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/account/sites/tencent/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/template/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps/template/backends/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/template/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4226 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/template/backends/mako.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-04-24 11:59:25.000000 blueapps-4.6.1/blueapps/template/context_processors.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-24 11:59:25.000000 blueapps-4.6.1/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     6106 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     4153 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      938 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-24 12:02:16.000000 blueapps-4.6.1/blueapps.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      833 2023-04-24 11:59:25.000000 blueapps-4.6.1/test.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-04-24 11:59:25.000000 blueapps-4.6.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     3383 2023-04-24 11:59:25.000000 blueapps-4.6.1/README.md
--rw-r--r--   0 root         (0) root         (0)     4153 2023-04-24 12:02:16.000000 blueapps-4.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-24 12:02:16.000000 blueapps-4.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7810 2023-04-24 11:59:25.000000 blueapps-4.6.1/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/middleware/
+-rw-r--r--   0 root         (0) root         (0)      842 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/request_provider.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/middleware/bkui/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/bkui/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/bkui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7918 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/pxfilter.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/utils.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/base.py
+-rw-r--r--   0 root         (0) root         (0)     3778 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/lock.py
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/request_provider.py
+-rw-r--r--   0 root         (0) root         (0)      884 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/jwt_client.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/time.py
+-rw-r--r--   0 root         (0) root         (0)     8333 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/esbclient.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/fancy_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/json.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/unique.py
+-rw-r--r--   0 root         (0) root         (0)     3694 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/db.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/local.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/open/
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/open/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/metric.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/assets/
+-rw-r--r--   0 root         (0) root         (0)   169851 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/assets/local_jaeger.png
+-rw-r--r--   0 root         (0) root         (0)     3491 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/trace.md
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/instrumentor.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/server.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/celery.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrumentor.py
+-rw-r--r--   0 root         (0) root         (0)     4919 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/setup.py
+-rw-r--r--   0 root         (0) root         (0)      671 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/README.md
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/apps.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/celery.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/
+-rw-r--r--   0 root         (0) root         (0)     5628 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/base.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/middleware.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/handler/
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/handler/wsgi.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/handler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/celery/
+-rw-r--r--   0 root         (0) root         (0)      835 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/celery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/celery/celery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/sites/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/sites/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/sites/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/
+-rw-r--r--   0 root         (0) root         (0)     5600 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/log.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/database.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/environ.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/validators.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      942 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/open/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/
+-rw-r--r--   0 root         (0) root         (0)     5954 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/base.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/app.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/
+-rw-r--r--   0 root         (0) root         (0)     6356 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celerybeat.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celery.py
+-rw-r--r--   0 root         (0) root         (0)     7158 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/templates.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      833 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/test.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/test/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/test/override_middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/dummy/
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/dummy/dummy_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/dummy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/serializer_fields.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/filters.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/pagination.py
+-rw-r--r--   0 root         (0) root         (0)     5453 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/serializers.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/viewset_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/viewsets.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/README.md
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/renderers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/swagger/
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/swagger/schemas.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/patch/
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/log.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/settings_paas_services.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/settings_open_saas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/management/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/management/commands/apigw_clean_cache.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/utils/
+-rw-r--r--   0 root         (0) root         (0)      940 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/utils/sms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/handlers/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6562 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/handlers/response.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/views.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/static/account/
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/static/account/login.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7830 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/models.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/null/
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/null/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/models.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/forms.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/backends.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/
+-rw-r--r--   0 root         (0) root         (0)     3668 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/models.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/templates/account/
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/templates/account/login_page.html
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/templates/account/login_success.html
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/readme.md
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/backends.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/conf.py
+-rw-r--r--   0 root         (0) root         (0)     8875 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/models.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0003_verifyinfo.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0002_init_superuser.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0004_create_cache_table.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0001_initial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/ieod/conf.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/open/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/tencent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/tencent/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/template/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/template/backends/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/backends/mako.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/context_processors.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      961 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      833 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/test.py
+-rw-r--r--   0 root         (0) root         (0)     4038 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     7810 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/LICENSE.txt
```

### Comparing `blueapps-4.6.1/blueapps/middleware/request_provider.py` & `blueapps-4.7.0rc0/blueapps/middleware/request_provider.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/__init__.py` & `blueapps-4.7.0rc0/blueapps/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/bkui/middlewares.py` & `blueapps-4.7.0rc0/blueapps/middleware/bkui/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/bkui/__init__.py` & `blueapps-4.7.0rc0/blueapps/middleware/bkui/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/xss/decorators.py` & `blueapps-4.7.0rc0/blueapps/middleware/xss/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/xss/middlewares.py` & `blueapps-4.7.0rc0/blueapps/middleware/xss/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/xss/__init__.py` & `blueapps-4.7.0rc0/blueapps/middleware/xss/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/xss/pxfilter.py` & `blueapps-4.7.0rc0/blueapps/middleware/xss/pxfilter.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/middleware/xss/utils.py` & `blueapps-4.7.0rc0/blueapps/middleware/xss/utils.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/__init__.py` & `blueapps-4.7.0rc0/blueapps/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-VERSION = "4.6.1"
+VERSION = "4.7.0rc0"
 __version__ = VERSION
 
 
 RUN_VER = ""
 
 
 def get_run_ver():
```

### Comparing `blueapps-4.6.1/blueapps/utils/request_provider.py` & `blueapps-4.7.0rc0/blueapps/utils/request_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
+import sys
+import uuid
 
 from django.dispatch import Signal
 from django.utils.deprecation import MiddlewareMixin
 
 from blueapps.conf import settings
 from blueapps.core.exceptions import AccessForbidden, ServerBlueException
+from blueapps.settings import blueapps_settings
+from blueapps.utils.local import inject_request_id, release_request_local, request_local
 
 # since each thread has its own greenlet we can just use those as identifiers
 # for the context.  If greenlets are not available we fall back to the
 # current thread ident depending on where it is.
 try:
     from greenlet import getcurrent as get_ident
 except ImportError:
@@ -32,17 +36,15 @@
 class AccessorSignal(Signal):
     allowed_receiver = "blueapps.utils.request_provider.RequestProvider"
 
     def __init__(self, providing_args=None):
         Signal.__init__(self, providing_args)
 
     def connect(self, receiver, sender=None, weak=True, dispatch_uid=None):
-        receiver_name = ".".join(
-            [receiver.__class__.__module__, receiver.__class__.__name__]
-        )
+        receiver_name = ".".join([receiver.__class__.__module__, receiver.__class__.__name__])
         if receiver_name != self.allowed_receiver:
             raise AccessForbidden(u"%s is not allowed to connect" % receiver_name)
         Signal.connect(self, receiver, sender, weak, dispatch_uid)
 
 
 request_accessor = AccessorSignal()
 
@@ -61,17 +63,15 @@
 
     def __init__(self, get_response):
         super(RequestProvider, self).__init__(get_response)
         self._request_pool = {}
         request_accessor.connect(self)
 
     def process_request(self, request):
-        request.is_mobile = lambda: bool(
-            settings.RE_MOBILE.search(request.META.get("HTTP_USER_AGENT", ""))
-        )
+        request.is_mobile = lambda: bool(settings.RE_MOBILE.search(request.META.get("HTTP_USER_AGENT", "")))
 
         # 是否为合法的RIO请求
         request.is_rio = lambda: bool(
             request.META.get("HTTP_STAFFNAME", "")
             and getattr(settings, "RIO_TOKEN", None)
             and settings.RE_WECHAT.search(request.META.get("HTTP_USER_AGENT", ""))
         )
@@ -84,18 +84,21 @@
             and not request.is_rio()
         )
 
         # JWT请求
         request.is_bk_jwt = lambda: bool(request.META.get("HTTP_X_BKAPI_JWT", ""))
 
         self._request_pool[get_ident()] = request
+        request_local.request = request
+        inject_request_id(request_local, request)
         return None
 
     def process_response(self, request, response):
         assert request is self._request_pool.pop(get_ident())
+        release_request_local()
         return response
 
     def __call__(self, *args, **kwargs):
         """
         1）接受 signal 请求响应，
         2）继承 MiddlewareMixin.__call__ 兼容 djagno 1.10 之前中间件
         """
@@ -119,11 +122,34 @@
 
 
 def get_x_request_id():
     x_request_id = ""
     http_request = get_request()
     if hasattr(http_request, "META"):
         meta = http_request.META
-        x_request_id = (
-            meta.get("HTTP_X_REQUEST_ID", "") if isinstance(meta, dict) else ""
-        )
+        x_request_id = meta.get("HTTP_X_REQUEST_ID", "") if isinstance(meta, dict) else ""
     return x_request_id
+
+
+def get_local_request():
+    return getattr(request_local, "request", None)
+
+
+def get_local_request_id():
+    return getattr(request_local, "request_id", str(uuid.uuid4()))
+
+
+def get_or_create_local_request_id():
+    if not hasattr(request_local, "request_id"):
+        request_local.request_id = str(uuid.uuid4())
+    return request_local.request_id
+
+
+def get_request_username():
+    operator = None
+    try:
+        operator = get_local_request().user.username
+    except (IndexError, AttributeError):
+        if blueapps_settings.NON_REQUEST_USERNAME_PROVIDER:
+            operator = blueapps_settings.NON_REQUEST_USERNAME_PROVIDER()
+
+    return operator
```

### Comparing `blueapps-4.6.1/blueapps/utils/logger.py` & `blueapps-4.7.0rc0/blueapps/utils/logger.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/__init__.py` & `blueapps-4.7.0rc0/blueapps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/jwt_client.py` & `blueapps-4.7.0rc0/blueapps/utils/jwt_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/tools.py` & `blueapps-4.7.0rc0/blueapps/utils/tools.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/esbclient.py` & `blueapps-4.7.0rc0/blueapps/utils/esbclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
 
 try:
     client = SDKClient()
     backend_client = SDKClient  # pylint: disable=invalid-name
     client.patch_sdk_component_api_class()
 except ImportError as err:
-    from blueapps.dummy.dummy_client import DummyClient
+    from blueapps.contrib.dummy.dummy_client import DummyClient
 
     client = DummyClient(err)
     backend_client = DummyClient  # pylint: disable=invalid-name
 
 
 def get_client_by_user(user_or_username):
     user_model = get_user_model()
```

### Comparing `blueapps-4.6.1/blueapps/utils/fancy_dict.py` & `blueapps-4.7.0rc0/blueapps/utils/fancy_dict.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/unique.py` & `blueapps-4.7.0rc0/blueapps/utils/unique.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/sites/ieod/__init__.py` & `blueapps-4.7.0rc0/blueapps/utils/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/sites/__init__.py` & `blueapps-4.7.0rc0/blueapps/utils/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/sites/open/__init__.py` & `blueapps-4.7.0rc0/blueapps/utils/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/utils/sites/tencent/__init__.py` & `blueapps-4.7.0rc0/blueapps/utils/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/docs/metric.md` & `blueapps-4.7.0rc0/blueapps/opentelemetry/docs/metric.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/docs/assets/local_jaeger.png` & `blueapps-4.7.0rc0/blueapps/opentelemetry/docs/assets/local_jaeger.png`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/docs/trace.md` & `blueapps-4.7.0rc0/blueapps/opentelemetry/docs/trace.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/export.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/export.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/metrics/middlewares.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/metrics/__init__.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/metrics/instrumentor.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/instrumentor.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/metrics/server.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/server.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/metrics/celery.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/__init__.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/instrumentor.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/instrumentor.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 import json
-
 from typing import Collection
 
-from django.conf import settings
-
-from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation import dbapi
-from opentelemetry.trace import Span, Status, StatusCode, format_trace_id
 from opentelemetry.instrumentation.celery import CeleryInstrumentor
 from opentelemetry.instrumentation.django import DjangoInstrumentor
+from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 from opentelemetry.instrumentation.redis import RedisInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
+from opentelemetry.trace import Span, Status, StatusCode, format_trace_id
+from requests import Response
+
+from blueapps.settings import blueapps_settings
 
 
-def requests_callback(span: Span, response):
+def requests_callback(span: Span, response: Response):
     """
     处理蓝鲸标准协议响应
     """
     try:
         json_result = response.json()
     except Exception:  # pylint: disable=broad-except
         return
@@ -59,18 +59,15 @@
         or response.headers.get("x-request-id")
         # old esb
         or json_result.get("request_id", "")
     )
     if request_id:
         span.set_attribute("request_id", request_id)
 
-    if code in [0, "0", "00"]:
-        span.set_status(Status(StatusCode.OK))
-    else:
-        span.set_status(Status(StatusCode.ERROR))
+    span.set_status(Status(StatusCode.OK if response.ok else StatusCode.ERROR))
 
 
 def django_request_hook(span, request):
     """
     在request注入trace_id，方便获取
     """
     trace_id = span.get_span_context().trace_id
@@ -107,18 +104,22 @@
     def _instrument(self, **kwargs):
         LoggingInstrumentor().instrument()
         RequestsInstrumentor().instrument(span_callback=requests_callback)
         DjangoInstrumentor().instrument(request_hook=django_request_hook, response_hook=django_response_hook)
         CeleryInstrumentor().instrument()
         RedisInstrumentor().instrument()
 
-        for instrumentor in getattr(settings, "BK_APP_OTEL_ADDTIONAL_INSTRUMENTORS", []):
+        for instrumentor in blueapps_settings.BK_APP_OTEL_ADDTIONAL_INSTRUMENTORS or getattr(
+            blueapps_settings, "BK_APP_OTEL_ADDTIONAL_INSTRUMENTORS", []
+        ):
             instrumentor.instrument()
 
-        if getattr(settings, "BK_APP_OTEL_INSTRUMENT_DB_API", False):
+        if blueapps_settings.BKAPP_OTEL_INSTRUMENT_DB_API or getattr(
+            blueapps_settings, "BK_APP_OTEL_INSTRUMENT_DB_API", False
+        ):
             import MySQLdb  # noqa
 
             dbapi.wrap_connect(
                 __name__,
                 MySQLdb,
                 "connect",
                 "mysql",
```

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/setup.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,42 +11,46 @@
 specific language governing permissions and limitations under the License.
 """
 
 import os
 
 from django.conf import settings
 from django.utils.log import configure_logging
-
 from opentelemetry import trace
-from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.resources import Resource, SERVICE_NAME
-from opentelemetry.sdk.trace.sampling import _KNOWN_SAMPLERS
 from opentelemetry.exporter.jaeger.thrift import JaegerExporter
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
+from opentelemetry.sdk.resources import SERVICE_NAME, Resource
+from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.trace.sampling import _KNOWN_SAMPLERS
 
 from blueapps.core.celery import celery_app
+from blueapps.opentelemetry.constants import DEFAULT_LOGGING_TRACE_FORMAT
 from blueapps.opentelemetry.instrumentor import BKAppInstrumentor
 from blueapps.opentelemetry.metrics.celery import MetricsServerStep
 from blueapps.opentelemetry.metrics.instrumentor import SaaSMetricsInstrumentor
-from blueapps.opentelemetry.constants import DEFAULT_LOGGING_TRACE_FORMAT
 from blueapps.opentelemetry.utils import inject_logging_trace_info
+from blueapps.settings import blueapps_settings
 from blueapps.opentelemetry.export import LazyBatchSpanProcessor
 
 
 def setup_trace_config(
-    service_name: str, bk_data_id: int, otel_sampler: str, otel_grpc_host: str, bk_data_token: str = "",
+    service_name: str,
+    bk_data_id: int,
+    otel_sampler: str,
+    otel_grpc_host: str,
+    bk_data_token: str = "",
 ):
     span_processor = getattr(settings, "BLUEAPPS_BKAPP_OTEL_SPAN_PROCESSOR", LazyBatchSpanProcessor)
+    service_name_handler = blueapps_settings.BKAPP_OTEL_SERVICE_NAME_HANDLER
+    service_name = service_name_handler(service_name).get_service_name()
     if settings.ENVIRONMENT == "dev":
         # local environment, use jaeger as trace service
         # docker run -p 16686:16686 -p 6831:6831/udp jaegertracing/all-in-one
         trace.set_tracer_provider(TracerProvider(resource=Resource.create({SERVICE_NAME: service_name})))
-        jaeger_exporter = JaegerExporter(
-            agent_host_name="localhost", agent_port=6831, udp_split_oversized_batches=True,
-        )
+        jaeger_exporter = JaegerExporter(agent_host_name="localhost", agent_port=6831, udp_split_oversized_batches=True)
         trace.get_tracer_provider().add_span_processor(span_processor(jaeger_exporter))
     else:
         # stage and prod environment, use bk_log as trace service
         trace.set_tracer_provider(
             tracer_provider=TracerProvider(
                 resource=Resource.create(
                     {"service.name": service_name, "bk_data_id": bk_data_id, "bk.data.token": bk_data_token},
@@ -57,47 +61,32 @@
         otlp_exporter = OTLPSpanExporter(endpoint=otel_grpc_host)
         span_processor = span_processor(otlp_exporter)
         trace.get_tracer_provider().add_span_processor(span_processor)
 
 
 def setup_by_settings():
     enable_paas_otel = True if getattr(settings, "OTEL_BK_DATA_TOKEN", "") else False
-    enable_trace = os.getenv("ENABLE_TRACE", enable_paas_otel) or getattr(
-        settings, "ENABLE_OTEL_TRACE", enable_paas_otel
-    )
+    enable_trace = os.getenv("ENABLE_TRACE", enable_paas_otel) or blueapps_settings.ENABLE_OTEL_TRACE
     if enable_trace:
         app_module_name = getattr(settings, "APP_MODULE_NAME", "")
         service_name = (
             os.getenv("BKAPP_OTEL_SERVICE_NAME")
             or getattr(settings, "BKAPP_OTEL_SERVICE_NAME", None)
             or (settings.APP_CODE + f"-{app_module_name}" if app_module_name else "")
         )
-        bk_data_id = int(os.getenv("BKAPP_OTEL_BK_DATA_ID") or getattr(settings, "BKAPP_OTEL_BK_DATA_ID", -1))
-        otel_sampler = (
-            os.getenv("BKAPP_OTEL_SAMPLER")
-            or getattr(settings, "BKAPP_OTEL_SAMPLER", None)
-            or getattr(settings, "OTEL_SAMPLER", None)
-            or "parentbased_always_off"
-        )
-        otel_grpc_host = (
-            os.getenv("BKAPP_OTEL_GRPC_HOST")
-            or getattr(settings, "BKAPP_OTEL_GRPC_HOST", None)
-            or getattr(settings, "OTEL_GRPC_HOST", None)
-        )
-        otel_bk_data_token = (
-            os.getenv("BKAPP_OTEL_BK_DATA_TOKEN")
-            or getattr(settings, "BKAPP_OTEL_BK_DATA_TOKEN", "")
-            or getattr(settings, "OTEL_BK_DATA_TOKEN", "")
-        )
-        setup_trace_config(
-            service_name, bk_data_id, otel_sampler, otel_grpc_host, bk_data_token=otel_bk_data_token,
-        )
+        bk_data_id = int(os.getenv("BKAPP_OTEL_BK_DATA_ID") or blueapps_settings.BKAPP_OTEL_BK_DATA_ID)
+        otel_sampler = os.getenv("BKAPP_OTEL_SAMPLER") or blueapps_settings.BKAPP_OTEL_SAMPLER
+        otel_grpc_host = os.getenv("BKAPP_OTEL_GRPC_HOST") or blueapps_settings.BKAPP_OTEL_GRPC_HOST
+        otel_bk_data_token = os.getenv("BKAPP_OTEL_BK_DATA_TOKEN") or blueapps_settings.BKAPP_OTEL_BK_DATA_TOKEN
+        setup_trace_config(service_name, bk_data_id, otel_sampler, otel_grpc_host, bk_data_token=otel_bk_data_token)
         BKAppInstrumentor().instrument()
         # 将Trace信息配置到项目日志中
-        trace_format = getattr(settings, "OTEL_LOGGING_TRACE_FORMAT", DEFAULT_LOGGING_TRACE_FORMAT)
+        trace_format = blueapps_settings.BKAPP_OTEL_LOGGING_TRACE_FORMAT or getattr(
+            blueapps_settings, "OTEL_LOGGING_TRACE_FORMAT", DEFAULT_LOGGING_TRACE_FORMAT
+        )
         inject_logging_trace_info(settings.LOGGING, ("verbose",), trace_format)
         configure_logging(settings.LOGGING_CONFIG, settings.LOGGING)
     # metrics
-    enable_metrics = os.getenv("ENABLE_METRICS") or getattr(settings, "ENABLE_OTEL_METRICS", False)
+    enable_metrics = os.getenv("ENABLE_METRICS") or blueapps_settings.ENABLE_OTEL_METRICS
     if enable_metrics:
         SaaSMetricsInstrumentor().instrument()
         celery_app.steps["worker"].add(MetricsServerStep)
```

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/README.md` & `blueapps-4.7.0rc0/blueapps/opentelemetry/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/constants.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/constants.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/instrument_app/apps.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/apps.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/instrument_app/__init__.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/opentelemetry/instrument_app/celery.py` & `blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/metrics.py` & `blueapps-4.7.0rc0/blueapps/metrics.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/wsgi.py` & `blueapps-4.7.0rc0/blueapps/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/exceptions/__init__.py` & `blueapps-4.7.0rc0/blueapps/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/exceptions/middleware.py` & `blueapps-4.7.0rc0/blueapps/core/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/__init__.py` & `blueapps-4.7.0rc0/blueapps/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/handler/wsgi.py` & `blueapps-4.7.0rc0/blueapps/core/handler/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/handler/__init__.py` & `blueapps-4.7.0rc0/blueapps/core/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/celery/__init__.py` & `blueapps-4.7.0rc0/blueapps/core/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/celery/celery.py` & `blueapps-4.7.0rc0/blueapps/core/celery/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/sites/__init__.py` & `blueapps-4.7.0rc0/blueapps/core/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/core/sites/middleware.py` & `blueapps-4.7.0rc0/blueapps/core/sites/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/log.py` & `blueapps-4.7.0rc0/blueapps/conf/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/__init__.py` & `blueapps-4.7.0rc0/blueapps/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/database.py` & `blueapps-4.7.0rc0/blueapps/conf/database.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/environ.py` & `blueapps-4.7.0rc0/blueapps/conf/environ.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/validators.py` & `blueapps-4.7.0rc0/blueapps/conf/validators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/default_settings.py` & `blueapps-4.7.0rc0/blueapps/conf/default_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     "whitenoise.middleware.WhiteNoiseMiddleware",
     # Auth middleware
     "blueapps.account.middlewares.RioLoginRequiredMiddleware",
     "blueapps.account.middlewares.WeixinLoginRequiredMiddleware",
     "blueapps.account.middlewares.LoginRequiredMiddleware",
     # exception middleware
     "blueapps.core.exceptions.middleware.AppExceptionMiddleware",
-    # django国际化中间件
     "django.middleware.locale.LocaleMiddleware",
 )
 
 DATABASES = {"default": get_default_database_config_dict(locals())}
 
 # Cache
```

### Comparing `blueapps-4.6.1/blueapps/conf/sites/ieod/__init__.py` & `blueapps-4.7.0rc0/blueapps/conf/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/sites/__init__.py` & `blueapps-4.7.0rc0/blueapps/conf/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/sites/open/__init__.py` & `blueapps-4.7.0rc0/blueapps/conf/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/conf/sites/tencent/__init__.py` & `blueapps-4.7.0rc0/blueapps/conf/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/base.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/base.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/app.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/app.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/__init__.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/handlers/__init__.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/__init__.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/celerybeat.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celerybeat.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/commands/celery.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/management/templates.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/templates.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/__init__.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/bk_commands/test.py` & `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/test.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/contrib/__init__.py` & `blueapps-4.7.0rc0/blueapps/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/dummy/dummy_client.py` & `blueapps-4.7.0rc0/blueapps/contrib/dummy/dummy_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/patch/log.py` & `blueapps-4.7.0rc0/blueapps/patch/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/patch/__init__.py` & `blueapps-4.7.0rc0/blueapps/contrib/drf/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/patch/settings_paas_services.py` & `blueapps-4.7.0rc0/blueapps/patch/settings_paas_services.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/patch/settings_open_saas.py` & `blueapps-4.7.0rc0/blueapps/patch/settings_open_saas.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/decorators.py` & `blueapps-4.7.0rc0/blueapps/account/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/middlewares.py` & `blueapps-4.7.0rc0/blueapps/account/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/management/__init__.py` & `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/management/commands/apigw_clean_cache.py` & `blueapps-4.7.0rc0/blueapps/account/management/commands/apigw_clean_cache.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/management/commands/__init__.py` & `blueapps-4.7.0rc0/blueapps/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/apps.py` & `blueapps-4.7.0rc0/blueapps/account/apps.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/utils/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/utils/http.py` & `blueapps-4.7.0rc0/blueapps/account/utils/http.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/utils/sms.py` & `blueapps-4.7.0rc0/blueapps/account/utils/sms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/handlers/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/handlers/response.py` & `blueapps-4.7.0rc0/blueapps/account/handlers/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-from django.conf import settings
 from django.http import HttpResponseRedirect, JsonResponse
 from django.utils.translation import ugettext_lazy as _
 
 from blueapps.account.utils.http import build_redirect_url
 from blueapps.core.exceptions import BkJwtVerifyError, RioVerifyError
+from blueapps.settings import blueapps_settings
 from blueapps.utils.tools import resolve_login_url
 
 try:
     from django.urls import reverse
 except Exception:  # pylint: disable=broad-except
     from django.core.urlresolvers import reverse
 
@@ -33,15 +33,15 @@
         """
         self._conf = _confFixture
         self._settings = _settings
 
     def build_401_response(self, request):
 
         # 强制要求进行跳转的方式
-        if getattr(settings, "IS_AJAX_PLAIN_MODE", False) and request.is_ajax():
+        if blueapps_settings.IS_AJAX_PLAIN_MODE and request.is_ajax():
             return self._build_ajax_401_response(request)
 
         # Just redirect to PAAS-LOGIN-PLATRORM no matter whether request.is_ajax
         if self._conf.HAS_PLAIN:
             if request.is_ajax():
                 return self._build_ajax_401_response(request)
             else:
@@ -55,16 +55,16 @@
 
     def _build_ajax_401_response(self, request):
         """
         Return 401 info, inlclude login_url to PAAS-LOGIN-PLATFORM,
         width & height for adjusting iframe window, login_url as
         http://xxx/login/?c_url=http%3A//xxx/t/data/&app_id=data
         """
-        if hasattr(settings, "BLUEAPPS_AJAX_401_RESPONSE_FUNC"):
-            return settings.BLUEAPPS_AJAX_401_RESPONSE_FUNC(request)
+        if blueapps_settings.AJAX_401_RESPONSE_FUNC:
+            return blueapps_settings.AJAX_401_RESPONSE_FUNC(request)
         _next = request.build_absolute_uri(reverse("account:login_success"))
 
         if self._conf.ADD_CROSS_PREFIX:
             _next = self._conf.CROSS_PREFIX + _next
 
         _login_url = build_redirect_url(
             _next,
@@ -83,92 +83,82 @@
         return JsonResponse(context, status=401)
 
     def _build_page_401_response(self, request):
         """
         Redirect to login page in self app, redirect url format as
         http://xxx:8000/account/login_page/?refer_url=http%3A//xxx%3A8000/
         """
-        if hasattr(settings, "BLUEAPPS_PAGE_401_RESPONSE_FUNC"):
-            return settings.BLUEAPPS_PAGE_401_RESPONSE_FUNC(request)
+        if blueapps_settings.PAGE_401_RESPONSE_FUNC:
+            return blueapps_settings.PAGE_401_RESPONSE_FUNC(request)
         _next = request.build_absolute_uri()
-        if request.method == "GET" and hasattr(
-            settings, "BLUEAPPS_SPECIFIC_REDIRECT_KEY"
-        ):
-            _next = request.GET.get(settings.BLUEAPPS_SPECIFIC_REDIRECT_KEY) or _next
+        if request.method == "GET" and blueapps_settings.SPECIFIC_REDIRECT_KEY:
+            _next = request.GET.get(blueapps_settings.SPECIFIC_REDIRECT_KEY) or _next
         _redirect = build_redirect_url(
             _next,
             resolve_login_url(self._conf.LOGIN_PLAIN_URL, request),
             self._conf.C_URL,
             extra_args=self._build_extra_args(),
         )
         return HttpResponseRedirect(_redirect)
 
     def _build_page_401_response_platform(self, request):
         """
         Directly redirect to PAAS-LOGIN-PLATFORM
         """
-        if hasattr(settings, "BLUEAPPS_PAGE_401_RESPONSE_PLATFORM_FUNC"):
-            return settings.BLUEAPPS_PAGE_401_RESPONSE_PLATFORM_FUNC(request)
+        if blueapps_settings.PAGE_401_RESPONSE_PLATFORM_FUNC:
+            return blueapps_settings.PAGE_401_RESPONSE_PLATFORM_FUNC(request)
         _next = request.build_absolute_uri()
-        if request.method == "GET" and hasattr(
-            settings, "BLUEAPPS_SPECIFIC_REDIRECT_KEY"
-        ):
-            _next = request.GET.get(settings.BLUEAPPS_SPECIFIC_REDIRECT_KEY) or _next
+        if request.method == "GET" and blueapps_settings.SPECIFIC_REDIRECT_KEY:
+            _next = request.GET.get(blueapps_settings.SPECIFIC_REDIRECT_KEY) or _next
         if self._conf.ADD_CROSS_PREFIX:
             _next = self._conf.CROSS_PREFIX + _next
 
         _login_url = build_redirect_url(
             _next,
             resolve_login_url(self._conf.LOGIN_URL, request),
             self._conf.C_URL,
             extra_args=self._build_extra_args(),
         )
         return HttpResponseRedirect(_login_url)
 
     def _build_extra_args(self):
         extra_args = None
         if self._conf.ADD_APP_CODE:
-            extra_args = {
-                self._conf.APP_KEY: getattr(self._settings, self._conf.SETTINGS_APP_KEY)
-            }
+            extra_args = {self._conf.APP_KEY: getattr(self._settings, self._conf.SETTINGS_APP_KEY)}
         return extra_args
 
     def build_weixin_401_response(self, request):
         """
         todo，说明 url 格式
         """
         _login_url = self._conf.WEIXIN_OAUTH_URL
         _next = request.build_absolute_uri()
-        if request.method == "GET" and hasattr(
-            settings, "BLUEAPPS_SPECIFIC_REDIRECT_KEY"
-        ):
-            _next = request.GET.get(settings.BLUEAPPS_SPECIFIC_REDIRECT_KEY) or _next
+        if request.method == "GET" and blueapps_settings.SPECIFIC_REDIRECT_KEY:
+            _next = request.GET.get(blueapps_settings.SPECIFIC_REDIRECT_KEY) or _next
 
         extra_args = {
             "appid": self._conf.WEIXIN_APP_ID,
             "response_type": "code",
             "scope": "snsapi_base",
             "state": request.session["WEIXIN_OAUTH_STATE"],
         }
-        _redirect = build_redirect_url(
-            _next, _login_url, "redirect_uri", extra_args=extra_args
-        )
+        _redirect = build_redirect_url(_next, _login_url, "redirect_uri", extra_args=extra_args)
         return HttpResponseRedirect(_redirect)
 
     def build_rio_401_response(self, request):
         context = {
             "result": False,
             "code": RioVerifyError.ERROR_CODE,
-            "message": _(u"您的登陆请求无法经智能网关正常检测，请与管理人员联系"),
+            "message": _("您的登陆请求无法经智能网关正常检测，请与管理人员联系"),
         }
         return JsonResponse(context, status=401)
 
     def build_bk_jwt_401_response(self, request):
         """
         BK_JWT鉴权异常
         """
         context = {
             "result": False,
             "code": BkJwtVerifyError.ERROR_CODE,
-            "message": _(u"您的登陆请求无法经BK JWT检测，请与管理人员联系"),
+            "message": _("您的登陆请求无法经BK JWT检测，请与管理人员联系"),
         }
         return JsonResponse(context, status=401)
```

### Comparing `blueapps-4.6.1/blueapps/account/views.py` & `blueapps-4.7.0rc0/blueapps/account/views.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/urls.py` & `blueapps-4.7.0rc0/blueapps/account/urls.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/static/account/login.js` & `blueapps-4.7.0rc0/blueapps/account/static/account/login.js`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_token/middlewares.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_token/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_token/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_token/backends.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_token/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_token/models.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_token/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_token/forms.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_token/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/null/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/null/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_ticket/middlewares.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_ticket/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_ticket/backends.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_ticket/models.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_ticket/forms.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_token/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/weixin/middlewares.py` & `blueapps-4.7.0rc0/blueapps/account/components/weixin/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/weixin/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/weixin/backends.py` & `blueapps-4.7.0rc0/blueapps/account/components/weixin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/weixin/forms.py` & `blueapps-4.7.0rc0/blueapps/account/components/weixin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/rio/middlewares.py` & `blueapps-4.7.0rc0/blueapps/account/components/rio/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/rio/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/rio/backends.py` & `blueapps-4.7.0rc0/blueapps/account/components/rio/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/rio/forms.py` & `blueapps-4.7.0rc0/blueapps/account/components/rio/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_jwt/middlewares.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_jwt/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/weixin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/bk_jwt/backends.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/ptlogin/middlewares.py` & `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/ptlogin/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/ptlogin/backends.py` & `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/ptlogin/models.py` & `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/components/ptlogin/forms.py` & `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/admin.py` & `blueapps-4.7.0rc0/blueapps/account/admin.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/templates/account/login_page.html` & `blueapps-4.7.0rc0/blueapps/account/templates/account/login_page.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/templates/account/login_success.html` & `blueapps-4.7.0rc0/blueapps/account/templates/account/login_success.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/readme.md` & `blueapps-4.7.0rc0/blueapps/account/readme.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/backends.py` & `blueapps-4.7.0rc0/blueapps/account/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/conf.py` & `blueapps-4.7.0rc0/blueapps/account/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 
 from blueapps.account.sites.default import ConfFixture as default_fixture
+from blueapps.settings import blueapps_settings
 
 
 class _ConfFixture:
-    ACCOUNT_CONF_PREFIX = "BLUEAPPS_ACCOUNT"
+    ACCOUNT_CONF_PREFIX = "ACCOUNT"
 
     def __init__(self, fixture_module):
         # store the module
         self._fixture = import_string(fixture_module)
 
     def __getattr__(self, name):
         # settings fixture, 优先返回开发者配置
         account_conf_key = f"{self.ACCOUNT_CONF_PREFIX}_{name}"
-        if hasattr(settings, account_conf_key):
-            return getattr(settings, account_conf_key)
+        if hasattr(blueapps_settings, account_conf_key):
+            return getattr(blueapps_settings, account_conf_key)
 
         # site fixture, 对应环境配置
         if hasattr(self._fixture, name):
             return getattr(self._fixture, name)
 
         # default fixture, 默认配置
         if hasattr(default_fixture, name):
```

### Comparing `blueapps-4.6.1/blueapps/account/models.py` & `blueapps-4.7.0rc0/blueapps/account/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/forms.py` & `blueapps-4.7.0rc0/blueapps/account/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/migrations/0003_verifyinfo.py` & `blueapps-4.7.0rc0/blueapps/account/migrations/0003_verifyinfo.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/migrations/0002_init_superuser.py` & `blueapps-4.7.0rc0/blueapps/account/migrations/0002_init_superuser.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/migrations/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/migrations/0004_create_cache_table.py` & `blueapps-4.7.0rc0/blueapps/account/migrations/0004_create_cache_table.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/migrations/0001_initial.py` & `blueapps-4.7.0rc0/blueapps/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/ieod/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/ieod/conf.py` & `blueapps-4.7.0rc0/blueapps/account/sites/ieod/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/open/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/open/conf.py` & `blueapps-4.7.0rc0/blueapps/account/sites/open/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/default.py` & `blueapps-4.7.0rc0/blueapps/account/sites/default.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/tencent/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/account/sites/tencent/conf.py` & `blueapps-4.7.0rc0/blueapps/account/sites/tencent/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/template/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/template/backends/__init__.py` & `blueapps-4.7.0rc0/blueapps/account/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/template/backends/mako.py` & `blueapps-4.7.0rc0/blueapps/template/backends/mako.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps/template/context_processors.py` & `blueapps-4.7.0rc0/blueapps/template/context_processors.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/blueapps.egg-info/SOURCES.txt` & `blueapps-4.7.0rc0/blueapps.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 test.py
 blueapps/__init__.py
 blueapps/metrics.py
+blueapps/settings.py
 blueapps.egg-info/PKG-INFO
 blueapps.egg-info/SOURCES.txt
 blueapps.egg-info/dependency_links.txt
 blueapps.egg-info/entry_points.txt
 blueapps.egg-info/not-zip-safe
 blueapps.egg-info/requires.txt
 blueapps.egg-info/top_level.txt
@@ -96,27 +97,43 @@
 blueapps/contrib/bk_commands/management/templates.py
 blueapps/contrib/bk_commands/management/commands/__init__.py
 blueapps/contrib/bk_commands/management/commands/celery.py
 blueapps/contrib/bk_commands/management/commands/celerybeat.py
 blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
 blueapps/contrib/bk_commands/management/handlers/__init__.py
 blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
+blueapps/contrib/drf/README.md
+blueapps/contrib/drf/__init__.py
+blueapps/contrib/drf/exception.py
+blueapps/contrib/drf/renderers.py
+blueapps/contrib/drf/serializer.py
+blueapps/contrib/drf/viewsets.py
+blueapps/contrib/drf/swagger/schemas.py
+blueapps/contrib/drf/utils/__init__.py
+blueapps/contrib/drf/utils/authentication.py
+blueapps/contrib/drf/utils/filters.py
+blueapps/contrib/drf/utils/pagination.py
+blueapps/contrib/drf/utils/serializer_fields.py
+blueapps/contrib/drf/utils/serializers.py
+blueapps/contrib/drf/utils/viewset_mixin.py
+blueapps/contrib/dummy/__init__.py
+blueapps/contrib/dummy/dummy_client.py
+blueapps/contrib/test/__init__.py
+blueapps/contrib/test/override_middleware.py
 blueapps/core/__init__.py
 blueapps/core/wsgi.py
 blueapps/core/celery/__init__.py
 blueapps/core/celery/celery.py
 blueapps/core/exceptions/__init__.py
 blueapps/core/exceptions/base.py
 blueapps/core/exceptions/middleware.py
 blueapps/core/handler/__init__.py
 blueapps/core/handler/wsgi.py
 blueapps/core/sites/__init__.py
 blueapps/core/sites/middleware.py
-blueapps/dummy/__init__.py
-blueapps/dummy/dummy_client.py
 blueapps/middleware/__init__.py
 blueapps/middleware/request_provider.py
 blueapps/middleware/bkui/__init__.py
 blueapps/middleware/bkui/middlewares.py
 blueapps/middleware/xss/__init__.py
 blueapps/middleware/xss/decorators.py
 blueapps/middleware/xss/middlewares.py
@@ -145,18 +162,26 @@
 blueapps/patch/settings_open_saas.py
 blueapps/patch/settings_paas_services.py
 blueapps/template/__init__.py
 blueapps/template/context_processors.py
 blueapps/template/backends/__init__.py
 blueapps/template/backends/mako.py
 blueapps/utils/__init__.py
+blueapps/utils/base.py
+blueapps/utils/cache.py
+blueapps/utils/constants.py
+blueapps/utils/db.py
 blueapps/utils/esbclient.py
 blueapps/utils/fancy_dict.py
+blueapps/utils/json.py
 blueapps/utils/jwt_client.py
+blueapps/utils/local.py
+blueapps/utils/lock.py
 blueapps/utils/logger.py
 blueapps/utils/request_provider.py
+blueapps/utils/time.py
 blueapps/utils/tools.py
 blueapps/utils/unique.py
 blueapps/utils/sites/__init__.py
 blueapps/utils/sites/ieod/__init__.py
 blueapps/utils/sites/open/__init__.py
 blueapps/utils/sites/tencent/__init__.py
```

### Comparing `blueapps-4.6.1/blueapps.egg-info/PKG-INFO` & `blueapps-4.7.0rc0/blueapps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.6.1
+Version: 4.7.0rc0
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
```

### Comparing `blueapps-4.6.1/blueapps.egg-info/requires.txt` & `blueapps-4.7.0rc0/blueapps.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 mysqlclient<=2.0.3,>=1.4.4
 bkoauth>=0.0.12
 MarkupSafe<2.0.0,>=1.1.1
 Mako<2.0,>=1.0.6
 requests<3.0.0,>=2.22.0
 python-json-logger>=0.1.7
 whitenoise<=5.2.0,>=3.3.0
+Werkzeug<2.0.0,>=1.0.0
 pyCryptodome>=3.9.7
 PyJWT<2.0,>=1.6.1
 cryptography<3.4,>=2.7
 
 [opentelemetry]
 opentelemetry-api<2.0.0,>=1.6.2
 opentelemetry-sdk<2.0.0,>=1.6.2
```

### Comparing `blueapps-4.6.1/test.py` & `blueapps-4.7.0rc0/test.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/setup.py` & `blueapps-4.7.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         "mysqlclient>=1.4.4,<=2.0.3",
         "bkoauth>=0.0.12",
         "MarkupSafe>=1.1.1,<2.0.0",
         "Mako>=1.0.6,<2.0",
         "requests>=2.22.0,<3.0.0",
         "python-json-logger>=0.1.7",
         "whitenoise>=3.3.0,<=5.2.0",
+        "Werkzeug>=1.0.0,<2.0.0",
         # jwt
         "pyCryptodome>=3.9.7",
         "PyJWT>=1.6.1,<2.0",
         "cryptography>=2.7,<3.4",
     ],
     extras_require={
         "opentelemetry": [
@@ -83,11 +84,9 @@
             "django-prometheus>=2.1.0,<3.0.0",
         ]
     },
     zip_safe=False,
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
-    entry_points={
-        "console_scripts": ["bk-admin=blueapps.contrib.bk_commands:bk_admin"],
-    },
+    entry_points={"console_scripts": ["bk-admin=blueapps.contrib.bk_commands:bk_admin"],},
 )
```

### Comparing `blueapps-4.6.1/README.md` & `blueapps-4.7.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.6.1/PKG-INFO` & `blueapps-4.7.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.6.1
+Version: 4.7.0rc0
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
```

### Comparing `blueapps-4.6.1/LICENSE.txt` & `blueapps-4.7.0rc0/LICENSE.txt`

 * *Files identical despite different names*

