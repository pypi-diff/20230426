# Comparing `tmp/django-phonenumber-field-7.0.2.tar.gz` & `tmp/django-phonenumber-field-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-phonenumber-field-7.0.2.tar", last modified: Mon Jan  9 16:25:47 2023, max compression
+gzip compressed data, was "django-phonenumber-field-7.1.0.tar", last modified: Wed Apr 26 20:44:00 2023, max compression
```

## Comparing `django-phonenumber-field-7.0.2.tar` & `django-phonenumber-field-7.1.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/
--rw-------   0 freitafr  (1000) freitafr  (1000)      213 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/.readthedocs.yaml
--rw-------   0 freitafr  (1000) freitafr  (1000)     3219 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/AUTHORS
--rw-------   0 freitafr  (1000) freitafr  (1000)     6553 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/CHANGELOG.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     1077 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/LICENSE
--rw-------   0 freitafr  (1000) freitafr  (1000)       60 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/MANIFEST.in
--rw-------   0 freitafr  (1000) freitafr  (1000)     2486 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/PKG-INFO
--rw-------   0 freitafr  (1000) freitafr  (1000)     1158 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/README.rst
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/
--rw-------   0 freitafr  (1000) freitafr  (1000)     2486 2023-01-09 16:25:47.000000 django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/PKG-INFO
--rw-------   0 freitafr  (1000) freitafr  (1000)     4203 2023-01-09 16:25:47.000000 django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/SOURCES.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)        1 2023-01-09 16:25:47.000000 django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/dependency_links.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)        1 2022-08-28 14:01:37.000000 django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/not-zip-safe
--rw-------   0 freitafr  (1000) freitafr  (1000)       92 2023-01-09 16:25:47.000000 django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/requires.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)       18 2023-01-09 16:25:47.000000 django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/top_level.txt
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/docs/
--rw-------   0 freitafr  (1000) freitafr  (1000)      634 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/Makefile
--rw-------   0 freitafr  (1000) freitafr  (1000)     1642 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/conf.py
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/docs/ext/
--rw-------   0 freitafr  (1000) freitafr  (1000)      136 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/ext/phonenumber_field_docs.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     1306 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/index.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)      800 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/make.bat
--rw-------   0 freitafr  (1000) freitafr  (1000)    11179 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/reference.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)       44 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/requirements.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)       79 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/docs/settings.py
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/phonenumber_field/
--rw-------   0 freitafr  (1000) freitafr  (1000)      168 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/__init__.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     2593 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/phonenumber_field/formfields.py
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.069971 django-phonenumber-field-7.0.2/phonenumber_field/locale/ar/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/phonenumber_field/locale/ar/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1122 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ar/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1695 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ar/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/az/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/phonenumber_field/locale/az/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      636 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/az/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1368 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/az/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/bg/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/phonenumber_field/locale/bg/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1170 2021-12-07 15:13:26.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/bg/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1604 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/bg/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/bn/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.076638 django-phonenumber-field-7.0.2/phonenumber_field/locale/bn/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      690 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/bn/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1453 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/bn/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/cs/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/cs/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      979 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/cs/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1160 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/cs/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/da/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/da/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      570 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/da/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1309 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/da/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/de/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/de/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1017 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/de/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1441 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/de/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/eo/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/eo/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      984 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/eo/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1239 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/eo/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/es/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/es/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      998 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/es/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1535 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/es/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/es_AR/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/es_AR/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      931 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/es_AR/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1533 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/es_AR/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/fa/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/fa/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1037 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/fa/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1481 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/fa/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/fi/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/fi/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      560 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/fi/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1290 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/fi/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/fr/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/fr/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1032 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/fr/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1515 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/fr/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/he/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/he/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1018 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/he/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1468 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/he/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/hy/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/hy/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1122 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/hy/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1664 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/hy/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/id/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/id/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1013 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/id/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1527 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/id/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/it/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/it/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      656 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/it/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1410 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/it/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/ko/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/ko/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      574 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ko/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1319 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ko/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/lt/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/lt/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1137 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/lt/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1642 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/lt/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/nb/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/nb/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      587 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/nb/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1343 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/nb/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/nl/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/nl/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      995 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/nl/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1433 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/nl/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/pl/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/pl/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1065 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/pl/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1605 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/pl/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1031 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1466 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt_BR/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.079971 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt_BR/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      907 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1512 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/ro/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/ro/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      633 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ro/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1342 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ro/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/ru/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/ru/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1238 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ru/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1699 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/ru/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/sk/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/sk/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      639 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/sk/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1369 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/sk/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/sv/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/sv/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      975 2023-01-09 16:14:35.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/sv/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1441 2023-01-09 16:14:35.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/sv/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/tr/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/tr/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1025 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/tr/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1467 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/tr/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1205 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1670 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk_UA/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk_UA/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      988 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1647 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.po
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.073304 django-phonenumber-field-7.0.2/phonenumber_field/locale/zh_Hans/
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/phonenumber_field/locale/zh_Hans/LC_MESSAGES/
--rw-------   0 freitafr  (1000) freitafr  (1000)      805 2021-10-21 08:09:13.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-------   0 freitafr  (1000) freitafr  (1000)     1453 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.po
--rw-------   0 freitafr  (1000) freitafr  (1000)     4033 2022-10-11 16:15:33.000000 django-phonenumber-field-7.0.2/phonenumber_field/modelfields.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     5776 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/phonenumber_field/phonenumber.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     1189 2022-12-06 08:06:23.000000 django-phonenumber-field-7.0.2/phonenumber_field/serializerfields.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      461 2022-09-01 12:38:12.000000 django-phonenumber-field-7.0.2/phonenumber_field/validators.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      160 2023-01-09 16:25:47.000000 django-phonenumber-field-7.0.2/phonenumber_field/version.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     6491 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/phonenumber_field/widgets.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      190 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/pyproject.toml
--rw-------   0 freitafr  (1000) freitafr  (1000)     1422 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/setup.cfg
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-01-09 16:25:47.083304 django-phonenumber-field-7.0.2/tests/
--rw-------   0 freitafr  (1000) freitafr  (1000)        0 2021-01-16 11:25:09.000000 django-phonenumber-field-7.0.2/tests/__init__.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      456 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/tests/forms.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     3044 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/tests/models.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      193 2021-12-06 14:23:51.000000 django-phonenumber-field-7.0.2/tests/settings.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     5503 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/tests/test_formfields.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     3025 2022-08-29 15:23:54.000000 django-phonenumber-field-7.0.2/tests/test_phonenumber.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     4465 2022-12-06 08:06:23.000000 django-phonenumber-field-7.0.2/tests/test_serializers.py
--rw-------   0 freitafr  (1000) freitafr  (1000)    12258 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/tests/test_widgets.py
--rw-------   0 freitafr  (1000) freitafr  (1000)    24556 2022-09-09 09:17:46.000000 django-phonenumber-field-7.0.2/tests/tests.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     1155 2022-10-11 15:33:32.000000 django-phonenumber-field-7.0.2/tox.ini
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      213 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/.readthedocs.yaml
+-rw-------   0 freitafr  (1000) freitafr  (1000)     3219 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/AUTHORS
+-rw-------   0 freitafr  (1000) freitafr  (1000)     6553 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/CHANGELOG.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1077 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/LICENSE
+-rw-------   0 freitafr  (1000) freitafr  (1000)       60 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/MANIFEST.in
+-rw-------   0 freitafr  (1000) freitafr  (1000)     2486 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/PKG-INFO
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1158 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/README.rst
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     2486 2023-04-26 20:44:00.000000 django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/PKG-INFO
+-rw-------   0 freitafr  (1000) freitafr  (1000)     4203 2023-04-26 20:44:00.000000 django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/SOURCES.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)        1 2023-04-26 20:44:00.000000 django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/dependency_links.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)        1 2022-08-28 14:01:37.000000 django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/not-zip-safe
+-rw-------   0 freitafr  (1000) freitafr  (1000)       92 2023-04-26 20:44:00.000000 django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/requires.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)       18 2023-04-26 20:44:00.000000 django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/top_level.txt
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/docs/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      634 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/docs/Makefile
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1642 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/docs/conf.py
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/docs/ext/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      136 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/docs/ext/phonenumber_field_docs.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1306 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/docs/index.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)      800 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/docs/make.bat
+-rw-------   0 freitafr  (1000) freitafr  (1000)    11363 2023-04-26 20:05:54.000000 django-phonenumber-field-7.1.0/docs/reference.rst
+-rw-------   0 freitafr  (1000) freitafr  (1000)       44 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/docs/requirements.txt
+-rw-------   0 freitafr  (1000) freitafr  (1000)       79 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/docs/settings.py
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      168 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/__init__.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     2593 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/phonenumber_field/formfields.py
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/ar/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/ar/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1122 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ar/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1695 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ar/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/az/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/az/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      636 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/az/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1368 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/az/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/bg/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/bg/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1170 2021-12-07 15:13:26.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/bg/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1604 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/bg/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/bn/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/bn/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      690 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/bn/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1453 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/bn/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/cs/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/cs/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      979 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/cs/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1160 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/cs/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/da/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/da/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      570 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/da/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1309 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/da/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/de/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/de/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1017 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/de/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1441 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/de/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/eo/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/eo/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      984 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/eo/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1239 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/eo/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/es/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/es/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      998 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/es/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1535 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/es/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/es_AR/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.900779 django-phonenumber-field-7.1.0/phonenumber_field/locale/es_AR/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      931 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/es_AR/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1533 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/es_AR/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/fa/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/fa/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1037 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/fa/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1481 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/fa/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/fi/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/fi/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      560 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/fi/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1290 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/fi/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/fr/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/fr/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1032 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/fr/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1515 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/fr/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/he/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/he/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1018 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/he/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1468 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/he/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/hy/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/hy/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1122 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/hy/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1664 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/hy/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.894112 django-phonenumber-field-7.1.0/phonenumber_field/locale/id/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/id/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1013 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/id/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1527 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/id/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/it/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/it/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      656 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/it/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1410 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/it/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/ko/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/ko/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      574 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ko/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1319 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ko/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/lt/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/lt/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1137 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/lt/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1642 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/lt/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/nb/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/nb/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      964 2023-04-26 20:05:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/nb/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1441 2023-04-26 20:05:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/nb/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/nl/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/nl/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      995 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/nl/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1433 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/nl/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/pl/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/pl/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1065 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/pl/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1605 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/pl/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1031 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1466 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt_BR/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt_BR/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      907 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1512 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/ro/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.904112 django-phonenumber-field-7.1.0/phonenumber_field/locale/ro/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      633 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ro/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1342 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ro/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/ru/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/phonenumber_field/locale/ru/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1238 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ru/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1699 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/ru/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/sk/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/phonenumber_field/locale/sk/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      639 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/sk/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1369 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/sk/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/sv/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/phonenumber_field/locale/sv/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      975 2023-01-09 16:14:35.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/sv/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1441 2023-01-09 16:14:35.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/sv/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/tr/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/phonenumber_field/locale/tr/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1025 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/tr/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1467 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/tr/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1205 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1670 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk_UA/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk_UA/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      988 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1647 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.po
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.897446 django-phonenumber-field-7.1.0/phonenumber_field/locale/zh_Hans/
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/phonenumber_field/locale/zh_Hans/LC_MESSAGES/
+-rw-------   0 freitafr  (1000) freitafr  (1000)      805 2021-10-21 08:09:13.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1453 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-------   0 freitafr  (1000) freitafr  (1000)     4033 2022-10-11 16:15:33.000000 django-phonenumber-field-7.1.0/phonenumber_field/modelfields.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     5776 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/phonenumber_field/phonenumber.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1189 2022-12-06 08:06:23.000000 django-phonenumber-field-7.1.0/phonenumber_field/serializerfields.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      461 2022-09-01 12:38:12.000000 django-phonenumber-field-7.1.0/phonenumber_field/validators.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      160 2023-04-26 20:44:00.000000 django-phonenumber-field-7.1.0/phonenumber_field/version.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     6491 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/phonenumber_field/widgets.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      190 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/pyproject.toml
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1462 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/setup.cfg
+drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 20:44:00.907446 django-phonenumber-field-7.1.0/tests/
+-rw-------   0 freitafr  (1000) freitafr  (1000)        0 2021-01-16 11:25:09.000000 django-phonenumber-field-7.1.0/tests/__init__.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      456 2022-08-29 15:23:54.000000 django-phonenumber-field-7.1.0/tests/forms.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     3044 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/tests/models.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)      193 2021-12-06 14:23:51.000000 django-phonenumber-field-7.1.0/tests/settings.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     5503 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/tests/test_formfields.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     3025 2023-02-20 09:54:47.000000 django-phonenumber-field-7.1.0/tests/test_phonenumber.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     4465 2022-12-06 08:06:23.000000 django-phonenumber-field-7.1.0/tests/test_serializers.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)    12258 2022-10-11 15:33:32.000000 django-phonenumber-field-7.1.0/tests/test_widgets.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)    24556 2022-09-09 09:17:46.000000 django-phonenumber-field-7.1.0/tests/tests.py
+-rw-------   0 freitafr  (1000) freitafr  (1000)     1155 2023-04-26 20:11:48.000000 django-phonenumber-field-7.1.0/tox.ini
```

### Comparing `django-phonenumber-field-7.0.2/AUTHORS` & `django-phonenumber-field-7.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/CHANGELOG.rst` & `django-phonenumber-field-7.1.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/LICENSE` & `django-phonenumber-field-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/PKG-INFO` & `django-phonenumber-field-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-phonenumber-field
-Version: 7.0.2
+Version: 7.1.0
 Summary: An international phone number field for django models.
 Home-page: https://github.com/stefanfoulis/django-phonenumber-field
 Author: Stefan Foulis
 Author-email: stefan@foulis.ch
 Maintainer: Stefan Foulis
 Maintainer-email: stefan@foulis.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-phonenumber-field-7.0.2/README.rst` & `django-phonenumber-field-7.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/PKG-INFO` & `django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-phonenumber-field
