# Comparing `tmp/lino-amici-23.2.0.tar.gz` & `tmp/lino-amici-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-amici-23.2.0.tar", last modified: Wed Feb 15 05:04:41 2023, max compression
+gzip compressed data, was "lino-amici-23.4.0.tar", last modified: Wed Apr 26 03:17:27 2023, max compression
```

## Comparing `lino-amici-23.2.0.tar` & `lino-amici-23.4.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:28.000000 lino-amici-23.2.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      190 2022-10-19 14:04:22.000000 lino-amici-23.2.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1584 2023-02-15 05:04:41.203174 lino-amici-23.2.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      691 2022-12-03 04:02:33.000000 lino-amici-23.2.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      464 2021-04-25 16:07:31.000000 lino-amici-23.2.0/lino_amici/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      242 2021-04-07 10:22:53.000000 lino-amici-23.2.0/lino_amici/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici/lib/amici/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      306 2021-04-07 10:22:54.000000 lino-amici-23.2.0/lino_amici/lib/amici/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      497 2021-06-12 03:15:08.000000 lino-amici-23.2.0/lino_amici/lib/amici/custom_layouts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      753 2021-02-14 21:14:30.000000 lino-amici-23.2.0/lino_amici/lib/amici/help_texts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici/lib/amici/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici/lib/amici/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-amici-23.2.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    14175 2019-03-29 11:27:30.000000 lino-amici-23.2.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici/lib/amici/locale/et/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-amici-23.2.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13385 2019-03-29 11:27:31.000000 lino-amici-23.2.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici/lib/amici/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-amici-23.2.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13352 2019-03-29 11:27:30.000000 lino-amici-23.2.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-06-12 03:05:36.000000 lino-amici-23.2.0/lino_amici/lib/amici/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4869 2021-08-13 06:30:11.000000 lino-amici-23.2.0/lino_amici/lib/amici/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2229 2022-12-03 11:54:35.000000 lino-amici-23.2.0/lino_amici/lib/amici/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      868 2021-04-07 10:22:54.000000 lino-amici-23.2.0/lino_amici/lib/amici/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      325 2021-04-07 10:22:54.000000 lino-amici-23.2.0/lino_amici/lib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-30 02:04:04.000000 lino-amici-23.2.0/lino_amici/lib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2017-04-30 02:04:26.000000 lino-amici-23.2.0/lino_amici/lib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       54 2017-05-03 12:11:20.000000 lino-amici-23.2.0/lino_amici/lib/contacts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6536 2022-09-17 02:10:54.000000 lino-amici-23.2.0/lino_amici/lib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/households/
--rw-rw-rw-   0 luc       (1000) www-data    (33)       42 2020-12-24 02:38:08.000000 lino-amici-23.2.0/lino_amici/lib/households/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/households/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2020-12-29 13:26:01.000000 lino-amici-23.2.0/lino_amici/lib/households/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       57 2020-12-24 02:41:05.000000 lino-amici-23.2.0/lino_amici/lib/households/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2020-12-24 02:38:56.000000 lino-amici-23.2.0/lino_amici/lib/households/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      532 2020-12-24 02:45:22.000000 lino-amici-23.2.0/lino_amici/lib/households/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      275 2021-04-07 10:22:54.000000 lino-amici-23.2.0/lino_amici/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-amici-23.2.0/lino_amici/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:52.000000 lino-amici-23.2.0/lino_amici/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:53.000000 lino-amici-23.2.0/lino_amici/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:53.000000 lino-amici-23.2.0/lino_amici/lib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2022-11-08 12:29:27.000000 lino-amici-23.2.0/lino_amici/lib/users/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      822 2022-11-08 12:30:48.000000 lino-amici-23.2.0/lino_amici/lib/users/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/projects/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-05-05 02:54:41.000000 lino-amici-23.2.0/lino_amici/projects/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/projects/amici1/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      230 2021-04-07 10:22:54.000000 lino-amici-23.2.0/lino_amici/projects/amici1/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      277 2023-01-10 07:35:25.000000 lino-amici-23.2.0/lino_amici/projects/amici1/manage.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/projects/amici1/settings/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1193 2021-04-18 15:44:21.000000 lino-amici-23.2.0/lino_amici/projects/amici1/settings/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      544 2022-11-01 14:52:31.000000 lino-amici-23.2.0/lino_amici/projects/amici1/settings/demo.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/projects/amici1/settings/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-03-26 04:42:38.000000 lino-amici-23.2.0/lino_amici/projects/amici1/settings/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1222 2021-04-07 10:22:55.000000 lino-amici-23.2.0/lino_amici/projects/amici1/settings/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       85 2015-09-19 04:09:04.000000 lino-amici-23.2.0/lino_amici/projects/amici1/settings/memory.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/lino_amici/projects/amici1/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-11-17 06:49:05.000000 lino-amici-23.2.0/lino_amici/projects/amici1/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2450 2021-04-07 10:22:54.000000 lino-amici-23.2.0/lino_amici/projects/amici1/tests/test_insert_person.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2886 2023-02-15 05:04:26.000000 lino-amici-23.2.0/lino_amici/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.199175 lino-amici-23.2.0/lino_amici.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1584 2023-02-15 05:04:41.000000 lino-amici-23.2.0/lino_amici.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2113 2023-02-15 05:04:41.000000 lino-amici-23.2.0/lino_amici.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-02-15 05:04:41.000000 lino-amici-23.2.0/lino_amici.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2017-05-03 11:30:38.000000 lino-amici-23.2.0/lino_amici.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       16 2023-02-15 05:04:41.000000 lino-amici-23.2.0/lino_amici.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-02-15 05:04:41.000000 lino-amici-23.2.0/lino_amici.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-12-03 20:13:34.000000 lino-amici-23.2.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-02-15 05:04:41.203174 lino-amici-23.2.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      181 2020-07-10 08:02:46.000000 lino-amici-23.2.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      416 2021-04-25 11:53:26.000000 lino-amici-23.2.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-02-15 05:04:41.203174 lino-amici-23.2.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-02 05:37:16.000000 lino-amici-23.2.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      113 2021-03-30 02:28:55.000000 lino-amici-23.2.0/tests/import_test.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      272 2021-02-15 13:04:51.000000 lino-amici-23.2.0/tests/test_demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2019-12-18 17:37:53.000000 lino-amici-23.2.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      417 2019-12-18 17:40:05.000000 lino-amici-23.2.0/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:28.000000 lino-amici-23.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      190 2022-10-19 14:04:22.000000 lino-amici-23.4.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1584 2023-04-26 03:17:27.784000 lino-amici-23.4.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      691 2022-12-03 04:02:33.000000 lino-amici-23.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      464 2021-04-25 16:07:31.000000 lino-amici-23.4.0/lino_amici/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      242 2021-04-07 10:22:53.000000 lino-amici-23.4.0/lino_amici/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      306 2021-04-07 10:22:54.000000 lino-amici-23.4.0/lino_amici/lib/amici/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      497 2021-06-12 03:15:08.000000 lino-amici-23.4.0/lino_amici/lib/amici/custom_layouts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      753 2021-02-14 21:14:30.000000 lino-amici-23.4.0/lino_amici/lib/amici/help_texts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-amici-23.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    14175 2019-03-29 11:27:30.000000 lino-amici-23.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/locale/et/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-amici-23.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13385 2019-03-29 11:27:31.000000 lino-amici-23.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-amici-23.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13352 2019-03-29 11:27:30.000000 lino-amici-23.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-06-12 03:05:36.000000 lino-amici-23.4.0/lino_amici/lib/amici/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4874 2023-04-22 19:08:19.000000 lino-amici-23.4.0/lino_amici/lib/amici/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2229 2022-12-03 11:54:35.000000 lino-amici-23.4.0/lino_amici/lib/amici/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      868 2021-04-07 10:22:54.000000 lino-amici-23.4.0/lino_amici/lib/amici/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/lib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      318 2023-03-25 08:39:35.000000 lino-amici-23.4.0/lino_amici/lib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/lib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-30 02:04:04.000000 lino-amici-23.4.0/lino_amici/lib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2017-04-30 02:04:26.000000 lino-amici-23.4.0/lino_amici/lib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       54 2017-05-03 12:11:20.000000 lino-amici-23.4.0/lino_amici/lib/contacts/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6536 2022-09-17 02:10:54.000000 lino-amici-23.4.0/lino_amici/lib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/lib/households/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       42 2020-12-24 02:38:08.000000 lino-amici-23.4.0/lino_amici/lib/households/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/lib/households/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2020-12-29 13:26:01.000000 lino-amici-23.4.0/lino_amici/lib/households/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       57 2020-12-24 02:41:05.000000 lino-amici-23.4.0/lino_amici/lib/households/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2020-12-24 02:38:56.000000 lino-amici-23.4.0/lino_amici/lib/households/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      532 2020-12-24 02:45:22.000000 lino-amici-23.4.0/lino_amici/lib/households/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/lib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      275 2021-04-07 10:22:54.000000 lino-amici-23.4.0/lino_amici/lib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/lib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-amici-23.4.0/lino_amici/lib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:52.000000 lino-amici-23.4.0/lino_amici/lib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:53.000000 lino-amici-23.4.0/lino_amici/lib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:53.000000 lino-amici-23.4.0/lino_amici/lib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2022-11-08 12:29:27.000000 lino-amici-23.4.0/lino_amici/lib/users/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      805 2023-04-15 09:46:55.000000 lino-amici-23.4.0/lino_amici/lib/users/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/projects/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-05-05 02:54:41.000000 lino-amici-23.4.0/lino_amici/projects/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/projects/amici1/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      230 2021-04-07 10:22:54.000000 lino-amici-23.4.0/lino_amici/projects/amici1/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      277 2023-01-10 07:35:25.000000 lino-amici-23.4.0/lino_amici/projects/amici1/manage.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/projects/amici1/settings/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1193 2021-04-18 15:44:21.000000 lino-amici-23.4.0/lino_amici/projects/amici1/settings/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      544 2023-04-05 00:19:32.000000 lino-amici-23.4.0/lino_amici/projects/amici1/settings/demo.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/projects/amici1/settings/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-03-26 04:42:38.000000 lino-amici-23.4.0/lino_amici/projects/amici1/settings/fixtures/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1225 2023-04-05 09:42:49.000000 lino-amici-23.4.0/lino_amici/projects/amici1/settings/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       85 2015-09-19 04:09:04.000000 lino-amici-23.4.0/lino_amici/projects/amici1/settings/memory.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/lino_amici/projects/amici1/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-11-17 06:49:05.000000 lino-amici-23.4.0/lino_amici/projects/amici1/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2450 2021-04-07 10:22:54.000000 lino-amici-23.4.0/lino_amici/projects/amici1/tests/test_insert_person.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2886 2023-04-26 03:17:16.000000 lino-amici-23.4.0/lino_amici/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.780000 lino-amici-23.4.0/lino_amici.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1584 2023-04-26 03:17:27.000000 lino-amici-23.4.0/lino_amici.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2113 2023-04-26 03:17:27.000000 lino-amici-23.4.0/lino_amici.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-04-26 03:17:27.000000 lino-amici-23.4.0/lino_amici.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2017-05-03 11:30:38.000000 lino-amici-23.4.0/lino_amici.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       16 2023-04-26 03:17:27.000000 lino-amici-23.4.0/lino_amici.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-04-26 03:17:27.000000 lino-amici-23.4.0/lino_amici.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-12-03 20:13:34.000000 lino-amici-23.4.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-04-26 03:17:27.784000 lino-amici-23.4.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      181 2020-07-10 08:02:46.000000 lino-amici-23.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      416 2021-04-25 11:53:26.000000 lino-amici-23.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:17:27.784000 lino-amici-23.4.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-02 05:37:16.000000 lino-amici-23.4.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      113 2021-03-30 02:28:55.000000 lino-amici-23.4.0/tests/import_test.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      272 2021-02-15 13:04:51.000000 lino-amici-23.4.0/tests/test_demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2019-12-18 17:37:53.000000 lino-amici-23.4.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      417 2019-12-18 17:40:05.000000 lino-amici-23.4.0/tests/test_packages.py
```

### Comparing `lino-amici-23.2.0/COPYING` & `lino-amici-23.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/PKG-INFO` & `lino-amici-23.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-amici
-Version: 23.2.0
+Version: 23.4.0
 Summary: A Lino for managing family contacts
 Home-page: https://gitlab.com/lino-framework/amici
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `lino-amici-23.2.0/README.rst` & `lino-amici-23.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/help_texts.py` & `lino-amici-23.4.0/lino_amici/lib/amici/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo` & `lino-amici-23.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po` & `lino-amici-23.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo` & `lino-amici-23.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po` & `lino-amici-23.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po` & `lino-amici-23.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/settings.py` & `lino-amici-23.4.0/lino_amici/lib/amici/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         # yield 'lino_xl.lib.meetings'
 
     def get_plugin_configs(self):
         for i in super(Site, self).get_plugin_configs():
             yield i
         # yield ('addresses', 'partner_model', 'contacts.Person')
         yield ('cal', 'partner_model', 'contacts.Person')
-        yield ('cal', 'demo_absences', False)
+        yield ('cal', 'with_demo_absences', False)
         yield ('contacts', 'with_roles_history', True)
 
     # def setup_plugins(self):
     #     super(Site, self).setup_plugins()
     #     # self.plugins.comments.configure(
     #     #     commentable_model='tickets.Ticket')
     #     # self.plugins.skills.configure(
```

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/user_types.py` & `lino-amici-23.4.0/lino_amici/lib/amici/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/amici/workflows.py` & `lino-amici-23.4.0/lino_amici/lib/amici/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/contacts/models.py` & `lino-amici-23.4.0/lino_amici/lib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/households/models.py` & `lino-amici-23.4.0/lino_amici/lib/households/models.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/lib/users/ui.py` & `lino-amici-23.4.0/lino_amici/lib/users/ui.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 
     general = dd.Panel("""
     box1
     remarks:40 AuthoritiesGiven:20
     """, label=_("General"))
 
     calendar = dd.Panel("""
-    event_type access_class
+    event_type 
     cal.SubscriptionsByUser
     # cal.MembershipsByUser
     """, label=dd.plugins.cal.verbose_name,
                         required_roles=dd.login_required(OfficeUser))
 
