# Comparing `tmp/moodle-dl-2.3.1.9.tar.gz` & `tmp/moodle-dl-2.3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodle-dl-2.3.1.9.tar", last modified: Wed Apr 26 11:23:31 2023, max compression
+gzip compressed data, was "moodle-dl-2.3.2.0.tar", last modified: Wed Apr 26 11:55:02 2023, max compression
```

## Comparing `moodle-dl-2.3.1.9.tar` & `moodle-dl-2.3.2.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.515198 moodle-dl-2.3.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-26 11:23:31.515198 moodle-dl-2.3.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.507197 moodle-dl-2.3.1.9/moodle_dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/cli/config_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/cli/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/cli/moodle_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/cli/notifications_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27295 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/download_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/echo360.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/helixmedia_lti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/kalvidres_lti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/opencast_lti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/owncloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/sharepointfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/fake_download_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    41144 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/downloader/task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17435 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/moodle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/cookie_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/core_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/forum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/lesson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/quiz.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/mods/workshop.py
--rw-r--r--   0 runner    (1001) docker     (123)    29312 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/moodle_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/moodle_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/request_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/moodle/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/notifications/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/console/console_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/notifications/mail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36960 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/mail/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/mail/header_extender.png
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/mail/mail_formater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/mail/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/mail/mail_shooter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/notification_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.511197 moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/telegram_formater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/telegram_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/telegram_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.515198 moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/xmpp_formater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/xmpp_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/xmpp_shooter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/moodle_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:23:31.507197 moodle-dl-2.3.1.9/moodle_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-26 11:23:31.000000 moodle-dl-2.3.1.9/moodle_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-26 11:23:31.000000 moodle-dl-2.3.1.9/moodle_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:23:31.000000 moodle-dl-2.3.1.9/moodle_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 11:23:31.000000 moodle-dl-2.3.1.9/moodle_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:23:31.000000 moodle-dl-2.3.1.9/moodle_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-26 11:23:31.000000 moodle-dl-2.3.1.9/moodle_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 11:23:31.000000 moodle-dl-2.3.1.9/moodle_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:23:31.515198 moodle-dl-2.3.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-26 11:23:21.000000 moodle-dl-2.3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.072639 moodle-dl-2.3.2.0/moodle_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.072639 moodle-dl-2.3.2.0/moodle_dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/cli/config_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/cli/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/cli/moodle_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/cli/notifications_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27295 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.072639 moodle-dl-2.3.2.0/moodle_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/download_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/echo360.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/helixmedia_lti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/kalvidres_lti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/opencast_lti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/owncloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/sharepointfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/fake_download_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41144 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/downloader/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17435 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/moodle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/cookie_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/core_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/lesson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/mods/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29312 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/moodle_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/moodle_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/request_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/moodle/result_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/notifications/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/console/console_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/notifications/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36960 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/mail/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/mail/header_extender.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/mail/mail_formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/mail/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/mail/mail_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/notification_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/telegram_formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/telegram_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/telegram_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/xmpp_formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/xmpp_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/xmpp_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/moodle_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:55:02.072639 moodle-dl-2.3.2.0/moodle_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-04-26 11:55:02.000000 moodle-dl-2.3.2.0/moodle_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-26 11:55:02.000000 moodle-dl-2.3.2.0/moodle_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:55:02.000000 moodle-dl-2.3.2.0/moodle_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 11:55:02.000000 moodle-dl-2.3.2.0/moodle_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:55:02.000000 moodle-dl-2.3.2.0/moodle_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-26 11:55:02.000000 moodle-dl-2.3.2.0/moodle_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 11:55:02.000000 moodle-dl-2.3.2.0/moodle_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:55:02.076639 moodle-dl-2.3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-26 11:54:51.000000 moodle-dl-2.3.2.0/setup.py
```

### Comparing `moodle-dl-2.3.1.9/LICENSE` & `moodle-dl-2.3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/PKG-INFO` & `moodle-dl-2.3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.1.9
+Version: 2.3.2.0
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle-dl-2.3.1.9/README.md` & `moodle-dl-2.3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/cli/__init__.py` & `moodle-dl-2.3.2.0/moodle_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/cli/config_wizard.py` & `moodle-dl-2.3.2.0/moodle_dl/cli/config_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/cli/database_manager.py` & `moodle-dl-2.3.2.0/moodle_dl/cli/database_manager.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/cli/moodle_wizard.py` & `moodle-dl-2.3.2.0/moodle_dl/cli/moodle_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/cli/notifications_wizard.py` & `moodle-dl-2.3.2.0/moodle_dl/cli/notifications_wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from getpass import getpass
 
