# Comparing `tmp/meerschaum-1.6.3.tar.gz` & `tmp/meerschaum-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-1.6.3.tar", last modified: Tue Mar 28 22:16:06 2023, max compression
+gzip compressed data, was "meerschaum-1.6.4.tar", last modified: Wed Apr 26 08:13:08 2023, max compression
```

## Comparing `meerschaum-1.6.3.tar` & `meerschaum-1.6.4.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.400127 meerschaum-1.6.3/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.6.3/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.6.3/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-03-28 22:16:06.399127 meerschaum-1.6.3/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.6.3/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.348128 meerschaum-1.6.3/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.6.3/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.350128 meerschaum-1.6.3/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.6.3/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.351128 meerschaum-1.6.3/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.6.3/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12624 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.352128 meerschaum-1.6.3/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.352128 meerschaum-1.6.3/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.353128 meerschaum-1.6.3/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.6.3/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.354128 meerschaum-1.6.3/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.6.3/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.6.3/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.354128 meerschaum-1.6.3/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.355128 meerschaum-1.6.3/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.6.3/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.6.3/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      788 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.361128 meerschaum-1.6.3/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8129 2022-10-26 04:20:20.000000 meerschaum-1.6.3/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10996 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.6.3/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6095 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.6.3/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-03-18 14:36:27.000000 meerschaum-1.6.3/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.6.3/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.6.3/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-03-18 14:36:27.000000 meerschaum-1.6.3/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.6.3/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.6.3/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5501 2022-10-25 06:38:00.000000 meerschaum-1.6.3/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.6.3/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.6.3/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.6.3/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.6.3/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.6.3/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.6.3/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.363128 meerschaum-1.6.3/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7638 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      966 2022-08-19 04:59:44.000000 meerschaum-1.6.3/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-08-19 04:59:44.000000 meerschaum-1.6.3/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.6.3/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.365128 meerschaum-1.6.3/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.6.3/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.6.3/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.367128 meerschaum-1.6.3/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.369128 meerschaum-1.6.3/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24874 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.6.3/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-03-18 14:36:27.000000 meerschaum-1.6.3/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6771 2022-10-31 13:18:31.000000 meerschaum-1.6.3/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.6.3/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.370128 meerschaum-1.6.3/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.6.3/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1425 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.6.3/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      886 2022-07-26 06:45:25.000000 meerschaum-1.6.3/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.6.3/meerschaum/api/dash/websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.371127 meerschaum-1.6.3/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.6.3/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.371127 meerschaum-1.6.3/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.371127 meerschaum-1.6.3/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.373128 meerschaum-1.6.3/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1592 2022-10-31 13:18:31.000000 meerschaum-1.6.3/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/css/styles.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.373128 meerschaum-1.6.3/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.374127 meerschaum-1.6.3/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/js/main.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.374127 meerschaum-1.6.3/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.375127 meerschaum-1.6.3/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.6.3/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.377127 meerschaum-1.6.3/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.6.3/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.6.3/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1702 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.6.3/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7239 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.6.3/meerschaum/api/routes/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.378127 meerschaum-1.6.3/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.380127 meerschaum-1.6.3/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.6.3/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5136 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.6.3/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.6.3/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.6.3/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.6.3/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.6.3/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.6.3/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2023-03-28 22:14:35.000000 meerschaum-1.6.3/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.381127 meerschaum-1.6.3/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.381127 meerschaum-1.6.3/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8233 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.381127 meerschaum-1.6.3/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.6.3/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.381127 meerschaum-1.6.3/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.382127 meerschaum-1.6.3/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.382127 meerschaum-1.6.3/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.382127 meerschaum-1.6.3/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3679 2023-03-18 14:36:27.000000 meerschaum-1.6.3/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.383127 meerschaum-1.6.3/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.386127 meerschaum-1.6.3/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4022 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.6.3/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/connectors/api/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.6.3/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/connectors/api/_get.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.6.3/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.6.3/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/connectors/api/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19816 2023-01-21 08:00:50.000000 meerschaum-1.6.3/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.6.3/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/connectors/api/_post.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.6.3/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.6.3/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.6.3/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.387127 meerschaum-1.6.3/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.6.3/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.389127 meerschaum-1.6.3/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8592 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-03-13 05:09:43.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11523 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    85618 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7921 2023-03-18 14:36:27.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24326 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9972 2023-03-18 14:36:27.000000 meerschaum-1.6.3/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.390127 meerschaum-1.6.3/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6482 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.390127 meerschaum-1.6.3/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.392127 meerschaum-1.6.3/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14954 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13019 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-03-20 03:20:55.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6847 2022-11-13 04:57:20.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6787 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2585 2022-10-25 06:38:00.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-03-20 03:20:55.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21901 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/core/Pipe/_sync.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.392127 meerschaum-1.6.3/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.393127 meerschaum-1.6.3/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.6.3/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.393127 meerschaum-1.6.3/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.6.3/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.396127 meerschaum-1.6.3/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.6.3/meerschaum/utils/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.396127 meerschaum-1.6.3/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24801 2023-03-28 22:14:35.000000 meerschaum-1.6.3/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.6.3/meerschaum/utils/daemon/Log.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.6.3/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.397127 meerschaum-1.6.3/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.6.3/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.6.3/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.6.3/meerschaum/utils/get_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.6.3/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    54184 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.6.3/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.398127 meerschaum-1.6.3/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    54888 2023-03-20 03:20:55.000000 meerschaum-1.6.3/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7992 2023-03-20 03:20:55.000000 meerschaum-1.6.3/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.6.3/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.6.3/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.6.3/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1635 2022-08-29 21:54:10.000000 meerschaum-1.6.3/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34619 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.6.3/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2498 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.398127 meerschaum-1.6.3/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.6.3/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-03-11 03:05:29.000000 meerschaum-1.6.3/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6610 2023-03-13 05:09:44.000000 meerschaum-1.6.3/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.6.3/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-03-28 22:16:06.350128 meerschaum-1.6.3/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-03-28 22:16:06.000000 meerschaum-1.6.3/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7834 2023-03-28 22:16:06.000000 meerschaum-1.6.3/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-03-28 22:16:06.000000 meerschaum-1.6.3/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-03-28 22:16:06.000000 meerschaum-1.6.3/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4683 2023-03-28 22:16:06.000000 meerschaum-1.6.3/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-03-28 22:16:06.000000 meerschaum-1.6.3/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-03-28 22:16:06.000000 meerschaum-1.6.3/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-03-28 22:16:06.400127 meerschaum-1.6.3/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-03-13 05:09:44.000000 meerschaum-1.6.3/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.519732 meerschaum-1.6.4/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.6.4/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.6.4/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-04-26 08:13:08.519732 meerschaum-1.6.4/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.6.4/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.504732 meerschaum-1.6.4/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.6.4/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.505732 meerschaum-1.6.4/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.6.4/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.505732 meerschaum-1.6.4/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.6.4/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12624 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.505732 meerschaum-1.6.4/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.505732 meerschaum-1.6.4/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.505732 meerschaum-1.6.4/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.6.4/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.506733 meerschaum-1.6.4/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.6.4/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.6.4/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.506733 meerschaum-1.6.4/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.506733 meerschaum-1.6.4/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.6.4/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.6.4/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      788 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.507732 meerschaum-1.6.4/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8129 2022-10-26 04:20:20.000000 meerschaum-1.6.4/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10996 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.6.4/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6095 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.6.4/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.6.4/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.6.4/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.6.4/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.6.4/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5501 2022-10-25 06:38:00.000000 meerschaum-1.6.4/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.6.4/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.6.4/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.6.4/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.6.4/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.6.4/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.6.4/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.508732 meerschaum-1.6.4/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7638 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      966 2022-08-19 04:59:44.000000 meerschaum-1.6.4/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-08-19 04:59:44.000000 meerschaum-1.6.4/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.6.4/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.509733 meerschaum-1.6.4/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.6.4/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.6.4/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.509733 meerschaum-1.6.4/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.510733 meerschaum-1.6.4/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24874 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.6.4/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6771 2022-10-31 13:18:31.000000 meerschaum-1.6.4/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.6.4/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.510733 meerschaum-1.6.4/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.6.4/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1425 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.6.4/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      886 2022-07-26 06:45:25.000000 meerschaum-1.6.4/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.6.4/meerschaum/api/dash/websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.510733 meerschaum-1.6.4/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.6.4/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.510733 meerschaum-1.6.4/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.510733 meerschaum-1.6.4/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.511732 meerschaum-1.6.4/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1592 2022-10-31 13:18:31.000000 meerschaum-1.6.4/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/css/styles.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.511732 meerschaum-1.6.4/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.511732 meerschaum-1.6.4/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/js/main.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.511732 meerschaum-1.6.4/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.511732 meerschaum-1.6.4/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.6.4/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.512732 meerschaum-1.6.4/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.6.4/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.6.4/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1702 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.6.4/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7239 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.6.4/meerschaum/api/routes/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.512732 meerschaum-1.6.4/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.6.4/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5136 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.6.4/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.6.4/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.6.4/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.6.4/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.6.4/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.6.4/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8233 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.6.4/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.513733 meerschaum-1.6.4/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3679 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.514732 meerschaum-1.6.4/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.514732 meerschaum-1.6.4/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4022 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.6.4/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/connectors/api/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.6.4/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/connectors/api/_get.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.6.4/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.6.4/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/connectors/api/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.6.4/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/connectors/api/_post.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.6.4/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.6.4/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.6.4/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.514732 meerschaum-1.6.4/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.6.4/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.515732 meerschaum-1.6.4/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8592 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11725 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    87902 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7921 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24328 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9972 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.515732 meerschaum-1.6.4/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6482 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.515732 meerschaum-1.6.4/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.516732 meerschaum-1.6.4/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14954 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6847 2022-11-13 04:57:20.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2585 2022-10-25 06:38:00.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22138 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/core/Pipe/_sync.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.516732 meerschaum-1.6.4/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.516732 meerschaum-1.6.4/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.6.4/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.516732 meerschaum-1.6.4/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.6.4/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.517732 meerschaum-1.6.4/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.6.4/meerschaum/utils/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.518732 meerschaum-1.6.4/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24801 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.6.4/meerschaum/utils/daemon/Log.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.6.4/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.518732 meerschaum-1.6.4/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.6.4/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.6.4/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.6.4/meerschaum/utils/get_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.6.4/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    59942 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.6.4/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.518732 meerschaum-1.6.4/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8054 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.6.4/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.6.4/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.6.4/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1635 2022-08-29 21:54:10.000000 meerschaum-1.6.4/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34619 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.6.4/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2498 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.518732 meerschaum-1.6.4/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.6.4/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.6.4/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6610 2023-04-25 23:57:31.000000 meerschaum-1.6.4/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.6.4/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-04-26 08:13:08.505732 meerschaum-1.6.4/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-04-26 08:13:08.000000 meerschaum-1.6.4/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7834 2023-04-26 08:13:08.000000 meerschaum-1.6.4/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-04-26 08:13:08.000000 meerschaum-1.6.4/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-04-26 08:13:08.000000 meerschaum-1.6.4/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4703 2023-04-26 08:13:08.000000 meerschaum-1.6.4/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-04-26 08:13:08.000000 meerschaum-1.6.4/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-04-26 08:13:08.000000 meerschaum-1.6.4/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-04-26 08:13:08.519732 meerschaum-1.6.4/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-04-26 08:12:55.000000 meerschaum-1.6.4/setup.py
```

### Comparing `meerschaum-1.6.3/LICENSE` & `meerschaum-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/PKG-INFO` & `meerschaum-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.3
+Version: 1.6.4
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.3/README.md` & `meerschaum-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/__init__.py` & `meerschaum-1.6.4/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/__main__.py` & `meerschaum-1.6.4/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/arguments/__init__.py` & `meerschaum-1.6.4/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-1.6.4/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/arguments/_parser.py` & `meerschaum-1.6.4/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/docs/index.py` & `meerschaum-1.6.4/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/entry.py` & `meerschaum-1.6.4/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/gui/__init__.py` & `meerschaum-1.6.4/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-1.6.4/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-1.6.4/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/gui/app/actions.py` & `meerschaum-1.6.4/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-1.6.4/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/shell/Shell.py` & `meerschaum-1.6.4/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-1.6.4/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-1.6.4/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-1.6.4/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/term/__init__.py` & `meerschaum-1.6.4/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/_internal/term/tools.py` & `meerschaum-1.6.4/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/__init__.py` & `meerschaum-1.6.4/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/api.py` & `meerschaum-1.6.4/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/bootstrap.py` & `meerschaum-1.6.4/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/clear.py` & `meerschaum-1.6.4/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/copy.py` & `meerschaum-1.6.4/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/delete.py` & `meerschaum-1.6.4/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/drop.py` & `meerschaum-1.6.4/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/edit.py` & `meerschaum-1.6.4/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/install.py` & `meerschaum-1.6.4/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/login.py` & `meerschaum-1.6.4/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/os.py` & `meerschaum-1.6.4/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/python.py` & `meerschaum-1.6.4/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/register.py` & `meerschaum-1.6.4/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/reload.py` & `meerschaum-1.6.4/meerschaum/actions/reload.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/setup.py` & `meerschaum-1.6.4/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/sh.py` & `meerschaum-1.6.4/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/show.py` & `meerschaum-1.6.4/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/sql.py` & `meerschaum-1.6.4/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/stack.py` & `meerschaum-1.6.4/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/start.py` & `meerschaum-1.6.4/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/stop.py` & `meerschaum-1.6.4/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/sync.py` & `meerschaum-1.6.4/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/uninstall.py` & `meerschaum-1.6.4/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/upgrade.py` & `meerschaum-1.6.4/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/actions/verify.py` & `meerschaum-1.6.4/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/__init__.py` & `meerschaum-1.6.4/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/_chain.py` & `meerschaum-1.6.4/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/_events.py` & `meerschaum-1.6.4/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/_oauth2.py` & `meerschaum-1.6.4/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/_websockets.py` & `meerschaum-1.6.4/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/__init__.py` & `meerschaum-1.6.4/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/actions.py` & `meerschaum-1.6.4/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-1.6.4/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-1.6.4/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-1.6.4/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-1.6.4/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-1.6.4/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-1.6.4/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/callbacks/login.py` & `meerschaum-1.6.4/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-1.6.4/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/callbacks/register.py` & `meerschaum-1.6.4/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/components.py` & `meerschaum-1.6.4/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/connectors.py` & `meerschaum-1.6.4/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/graphs.py` & `meerschaum-1.6.4/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/jobs.py` & `meerschaum-1.6.4/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/keys.py` & `meerschaum-1.6.4/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-1.6.4/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/pages/error.py` & `meerschaum-1.6.4/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/pages/login.py` & `meerschaum-1.6.4/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/pages/plugins.py` & `meerschaum-1.6.4/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/pages/register.py` & `meerschaum-1.6.4/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/pipes.py` & `meerschaum-1.6.4/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/plugins.py` & `meerschaum-1.6.4/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/users.py` & `meerschaum-1.6.4/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/dash/websockets.py` & `meerschaum-1.6.4/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-1.6.4/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/static/css/dash.css` & `meerschaum-1.6.4/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-1.6.4/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-1.6.4/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-1.6.4/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/templates/index.html` & `meerschaum-1.6.4/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/templates/old_index.html` & `meerschaum-1.6.4/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/resources/templates/termpage.html` & `meerschaum-1.6.4/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/__init__.py` & `meerschaum-1.6.4/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_actions.py` & `meerschaum-1.6.4/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_connectors.py` & `meerschaum-1.6.4/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_index.py` & `meerschaum-1.6.4/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_login.py` & `meerschaum-1.6.4/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_misc.py` & `meerschaum-1.6.4/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_pipes.py` & `meerschaum-1.6.4/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_plugins.py` & `meerschaum-1.6.4/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_users.py` & `meerschaum-1.6.4/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/routes/_version.py` & `meerschaum-1.6.4/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/api/tables/__init__.py` & `meerschaum-1.6.4/meerschaum/api/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/__init__.py` & `meerschaum-1.6.4/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_default.py` & `meerschaum-1.6.4/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_edit.py` & `meerschaum-1.6.4/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_environment.py` & `meerschaum-1.6.4/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_formatting.py` & `meerschaum-1.6.4/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_jobs.py` & `meerschaum-1.6.4/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_patch.py` & `meerschaum-1.6.4/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_paths.py` & `meerschaum-1.6.4/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_preprocess.py` & `meerschaum-1.6.4/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_read_config.py` & `meerschaum-1.6.4/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_shell.py` & `meerschaum-1.6.4/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/_sync.py` & `meerschaum-1.6.4/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/stack/__init__.py` & `meerschaum-1.6.4/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-1.6.4/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/config/static/__init__.py` & `meerschaum-1.6.4/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/Connector.py` & `meerschaum-1.6.4/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/__init__.py` & `meerschaum-1.6.4/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/APIConnector.py` & `meerschaum-1.6.4/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_actions.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_delete.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_fetch.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_get.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_get.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_login.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_misc.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_patch.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_pipes.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_pipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,23 @@
     from meerschaum.utils.misc import parse_df_datetimes
     pd = import_pandas()
     try:
         df = pd.read_json(response.text)
     except Exception as e:
         warn(str(e))
         return None