-Version: 7.0.2
+Version: 7.1.0
 Summary: An international phone number field for django models.
 Home-page: https://github.com/stefanfoulis/django-phonenumber-field
 Author: Stefan Foulis
 Author-email: stefan@foulis.ch
 Maintainer: Stefan Foulis
 Maintainer-email: stefan@foulis.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-phonenumber-field-7.0.2/django_phonenumber_field.egg-info/SOURCES.txt` & `django-phonenumber-field-7.1.0/django_phonenumber_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/docs/Makefile` & `django-phonenumber-field-7.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/docs/conf.py` & `django-phonenumber-field-7.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/docs/index.rst` & `django-phonenumber-field-7.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/docs/make.bat` & `django-phonenumber-field-7.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/docs/reference.rst` & `django-phonenumber-field-7.1.0/docs/reference.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
    import django
    from bs4 import BeautifulSoup
 
    django.setup()
 
    def print_html(html):
-       print(BeautifulSoup(html).prettify())
+       print(BeautifulSoup(html).prettify().strip())
 
 
 The PhoneNumber wrapper
 =======================
 
 .. autoclass:: phonenumber_field.phonenumber.PhoneNumber()
 
@@ -362,17 +362,17 @@
 
 Store phone numbers strings in the specified format.
 
 Default: ``"E164"``.
 
 Choices:
 