-from aioxmpp.errors import StanzaError, UserError
-
 from moodle_dl.config import ConfigHelper
 from moodle_dl.notifications.mail.mail_formater import create_full_welcome_mail
 from moodle_dl.notifications.mail.mail_shooter import MailShooter
 from moodle_dl.notifications.telegram.telegram_shooter import (
     RequestRejectedError,
     TelegramShooter,
 )
@@ -151,16 +149,14 @@
                 print('Testing XMPP-Config...')
 
                 try:
                     xmpp_shooter = XmppShooter(sender, password, target)
                     xmpp_shooter.send('This is a test message from moodle-dl!')
                 except (
                     ConnectionError,
-                    StanzaError,
-                    UserError,
                     OSError,
                     RuntimeError,
                 ) as e:
                     print(f'Error while sending the test message: {str(e)}')
                     continue
 
                 else:
```

### Comparing `moodle-dl-2.3.1.9/moodle_dl/config.py` & `moodle-dl-2.3.2.0/moodle_dl/config.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/database.py` & `moodle-dl-2.3.2.0/moodle_dl/database.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/download_service.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/download_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/__init__.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/echo360.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/echo360.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/googledrive.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/googledrive.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/helixmedia_lti.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/helixmedia_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/kalvidres_lti.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/kalvidres_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/opencast_lti.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/opencast_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/owncloud.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/owncloud.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/sharepoint.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/extractors/sharepointfiles.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/extractors/sharepointfiles.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/fake_download_service.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/fake_download_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/downloader/task.py` & `moodle-dl-2.3.2.0/moodle_dl/downloader/task.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/main.py` & `moodle-dl-2.3.2.0/moodle_dl/main.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/cookie_handler.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/core_handler.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/core_handler.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/__init__.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/assign.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/assign.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/common.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/common.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/data.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/data.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/folder.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/folder.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/forum.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/forum.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/lesson.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/lesson.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/page.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/page.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/quiz.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/quiz.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/mods/workshop.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/mods/workshop.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/moodle_constants.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/moodle_constants.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/moodle_service.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/moodle_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/request_helper.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/request_helper.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/moodle/result_builder.py` & `moodle-dl-2.3.2.0/moodle_dl/moodle/result_builder.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/__init__.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/console/console_service.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/console/console_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/mail/header.png` & `moodle-dl-2.3.2.0/moodle_dl/notifications/mail/header.png`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/mail/header_extender.png` & `moodle-dl-2.3.2.0/moodle_dl/notifications/mail/header_extender.png`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/mail/mail_formater.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/mail/mail_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/mail/mail_service.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/mail/mail_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/mail/mail_shooter.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/mail/mail_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/notification_service.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/notification_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/telegram_formater.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/telegram_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/telegram_service.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/telegram_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/telegram/telegram_shooter.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/telegram/telegram_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/xmpp_formater.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/xmpp_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/xmpp_service.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/xmpp_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/notifications/xmpp/xmpp_shooter.py` & `moodle-dl-2.3.2.0/moodle_dl/notifications/xmpp/xmpp_shooter.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,10 +11,12 @@
         self.password = password
         self.recipient = xmpp.protocol.JID(recipient)
 
     def send(self, message):
         if not self.is_connected:
             self.connection.connect()
             self.connection.auth(user=self.jid.getNode(), password=self.password, resource=self.jid.getResource())
+            if not hasattr(self.connection, 'Bind') or getattr(self.connection, 'Bind').session != 1:
+                raise ConnectionError('XMPP Session could not be opend')
             self.is_connected = True
 
         self.connection.send(xmpp.protocol.Message(to=self.recipient, body=message))
```

### Comparing `moodle-dl-2.3.1.9/moodle_dl/types.py` & `moodle-dl-2.3.2.0/moodle_dl/types.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl/utils.py` & `moodle-dl-2.3.2.0/moodle_dl/utils.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/moodle_dl.egg-info/PKG-INFO` & `moodle-dl-2.3.2.0/moodle_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.1.9
+Version: 2.3.2.0
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle-dl-2.3.1.9/moodle_dl.egg-info/SOURCES.txt` & `moodle-dl-2.3.2.0/moodle_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.1.9/setup.py` & `moodle-dl-2.3.2.0/setup.py`

 * *Files identical despite different names*

