# Comparing `tmp/aprsd-3.0.2.tar.gz` & `tmp/aprsd-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd-3.0.2.tar", last modified: Mon Jan 16 16:41:22 2023, max compression
+gzip compressed data, was "aprsd-3.0.3.tar", last modified: Tue Apr 25 18:44:13 2023, max compression
```

## Comparing `aprsd-3.0.2.tar` & `aprsd-3.0.3.tar`

### file list

```diff
@@ -1,228 +1,229 @@
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:22.101292 aprsd-3.0.2/
--rw-r--r--   0 i530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.0.2/.coveragerc
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.242739 aprsd-3.0.2/.github/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.337664 aprsd-3.0.2/.github/workflows/
--rw-r--r--   0 i530566    (501) staff       (20)     1624 2022-12-16 13:25:52.000000 aprsd-3.0.2/.github/workflows/master-build.yml
--rw-r--r--   0 i530566    (501) staff       (20)      526 2022-11-23 18:33:33.000000 aprsd-3.0.2/.github/workflows/python.yml
--rw-r--r--   0 i530566    (501) staff       (20)     1283 2022-12-16 13:25:52.000000 aprsd-3.0.2/.github/workflows/release_build.yml
--rw-r--r--   0 i530566    (501) staff       (20)      536 2021-08-30 17:18:20.000000 aprsd-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 i530566    (501) staff       (20)      397 2023-01-16 16:41:08.000000 aprsd-3.0.2/AUTHORS
--rw-r--r--   0 i530566    (501) staff       (20)    20474 2023-01-16 16:41:07.000000 aprsd-3.0.2/ChangeLog
--rw-r--r--   0 i530566    (501) staff       (20)      753 2021-08-13 16:31:50.000000 aprsd-3.0.2/INSTALL.txt
--rw-r--r--   0 i530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.0.2/LICENSE
--rw-r--r--   0 i530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.0.2/MANIFEST.in
--rw-r--r--   0 i530566    (501) staff       (20)     2730 2022-12-29 19:14:43.000000 aprsd-3.0.2/Makefile
--rw-r--r--   0 i530566    (501) staff       (20)    20836 2023-01-16 16:41:22.101888 aprsd-3.0.2/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)    20002 2022-12-29 19:14:43.000000 aprsd-3.0.2/README.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.348598 aprsd-3.0.2/aprsd/
--rw-r--r--   0 i530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.0.2/aprsd/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     4566 2023-01-03 14:01:59.000000 aprsd-3.0.2/aprsd/aprsd.py
--rw-r--r--   0 i530566    (501) staff       (20)     3212 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/cli_helper.py
--rw-r--r--   0 i530566    (501) staff       (20)     8376 2023-01-02 19:20:16.000000 aprsd-3.0.2/aprsd/client.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.365089 aprsd-3.0.2/aprsd/clients/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.0.2/aprsd/clients/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     6916 2022-12-21 21:26:43.000000 aprsd-3.0.2/aprsd/clients/aprsis.py
--rw-r--r--   0 i530566    (501) staff       (20)     3368 2023-01-07 19:57:29.000000 aprsd-3.0.2/aprsd/clients/kiss.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.394828 aprsd-3.0.2/aprsd/cmds/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.2/aprsd/cmds/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1764 2022-12-12 18:34:05.000000 aprsd-3.0.2/aprsd/cmds/completion.py
--rw-r--r--   0 i530566    (501) staff       (20)     3111 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/cmds/dev.py
--rw-r--r--   0 i530566    (501) staff       (20)     2810 2022-12-31 21:31:43.000000 aprsd-3.0.2/aprsd/cmds/healthcheck.py
--rw-r--r--   0 i530566    (501) staff       (20)     7921 2022-12-12 18:34:06.000000 aprsd-3.0.2/aprsd/cmds/list_plugins.py
--rw-r--r--   0 i530566    (501) staff       (20)     4979 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/cmds/listen.py
--rw-r--r--   0 i530566    (501) staff       (20)     4717 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/cmds/send_message.py
--rw-r--r--   0 i530566    (501) staff       (20)     3069 2023-01-07 19:57:29.000000 aprsd-3.0.2/aprsd/cmds/server.py
--rw-r--r--   0 i530566    (501) staff       (20)    14234 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/cmds/webchat.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.403163 aprsd-3.0.2/aprsd/conf/
--rw-r--r--   0 i530566    (501) staff       (20)     1733 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/conf/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2353 2023-01-02 19:20:16.000000 aprsd-3.0.2/aprsd/conf/client.py
--rw-r--r--   0 i530566    (501) staff       (20)     4339 2023-01-03 20:38:25.000000 aprsd-3.0.2/aprsd/conf/common.py
--rw-r--r--   0 i530566    (501) staff       (20)     1235 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/conf/log.py
--rw-r--r--   0 i530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/conf/opts.py
--rw-r--r--   0 i530566    (501) staff       (20)     2308 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/conf/plugin_common.py
--rw-r--r--   0 i530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.0.2/aprsd/conf/plugin_email.py
--rw-r--r--   0 i530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.0.2/aprsd/exception.py
--rw-r--r--   0 i530566    (501) staff       (20)    10299 2022-12-31 21:31:43.000000 aprsd-3.0.2/aprsd/flask.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.407385 aprsd-3.0.2/aprsd/logging/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.2/aprsd/logging/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2690 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/logging/log.py
--rw-r--r--   0 i530566    (501) staff       (20)     5549 2022-12-12 18:34:07.000000 aprsd-3.0.2/aprsd/logging/rich.py
--rw-r--r--   0 i530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.0.2/aprsd/messaging.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.435527 aprsd-3.0.2/aprsd/packets/
--rw-r--r--   0 i530566    (501) staff       (20)      432 2023-01-16 16:38:59.000000 aprsd-3.0.2/aprsd/packets/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)    16644 2023-01-14 17:53:27.000000 aprsd-3.0.2/aprsd/packets/core.py
--rw-r--r--   0 i530566    (501) staff       (20)     1457 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/packets/packet_list.py
--rw-r--r--   0 i530566    (501) staff       (20)     1071 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/packets/seen_list.py
--rw-r--r--   0 i530566    (501) staff       (20)     3205 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/packets/tracker.py
--rw-r--r--   0 i530566    (501) staff       (20)     2880 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/packets/watch_list.py
--rw-r--r--   0 i530566    (501) staff       (20)    15814 2022-12-29 19:18:53.000000 aprsd-3.0.2/aprsd/plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/plugin_utils.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.449890 aprsd-3.0.2/aprsd/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.0.2/aprsd/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)    23077 2022-12-29 19:18:54.000000 aprsd-3.0.2/aprsd/plugins/email.py
--rw-r--r--   0 i530566    (501) staff       (20)     1463 2022-12-29 19:18:51.000000 aprsd-3.0.2/aprsd/plugins/fortune.py
--rw-r--r--   0 i530566    (501) staff       (20)     2844 2022-12-29 19:18:51.000000 aprsd-3.0.2/aprsd/plugins/location.py
--rw-r--r--   0 i530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/plugins/notify.py
--rw-r--r--   0 i530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.0.2/aprsd/plugins/ping.py
--rw-r--r--   0 i530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/plugins/query.py
--rw-r--r--   0 i530566    (501) staff       (20)     3496 2022-12-29 19:18:51.000000 aprsd-3.0.2/aprsd/plugins/time.py
--rw-r--r--   0 i530566    (501) staff       (20)      849 2022-12-29 19:18:51.000000 aprsd-3.0.2/aprsd/plugins/version.py
--rw-r--r--   0 i530566    (501) staff       (20)    13054 2022-12-29 19:18:52.000000 aprsd-3.0.2/aprsd/plugins/weather.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.453817 aprsd-3.0.2/aprsd/rpc/
--rw-r--r--   0 i530566    (501) staff       (20)      343 2022-12-31 21:45:32.000000 aprsd-3.0.2/aprsd/rpc/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     4192 2022-12-31 21:45:32.000000 aprsd-3.0.2/aprsd/rpc/client.py
--rw-r--r--   0 i530566    (501) staff       (20)     2424 2022-12-31 21:45:32.000000 aprsd-3.0.2/aprsd/rpc/server.py
--rw-r--r--   0 i530566    (501) staff       (20)     6752 2022-12-30 14:44:36.000000 aprsd-3.0.2/aprsd/stats.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.464324 aprsd-3.0.2/aprsd/threads/
--rw-r--r--   0 i530566    (501) staff       (20)      274 2022-12-20 22:38:48.000000 aprsd-3.0.2/aprsd/threads/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1890 2022-12-20 22:38:48.000000 aprsd-3.0.2/aprsd/threads/aprsd.py
--rw-r--r--   0 i530566    (501) staff       (20)     2968 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/threads/keep_alive.py
--rw-r--r--   0 i530566    (501) staff       (20)     2040 2022-12-29 19:14:43.000000 aprsd-3.0.2/aprsd/threads/log_monitor.py
--rw-r--r--   0 i530566    (501) staff       (20)    10430 2023-01-14 17:53:27.000000 aprsd-3.0.2/aprsd/threads/rx.py
--rw-r--r--   0 i530566    (501) staff       (20)     5160 2022-12-29 19:14:44.000000 aprsd-3.0.2/aprsd/threads/tx.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.491279 aprsd-3.0.2/aprsd/utils/
--rw-r--r--   0 i530566    (501) staff       (20)     3532 2022-12-16 13:25:52.000000 aprsd-3.0.2/aprsd/utils/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1151 2022-12-20 22:38:48.000000 aprsd-3.0.2/aprsd/utils/counter.py
--rw-r--r--   0 i530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.0.2/aprsd/utils/fuzzyclock.py
--rw-r--r--   0 i530566    (501) staff       (20)     1871 2022-12-20 22:38:48.000000 aprsd-3.0.2/aprsd/utils/json.py
--rw-r--r--   0 i530566    (501) staff       (20)     3200 2022-12-29 19:14:44.000000 aprsd-3.0.2/aprsd/utils/objectstore.py
--rw-r--r--   0 i530566    (501) staff       (20)     1111 2022-12-20 22:38:48.000000 aprsd-3.0.2/aprsd/utils/ring_buffer.py
--rw-r--r--   0 i530566    (501) staff       (20)     5558 2022-12-12 18:34:08.000000 aprsd-3.0.2/aprsd/utils/trace.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.492340 aprsd-3.0.2/aprsd/web/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.2/aprsd/web/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.493331 aprsd-3.0.2/aprsd/web/admin/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.2/aprsd/web/admin/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.250616 aprsd-3.0.2/aprsd/web/admin/static/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.503578 aprsd-3.0.2/aprsd/web/admin/static/css/
--rw-r--r--   0 i530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/css/index.css
--rw-r--r--   0 i530566    (501) staff       (20)     3467 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/css/prism.css
--rw-r--r--   0 i530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/css/tabs.css
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.546443 aprsd-3.0.2/aprsd/web/admin/static/images/
--rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/images/Untitled.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.610727 aprsd-3.0.2/aprsd/web/admin/static/js/
--rw-r--r--   0 i530566    (501) staff       (20)     7360 2022-12-20 22:38:48.000000 aprsd-3.0.2/aprsd/web/admin/static/js/charts.js
--rw-r--r--   0 i530566    (501) staff       (20)      658 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/js/logs.js
--rw-r--r--   0 i530566    (501) staff       (20)     6796 2022-12-29 19:14:44.000000 aprsd-3.0.2/aprsd/web/admin/static/js/main.js
--rw-r--r--   0 i530566    (501) staff       (20)    64705 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/js/prism.js
--rw-r--r--   0 i530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.0.2/aprsd/web/admin/static/js/send-message.js
--rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/js/tabs.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.640313 aprsd-3.0.2/aprsd/web/admin/static/json-viewer/
--rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.646986 aprsd-3.0.2/aprsd/web/admin/templates/
--rw-r--r--   0 i530566    (501) staff       (20)     8010 2022-12-29 19:14:44.000000 aprsd-3.0.2/aprsd/web/admin/templates/index.html
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.254690 aprsd-3.0.2/aprsd/web/chat/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.253965 aprsd-3.0.2/aprsd/web/chat/static/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.701595 aprsd-3.0.2/aprsd/web/chat/static/css/
--rw-r--r--   0 i530566    (501) staff       (20)     1376 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/css/index.css
--rw-r--r--   0 i530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/css/style.css.map
--rw-r--r--   0 i530566    (501) staff       (20)      718 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/css/tabs.css
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.744369 aprsd-3.0.2/aprsd/web/chat/static/images/
--rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/images/Untitled.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.793969 aprsd-3.0.2/aprsd/web/chat/static/js/
--rw-r--r--   0 i530566    (501) staff       (20)     1906 2022-12-16 17:08:52.000000 aprsd-3.0.2/aprsd/web/chat/static/js/gps.js
--rw-r--r--   0 i530566    (501) staff       (20)     1226 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/js/main.js
--rw-r--r--   0 i530566    (501) staff       (20)     6304 2022-12-04 23:39:18.000000 aprsd-3.0.2/aprsd/web/chat/static/js/send-message-mobile.js
--rw-r--r--   0 i530566    (501) staff       (20)     6041 2022-12-04 23:39:18.000000 aprsd-3.0.2/aprsd/web/chat/static/js/send-message.js
--rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/js/tabs.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.798878 aprsd-3.0.2/aprsd/web/chat/static/json-viewer/
--rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.0.2/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.834170 aprsd-3.0.2/aprsd/web/chat/templates/
--rw-r--r--   0 i530566    (501) staff       (20)     4020 2022-12-04 23:39:18.000000 aprsd-3.0.2/aprsd/web/chat/templates/index.html
--rw-r--r--   0 i530566    (501) staff       (20)     4055 2022-12-04 23:39:18.000000 aprsd-3.0.2/aprsd/web/chat/templates/mobile.html
--rw-r--r--   0 i530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.0.2/aprsd-lnav.json
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.360666 aprsd-3.0.2/aprsd.egg-info/
--rw-r--r--   0 i530566    (501) staff       (20)    20836 2023-01-16 16:41:08.000000 aprsd-3.0.2/aprsd.egg-info/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)     4926 2023-01-16 16:41:21.000000 aprsd-3.0.2/aprsd.egg-info/SOURCES.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-01-16 16:41:08.000000 aprsd-3.0.2/aprsd.egg-info/dependency_links.txt
--rw-r--r--   0 i530566    (501) staff       (20)      172 2023-01-16 16:41:08.000000 aprsd-3.0.2/aprsd.egg-info/entry_points.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-01-09 16:04:15.000000 aprsd-3.0.2/aprsd.egg-info/not-zip-safe
--rw-r--r--   0 i530566    (501) staff       (20)       46 2023-01-16 16:41:08.000000 aprsd-3.0.2/aprsd.egg-info/pbr.json
--rw-r--r--   0 i530566    (501) staff       (20)     1077 2023-01-16 16:41:08.000000 aprsd-3.0.2/aprsd.egg-info/requires.txt
--rw-r--r--   0 i530566    (501) staff       (20)        6 2023-01-16 16:41:08.000000 aprsd-3.0.2/aprsd.egg-info/top_level.txt
--rw-r--r--   0 i530566    (501) staff       (20)      221 2022-12-07 14:15:59.000000 aprsd-3.0.2/dev-requirements.in
--rw-r--r--   0 i530566    (501) staff       (20)     3910 2023-01-07 19:53:27.000000 aprsd-3.0.2/dev-requirements.txt
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.848196 aprsd-3.0.2/docker/
--rw-r--r--   0 i530566    (501) staff       (20)     1567 2023-01-14 17:53:27.000000 aprsd-3.0.2/docker/Dockerfile
--rw-r--r--   0 i530566    (501) staff       (20)     2007 2023-01-02 19:13:49.000000 aprsd-3.0.2/docker/Dockerfile-dev
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.853575 aprsd-3.0.2/docker/bin/
--rwxr-xr-x   0 i530566    (501) staff       (20)      812 2022-12-30 15:13:03.000000 aprsd-3.0.2/docker/bin/run.sh
--rwxr-xr-x   0 i530566    (501) staff       (20)     2548 2023-01-14 17:53:27.000000 aprsd-3.0.2/docker/build.sh
--rw-r--r--   0 i530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.0.2/docker/docker-compose.yml
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.943941 aprsd-3.0.2/docs/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.958170 aprsd-3.0.2/docs/_static/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.0.2/docs/_static/.keep
--rw-r--r--   0 i530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.0.2/docs/_static/aprsd_overview.png
--rw-r--r--   0 i530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.0.2/docs/_static/aprsd_overview.svg
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.959811 aprsd-3.0.2/docs/_templates/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.0.2/docs/_templates/.keep
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:22.047340 aprsd-3.0.2/docs/apidoc/
--rw-r--r--   0 i530566    (501) staff       (20)      477 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.clients.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1357 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.cmds.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1044 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.conf.rst
--rw-r--r--   0 i530566    (501) staff       (20)      468 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.logging.rst
--rw-r--r--   0 i530566    (501) staff       (20)      969 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.packets.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1523 2023-01-01 19:58:19.000000 aprsd-3.0.2/docs/apidoc/aprsd.plugins.rst
--rw-r--r--   0 i530566    (501) staff       (20)      447 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.rpc.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1539 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.rst
--rw-r--r--   0 i530566    (501) staff       (20)      934 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.threads.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1075 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.utils.rst
--rw-r--r--   0 i530566    (501) staff       (20)      168 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.web.admin.rst
--rw-r--r--   0 i530566    (501) staff       (20)      225 2023-01-02 19:13:49.000000 aprsd-3.0.2/docs/apidoc/aprsd.web.rst
--rw-r--r--   0 i530566    (501) staff       (20)       52 2023-01-01 19:58:20.000000 aprsd-3.0.2/docs/apidoc/modules.rst
--rw-r--r--   0 i530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.0.2/docs/aprsd.drawio
--rw-r--r--   0 i530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.0.2/docs/changelog.rst
--rw-r--r--   0 i530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.0.2/docs/clean_docs.py
--rw-r--r--   0 i530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.0.2/docs/conf.py
--rw-r--r--   0 i530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.0.2/docs/configure.rst
--rw-r--r--   0 i530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.0.2/docs/index.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.0.2/docs/install.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.0.2/docs/links.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.0.2/docs/plugin.rst
--rw-r--r--   0 i530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.0.2/docs/readme.rst
--rw-r--r--   0 i530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.0.2/docs/server.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:21.258405 aprsd-3.0.2/examples/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:22.054066 aprsd-3.0.2/examples/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.2/examples/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)      409 2022-12-20 22:38:48.000000 aprsd-3.0.2/examples/plugins/example_plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.0.2/gray.conf
--rw-r--r--   0 i530566    (501) staff       (20)      538 2021-08-30 17:18:20.000000 aprsd-3.0.2/pyproject.toml
--rw-r--r--   0 i530566    (501) staff       (20)      539 2023-01-07 19:57:15.000000 aprsd-3.0.2/requirements.in
--rw-r--r--   0 i530566    (501) staff       (20)     3350 2023-01-07 19:53:14.000000 aprsd-3.0.2/requirements.txt
--rw-r--r--   0 i530566    (501) staff       (20)     1246 2023-01-16 16:41:22.107451 aprsd-3.0.2/setup.cfg
--rw-r--r--   0 i530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.0.2/setup.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:22.062904 aprsd-3.0.2/tests/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.2/tests/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:22.083701 aprsd-3.0.2/tests/cmds/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.0.2/tests/cmds/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1819 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/cmds/test_send_message.py
--rw-r--r--   0 i530566    (501) staff       (20)     2505 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/cmds/test_webchat.py
--rw-r--r--   0 i530566    (501) staff       (20)     1674 2022-12-20 22:38:48.000000 aprsd-3.0.2/tests/fake.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:22.095809 aprsd-3.0.2/tests/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.2/tests/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_fortune.py
--rw-r--r--   0 i530566    (501) staff       (20)     3793 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_location.py
--rw-r--r--   0 i530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_notify.py
--rw-r--r--   0 i530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_ping.py
--rw-r--r--   0 i530566    (501) staff       (20)     1696 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_query.py
--rw-r--r--   0 i530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_time.py
--rw-r--r--   0 i530566    (501) staff       (20)      970 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_version.py
--rw-r--r--   0 i530566    (501) staff       (20)     7613 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/plugins/test_weather.py
--rw-r--r--   0 i530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/test_email.py
--rw-r--r--   0 i530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/test_main.py
--rw-r--r--   0 i530566    (501) staff       (20)     3070 2022-12-22 17:04:16.000000 aprsd-3.0.2/tests/test_packets.py
--rw-r--r--   0 i530566    (501) staff       (20)     6486 2022-12-29 19:14:44.000000 aprsd-3.0.2/tests/test_plugin.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-01-16 16:41:22.100211 aprsd-3.0.2/tools/
--rwxr-xr-x   0 i530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.0.2/tools/fast8.sh
--rw-r--r--   0 i530566    (501) staff       (20)     2596 2022-12-20 22:38:48.000000 aprsd-3.0.2/tox.ini
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.399247 aprsd-3.0.3/
+-rw-r--r--   0 i530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.0.3/.coveragerc
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.309467 aprsd-3.0.3/.github/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.448006 aprsd-3.0.3/.github/workflows/
+-rw-r--r--   0 i530566    (501) staff       (20)     1624 2022-12-16 13:25:52.000000 aprsd-3.0.3/.github/workflows/master-build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      526 2022-11-23 18:33:33.000000 aprsd-3.0.3/.github/workflows/python.yml
+-rw-r--r--   0 i530566    (501) staff       (20)     1283 2022-12-16 13:25:52.000000 aprsd-3.0.3/.github/workflows/release_build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      536 2021-08-30 17:18:20.000000 aprsd-3.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 i530566    (501) staff       (20)      397 2023-04-25 18:43:57.000000 aprsd-3.0.3/AUTHORS
+-rw-r--r--   0 i530566    (501) staff       (20)    20802 2023-04-25 18:43:56.000000 aprsd-3.0.3/ChangeLog
+-rw-r--r--   0 i530566    (501) staff       (20)      753 2021-08-13 16:31:50.000000 aprsd-3.0.3/INSTALL.txt
+-rw-r--r--   0 i530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.0.3/LICENSE
+-rw-r--r--   0 i530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.0.3/MANIFEST.in
+-rw-r--r--   0 i530566    (501) staff       (20)     2730 2022-12-29 19:14:43.000000 aprsd-3.0.3/Makefile
+-rw-r--r--   0 i530566    (501) staff       (20)    20836 2023-04-25 18:44:13.399639 aprsd-3.0.3/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)    20002 2022-12-29 19:14:43.000000 aprsd-3.0.3/README.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.479151 aprsd-3.0.3/aprsd/
+-rw-r--r--   0 i530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4566 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/aprsd.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3212 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/cli_helper.py
+-rw-r--r--   0 i530566    (501) staff       (20)     8651 2023-04-10 17:40:19.000000 aprsd-3.0.3/aprsd/client.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.510176 aprsd-3.0.3/aprsd/clients/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.0.3/aprsd/clients/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7021 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/clients/aprsis.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3413 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/clients/kiss.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.543321 aprsd-3.0.3/aprsd/cmds/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/cmds/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1764 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/cmds/completion.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3075 2023-04-17 14:51:22.000000 aprsd-3.0.3/aprsd/cmds/dev.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2810 2022-12-31 21:31:43.000000 aprsd-3.0.3/aprsd/cmds/healthcheck.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7921 2022-12-12 18:34:06.000000 aprsd-3.0.3/aprsd/cmds/list_plugins.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6056 2023-04-17 19:37:53.000000 aprsd-3.0.3/aprsd/cmds/listen.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4717 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/cmds/send_message.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3401 2023-04-20 18:32:02.000000 aprsd-3.0.3/aprsd/cmds/server.py
+-rw-r--r--   0 i530566    (501) staff       (20)    14234 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/cmds/webchat.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.554285 aprsd-3.0.3/aprsd/conf/
+-rw-r--r--   0 i530566    (501) staff       (20)     1733 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/conf/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2353 2023-01-02 19:20:16.000000 aprsd-3.0.3/aprsd/conf/client.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4863 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/conf/common.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1235 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/conf/log.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/conf/opts.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2308 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/conf/plugin_common.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.0.3/aprsd/conf/plugin_email.py
+-rw-r--r--   0 i530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/exception.py
+-rw-r--r--   0 i530566    (501) staff       (20)    10299 2022-12-31 21:31:43.000000 aprsd-3.0.3/aprsd/flask.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.559034 aprsd-3.0.3/aprsd/logging/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.3/aprsd/logging/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2690 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/logging/log.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5549 2022-12-12 18:34:07.000000 aprsd-3.0.3/aprsd/logging/rich.py
+-rw-r--r--   0 i530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/messaging.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.585487 aprsd-3.0.3/aprsd/packets/
+-rw-r--r--   0 i530566    (501) staff       (20)      432 2023-01-16 16:38:59.000000 aprsd-3.0.3/aprsd/packets/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    16872 2023-04-17 14:51:23.000000 aprsd-3.0.3/aprsd/packets/core.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1457 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/packet_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1071 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/seen_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3205 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/tracker.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2880 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/packets/watch_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)    16435 2023-04-25 18:29:36.000000 aprsd-3.0.3/aprsd/plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2458 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/plugin_utils.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.598755 aprsd-3.0.3/aprsd/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    23077 2022-12-29 19:18:54.000000 aprsd-3.0.3/aprsd/plugins/email.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1463 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/fortune.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2844 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/location.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/plugins/notify.py
+-rw-r--r--   0 i530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.0.3/aprsd/plugins/ping.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/plugins/query.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3496 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/time.py
+-rw-r--r--   0 i530566    (501) staff       (20)      849 2022-12-29 19:18:51.000000 aprsd-3.0.3/aprsd/plugins/version.py
+-rw-r--r--   0 i530566    (501) staff       (20)    13054 2023-04-07 15:21:31.000000 aprsd-3.0.3/aprsd/plugins/weather.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.603258 aprsd-3.0.3/aprsd/rpc/
+-rw-r--r--   0 i530566    (501) staff       (20)      343 2022-12-31 21:45:32.000000 aprsd-3.0.3/aprsd/rpc/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4192 2022-12-31 21:45:32.000000 aprsd-3.0.3/aprsd/rpc/client.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2454 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/rpc/server.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6790 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/stats.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.630698 aprsd-3.0.3/aprsd/threads/
+-rw-r--r--   0 i530566    (501) staff       (20)      274 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/threads/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2023 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/threads/aprsd.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3588 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/threads/keep_alive.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2040 2022-12-29 19:14:43.000000 aprsd-3.0.3/aprsd/threads/log_monitor.py
+-rw-r--r--   0 i530566    (501) staff       (20)    10431 2023-04-18 18:13:29.000000 aprsd-3.0.3/aprsd/threads/rx.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5977 2023-01-19 19:14:47.000000 aprsd-3.0.3/aprsd/threads/tx.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.640640 aprsd-3.0.3/aprsd/utils/
+-rw-r--r--   0 i530566    (501) staff       (20)     3532 2022-12-16 13:25:52.000000 aprsd-3.0.3/aprsd/utils/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1151 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/utils/counter.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/utils/fuzzyclock.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1871 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/utils/json.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3200 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/utils/objectstore.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1111 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/utils/ring_buffer.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5558 2022-12-12 18:34:08.000000 aprsd-3.0.3/aprsd/utils/trace.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.641786 aprsd-3.0.3/aprsd/web/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/web/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.642669 aprsd-3.0.3/aprsd/web/admin/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/aprsd/web/admin/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.333545 aprsd-3.0.3/aprsd/web/admin/static/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.659116 aprsd-3.0.3/aprsd/web/admin/static/css/
+-rw-r--r--   0 i530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/css/index.css
+-rw-r--r--   0 i530566    (501) staff       (20)     3467 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/css/prism.css
+-rw-r--r--   0 i530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/css/tabs.css
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.701818 aprsd-3.0.3/aprsd/web/admin/static/images/
+-rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/Untitled.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.798151 aprsd-3.0.3/aprsd/web/admin/static/js/
+-rw-r--r--   0 i530566    (501) staff       (20)     7360 2022-12-20 22:38:48.000000 aprsd-3.0.3/aprsd/web/admin/static/js/charts.js
+-rw-r--r--   0 i530566    (501) staff       (20)      658 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/js/logs.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6796 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/web/admin/static/js/main.js
+-rw-r--r--   0 i530566    (501) staff       (20)    64705 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/js/prism.js
+-rw-r--r--   0 i530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/web/admin/static/js/send-message.js
+-rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/js/tabs.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.830654 aprsd-3.0.3/aprsd/web/admin/static/json-viewer/
+-rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.840171 aprsd-3.0.3/aprsd/web/admin/templates/
+-rw-r--r--   0 i530566    (501) staff       (20)     8010 2022-12-29 19:14:44.000000 aprsd-3.0.3/aprsd/web/admin/templates/index.html
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.336687 aprsd-3.0.3/aprsd/web/chat/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.336274 aprsd-3.0.3/aprsd/web/chat/static/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.911909 aprsd-3.0.3/aprsd/web/chat/static/css/
+-rw-r--r--   0 i530566    (501) staff       (20)     1376 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/css/index.css
+-rw-r--r--   0 i530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/css/style.css.map
+-rw-r--r--   0 i530566    (501) staff       (20)      718 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/css/tabs.css
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.953583 aprsd-3.0.3/aprsd/web/chat/static/images/
+-rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/Untitled.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.034365 aprsd-3.0.3/aprsd/web/chat/static/js/
+-rw-r--r--   0 i530566    (501) staff       (20)     1906 2022-12-16 17:08:52.000000 aprsd-3.0.3/aprsd/web/chat/static/js/gps.js
+-rw-r--r--   0 i530566    (501) staff       (20)     1226 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/js/main.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6304 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/static/js/send-message-mobile.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6041 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/static/js/send-message.js
+-rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/js/tabs.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.045921 aprsd-3.0.3/aprsd/web/chat/static/json-viewer/
+-rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.084993 aprsd-3.0.3/aprsd/web/chat/templates/
+-rw-r--r--   0 i530566    (501) staff       (20)     4020 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/templates/index.html
+-rw-r--r--   0 i530566    (501) staff       (20)     4055 2022-12-04 23:39:18.000000 aprsd-3.0.3/aprsd/web/chat/templates/mobile.html
+-rw-r--r--   0 i530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.0.3/aprsd-lnav.json
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.504980 aprsd-3.0.3/aprsd.egg-info/
+-rw-r--r--   0 i530566    (501) staff       (20)    20836 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)     4947 2023-04-25 18:44:12.000000 aprsd-3.0.3/aprsd.egg-info/SOURCES.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/dependency_links.txt
+-rw-r--r--   0 i530566    (501) staff       (20)      172 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/entry_points.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/not-zip-safe
+-rw-r--r--   0 i530566    (501) staff       (20)       47 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/pbr.json
+-rw-r--r--   0 i530566    (501) staff       (20)     1104 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/requires.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        6 2023-04-25 18:43:57.000000 aprsd-3.0.3/aprsd.egg-info/top_level.txt
+-rw-r--r--   0 i530566    (501) staff       (20)      221 2022-12-07 14:15:59.000000 aprsd-3.0.3/dev-requirements.in
+-rw-r--r--   0 i530566    (501) staff       (20)     3919 2023-01-19 19:14:47.000000 aprsd-3.0.3/dev-requirements.txt
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.105666 aprsd-3.0.3/docker/
+-rw-r--r--   0 i530566    (501) staff       (20)     1640 2023-04-17 19:01:56.000000 aprsd-3.0.3/docker/Dockerfile
+-rw-r--r--   0 i530566    (501) staff       (20)     2032 2023-04-17 19:01:56.000000 aprsd-3.0.3/docker/Dockerfile-dev
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.134451 aprsd-3.0.3/docker/bin/
+-rwxr-xr-x   0 i530566    (501) staff       (20)      857 2023-04-17 19:30:57.000000 aprsd-3.0.3/docker/bin/listen.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)      812 2022-12-30 15:13:03.000000 aprsd-3.0.3/docker/bin/run.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.0.3/docker/build.sh
+-rw-r--r--   0 i530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.0.3/docker/docker-compose.yml
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.243913 aprsd-3.0.3/docs/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.259216 aprsd-3.0.3/docs/_static/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/_static/.keep
+-rw-r--r--   0 i530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.0.3/docs/_static/aprsd_overview.png
+-rw-r--r--   0 i530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.0.3/docs/_static/aprsd_overview.svg
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.261261 aprsd-3.0.3/docs/_templates/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/_templates/.keep
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.349525 aprsd-3.0.3/docs/apidoc/
+-rw-r--r--   0 i530566    (501) staff       (20)      477 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.clients.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1357 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.cmds.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1044 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.conf.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      468 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.logging.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      969 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.packets.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1523 2023-01-01 19:58:19.000000 aprsd-3.0.3/docs/apidoc/aprsd.plugins.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      447 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.rpc.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1539 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      934 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.threads.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1075 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.utils.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      168 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.web.admin.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      225 2023-01-02 19:13:49.000000 aprsd-3.0.3/docs/apidoc/aprsd.web.rst
+-rw-r--r--   0 i530566    (501) staff       (20)       52 2023-01-01 19:58:20.000000 aprsd-3.0.3/docs/apidoc/modules.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.0.3/docs/aprsd.drawio
+-rw-r--r--   0 i530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.0.3/docs/changelog.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.0.3/docs/clean_docs.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.0.3/docs/conf.py
+-rw-r--r--   0 i530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.0.3/docs/configure.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/index.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/install.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/links.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.0.3/docs/plugin.rst
+-rw-r--r--   0 i530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.0.3/docs/readme.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.0.3/docs/server.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:12.339922 aprsd-3.0.3/examples/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.357473 aprsd-3.0.3/examples/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.3/examples/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)      409 2022-12-20 22:38:48.000000 aprsd-3.0.3/examples/plugins/example_plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.0.3/gray.conf
+-rw-r--r--   0 i530566    (501) staff       (20)      538 2021-08-30 17:18:20.000000 aprsd-3.0.3/pyproject.toml
+-rw-r--r--   0 i530566    (501) staff       (20)      551 2023-01-19 19:14:47.000000 aprsd-3.0.3/requirements.in
+-rw-r--r--   0 i530566    (501) staff       (20)     3401 2023-01-19 19:14:47.000000 aprsd-3.0.3/requirements.txt
+-rw-r--r--   0 i530566    (501) staff       (20)     1246 2023-04-25 18:44:13.406996 aprsd-3.0.3/setup.cfg
+-rw-r--r--   0 i530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.0.3/setup.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.382803 aprsd-3.0.3/tests/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.0.3/tests/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.385445 aprsd-3.0.3/tests/cmds/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.0.3/tests/cmds/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1819 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/cmds/test_send_message.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2505 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/cmds/test_webchat.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1674 2022-12-20 22:38:48.000000 aprsd-3.0.3/tests/fake.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.394355 aprsd-3.0.3/tests/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.0.3/tests/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_fortune.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3793 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_location.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_notify.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_ping.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1696 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_query.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_time.py
+-rw-r--r--   0 i530566    (501) staff       (20)      970 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_version.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7613 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/plugins/test_weather.py
+-rw-r--r--   0 i530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/test_email.py
+-rw-r--r--   0 i530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/test_main.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3070 2022-12-22 17:04:16.000000 aprsd-3.0.3/tests/test_packets.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6486 2022-12-29 19:14:44.000000 aprsd-3.0.3/tests/test_plugin.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-04-25 18:44:13.398513 aprsd-3.0.3/tools/
+-rwxr-xr-x   0 i530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.0.3/tools/fast8.sh
+-rw-r--r--   0 i530566    (501) staff       (20)     2596 2022-12-20 22:38:48.000000 aprsd-3.0.3/tox.ini
```

### Comparing `aprsd-3.0.2/.github/workflows/master-build.yml` & `aprsd-3.0.3/.github/workflows/master-build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/.github/workflows/python.yml` & `aprsd-3.0.3/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/.github/workflows/release_build.yml` & `aprsd-3.0.3/.github/workflows/release_build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/.pre-commit-config.yaml` & `aprsd-3.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/ChangeLog` & `aprsd-3.0.3/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,10 @@
 CHANGES
 =======
 