-    
+
 
     box1 = """
     username user_type:20 partner
     first_name last_name initials
     email language
     id created modified
     """
 
 # Users.detail_layout = UserDetail()
-
```

### Comparing `lino-amici-23.2.0/lino_amici/projects/amici1/settings/__init__.py` & `lino-amici-23.4.0/lino_amici/projects/amici1/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/projects/amici1/settings/demo.py` & `lino-amici-23.4.0/lino_amici/projects/amici1/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/projects/amici1/settings/fixtures/demo.py` & `lino-amici-23.4.0/lino_amici/projects/amici1/settings/fixtures/demo.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """Some demo data for the Vilma project.
 
 """
 
 from lino.api import dd, rt, _
 from lino.utils.mldbc import babel_named as named
 from lino.utils.cycler import Cycler
-from lino_xl.lib.cal.choicelists import Recurrencies
+from lino.modlib.system.choicelists import Recurrencies
 
 def objects():
     Topic = rt.models.topics.Topic
     EventType = rt.models.cal.EventType
     Room = rt.models.cal.Room
     Company = rt.models.contacts.Company
     Person = rt.models.contacts.Person
```

### Comparing `lino-amici-23.2.0/lino_amici/projects/amici1/tests/test_insert_person.py` & `lino-amici-23.4.0/lino_amici/projects/amici1/tests/test_insert_person.py`

 * *Files identical despite different names*

### Comparing `lino-amici-23.2.0/lino_amici/setup_info.py` & `lino-amici-23.4.0/lino_amici/setup_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright 2017-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 # $ python setup.py test -s tests.test_packages
 
 SETUP_INFO = dict(
     name='lino-amici',
-    version='23.2.0',
+    version='23.4.0',
     install_requires=['lino-xl', 'vobject'],
 
     # tests_require=['pytest', 'mock'],
     test_suite='tests',
     description=("A Lino for managing family contacts"),
     long_description="""\
```

### Comparing `lino-amici-23.2.0/lino_amici.egg-info/PKG-INFO` & `lino-amici-23.4.0/lino_amici.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-amici
-Version: 23.2.0
+Version: 23.4.0
 Summary: A Lino for managing family contacts
 Home-page: https://gitlab.com/lino-framework/amici
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `lino-amici-23.2.0/lino_amici.egg-info/SOURCES.txt` & `lino-amici-23.4.0/lino_amici.egg-info/SOURCES.txt`

 * *Files identical despite different names*

