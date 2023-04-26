# Comparing `tmp/aa_fleetfinder-1.1.0.tar.gz` & `tmp/aa_fleetfinder-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_fleetfinder-1.1.0.tar", last modified: Sun Apr 16 16:45:13 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa_fleetfinder-1.1.0.tar` & `aa_fleetfinder-1.2.0.tar`

### file list

```diff
@@ -1,106 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:13.001982 aa_fleetfinder-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-16 16:45:13.001982 aa_fleetfinder-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.989982 aa_fleetfinder-1.1.0/aa_fleetfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-16 16:45:12.000000 aa_fleetfinder-1.1.0/aa_fleetfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-16 16:45:12.000000 aa_fleetfinder-1.1.0/aa_fleetfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:45:12.000000 aa_fleetfinder-1.1.0/aa_fleetfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:45:12.000000 aa_fleetfinder-1.1.0/aa_fleetfinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 16:45:12.000000 aa_fleetfinder-1.1.0/aa_fleetfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 16:45:12.000000 aa_fleetfinder-1.1.0/aa_fleetfinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.989982 aa_fleetfinder-1.1.0/fleetfinder/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.981982 aa_fleetfinder-1.1.0/fleetfinder/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/css/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/css/fleetfinder.css
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/multi-select/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.993982 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35554 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.997982 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.997982 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/css/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.997982 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/js/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/create-fleet.html
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/edit-fleet.html
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/fleet-details.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/join-fleet.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.985982 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/partials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.997982 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.997982 aa_fleetfinder-1.1.0/fleetfinder/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/templatetags/fleetfinder_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:45:12.997982 aa_fleetfinder-1.1.0/fleetfinder/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/fleetfinder/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 16:44:51.000000 aa_fleetfinder-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-16 16:45:13.001982 aa_fleetfinder-1.1.0/setup.cfg
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/apps.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/auth_hooks.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/constants.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/models.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/providers.py
+-rw-r--r--   0        0        0    10216 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tasks.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/urls.py
+-rw-r--r--   0        0        0     9365 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/views.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/django.pot
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/migrations/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/fleetfinder.css
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
+-rw-r--r--   0        0        0    35554 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/base.html
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/create-fleet.html
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/dashboard.html
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/edit-fleet.html
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/fleet-details.html
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/join-fleet.html
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templatetags/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/templatetags/fleetfinder_versioned_static.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/__init__.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/test_access.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/fleetfinder/tests/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 aa_fleetfinder-1.2.0/PKG-INFO
```

### Comparing `aa_fleetfinder-1.1.0/LICENSE` & `aa_fleetfinder-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/PKG-INFO` & `aa_fleetfinder-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: aa_fleetfinder
-Version: 1.1.0
+Name: aa-fleetfinder
+Version: 1.2.0
 Summary: Fleet finder plugin for Alliance Auth
-Home-page: https://github.com/ppfeufer/aa-fleetfinder
-Author: Peter Pfeufer
-Author-email: develop@ppfeufer.de
-Maintainer: Peter Pfeufer
-Maintainer-email: develop@ppfeufer.de
-License: GPL-3.0
-Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-fleetfinder/issues
+Project-URL: Homepage, https://github.com/ppfeufer/aa-fleetfinder
+Project-URL: Documentation, https://github.com/ppfeufer/aa-fleetfinder/blob/master/README.md
+Project-URL: Source, https://github.com/ppfeufer/aa-fleetfinder.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetfinder/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://github.com/ppfeufer/aa-fleetfinder/issues
+Author-email: Peter Pfeufer <develop@ppfeufer.de>
+License-Expression: GPL-3.0
+License-File: LICENSE
 Keywords: allianceauth,eveonline,fleetfinder
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -22,16 +22,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
+Requires-Dist: allianceauth-app-utils>=1.14.2
+Requires-Dist: allianceauth>=3.0.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # AA Fleet Finder
 
 [![Version](https://img.shields.io/pypi/v/aa-fleetfinder?label=release)](https://pypi.org/project/aa-fleetfinder/)
 [![License](https://img.shields.io/github/license/ppfeufer/aa-fleetfinder)](https://github.com/ppfeufer/aa-fleetfinder/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/aa-fleetfinder)](https://pypi.org/project/aa-fleetfinder/)
 [![Django](https://img.shields.io/pypi/djversions/aa-fleetfinder?label=django)](https://pypi.org/project/aa-fleetfinder/)
```

### Comparing `aa_fleetfinder-1.1.0/README.md` & `aa_fleetfinder-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/auth_hooks.py` & `aa_fleetfinder-1.2.0/fleetfinder/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/constants.py` & `aa_fleetfinder-1.2.0/fleetfinder/constants.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/de/LC_MESSAGES/django.mo` & `aa_fleetfinder-1.2.0/fleetfinder/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/de/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/es/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/ja/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo` & `aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -6,17 +6,16 @@
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetfinder/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 4.16.4\n"
 
 msgid "<h4>Error!</h4><p>Fleet advert is no longer valid</p>"
 msgstr "<h4>Ошибка!</h4><p>Оповещение некорректно</p>"
 
 msgid "Available Fleets"
 msgstr "Доступные флота"
```

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/ru/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-12 08:35+0200\n"
-"PO-Revision-Date: 2023-04-16 16:11+0000\n"
+"PO-Revision-Date: 2023-04-21 14:50+0000\n"
 "Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetfinder/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || ("
-"n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 4.16.4\n"
 
 #: auth_hooks.py:25 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr "Поиск флота"
 
 #: templates/fleetfinder/create-fleet.html:14
```

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_fleetfinder-1.2.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/migrations/0001_initial.py` & `aa_fleetfinder-1.2.0/fleetfinder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/models.py` & `aa_fleetfinder-1.2.0/fleetfinder/models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/css/fleetfinder.css` & `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/css/fleetfinder.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js` & `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js` & `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css` & `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css` & `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js` & `aa_fleetfinder-1.2.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/tasks.py` & `aa_fleetfinder-1.2.0/fleetfinder/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/create-fleet.html` & `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/create-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/dashboard.html` & `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/edit-fleet.html` & `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/edit-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/fleet-details.html` & `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/join-fleet.html` & `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/join-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html` & `aa_fleetfinder-1.2.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/templatetags/fleetfinder_versioned_static.py` & `aa_fleetfinder-1.2.0/fleetfinder/templatetags/fleetfinder_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/tests/test_access.py` & `aa_fleetfinder-1.2.0/fleetfinder/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/tests/test_auth_hooks.py` & `aa_fleetfinder-1.2.0/fleetfinder/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/tests/test_templatetags.py` & `aa_fleetfinder-1.2.0/fleetfinder/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/tests/utils.py` & `aa_fleetfinder-1.2.0/fleetfinder/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/urls.py` & `aa_fleetfinder-1.2.0/fleetfinder/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.1.0/fleetfinder/views.py` & `aa_fleetfinder-1.2.0/fleetfinder/views.py`

 * *Files identical despite different names*

