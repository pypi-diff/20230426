# Comparing `tmp/lino-noi-23.3.0.tar.gz` & `tmp/lino-noi-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-noi-23.3.0.tar", last modified: Sat Mar 18 04:03:15 2023, max compression
+gzip compressed data, was "lino-noi-23.4.0.tar", last modified: Wed Apr 26 03:16:10 2023, max compression
```

## Comparing `lino-noi-23.3.0.tar` & `lino-noi-23.4.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/.idea/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.3.0/.idea/encodings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1839 2015-09-19 04:08:02.000000 lino-noi-23.3.0/.idea/misc.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2015-09-19 04:08:02.000000 lino-noi-23.3.0/.idea/modules.xml
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/.idea/scopes/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      139 2015-09-19 04:08:02.000000 lino-noi-23.3.0/.idea/scopes/scope_settings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.3.0/.idea/vcs.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2202 2015-09-19 04:08:02.000000 lino-noi-23.3.0/.idea/workspace.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:54:16.000000 lino-noi-23.3.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      109 2016-08-14 01:22:00.000000 lino-noi-23.3.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1518 2023-03-18 04:03:15.868612 lino-noi-23.3.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-03-17 19:56:10.000000 lino-noi-23.3.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2022-08-17 01:06:46.000000 lino-noi-23.3.0/lino_noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/cal/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      299 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-04 14:35:11.000000 lino-noi-23.3.0/lino_noi/lib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2017-04-04 14:35:11.000000 lino-noi-23.3.0/lino_noi/lib/cal/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3536 2021-08-28 22:25:13.000000 lino-noi-23.3.0/lino_noi/lib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      274 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      245 2021-04-07 10:22:55.000000 lino-noi-23.3.0/lino_noi/lib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2020-04-04 06:56:19.000000 lino-noi-23.3.0/lino_noi/lib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-05-26 22:13:00.000000 lino-noi-23.3.0/lino_noi/lib/contacts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2587 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/courses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      812 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/courses/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      717 2022-11-08 12:29:27.000000 lino-noi-23.3.0/lino_noi/lib/courses/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2532 2022-11-08 12:30:48.000000 lino-noi-23.3.0/lino_noi/lib/courses/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/groups/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      319 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/groups/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      749 2021-08-16 10:54:17.000000 lino-noi-23.3.0/lino_noi/lib/groups/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      329 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/noi/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:02.000000 lino-noi-23.3.0/lino_noi/lib/noi/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6630 2022-10-18 23:19:00.000000 lino-noi-23.3.0/lino_noi/lib/noi/fixtures/linotickets.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2138 2023-03-17 19:57:48.000000 lino-noi-23.3.0/lino_noi/lib/noi/help_texts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      540 2021-06-15 17:12:44.000000 lino-noi-23.3.0/lino_noi/lib/noi/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/noi/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/noi/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-noi-23.3.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    14514 2019-03-29 11:25:54.000000 lino-noi-23.3.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/noi/locale/et/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-noi-23.3.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13858 2019-03-29 11:25:55.000000 lino-noi-23.3.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/noi/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-noi-23.3.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13846 2019-03-29 11:25:54.000000 lino-noi-23.3.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)    22188 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/noi/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1131 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/noi/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     6636 2023-03-13 22:30:18.000000 lino-noi-23.3.0/lino_noi/lib/noi/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2810 2022-12-23 05:58:38.000000 lino-noi-23.3.0/lino_noi/lib/noi/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      383 2021-05-29 09:01:55.000000 lino-noi-23.3.0/lino_noi/lib/noi/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/products/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      301 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/products/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      522 2021-04-23 19:31:33.000000 lino-noi-23.3.0/lino_noi/lib/products/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/public/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1166 2021-12-22 12:48:36.000000 lino-noi-23.3.0/lino_noi/lib/public/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/public/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/public/config/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2019-11-25 17:29:52.000000 lino-noi-23.3.0/lino_noi/lib/public/config/noi/index.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      720 2022-09-01 18:33:50.000000 lino-noi-23.3.0/lino_noi/lib/public/config/noi/tickets.Ticket.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      554 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/public/renderer.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1583 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/public/views.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/sales/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      311 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/sales/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/sales/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi/lib/sales/config/sales/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/sales/config/sales/VatProductInvoice/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1413 2023-02-15 06:31:52.000000 lino-noi-23.3.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/sales/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-05-09 16:04:58.000000 lino-noi-23.3.0/lino_noi/lib/sales/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2017-02-26 08:07:55.000000 lino-noi-23.3.0/lino_noi/lib/sales/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      985 2022-12-26 16:50:31.000000 lino-noi-23.3.0/lino_noi/lib/sales/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/subscriptions/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2023-01-06 20:30:18.000000 lino-noi-23.3.0/lino_noi/lib/subscriptions/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      378 2023-01-06 20:50:15.000000 lino-noi-23.3.0/lino_noi/lib/subscriptions/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/tickets/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1658 2023-01-08 01:21:19.000000 lino-noi-23.3.0/lino_noi/lib/tickets/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    15885 2023-02-16 20:05:18.000000 lino-noi-23.3.0/lino_noi/lib/tickets/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3858 2022-10-30 00:45:53.000000 lino-noi-23.3.0/lino_noi/lib/tickets/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/topics/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/topics/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      622 2021-04-07 10:22:54.000000 lino-noi-23.3.0/lino_noi/lib/topics/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)       37 2023-03-06 06:43:39.000000 lino-noi-23.3.0/lino_noi/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/lino_noi/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:00.000000 lino-noi-23.3.0/lino_noi/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:49.000000 lino-noi-23.3.0/lino_noi/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:50.000000 lino-noi-23.3.0/lino_noi/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:50.000000 lino-noi-23.3.0/lino_noi/lib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-11-08 12:29:27.000000 lino-noi-23.3.0/lino_noi/lib/users/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2322 2023-01-20 07:08:43.000000 lino-noi-23.3.0/lino_noi/lib/users/ui.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3080 2023-03-18 04:03:04.000000 lino-noi-23.3.0/lino_noi/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.864612 lino-noi-23.3.0/lino_noi.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1518 2023-03-18 04:03:15.000000 lino-noi-23.3.0/lino_noi.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2507 2023-03-18 04:03:15.000000 lino-noi-23.3.0/lino_noi.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-03-18 04:03:15.000000 lino-noi-23.3.0/lino_noi.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-08-31 16:13:18.000000 lino-noi-23.3.0/lino_noi.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2023-03-18 04:03:15.000000 lino-noi-23.3.0/lino_noi.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2023-03-18 04:03:15.000000 lino-noi-23.3.0/lino_noi.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      263 2021-05-05 05:16:56.000000 lino-noi-23.3.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-03-18 04:03:15.868612 lino-noi-23.3.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      179 2020-07-10 07:49:24.000000 lino-noi-23.3.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2021-04-25 11:53:26.000000 lino-noi-23.3.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-18 04:03:15.868612 lino-noi-23.3.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-18 18:50:53.000000 lino-noi-23.3.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2019-12-18 18:51:44.000000 lino-noi-23.3.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      186 2019-12-18 18:51:08.000000 lino-noi-23.3.0/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/.idea/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.4.0/.idea/encodings.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1839 2015-09-19 04:08:02.000000 lino-noi-23.4.0/.idea/misc.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2015-09-19 04:08:02.000000 lino-noi-23.4.0/.idea/modules.xml
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/.idea/scopes/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      139 2015-09-19 04:08:02.000000 lino-noi-23.4.0/.idea/scopes/scope_settings.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.4.0/.idea/vcs.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2202 2015-09-19 04:08:02.000000 lino-noi-23.4.0/.idea/workspace.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:54:16.000000 lino-noi-23.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      109 2016-08-14 01:22:00.000000 lino-noi-23.4.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1518 2023-04-26 03:16:10.743524 lino-noi-23.4.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-03-29 14:44:08.000000 lino-noi-23.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2022-08-17 01:06:46.000000 lino-noi-23.4.0/lino_noi/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/cal/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      299 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/cal/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-04 14:35:11.000000 lino-noi-23.4.0/lino_noi/lib/cal/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2017-04-04 14:35:11.000000 lino-noi-23.4.0/lino_noi/lib/cal/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3523 2023-04-15 09:49:10.000000 lino-noi-23.4.0/lino_noi/lib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      274 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      245 2021-04-07 10:22:55.000000 lino-noi-23.4.0/lino_noi/lib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2020-04-04 06:56:19.000000 lino-noi-23.4.0/lino_noi/lib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-05-26 22:13:00.000000 lino-noi-23.4.0/lino_noi/lib/contacts/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2587 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/courses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      812 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/courses/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      717 2022-11-08 12:29:27.000000 lino-noi-23.4.0/lino_noi/lib/courses/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2532 2022-11-08 12:30:48.000000 lino-noi-23.4.0/lino_noi/lib/courses/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/groups/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      319 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/groups/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      749 2021-08-16 10:54:17.000000 lino-noi-23.4.0/lino_noi/lib/groups/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      329 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/noi/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/noi/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:02.000000 lino-noi-23.4.0/lino_noi/lib/noi/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6630 2022-10-18 23:19:00.000000 lino-noi-23.4.0/lino_noi/lib/noi/fixtures/linotickets.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2138 2023-04-25 20:07:29.000000 lino-noi-23.4.0/lino_noi/lib/noi/help_texts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      540 2021-06-15 17:12:44.000000 lino-noi-23.4.0/lino_noi/lib/noi/layouts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/noi/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/noi/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-noi-23.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    14514 2019-03-29 11:25:54.000000 lino-noi-23.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/noi/locale/et/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-noi-23.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13858 2019-03-29 11:25:55.000000 lino-noi-23.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/noi/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-noi-23.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13846 2019-03-29 11:25:54.000000 lino-noi-23.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    22188 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/noi/migrate.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1131 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/noi/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     6636 2023-03-13 22:30:18.000000 lino-noi-23.4.0/lino_noi/lib/noi/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2810 2022-12-23 05:58:38.000000 lino-noi-23.4.0/lino_noi/lib/noi/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      383 2021-05-29 09:01:55.000000 lino-noi-23.4.0/lino_noi/lib/noi/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/products/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      301 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/products/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      522 2021-04-23 19:31:33.000000 lino-noi-23.4.0/lino_noi/lib/products/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/public/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1166 2021-12-22 12:48:36.000000 lino-noi-23.4.0/lino_noi/lib/public/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/public/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/public/config/noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2019-11-25 17:29:52.000000 lino-noi-23.4.0/lino_noi/lib/public/config/noi/index.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      720 2022-09-01 18:33:50.000000 lino-noi-23.4.0/lino_noi/lib/public/config/noi/tickets.Ticket.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      554 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/public/renderer.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1583 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/public/views.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/sales/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      311 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/sales/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/sales/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi/lib/sales/config/sales/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/sales/config/sales/VatProductInvoice/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1413 2023-02-15 06:31:52.000000 lino-noi-23.4.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/sales/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-05-09 16:04:58.000000 lino-noi-23.4.0/lino_noi/lib/sales/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2017-02-26 08:07:55.000000 lino-noi-23.4.0/lino_noi/lib/sales/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      985 2022-12-26 16:50:31.000000 lino-noi-23.4.0/lino_noi/lib/sales/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/subscriptions/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2023-01-06 20:30:18.000000 lino-noi-23.4.0/lino_noi/lib/subscriptions/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      378 2023-01-06 20:50:15.000000 lino-noi-23.4.0/lino_noi/lib/subscriptions/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/tickets/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1658 2023-01-08 01:21:19.000000 lino-noi-23.4.0/lino_noi/lib/tickets/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    15885 2023-02-16 20:05:18.000000 lino-noi-23.4.0/lino_noi/lib/tickets/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3858 2022-10-30 00:45:53.000000 lino-noi-23.4.0/lino_noi/lib/tickets/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/topics/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/topics/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      622 2021-04-07 10:22:54.000000 lino-noi-23.4.0/lino_noi/lib/topics/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       37 2023-03-06 06:43:39.000000 lino-noi-23.4.0/lino_noi/lib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/lino_noi/lib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:00.000000 lino-noi-23.4.0/lino_noi/lib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:49.000000 lino-noi-23.4.0/lino_noi/lib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:50.000000 lino-noi-23.4.0/lino_noi/lib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:50.000000 lino-noi-23.4.0/lino_noi/lib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-11-08 12:29:27.000000 lino-noi-23.4.0/lino_noi/lib/users/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1636 2023-04-15 09:49:32.000000 lino-noi-23.4.0/lino_noi/lib/users/ui.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3080 2023-04-26 03:15:50.000000 lino-noi-23.4.0/lino_noi/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.739524 lino-noi-23.4.0/lino_noi.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1518 2023-04-26 03:16:10.000000 lino-noi-23.4.0/lino_noi.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2507 2023-04-26 03:16:10.000000 lino-noi-23.4.0/lino_noi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-04-26 03:16:10.000000 lino-noi-23.4.0/lino_noi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-08-31 16:13:18.000000 lino-noi-23.4.0/lino_noi.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2023-04-26 03:16:10.000000 lino-noi-23.4.0/lino_noi.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2023-04-26 03:16:10.000000 lino-noi-23.4.0/lino_noi.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      263 2021-05-05 05:16:56.000000 lino-noi-23.4.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-04-26 03:16:10.743524 lino-noi-23.4.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      179 2020-07-10 07:49:24.000000 lino-noi-23.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2021-04-25 11:53:26.000000 lino-noi-23.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:10.743524 lino-noi-23.4.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-18 18:50:53.000000 lino-noi-23.4.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2019-12-18 18:51:44.000000 lino-noi-23.4.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      186 2019-12-18 18:51:08.000000 lino-noi-23.4.0/tests/test_packages.py
```

### Comparing `lino-noi-23.3.0/.idea/misc.xml` & `lino-noi-23.4.0/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/.idea/workspace.xml` & `lino-noi-23.4.0/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/COPYING` & `lino-noi-23.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/PKG-INFO` & `lino-noi-23.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 23.3.0
+Version: 23.4.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 
 
 Lino Noi is a customizable ticket management and time tracking
 system to use when time is more than money.
 
 - Documentation: https://noi.lino-framework.org
 