-- ``"E164"``,
-- ``"INTERNATIONAL"``,
-- ``"RFC3966"``,
+- ``"E164"`` (public international numbers),
+- ``"INTERNATIONAL"`` (international numbers, possibly with phone extensions),
+- ``"RFC3966"`` (international numbers, possibly with phone extensions),
 - ``"NATIONAL"`` (discouraged, requires :setting:`PHONENUMBER_DEFAULT_REGION`).
 
 .. setting:: PHONENUMBER_DEFAULT_REGION
 
 ``PHONENUMBER_DEFAULT_REGION``
 ------------------------------
 
@@ -388,11 +388,11 @@
 
 String formatting of phone numbers.
 
 Default: ``"E164"``.
 
 Choices:
 
-- ``"E164"``,
+- ``"E164"`` (no support of phone extensions),
 - ``"INTERNATIONAL"``,
 - ``"RFC3966"``,
 - ``"NATIONAL"`` (discouraged, fails to represent international phone numbers).
```

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/formfields.py` & `django-phonenumber-field-7.1.0/phonenumber_field/formfields.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/ar/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/ar/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/az/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/az/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/az/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/bg/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/bg/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/bn/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/bn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/bn/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/cs/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/cs/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/da/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/da/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/de/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/de/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/eo/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/eo/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/es/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/es/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/es_AR/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/es_AR/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/fa/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/fa/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/fi/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/fi/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/fr/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/fr/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/he/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/he/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/hy/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/hy/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/hy/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/hy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/id/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/id/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/it/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/it/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/ko/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/ko/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/lt/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/lt/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/nb/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ro/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2016-10-21 15:04+0200\n"
-"Last-Translator: Kristian Klette <klette@klette.us>\n"
+"PO-Revision-Date: 2018-10-19 14:07+0300\n"
+"Last-Translator: Cristi Vîjdea <cristi@cvjd.me>\n"
 "Language-Team: \n"
-"Language: nb\n"
+"Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.8.9\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
+"2:1));\n"
 
 msgid "Enter a valid phone number."
-msgstr "Tast inn et gyldig telefonnummer"
+msgstr "Introduceți un număr de telefon valid."
 
 msgid "Phone number"
-msgstr "Telefonnummer"
+msgstr "Număr de telefon"
 
 msgid "The phone number entered is not valid."
-msgstr "Ugyldig telefonnummer"
+msgstr "Numărul de telefon introdus nu este valid."
```

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/nb/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/nb/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# Norwegian Bokmaal Translation for django-phonenumber-field.
+# Norwegian Bokmål Translation for django-phonenumber-field.
 # Copyright (C) 2016
 # This file is distributed under the same license as the django-phonenumber-field package.
 # FIRST AUTHOR <klette@klette.us>, 2016.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-05-28 13:04-0700\n"