-v3.0.2
-------
-
-* Import RejectPacket
-
-v3.0.1
-------
-
-* 3.0.1
-* Add support to Reject messages
-* Update Docker builds for 3.0.0
-
-v3.0.0
-------
-
-* Update Changelog for 3.0.0
-* Ensure server command main thread doesn't exit
-* Fixed save directory default
-* Fixed pep8 failure
-* Cleaned up KISS interfaces use of old config
-* reworked usage of importlib.metadata
-* Added new docs files for 3.0.0
-* Removed url option from healthcheck in dev
-* Updated Healthcheck to use rpc to call aprsd
-* Updated docker/bin/run.sh to use new conf
-* Added ObjectPacket
-* Update regex processing and regex for plugins
-* Change ordering of starting up of server command
-* Update documentation and README
 * Decouple admin web interface from server command
 * Dockerfile now produces aprsd.conf
 * Fix some unit tests and loading of CONF w/o file
 * Added missing conf
 * Removed references to old custom config
 * Convert config to oslo\_config
 * Added rain formatting unit tests to WeatherPacket
```

### Comparing `aprsd-3.0.2/INSTALL.txt` & `aprsd-3.0.3/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/LICENSE` & `aprsd-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/Makefile` & `aprsd-3.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/PKG-INFO` & `aprsd-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.0.2
+Version: 3.0.3
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
```

### Comparing `aprsd-3.0.2/README.rst` & `aprsd-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/__init__.py` & `aprsd-3.0.3/aprsd/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/aprsd.py` & `aprsd-3.0.3/aprsd/aprsd.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/cli_helper.py` & `aprsd-3.0.3/aprsd/cli_helper.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/client.py` & `aprsd-3.0.3/aprsd/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,14 +80,16 @@
     @abc.abstractmethod
     def decode_packet(self, *args, **kwargs):
         pass
 
 
 class APRSISClient(Client):
 