-- Technical specs are at https://www.lino-framework.org/specs/noi
+- Technical specs are at https://dev.lino-framework.org/specs/noi
 
 - This is an integral part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - The changelog is at https://www.lino-framework.org/changes
 
 - For introductions, commercial information and hosting solutions
```

### Comparing `lino-noi-23.3.0/README.rst` & `lino-noi-23.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 Lino Noi is a customizable ticket management and time tracking
 system to use when time is more than money.
 
 - Documentation: https://noi.lino-framework.org
 
-- Technical specs are at https://www.lino-framework.org/specs/noi
+- Technical specs are at https://dev.lino-framework.org/specs/noi
 
 - This is an integral part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - The changelog is at https://www.lino-framework.org/changes
 
 - For introductions, commercial information and hosting solutions
```

### Comparing `lino-noi-23.3.0/lino_noi/lib/cal/models.py` & `lino-noi-23.4.0/lino_noi/lib/cal/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 class EventDetail(EventDetail):
     start = "start_date start_time"
     end = "end_date end_time"
     notify = "notify_before notify_unit"
     main = "general GuestsByEvent"
     general = dd.Panel("""
     event_type:20 summary:60 id notify
-    start end access_class #all_day #assigned_to #duration #state
+    start end #all_day #assigned_to #duration #state
     user room company contact_person
     project owner workflow_buttons
     # owner created:20 modified:20
     description #blogs.EntriesByController #outbox.MailsByController
     """, label=_("General"))
 
 # Events.set_detail_layout(EventDetail())
