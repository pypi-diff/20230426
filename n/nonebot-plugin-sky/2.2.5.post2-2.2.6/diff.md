# Comparing `tmp/nonebot-plugin-sky-2.2.5.post2.tar.gz` & `tmp/nonebot-plugin-sky-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sky-2.2.5.post2.tar", last modified: Wed Apr 12 10:11:53 2023, max compression
+gzip compressed data, was "nonebot-plugin-sky-2.2.6.tar", last modified: Wed Apr 26 07:19:48 2023, max compression
```

## Comparing `nonebot-plugin-sky-2.2.5.post2.tar` & `nonebot-plugin-sky-2.2.6.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.237843 nonebot-plugin-sky-2.2.5.post2/
--rw-rw-rw-   0        0        0    35823 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/LICENSE
--rw-rw-rw-   0        0        0    15750 2023-04-12 10:11:53.237843 nonebot-plugin-sky-2.2.5.post2/PKG-INFO
--rw-rw-rw-   0        0        0    15220 2023-04-12 09:44:24.000000 nonebot-plugin-sky-2.2.5.post2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.159032 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/
--rw-rw-rw-   0        0        0     6153 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.172999 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/__init__.py
--rw-rw-rw-   0        0        0     5707 2023-03-02 08:15:25.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/command.py
--rw-rw-rw-   0        0        0     1810 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/helper_at_all.py
--rw-rw-rw-   0        0        0     1261 2023-02-24 05:45:59.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/load_config.py
--rw-rw-rw-   0        0        0     1747 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/msg_forward.py
--rw-rw-rw-   0        0        0     1560 2023-02-24 02:36:59.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/travelling_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.176989 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/
--rw-rw-rw-   0        0        0     1160 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/light_beauty.py
--rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/light_cute.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.182975 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.187963 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/__init__.py
--rw-rw-rw-   0        0        0     2547 2023-04-04 06:39:21.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/international.py
--rw-rw-rw-   0        0        0     3077 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/national.py
--rw-rw-rw-   0        0        0      637 2023-03-02 07:17:23.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/public_notice.py
--rw-rw-rw-   0        0        0    13738 2023-03-02 03:54:13.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/query_tools.py
--rw-rw-rw-   0        0        0     1080 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/queue.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.191953 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/international.py
--rw-rw-rw-   0        0        0     2996 2023-04-12 10:08:03.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/national.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.196951 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.217891 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/
--rw-rw-rw-   0        0        0    16051 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/eating.jpg
--rw-rw-rw-   0        0        0    89789 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_braid.gif
--rw-rw-rw-   0        0        0    79644 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_bun.gif
--rw-rw-rw-   0        0        0    72146 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_cat.gif
--rw-rw-rw-   0        0        0    87935 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_fox.gif
--rw-rw-rw-   0        0        0    80542 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
--rw-rw-rw-   0        0        0    95522 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/go.jpg
--rw-rw-rw-   0        0        0      274 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.219886 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu_image/
--rw-rw-rw-   0        0        0   824527 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu_image/menu.png
--rw-rw-rw-   0        0        0       95 2023-02-20 02:53:16.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/pusher.py
--rw-rw-rw-   0        0        0     3791 2023-03-02 09:17:27.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.236845 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/
--rw-rw-rw-   0        0        0     2280 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/__init__.py
--rw-rw-rw-   0        0        0      405 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/bot_loader.py
--rw-rw-rw-   0        0        0      607 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/chain_reply.py
--rw-rw-rw-   0        0        0     5067 2023-04-12 09:51:04.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/check_update.py
--rw-rw-rw-   0        0        0     6369 2023-03-23 08:02:10.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/data_pack.py
--rw-rw-rw-   0        0        0      391 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/date_util.py
--rw-rw-rw-   0        0        0      746 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/json_cards.py
--rw-rw-rw-   0        0        0     1264 2023-04-04 07:30:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/notice_board.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.165019 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/
--rw-rw-rw-   0        0        0    15750 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1950 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 10:11:53.238840 nonebot-plugin-sky-2.2.5.post2/setup.cfg
--rw-rw-rw-   0        0        0     1397 2023-04-12 09:44:24.000000 nonebot-plugin-sky-2.2.5.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.493358 nonebot-plugin-sky-2.2.6/
+-rw-rw-rw-   0        0        0    35823 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/LICENSE
+-rw-rw-rw-   0        0        0    15893 2023-04-26 07:19:48.492361 nonebot-plugin-sky-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    15369 2023-04-26 07:02:50.000000 nonebot-plugin-sky-2.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.402601 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/
+-rw-rw-rw-   0        0        0     6153 2023-04-13 02:27:05.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.418558 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/__init__.py
+-rw-rw-rw-   0        0        0     5707 2023-03-02 08:15:25.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/command.py
+-rw-rw-rw-   0        0        0     1810 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/helper_at_all.py
+-rw-rw-rw-   0        0        0     1261 2023-02-24 05:45:59.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/load_config.py
+-rw-rw-rw-   0        0        0     1747 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/msg_forward.py
+-rw-rw-rw-   0        0        0     1560 2023-02-24 02:36:59.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/travelling_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.423545 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/
+-rw-rw-rw-   0        0        0     1160 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/light_beauty.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/light_cute.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.430526 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.434540 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2547 2023-04-04 06:39:21.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/international.py
+-rw-rw-rw-   0        0        0     3077 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/national.py
+-rw-rw-rw-   0        0        0   459817 2023-04-26 06:51:25.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/get_id.png
+-rw-rw-rw-   0        0        0      637 2023-03-02 07:17:23.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/public_notice.py
+-rw-rw-rw-   0        0        0    13536 2023-04-26 07:15:44.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/query_tools.py
+-rw-rw-rw-   0        0        0     1080 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/queue.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.438530 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
+-rw-rw-rw-   0        0        0     3041 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/international.py
+-rw-rw-rw-   0        0        0     2996 2023-04-12 10:08:03.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/national.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.444490 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.466431 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/
+-rw-rw-rw-   0        0        0    16051 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/eating.jpg
+-rw-rw-rw-   0        0        0    89789 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_braid.gif
+-rw-rw-rw-   0        0        0    79644 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_bun.gif
+-rw-rw-rw-   0        0        0    72146 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_cat.gif
+-rw-rw-rw-   0        0        0    87935 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_fox.gif
+-rw-rw-rw-   0        0        0    80542 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
+-rw-rw-rw-   0        0        0    95522 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/go.jpg
+-rw-rw-rw-   0        0        0      274 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.469450 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu_image/
+-rw-rw-rw-   0        0        0   824527 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu_image/menu.png
+-rw-rw-rw-   0        0        0       95 2023-02-20 02:53:16.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/pusher.py
+-rw-rw-rw-   0        0        0     3791 2023-03-02 09:17:27.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.490366 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/
+-rw-rw-rw-   0        0        0     2280 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/bot_loader.py
+-rw-rw-rw-   0        0        0      607 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/chain_reply.py
+-rw-rw-rw-   0        0        0     5061 2023-04-26 07:02:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/check_update.py
+-rw-rw-rw-   0        0        0     6369 2023-03-23 08:02:10.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/data_pack.py
+-rw-rw-rw-   0        0        0      391 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/date_util.py
+-rw-rw-rw-   0        0        0      746 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/json_cards.py
+-rw-rw-rw-   0        0        0     1264 2023-04-04 07:30:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/notice_board.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.408586 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/
+-rw-rw-rw-   0        0        0    15893 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 07:19:48.493358 nonebot-plugin-sky-2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1450 2023-04-26 07:19:24.000000 nonebot-plugin-sky-2.2.6/setup.py
```

### Comparing `nonebot-plugin-sky-2.2.5.post2/LICENSE` & `nonebot-plugin-sky-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/PKG-INFO` & `nonebot-plugin-sky-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.5.post2
+Version: 2.2.6
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -286,14 +286,20 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.25 v2.2.6
+
+1.修复获取uid帮助图片无法发送的问题
+
+2.当处于季节真空期时查询季蜡、蜡烛数返回相应提示
+
 2023.4.12 v2.2.5.post2
 
 修复已知问题
 
 2023.4.4 v2.2.5.post1
 
 修复插件公告镜像源地址
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.5.post2 Summary:
-nonebot2 plugin sky Home-page: https://github.com/Kaguya233qwq/
-nonebot_plugin_sky Author: Kaguya233qwq Author-email: 1435608435@qq.com
-Keywords: pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
-General Public License v3 (GPLv3) Classifier: Natural Language :: Chinese
-(Simplified) Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.6 Summary: nonebot2
+plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
+Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
+pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
+Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
       # nonebot_plugin_sky _â¨ åºäº [NoneBot2](https://v2.nonebot.dev/
                       ) çåéæ¯æ¥æ»ç¥æä»¶ â¨_
                            [Python] [NoneBot] [pypi]
                              _âå åèéâ_
 # â¨å®è£ä¸é¨ç½²â¨
 ##ä»¥ä¸ä¸ç§ç±»åè¯·éæ©éåèªå·±çæ¹æ¡è¿è¡é¨ç½²ï¼