+    _client = None
+
     @staticmethod
     def is_enabled():
         # Defaults to True if the enabled flag is non existent
         try:
             return CONF.aprs_network.enabled
         except KeyError:
             return False
@@ -111,14 +113,20 @@
                 raise exception.MissingConfigOptionException(
                     "aprs_network.host is not set.",
                 )
 
             return True
         return True
 
+    def is_alive(self):
+        if self._client:
+            return self._client.is_alive()
+        else:
+            return False
+
     @staticmethod
     def transport():
         return TRANSPORT_APRSIS
 
     def decode_packet(self, *args, **kwargs):
         """APRS lib already decodes this."""
         return core.Packet.factory(args[0])
@@ -153,14 +161,16 @@
         LOG.debug(f"Logging in to APRS-IS with user '{user}'")
         self._client = aprs_client
         return aprs_client
 
 
 class KISSClient(Client):
 
+    _client = None
+
     @staticmethod
     def is_enabled():
         """Return if tcp or serial KISS is enabled."""
         if CONF.kiss_serial.enabled:
             return True
 
         if CONF.kiss_tcp.enabled:
@@ -185,14 +195,20 @@
                     raise exception.MissingConfigOptionException(
                         "kiss_tcp.host is not set.",
                     )
 
             return True
         return False
 