```

### Comparing `lino-noi-23.3.0/lino_noi/lib/contacts/models.py` & `lino-noi-23.4.0/lino_noi/lib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/courses/__init__.py` & `lino-noi-23.4.0/lino_noi/lib/courses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/courses/models.py` & `lino-noi-23.4.0/lino_noi/lib/courses/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/courses/ui.py` & `lino-noi-23.4.0/lino_noi/lib/courses/ui.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/groups/models.py` & `lino-noi-23.4.0/lino_noi/lib/groups/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/fixtures/linotickets.py` & `lino-noi-23.4.0/lino_noi/lib/noi/fixtures/linotickets.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/help_texts.py` & `lino-noi-23.4.0/lino_noi/lib/noi/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/layouts.py` & `lino-noi-23.4.0/lino_noi/lib/noi/layouts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo` & `lino-noi-23.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po` & `lino-noi-23.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo` & `lino-noi-23.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po` & `lino-noi-23.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po` & `lino-noi-23.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/migrate.py` & `lino-noi-23.4.0/lino_noi/lib/noi/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/models.py` & `lino-noi-23.4.0/lino_noi/lib/noi/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/settings.py` & `lino-noi-23.4.0/lino_noi/lib/noi/settings.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/noi/user_types.py` & `lino-noi-23.4.0/lino_noi/lib/noi/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/products/models.py` & `lino-noi-23.4.0/lino_noi/lib/products/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/public/__init__.py` & `lino-noi-23.4.0/lino_noi/lib/public/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/public/config/noi/tickets.Ticket.html` & `lino-noi-23.4.0/lino_noi/lib/public/config/noi/tickets.Ticket.html`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/public/renderer.py` & `lino-noi-23.4.0/lino_noi/lib/public/renderer.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/public/views.py` & `lino-noi-23.4.0/lino_noi/lib/public/views.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html` & `lino-noi-23.4.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/sales/models.py` & `lino-noi-23.4.0/lino_noi/lib/sales/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/tickets/__init__.py` & `lino-noi-23.4.0/lino_noi/lib/tickets/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/tickets/models.py` & `lino-noi-23.4.0/lino_noi/lib/tickets/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/tickets/workflows.py` & `lino-noi-23.4.0/lino_noi/lib/tickets/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/topics/models.py` & `lino-noi-23.4.0/lino_noi/lib/topics/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.3.0/lino_noi/lib/users/ui.py` & `lino-noi-23.4.0/lino_noi/lib/users/ui.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     #
     #
     #     """, label=_("Clocking"), required_roles=dd.login_required(Worker))
     # else:
     #     working = dd.DummyPanel()
 
     calendar = dd.Panel("""
-    event_type access_class
+    event_type
     cal.SubscriptionsByUser
     # cal.MembershipsByUser
     """, label=dd.plugins.cal.verbose_name, required_roles=dd.login_required(OfficeUser))
 
     general1 = """
     username user_type:20
     first_name last_name initials
@@ -57,38 +57,10 @@
 
     general3 = """
     created:12 modified:12 id
     date_format time_zone
     #github_username
     """
 
-    # cal_left = """
-    # event_type access_class
-    # cal.SubscriptionsByUser
-    # """
-
-    # cal = dd.Panel("""
-    # cal_left:30 cal.TasksByUser:60
-    # """, label=dd.plugins.cal.verbose_name,
-    #                required_roles=dd.login_required(OfficeUser))
-
-    # contact = dd.Panel("""
-    # address_box info_box
-    # remarks:40 users.AuthoritiesGiven:20
-    # """, label=_("Contact"))
-    #
-    # info_box = """
-    # email:40
-    # # url
-    # phone
-    # gsm
-    # """
-    # address_box = """
-    # first_name last_name #initials
-    # country region city zip_code:10
-    # #addr1
-    # #street_prefix street:25 street_no #street_box
-    # # addr2
-    # """
 
 
 # Users.detail_layout = UserDetail()
```