+"POT-Creation-Date: 2023-03-22 22:50+0100\n"
 "PO-Revision-Date: 2016-10-21 15:04+0200\n"
 "Last-Translator: Kristian Klette <klette@klette.us>\n"
 "Language-Team: \n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.9\n"
 
-#: formfields.py:27
+#: formfields.py:43
 #, python-brace-format
 msgid ""
 "Enter a valid phone number (e.g. {example_number}) or a number with an "
 "international call prefix."
 msgstr ""
+"Tast inn et gyldig telefonnummer (f.eks. {example_number}) eller et nummer "
+"med internasjonal landskode."
 
 #. Translators: {example_number} is an international phone number.
-#: formfields.py:33
-#, fuzzy, python-brace-format
-#| msgid "Enter a valid phone number."
+#: formfields.py:49
+#, python-brace-format
 msgid "Enter a valid phone number (e.g. {example_number})."
-msgstr "Tast inn et gyldig telefonnummer"
+msgstr "Tast inn et gyldig telefonnummer (f.eks. {example_number})."
 
-#: modelfields.py:51
+#: modelfields.py:53
 msgid "Phone number"
 msgstr "Telefonnummer"
 
-#: serializerfields.py:9
+#: serializerfields.py:10
 msgid "Enter a valid phone number."