+    def is_alive(self):
+        if self._client:
+            return self._client.is_alive()
+        else:
+            return False
+
     @staticmethod
     def transport():
         if CONF.kiss_serial.enabled:
             return TRANSPORT_SERIALKISS
 
         if CONF.kiss_tcp.enabled:
             return TRANSPORT_TCPKISS
@@ -210,16 +226,16 @@
         # LOG.debug(f"Decoding {msg}")
 
         raw = aprslib.parse(str(frame))
         return core.Packet.factory(raw)
 
     @trace.trace
     def setup_connection(self):
-        client = kiss.KISS3Client()
-        return client
+        self._client = kiss.KISS3Client()
+        return self._client
 
 
 class ClientFactory:
     _instance = None
 
     def __new__(cls, *args, **kwargs):
         """This magic turns this into a singleton."""
@@ -237,15 +253,14 @@
     def create(self, key=None):
         if not key:
             if APRSISClient.is_enabled():
                 key = TRANSPORT_APRSIS
             elif KISSClient.is_enabled():
                 key = KISSClient.transport()
 
-        LOG.debug(f"GET client '{key}'")
         builder = self._builders.get(key)
         if not builder:
             raise ValueError(key)
         return builder()
 
     def is_client_enabled(self):
         """Make sure at least one client is enabled."""
```

### Comparing `aprsd-3.0.2/aprsd/clients/aprsis.py` & `aprsd-3.0.3/aprsd/clients/aprsis.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         LOG.info("Shutdown Aprsdis client.")
 
     @wrapt.synchronized(lock)
     def send(self, packet: core.Packet):
         """Send an APRS Message object."""
         self.sendall(packet.raw)
 
+    def is_alive(self):
+        """If the connection is alive or not."""
+        return self._connected
+
     def _socket_readlines(self, blocking=False):
         """
         Generator for complete lines, received from the server
         """
         try:
             self.sock.setblocking(0)
         except OSError as e:
```

### Comparing `aprsd-3.0.2/aprsd/clients/kiss.py` & `aprsd-3.0.3/aprsd/clients/kiss.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 LOG = logging.getLogger("APRSD")
 
 
 class KISS3Client:
     def __init__(self):
         self.setup()
 