-    df = parse_df_datetimes(df, debug=debug)
+    df = parse_df_datetimes(
+        df,
+        ignore_cols = [
+            col
+            for col, dtype in pipe.dtypes.items()
+            if 'datetime' not in str(dtype)
+        ],
+        debug = debug,
+    )
     return df
 
 
 def get_backtrack_data(
         self,
         pipe: meerschaum.Pipe,
         begin: datetime.datetime,
```

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_plugins.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_post.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_post.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_uri.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/api/_users.py` & `meerschaum-1.6.4/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/parse.py` & `meerschaum-1.6.4/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-1.6.4/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/poll.py` & `meerschaum-1.6.4/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_cli.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_fetch.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,23 @@
         debug = debug,
         **kw
     )
     df = self.read(meta_def, chunk_hook=chunk_hook, chunksize=chunksize, debug=debug)
     ### if sqlite, parse for datetimes
     if self.flavor == 'sqlite':
         from meerschaum.utils.misc import parse_df_datetimes
-        df = parse_df_datetimes(df, debug=debug)
+        df = parse_df_datetimes(
+            df,
+            ignore_cols = [
+                col
+                for col, dtype in pipe.dtypes.items()
+                if 'datetime' not in str(dtype)
+            ],
+            debug = debug,
+        )
     return df
 
 
 def get_pipe_metadef(
         self,
         pipe: meerschaum.Pipe,
         params: Optional[Dict[str, Any]] = None,
```

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_pipes.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_pipes.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,17 +729,38 @@
         debug = debug,
         **kw
     )
     if self.flavor == 'sqlite':
         from meerschaum.utils.misc import parse_df_datetimes
         from meerschaum.utils.packages import import_pandas
         pd = import_pandas()