@@ -111,16 +111,19 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4
-v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
+â¨æ´æ°æ¥å¿â¨ 2023.4.25 v2.2.6
+1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
+2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
+2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
+ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
 3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
 ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
 ä¿®å¤å·²ç¥çé®é¢ 2023.3.7 v2.2.2
 åéééå å·¥ä½å¿æ²¡ææ¶é´æ´æ°ï¼
 æ´æ¢å¤å»æ°æ®æºä¸ºå¾®å@åéåå1å· 2023.3.2 v2.2.1
```

### Comparing `nonebot-plugin-sky-2.2.5.post2/README.md` & `nonebot-plugin-sky-2.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,20 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.25 v2.2.6
+
+1.修复获取uid帮助图片无法发送的问题
+
+2.当处于季节真空期时查询季蜡、蜡烛数返回相应提示
+
 2023.4.12 v2.2.5.post2
 
 修复已知问题
 
 2023.4.4 v2.2.5.post1
 
 修复插件公告镜像源地址
```

#### html2text {}

```diff
@@ -104,16 +104,19 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4
-v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
+â¨æ´æ°æ¥å¿â¨ 2023.4.25 v2.2.6
+1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
+2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
+2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
+ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
 3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
 ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
 ä¿®å¤å·²ç¥çé®é¢ 2023.3.7 v2.2.2
 åéééå å·¥ä½å¿æ²¡ææ¶é´æ´æ°ï¼
 æ´æ¢å¤å»æ°æ®æºä¸ºå¾®å@åéåå1å· 2023.3.2 v2.2.1