-msgstr "Tast inn et gyldig telefonnummer"
+msgstr "Tast inn et gyldig telefonnummer."
 
 #: validators.py:11
 msgid "The phone number entered is not valid."
-msgstr "Ugyldig telefonnummer"
+msgstr "Telefonnummeret er ugyldig."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/nl/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/nl/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/pl/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/pl/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/pt/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/pt/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/ro/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/ru/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/ru/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/sk/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/sk/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/sv/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/sv/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/tr/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/tr/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/uk/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/uk/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.po` & `django-phonenumber-field-7.1.0/phonenumber_field/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/modelfields.py` & `django-phonenumber-field-7.1.0/phonenumber_field/modelfields.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/phonenumber.py` & `django-phonenumber-field-7.1.0/phonenumber_field/phonenumber.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/serializerfields.py` & `django-phonenumber-field-7.1.0/phonenumber_field/serializerfields.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/phonenumber_field/widgets.py` & `django-phonenumber-field-7.1.0/phonenumber_field/widgets.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/setup.cfg` & `django-phonenumber-field-7.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 maintainer = Stefan Foulis
 maintainer_email = stefan@foulis.ch
 platforms = OS Independent
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
@@ -43,14 +43,18 @@
 	phonenumbers >= 7.0.2
 phonenumberslite = 
 	phonenumberslite >= 7.0.2
 
 [flake8]
 max-line-length = 88
 show-source = True
+extend-exclude = 
+	.env/
+	.venv/
+	venv/
 
 [isort]
 profile = black
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-phonenumber-field-7.0.2/tests/models.py` & `django-phonenumber-field-7.1.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/tests/test_formfields.py` & `django-phonenumber-field-7.1.0/tests/test_formfields.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/tests/test_phonenumber.py` & `django-phonenumber-field-7.1.0/tests/test_phonenumber.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/tests/test_serializers.py` & `django-phonenumber-field-7.1.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/tests/test_widgets.py` & `django-phonenumber-field-7.1.0/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/tests/tests.py` & `django-phonenumber-field-7.1.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-phonenumber-field-7.0.2/tox.ini` & `django-phonenumber-field-7.1.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tox]
 envlist =
     black
     flake8
     isort
     dj32
-    dj40
     dj41
+    dj42
     djmain
 isolated_build = true
 minversion = 1.9
 
 [testenv]
 deps =
     babel
     coverage
     dj32: Django>=3.2,<4.0
-    dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<4.3
     djmain: https://github.com/django/django/archive/main.tar.gz
     djangorestframework
 extras = phonenumberslite
 commands =
     coverage run --source phonenumber_field -m django test --settings=tests.settings {posargs}
     coverage xml -o coverage-reports/coverage.xml
     coverage html -d coverage-reports/html
```

