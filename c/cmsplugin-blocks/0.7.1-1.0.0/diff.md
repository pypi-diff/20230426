# Comparing `tmp/cmsplugin-blocks-0.7.1.tar.gz` & `tmp/cmsplugin-blocks-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmsplugin-blocks-0.7.1.tar", last modified: Sat Jun  6 15:05:39 2020, max compression
+gzip compressed data, was "cmsplugin-blocks-1.0.0.tar", last modified: Wed Apr 26 20:11:24 2023, max compression
```

## Comparing `cmsplugin-blocks-0.7.1.tar` & `cmsplugin-blocks-1.0.0.tar`

### file list

```diff
@@ -1,97 +1,109 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2671 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2020-05-31 15:16:49.000000 cmsplugin-blocks-0.7.1/setup.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1981 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      337 2020-06-06 10:38:38.000000 cmsplugin-blocks-0.7.1/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1257 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/README.rst
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1057 2020-05-11 01:13:41.000000 cmsplugin-blocks-0.7.1/LICENCE.txt
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4081 2020-05-23 01:06:25.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/album/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      663 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/album/default.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/hero/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      365 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/hero/default.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/card/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      466 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/card/default.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/fileinputbutton/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1948 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/fileinputbutton/clearable_file_input.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      631 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/fileinputbutton/file.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/slider/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      988 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      773 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/cms_plugins.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1854 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/admin/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      896 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/admin/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1655 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1031 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      957 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1296 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/locale/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/locale/fr/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1926 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3560 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2927 2020-06-06 13:45:04.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/settings.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      803 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/exceptions.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1011 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      887 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      686 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      247 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1450 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/slider.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      411 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/user.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      699 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2815 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/smart_format.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      474 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2676 2020-05-11 01:00:50.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/validators.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2341 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/factories.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4501 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/archive.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6432 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/0001_initial.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1690 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      432 2020-05-11 00:46:37.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/0003_slideitem_title.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      471 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/0002_add_slide_item_order.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/forms/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2775 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/forms/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      723 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/forms/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      698 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/forms/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      349 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/forms/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1016 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/forms/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4163 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2807 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2311 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      305 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4460 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templatetags/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4793 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templatetags/smart_format.py
--rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2020-06-06 13:07:10.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/templatetags/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      709 2020-05-11 00:35:17.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/choices_helpers.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6092 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3705 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7532 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6092 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3675 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1557 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/js/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2736 2020-06-06 00:34:06.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks/widgets.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       25 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2834 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2671 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      159 2020-06-06 15:05:39.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2020-05-11 01:07:16.000000 cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/zip-safe
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1057 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      337 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.0.0/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3302 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1841 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      179 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1365 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1854 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/slider.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      598 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/apps.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1782 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/choices_helpers.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      839 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/cms_plugins.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/contrib/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/contrib/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2317 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/contrib/django_configuration.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3546 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/defaults.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      756 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/exceptions.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      418 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1752 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1297 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1119 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1028 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2090 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/slider.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/user.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      327 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3371 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      950 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      930 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      874 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1611 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/forms/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1926 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3560 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6408 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0001_initial.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      447 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0002_add_slide_item_order.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      432 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0003_slideitem_title.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1690 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10292 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-25 23:04:05.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2925 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/modelfields.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      271 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5838 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3855 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3555 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3285 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6136 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2078 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1776 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1582 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1369 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1579 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1246 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2577 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1557 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/js/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.777161 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4081 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       49 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      856 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.785160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      980 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       53 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1037 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       50 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1266 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      385 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4372 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/archive.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4859 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/cms_tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2558 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/factories.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7647 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4058 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/validators.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:24.781160 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3302 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3371 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      212 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       25 2023-04-26 20:11:24.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-24 20:19:54.000000 cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2200 2023-04-26 20:11:24.789160 cmsplugin-blocks-1.0.0/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cmsplugin-blocks-0.7.1/setup.cfg` & `cmsplugin-blocks-1.0.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,104 @@
 [metadata]
 name = cmsplugin-blocks
-version = 0.7.1
-description = A set of DjangoCMS plugins for content structures
+version = 1.0.0
+description = A set of DjangoCMS plugins for structured contents in CMS pages
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = dthenon@emencia.com
 url = https://github.com/emencia/cmsplugin-blocks
+project_urls = 
+	Source Code = https://github.com/emencia/cmsplugin-blocks
+	Issue Tracker = https://github.com/emencia/cmsplugin-blocks/issues
+	Changelog = https://cmspluginblocks.readthedocs.io/en/latest/history.html
+	Documentation = https://cmspluginblocks.readthedocs.io/
 license = MIT
-keywords = Django, Django-CMS, Structure, Content
+keywords = django, django-cms, structure, content
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
-	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.5
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Framework :: Django
-	Framework :: Django :: 2.0
-	Framework :: Django :: 2.1
-	Framework :: Django :: 2.2
-	Framework :: Django :: 3.0
+	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = True
 install_requires = 
-	django-cms>=3.6
-	djangocms-text-ckeditor>=3.6.1
-	sorl-thumbnail
+	django-cms>=3.11.0
+	djangocms-text-ckeditor>=5.0.1
+	django-smart-media
 packages = find:
 zip_safe = True
 
 [options.extras_require]
 dev = 
-	flake8
 	pytest
 	pytest-django
 	factory-boy
-	boussole
-	sphinx
-	sphinx-rtd-theme
+	pyquery
+quality = 
+	flake8
+	tox
+doc = 
+	sphinx>=4.3.0
+	sphinx-rtd-theme==1.1.0
 	livereload
+release = 
 	twine
 
 [options.packages.find]
 where = .
 exclude = 
 	data
 	docs
 	tests
 	sandbox
 
 [wheel]
-universal = 1
+universal = 0
 
 [flake8]
 max-line-length = 88
 exclude = 
 	.git,
 	.venv,
 	build,