```

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/__init__.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/command.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/command.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/helper_at_all.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/helper_at_all.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/load_config.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/msg_forward.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/msg_forward.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/travelling_cache.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/travelling_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/__init__.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/international.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/national.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/public_notice.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/public_notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/query_tools.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/query_tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from nonebot.internal.params import ArgPlainText
 from nonebot.params import CommandArg
 
 from ..utils_ import send_forward_msg
 from ..config.msg_forward import is_forward
 from ..config.command import *
 
+NO_CACHE_ID_MSG = '没有相应缓存数据，请先私聊bot进行id绑定操作。\n'
+NO_BIND_MSG = '您还没有绑定您的光遇id，请私聊bot发送“光遇绑定”来进行绑定\n'
+
 
 async def save_sky_id(qq: str, sky_id: str) -> None:
     """
     保存qq号与对应的sky_id
     """
     if not os.path.isfile('Sky/origin_id'):
         with open("Sky/origin_id", "a") as f:
@@ -47,20 +50,23 @@
         if content != '' and content is not None:
             tmp = json.loads(content)
         else:
             return None
         return tmp.get(qq, None)
 
 
+def get_id_img():
+    abspath_ = os.path.abspath(__file__).strip('query_tools.py')
+    path = 'file:///' + abspath_ + 'get_id.png'
+    return MessageSegment.image(path)
+
+
 To_Get_Uid = (
         '如何获取uid？见下图：' +
-        MessageSegment.image(
-            'https://gitee.com/Kaguya233qwq/'
-            'nonebot_plugin_sky/raw/main/'
-            '.README_images/get_uid.jpg')
+        get_id_img()
 )
 
 
 class Sprite:
 
     def __init__(self):
         self.api_get_token = 'https://live-gms-sky-merge.game.163.com:9005/gms_cmd'
@@ -204,23 +210,26 @@
         查询季节蜡烛的记录
         """
         token = await self.__get_token(sky_id)
         results: dict = await self.request_to_sprite(token, '季节蜡烛查询')
         try:
             if results.get('answer'):
                 answer = results.get('answer')
-                changes: str = answer.strip(
-                    '<默认回复>小易帮您查到'
-                    '最近季节蜡烛变化记录：#r请留意：'
-                    '#R维护补偿#n所获得道具记录本功能不显示'
-                )
-                log = changes.replace('#r', '\n').replace('#R', '【').replace('#n', '】').strip(
-                    '若您想要查询更多蜡烛变化请点击<ask>【更多蜡烛查询】</ask'
-                )
-                return f'---最近的季节蜡烛变化记录---\n{log}'
+                if '小易帮您查到' in answer:
+                    changes: str = answer.strip(
+                        '<默认回复>小易帮您查到'
+                        '最近季节蜡烛变化记录：#r请留意：'
+                        '#R维护补偿#n所获得道具记录本功能不显示'
+                    )
+                    log = changes.replace('#r', '\n').replace('#R', '【').replace('#n', '】').strip(
+                        '若您想要查询更多蜡烛变化请点击<ask>【更多蜡烛查询】</ask'
+                    )
+                    return f'---最近的季节蜡烛变化记录---\n{log}'
+                elif '请稍候再查看' in answer:
+                    return '季节真空期，季蜡数默认为零'
             else:
                 return '服务器异常，返回结果时出现错误'
         except Exception as e:
             str(e)
             return '查询失败，未知错误'
 
 
@@ -253,22 +262,21 @@
 
 
 @QueryWhiteCandles.handle()
 async def white_candles_handler(bot: Bot, event: MessageEvent):
     sky_id = await load_sky_id(str(event.sender.user_id))
     if not sky_id:
         await QueryWhiteCandles.send(
-            '没有相应缓存数据，请先私聊bot进行id绑定操作。\n'
+            NO_CACHE_ID_MSG
             + To_Get_Uid
         )
     else:
         if sky_id == '':
             await QueryWhiteCandles.send(
-                '您还没有绑定您的光遇id，'
-                '请私聊bot发送“光遇绑定”来进行绑定\n' +
+                NO_BIND_MSG +
                 To_Get_Uid
             )
         query = Sprite()
         results = await query.get_candles(sky_id)
         if '这边查询一下' not in results:
             pass
         else:
@@ -281,22 +289,21 @@
 
 
 @QuerySeasonCandles.handle()
 async def season_candles_handler(bot: Bot, event: MessageEvent):
     sky_id = await load_sky_id(str(event.sender.user_id))
     if not sky_id:
         await QuerySeasonCandles.send(
-            '没有相应缓存数据，请先私聊bot进行id绑定操作。\n' +
+            NO_CACHE_ID_MSG +
             To_Get_Uid
         )
     else:
         if sky_id == '':
             await QuerySeasonCandles.send(
-                '您还没有绑定您的光遇id，'
-                '请私聊bot发送“光遇绑定”来进行绑定\n' +
+                NO_BIND_MSG +
                 To_Get_Uid
             )
         query = Sprite()
         results = await query.get_season_candles(sky_id)
         if '这边查询一下' not in results:
             pass
         else:
@@ -309,37 +316,40 @@
 
 
 @CandlesView.handle()
 async def candle_view(event: MessageEvent):
     sky_id = await load_sky_id(str(event.sender.user_id))
     if not sky_id:
         await CandlesView.send(
-            '没有相应缓存数据，请先私聊bot进行id绑定操作。\n' +
+            NO_CACHE_ID_MSG +
             To_Get_Uid
         )
     else:
         if sky_id == '':
             await CandlesView.send(
-                '您还没有绑定您的光遇id，'
-                '请私聊bot发送“光遇绑定”来进行绑定\n' +
+                NO_BIND_MSG +
                 To_Get_Uid
             )
         query = Sprite()
 
         try:
             season = await query.get_season_candles(sky_id)
             white = await query.get_candles(sky_id)
 
             if '这边查询一下' not in season and '这边查询一下' not in white:
                 pass
             else:
                 time.sleep(1)
                 season = await query.get_season_candles(sky_id)
                 white = await query.get_candles(sky_id)
-            season_left = re.findall('剩余：(\d+)+?', season)[0]
+            try:
+                season_left = re.findall('剩余：(\d+)+?', season)[0]
+            except Exception as e:
+                e.__str__()
+                season_left = 0
             white_left = re.findall('剩余：(\d+)+?', white)[0]
             await CandlesView.send(
                 f'蜡烛总览：\n●普通蜡烛：{white_left}\n●季节蜡烛：{season_left}'
             )
         except Exception as e:
             str(e)
             await CandlesView.send('查询失败，返回结果异常')
@@ -347,42 +357,40 @@
 
 @Weather.handle()
 async def weather_handle(event: MessageEvent):
     query = Sprite()
     sky_id = await load_sky_id(str(event.sender.user_id))
     if not sky_id:
         await Weather.send(
-            '没有相应缓存数据，请先私聊bot进行id绑定操作。\n' +
+            NO_CACHE_ID_MSG +
             To_Get_Uid
         )
     else:
         if sky_id == '':
             await Weather.send(
-                '您还没有绑定您的光遇id，'
-                '请私聊bot发送“光遇绑定”来进行绑定\n' +
+                NO_BIND_MSG +
                 To_Get_Uid
             )
         results = await query.get_weather(sky_id)
         await Weather.send(MessageSegment.image(results))
 
 
 @Activities.handle()
 async def act_handle(event: MessageEvent):
     query = Sprite()
     sky_id = await load_sky_id(str(event.sender.user_id))
     if not sky_id:
         await Activities.send(
-            '没有相应缓存数据，请先私聊bot进行id绑定操作。\n' +
+            NO_CACHE_ID_MSG +
             To_Get_Uid
         )
     else:
         if sky_id == '':
             await Activities.send(
-                '您还没有绑定您的光遇id，'
-                '请私聊bot发送“光遇绑定”来进行绑定\n' +
+                NO_BIND_MSG +
                 To_Get_Uid
             )
         results = await query.get_activities(sky_id)
         await Activities.send(results)
 
 
 __all__ = (
```

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/queue.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/queue.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/international.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/national.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/eating.jpg` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/eating.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_braid.gif` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_braid.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_bun.gif` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_bun.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_cat.gif` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_fox.gif` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_fox.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/go.jpg` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/go.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu_image/menu.png` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu_image/menu.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/scheduler.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/__init__.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/chain_reply.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/chain_reply.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/check_update.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/check_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 from nonebot import on_command, logger
 from ..config.command import get_cmd_alias
 
 logging.captureWarnings(True)  # 去掉建议使用SSL验证的显示
 
-Version = '2.2.5.post2'  # 全局插件版本信息  （不用加v！）
+Version = '2.2.6'  # 全局插件版本信息  （不用加v！）
 
 
 async def get_datapack_ver():
     """
     检查本地数据包版本
     """
     try:
```

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/data_pack.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/data_pack.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/json_cards.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/json_cards.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/notice_board.py` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/notice_board.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/PKG-INFO` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.5.post2
+Version: 2.2.6
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -286,14 +286,20 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.25 v2.2.6
+
+1.修复获取uid帮助图片无法发送的问题
+
+2.当处于季节真空期时查询季蜡、蜡烛数返回相应提示
+
 2023.4.12 v2.2.5.post2
 
 修复已知问题
 
 2023.4.4 v2.2.5.post1
 
 修复插件公告镜像源地址
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.5.post2 Summary:
-nonebot2 plugin sky Home-page: https://github.com/Kaguya233qwq/
-nonebot_plugin_sky Author: Kaguya233qwq Author-email: 1435608435@qq.com
-Keywords: pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
-General Public License v3 (GPLv3) Classifier: Natural Language :: Chinese
-(Simplified) Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.6 Summary: nonebot2
+plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
+Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
+pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
+Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
       # nonebot_plugin_sky _â¨ åºäº [NoneBot2](https://v2.nonebot.dev/
                       ) çåéæ¯æ¥æ»ç¥æä»¶ â¨_
                            [Python] [NoneBot] [pypi]
                              _âå åèéâ_
 # â¨å®è£ä¸é¨ç½²â¨
 ##ä»¥ä¸ä¸ç§ç±»åè¯·éæ©éåèªå·±çæ¹æ¡è¿è¡é¨ç½²ï¼