-        ### NOTE: We have to consume the iterator here to ensure that datatimes are parsed correctly
-        df = parse_df_datetimes(df, debug=debug) if isinstance(df, pd.DataFrame) else (
-            [parse_df_datetimes(c, debug=debug) for c in df]
+        ### NOTE: We have to consume the iterator here to ensure that datetimes are parsed correctly
+        df = (
+            parse_df_datetimes(
+                df,
+                ignore_cols = [
+                    col
+                    for col, dtype in pipe.dtypes.items()
+                    if 'datetime' not in str(dtype)
+                ],
+                debug = debug,
+            ) if isinstance(df, pd.DataFrame) else (
+                [
+                    parse_df_datetimes(
+                        c,
+                        ignore_cols = [
+                            col
+                            for col, dtype in pipe.dtypes.items()
+                            if 'datetime' not in str(dtype)
+                        ],
+                        debug = debug,
+                    )
+                    for c in df
+                ]
+            )
         )
         for col, typ in dtypes.items():
             if typ != 'json':
                 continue
             df[col] = df[col].apply(lambda x: json.loads(x) if x is not None else x)
     return df
 
@@ -1109,15 +1130,16 @@
             if not self.exec_queries(add_cols_queries, debug=debug):
                 warn(f"Failed to add new columns to {pipe}.")
 
         alter_cols_queries = self.get_alter_columns_queries(pipe, df, debug=debug)
         if alter_cols_queries:
             if not self.exec_queries(alter_cols_queries, debug=debug):
                 warn(f"Failed to alter columns for {pipe}.")
-
+            else:
+                pipe.infer_dtypes(persist=True)
 
     unseen_df, update_df, delta_df = (
         pipe.filter_existing(
             df,
             chunksize = chunksize,
             begin = begin,
             end = end,
@@ -1369,14 +1391,16 @@
         if not self.exec_queries(add_cols_queries, debug=debug):
             warn(f"Failed to add new columns to {pipe}.")
 
     alter_cols_queries = self.get_alter_columns_queries(pipe, new_cols, debug=debug)
     if alter_cols_queries:
         if not self.exec_queries(alter_cols_queries, debug=debug):
             warn(f"Failed to alter columns for {pipe}.")
+        else:
+            pipe.infer_dtypes(persist=True)
 
     if not check_existing:
         new_count = self.value(f"SELECT COUNT(*) FROM {new_table_name}", debug=debug)
         insert_queries = [
             (
                 f"INSERT INTO {pipe_name}\n"
                 + f"SELECT *\nFROM {new_table_name}"
@@ -2381,21 +2405,21 @@
         The pandas DataFrame which may contain altered columns.
         If a dict is provided, assume it maps columns to Pandas data types.
 
     Returns
     -------
     A list of the `ALTER TABLE` SQL query or queries to be executed on the provided connector.
     """
-    if self.flavor == 'sqlite':
-        return []
     if not pipe.exists(debug=debug):
         return []
     from meerschaum.utils.sql import get_pd_type, get_db_type, sql_item_name
-    from meerschaum.utils.misc import flatten_list
+    from meerschaum.utils.misc import flatten_list, generate_password
     table_obj = self.get_pipe_table(pipe, debug=debug)
+    target = pipe.target
+    session_id = generate_password(3)
     df_cols_types = (
         {col: str(typ) for col, typ in df.dtypes.items()}
         if not isinstance(df, dict) else df
     )
     db_cols_types = {col: get_pd_type(str(typ.type)) for col, typ in table_obj.columns.items()}
     altered_cols = [
         col for col, typ in df_cols_types.items()
@@ -2407,70 +2431,114 @@
 
     text_type = get_db_type('str', self.flavor)
     altered_cols_types = {
         col: text_type
         for col in altered_cols
     }
 
+    if self.flavor == 'sqlite':
+        temp_table_name = '_' + session_id + '_' + target
+        rename_query = (
+            "ALTER TABLE "
+            + sql_item_name(target, self.flavor)
+            + " RENAME TO "
+            + sql_item_name(temp_table_name, self.flavor)
+        )
+        create_query = (
+            "CREATE TABLE "
+            + sql_item_name(target, self.flavor)
+            + " (\n"
+        )
+        for col_name, col_obj in table_obj.columns.items():
+            create_query += (
+                sql_item_name(col_name, self.flavor)
+                + " "
+                + (str(col_obj.type) if col_name not in altered_cols else text_type)
+                + ",\n"
+            )
+        create_query = create_query[:-2] + "\n)"
+
+        insert_query = (
+            "INSERT INTO "
+            + sql_item_name(target, self.flavor)
+            + "\nSELECT\n"
+        )
+        for col_name, col_obj in table_obj.columns.items():
+            new_col_str = (
+                sql_item_name(col_name, self.flavor)
+                if col_name not in altered_cols
+                else f"CAST({sql_item_name(col_name, self.flavor)} AS {text_type})"
+            )
+            insert_query += new_col_str + ",\n"
+        insert_query = insert_query[:-2] + f"\nFROM {sql_item_name(temp_table_name, self.flavor)}"
+
+        drop_query = f"DROP TABLE {sql_item_name(temp_table_name, self.flavor)}"
+        return [
+            rename_query,
+            create_query,
+            insert_query,
+            drop_query,
+        ]
+
     queries = []
     if self.flavor == 'oracle':
-        add_query = "ALTER TABLE " + sql_item_name(pipe.target, self.flavor)
+        add_query = "ALTER TABLE " + sql_item_name(target, self.flavor)
         for col, typ in altered_cols_types.items():
             add_query += "\nADD " + sql_item_name(col + '_temp', self.flavor) + " " + typ + ","
         add_query = add_query[:-1]
         queries.append(add_query)
 
-        populate_temp_query = "UPDATE " + sql_item_name(pipe.target, self.flavor)
+        populate_temp_query = "UPDATE " + sql_item_name(target, self.flavor)
         for col, typ in altered_cols_types.items():
             populate_temp_query += (
                 "\nSET " + sql_item_name(col + '_temp', self.flavor)
                 + ' = ' + sql_item_name(col, self.flavor) + ','
             )
         populate_temp_query = populate_temp_query[:-1]
         queries.append(populate_temp_query)
 
-        set_old_cols_to_null_query = "UPDATE " + sql_item_name(pipe.target, self.flavor)
+        set_old_cols_to_null_query = "UPDATE " + sql_item_name(target, self.flavor)
         for col, typ in altered_cols_types.items():
             set_old_cols_to_null_query += (
                 "\nSET " + sql_item_name(col, self.flavor)
                 + ' = NULL,'
             )
         set_old_cols_to_null_query = set_old_cols_to_null_query[:-1]
         queries.append(set_old_cols_to_null_query)
 
-        alter_type_query = "ALTER TABLE " + sql_item_name(pipe.target, self.flavor)
+        alter_type_query = "ALTER TABLE " + sql_item_name(target, self.flavor)
         for col, typ in altered_cols_types.items():
             alter_type_query += (
                 "\nMODIFY " + sql_item_name(col, self.flavor) + ' '
                 + typ + ','
             )
         alter_type_query = alter_type_query[:-1]
         queries.append(alter_type_query)
 
-        set_old_to_temp_query = "UPDATE " + sql_item_name(pipe.target, self.flavor)
+        set_old_to_temp_query = "UPDATE " + sql_item_name(target, self.flavor)
         for col, typ in altered_cols_types.items():
             set_old_to_temp_query += (
                 "\nSET " + sql_item_name(col, self.flavor)
                 + ' = ' + sql_item_name(col + '_temp', self.flavor) + ','
             )
         set_old_to_temp_query = set_old_to_temp_query[:-1]
         queries.append(set_old_to_temp_query)
 
-        drop_temp_query = "ALTER TABLE " + sql_item_name(pipe.target, self.flavor)
+        drop_temp_query = "ALTER TABLE " + sql_item_name(target, self.flavor)
         for col, typ in altered_cols_types.items():
             drop_temp_query += (
                 "\nDROP COLUMN " + sql_item_name(col + '_temp', self.flavor) + ','
             )
         drop_temp_query = drop_temp_query[:-1]
         queries.append(drop_temp_query)
 
         return queries
 
 
-    query = "ALTER TABLE " + sql_item_name(pipe.target, self.flavor)
+    query = "ALTER TABLE " + sql_item_name(target, self.flavor)
     for col, typ in altered_cols_types.items():
         alter_col_prefix = (
             'ALTER' if self.flavor not in ('mysql', 'mariadb', 'oracle')
             else 'MODIFY'
         )
         type_prefix = (
             '' if self.flavor in ('mssql', 'mariadb', 'mysql')
```

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_plugins.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_sql.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,19 +609,18 @@
 
         to_sql_kw['dtype'] = dtype
 
     ### Check for JSON columns.
     if self.flavor not in json_flavors:
         json_cols = get_json_cols(df)
         if json_cols:
-            df = df.copy()
             for col in json_cols:
                 df[col] = df[col].apply(
                     (
-                        lambda x: json.dumps(x)
+                        lambda x: json.dumps(x, default=str, sort_keys=True)
                         if not isinstance(x, Hashable)
                         else x
                     )
                 )
 
     ### Check if the name is too long.
     truncated_name = truncate_item_name(name, self.flavor)
```

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_uri.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/_users.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/connectors/sql/tables/types.py` & `meerschaum-1.6.4/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/__init__.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_attributes.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,14 +412,21 @@
     self.parameters['target'] = _target
 
 
 def guess_datetime(self) -> Union[str, None]:
     """
     Try to determine a pipe's datetime column.
     """
+    dtypes = self.dtypes
+
+    ### Abort if the user explictly disallows a datetime index.
+    if 'datetime' in dtypes:
+        if dtypes['datetime'] is None:
+            return None
+
     dt_cols = [
         col for col, typ in self.dtypes.items()
         if str(typ).startswith('datetime')
     ]
     if not dt_cols:
         return None
     return dt_cols[0]
```

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_clear.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_data.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_delete.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_drop.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_edit.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_fetch.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_register.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_show.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/core/Pipe/_sync.py` & `meerschaum-1.6.4/meerschaum/core/Pipe/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -480,20 +480,22 @@
         df = self.enforce_dtypes(df, debug=debug)
 
     if df.empty:
         return df, df, df
 
     ### begin is the oldest data in the new dataframe
     dt_col = self.columns.get('datetime', None)
+    if dt_col is None and begin:
+        dt_col = self.guess_datetime()
     dt_type = self.dtypes.get(dt_col, 'datetime64[ns]') if dt_col else None
     try:
         min_dt_val = df[dt_col].min(skipna=True) if dt_col else None
         min_dt = (
             pd.to_datetime(min_dt_val).to_pydatetime()
-            if 'datetime' in dt_type
+            if min_dt_val is not None and 'datetime' in str(dt_type)
             else min_dt_val
         )
     except Exception as e:
         min_dt = None
     if not ('datetime' in str(type(min_dt))) or str(min_dt) == 'NaT':
         if 'int' not in str(type(min_dt)).lower():
             min_dt = None
@@ -503,24 +505,28 @@
             round_time(
                 min_dt,
                 to = 'down'
             ) - datetime.timedelta(minutes=1)
         )
     elif dt_type and 'int' in dt_type.lower():
         begin = min_dt
+    elif dt_col is None:
+        begin = None
 
     ### end is the newest data in the new dataframe
     try:
         max_dt_val = df[dt_col].max(skipna=True) if dt_col else None
         max_dt = (
             pd.to_datetime(max_dt_val).to_pydatetime()
-            if 'datetime' in dt_type
+            if max_dt_val is not None and 'datetime' in str(dt_type)
             else max_dt_val
         )
     except Exception as e:
+        import traceback
+        traceback.print_exc()
         max_dt = None
 
     if not ('datetime' in str(type(max_dt))) or str(min_dt) == 'NaT':
         if 'int' not in str(type(max_dt)).lower():
             max_dt = None
 
     if end is None:
```

### Comparing `meerschaum-1.6.3/meerschaum/core/User/_User.py` & `meerschaum-1.6.4/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/plugins/_Plugin.py` & `meerschaum-1.6.4/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/plugins/__init__.py` & `meerschaum-1.6.4/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/daemon/Daemon.py` & `meerschaum-1.6.4/meerschaum/utils/daemon/Daemon.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/daemon/Log.py` & `meerschaum-1.6.4/meerschaum/utils/daemon/Log.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/daemon/__init__.py` & `meerschaum-1.6.4/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/daemon/_names.py` & `meerschaum-1.6.4/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/debug.py` & `meerschaum-1.6.4/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/formatting/__init__.py` & `meerschaum-1.6.4/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/formatting/_jobs.py` & `meerschaum-1.6.4/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/formatting/_pipes.py` & `meerschaum-1.6.4/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/formatting/_pprint.py` & `meerschaum-1.6.4/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/formatting/_shell.py` & `meerschaum-1.6.4/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/get_pipes.py` & `meerschaum-1.6.4/meerschaum/utils/get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/interactive.py` & `meerschaum-1.6.4/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/misc.py` & `meerschaum-1.6.4/meerschaum/utils/misc.py`

 * *Files 23% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     """
     from functools import wraps
 
     is_class = isinstance(class_def, type)
     
     @wraps(func)
     def wrapper(self, *args, **kw):
-        print(self, args, kw)
         return func(*args, **kw)
 
     if method_name is None:
         method_name = func.__name__
 
     setattr(class_def, method_name, (
             wrapper if ((is_class and keep_self is None) or keep_self is False) else func
@@ -651,30 +650,35 @@
             rounding = (seconds + round_to / 2) // round_to * round_to
 
     return dt + datetime.timedelta(0, rounding - seconds, - dt.microsecond)
 
 
 def parse_df_datetimes(
         df: 'pd.DataFrame',
-        debug: bool = False
+        ignore_cols: Optional[Iterable[str]] = None,
+        debug: bool = False,
     ) -> 'pd.DataFrame':
     """
     Parse a pandas DataFrame for datetime columns and cast as datetimes.
 
     Parameters
     ----------
     df: pd.DataFrame
         The pandas DataFrame to parse.
+
+    ignore_cols: Optional[Iterable[str]], default None
+        If provided, do not attempt to coerce these columns as datetimes.
         
     debug: bool, default False
         Verbosity toggle.
 
     Returns
     -------
-    A new pandas DataFrame with the determined datetime columns (usually ISO strings) cast as datetimes.
+    A new pandas DataFrame with the determined datetime columns
+    (usually ISO strings) cast as datetimes.
 
     Examples
     --------
     ```python
     >>> import pandas as pd
     >>> df = pd.DataFrame({'a': ['2022-01-01 00:00:00']}) 
     >>> df.dtypes
@@ -685,50 +689,72 @@
     a    datetime64[ns]
     dtype: object
 
     ```
 
     """
     from meerschaum.utils.packages import import_pandas
-    ### import pandas (or pandas replacement)
     from meerschaum.utils.debug import dprint
+    from meerschaum.utils.warnings import warn
+    import traceback
     pd = import_pandas()
 
     ### if df is a dict, build DataFrame
     if not isinstance(df, pd.DataFrame):
         if debug:
             dprint(f"df is not a DataFrame. Casting to DataFrame...")
         df = pd.DataFrame(df)
 
     ### skip parsing if DataFrame is empty
     if len(df) == 0:
         if debug:
             dprint(f"df is empty. Returning original DataFrame without casting datetime columns...")
         return df
 
+    ignore_cols = ignore_cols or []
+    cols_to_inspect = [col for col in df.columns if col not in ignore_cols]
+
+    if len(cols_to_inspect) == 0:
+        if debug:
+            dprint(f"All columns are ignored, skipping datetime detection...")
+        return df
+
     ### apply regex to columns to determine which are ISO datetimes
     iso_dt_regex = r'\d{4}-\d{2}-\d{2}.\d{2}\:\d{2}\:\d+'
-    dt_mask = df.astype(str).apply(
+    dt_mask = df[cols_to_inspect].astype(str).apply(
         lambda s: s.str.match(iso_dt_regex).all()
     )
 
     ### list of datetime column names
-    datetimes = list(df.loc[:, dt_mask])
+    datetime_cols = [col for col in df[cols_to_inspect].loc[:, dt_mask]]
+    if not datetime_cols:
+        if debug:
+            dprint("No columns detected as datetimes, returning...")
+        return df
+
     if debug:
-        dprint("Converting columns to datetimes: " + str(datetimes))
+        dprint("Converting columns to datetimes: " + str(datetime_cols))
 
-    ### apply to_datetime
-    df[datetimes] = df[datetimes].apply(pd.to_datetime)
+    try:
+        df[datetime_cols] = df[datetime_cols].apply(pd.to_datetime, utc=True)
+    except Exception as e:
+        warn(
+            f"Unable to apply `pd.to_datetime` to {items_str(datetime_cols)}:\n"
+            + f"{traceback.format_exc()}"
+        )
 
-    ### strip timezone information
-    for dt in datetimes:
-        df[dt] = df[dt].dt.tz_localize(None)
+    for dt in datetime_cols:
+        try:
+            df[dt] = df[dt].dt.tz_localize(None)
+        except Exception as e:
+            warn(f"Unable to convert column '{dt}' to naive datetime:\n{traceback.format_exc()}")
 
     return df
 
+
 def timed_input(
         seconds: int = 10,
         timeout_message: str = "",
         prompt: str = "",
         icon: bool = False,
         **kw
     ) -> Union[str, None]:
@@ -1919,7 +1945,155 @@
         for col, ix in cols_indices.items()
         if (
             ix is not None
             and
             not isinstance(df.loc[ix][col], Hashable)
         )
     ]
+
+
+def enforce_dtypes(
+        df: 'pd.DataFrame',
+        dtypes: Dict[str, str],
+        debug: bool = False,
+    ) -> 'pd.DataFrame':
+    """
+    Enforce the `dtypes` dictionary on a DataFrame.
+
+    Parameters
+    ----------
+    df: pd.DataFrame
+        The DataFrame on which to enforce dtypes.
+
+    dtypes: Dict[str, str]
+        The data types to attempt to enforce on the DataFrame.
+
+    debug: bool, default False
+        Verbosity toggle.
+
+    Returns
+    -------
+    The Pandas DataFrame with the types enforced.
+    """
+    import json
+    import traceback
+    from meerschaum.utils.debug import dprint
+    from meerschaum.utils.warnings import warn
+    from meerschaum.utils.formatting import pprint
+    from meerschaum.config.static import STATIC_CONFIG
+    from meerschaum.utils.packages import import_pandas
+    df_dtypes = {c: str(t) for c, t in df.dtypes.items()}
+    if len(df_dtypes) == 0:
+        if debug:
+            dprint("Incoming DataFrame has no columns. Skipping enforcement...")
+        return df
+
+    pipe_pandas_dtypes = {
+        col: to_pandas_dtype(typ)
+        for col, typ in dtypes.items()
+    }
+    json_cols = [
+        col
+        for col, typ in dtypes.items()
+        if typ == 'json'
+    ]
+    if debug:
+        dprint(f"Desired data types:")
+        pprint(dtypes)
+        dprint(f"Data types for incoming DataFrame:")
+        pprint(df_dtypes)
+
+    if json_cols and len(df) > 0:
+        if debug:
+            dprint(f"Checking columns for JSON encoding: {json_cols}")
+        for col in json_cols:
+            if col in df.columns:
+                try:
+                    df[col] = df[col].apply(
+                        (
+                            lambda x: (
+                                json.loads(x)
+                                if isinstance(x, str)
+                                else x
+                            )
+                        )
+                    )
+                except Exception as e:
+                    if debug:
+                        dprint(f"Unable to parse column '{col}' as JSON:\n{e}")
+
+    if df_dtypes == pipe_pandas_dtypes:
+        if debug:
+            dprint(f"Data types match. Exiting enforcement...")
+        return df
+
+    common_dtypes = {}
+    common_diff_dtypes = {}
+    for col, typ in pipe_pandas_dtypes.items():
+        if col in df_dtypes:
+            common_dtypes[col] = typ
+            if typ != df_dtypes[col]:
+                common_diff_dtypes[col] = df_dtypes[col]
+
+    if debug:
+        dprint(f"Common columns with different dtypes:")
+        pprint(common_diff_dtypes)
+
+    detected_dt_cols = {}
+    for col, typ in common_diff_dtypes.items():
+        if 'datetime' in typ and 'datetime' in common_dtypes[col]:
+            df_dtypes[col] = typ
+            detected_dt_cols[col] = (common_dtypes[col], common_diff_dtypes[col])
+    for col in detected_dt_cols:
+        del common_diff_dtypes[col]
+
+    if debug:
+        dprint(f"Common columns with different dtypes (after dates):")
+        pprint(common_diff_dtypes)
+
+    if df_dtypes == pipe_pandas_dtypes:
+        if debug:
+            dprint(
+                "The incoming DataFrame has mostly the same types, skipping enforcement."
+                + f"The only detected difference was in the following datetime columns.\n"
+                + "    Timezone information may be stripped."
+            )
+            pprint(detected_dt_cols)
+        return df
+
+    if set(common_dtypes) == set(df_dtypes):
+        min_ratio = STATIC_CONFIG['pipes']['dtypes']['min_ratio_columns_changed_for_full_astype']
+        if (
+            len(common_diff_dtypes) >= int(len(common_dtypes) * min_ratio)
+        ):
+            if debug:
+                dprint(f"Enforcing dtypes columns on incoming DataFrame...")
+                pprint(common_dtypes)
+            try:
+                return df[
+                    list(common_dtypes.keys())
+                ].astype({
+                    col: typ
+                    for col, typ in pipe_pandas_dtypes.items()
+                    if col in common_dtypes
+                })
+            except Exception as e:
+                if debug:
+                    dprint(f"Encountered an error when enforcing data types:\n{e}")
+    
+    for d in common_diff_dtypes:
+        t = common_dtypes[d]
+        if debug:
+            dprint(f"Casting column {d} to dtype {t}.")
+        try:
+            df[d] = df[d].astype(t)
+        except Exception as e:
+            if debug:
+                dprint(f"Encountered an error when casting column {d} to type {t}:\n{e}")
+            if 'int' in str(t.lower()):
+                try:
+                    df[d] = df[d].astype('float64').astype(t)
+                except Exception as e:
+                    if debug:
+                        dprint(f"Was unable to convert to float then {t}.")
+    return df
+
```

### Comparing `meerschaum-1.6.3/meerschaum/utils/networking.py` & `meerschaum-1.6.4/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/packages/__init__.py` & `meerschaum-1.6.4/meerschaum/utils/packages/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,29 +85,22 @@
 
     if not candidates:
         if _try_install_name_on_fail:
             return get_module_path(
                 import_name, venv=venv, debug=debug,
                 _try_install_name_on_fail=False
             )
-        if debug:
-            dprint(f"No candidates found for '{import_name}' in venv '{venv}'.", color=False)
         return None
 
     specs_paths = []
     for candidate_path in candidates:
         spec = importlib.util.spec_from_file_location(import_name, str(candidate_path))
         if spec is not None:
             return candidate_path
     
-    if debug:
-        dprint(
-            f"Was unable to find a file location for '{import_name}' in venv '{venv}'.",
-            color = False,
-        )
     return None
 
 
 def manually_import_module(
         import_name: str,
         venv: Optional[str] = 'mrsm',
         check_update: bool = True,
@@ -203,19 +196,15 @@
     _version = (
         determine_version(
             pathlib.Path(root_spec.origin),
             import_name=root_name, venv=venv, debug=debug
         ) if root_spec is not None and root_spec.origin is not None else None
     )
 
-    if debug:
-        dprint(f'root_name: {root_name}', color=color)
     if _version is not None:
-        if debug:
-            dprint(f'_version: {_version}', color=color)
         if check_update:
             if need_update(
                 None,
                 import_name = root_name,
                 version = _version,
                 check_pypi = check_pypi,
                 debug = debug,
@@ -390,16 +379,14 @@
             _v = filename.replace('.dist-info', '').split("-")[-1]
             _found_versions.append(_v)
 
     if len(_found_versions) == 1:
         _version = _found_versions[0]
         with _locks['import_versions']:
             import_versions[venv][import_name] = _version
-        if debug:
-            print(f"Found version {_version} for {import_name}.")
         return _found_versions[0]
 
     if not _found_versions:
         try:
             import importlib.metadata as importlib_metadata
         except ImportError:
             importlib_metadata = attempt_import(
@@ -559,36 +546,29 @@
     install_name = install_name or _import_to_install_name(root_name)
     with _locks['_checked_for_updates']:
         if install_name in _checked_for_updates:
             return False
         _checked_for_updates.add(install_name)
 
     _install_no_version = get_install_no_version(install_name)
-    if debug:
-        dprint(f"_install_no_version: {_install_no_version}", color=color)
     required_version = install_name.replace(_install_no_version, '')
     if ']' in required_version:
         required_version = required_version.split(']')[1]
 
     ### No minimum version was specified, and we're not going to check PyPI.
     if not required_version and not check_pypi:
         return False
 
-    if debug:
-        dprint(f"required_version: {required_version}", color=color)
-
     try:
         if not version:
             if not _run_determine_version:
                 version = determine_version(
                     pathlib.Path(package.__file__),
                     import_name=root_name, warn=False, debug=debug
                 )
-        if debug:
-            dprint(f"version: {version}", color=color)
         if version is None:
             return False
     except Exception as e:
         if debug:
             dprint(str(e), color=color)
             dprint("No version could be determined from the installed package.", color=color)
         return False
@@ -625,18 +605,14 @@
         result = checker.check(_install_no_version, version)
     else:
         ### Skip PyPI and assume we can't be sure.
         result = None
 
     ### Compare PyPI's version with our own.
     if result is not None:
-        if debug:
-            dprint(f"Available version: {result.available_version}", color=color)
-            dprint(f"Required version: {required_version}", color=color)
-
         ### We have a result from PyPI and a stated required version.
         if required_version:
             try:
                 return semver.Version.parse(result.available_version).match(required_version)
             except AttributeError as e:
                 pip_install(_import_to_install_name('semver'), venv='mrsm', debug=debug)
                 semver = manually_import_module('semver', venv='mrsm')
@@ -1518,20 +1494,14 @@
                 get_module_path(root_name, venv=venv, debug=debug)
                 or
                 importlib.util.find_spec(root_name).origin
             )
         except (ModuleNotFoundError, ValueError, AttributeError, TypeError) as e:
             spec_path = None
 
-        if debug:
-            if spec_path is not None:
-                dprint(f"Found a path for '{root_name}':\n{spec_path}", color=False)
-            else:
-                dprint(f"Could not find a path for '{root_name}':\n{spec_path}", color=False)
-
         found = (
             not need_update(
                 None, import_name = root_name,
                 _run_determine_version = False,
                 check_pypi = False,
                 version = determine_version(
                     spec_path, venv=venv, debug=debug, import_name=root_name
```

### Comparing `meerschaum-1.6.3/meerschaum/utils/packages/_packages.py` & `meerschaum-1.6.4/meerschaum/utils/packages/_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     },
     'dev-tools': {
         'twine'                      : 'twine>=3.2.0',
         'tuna'                       : 'tuna>=0.5.3',
         'snakeviz'                   : 'snakeviz>=2.1.0',
         'mypy'                       : 'mypy>=0.812.0',
         'pytest'                     : 'pytest>=6.2.2',
+        'pytest_xdist'               : 'pytest-xdist>=3.2.1',
         'heartrate'                  : 'heartrate>=0.2.1',
         'pyheat'                     : 'py-heat>=0.0.6',
     },
     'setup': {
     },
     'docs': {
         'mkdocs'                     : 'mkdocs>=1.1.2',
```

### Comparing `meerschaum-1.6.3/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-1.6.4/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/pool.py` & `meerschaum-1.6.4/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/process.py` & `meerschaum-1.6.4/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/prompt.py` & `meerschaum-1.6.4/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/schedule.py` & `meerschaum-1.6.4/meerschaum/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/sql.py` & `meerschaum-1.6.4/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/threading.py` & `meerschaum-1.6.4/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/typing.py` & `meerschaum-1.6.4/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/venv/_Venv.py` & `meerschaum-1.6.4/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/venv/__init__.py` & `meerschaum-1.6.4/meerschaum/utils/venv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,14 @@
     if debug:
         from meerschaum.utils.debug import dprint
     if venv is not None:
         init_venv(venv=venv, debug=debug)
     with LOCKS['active_venvs']:
         if thread_id not in threads_active_venvs:
             threads_active_venvs[thread_id] = {}
-        if debug:
-            dprint(f"Activating virtual environment '{venv}'...", color=color)
         active_venvs.add(venv)
         if venv not in threads_active_venvs[thread_id]:
             threads_active_venvs[thread_id][venv] = 1
         else:
             threads_active_venvs[thread_id][venv] += 1
 
         target = str(venv_target_path(venv, debug=debug))
@@ -140,63 +138,43 @@
     import sys
     thread_id = get_ident()
     if venv is None:
         if venv in active_venvs:
             active_venvs.remove(venv)
         return True
 
-    if debug:
-        from meerschaum.utils.debug import dprint
-
     if previously_active_venvs and venv in previously_active_venvs and not force:
-        if debug:
-            dprint(f"Ignore call to deactivate virtual environment '{venv}'...", color=color)
         return True
 
     with LOCKS['active_venvs']:
         if venv in threads_active_venvs.get(thread_id, {}):
             new_count = threads_active_venvs[thread_id][venv] - 1
             if new_count > 0 and not force:
                 threads_active_venvs[thread_id][venv] = new_count
-                if debug:
-                    dprint(
-                        f"Decremented venv '{venv}' to {new_count} on thread {thread_id}, "
-                        + "staying active...",
-                        color = color,
-                    )
                 return True
             else:
                 del threads_active_venvs[thread_id][venv]
 
         if not force:
             for other_thread_id, other_venvs in threads_active_venvs.items():
                 if other_thread_id == thread_id:
                     continue
                 if venv in other_venvs:
-                    if debug:
-                        dprint(
-                            f"Venv '{venv}' is still being used by other threads,"
-                            + "keeping active...",
-                            color = color,
-                        )
                     return True
         else:
             to_delete = [other_thread_id for other_thread_id in threads_active_venvs]
             for other_thread_id in to_delete:
                 del threads_active_venvs[other_thread_id]
 
         if venv in active_venvs:
             active_venvs.remove(venv)
 
     if sys.path is None:
         return False
 
-    if debug:
-        dprint(f"Deactivating virtual environment '{venv}'...", color=color)
-
     target = str(venv_target_path(venv, allow_nonexistent=force, debug=debug))
     with LOCKS['sys.path']:
         if target in sys.path:
             sys.path.remove(target)
             try:
                 active_venvs_order.remove(venv)
             except Exception as e:
@@ -225,17 +203,14 @@
         Verbosity toggle.
 
     Returns
     -------
     A bool indicating whether the virtual environment `venv` is active.
 
     """
-    if debug:
-        from meerschaum.utils.debug import dprint
-        dprint(f"Checking if virtual environment '{venv}' is active.", color=color)
     return venv in active_venvs
 
 
 verified_venvs = set()
 def verify_venv(
         venv: str,
         debug: bool = False,
```

### Comparing `meerschaum-1.6.3/meerschaum/utils/warnings.py` & `meerschaum-1.6.4/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum/utils/yaml.py` & `meerschaum-1.6.4/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum.egg-info/PKG-INFO` & `meerschaum-1.6.4/meerschaum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.3
+Version: 1.6.4
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.3/meerschaum.egg-info/SOURCES.txt` & `meerschaum-1.6.4/meerschaum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.3/meerschaum.egg-info/requires.txt` & `meerschaum-1.6.4/meerschaum.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 
 [dev-tools]
 twine>=3.2.0
 tuna>=0.5.3
 snakeviz>=2.1.0
 mypy>=0.812.0
 pytest>=6.2.2
+pytest-xdist>=3.2.1
 heartrate>=0.2.1
 py-heat>=0.0.6
 
 [docs]
 mkdocs>=1.1.2
 mkdocs-material>=6.2.5
 mkdocs-material-extensions>=1.0.3
```

### Comparing `meerschaum-1.6.3/setup.py` & `meerschaum-1.6.4/setup.py`

 * *Files identical despite different names*