-	venv,
-	__pycache__,
+	__pycache__
 	*/migrations/*
 
 [tool:pytest]
-django_settings_module = sandbox.settings.tests
+DJANGO_SETTINGS_MODULE = sandbox.settings.tests
 addopts = -vv
 python_files = 
 	*.py
 testpaths = 
 	tests
 
 [tox:tox]
 minversion = 3.4.0
-envlist = py35-django{20,21,22,30}-cms
+envlist = py{38,310}-django{32,40,41}-cms{311}
 
 [testenv]
 deps = 
-	django111: Django>=1.11,<2.0
-	django20: Django>=2.0,<2.1
-	django21: Django>=2.1,<2.2
-	django22: Django>=2.2,<2.3
-	django111-cms: django-cms>=3.5,<3.6
-	django20-cms: django-cms>=3.6,<3.7
-	django21-cms: django-cms>=3.7,<3.8
-	django22-cms: django-cms>=3.7,<3.8
-	django30-cms: django-cms>=3.7,<3.8
+	django32: Django>=3.2,<4.0
+	django40: Django>=4.0,<4.1
+	django41: Django>=4.1,<4.2
+	cms311: django-cms>=3.11.0,<4.0
+	py38-django32: backports.zoneinfo
 commands = 
 	pip install -e .[dev]
 	pytest -vv tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cmsplugin-blocks-0.7.1/LICENCE.txt` & `cmsplugin-blocks-1.0.0/LICENCE.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2020 Emencia.
+Copyright (c) 2017-2023 Emencia.
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-{% load i18n smart_format %}{% spaceless %}
-<div class="block slider">
-    <p class="slider__title">{{ instance.title }}</p>
+{% load i18n smart_image %}{% spaceless %}
+    <div class="slider{% if instance.features %} {{ instance.get_features }}{% endif %}">
+        <p class="slider__title">{{ instance.title }}</p>
 
-    <div class="slider__items">
-        {% for item in slides %}
-            {% media_thumb item.image "1200x400" as thumb %}
-            <div class="slider__item" style="background-image: url({{ thumb.url }})">
-                <p class="slider__item-title">{{ item.title }}</p>
-                {% if item.content %}<div class="slider__item-content">{{ item.content|safe }}</div>{% endif %}
+        <div class="slider__items">
+            {% for item in slides %}
+                {% media_thumb item.image "1200x400" as thumb %}
+                <div class="slider__item{% if item.features %} {{ item.get_features }}{% endif %}"
+                     style="background-image: url({{ thumb.url }})">
+                    <p class="slider__item-title">{{ item.title }}</p>
+                    {% if item.content %}
+                        <div class="slider__item-content">{{ item.content|safe }}</div>
+                    {% endif %}
 
-                {% if item.link_url %}
-                <p class="slider__item-link">
-                    <a href="{{ item.link_url }}" class="button"{% if item.link_open_blank %} target="_blank"{% endif %}>
-                        {% if item.link_name %}{{ item.link_name }}{% else %}{% trans "Read more" %}{% endif %}
-                    </a>
-                </p>
-                {% endif %}
-            </div>
-        {% endfor %}
+                    {% if item.link_url %}
+                        <p class="slider__item-link">
+                            <a href="{{ item.link_url }}" class="button"{% if item.link_open_blank %} target="_blank"{% endif %}>
+                                {% if item.link_name %}{{ item.link_name }}{% else %}{% trans "Read more" %}{% endif %}
+                            </a>
+                        </p>
+                    {% endif %}
+                </div>
+            {% endfor %}
+        </div>
     </div>
-</div>
 {% endspaceless %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% load i18n smart_format %}{% spaceless %}
+{% load i18n smart_image %}{% spaceless %}
 {{ instance.title }}
 {% for item in slides %} {% media_thumb item.image "1200x400" as thumb %}
 {{ item.title }}
 {% if item.content %}
 {{ item.content|safe }}
 {% endif %} {% if item.link_url %}
 % if item.link_open_blank %} target="_blank"{% endif %}> {% if item.link_name
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/cms_plugins.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/cms_plugins.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-# -*- coding: utf-8 -*-
 """
 CMS Plugins installations
 """
 from django.conf import settings
 
 from cms.plugin_pool import plugin_pool
 
-from cmsplugin_blocks.plugins.album import AlbumPlugin
-from cmsplugin_blocks.plugins.card import CardPlugin
-from cmsplugin_blocks.plugins.hero import HeroPlugin
-from cmsplugin_blocks.plugins.slider import SliderPlugin
+from .plugins.album import AlbumPlugin
+from .plugins.card import CardPlugin
+from .plugins.container import ContainerPlugin
+from .plugins.hero import HeroPlugin
+from .plugins.slider import SliderPlugin
 
 
 # Register enabled plugins
 if "AlbumPlugin" in settings.BLOCKS_ENABLED_PLUGINS:
     plugin_pool.register_plugin(AlbumPlugin)
 
 if "HeroPlugin" in settings.BLOCKS_ENABLED_PLUGINS:
     plugin_pool.register_plugin(HeroPlugin)
 
 if "CardPlugin" in settings.BLOCKS_ENABLED_PLUGINS:
     plugin_pool.register_plugin(CardPlugin)
 
+if "ContainerPlugin" in settings.BLOCKS_ENABLED_PLUGINS:
+    plugin_pool.register_plugin(ContainerPlugin)
+
 if "SliderPlugin" in settings.BLOCKS_ENABLED_PLUGINS:
     plugin_pool.register_plugin(SliderPlugin)
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/admin/slider.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/admin/slider.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,63 @@
-# -*- coding: utf-8 -*-
-"""
-Slider admin interface
-"""
 from django.contrib import admin
 from django.utils.translation import gettext_lazy as _
 
-from cmsplugin_blocks.models.slider import SlideItem
-from cmsplugin_blocks.forms.slider import SlideItemForm
+from smart_media.admin import SmartModelAdmin
+
+from ..choices_helpers import get_slideritem_feature_choices
+from ..models.slider import SlideItem
+from ..forms.slider import SlideItemForm
 
 
 class SlideItemAdmin(admin.StackedInline):
     """
     Plugin admin form to enable inline mode inside SliderPlugin
     """
     model = SlideItem
     form = SlideItemForm
     extra = 0
     verbose_name = _("Slide")
     ordering = ["order"]
-    fieldsets = (
-        (None, {
-            "fields": (
-                "slider",
-                "title",
-                (
-                    "image",
-                    "order",
-                ),
-                "content",
-                (
-                    "link_name",
-                    "link_url",
-                ),
-                "link_open_blank",
-            ),
-        }),
-    )
+    formfield_overrides = SmartModelAdmin.formfield_overrides
+
+    def get_fieldsets(self, request, obj=None):
+        if len(get_slideritem_feature_choices()) > 0:
+            fieldsets = (
+                (None, {
+                    "fields": (
+                        "slider",
+                        "title",
+                        (
+                            "image",
+                            "order",
+                            "features",
+                        ),
+                        "content",
+                        (
+                            "link_name",
+                            "link_url",
+                        ),
+                        "link_open_blank",
+                    ),
+                }),
+            )
+        else:
+            fieldsets = (
+                (None, {
+                    "fields": (
+                        "slider",
+                        "title",
+                        (
+                            "image",
+                            "order",
+                        ),
+                        "content",
+                        (
+                            "link_name",
+                            "link_url",
+                        ),
+                        "link_open_blank",
+                    ),
+                }),
+            )
+
+        return fieldsets
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/album.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/album.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,60 @@
-# -*- coding: utf-8 -*-
-"""
-CMS Plugin interface definitions
-"""
 from django.utils.translation import gettext_lazy as _
 
 from cms.plugin_base import CMSPluginBase
 
-from cmsplugin_blocks.admin.album import AlbumItemAdmin
-
-from cmsplugin_blocks.choices_helpers import get_album_default_template
-
-from cmsplugin_blocks.models.album import Album
-from cmsplugin_blocks.forms.album import AlbumForm
+from ..admin.album import AlbumItemAdmin
+from ..choices_helpers import (
+    get_album_feature_choices,
+    get_album_template_default,
+)
+from ..forms.album import AlbumForm
+from ..models.album import Album
 
 
 class AlbumPlugin(CMSPluginBase):
     """
     Album interface is able to add/edit/remove items within inline forms.
 
     Also used template is dynamically retrieved from "template" value.
     """
     module = _("Blocks")
     name = _("Album")
     model = Album
     form = AlbumForm
     inlines = (AlbumItemAdmin,)
-    render_template = get_album_default_template()
+    render_template = get_album_template_default()
     cache = True
-    fieldsets = (
-        (None, {
-            "fields": (
-                "title",
-                (
-                    "template",
-                    "mass_upload",
-                ),
-            ),
-        }),
-    )
+
+    def get_fieldsets(self, request, obj=None):
+        if len(get_album_feature_choices()) > 0:
+            fieldsets = (
+                (None, {
+                    "fields": (
+                        "title",
+                        (
+                            "template",
+                            "features",
+                        ),
+                        "mass_upload",
+                    ),
+                }),
+            )
+        else:
+            fieldsets = (
+                (None, {
+                    "fields": (
+                        "title",
+                        "template",
+                        "mass_upload",
+                    ),
+                }),
+            )
+
+        return fieldsets
 
     def render(self, context, instance, placeholder):
         context = super().render(context, instance, placeholder)
         self.render_template = instance.template
         ressources = instance.album_item.all().order_by("order")
         context.update({
             "instance": instance,
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/plugins/slider.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/plugins/hero.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,54 @@
-# -*- coding: utf-8 -*-
-"""
-Slider CMS Plugin interface definitions
-"""
 from django.utils.translation import gettext_lazy as _
 
 from cms.plugin_base import CMSPluginBase
 
-from cmsplugin_blocks.admin.slider import SlideItemAdmin
+from ..choices_helpers import (
+    get_hero_feature_choices,
+    get_hero_template_default,
+)
+from ..forms.hero import HeroForm
+from ..models.hero import Hero
 
-from cmsplugin_blocks.choices_helpers import get_slider_default_template
 
-from cmsplugin_blocks.models.slider import Slider
-from cmsplugin_blocks.forms.slider import SliderForm
-
-
-class SliderPlugin(CMSPluginBase):
-    """
-    Slider interface is able to add/edit/remove slide items as inline forms.
-
-    Also used template is dynamically retrieved from 'template' value.
-    """
+class HeroPlugin(CMSPluginBase):
     module = _("Blocks")
-    name = _("Slider")
-    model = Slider
-    form = SliderForm
-    inlines = (SlideItemAdmin,)
-    render_template = get_slider_default_template()
+    name = _("Hero")
+    model = Hero
+    form = HeroForm
+    render_template = get_hero_template_default()
     cache = True
-    fieldsets = (
-        (None, {
-            "fields": (
-                "title",
-                "template",
-            ),
-        }),
-    )
+
+    def get_fieldsets(self, request, obj=None):
+        if len(get_hero_feature_choices()) > 0:
+            fieldsets = (
+                (None, {
+                    "fields": (
+                        "template",
+                        "features",
+                        "image",
+                        "content",
+                    ),
+                }),
+            )
+        else:
+            fieldsets = (
+                (None, {
+                    "fields": (
+                        "template",
+                        "image",
+                        "content",
+                    ),
+                }),
+            )
+
+        return fieldsets
 
     def render(self, context, instance, placeholder):
         context = super().render(context, instance, placeholder)
         self.render_template = instance.template
-        slides = instance.slide_item.all().order_by("order")
+
         context.update({
             "instance": instance,
-            "slides": slides,
         })
+
         return context
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/exceptions.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-# -*- coding: utf-8 -*-
 """
-Exceptions
-==========
-
 Specific application exceptions.
 """
 
 
 class SmartFormatBaseException(Exception):
     """
     Base for every SmartFormat template tag exceptions.
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/hero.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/container.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,43 @@
-# -*- coding: utf-8 -*-
+import random
+
 import factory
 
-from cmsplugin_blocks.choices_helpers import get_hero_default_template
-from cmsplugin_blocks.utils.factories import create_image_file
-from cmsplugin_blocks.models import Hero
+from ..choices_helpers import (
+    get_container_feature_choices,
+    get_container_template_default,
+)
+from ..utils.factories import create_image_file
+from ..models import Container
 
 
-class HeroFactory(factory.django.DjangoModelFactory):
+class ContainerFactory(factory.django.DjangoModelFactory):
     """
-    Factory to create instance of a Hero.
+    Factory to create instance of a Container.
     """
-    template = get_hero_default_template()
+    title = factory.Faker("text", max_nb_chars=20)
+    template = get_container_template_default()
     content = factory.Faker("text", max_nb_chars=42)
 
     class Meta:
-        model = Hero
+        model = Container
+
+    @factory.lazy_attribute
+    def features(self):
+        """
+        Build features value with an item from feature choices.
+
+        If there is no feature choices available, just return an empty string.
+        """
+        choices = get_container_feature_choices()
+
+        if not choices:
+            return []
+
+        return [random.choice(choices)[0]]
 
     @factory.lazy_attribute
     def image(self):
         """
         Fill file field with generated image.
 
         Returns:
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/factories/slider.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/factories/card.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-# -*- coding: utf-8 -*-
 import random
-import factory
-
-from cmsplugin_blocks.choices_helpers import get_slider_default_template
-from cmsplugin_blocks.utils.factories import create_image_file
-from cmsplugin_blocks.models import Slider, SlideItem
 
+import factory
+import faker
 
-class SliderFactory(factory.django.DjangoModelFactory):
-    """
-    Factory to create instance of a Slider.
-    """
-    template = get_slider_default_template()
-    title = factory.Faker("text", max_nb_chars=20)
-
-    class Meta:
-        model = Slider
+from ..choices_helpers import (
+    get_card_feature_choices,
+    get_card_template_default,
+)
+from ..utils.factories import create_image_file
+from ..models import Card
 
 
-class SlideItemFactory(factory.django.DjangoModelFactory):
+class CardFactory(factory.django.DjangoModelFactory):
     """
-    Factory to create instance of a SlideItem.
+    Factory to create instance of a Card.
     """
-    slider = factory.SubFactory(SliderFactory)
     title = factory.Faker("text", max_nb_chars=20)
+    template = get_card_template_default()
     content = factory.Faker("text", max_nb_chars=42)
-    order = factory.Sequence(lambda n: 10 * n)
-    link_name = factory.Faker("text", max_nb_chars=10)
     link_open_blank = factory.Faker("pybool")
 
     class Meta:
-        model = SlideItem
+        model = Card
 
     @factory.lazy_attribute
-    def link_url(self):
+    def features(self):
         """
-        Set a random url or nothing, randomly
+        Build features value with an item from feature choices.
+
+        If there is no feature choices available, just return an empty string.
         """
-        trigger = random.choice([True, False])
+        choices = get_card_feature_choices()
 
-        if trigger:
-            return factory.Faker("url").generate({})
+        if not choices:
+            return []
 
-        return ""
+        return [random.choice(choices)[0]]
 
     @factory.lazy_attribute
     def image(self):
         """
         Fill file field with generated image.
 
         Returns:
             django.core.files.File: File object.
         """
 
         return create_image_file()
+
+    @factory.lazy_attribute
+    def link_url(self):
+        """
+        Set a random url
+        """
+        Faker = faker.Faker()
+        return Faker.url()
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/factories.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/factories.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,26 @@
-# -*- coding: utf-8 -*-
 import io
 
 from PIL import Image as PILimage
 
 from django.core.files import File
 
+import faker
+
+
+def get_fake_words(length=1):
+    """
+    Shortand to build a string of fake words depending given required count of
+    words.
+    """
+    Faker = faker.Faker()
+    words = Faker.words(nb=length)
+
+    return " ".join(words)
+
 
 def create_image_file(filename=None, size=(100, 100), color="blue",
                       format_name="PNG"):
     """
     Return a File object with a dummy generated image on the fly by PIL or
     possibly a SVG file.
 
@@ -42,15 +54,15 @@
 
     # Manage correct mode depending format
     mode = "RGB"
     if format_name == "PNG":
         mode = "RGBA"
 
     # Create a SVG file
-    if format_name == 'SVG':
+    if format_name == "SVG":
         width, height = size
         html = (
             """<svg xmlns="http://www.w3.org/2000/svg" """
             """viewBox="0 0 {width} {height}">"""
             """<path fill="{color}" d="M0 0h{width}v{height}H0z"/>"""
             """</svg>"""
         ).format(
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/utils/archive.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/utils/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-# -*- coding: utf-8 -*-
 import collections
 import logging
 
 from io import BytesIO
 
-# For Python 2/3 support
-try:
-    import Image as PILImage
-except ImportError:
-    from PIL import Image as PILImage
+from PIL import Image as PILimage
 
 from django.core.files.base import ContentFile
 
-from cmsplugin_blocks.utils.validators import is_valid_image_filename
+from .validators import is_valid_image_filename
 
 
 def store_images_from_zip(instance, zip_fileobject, item_model,
                           link_attrname, image_attrname,
                           label_attrname=None):
     """
     Collect every image from a ZIP as an item object linked to given
@@ -58,34 +53,34 @@
     logger = logging.getLogger("cmsplugin_blocks.utils")
 
     stored_items = []
 
     if zip_fileobject:
         for filename in sorted(zip_fileobject.namelist()):
             # Don't process invalid filename or directory
-            if filename.endswith('/') or not is_valid_image_filename(filename):
+            if filename.endswith("/") or not is_valid_image_filename(filename):
                 continue
 
             # Get archived file from ZIP
             data = zip_fileobject.read(filename)
             if len(data):
                 try:
                     # Following code is taken from
                     # django.forms.fields.ImageField: load() could spot a
                     # truncated JPEG, but it loads the entire image in memory,
                     # which is a DoS vector. See #3848 and #18520. verify()
                     # must be called immediately after the constructor.
-                    PILImage.open(BytesIO(data)).verify()
+                    PILimage.open(BytesIO(data)).verify()
                 except Exception as e:
                     # if a "bad" file is found we just skip it.
-                    msg = 'Error verifying image: {}'.format(str(e))
+                    msg = "Error verifying image: {}".format(str(e))
                     logger.error(msg)
                     continue
 
-                if hasattr(data, 'seek') and isinstance(data.seek,
+                if hasattr(data, "seek") and isinstance(data.seek,
                                                         collections.Callable):
                     data.seek(0)
 
                 try:
                     item = item_model(**{link_attrname: instance})
                     # Lazy save since we dont have album id yet when creating
                     getattr(
@@ -97,15 +92,15 @@
                         save=False
                     )
 
                     # Optional string field to fill from filename
                     if label_attrname:
                         setattr(item, label_attrname, filename)
                 except Exception as e:
-                    msg = 'Error creating item from file: {}'.format(str(e))
+                    msg = "Error creating item from file: {}".format(str(e))
                     logger.error(msg)
                 else:
                     # Store created item to be saved further in plugin
                     # 'save_model' method
                     stored_items.append(item)
 
         # Drop ZIP file object from memory/tempdir when finished
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/0001_initial.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0001_initial.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 # Generated by Django 1.10.8 on 2018-02-24 13:49
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 from cmsplugin_blocks.choices_helpers import (
-    get_album_default_template,
+    get_album_template_default,
     get_album_template_choices,
-    get_card_default_template,
+    get_card_template_default,
     get_card_template_choices,
-    get_hero_default_template,
+    get_hero_template_default,
     get_hero_template_choices,
-    get_slider_default_template,
+    get_slider_template_default,
     get_slider_template_choices
 )
 
 
 class Migration(migrations.Migration):
 
     initial = True
@@ -28,15 +27,15 @@
 
     operations = [
         migrations.CreateModel(
             name='Album',
             fields=[
                 ('cmsplugin_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, related_name='cmsplugin_blocks_album', serialize=False, to='cms.CMSPlugin')),
                 ('title', models.CharField(default='', max_length=150, verbose_name='Title')),
-                ('template', models.CharField(choices=get_album_template_choices(), default=get_album_default_template(), help_text='Used template for content formatting.', max_length=150, verbose_name='Template')),
+                ('template', models.CharField(choices=get_album_template_choices(), default=get_album_template_default(), help_text='Used template for content formatting.', max_length=150, verbose_name='Template')),
             ],
             options={
                 'verbose_name_plural': 'Albums',
                 'verbose_name': 'Album',
             },
             bases=('cms.cmsplugin',),
         ),
@@ -55,29 +54,29 @@
             },
         ),
         migrations.CreateModel(
             name='Card',
             fields=[
                 ('cmsplugin_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, related_name='cmsplugin_blocks_card', serialize=False, to='cms.CMSPlugin')),
                 ('alignment', models.CharField(choices=[('left', 'Content to the left, image to the right'), ('right', 'Image to the left, content to the reft')], default='left', max_length=15, verbose_name='Alignment')),
-                ('template', models.CharField(choices=get_card_template_choices(), default=get_card_default_template(), help_text='Used template for content look.', max_length=150, verbose_name='Template')),
+                ('template', models.CharField(choices=get_card_template_choices(), default=get_card_template_default(), help_text='Used template for content look.', max_length=150, verbose_name='Template')),
                 ('image', models.ImageField(blank=True, default=None, max_length=255, null=True, upload_to='blocks/card/%y/%m', verbose_name='Image')),
                 ('content', models.TextField(default='', verbose_name='Content')),
             ],
             options={
                 'verbose_name_plural': 'Cards',
                 'verbose_name': 'Card',
             },
             bases=('cms.cmsplugin',),
         ),
         migrations.CreateModel(
             name='Hero',
             fields=[
                 ('cmsplugin_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, related_name='cmsplugin_blocks_hero', serialize=False, to='cms.CMSPlugin')),
-                ('template', models.CharField(choices=get_hero_template_choices(), default=get_hero_default_template(), help_text='Used template for content look.', max_length=150, verbose_name='Template')),
+                ('template', models.CharField(choices=get_hero_template_choices(), default=get_hero_template_default(), help_text='Used template for content look.', max_length=150, verbose_name='Template')),
                 ('image', models.ImageField(blank=True, default=None, max_length=255, null=True, upload_to='blocks/hero/%y/%m', verbose_name='Image')),
                 ('content', models.TextField(default='', verbose_name='Content')),
             ],
             options={
                 'verbose_name_plural': 'Heros',
                 'verbose_name': 'Hero',
             },
@@ -99,15 +98,15 @@
             },
         ),
         migrations.CreateModel(
             name='Slider',
             fields=[
                 ('cmsplugin_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, related_name='cmsplugin_blocks_slider', serialize=False, to='cms.CMSPlugin')),
                 ('title', models.CharField(default='', max_length=150, verbose_name='Title')),
-                ('template', models.CharField(choices=get_slider_template_choices(), default=get_slider_default_template(), help_text='Used template for content look.', max_length=150, verbose_name='Template')),
+                ('template', models.CharField(choices=get_slider_template_choices(), default=get_slider_template_default(), help_text='Used template for content look.', max_length=150, verbose_name='Template')),
             ],
             options={
                 'verbose_name_plural': 'Sliders',
                 'verbose_name': 'Slider',
             },
             bases=('cms.cmsplugin',),
         ),
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/card.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/hero.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,69 @@
-# -*- coding: utf-8 -*-
 """
-====
-Card
-====
-
-A card component with a title, image and content. Optionally there is a choice
-to define a direction for content and image.
-
+A hero component with an image (commonly for background) and a content.
 """
 from django.conf import settings
-from django.core.validators import FileExtensionValidator
 from django.db import models
-from django.utils.encoding import force_text
+from django.db.models.signals import post_delete, pre_save
+from django.utils.encoding import force_str
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
-from cmsplugin_blocks.choices_helpers import (get_card_default_template,
-                                              get_card_template_choices)
-from cmsplugin_blocks.utils import SmartFormatMixin
-
+from smart_media.mixins import SmartFormatMixin
+from smart_media.modelfields import SmartMediaField
+from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+
+from ..choices_helpers import (
+    get_hero_feature_choices,
+    get_hero_template_choices,
+    get_hero_template_default,
+)
+from ..modelfields import CommaSeparatedStringsField
+from ..utils.validators import validate_css_classnames
 
-class Card(SmartFormatMixin, CMSPlugin):
-    """
-    Card component.
-    """
-    ALIGNMENT_CHOICES = [
-        ("left", _("Content to the left, image to the right")),
-        ("right", _("Image to the left, content to the reft")),
-    ]
 
-    alignment = models.CharField(
-        _("Alignment"),
-        choices=ALIGNMENT_CHOICES,
-        max_length=15,
-        blank=False,
-        default="left",
-    )
+class Hero(SmartFormatMixin, CMSPlugin):
     """
-    Content alignment choice, either content to the left and image to the right
-    or vice versa.
+    Hero component.
     """
-
     template = models.CharField(
         _("Template"),
         blank=False,
         max_length=150,
-        choices=get_card_template_choices(),
-        default=get_card_default_template(),
+        choices=get_hero_template_choices(),
+        default=get_hero_template_default(),
         help_text=_("Used template for content look."),
     )
     """
     Template choice from available plugin templates in setting
-    ``BLOCKS_CARD_TEMPLATES``. Default to the first choice item.
+    ``BLOCKS_HERO_TEMPLATES``. Default to the first choice item.
     """
 
-    image = models.FileField(
+    features = CommaSeparatedStringsField(
+        _("Layout features"),
+        choices=get_hero_feature_choices(),
+        blank=True,
+        default="",
+        max_length=255,
+        validators=[validate_css_classnames],
+    )
+    """
+    Optional string of CSS class names divided by a single comma.
+    """
+
+    image = SmartMediaField(
         _("Image"),
-        upload_to="blocks/card/%y/%m",
         max_length=255,
         blank=True,
         null=True,
         default=None,
-        validators=[
-            FileExtensionValidator(
-                allowed_extensions=settings.BLOCKS_ALLOWED_IMAGE_EXTENSIONS
-            ),
-        ]
+        upload_to="blocks/hero/%y/%m",
     )
     """
     Optional image file, limited to enabled image formats from settings
     ``BLOCKS_ALLOWED_IMAGE_EXTENSIONS``.
     """
 
     content = models.TextField(
@@ -82,21 +73,47 @@
     )
     """
     Required long text, it will be editable through CKeditor on plugin form.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.content = force_text(self.content)
+        self.content = force_str(self.content)
 
     def __str__(self):
         return Truncator(strip_tags(self.content)).words(
             settings.BLOCKS_MODEL_TRUNCATION_LENGTH,
             truncate=settings.BLOCKS_MODEL_TRUNCATION_CHR
         )
 
+    def get_features(self):
+        """
+        Merge feature items into a string with a comma divider.
+
+        Returns:
+            string: Feature items divided by a comma. Duplicate items are removed
+            and original order is preserved.
+        """
+        return " ".join(
+            list(dict.fromkeys(self.features))
+        )
+
     def get_image_format(self):
         return self.media_format(self.image)
 
     class Meta:
-        verbose_name = _("Card")
-        verbose_name_plural = _("Cards")
+        verbose_name = _("Hero")
+        verbose_name_plural = _("Heros")
+
+
+post_delete.connect(
+    auto_purge_files_on_delete(["image"]),
+    dispatch_uid="block_hero_files_on_delete",
+    sender=Hero,
+    weak=False,
+)
+pre_save.connect(
+    auto_purge_files_on_change(["image"]),
+    dispatch_uid="block_hero_files_on_change",
+    sender=Hero,
+    weak=False,
+)
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/hero.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/card.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,148 @@
-# -*- coding: utf-8 -*-
 """
-====
-Hero
-====
-
-A hero component with an image (commonly for background) and a content.
-
+A card component with a title, image, features and content.
 """
 from django.conf import settings
-from django.core.validators import FileExtensionValidator
 from django.db import models
-from django.utils.encoding import force_text
+from django.db.models.signals import post_delete, pre_save
+from django.utils.encoding import force_str
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
-from cmsplugin_blocks.choices_helpers import (get_hero_default_template,
-                                              get_hero_template_choices)
-from cmsplugin_blocks.utils import SmartFormatMixin
+from smart_media.mixins import SmartFormatMixin
+from smart_media.modelfields import SmartMediaField
+from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+
+from ..choices_helpers import (
+    get_card_feature_choices,
+    get_card_template_choices,
+    get_card_template_default,
+)
+from ..modelfields import CommaSeparatedStringsField
+from ..utils.validators import validate_css_classnames
+
 
+class Card(SmartFormatMixin, CMSPlugin):
+    """
+    Card component.
+    """
 
-class Hero(SmartFormatMixin, CMSPlugin):
+    title = models.CharField(
+        _("Title"),
+        blank=True,
+        max_length=150,
+        default="",
+    )
     """
-    Hero component.
+    An optional title string.
     """
+
     template = models.CharField(
         _("Template"),
         blank=False,
         max_length=150,
-        choices=get_hero_template_choices(),
-        default=get_hero_default_template(),
+        choices=get_card_template_choices(),
+        default=get_card_template_default(),
         help_text=_("Used template for content look."),
     )
     """
     Template choice from available plugin templates in setting
-    ``BLOCKS_HERO_TEMPLATES``. Default to the first choice item.
+    ``BLOCKS_CARD_TEMPLATES``. Default to the first choice item.
+    """
+
+    features = CommaSeparatedStringsField(
+        _("Layout features"),
+        choices=get_card_feature_choices(),
+        blank=True,
+        default="",
+        max_length=255,
+        validators=[validate_css_classnames],
+    )
+    """
+    Optional string of CSS class names divided by a single comma.
     """
 
-    image = models.FileField(
+    image = SmartMediaField(
         _("Image"),
-        upload_to="blocks/hero/%y/%m",
         max_length=255,
         blank=True,
         null=True,
         default=None,
-        validators=[
-            FileExtensionValidator(
-                allowed_extensions=settings.BLOCKS_ALLOWED_IMAGE_EXTENSIONS
-            ),
-        ]
+        upload_to="blocks/card/%y/%m",
     )
     """
     Optional image file, limited to enabled image formats from settings
     ``BLOCKS_ALLOWED_IMAGE_EXTENSIONS``.
     """
 
     content = models.TextField(
-        _(u"Content"),
+        _("Content"),
         blank=False,
         default="",
     )
     """
     Required long text, it will be editable through CKeditor on plugin form.
     """
 
+    link_url = models.CharField(
+        _("Link url"),
+        blank=True,
+        max_length=255,
+    )
+    """
+    Optional string for link URL.
+    """
+
+    link_open_blank = models.BooleanField(
+        _("Open in new window"),
+        default=False,
+        help_text=_("If checked the link will be opened in a new window"),
+    )
+    """
+    Checkbox to enable opening link URL in a new window/tab.
+    """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.content = force_text(self.content)
+        self.content = force_str(self.content)
 
     def __str__(self):
         return Truncator(strip_tags(self.content)).words(
             settings.BLOCKS_MODEL_TRUNCATION_LENGTH,
             truncate=settings.BLOCKS_MODEL_TRUNCATION_CHR
         )
 
     def get_image_format(self):
         return self.media_format(self.image)
 
+    def get_features(self):
+        """
+        Merge feature items into a string with a comma divider.
+
+        Returns:
+            string: Feature items divided by a comma. Duplicate items are removed
+            and original order is preserved.
+        """
+        return " ".join(
+            list(dict.fromkeys(self.features))
+        )
+
     class Meta:
-        verbose_name = _("Hero")
-        verbose_name_plural = _("Heros")
+        verbose_name = _("Card")
+        verbose_name_plural = _("Cards")
+
+
+post_delete.connect(
+    auto_purge_files_on_delete(["image"]),
+    dispatch_uid="block_card_files_on_delete",
+    sender=Card,
+    weak=False,
+)
+pre_save.connect(
+    auto_purge_files_on_change(["image"]),
+    dispatch_uid="block_card_files_on_change",
+    sender=Card,
+    weak=False,
+)
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/models/slider.py` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/models/container.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,131 @@
-# -*- coding: utf-8 -*-
 """
-======
-Slider
-======
-
-A slideshow component which may be similar to Album but with difference that
-a slide item can have HTML content.
-
-Slide items are ordered from their ``order`` field value. Items with a zero
-value for their order will be ordered in an almost arbitrary order (mostly
-depending from item object id).
-
+A container component with a title, image, features, content and able to include other
+plugins.
 """
 from django.conf import settings
-from django.core.validators import FileExtensionValidator
 from django.db import models
+from django.db.models.signals import post_delete, pre_save
+from django.utils.encoding import force_str
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
 
 from cms.models.pluginmodel import CMSPlugin
 
-from cmsplugin_blocks.choices_helpers import (get_slider_default_template,
-                                              get_slider_template_choices)
-from cmsplugin_blocks.utils import SmartFormatMixin
+from smart_media.mixins import SmartFormatMixin
+from smart_media.modelfields import SmartMediaField
+from smart_media.signals import auto_purge_files_on_change, auto_purge_files_on_delete
+
+from ..choices_helpers import (
+    get_container_feature_choices,
+    get_container_template_choices,
+    get_container_template_default,
+)
+from ..modelfields import CommaSeparatedStringsField
+from ..utils.validators import validate_css_classnames
 
 
-class Slider(CMSPlugin):
+class Container(SmartFormatMixin, CMSPlugin):
     """
-    Slide container for items.
+    Container component.
     """
+
     title = models.CharField(
         _("Title"),
-        blank=False,
+        blank=True,
         max_length=150,
         default="",
     )
     """
-    A required title string.
+    An optional title string.
     """
 
     template = models.CharField(
         _("Template"),
         blank=False,
         max_length=150,
-        choices=get_slider_template_choices(),
-        default=get_slider_default_template(),
+        choices=get_container_template_choices(),
+        default=get_container_template_default(),
         help_text=_("Used template for content look."),
     )
     """
     Template choice from available plugin templates in setting
-    ``BLOCKS_SLIDER_TEMPLATES``. Default to the first choice item.
-    """
-
-    def __str__(self):
-        return Truncator(strip_tags(self.title)).words(
-            settings.BLOCKS_MODEL_TRUNCATION_LENGTH,
-            truncate=settings.BLOCKS_MODEL_TRUNCATION_CHR
-        )
-
-    def copy_relations(self, oldinstance):
-        """
-        Copy FK relations when plugin object is copied as another object
-
-        See:
-
-        http://docs.django-cms.org/en/latest/how_to/custom_plugins.html#for-foreign-key-relations-from-other-objects
-
-        :meta private:
-        """
-        self.slide_item.all().delete()
-
-        for slide_item in oldinstance.slide_item.all():
-            slide_item.pk = None
-            slide_item.slider = self
-            slide_item.save()
-
-    class Meta:
-        verbose_name = _("Slider")
-        verbose_name_plural = _("Sliders")
-
-
-class SlideItem(SmartFormatMixin, models.Model):
+    ``BLOCKS_CONTAINER_TEMPLATES``. Default to the first choice item.
     """
-    Slide item to include in container.
-    """
-    slider = models.ForeignKey(
-        Slider,
-        related_name="slide_item",
-        on_delete=models.CASCADE
-    )
 
-    title = models.CharField(
-        _("Title"),
-        blank=False,
-        max_length=150,
-        default="",
-    )
-    """
-    Required title string.
-    """
-
-    image = models.FileField(
+    image = SmartMediaField(
         _("Image"),
-        upload_to="blocks/slider/%y/%m",
         max_length=255,
+        blank=True,
         null=True,
-        blank=False,
         default=None,
-        validators=[
-            FileExtensionValidator(
-                allowed_extensions=settings.BLOCKS_ALLOWED_IMAGE_EXTENSIONS
-            ),
-        ]
+        upload_to="blocks/container/%y/%m",
     )
     """
-    Required image file, limited to enabled image formats from settings
+    Optional image file, limited to enabled image formats from settings
     ``BLOCKS_ALLOWED_IMAGE_EXTENSIONS``.
     """
 
     content = models.TextField(
-        _(u"Content"),
+        _("Content"),
         blank=True,
         default="",
     )
     """
-    Optional long text, it will be editable through CKeditor on plugin form.
-    """
-
-    order = models.IntegerField(
-        _("Order"),
-        blank=False,
-        default=0
-    )
-    """
-    Number for order position in item list.
+    Required long text, it will be editable through CKeditor on plugin form.
     """
 
-    link_name = models.CharField(
-        _("link name"),
-        blank=True,
-        max_length=45,
-    )
-    """
-    Optional string for link name.
-    """
-
-    link_url = models.CharField(
-        _("link url"),
+    features = CommaSeparatedStringsField(
+        _("Layout features"),
+        choices=get_container_feature_choices(),
         blank=True,
+        default="",
         max_length=255,
+        validators=[validate_css_classnames],
     )
     """
-    Optional string for link URL.
+    Optional string of CSS class names divided by a single comma.
     """
 
-    link_open_blank = models.BooleanField(
-        _("open new window"),
-        default=False,
-        help_text=_("If checked the link will be open in a new window"),
-    )
-    """
-    Checkbox to enable opening link URL in a new window/tab.
-    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.content = force_str(self.content)
 
     def __str__(self):
-        return Truncator(strip_tags(self.title)).words(
+        return Truncator(strip_tags(self.content)).words(
             settings.BLOCKS_MODEL_TRUNCATION_LENGTH,
             truncate=settings.BLOCKS_MODEL_TRUNCATION_CHR
         )
 
     def get_image_format(self):
         return self.media_format(self.image)
 
+    def get_features(self):
+        """
+        Merge feature items into a string with a space divider.
+
+        Returns:
+            string: Feature items divided by a comma. Duplicate items are removed
+            and original order is preserved.
+        """
+        return " ".join(
+            list(dict.fromkeys(self.features))
+        )
+
     class Meta:
-        verbose_name = _("Slide item")
-        verbose_name_plural = _("Slide items")
+        verbose_name = _("Container")
+        verbose_name_plural = _("Containers")
+
+
+post_delete.connect(
+    auto_purge_files_on_delete(["image"]),
+    dispatch_uid="block_container_files_on_delete",
+    sender=Container,
+    weak=False,
+)
+pre_save.connect(
+    auto_purge_files_on_change(["image"]),
+    dispatch_uid="block_container_files_on_change",
+    sender=Container,
+    weak=False,
+)
```

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-0.7.1/cmsplugin_blocks.egg-info/SOURCES.txt` & `cmsplugin-blocks-1.0.0/cmsplugin_blocks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,81 @@
 LICENCE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 cmsplugin_blocks/__init__.py
+cmsplugin_blocks/apps.py
 cmsplugin_blocks/choices_helpers.py
 cmsplugin_blocks/cms_plugins.py
+cmsplugin_blocks/defaults.py
 cmsplugin_blocks/exceptions.py
-cmsplugin_blocks/settings.py
-cmsplugin_blocks/widgets.py
+cmsplugin_blocks/modelfields.py
 cmsplugin_blocks.egg-info/PKG-INFO
 cmsplugin_blocks.egg-info/SOURCES.txt
 cmsplugin_blocks.egg-info/dependency_links.txt
 cmsplugin_blocks.egg-info/requires.txt
 cmsplugin_blocks.egg-info/top_level.txt
 cmsplugin_blocks.egg-info/zip-safe
 cmsplugin_blocks/admin/__init__.py
 cmsplugin_blocks/admin/album.py
 cmsplugin_blocks/admin/slider.py
+cmsplugin_blocks/contrib/__init__.py
+cmsplugin_blocks/contrib/django_configuration.py
 cmsplugin_blocks/factories/__init__.py
 cmsplugin_blocks/factories/album.py
 cmsplugin_blocks/factories/card.py
+cmsplugin_blocks/factories/container.py
 cmsplugin_blocks/factories/hero.py
 cmsplugin_blocks/factories/slider.py
 cmsplugin_blocks/factories/user.py
 cmsplugin_blocks/forms/__init__.py
 cmsplugin_blocks/forms/album.py
 cmsplugin_blocks/forms/card.py
+cmsplugin_blocks/forms/container.py
 cmsplugin_blocks/forms/hero.py
 cmsplugin_blocks/forms/slider.py
 cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
 cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
 cmsplugin_blocks/migrations/0001_initial.py
 cmsplugin_blocks/migrations/0002_add_slide_item_order.py
 cmsplugin_blocks/migrations/0003_slideitem_title.py
 cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
+cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
 cmsplugin_blocks/migrations/__init__.py
 cmsplugin_blocks/models/__init__.py
 cmsplugin_blocks/models/album.py
 cmsplugin_blocks/models/card.py
+cmsplugin_blocks/models/container.py
 cmsplugin_blocks/models/hero.py
 cmsplugin_blocks/models/slider.py
 cmsplugin_blocks/plugins/__init__.py
 cmsplugin_blocks/plugins/album.py
 cmsplugin_blocks/plugins/card.py
+cmsplugin_blocks/plugins/container.py
 cmsplugin_blocks/plugins/hero.py
 cmsplugin_blocks/plugins/slider.py
 cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css
 cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css
 cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css
 cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css
+cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css
 cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css
 cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css
 cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js
 cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html
 cmsplugin_blocks/templates/cmsplugin_blocks/album/default.html
+cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html
 cmsplugin_blocks/templates/cmsplugin_blocks/card/default.html
-cmsplugin_blocks/templates/cmsplugin_blocks/fileinputbutton/clearable_file_input.html
-cmsplugin_blocks/templates/cmsplugin_blocks/fileinputbutton/file.html
+cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html
+cmsplugin_blocks/templates/cmsplugin_blocks/container/default.html
+cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html
 cmsplugin_blocks/templates/cmsplugin_blocks/hero/default.html
+cmsplugin_blocks/templates/cmsplugin_blocks/hero/test.html
 cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html
-cmsplugin_blocks/templatetags/__init__.py
-cmsplugin_blocks/templatetags/smart_format.py
+cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html
 cmsplugin_blocks/utils/__init__.py
 cmsplugin_blocks/utils/archive.py
+cmsplugin_blocks/utils/cms_tests.py
 cmsplugin_blocks/utils/factories.py
-cmsplugin_blocks/utils/smart_format.py
+cmsplugin_blocks/utils/tests.py
 cmsplugin_blocks/utils/validators.py
```

