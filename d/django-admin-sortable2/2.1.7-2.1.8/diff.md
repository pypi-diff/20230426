# Comparing `tmp/django-admin-sortable2-2.1.7.tar.gz` & `tmp/django-admin-sortable2-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-sortable2-2.1.7.tar", last modified: Tue Apr 25 15:08:56 2023, max compression
+gzip compressed data, was "django-admin-sortable2-2.1.8.tar", last modified: Tue Apr 25 15:34:44 2023, max compression
```

## Comparing `django-admin-sortable2-2.1.7.tar` & `django-admin-sortable2-2.1.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.900704 django-admin-sortable2-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-25 15:08:56.900704 django-admin-sortable2-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/management/commands/reorder.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/css/sortable.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/icons/drag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/js/
--rw-r--r--   0 runner    (1001) docker     (123)   113660 2023-04-25 15:08:46.000000 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/js/adminsortable2.js
--rw-r--r--   0 runner    (1001) docker     (123)   191513 2023-04-25 15:08:46.000000 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/js/adminsortable2.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-04-25 15:08:48.000000 django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/js/adminsortable2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/adminsortable2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.896705 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.900704 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-25 15:08:49.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-25 15:08:49.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-25 15:08:49.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-25 15:08:49.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-25 15:08:49.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-25 15:08:49.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-25 15:08:49.000000 django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.900704 django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-25 15:08:56.000000 django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-25 15:08:56.000000 django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:08:56.000000 django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:08:56.000000 django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 15:08:56.000000 django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 15:08:56.000000 django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:08:56.900704 django-admin-sortable2-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.892704 django-admin-sortable2-2.1.7/testapp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:56.900704 django-admin-sortable2-2.1.7/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:08:28.000000 django-admin-sortable2-2.1.7/testapp/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/management/commands/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/css/sortable.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.501535 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/icons/drag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   113660 2023-04-25 15:34:34.000000 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/js/adminsortable2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   191513 2023-04-25 15:34:34.000000 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/js/adminsortable2.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-04-25 15:34:35.000000 django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/js/adminsortable2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/adminsortable2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-25 15:34:35.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-25 15:34:36.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-25 15:34:36.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-25 15:34:35.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-25 15:34:36.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-25 15:34:36.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-25 15:34:36.000000 django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-25 15:34:44.000000 django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-25 15:34:44.000000 django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:34:44.000000 django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:34:44.000000 django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 15:34:44.000000 django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 15:34:44.000000 django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.497535 django-admin-sortable2-2.1.8/testapp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:44.505535 django-admin-sortable2-2.1.8/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:34:10.000000 django-admin-sortable2-2.1.8/testapp/migrations/__init__.py
```

### Comparing `django-admin-sortable2-2.1.7/LICENSE` & `django-admin-sortable2-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/PKG-INFO` & `django-admin-sortable2-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-sortable2
-Version: 2.1.7
+Version: 2.1.8
 Summary: Generic drag-and-drop sorting for the List, the Stacked- and the Tabular-Inlines Views in the Django Admin
 Home-page: https://github.com/jrief/django-admin-sortable2
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django
 Platform: OS Independent
```

### Comparing `django-admin-sortable2-2.1.7/README.md` & `django-admin-sortable2-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/admin.py` & `django-admin-sortable2-2.1.8/adminsortable2/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/de/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.8/adminsortable2/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/de/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/en/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/es/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.8/adminsortable2/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/es/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/fr/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.8/adminsortable2/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/fr/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/it/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.8/adminsortable2/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/it/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/pl/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.8/adminsortable2/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/pl/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/ru/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.8/adminsortable2/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/ru/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/uk/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.8/adminsortable2/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/locale/uk/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.8/adminsortable2/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/management/commands/reorder.py` & `django-admin-sortable2-2.1.8/adminsortable2/management/commands/reorder.py`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/css/sortable.css` & `django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/css/sortable.css`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/icons/drag.png` & `django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/icons/drag.png`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/js/adminsortable2.js` & `django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/js/adminsortable2.js`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/js/adminsortable2.js.map` & `django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/js/adminsortable2.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/static/adminsortable2/js/adminsortable2.min.js` & `django-admin-sortable2-2.1.8/adminsortable2/static/adminsortable2/js/adminsortable2.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html` & `django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html` & `django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html` & `django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html` & `django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html` & `django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html` & `django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig` & `django-admin-sortable2-2.1.8/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/PKG-INFO` & `django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-sortable2
-Version: 2.1.7
+Version: 2.1.8
 Summary: Generic drag-and-drop sorting for the List, the Stacked- and the Tabular-Inlines Views in the Django Admin
 Home-page: https://github.com/jrief/django-admin-sortable2
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django
 Platform: OS Independent
```

### Comparing `django-admin-sortable2-2.1.7/django_admin_sortable2.egg-info/SOURCES.txt` & `django-admin-sortable2-2.1.8/django_admin_sortable2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/setup.py` & `django-admin-sortable2-2.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.7/testapp/migrations/0001_initial.py` & `django-admin-sortable2-2.1.8/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