### Comparing `lino-noi-23.3.0/lino_noi/setup_info.py` & `lino-noi-23.4.0/lino_noi/setup_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,27 +10,27 @@
     # srcref_url='https://gitlab.com/lino-framework/cosi/blob/master/%s',
     intersphinx_urls = dict(
         docs="https://noi.lino-framework.org"))
 
 
 SETUP_INFO = dict(
     name='lino-noi',
-    version='23.3.0',
+    version='23.4.0',
     install_requires=['lino-xl'],
     # tests_require=['pytest', 'mock'],
     test_suite='tests',
     description=("Manage support tickets and working time."),
     long_description="""\
 
 Lino Noi is a customizable ticket management and time tracking
 system to use when time is more than money.
 
 - Documentation: https://noi.lino-framework.org
 
-- Technical specs are at https://www.lino-framework.org/specs/noi
+- Technical specs are at https://dev.lino-framework.org/specs/noi
 
 - This is an integral part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - The changelog is at https://www.lino-framework.org/changes
 
 - For introductions, commercial information and hosting solutions
```

### Comparing `lino-noi-23.3.0/lino_noi.egg-info/PKG-INFO` & `lino-noi-23.4.0/lino_noi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 23.3.0
+Version: 23.4.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 
 
 Lino Noi is a customizable ticket management and time tracking
 system to use when time is more than money.
 
 - Documentation: https://noi.lino-framework.org
 
-- Technical specs are at https://www.lino-framework.org/specs/noi
+- Technical specs are at https://dev.lino-framework.org/specs/noi
 
 - This is an integral part of the Lino framework, which is documented
   at https://www.lino-framework.org
 
 - The changelog is at https://www.lino-framework.org/changes
 
 - For introductions, commercial information and hosting solutions
```

### Comparing `lino-noi-23.3.0/lino_noi.egg-info/SOURCES.txt` & `lino-noi-23.4.0/lino_noi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