+    def is_alive(self):
+        return True
+
     def setup(self):
         # we can be TCP kiss or Serial kiss
         if CONF.kiss_serial.enabled:
             LOG.debug(
                 "KISS({}) Serial connection to {}".format(
                     kiss.__version__,
                     CONF.kiss_serial.device,
```

### Comparing `aprsd-3.0.2/aprsd/cmds/completion.py` & `aprsd-3.0.3/aprsd/cmds/completion.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/cmds/dev.py` & `aprsd-3.0.3/aprsd/cmds/dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,30 +97,28 @@
         trace.setup_tracing(["method", "api"])
 
     client.Client()
 
     pm = plugin.PluginManager()
     if load_all:
         pm.setup_plugins()
-    else:
-        pm._init()
     obj = pm._create_class(plugin_path, plugin.APRSDPluginBase)
     if not obj:
         click.echo(ctx.get_help())
         click.echo("")
         ctx.fail(f"Failed to create object from plugin path '{plugin_path}'")
         ctx.exit()
 
     # Register the plugin they wanted tested.
     LOG.info(
         "Testing plugin {} Version {}".format(
             obj.__class__, obj.version,
         ),
     )
-    pm._pluggy_pm.register(obj)
+    pm.register_msg(obj)
 
     packet = packets.MessagePacket(
         from_call=fromcall,
         to_call=CONF.callsign,
         msgNo=1,
         message_text=message,
     )
```

### Comparing `aprsd-3.0.2/aprsd/cmds/healthcheck.py` & `aprsd-3.0.3/aprsd/cmds/healthcheck.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/cmds/list_plugins.py` & `aprsd-3.0.3/aprsd/cmds/list_plugins.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/cmds/listen.py` & `aprsd-3.0.3/aprsd/cmds/send_message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,174 @@
-#
-# License GPLv2
-#
-
-# python included libs
-import datetime
 import logging
-import signal
 import sys
 import time
 
+import aprslib
+from aprslib.exceptions import LoginError
 import click
 from oslo_config import cfg
-from rich.console import Console
 
-# local imports here
 import aprsd
-from aprsd import cli_helper, client, packets, stats, threads
+from aprsd import cli_helper, client, packets
+from aprsd import conf  # noqa : F401
 from aprsd.aprsd import cli
-from aprsd.threads import rx
+from aprsd.threads import tx
 
 
-# setup the global logger
-# logging.basicConfig(level=logging.DEBUG) # level=10
-LOG = logging.getLogger("APRSD")
 CONF = cfg.CONF
-console = Console()
-
-
-def signal_handler(sig, frame):
-    threads.APRSDThreadList().stop_all()
-    if "subprocess" not in str(frame):
-        LOG.info(
-            "Ctrl+C, Sending all threads exit! Can take up to 10 seconds {}".format(
-                datetime.datetime.now(),
-            ),
-        )
-        time.sleep(5)
-        LOG.info(stats.APRSDStats())
-
-
-class APRSDListenThread(rx.APRSDRXThread):
-    def __init__(self, packet_queue, packet_filter=None):
-        super().__init__(packet_queue)
-        self.packet_filter = packet_filter
-
-    def process_packet(self, *args, **kwargs):
-        packet = self._client.decode_packet(*args, **kwargs)
-        filters = {
-            packets.Packet.__name__: packets.Packet,
-            packets.AckPacket.__name__: packets.AckPacket,
-            packets.GPSPacket.__name__: packets.GPSPacket,
-            packets.MessagePacket.__name__: packets.MessagePacket,
-            packets.MicEPacket.__name__: packets.MicEPacket,
-            packets.WeatherPacket.__name__: packets.WeatherPacket,
-        }
-
-        if self.packet_filter:
-            filter_class = filters[self.packet_filter]
-            if isinstance(packet, filter_class):
-                packet.log(header="RX")
-        else:
-            packet.log(header="RX")
-
-        packets.PacketList().rx(packet)
+LOG = logging.getLogger("APRSD")
 
 
 @cli.command()
 @cli_helper.add_options(cli_helper.common_options)
 @click.option(
     "--aprs-login",
     envvar="APRS_LOGIN",
     show_envvar=True,
-    help="What callsign to send the message from.",
+    help="What callsign to send the message from. Defaults to config entry.",
 )
 @click.option(
     "--aprs-password",
     envvar="APRS_PASSWORD",
     show_envvar=True,
-    help="the APRS-IS password for APRS_LOGIN",
+    help="the APRS-IS password for APRS_LOGIN. Defaults to config entry.",
 )
 @click.option(
-    "--packet-filter",
-    type=click.Choice(
-        [
-            packets.Packet.__name__,
-            packets.AckPacket.__name__,
-            packets.GPSPacket.__name__,
-            packets.MicEPacket.__name__,
-            packets.MessagePacket.__name__,
-            packets.WeatherPacket.__name__,
-        ],
-        case_sensitive=False,
-    ),
-    help="Filter by packet type",
+    "--no-ack",
+    "-n",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Don't wait for an ack, just sent it to APRS-IS and bail.",
 )
-@click.argument(
-    "filter",
-    nargs=-1,
-    required=True,
+@click.option(
+    "--wait-response",
+    "-w",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Wait for a response to the message?",
 )
+@click.option("--raw", default=None, help="Send a raw message.  Implies --no-ack")
+@click.argument("tocallsign", required=True)
+@click.argument("command", nargs=-1, required=True)
 @click.pass_context
 @cli_helper.process_standard_options
-def listen(
+def send_message(
     ctx,
     aprs_login,
     aprs_password,
-    packet_filter,
-    filter,
+    no_ack,
+    wait_response,
+    raw,
+    tocallsign,
+    command,
 ):
-    """Listen to packets on the APRS-IS Network based on FILTER.
-
-    FILTER is the APRS Filter to use.\n
-     see http://www.aprs-is.net/javAPRSFilter.aspx\n
-    r/lat/lon/dist - Range Filter Pass posits and objects within dist km from lat/lon.\n
-    p/aa/bb/cc... - Prefix Filter Pass traffic with fromCall that start with aa or bb or cc.\n
-    b/call1/call2... - Budlist Filter Pass all traffic from exact call: call1, call2, ... (* wild card allowed) \n
-    o/obj1/obj2... - Object Filter Pass all objects with the exact name of obj1, obj2, ... (* wild card allowed)\n
-
-    """
-    signal.signal(signal.SIGINT, signal_handler)
-    signal.signal(signal.SIGTERM, signal_handler)
+    """Send a message to a callsign via APRS_IS."""
+    global got_ack, got_response
+    quiet = ctx.obj["quiet"]
 
     if not aprs_login:
-        click.echo(ctx.get_help())
-        click.echo("")
-        ctx.fail("Must set --aprs_login or APRS_LOGIN")
-        ctx.exit()
+        if CONF.aprs_network.login == conf.client.DEFAULT_LOGIN:
+            click.echo("Must set --aprs_login or APRS_LOGIN")
+            ctx.exit(-1)
+            return
+        else:
+            aprs_login = CONF.aprs_network.login
 
     if not aprs_password:
-        click.echo(ctx.get_help())
-        click.echo("")
-        ctx.fail("Must set --aprs-password or APRS_PASSWORD")
-        ctx.exit()
-
-    # CONF.aprs_network.login = aprs_login
-    # config["aprs"]["password"] = aprs_password
-
-    LOG.info(f"APRSD Listen Started version: {aprsd.__version__}")
-
-    CONF.log_opt_values(LOG, logging.DEBUG)
-
-    # Try and load saved MsgTrack list
-    LOG.debug("Loading saved MsgTrack object.")
-
-    # Initialize the client factory and create
-    # The correct client object ready for use
-    client.ClientFactory.setup()
-    # Make sure we have 1 client transport enabled
-    if not client.factory.is_client_enabled():
-        LOG.error("No Clients are enabled in config.")
+        LOG.warning(CONF.aprs_network.password)
+        if not CONF.aprs_network.password:
+            click.echo("Must set --aprs-password or APRS_PASSWORD")
+            ctx.exit(-1)
+            return
+        else:
+            aprs_password = CONF.aprs_network.password
+
+    LOG.info(f"APRSD LISTEN Started version: {aprsd.__version__}")
+    if type(command) is tuple:
+        command = " ".join(command)
+    if not quiet:
+        if raw:
+            LOG.info(f"L'{aprs_login}' R'{raw}'")
+        else:
+            LOG.info(f"L'{aprs_login}' To'{tocallsign}' C'{command}'")
+
+    packets.PacketList()
+    packets.WatchList()
+    packets.SeenList()
+
+    got_ack = False
+    got_response = False
+
+    def rx_packet(packet):
+        global got_ack, got_response
+        cl = client.factory.create()
+        packet = cl.decode_packet(packet)
+        packets.PacketList().rx(packet)
+        packet.log("RX")
+        # LOG.debug("Got packet back {}".format(packet))
+        if isinstance(packet, packets.AckPacket):
+            got_ack = True
+        else:
+            got_response = True
+            from_call = packet.from_call
+            our_call = CONF.callsign.lower()
+            tx.send(
+                packets.AckPacket(
+                    from_call=our_call,
+                    to_call=from_call,
+                    msgNo=packet.msgNo,
+                ),
+                direct=True,
+            )
+
+        if got_ack:
+            if wait_response:
+                if got_response:
+                    sys.exit(0)
+            else:
+                sys.exit(0)
+
+    try:
+        client.ClientFactory.setup()
+        client.factory.create().client
+    except LoginError:
         sys.exit(-1)
 
-    # Creates the client object
-    LOG.info("Creating client connection")
-    aprs_client = client.factory.create()
-    LOG.info(aprs_client)
-
-    LOG.debug(f"Filter by '{filter}'")
-    aprs_client.set_filter(filter)
-
-    keepalive = threads.KeepAliveThread()
-    keepalive.start()
-
-    LOG.debug("Create APRSDListenThread")
-    listen_thread = APRSDListenThread(
-        packet_queue=threads.packet_queue,
-        packet_filter=packet_filter,
-    )
-    LOG.debug("Start APRSDListenThread")
-    listen_thread.start()
-    LOG.debug("keepalive Join")
-    keepalive.join()
-    LOG.debug("listen_thread Join")
-    listen_thread.join()
+    # Send a message
+    # then we setup a consumer to rx messages
+    # We should get an ack back as well as a new message
+    # we should bail after we get the ack and send an ack back for the
+    # message
+    if raw:
+        tx.send(
+            packets.Packet(from_call="", to_call="", raw=raw),
+            direct=True,
+        )
+        sys.exit(0)
+    else:
+        tx.send(
+            packets.MessagePacket(
+                from_call=aprs_login,
+                to_call=tocallsign,
+                message_text=command,
+            ),
+            direct=True,
+        )
+
+    if no_ack:
+        sys.exit(0)
+
+    try:
+        # This will register a packet consumer with aprslib
+        # When new packets come in the consumer will process
+        # the packet
+        aprs_client = client.factory.create().client
+        aprs_client.consumer(rx_packet, raw=False)
+    except aprslib.exceptions.ConnectionDrop:
+        LOG.error("Connection dropped, reconnecting")
+        time.sleep(5)
+        # Force the deletion of the client object connected to aprs
+        # This will cause a reconnect, next time client.get_client()
+        # is called
+        aprs_client.reset()
```

### Comparing `aprsd-3.0.2/aprsd/cmds/server.py` & `aprsd-3.0.3/aprsd/cmds/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,22 @@
     # log file output.
     LOG.info("Loading Plugin Manager and registering plugins")
     plugin_manager = plugin.PluginManager()
     plugin_manager.setup_plugins()
 
     # Dump all the config options now.
     CONF.log_opt_values(LOG, logging.DEBUG)
+    message_plugins = plugin_manager.get_message_plugins()
+    watchlist_plugins = plugin_manager.get_watchlist_plugins()
+    LOG.info("Message Plugins enabled and running:")
+    for p in message_plugins:
+        LOG.info(p)
+    LOG.info("Watchlist Plugins enabled and running:")
+    for p in watchlist_plugins:
+        LOG.info(p)
 
     # Make sure we have 1 client transport enabled
     if not client.factory.is_client_enabled():
         LOG.error("No Clients are enabled in config.")
         sys.exit(-1)
 
     if not client.factory.is_client_configured():
```

### Comparing `aprsd-3.0.2/aprsd/cmds/webchat.py` & `aprsd-3.0.3/aprsd/cmds/webchat.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/conf/__init__.py` & `aprsd-3.0.3/aprsd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/conf/client.py` & `aprsd-3.0.3/aprsd/conf/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/conf/common.py` & `aprsd-3.0.3/aprsd/conf/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,14 +43,28 @@
         help="Enable code tracing",
     ),
     cfg.StrOpt(
         "units",
         default="imperial",
         help="Units for display, imperial or metric",
     ),
+    cfg.IntOpt(
+        "ack_rate_limit_period",
+        default=1,
+        help="The wait period in seconds per Ack packet being sent."
+             "1 means 1 ack packet per second allowed."
+             "2 means 1 pack packet every 2 seconds allowed",
+    ),
+    cfg.IntOpt(
+        "msg_rate_limit_period",
+        default=2,
+        help="Wait period in seconds per non AckPacket being sent."
+             "2 means 1 packet every 2 seconds allowed."
+             "5 means 1 pack packet every 5 seconds allowed",
+    ),
 ]
 
 watch_list_opts = [
     cfg.BoolOpt(
         "enabled",
         default=False,
         help="Enable the watch list feature.  Still have to enable "
```

### Comparing `aprsd-3.0.2/aprsd/conf/log.py` & `aprsd-3.0.3/aprsd/conf/log.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/conf/opts.py` & `aprsd-3.0.3/aprsd/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/conf/plugin_common.py` & `aprsd-3.0.3/aprsd/conf/plugin_common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/conf/plugin_email.py` & `aprsd-3.0.3/aprsd/conf/plugin_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/flask.py` & `aprsd-3.0.3/aprsd/flask.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/logging/log.py` & `aprsd-3.0.3/aprsd/logging/log.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/logging/rich.py` & `aprsd-3.0.3/aprsd/logging/rich.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/packets/core.py` & `aprsd-3.0.3/aprsd/packets/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,24 @@
         return re.sub("fuck|shit|cunt|piss|cock|bitch", "****", message)
 
     def __str__(self):
         """Show the raw version of the packet"""
         self.prepare()
         return self.raw
 
+    def __repr__(self):
+        """Build the repr version of the packet."""
+        repr = (
+            f"{self.__class__.__name__}:"
+            f" From: {self.from_call}  "
+            " To: "
+        )
+
+        return repr
+
 
 @dataclass
 class PathPacket(Packet):
     path: List[str] = field(default_factory=list)
     via: str = None
 
     def _build_raw(self):
```

### Comparing `aprsd-3.0.2/aprsd/packets/packet_list.py` & `aprsd-3.0.3/aprsd/packets/packet_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/packets/seen_list.py` & `aprsd-3.0.3/aprsd/packets/seen_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/packets/tracker.py` & `aprsd-3.0.3/aprsd/packets/tracker.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/packets/watch_list.py` & `aprsd-3.0.3/aprsd/packets/watch_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugin.py` & `aprsd-3.0.3/aprsd/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,21 +203,22 @@
 
     def setup(self):
         """Do any plugin setup here."""
         self.enabled = True
 
     @hookimpl
     def filter(self, packet: packets.core.MessagePacket):
+        LOG.info(f"{self.__class__.__name__} called")
         if not self.enabled:
             result = f"{self.__class__.__name__} isn't enabled"
             LOG.warning(result)
             return result
 
         if not isinstance(packet, packets.core.MessagePacket):
-            LOG.warning(f"Got a {packet.__class__.__name__} ignoring")
+            LOG.warning(f"{self.__class__.__name__} Got a {packet.__class__.__name__} ignoring")
             return packets.NULL_MESSAGE
 
         result = None
 
         message = packet.message_text
         tocall = packet.to_call
 
@@ -320,32 +321,25 @@
     _instance = None
 
     # the pluggy PluginManager for all Message plugins
     _pluggy_pm = None
     # the pluggy PluginManager for all WatchList plugins
     _watchlist_pm = None
 
-    # aprsd config dict
-    config = None
-
     lock = None
 
     def __new__(cls, *args, **kwargs):
         """This magic turns this into a singleton."""
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             # Put any initialization here.
             cls._instance.lock = threading.Lock()
+            cls._instance._init()
         return cls._instance
 
-    def __init__(self, config=None):
-        self.obj_list = []
-        if config:
-            self.config = config
-
     def _init(self):
         self._pluggy_pm = pluggy.PluginManager("aprsd")
         self._pluggy_pm.add_hookspecs(APRSDPluginSpec)
         # For the watchlist plugins
         self._watchlist_pm = pluggy.PluginManager("aprsd")
         self._watchlist_pm.add_hookspecs(APRSDPluginSpec)
 
@@ -418,58 +412,69 @@
                                 plugin_name,
                                 plugin_obj.version,
                             ),
                         )
                         self._watchlist_pm.register(plugin_obj)
                     else:
                         LOG.warning(f"Plugin {plugin_obj.__class__.__name__} is disabled")
-                else:
+                elif isinstance(plugin_obj, APRSDRegexCommandPluginBase):
                     if plugin_obj.enabled:
                         LOG.info(
-                            "Registering plugin '{}'({}) -- {}".format(
+                            "Registering Regex plugin '{}'({}) -- {}".format(
                                 plugin_name,
                                 plugin_obj.version,
                                 plugin_obj.command_regex,
                             ),
                         )
                         self._pluggy_pm.register(plugin_obj)
                     else:
                         LOG.warning(f"Plugin {plugin_obj.__class__.__name__} is disabled")
+                elif isinstance(plugin_obj, APRSDPluginBase):
+                    if plugin_obj.enabled:
+                        LOG.info(
+                            "Registering Base plugin '{}'({})".format(
+                                plugin_name,
+                                plugin_obj.version,
+                            ),
+                        )
+                        self._pluggy_pm.register(plugin_obj)
+                    else:
+                        LOG.warning(f"Plugin {plugin_obj.__class__.__name__} is disabled")
         except Exception as ex:
             LOG.error(f"Couldn't load plugin '{plugin_name}'")
             LOG.exception(ex)
 
     def reload_plugins(self):
         with self.lock:
             del self._pluggy_pm
             self.setup_plugins()
 
-    def setup_plugins(self):
+    def setup_plugins(self, load_help_plugin=True):
         """Create the plugin manager and register plugins."""
 
         LOG.info("Loading APRSD Plugins")
-        self._init()
         # Help plugin is always enabled.
-        _help = HelpPlugin()
-        self._pluggy_pm.register(_help)
+        if load_help_plugin:
+            _help = HelpPlugin()
+            self._pluggy_pm.register(_help)
 
         enabled_plugins = CONF.enabled_plugins
         if enabled_plugins:
             for p_name in enabled_plugins:
                 self._load_plugin(p_name)
         else:
             # Enabled plugins isn't set, so we default to loading all of
             # the core plugins.
             for p_name in CORE_MESSAGE_PLUGINS:
                 self._load_plugin(p_name)
 
         LOG.info("Completed Plugin Loading.")
 
     def run(self, packet: packets.core.MessagePacket):
-        """Execute all the pluguns run method."""
+        """Execute all the plugins run method."""
         with self.lock:
             return self._pluggy_pm.hook.filter(packet=packet)
 
     def run_watchlist(self, packet: packets.core.Packet):
         with self.lock:
             return self._watchlist_pm.hook.filter(packet=packet)
 
@@ -478,15 +483,16 @@
         with self.lock:
             for p in self.get_plugins():
                 if hasattr(p, "stop_threads"):
                     p.stop_threads()
 
     def register_msg(self, obj):
         """Register the plugin."""
-        self._pluggy_pm.register(obj)
+        with self.lock:
+            self._pluggy_pm.register(obj)
 
     def get_plugins(self):
         plugin_list = []
         if self._pluggy_pm:
             for plug in self._pluggy_pm.get_plugins():
                 plugin_list.append(plug)
         if self._watchlist_pm:
```

### Comparing `aprsd-3.0.2/aprsd/plugin_utils.py` & `aprsd-3.0.3/aprsd/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/email.py` & `aprsd-3.0.3/aprsd/plugins/email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/fortune.py` & `aprsd-3.0.3/aprsd/plugins/fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/location.py` & `aprsd-3.0.3/aprsd/plugins/location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/notify.py` & `aprsd-3.0.3/aprsd/plugins/notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/ping.py` & `aprsd-3.0.3/aprsd/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/query.py` & `aprsd-3.0.3/aprsd/plugins/query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/time.py` & `aprsd-3.0.3/aprsd/plugins/time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/version.py` & `aprsd-3.0.3/aprsd/plugins/version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/plugins/weather.py` & `aprsd-3.0.3/aprsd/plugins/weather.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/rpc/client.py` & `aprsd-3.0.3/aprsd/rpc/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/rpc/server.py` & `aprsd-3.0.3/aprsd/rpc/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         LOG.info("Disconnected")
         self._conn = None
 
     @rpyc.exposed
     def get_stats(self):
         stat = stats.APRSDStats()
         stats_dict = stat.stats()
+        LOG.debug(stats_dict)
         return json.dumps(stats_dict, indent=4, sort_keys=True, default=str)
 
     @rpyc.exposed
     def get_stats_obj(self):
         return stats.APRSDStats()
 
     @rpyc.exposed
```

### Comparing `aprsd-3.0.2/aprsd/stats.py` & `aprsd-3.0.3/aprsd/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,15 @@
                 "enabled": CONF.email_plugin.enabled,
                 "sent": int(self._email_tx),
                 "received": int(self._email_rx),
                 "thread_last_update": last_update,
             },
             "plugins": plugin_stats,
         }
+        LOG.debug(f"STATS = {stats}")
         return stats
 
     def __str__(self):
         pl = packets.PacketList()
         return (
             "Uptime:{} Msgs TX:{} RX:{} "
             "ACK: TX:{} RX:{} "
```

### Comparing `aprsd-3.0.2/aprsd/threads/aprsd.py` & `aprsd-3.0.3/aprsd/threads/aprsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,18 @@
     @abc.abstractmethod
     def loop(self):
         pass
 
     def _cleanup(self):
         """Add code to subclass to do any cleanup"""
 
+    def __str__(self):
+        out = f"Thread <{self.__class__.__name__}({self.name}) Alive? {self.is_alive()}>"
+        return out
+
     def run(self):
         LOG.debug("Starting")
         while not self._should_quit():
             can_loop = self.loop()
             if not can_loop:
                 self.stop()
         self._cleanup()
```

### Comparing `aprsd-3.0.2/aprsd/threads/keep_alive.py` & `aprsd-3.0.3/aprsd/threads/keep_alive.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,30 +60,43 @@
                 last_msg_time,
                 email_thread_time,
                 utils.human_size(current),
                 utils.human_size(peak),
                 len(thread_list),
             )
             LOG.info(keepalive)
+            thread_out = []
+            for thread in thread_list.threads_list:
+                alive = thread.is_alive()
+                thread_out.append(f"{thread.__class__.__name__}:{alive}")
+                if not alive:
+                    LOG.error(f"Thread {thread}")
+            LOG.info(",".join(thread_out))
 
-            # See if we should reset the aprs-is client
-            # Due to losing a keepalive from them
-            delta_dict = utils.parse_delta_str(last_msg_time)
-            delta = datetime.timedelta(**delta_dict)
+            # check the APRS connection
+            cl = client.factory.create()
+            if not cl.is_alive():
+                LOG.error(f"{cl.__class__.__name__} is not alive!!! Resetting")
+                client.factory.create().reset()
+            else:
+                # See if we should reset the aprs-is client
+                # Due to losing a keepalive from them
+                delta_dict = utils.parse_delta_str(last_msg_time)
+                delta = datetime.timedelta(**delta_dict)
 
-            if delta > self.max_delta:
-                #  We haven't gotten a keepalive from aprs-is in a while
-                # reset the connection.a
-                if not client.KISSClient.is_enabled():
-                    LOG.warning(f"Resetting connection to APRS-IS {delta}")
-                    client.factory.create().reset()
+                if delta > self.max_delta:
+                    #  We haven't gotten a keepalive from aprs-is in a while
+                    # reset the connection.a
+                    if not client.KISSClient.is_enabled():
+                        LOG.warning(f"Resetting connection to APRS-IS {delta}")
+                        client.factory.create().reset()
 
-            # Check version every hour
+            # Check version every day
             delta = now - self.checker_time
-            if delta > datetime.timedelta(hours=1):
+            if delta > datetime.timedelta(hours=24):
                 self.checker_time = now
                 level, msg = utils._check_version()
                 if level:
                     LOG.warning(msg)
         self.cntr += 1
         time.sleep(1)
         return True
```

### Comparing `aprsd-3.0.2/aprsd/threads/log_monitor.py` & `aprsd-3.0.3/aprsd/threads/log_monitor.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/threads/rx.py` & `aprsd-3.0.3/aprsd/threads/rx.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 class APRSDPluginRXThread(APRSDRXThread):
     """Process received packets.
 
     This is the main APRSD Server command thread that
     receives packets from APRIS and then sends them for
     processing in the PluginProcessPacketThread.
     """
+
     def process_packet(self, *args, **kwargs):
         packet = self._client.decode_packet(*args, **kwargs)
         # LOG.debug(raw)
         packet.log(header="RX")
         packets.PacketList().rx(packet)
         self.packet_queue.put(packet)
```

### Comparing `aprsd-3.0.2/aprsd/threads/tx.py` & `aprsd-3.0.3/aprsd/threads/tx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,66 @@
 import datetime
 import logging
 import time
 
+from oslo_config import cfg
+from ratelimiter import RateLimiter
+
 from aprsd import client
 from aprsd import threads as aprsd_threads
 from aprsd.packets import core, tracker
 
 
+CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
+def limited(until):
+    duration = int(round(until - time.time()))
+    LOG.debug(f"Rate limited, sleeping for {duration:d} seconds")
+
+
 def send(packet: core.Packet, direct=False, aprs_client=None):
     """Send a packet either in a thread or directly to the client."""
     # prepare the packet for sending.
     # This constructs the packet.raw
     packet.prepare()
+    if isinstance(packet, core.AckPacket):
+        _send_ack(packet, direct=direct, aprs_client=aprs_client)
+    else:
+        _send_packet(packet, direct=direct, aprs_client=aprs_client)
+
+
+@RateLimiter(max_calls=1, period=CONF.msg_rate_limit_period, callback=limited)
+def _send_packet(packet: core.Packet, direct=False, aprs_client=None):
     if not direct:
-        if isinstance(packet, core.AckPacket):
-            thread = SendAckThread(packet=packet)
-        else:
-            thread = SendPacketThread(packet=packet)
+        thread = SendPacketThread(packet=packet)
         thread.start()
     else:
-        if aprs_client:
-            cl = aprs_client
-        else:
-            cl = client.factory.create()
-
-        packet.update_timestamp()
-        packet.log(header="TX")
-        cl.send(packet)
+        _send_direct(packet, aprs_client=aprs_client)
+
+
+@RateLimiter(max_calls=1, period=CONF.ack_rate_limit_period, callback=limited)
+def _send_ack(packet: core.AckPacket, direct=False, aprs_client=None):
+    if not direct:
+        thread = SendAckThread(packet=packet)
+        thread.start()
+    else:
+        _send_direct(packet, aprs_client=aprs_client)
+
+
+def _send_direct(packet, aprs_client=None):
+    if aprs_client:
+        cl = aprs_client
+    else:
+        cl = client.factory.create()
+
+    packet.update_timestamp()
+    packet.log(header="TX")
+    cl.send(packet)
 
 
 class SendPacketThread(aprsd_threads.APRSDThread):
     loop_count: int = 1
 
     def __init__(self, packet):
         self.packet = packet
```

### Comparing `aprsd-3.0.2/aprsd/utils/__init__.py` & `aprsd-3.0.3/aprsd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/utils/counter.py` & `aprsd-3.0.3/aprsd/utils/counter.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/utils/fuzzyclock.py` & `aprsd-3.0.3/aprsd/utils/fuzzyclock.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/utils/json.py` & `aprsd-3.0.3/aprsd/utils/json.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/utils/objectstore.py` & `aprsd-3.0.3/aprsd/utils/objectstore.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/utils/ring_buffer.py` & `aprsd-3.0.3/aprsd/utils/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/utils/trace.py` & `aprsd-3.0.3/aprsd/utils/trace.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/css/index.css` & `aprsd-3.0.3/aprsd/web/admin/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/css/prism.css` & `aprsd-3.0.3/aprsd/web/admin/static/css/prism.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/css/tabs.css` & `aprsd-3.0.3/aprsd/web/admin/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/images/Untitled.png` & `aprsd-3.0.3/aprsd/web/admin/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-16-0.png` & `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-16-1.png` & `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-64-0.png` & `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-64-1.png` & `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/images/aprs-symbols-64-2.png` & `aprsd-3.0.3/aprsd/web/admin/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/js/charts.js` & `aprsd-3.0.3/aprsd/web/admin/static/js/charts.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/js/logs.js` & `aprsd-3.0.3/aprsd/web/admin/static/js/logs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/js/main.js` & `aprsd-3.0.3/aprsd/web/admin/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/js/prism.js` & `aprsd-3.0.3/aprsd/web/admin/static/js/prism.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/js/send-message.js` & `aprsd-3.0.3/aprsd/web/admin/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/js/tabs.js` & `aprsd-3.0.3/aprsd/web/admin/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.0.3/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/admin/templates/index.html` & `aprsd-3.0.3/aprsd/web/admin/templates/index.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/css/index.css` & `aprsd-3.0.3/aprsd/web/chat/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/css/style.css.map` & `aprsd-3.0.3/aprsd/web/chat/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/css/tabs.css` & `aprsd-3.0.3/aprsd/web/chat/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/images/Untitled.png` & `aprsd-3.0.3/aprsd/web/chat/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-16-0.png` & `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-16-1.png` & `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-64-0.png` & `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-64-1.png` & `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/images/aprs-symbols-64-2.png` & `aprsd-3.0.3/aprsd/web/chat/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/js/gps.js` & `aprsd-3.0.3/aprsd/web/chat/static/js/gps.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/js/main.js` & `aprsd-3.0.3/aprsd/web/chat/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/js/send-message-mobile.js` & `aprsd-3.0.3/aprsd/web/chat/static/js/send-message-mobile.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/js/send-message.js` & `aprsd-3.0.3/aprsd/web/chat/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/js/tabs.js` & `aprsd-3.0.3/aprsd/web/chat/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.0.3/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/templates/index.html` & `aprsd-3.0.3/aprsd/web/chat/templates/index.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd/web/chat/templates/mobile.html` & `aprsd-3.0.3/aprsd/web/chat/templates/mobile.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd-lnav.json` & `aprsd-3.0.3/aprsd-lnav.json`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/aprsd.egg-info/PKG-INFO` & `aprsd-3.0.3/aprsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.0.2
+Version: 3.0.3
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
```

### Comparing `aprsd-3.0.2/aprsd.egg-info/SOURCES.txt` & `aprsd-3.0.3/aprsd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
 aprsd/web/chat/templates/index.html
 aprsd/web/chat/templates/mobile.html
 docker/Dockerfile
 docker/Dockerfile-dev
 docker/build.sh
 docker/docker-compose.yml
+docker/bin/listen.sh
 docker/bin/run.sh
 docs/aprsd.drawio
 docs/changelog.rst
 docs/clean_docs.py
 docs/conf.py
 docs/configure.rst
 docs/index.rst
```

### Comparing `aprsd-3.0.2/aprsd.egg-info/requires.txt` & `aprsd-3.0.3/aprsd.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,61 +2,62 @@
 attrs==22.2.0
 ax253==0.1.5.post1
 beautifulsoup4==4.11.1
 bidict==0.22.1
 bitarray==2.6.2
 certifi==2022.12.7
 cffi==1.15.1
-charset-normalizer==2.1.1
+charset-normalizer==3.0.1
 click==8.1.3
 click-completion==0.5.2
 commonmark==0.9.1
 cryptography==38.0.1
 dacite2==2.0.0
 dataclasses==0.6
 debtcollector==2.5.0
-dnspython==2.2.1
-eventlet==0.33.2
+dnspython==2.3.0
+eventlet==0.33.3
 flask==2.1.2
 flask-classful==0.14.2
 flask-httpauth==4.7.0
 flask-socketio==5.3.2
 greenlet==2.0.1
 idna==3.4
 imapclient==2.3.1
 importlib-metadata==6.0.0
 itsdangerous==2.1.2
 jinja2==3.1.2
 kiss3==8.0.0
-markupsafe==2.1.1
+markupsafe==2.1.2
 netaddr==0.8.0
 oslo-config==9.1.0
 oslo-i18n==5.1.0
-pbr==5.11.0
+pbr==5.11.1
 pluggy==1.0.0
 plumbum==1.8.1
 pycparser==2.21
 pygments==2.14.0
 pyopenssl==23.0.0
 pyserial==3.5
 pyserial-asyncio==0.6
 python-engineio==4.3.4
 python-socketio==5.7.2
-pytz==2022.7
+pytz==2022.7.1
 pyyaml==6.0
-requests==2.28.1
+ratelimiter==1.2.0.post0
+requests==2.28.2
 rfc3986==2.0.0
 rich==12.6.0
 rpyc==5.3.0
 shellingham==1.5.0.post1
 six==1.16.0
 soupsieve==2.3.2.post1
 stevedore==4.1.1
 tabulate==0.9.0
 thesmuggler==1.0.1
 ua-parser==0.16.1
 update-checker==0.18.0
-urllib3==1.26.13
+urllib3==1.26.14
 user-agents==2.2.0
 werkzeug==2.1.2
 wrapt==1.14.1
 zipp==3.11.0
```

### Comparing `aprsd-3.0.2/dev-requirements.txt` & `aprsd-3.0.3/dev-requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --annotation-style=line --resolver=backtracking dev-requirements.in
 #
 add-trailing-comma==2.4.0  # via gray
-alabaster==0.7.12         # via sphinx
+alabaster==0.7.13         # via sphinx
 attrs==22.2.0             # via jsonschema, pytest
 autoflake==1.5.3          # via gray
 babel==2.11.0             # via sphinx
 black==22.12.0            # via gray
-build==0.9.0              # via pip-tools
-cachetools==5.2.0         # via tox
+build==0.10.0             # via pip-tools
+cachetools==5.2.1         # via tox
 certifi==2022.12.7        # via requests
 cfgv==3.3.1               # via pre-commit
 chardet==5.1.0            # via tox
-charset-normalizer==2.1.1  # via requests
+charset-normalizer==3.0.1  # via requests
 click==8.1.3              # via black, pip-tools
 colorama==0.4.6           # via tox
 commonmark==0.9.1         # via rich
 configargparse==1.5.3     # via gray
-coverage[toml]==7.0.3     # via pytest-cov
+coverage[toml]==7.0.5     # via pytest-cov
 distlib==0.3.6            # via virtualenv
 docutils==0.19            # via sphinx
 exceptiongroup==1.1.0     # via pytest
 filelock==3.9.0           # via tox, virtualenv
 fixit==0.1.4              # via gray
 flake8==6.0.0             # via -r dev-requirements.in, fixit, pep8-naming
 gray==0.13.0              # via -r dev-requirements.in
-identify==2.5.12          # via pre-commit
+identify==2.5.13          # via pre-commit
 idna==3.4                 # via requests
 imagesize==1.4.1          # via sphinx
 importlib-metadata==6.0.0  # via sphinx
 importlib-resources==5.10.2  # via fixit
 iniconfig==2.0.0          # via pytest
 isort==5.11.4             # via -r dev-requirements.in, gray
 jinja2==3.1.2             # via sphinx
 jsonschema==4.17.3        # via fixit
 libcst==0.4.9             # via fixit
-markupsafe==2.1.1         # via jinja2
+markupsafe==2.1.2         # via jinja2
 mccabe==0.7.0             # via flake8
 mypy==0.991               # via -r dev-requirements.in
 mypy-extensions==0.4.3    # via black, mypy, typing-inspect
 nodeenv==1.7.0            # via pre-commit
-packaging==22.0           # via build, pyproject-api, pytest, sphinx, tox
+packaging==23.0           # via build, pyproject-api, pytest, sphinx, tox
 pathspec==0.10.3          # via black
-pep517==0.13.0            # via build
 pep8-naming==0.13.3       # via -r dev-requirements.in
 pip-tools==6.12.1         # via -r dev-requirements.in
 platformdirs==2.6.2       # via black, tox, virtualenv
 pluggy==1.0.0             # via pytest, tox
 pre-commit==2.21.0        # via -r dev-requirements.in
 pycodestyle==2.10.0       # via flake8
 pyflakes==3.0.1           # via autoflake, flake8
 pygments==2.14.0          # via rich, sphinx
-pyproject-api==1.4.0      # via tox
+pyproject-api==1.5.0      # via tox
+pyproject-hooks==1.0.0    # via build
 pyrsistent==0.19.3        # via jsonschema
-pytest==7.2.0             # via -r dev-requirements.in, pytest-cov
+pytest==7.2.1             # via -r dev-requirements.in, pytest-cov
 pytest-cov==4.0.0         # via -r dev-requirements.in
-pytz==2022.7              # via babel
+pytz==2022.7.1            # via babel
 pyupgrade==3.3.1          # via gray
 pyyaml==6.0               # via fixit, libcst, pre-commit
-requests==2.28.1          # via sphinx
+requests==2.28.2          # via sphinx
 rich==12.6.0              # via gray
 snowballstemmer==2.2.0    # via sphinx
-sphinx==6.1.2             # via -r dev-requirements.in
-sphinxcontrib-applehelp==1.0.2  # via sphinx
+sphinx==6.1.3             # via -r dev-requirements.in
+sphinxcontrib-applehelp==1.0.3  # via sphinx
 sphinxcontrib-devhelp==1.0.2  # via sphinx
 sphinxcontrib-htmlhelp==2.0.0  # via sphinx
 sphinxcontrib-jsmath==1.0.1  # via sphinx
 sphinxcontrib-qthelp==1.0.3  # via sphinx
 sphinxcontrib-serializinghtml==1.1.5  # via sphinx
 tokenize-rt==5.0.0        # via add-trailing-comma, pyupgrade
 toml==0.10.2              # via autoflake
-tomli==2.0.1              # via black, build, coverage, mypy, pep517, pyproject-api, pytest, tox
-tox==4.2.6                # via -r dev-requirements.in
+tomli==2.0.1              # via black, build, coverage, mypy, pyproject-api, pyproject-hooks, pytest, tox
+tox==4.3.5                # via -r dev-requirements.in
 typing-extensions==4.4.0  # via black, libcst, mypy, typing-inspect
 typing-inspect==0.8.0     # via libcst
 unify==0.5                # via gray
 untokenize==0.1.1         # via unify
-urllib3==1.26.13          # via requests
+urllib3==1.26.14          # via requests
 virtualenv==20.17.1       # via pre-commit, tox
 wheel==0.38.4             # via pip-tools
 zipp==3.11.0              # via importlib-metadata, importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `aprsd-3.0.2/docker/Dockerfile` & `aprsd-3.0.3/docker/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -33,26 +33,27 @@
 # 32-bit architectures within QEMU running on a 64-bit host (issue #30).
 RUN if [ "${BUILDX_QEMU_ENV}" = "true" -a "$(getconf LONG_BIT)" = "32" ]; then \
         pip3 install -U cryptography==3.3.2; \
     else \
         pip3 install cryptography ;\
     fi
 
-# Install aprsd
-RUN pip3 install aprsd==$APRSD_PIP_VERSION
-
 # Ensure /config is there with a default config file
 USER root
+# Install aprsd
+RUN pip3 install aprsd==$APRSD_PIP_VERSION
 RUN mkdir -p /config
 RUN aprsd sample-config > /config/aprsd.conf
 RUN chown -R $APRS_USER:$APRS_USER /config
+RUN chown -R $APRS_USER:$APRS_USER $HOME
 
 # override this to run another configuration
 ENV CONF default
 VOLUME ["/config", "/plugins"]
 
 USER $APRS_USER
 ADD bin/run.sh /usr/local/bin
+ADD bin/listen.sh /usr/local/bin
 ENTRYPOINT ["/usr/local/bin/run.sh"]
 
 HEALTHCHECK --interval=5m --timeout=12s --start-period=30s \
     CMD aprsd healthcheck --config /config/aprsd.conf
```

### Comparing `aprsd-3.0.2/docker/Dockerfile-dev` & `aprsd-3.0.3/docker/Dockerfile-dev`

 * *Files 2% similar despite different names*

```diff
@@ -60,11 +60,12 @@
 
 # override this to run another configuration
 ENV CONF default
 USER $APRS_USER
 VOLUME ["/config", "/plugins"]
 
 ADD bin/run.sh $HOME/
+ADD bin/listen.sh $HOME/
 ENTRYPOINT ["/home/aprs/run.sh"]
 
 HEALTHCHECK --interval=5m --timeout=12s --start-period=30s \
     CMD aprsd healthcheck --config /config/aprsd.conf
```

### Comparing `aprsd-3.0.2/docker/bin/run.sh` & `aprsd-3.0.3/docker/bin/run.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docker/build.sh` & `aprsd-3.0.3/docker/build.sh`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 OPTIONS:
    -h      Show help
    -t      The tag/version (${TAG}) (default = master)
    -d      Use Dockerfile-dev for a git clone build
    -b      Branch to use (default = master)
    -r      Destroy and rebuild the buildx environment
+   -v      aprsd version to build
 EOF
 }
 
 
 ALL_PLATFORMS=0
 DEV=0
 REBUILD_BUILDX=0
@@ -58,16 +59,17 @@
            ;;
     esac
 done
 
 
 if [ $ALL_PLATFORMS -eq 1 ]
 then
-    PLATFORMS="linux/arm/v7,linux/arm64,linux/amd64"
+    PLATFORMS="linux/arm64,linux/amd64"
     #PLATFORMS="linux/arm/v7,linux/arm/v6,linux/amd64"
+    #PLATFORMS="linux/arm64"
 else
     PLATFORMS="linux/amd64"
 fi
 
 
 
 if [ $REBUILD_BUILDX -eq 1 ]
@@ -83,15 +85,15 @@
 fi
 
 if [ $DEV -eq 1 ]
 then
     echo "Build -DEV- with tag=${TAG} BRANCH=${BRANCH} platforms?=${PLATFORMS}"
     # Use this script to locally build the docker image
     docker buildx build --push --platform $PLATFORMS \
-        -t harbor.hemna.com/hemna6969/aprsd:$TAG \
+        -t hemna6969/aprsd:$TAG \
         -f Dockerfile-dev --build-arg branch=$BRANCH \
         --build-arg BUILDX_QEMU_ENV=true \
         --no-cache .
 else
     # Use this script to locally build the docker image
     echo "Build with tag=${TAG} BRANCH=${BRANCH} dev?=${DEV} platforms?=${PLATFORMS} VERSION=${VERSION}"
     docker buildx build --push --platform $PLATFORMS \
```

### Comparing `aprsd-3.0.2/docs/_static/aprsd_overview.png` & `aprsd-3.0.3/docs/_static/aprsd_overview.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/_static/aprsd_overview.svg` & `aprsd-3.0.3/docs/_static/aprsd_overview.svg`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/apidoc/aprsd.cmds.rst` & `aprsd-3.0.3/docs/apidoc/aprsd.cmds.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/apidoc/aprsd.conf.rst` & `aprsd-3.0.3/docs/apidoc/aprsd.conf.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/apidoc/aprsd.packets.rst` & `aprsd-3.0.3/docs/apidoc/aprsd.packets.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/apidoc/aprsd.plugins.rst` & `aprsd-3.0.3/docs/apidoc/aprsd.plugins.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/apidoc/aprsd.rst` & `aprsd-3.0.3/docs/apidoc/aprsd.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/apidoc/aprsd.threads.rst` & `aprsd-3.0.3/docs/apidoc/aprsd.threads.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/apidoc/aprsd.utils.rst` & `aprsd-3.0.3/docs/apidoc/aprsd.utils.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/aprsd.drawio` & `aprsd-3.0.3/docs/aprsd.drawio`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/changelog.rst` & `aprsd-3.0.3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,53 @@
 CHANGES
 =======
 
+v3.0.3
+------
+
+* cleanup some debug messages
+* Fixed loading of plugins for server
+* Don't load help plugin for listen command
+* Added listen args
+* Change listen command plugins
+* Added listen.sh for docker
+* Update Listen command
+* Update Dockerfile
+* Add ratelimiting for acks and other packets
+
+v3.0.2
+------
+
+* Update Changelog for 3.0.2
+* Import RejectPacket
+
+v3.0.1
+------
+
+* 3.0.1
+* Add support to Reject messages
+* Update Docker builds for 3.0.0
+
+v3.0.0
+------
+
+* Update Changelog for 3.0.0
+* Ensure server command main thread doesn't exit
+* Fixed save directory default
+* Fixed pep8 failure
+* Cleaned up KISS interfaces use of old config
+* reworked usage of importlib.metadata
+* Added new docs files for 3.0.0
+* Removed url option from healthcheck in dev
+* Updated Healthcheck to use rpc to call aprsd
+* Updated docker/bin/run.sh to use new conf
+* Added ObjectPacket
+* Update regex processing and regex for plugins
+* Change ordering of starting up of server command
+* Update documentation and README
 * Decouple admin web interface from server command
 * Dockerfile now produces aprsd.conf
 * Fix some unit tests and loading of CONF w/o file
 * Added missing conf
 * Removed references to old custom config
 * Convert config to oslo\_config
 * Added rain formatting unit tests to WeatherPacket
```

### Comparing `aprsd-3.0.2/docs/clean_docs.py` & `aprsd-3.0.3/docs/clean_docs.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/conf.py` & `aprsd-3.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/configure.rst` & `aprsd-3.0.3/docs/configure.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/index.rst` & `aprsd-3.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/install.rst` & `aprsd-3.0.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/links.rst` & `aprsd-3.0.3/docs/links.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/plugin.rst` & `aprsd-3.0.3/docs/plugin.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/readme.rst` & `aprsd-3.0.3/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/docs/server.rst` & `aprsd-3.0.3/docs/server.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/pyproject.toml` & `aprsd-3.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/requirements.in` & `aprsd-3.0.3/requirements.in`

 * *Files 20% similar despite different names*

```diff
@@ -32,7 +32,8 @@
 dacite2
 oslo.config
 rpyc
 # Pin this here so it doesn't require a compile on
 # raspi
 cryptography==38.0.1
 shellingham==1.5.0.post1
+ratelimiter
```

### Comparing `aprsd-3.0.2/requirements.txt` & `aprsd-3.0.3/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,61 +8,62 @@
 attrs==22.2.0             # via -r requirements.in, ax253, kiss3
 ax253==0.1.5.post1        # via kiss3
 beautifulsoup4==4.11.1    # via -r requirements.in
 bidict==0.22.1            # via python-socketio
 bitarray==2.6.2           # via ax253, kiss3
 certifi==2022.12.7        # via requests
 cffi==1.15.1              # via cryptography
-charset-normalizer==2.1.1  # via requests
+charset-normalizer==3.0.1  # via requests
 click==8.1.3              # via -r requirements.in, click-completion, flask
 click-completion==0.5.2   # via -r requirements.in
 commonmark==0.9.1         # via rich
 cryptography==38.0.1      # via -r requirements.in, pyopenssl
 dacite2==2.0.0            # via -r requirements.in
 dataclasses==0.6          # via -r requirements.in
 debtcollector==2.5.0      # via oslo-config
-dnspython==2.2.1          # via eventlet
-eventlet==0.33.2          # via -r requirements.in
+dnspython==2.3.0          # via eventlet
+eventlet==0.33.3          # via -r requirements.in
 flask==2.1.2              # via -r requirements.in, flask-classful, flask-httpauth, flask-socketio
 flask-classful==0.14.2    # via -r requirements.in
 flask-httpauth==4.7.0     # via -r requirements.in
 flask-socketio==5.3.2     # via -r requirements.in
 greenlet==2.0.1           # via eventlet
 idna==3.4                 # via requests
 imapclient==2.3.1         # via -r requirements.in
 importlib-metadata==6.0.0  # via ax253, flask, kiss3
 itsdangerous==2.1.2       # via flask
 jinja2==3.1.2             # via click-completion, flask
 kiss3==8.0.0              # via -r requirements.in
-markupsafe==2.1.1         # via jinja2
+markupsafe==2.1.2         # via jinja2
 netaddr==0.8.0            # via oslo-config
 oslo-config==9.1.0        # via -r requirements.in
 oslo-i18n==5.1.0          # via oslo-config
-pbr==5.11.0               # via -r requirements.in, oslo-i18n, stevedore
+pbr==5.11.1               # via -r requirements.in, oslo-i18n, stevedore
 pluggy==1.0.0             # via -r requirements.in
 plumbum==1.8.1            # via rpyc
 pycparser==2.21           # via cffi
 pygments==2.14.0          # via rich
 pyopenssl==23.0.0         # via -r requirements.in
 pyserial==3.5             # via pyserial-asyncio
 pyserial-asyncio==0.6     # via kiss3
 python-engineio==4.3.4    # via python-socketio
 python-socketio==5.7.2    # via flask-socketio
-pytz==2022.7              # via -r requirements.in
+pytz==2022.7.1            # via -r requirements.in
 pyyaml==6.0               # via -r requirements.in, oslo-config
-requests==2.28.1          # via -r requirements.in, oslo-config, update-checker
+ratelimiter==1.2.0.post0  # via -r requirements.in
+requests==2.28.2          # via -r requirements.in, oslo-config, update-checker
 rfc3986==2.0.0            # via oslo-config
 rich==12.6.0              # via -r requirements.in
 rpyc==5.3.0               # via -r requirements.in
 shellingham==1.5.0.post1  # via -r requirements.in, click-completion
 six==1.16.0               # via -r requirements.in, click-completion, eventlet, imapclient
 soupsieve==2.3.2.post1    # via beautifulsoup4
 stevedore==4.1.1          # via oslo-config
 tabulate==0.9.0           # via -r requirements.in
 thesmuggler==1.0.1        # via -r requirements.in
 ua-parser==0.16.1         # via user-agents
 update-checker==0.18.0    # via -r requirements.in
-urllib3==1.26.13          # via requests
+urllib3==1.26.14          # via requests
 user-agents==2.2.0        # via -r requirements.in
 werkzeug==2.1.2           # via -r requirements.in, flask
 wrapt==1.14.1             # via -r requirements.in, debtcollector
 zipp==3.11.0              # via importlib-metadata
```

### Comparing `aprsd-3.0.2/setup.cfg` & `aprsd-3.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/setup.py` & `aprsd-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/cmds/test_send_message.py` & `aprsd-3.0.3/tests/cmds/test_send_message.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/cmds/test_webchat.py` & `aprsd-3.0.3/tests/cmds/test_webchat.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/fake.py` & `aprsd-3.0.3/tests/fake.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_fortune.py` & `aprsd-3.0.3/tests/plugins/test_fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_location.py` & `aprsd-3.0.3/tests/plugins/test_location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_notify.py` & `aprsd-3.0.3/tests/plugins/test_notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_ping.py` & `aprsd-3.0.3/tests/plugins/test_ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_query.py` & `aprsd-3.0.3/tests/plugins/test_query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_time.py` & `aprsd-3.0.3/tests/plugins/test_time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_version.py` & `aprsd-3.0.3/tests/plugins/test_version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/plugins/test_weather.py` & `aprsd-3.0.3/tests/plugins/test_weather.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/test_email.py` & `aprsd-3.0.3/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/test_main.py` & `aprsd-3.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/test_packets.py` & `aprsd-3.0.3/tests/test_packets.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tests/test_plugin.py` & `aprsd-3.0.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tools/fast8.sh` & `aprsd-3.0.3/tools/fast8.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.0.2/tox.ini` & `aprsd-3.0.3/tox.ini`

 * *Files identical despite different names*