@@ -111,16 +111,19 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4
-v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
+â¨æ´æ°æ¥å¿â¨ 2023.4.25 v2.2.6
+1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
+2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
+2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
+ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
 3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
 ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
 ä¿®å¤å·²ç¥çé®é¢ 2023.3.7 v2.2.2
 åéééå å·¥ä½å¿æ²¡ææ¶é´æ´æ°ï¼
 æ´æ¢å¤å»æ°æ®æºä¸ºå¾®å@åéåå1å· 2023.3.2 v2.2.1
```

### Comparing `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/SOURCES.txt` & `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 nonebot_plugin_sky/config/load_config.py
 nonebot_plugin_sky/config/msg_forward.py
 nonebot_plugin_sky/config/travelling_cache.py
 nonebot_plugin_sky/guild/__init__.py
 nonebot_plugin_sky/guild/light_beauty.py
 nonebot_plugin_sky/guild/light_cute.py
 nonebot_plugin_sky/sky/__init__.py
+nonebot_plugin_sky/sky/get_id.png
 nonebot_plugin_sky/sky/public_notice.py
 nonebot_plugin_sky/sky/query_tools.py
 nonebot_plugin_sky/sky/queue.py
 nonebot_plugin_sky/sky/daily_tasks/__init__.py
 nonebot_plugin_sky/sky/daily_tasks/international.py
 nonebot_plugin_sky/sky/daily_tasks/national.py
 nonebot_plugin_sky/sky/travelling_spirit/__init__.py
```

### Comparing `nonebot-plugin-sky-2.2.5.post2/setup.py` & `nonebot-plugin-sky-2.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 def get_files(path):
     """获取路径下所有文件相对路径"""
     file_list = []
     files = os.listdir(path)
     for file in files:
         file_list.append(path + '/' + file)
     file_list.append('nonebot_plugin_sky/tools/menu_image/menu.png')
+    file_list.append('nonebot_plugin_sky/sky/get_id.png')
     return file_list
 
 
 Files = get_files(r'nonebot_plugin_sky/tools/helper_image')
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
 setuptools.setup(
     name='nonebot-plugin-sky',
-    version='v2.2.5.post2',
+    version='v2.2.6',
     author='Kaguya233qwq',
     author_email='1435608435@qq.com',
     keywords=["pip", "nonebot2", "nonebot", "sky光遇", "光遇"],
     url='https://github.com/Kaguya233qwq/nonebot_plugin_sky',
     description='''nonebot2 plugin sky''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

