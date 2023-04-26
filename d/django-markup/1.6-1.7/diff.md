# Comparing `tmp/django-markup-1.6.tar.gz` & `tmp/django-markup-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-markup-1.6.tar", last modified: Sun Aug 14 09:03:01 2022, max compression
+gzip compressed data, was "django-markup-1.7.tar", last modified: Wed Apr 26 19:23:31 2023, max compression
```

## Comparing `django-markup-1.6.tar` & `django-markup-1.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/
--rw-r--r--   0 martin     (501) staff       (20)     2659 2022-08-14 08:53:51.000000 django-markup-1.6/CHANGELOG.rst
--rw-r--r--   0 martin     (501) staff       (20)     1534 2022-08-14 08:39:58.000000 django-markup-1.6/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)      266 2022-08-14 08:39:58.000000 django-markup-1.6/MANIFEST.in
--rw-r--r--   0 martin     (501) staff       (20)     6673 2022-08-14 09:03:01.000000 django-markup-1.6/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      553 2022-08-14 08:43:41.000000 django-markup-1.6/Pipfile
--rw-r--r--   0 martin     (501) staff       (20)    16398 2022-08-14 08:39:58.000000 django-markup-1.6/Pipfile.lock
--rw-r--r--   0 martin     (501) staff       (20)     1809 2022-08-14 09:00:50.000000 django-markup-1.6/README.rst
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1259 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/defaults.py
--rw-r--r--   0 martin     (501) staff       (20)     1053 2022-08-14 08:44:22.000000 django-markup-1.6/django_markup/fields.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup/filter/
--rw-r--r--   0 martin     (501) staff       (20)      288 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      235 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/creole_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      475 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/linebreaks_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     1360 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/markdown_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      237 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/none_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      897 2022-08-14 08:44:39.000000 django-markup-1.6/django_markup/filter/rst_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      246 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/smartypants_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      226 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/textile_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      206 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/filter/widont_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     3586 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/markup.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup/templatetags/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/templatetags/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      255 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/templatetags/markup_tags.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup/tests/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/__init__.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup/tests/files/
--rw-r--r--   0 martin     (501) staff       (20)       85 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/files/rst_header.txt
--rw-r--r--   0 martin     (501) staff       (20)      212 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/files/rst_header_expected.txt
--rw-r--r--   0 martin     (501) staff       (20)       64 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/files/rst_raw.txt
--rw-r--r--   0 martin     (501) staff       (20)       87 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/files/rst_with_pygments.txt
--rw-r--r--   0 martin     (501) staff       (20)      320 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/files/rst_with_pygments_expected.txt
--rw-r--r--   0 martin     (501) staff       (20)     1213 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/markup_strings.py
--rw-r--r--   0 martin     (501) staff       (20)      756 2022-08-14 08:48:00.000000 django-markup-1.6/django_markup/tests/settings.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup/tests/templates/
--rw-r--r--   0 martin     (501) staff       (20)       54 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/templates/test_templatetag.html
--rw-r--r--   0 martin     (501) staff       (20)       82 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/templates/test_templatetag_filterwrapper.html
--rw-r--r--   0 martin     (501) staff       (20)     2500 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/test_custom_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     4190 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/test_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     1960 2022-08-14 08:39:58.000000 django-markup-1.6/django_markup/tests/test_templatetag.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     6673 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1939 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2022-08-14 08:46:44.000000 django-markup-1.6/django_markup.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)      170 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       14 2022-08-14 09:03:01.000000 django-markup-1.6/django_markup.egg-info/top_level.txt
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/docs/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/docs/_static/
--rw-r--r--   0 martin     (501) staff       (20)     6488 2022-08-14 08:39:58.000000 django-markup-1.6/docs/_static/basic.css
--rw-r--r--   0 martin     (501) staff       (20)     3791 2022-08-14 08:39:58.000000 django-markup-1.6/docs/_static/default.css
--rw-r--r--   0 martin     (501) staff       (20)     2717 2022-08-14 08:39:58.000000 django-markup-1.6/docs/_static/pygments.css
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-08-14 09:03:01.000000 django-markup-1.6/docs/bundled_filter/
--rw-r--r--   0 martin     (501) staff       (20)      252 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/creole.rst
--rw-r--r--   0 martin     (501) staff       (20)      300 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/linebreaks.rst
--rw-r--r--   0 martin     (501) staff       (20)      418 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/markdown.rst
--rw-r--r--   0 martin     (501) staff       (20)      126 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/none.rst
--rw-r--r--   0 martin     (501) staff       (20)     2263 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/rst.rst
--rw-r--r--   0 martin     (501) staff       (20)      314 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/smartypants.rst
--rw-r--r--   0 martin     (501) staff       (20)      500 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/textile.rst
--rw-r--r--   0 martin     (501) staff       (20)      208 2022-08-14 08:39:58.000000 django-markup-1.6/docs/bundled_filter/widont.rst
--rw-r--r--   0 martin     (501) staff       (20)     6322 2022-08-14 08:39:58.000000 django-markup-1.6/docs/conf.py
--rw-r--r--   0 martin     (501) staff       (20)      384 2022-08-14 08:39:58.000000 django-markup-1.6/docs/configuration.rst
--rw-r--r--   0 martin     (501) staff       (20)     1211 2022-08-14 08:39:58.000000 django-markup-1.6/docs/filter.rst
--rw-r--r--   0 martin     (501) staff       (20)     1351 2022-08-14 08:39:58.000000 django-markup-1.6/docs/filter_settings.rst
--rw-r--r--   0 martin     (501) staff       (20)     2689 2022-08-14 08:39:58.000000 django-markup-1.6/docs/formatter.rst
--rw-r--r--   0 martin     (501) staff       (20)     1183 2022-08-14 08:39:58.000000 django-markup-1.6/docs/index.rst
--rw-r--r--   0 martin     (501) staff       (20)      773 2022-08-14 08:39:58.000000 django-markup-1.6/docs/installation.rst
--rw-r--r--   0 martin     (501) staff       (20)      759 2022-08-14 08:39:58.000000 django-markup-1.6/docs/usage_models.rst
--rw-r--r--   0 martin     (501) staff       (20)      107 2022-08-14 08:39:58.000000 django-markup-1.6/docs/usage_python.rst
--rw-r--r--   0 martin     (501) staff       (20)     1137 2022-08-14 08:39:58.000000 django-markup-1.6/docs/usage_templates.rst
--rw-r--r--   0 martin     (501) staff       (20)     1690 2022-08-14 09:03:01.000000 django-markup-1.6/setup.cfg
--rwxr-xr-x   0 martin     (501) staff       (20)       59 2022-08-14 08:39:58.000000 django-markup-1.6/setup.py
--rw-r--r--   0 martin     (501) staff       (20)      776 2022-08-14 08:48:42.000000 django-markup-1.6/tox.ini
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.108317 django-markup-1.7/
+-rw-r--r--   0 martin     (501) staff       (20)     2776 2023-04-26 19:19:16.000000 django-markup-1.7/CHANGELOG.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1534 2022-08-14 08:39:58.000000 django-markup-1.7/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)      266 2022-08-14 08:39:58.000000 django-markup-1.7/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     5564 2023-04-26 19:23:31.108415 django-markup-1.7/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      582 2023-04-26 19:09:41.000000 django-markup-1.7/Pipfile
+-rw-r--r--   0 martin     (501) staff       (20)    21963 2023-04-26 19:09:52.000000 django-markup-1.7/Pipfile.lock
+-rw-r--r--   0 martin     (501) staff       (20)     1888 2023-04-26 19:18:12.000000 django-markup-1.7/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.100173 django-markup-1.7/django_markup/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1259 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/defaults.py
+-rw-r--r--   0 martin     (501) staff       (20)     1053 2022-08-14 08:44:22.000000 django-markup-1.7/django_markup/fields.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.102571 django-markup-1.7/django_markup/filter/
+-rw-r--r--   0 martin     (501) staff       (20)      288 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      235 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/creole_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      475 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/linebreaks_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     1360 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/markdown_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      237 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/none_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      897 2022-08-14 08:44:39.000000 django-markup-1.7/django_markup/filter/rst_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      246 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/smartypants_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      226 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/textile_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      206 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/widont_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     3534 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/markup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.102853 django-markup-1.7/django_markup/templatetags/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/templatetags/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      255 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/templatetags/markup_tags.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.103725 django-markup-1.7/django_markup/tests/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/__init__.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.104496 django-markup-1.7/django_markup/tests/files/
+-rw-r--r--   0 martin     (501) staff       (20)       85 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_header.txt
+-rw-r--r--   0 martin     (501) staff       (20)      212 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_header_expected.txt
+-rw-r--r--   0 martin     (501) staff       (20)       64 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_raw.txt
+-rw-r--r--   0 martin     (501) staff       (20)       87 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_with_pygments.txt
+-rw-r--r--   0 martin     (501) staff       (20)      352 2023-04-26 19:13:49.000000 django-markup-1.7/django_markup/tests/files/rst_with_pygments_expected.txt
+-rw-r--r--   0 martin     (501) staff       (20)     1213 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/tests/markup_strings.py
+-rw-r--r--   0 martin     (501) staff       (20)      756 2022-08-14 08:48:00.000000 django-markup-1.7/django_markup/tests/settings.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.104805 django-markup-1.7/django_markup/tests/templates/
+-rw-r--r--   0 martin     (501) staff       (20)       54 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/templates/test_templatetag.html
+-rw-r--r--   0 martin     (501) staff       (20)       81 2023-04-26 19:13:10.000000 django-markup-1.7/django_markup/tests/templates/test_templatetag_filterwrapper.html
+-rw-r--r--   0 martin     (501) staff       (20)     2478 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/tests/test_custom_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     4169 2023-04-26 19:14:13.000000 django-markup-1.7/django_markup/tests/test_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     1960 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/tests/test_templatetag.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.101155 django-markup-1.7/django_markup.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     5564 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1939 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 18:45:56.000000 django-markup-1.7/django_markup.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)      171 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       14 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.106434 django-markup-1.7/docs/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.106951 django-markup-1.7/docs/_static/
+-rw-r--r--   0 martin     (501) staff       (20)     6488 2022-08-14 08:39:58.000000 django-markup-1.7/docs/_static/basic.css
+-rw-r--r--   0 martin     (501) staff       (20)     3791 2022-08-14 08:39:58.000000 django-markup-1.7/docs/_static/default.css
+-rw-r--r--   0 martin     (501) staff       (20)     2717 2022-08-14 08:39:58.000000 django-markup-1.7/docs/_static/pygments.css
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.108175 django-markup-1.7/docs/bundled_filter/
+-rw-r--r--   0 martin     (501) staff       (20)      252 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/creole.rst
+-rw-r--r--   0 martin     (501) staff       (20)      300 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/linebreaks.rst
+-rw-r--r--   0 martin     (501) staff       (20)      418 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/markdown.rst
+-rw-r--r--   0 martin     (501) staff       (20)      126 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/none.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2263 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/rst.rst
+-rw-r--r--   0 martin     (501) staff       (20)      314 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/smartypants.rst
+-rw-r--r--   0 martin     (501) staff       (20)      500 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/textile.rst
+-rw-r--r--   0 martin     (501) staff       (20)      208 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/widont.rst
+-rw-r--r--   0 martin     (501) staff       (20)     6322 2022-08-14 08:39:58.000000 django-markup-1.7/docs/conf.py
+-rw-r--r--   0 martin     (501) staff       (20)      384 2022-08-14 08:39:58.000000 django-markup-1.7/docs/configuration.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1211 2022-08-14 08:39:58.000000 django-markup-1.7/docs/filter.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1351 2022-08-14 08:39:58.000000 django-markup-1.7/docs/filter_settings.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2689 2022-08-14 08:39:58.000000 django-markup-1.7/docs/formatter.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1183 2022-08-14 08:39:58.000000 django-markup-1.7/docs/index.rst
+-rw-r--r--   0 martin     (501) staff       (20)      773 2022-08-14 08:39:58.000000 django-markup-1.7/docs/installation.rst
+-rw-r--r--   0 martin     (501) staff       (20)      759 2022-08-14 08:39:58.000000 django-markup-1.7/docs/usage_models.rst
+-rw-r--r--   0 martin     (501) staff       (20)      107 2022-08-14 08:39:58.000000 django-markup-1.7/docs/usage_python.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1137 2022-08-14 08:39:58.000000 django-markup-1.7/docs/usage_templates.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1691 2023-04-26 19:23:31.108852 django-markup-1.7/setup.cfg
+-rwxr-xr-x   0 martin     (501) staff       (20)       59 2023-04-26 19:06:37.000000 django-markup-1.7/setup.py
+-rw-r--r--   0 martin     (501) staff       (20)      793 2023-04-26 19:21:41.000000 django-markup-1.7/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-markup-1.6/CHANGELOG.rst` & `django-markup-1.7/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+v1.7 (2023-04-25):
+------------------
+
+- Django 4.2 compatibility and tests.
+- Python 3.11 compatibility and tests.
+
 v1.6 (2022-08-14):
 ------------------
 
 - Dropped support for Django <3.2 and Python <3.7.
 - Django 3.2 (LTS) compatibility and tests.
 - Django 4.0 compatibility and tests.
 - Django 4.1 compatibility and tests.
```

### Comparing `django-markup-1.6/LICENSE` & `django-markup-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/PKG-INFO` & `django-markup-1.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,185 +1,192 @@
 Metadata-Version: 2.1
 Name: django-markup
-Version: 1.6
+Version: 1.7
 Summary: A generic Django application to convert text with specific markup to html.
 Home-page: https://github.com/bartTC/django-markup
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
-Description: .. image:: https://img.shields.io/pypi/v/django-markup.svg
-            :target: https://pypi.org/project/django-markup/
-        
-        .. image:: https://github.com/bartTC/django-markup/actions/workflows/push.yml/badge.svg?branch=main
-            :target: https://github.com/bartTC/django-markup/actions
-        
-        ----
-        
-        📖 Full documentation on https://django-markup.readthedocs.io/en/latest/
-        
-        =============
-        django-markup
-        =============
-        
-        This app is a generic way to provide filters that convert text into html.
-        
-        Compatibility Matrix:
-        =====================
-        
-        ========= === === === ====
-        Py/Dj     3.7 3.8 3.9 3.10
-        ========= === === === ====
-        3.2 (LTS)  ✓   ✓   ✓   ✓
-        4.1            ✓   ✓   ✓
-        4.2            ✓   ✓   ✓
-        ========= === === === ====
-        
-        Quickstart
-        ==========
-        
-        Download and install the package from the python package index (pypi)::
-        
-            $ pip install django-markup
-        
-        Note that `django-markup` ships with some filters ready to use, but the more
-        complex packages such as Markdown or ReStructuredText are not part of the code.
-        Please refer the docs which packages are used for the built-in filter.
-        
-        An alternative is to install django-markup with all filter dependencies
-        right away. Do so with::
-        
-            $ pip install django-markup[all_filter_dependencies]
-        
-        Then add it to the ``INSTALLED_APPS`` list::
-        
-            INSTALLED_APPS = (
-                ...
-                'django_markup',
-            )
-        
-        Use it in the template::
-        
-            {% load markup_tags %}
-            {{ the_text|apply_markup:"markdown" }}
-        
-        Or in Python code::
-        
-            from django_markup.markup import formatter
-            formatter('Some *Markdown* text.', filter_name='markdown')
-        
-        Testsuite
-        =========
-        
-        To run the testsuite install the project with pipenv and run it::
-        
-            % pipenv install --dev
-            $ pipenv run test
-        
-        You can also test against a variation of Django and Python versions
-        using tox::
-        
-            $ tox
-        
-        Changelog
-        =========
-        
-        v1.6 (2022-08-14):
-        ------------------
-        
-        - Dropped support for Django <3.2 and Python <3.7.
-        - Django 3.2 (LTS) compatibility and tests.
-        - Django 4.0 compatibility and tests.
-        - Django 4.1 compatibility and tests.
-        - Python 3.9 compatibility and tests.
-        - Python 3.10 compatibility and tests.
-        
-        
-        v1.5 (2020-06-12):
-        ------------------
-        
-        - Dropped support for Django <=1.11 and Python <=3.5.
-        - Python 3.8 compatibility and tests.
-        - Django 3.0 compatibility and tests.
-        - bleach-whitelist dependency is no longer necessary as tags are now shipped
-          with the built-in markdown filter.
-        - Uses pytest for testing.
-        
-        v1.4 (2019-03-15):
-        ------------------
-        
-        - Markdown's safe_mode was deprecated and no longer functional, it's behavior
-          was replaced with bleach_.
-        - Pipfile support for local development and general code cleanup.
-        
-        .. _bleach: https://github.com/mozilla/bleach
-        
-        v1.3 (2018-09-07):
-        ------------------
-        
-        - Python 3.6 and 3.7 compatibility and tests.
-        - Django 2.0 and 2.1 compatibility and tests.
-        - The package setup script now provides the ability to install all filter
-          dependencies automatically. See the installation Readme for details.
-        
-        v1.2 (2017-03-18):
-        ------------------
-        
-        - Django 1.10 compatibility and tests.
-        - Updated all filter dependencies. most notably SmartyPants to v2.0
-          which changed it's API, so your project dependencies need to update it
-          as well.
-        
-        v1.1 (2016-05-02):
-        ------------------
-        
-        - The Markdown filter has the ``safe_mode`` option enabled by default.
-        - The RestructuredText filter has the file and raw content inclusion
-          disabled by default.
-        
-        v1.0 (2016-01-02):
-        ------------------
-        
-        - Removed some 5 year old dust
-        - Django 1.8+ compatible
-        - Tests
-        
-        Backwards incompatible changes:
-        
-        - Removed Pygments highlighting in the Markdown and RestructuredText filter.
-        - Removed CreoleParser library in favor of a pypi package.
-        - Removed Lightbox filter.
-        - The RestructuredText filter now renders level 1 and 2 headers.
-          See Github `Issue 14`_ for details and a backwards compatible workaround.
-        
-        v0.4 (2011-06-01):
-        ------------------
-        
-        - Added a widont filter
-        - MarkupField is South compatible.
-        - Tested with Django 1.3
-        
-        v0.3 (2009-07-29):
-        ------------------
-        
-        django-markup now ships with a builtin creole parser. Advantage is, that
-        the recently used Creoleparser library needs the Genshi lib, which needs
-        a c-compiler and so on. The builtin creole parser is a pure python library
-        without any dependencies and follows the wikicreole.org specifications.
-        django-markup uses the `WikiCreole library`_.
-        
-        .. _WikiCreole library: http://devel.sheep.art.pl/creole/
-        .. _Issue 14: https://github.com/bartTC/django-markup/issues/14
-        
 Keywords: django,markup,markdown,restructuredtext,format,text
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Provides-Extra: all_filter_dependencies
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-markup.svg
+    :target: https://pypi.org/project/django-markup/
+
+.. image:: https://github.com/bartTC/django-markup/actions/workflows/push.yml/badge.svg?branch=main
+    :target: https://github.com/bartTC/django-markup/actions
+
+----
+
+📖 Full documentation on https://django-markup.readthedocs.io/en/latest/
+
+=============
+django-markup
+=============
+
+This app is a generic way to provide filters that convert text into html.
+
+Compatibility Matrix:
+=====================
+
+========= === === === ==== ====
+Py/Dj     3.7 3.8 3.9 3.10 3.11
+========= === === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓   ✓    ✓
+4.0            ✓   ✓   ✓    ✓
+4.1            ✓   ✓   ✓    ✓
+4.2 (LTS)      ✓   ✓   ✓    ✓
+========= === === === ==== ====
+
+Quickstart
+==========
+
+Download and install the package from the python package index (pypi)::
+
+    $ pip install django-markup
+
+Note that `django-markup` ships with some filters ready to use, but the more
+complex packages such as Markdown or ReStructuredText are not part of the code.
+Please refer the docs which packages are used for the built-in filter.
+
+An alternative is to install django-markup with all filter dependencies
+right away. Do so with::
+
+    $ pip install django-markup[all_filter_dependencies]
+
+Then add it to the ``INSTALLED_APPS`` list::
+
+    INSTALLED_APPS = (
+        ...
+        'django_markup',
+    )
+
+Use it in the template::
+
+    {% load markup_tags %}
+    {{ the_text|apply_markup:"markdown" }}
+
+Or in Python code::
+
+    from django_markup.markup import formatter
+    formatter('Some *Markdown* text.', filter_name='markdown')
+
+Testsuite
+=========
+
+To run the testsuite install the project with pipenv and run it::
+
+    % pipenv install --dev
+    $ pipenv run test
+
+You can also test against a variation of Django and Python versions
+using tox::
+
+    $ tox
+
+Changelog
+=========
+
+v1.7 (2023-04-25):
+------------------
+
+- Django 4.2 compatibility and tests.
+- Python 3.11 compatibility and tests.
+
+v1.6 (2022-08-14):
+------------------
+
+- Dropped support for Django <3.2 and Python <3.7.
+- Django 3.2 (LTS) compatibility and tests.
+- Django 4.0 compatibility and tests.
+- Django 4.1 compatibility and tests.
+- Python 3.9 compatibility and tests.
+- Python 3.10 compatibility and tests.
+
+
+v1.5 (2020-06-12):
+------------------
+
+- Dropped support for Django <=1.11 and Python <=3.5.
+- Python 3.8 compatibility and tests.
+- Django 3.0 compatibility and tests.
+- bleach-whitelist dependency is no longer necessary as tags are now shipped
+  with the built-in markdown filter.
+- Uses pytest for testing.
+
+v1.4 (2019-03-15):
+------------------
+
+- Markdown's safe_mode was deprecated and no longer functional, it's behavior
+  was replaced with bleach_.
+- Pipfile support for local development and general code cleanup.
+
+.. _bleach: https://github.com/mozilla/bleach
+
+v1.3 (2018-09-07):
+------------------
+
+- Python 3.6 and 3.7 compatibility and tests.
+- Django 2.0 and 2.1 compatibility and tests.
+- The package setup script now provides the ability to install all filter
+  dependencies automatically. See the installation Readme for details.
+
+v1.2 (2017-03-18):
+------------------
+
+- Django 1.10 compatibility and tests.
+- Updated all filter dependencies. most notably SmartyPants to v2.0
+  which changed it's API, so your project dependencies need to update it
+  as well.
+
+v1.1 (2016-05-02):
+------------------
+
+- The Markdown filter has the ``safe_mode`` option enabled by default.
+- The RestructuredText filter has the file and raw content inclusion
+  disabled by default.
+
+v1.0 (2016-01-02):
+------------------
+
+- Removed some 5 year old dust
+- Django 1.8+ compatible
+- Tests
+
+Backwards incompatible changes:
+
+- Removed Pygments highlighting in the Markdown and RestructuredText filter.
+- Removed CreoleParser library in favor of a pypi package.
+- Removed Lightbox filter.
+- The RestructuredText filter now renders level 1 and 2 headers.
+  See Github `Issue 14`_ for details and a backwards compatible workaround.
+
+v0.4 (2011-06-01):
+------------------
+
+- Added a widont filter
+- MarkupField is South compatible.
+- Tested with Django 1.3
+
+v0.3 (2009-07-29):
+------------------
+
+django-markup now ships with a builtin creole parser. Advantage is, that
+the recently used Creoleparser library needs the Genshi lib, which needs
+a c-compiler and so on. The builtin creole parser is a pure python library
+without any dependencies and follows the wikicreole.org specifications.
+django-markup uses the `WikiCreole library`_.
+
+.. _WikiCreole library: http://devel.sheep.art.pl/creole/
+.. _Issue 14: https://github.com/bartTC/django-markup/issues/14
```

### Comparing `django-markup-1.6/Pipfile` & `django-markup-1.7/Pipfile`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 [dev-packages]
 isort = "*"
 black = "*"
 coverage = "*"
 pytest = "*"
 pytest-django = "*"
 pytest-cov = "*"
+wheel = "*"
+setuptools = "*"
 
 [scripts]
 cleanup = "sh -c \"black --exclude='/(migrations)/' django_markup && isort django_markup\""
 test = "sh -c \"coverage erase && pytest && coverage html && echo Coverage report in /tmp/coverage_report/django-markup/index.html\""
 
 [pipenv]
 allow_prereleases = true
```

### Comparing `django-markup-1.6/Pipfile.lock` & `django-markup-1.7/Pipfile.lock`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.741761982570806%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'a9360d4391ff9ebcf5de6e5f66b7247afb2f50fb5463b429facd33b61f868097'}}",*

 * * "'default'": "{'bleach': {'hashes': "*

 * *              "['sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414', "*

 * *              "'sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4'], "*

 * *              '\'version\': \'==6.0.0\', \'markers\': "python_version >= \'3.7\'", delete: '*

 * *              "['index']}, 'six': {'hashes': "*

 * *              "['sha256:1e61 […]*

```diff
@@ -1,298 +1,386 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "4d86bcb1fd47e76afebfb980f8f60baea29fa8d14f9dc14f24955f907cf42a95"
+            "sha256": "a9360d4391ff9ebcf5de6e5f66b7247afb2f50fb5463b429facd33b61f868097"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
+        "asgiref": {
+            "hashes": [
+                "sha256:71e68008da809b957b7ee4b43dbccff33d1b23519fb8344e33f049897077afac",
+                "sha256:9567dfe7bd8d3c8c892227827c41cce860b368104c3431da67a0c5a65a949506"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.6.0"
+        },
         "bleach": {
             "hashes": [
-                "sha256:6123ddc1052673e52bab52cdc955bcb57a015264a1c57d37bea2f6b817af0125",
-                "sha256:98b3170739e5e83dd9dc19633f074727ad848cbedb6026708c8ac2d3b697a433"
+                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
+                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
-            "index": "pypi",
-            "version": "==3.3.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==6.0.0"
+        },
+        "django": {
+            "hashes": [
+                "sha256:ad33ed68db9398f5dfb33282704925bce044bef4261cd4fb59e4e7f9ae505a78",
+                "sha256:c36e2ab12824e2ac36afa8b2515a70c53c7742f0d6eaefa7311ec379558db997"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==4.2"
         },
         "django-markup": {
             "editable": true,
             "extras": [
                 "all_filter_dependencies"
             ],
             "path": "."
         },
-        "packaging": {
+        "docutils": {
+            "hashes": [
+                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
+                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.19"
+        },
+        "html5lib": {
+            "hashes": [
+                "sha256:0d78f8fde1c230e99fe37986a60526d7049ed4bf8a9fadbad5f00e22e58e041d",
+                "sha256:b2e5b40261e20f354d198eae92afc10d750afb487ed5e50f9c4eaf07c184146f"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==1.1"
+        },
+        "markdown": {
+            "hashes": [
+                "sha256:065fd4df22da73a625f14890dd77eb8040edcbd68794bcd35943be14490608b2",
+                "sha256:8bf101198e004dc93e84a12a7395e31aac6a9c9942848ae1d99b9d72cf9b3520"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.4.3"
+        },
+        "pygments": {
+            "hashes": [
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
+        },
+        "python-creole": {
             "hashes": [
-                "sha256:5b327ac1320dc863dca72f4514ecc086f31186744b84a230374cc1fd776feae5",
-                "sha256:67714da7f7bc052e064859c05c595155bd1ee9f69f76557e21f051443c20947a"
+                "sha256:8f51d19fc1934acfa2d462c0c555a23167f45d8f695b80612904ca0c0da4a08f",
+                "sha256:f1c04931242b90df81700daf1bbb6fc690e0b5aed8d5cb54663866eff1dd8ac2"
             ],
-            "version": "==20.9"
+            "markers": "python_version >= '3.7' and python_full_version < '4.0.0'",
+            "version": "==1.5.0rc3"
         },
-        "pyparsing": {
+        "regex": {
             "hashes": [
-                "sha256:1c6409312ce2ce2997896af5756753778d5f1603666dba5587804f09ad82ed27",
-                "sha256:f4896b4cc085a1f8f8ae53a1a90db5a86b3825ff73eb974dffee3d9e701007f4"
+                "sha256:086afe222d58b88b62847bdbd92079b4699350b4acab892f88a935db5707c790",
+                "sha256:0b8eb1e3bca6b48dc721818a60ae83b8264d4089a4a41d62be6d05316ec38e15",
+                "sha256:11d00c31aeab9a6e0503bc77e73ed9f4527b3984279d997eb145d7c7be6268fd",
+                "sha256:11d1f2b7a0696dc0310de0efb51b1f4d813ad4401fe368e83c0c62f344429f98",
+                "sha256:1b1fc2632c01f42e06173d8dd9bb2e74ab9b0afa1d698058c867288d2c7a31f3",
+                "sha256:20abe0bdf03630fe92ccafc45a599bca8b3501f48d1de4f7d121153350a2f77d",
+                "sha256:22720024b90a6ba673a725dcc62e10fb1111b889305d7c6b887ac7466b74bedb",
+                "sha256:2472428efc4127374f494e570e36b30bb5e6b37d9a754f7667f7073e43b0abdd",
+                "sha256:25f0532fd0c53e96bad84664171969de9673b4131f2297f1db850d3918d58858",
+                "sha256:2848bf76673c83314068241c8d5b7fa9ad9bed866c979875a0e84039349e8fa7",
+                "sha256:37ae17d3be44c0b3f782c28ae9edd8b47c1f1776d4cabe87edc0b98e1f12b021",
+                "sha256:3cd9f5dd7b821f141d3a6ca0d5d9359b9221e4f051ca3139320adea9f1679691",
+                "sha256:4479f9e2abc03362df4045b1332d4a2b7885b245a30d4f4b051c4083b97d95d8",
+                "sha256:4c49552dc938e3588f63f8a78c86f3c9c75301e813bca0bef13bdb4b87ccf364",
+                "sha256:539dd010dc35af935b32f248099e38447bbffc10b59c2b542bceead2bed5c325",
+                "sha256:54c3fa855a3f7438149de3211738dd9b5f0c733f48b54ae05aa7fce83d48d858",
+                "sha256:55ae114da21b7a790b90255ea52d2aa3a0d121a646deb2d3c6a3194e722fc762",
+                "sha256:5ccfafd98473e007cebf7da10c1411035b7844f0f204015efd050601906dbb53",
+                "sha256:5fc33b27b1d800fc5b78d7f7d0f287e35079ecabe68e83d46930cf45690e1c8c",
+                "sha256:6560776ec19c83f3645bbc5db64a7a5816c9d8fb7ed7201c5bcd269323d88072",
+                "sha256:6572ff287176c0fb96568adb292674b421fa762153ed074d94b1d939ed92c253",
+                "sha256:6b190a339090e6af25f4a5fd9e77591f6d911cc7b96ecbb2114890b061be0ac1",
+                "sha256:7304863f3a652dab5e68e6fb1725d05ebab36ec0390676d1736e0571ebb713ef",
+                "sha256:75f288c60232a5339e0ff2fa05779a5e9c74e9fc085c81e931d4a264501e745b",
+                "sha256:7868b8f218bf69a2a15402fde08b08712213a1f4b85a156d90473a6fb6b12b09",
+                "sha256:787954f541ab95d8195d97b0b8cf1dc304424adb1e07365967e656b92b38a699",
+                "sha256:78ac8dd8e18800bb1f97aad0d73f68916592dddf233b99d2b5cabc562088503a",
+                "sha256:79e29fd62fa2f597a6754b247356bda14b866131a22444d67f907d6d341e10f3",
+                "sha256:845a5e2d84389c4ddada1a9b95c055320070f18bb76512608374aca00d22eca8",
+                "sha256:86b036f401895e854de9fefe061518e78d506d8a919cc250dc3416bca03f6f9a",
+                "sha256:87d9951f5a538dd1d016bdc0dcae59241d15fa94860964833a54d18197fcd134",
+                "sha256:8a9c63cde0eaa345795c0fdeb19dc62d22e378c50b0bc67bf4667cd5b482d98b",
+                "sha256:93f3f1aa608380fe294aa4cb82e2afda07a7598e828d0341e124b8fd9327c715",
+                "sha256:9bf4a5626f2a0ea006bf81e8963f498a57a47d58907eaa58f4b3e13be68759d8",
+                "sha256:9d764514d19b4edcc75fd8cb1423448ef393e8b6cbd94f38cab983ab1b75855d",
+                "sha256:a610e0adfcb0fc84ea25f6ea685e39e74cbcd9245a72a9a7aab85ff755a5ed27",
+                "sha256:a81c9ec59ca2303acd1ccd7b9ac409f1e478e40e96f8f79b943be476c5fdb8bb",
+                "sha256:b7006105b10b59971d3b248ad75acc3651c7e4cf54d81694df5a5130a3c3f7ea",
+                "sha256:c07ce8e9eee878a48ebeb32ee661b49504b85e164b05bebf25420705709fdd31",
+                "sha256:c125a02d22c555e68f7433bac8449992fa1cead525399f14e47c2d98f2f0e467",
+                "sha256:c37df2a060cb476d94c047b18572ee2b37c31f831df126c0da3cd9227b39253d",
+                "sha256:c869260aa62cee21c5eb171a466c0572b5e809213612ef8d495268cd2e34f20d",
+                "sha256:c88e8c226473b5549fe9616980ea7ca09289246cfbdf469241edf4741a620004",
+                "sha256:cd1671e9d5ac05ce6aa86874dd8dfa048824d1dbe73060851b310c6c1a201a96",
+                "sha256:cde09c4fdd070772aa2596d97e942eb775a478b32459e042e1be71b739d08b77",
+                "sha256:cf86b4328c204c3f315074a61bc1c06f8a75a8e102359f18ce99fbcbbf1951f0",
+                "sha256:d5bbe0e1511b844794a3be43d6c145001626ba9a6c1db8f84bdc724e91131d9d",
+                "sha256:d895b4c863059a4934d3e874b90998df774644a41b349ebb330f85f11b4ef2c0",
+                "sha256:db034255e72d2995cf581b14bb3fc9c00bdbe6822b49fcd4eef79e1d5f232618",
+                "sha256:dbb3f87e15d3dd76996d604af8678316ad2d7d20faa394e92d9394dfd621fd0c",
+                "sha256:dc80df325b43ffea5cdea2e3eaa97a44f3dd298262b1c7fe9dbb2a9522b956a7",
+                "sha256:dd7200b4c27b68cf9c9646da01647141c6db09f48cc5b51bc588deaf8e98a797",
+                "sha256:df45fac182ebc3c494460c644e853515cc24f5ad9da05f8ffb91da891bfee879",
+                "sha256:e152461e9a0aedec7d37fc66ec0fa635eca984777d3d3c3e36f53bf3d3ceb16e",
+                "sha256:e2396e0678167f2d0c197da942b0b3fb48fee2f0b5915a0feb84d11b6686afe6",
+                "sha256:e76b6fc0d8e9efa39100369a9b3379ce35e20f6c75365653cf58d282ad290f6f",
+                "sha256:ea3c0cb56eadbf4ab2277e7a095676370b3e46dbfc74d5c383bd87b0d6317910",
+                "sha256:ef3f528fe1cc3d139508fe1b22523745aa77b9d6cb5b0bf277f48788ee0b993f",
+                "sha256:fdf7ad455f1916b8ea5cdbc482d379f6daf93f3867b4232d14699867a5a13af7",
+                "sha256:fffe57312a358be6ec6baeb43d253c36e5790e436b7bf5b7a38df360363e88e9"
             ],
-            "version": "==3.0.0b2"
+            "markers": "implementation_name != 'pypy'",
+            "version": "==2023.3.23"
         },
         "six": {
             "hashes": [
-                "sha256:30639c035cdb23534cd4aa2dd52c3bf48f06e5f4a941509c8bafd8ce11080259",
-                "sha256:8b74bedcbbbaca38ff6d7491d76f2b06b3592611af620f8426e82dddb04a5ced"
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
+        },
+        "smartypants": {
+            "hashes": [
+                "sha256:8db97f7cbdf08d15b158a86037cd9e116b4cf37703d24e0419a0d64ca5808f0d"
             ],
-            "version": "==1.15.0"
+            "version": "==2.0.1"
+        },
+        "sqlparse": {
+            "hashes": [
+                "sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3",
+                "sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==0.4.4"
+        },
+        "textile": {
+            "hashes": [
+                "sha256:5894d78a321656a8f72414844c04b10477edd1e2e14f5b05aa1307f02cee9777",
+                "sha256:721696412627ee67f8619d16f4abf112536563a8a74a909eb73d122cb4803d39"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==4.0.2"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         }
     },
     "develop": {
-        "appdirs": {
-            "hashes": [
-                "sha256:7d5d0167b2b1ba821647616af46a749d1c653740dd0d2415100fe26e27afdf41",
-                "sha256:a841dacd6b99318a741b166adb07e19ee71a274450e68237b4650ca1055ab128"
-            ],
-            "version": "==1.4.4"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:31b2eced602aa8423c2aea9c76a724617ed67cf9513173fd3a4f03e3a929c7e6",
-                "sha256:832aa3cde19744e49938b91fea06d69ecb9e649c93ba974535d08ad92164f700"
-            ],
-            "version": "==20.3.0"
-        },
         "black": {
             "hashes": [
-                "sha256:1b30e59be925fafc1ee4565e5e08abef6b03fe455102883820fe5ee2e4734e0b",
-                "sha256:c2edb73a08e9e0e6f65a0e6af18b059b8b1cdd5bef997d7a0b181df93dc81539"
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
             ],
             "index": "pypi",
-            "version": "==19.10b0"
+            "version": "==23.3.0"
         },
         "click": {
             "hashes": [
-                "sha256:681c9380a24b22fec089c8e5ffe40aa16a0da79f248a26fe2481bfa8170bfcc1",
-                "sha256:e4315a188403c0258bbc4a4e31863e48fc301c4e95b8007a8eeda0391158df13"
+                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
+                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
-            "version": "==8.0.0a1"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.3"
         },
         "coverage": {
             "hashes": [
-                "sha256:00f1d23f4336efc3b311ed0d807feb45098fc86dee1ca13b3d6768cdab187c8a",
-                "sha256:01333e1bd22c59713ba8a79f088b3955946e293114479bbfc2e37d522be03355",
-                "sha256:0cb4be7e784dcdc050fc58ef05b71aa8e89b7e6636b99967fadbdba694cf2b65",
-                "sha256:0e61d9803d5851849c24f78227939c701ced6704f337cad0a91e0972c51c1ee7",
-                "sha256:1601e480b9b99697a570cea7ef749e88123c04b92d84cedaa01e117436b4a0a9",
-                "sha256:2742c7515b9eb368718cd091bad1a1b44135cc72468c731302b3d641895b83d1",
-                "sha256:2d27a3f742c98e5c6b461ee6ef7287400a1956c11421eb574d843d9ec1f772f0",
-                "sha256:402e1744733df483b93abbf209283898e9f0d67470707e3c7516d84f48524f55",
-                "sha256:5c542d1e62eece33c306d66fe0a5c4f7f7b3c08fecc46ead86d7916684b36d6c",
-                "sha256:5f2294dbf7875b991c381e3d5af2bcc3494d836affa52b809c91697449d0eda6",
-                "sha256:6402bd2fdedabbdb63a316308142597534ea8e1895f4e7d8bf7476c5e8751fef",
-                "sha256:66460ab1599d3cf894bb6baee8c684788819b71a5dc1e8fa2ecc152e5d752019",
-                "sha256:782caea581a6e9ff75eccda79287daefd1d2631cc09d642b6ee2d6da21fc0a4e",
-                "sha256:79a3cfd6346ce6c13145731d39db47b7a7b859c0272f02cdb89a3bdcbae233a0",
-                "sha256:7a5bdad4edec57b5fb8dae7d3ee58622d626fd3a0be0dfceda162a7035885ecf",
-                "sha256:8fa0cbc7ecad630e5b0f4f35b0f6ad419246b02bc750de7ac66db92667996d24",
-                "sha256:a027ef0492ede1e03a8054e3c37b8def89a1e3c471482e9f046906ba4f2aafd2",
-                "sha256:a3f3654d5734a3ece152636aad89f58afc9213c6520062db3978239db122f03c",
-                "sha256:a82b92b04a23d3c8a581fc049228bafde988abacba397d57ce95fe95e0338ab4",
-                "sha256:acf3763ed01af8410fc36afea23707d4ea58ba7e86a8ee915dfb9ceff9ef69d0",
-                "sha256:adeb4c5b608574a3d647011af36f7586811a2c1197c861aedb548dd2453b41cd",
-                "sha256:b83835506dfc185a319031cf853fa4bb1b3974b1f913f5bb1a0f3d98bdcded04",
-                "sha256:bb28a7245de68bf29f6fb199545d072d1036a1917dca17a1e75bbb919e14ee8e",
-                "sha256:bf9cb9a9fd8891e7efd2d44deb24b86d647394b9705b744ff6f8261e6f29a730",
-                "sha256:c317eaf5ff46a34305b202e73404f55f7389ef834b8dbf4da09b9b9b37f76dd2",
-                "sha256:dbe8c6ae7534b5b024296464f387d57c13caa942f6d8e6e0346f27e509f0f768",
-                "sha256:de807ae933cfb7f0c7d9d981a053772452217df2bf38e7e6267c9cbf9545a796",
-                "sha256:dead2ddede4c7ba6cb3a721870f5141c97dc7d85a079edb4bd8d88c3ad5b20c7",
-                "sha256:dec5202bfe6f672d4511086e125db035a52b00f1648d6407cc8e526912c0353a",
-                "sha256:e1ea316102ea1e1770724db01998d1603ed921c54a86a2efcb03428d5417e489",
-                "sha256:f90bfc4ad18450c80b024036eaf91e4a246ae287701aaa88eaebebf150868052"
+                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
+                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
+                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
+                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
+                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
+                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
+                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
+                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
+                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
+                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
+                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
+                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
+                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
+                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
+                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
+                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
+                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
+                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
+                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
+                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
+                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
+                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
+                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
+                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
+                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
+                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
+                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
+                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
+                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
+                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
+                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
+                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
+                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
+                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
+                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
+                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
+                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
+                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
+                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
+                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
+                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
+                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
+                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
+                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
+                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
+                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
+                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
+                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
+                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
+                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
+                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "index": "pypi",
-            "version": "==5.1"
+            "version": "==7.2.3"
+        },
+        "iniconfig": {
+            "hashes": [
+                "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
+                "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.0"
         },
         "isort": {
             "hashes": [
-                "sha256:54da7e92468955c4fceacd0c86bd0ec997b0e1ee80d97f67c35a78b719dccab1",
-                "sha256:6e811fcb295968434526407adb8796944f1988c5b65e8139058f2014cbe100fd"
+                "sha256:0ec8b74806e80fec33e6e7ba89d35e17b3eb1c4c74316ea44cf877cc26e8b118",
+                "sha256:cde11e804641edbe1b6b95d56582eb541f27eebc77864c6015545944bb0e9c76"
             ],
             "index": "pypi",
-            "version": "==4.3.21"
+            "version": "==6.0.0b2"
         },
-        "more-itertools": {
+        "mypy-extensions": {
             "hashes": [
-                "sha256:8e1a2a43b2f2727425f2b5839587ae37093f19153dc26c0927d1048ff6557330",
-                "sha256:b3a9005928e5bed54076e6e549c792b306fddfe72b2d1d22dd63d42d5d3899cf"
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
-            "version": "==8.6.0"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:5b327ac1320dc863dca72f4514ecc086f31186744b84a230374cc1fd776feae5",
-                "sha256:67714da7f7bc052e064859c05c595155bd1ee9f69f76557e21f051443c20947a"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "version": "==20.9"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
         },
         "pathspec": {
             "hashes": [
-                "sha256:86379d6b86d75816baba717e64b1a3a3469deb93bb76d613c9ce79edc5cb68fd",
-                "sha256:aa0cb481c4041bf52ffa7b0d8fa6cd3e88a2ca4879c533c9153882ee2556790d"
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
-            "version": "==0.8.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
         },
-        "pluggy": {
+        "platformdirs": {
             "hashes": [
-                "sha256:15b2acde666561e1298d71b523007ed7364de07029219b604cf808bfa1c765b0",
-                "sha256:966c145cd83c96502c3c3868f50408687b38434af77734af1e9ca461a4081d2d"
+                "sha256:01437886022decaf285d8972f9526397bfae2ac55480ed372ed6d9eca048870a",
+                "sha256:a5e1536e5ea4b1c238a1364da17ff2993d5bd28e15600c2c8224008aff6bbcad"
             ],
-            "version": "==0.13.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.4.0"
         },
-        "py": {
-            "hashes": [
-                "sha256:21b81bda15b66ef5e1a777a21c4dcd9c20ad3efd0b3f817e7a809035269e1bd3",
-                "sha256:3b80836aa6d1feeaa108e046da6423ab8f6ceda6468545ae8d02d9d58d18818a"
-            ],
-            "version": "==1.10.0"
-        },
-        "pyparsing": {
+        "pluggy": {
             "hashes": [
-                "sha256:1c6409312ce2ce2997896af5756753778d5f1603666dba5587804f09ad82ed27",
-                "sha256:f4896b4cc085a1f8f8ae53a1a90db5a86b3825ff73eb974dffee3d9e701007f4"
+                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
+                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
-            "version": "==3.0.0b2"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:5c0db86b698e8f170ba4582a492248919255fcd4c79b1ee64ace34301fb589a1",
-                "sha256:7979331bfcba207414f5e1263b5a0f8f521d0f457318836a7355531ed1a4c7d8"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
-            "version": "==5.4.3"
+            "version": "==7.3.1"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:b6a814b8ed6247bd81ff47f038511b57fe1ce7f4cc25b9106f1a4b106f1d9322",
-                "sha256:c87dfd8465d865655a8213859f1b4749b43448b5fae465cb981e16d52a811424"
+                "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
+                "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "index": "pypi",
-            "version": "==2.9.0"
+            "version": "==4.0.0"
         },
         "pytest-django": {
             "hashes": [
-                "sha256:64f99d565dd9497af412fcab2989fe40982c1282d4118ff422b407f3f7275ca5",
-                "sha256:664e5f42242e5e182519388f01b9f25d824a9feb7cd17d8f863c8d776f38baf9"
+                "sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e",
+                "sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2"
             ],
             "index": "pypi",
-            "version": "==3.9.0"
+            "version": "==4.5.2"
         },
-        "regex": {
+        "setuptools": {
             "hashes": [
-                "sha256:02951b7dacb123d8ea6da44fe45ddd084aa6777d4b2454fa0da61d569c6fa538",
-                "sha256:0d08e71e70c0237883d0bef12cad5145b84c3705e9c6a588b2a9c7080e5af2a4",
-                "sha256:1862a9d9194fae76a7aaf0150d5f2a8ec1da89e8b55890b1786b8f88a0f619dc",
-                "sha256:1ab79fcb02b930de09c76d024d279686ec5d532eb814fd0ed1e0051eb8bd2daa",
-                "sha256:1fa7ee9c2a0e30405e21031d07d7ba8617bc590d391adfc2b7f1e8b99f46f444",
-                "sha256:262c6825b309e6485ec2493ffc7e62a13cf13fb2a8b6d212f72bd53ad34118f1",
-                "sha256:2a11a3e90bd9901d70a5b31d7dd85114755a581a5da3fc996abfefa48aee78af",
-                "sha256:2c99e97d388cd0a8d30f7c514d67887d8021541b875baf09791a3baad48bb4f8",
-                "sha256:3128e30d83f2e70b0bed9b2a34e92707d0877e460b402faca908c6667092ada9",
-                "sha256:38c8fd190db64f513fe4e1baa59fed086ae71fa45083b6936b52d34df8f86a88",
-                "sha256:3bddc701bdd1efa0d5264d2649588cbfda549b2899dc8d50417e47a82e1387ba",
-                "sha256:4902e6aa086cbb224241adbc2f06235927d5cdacffb2425c73e6570e8d862364",
-                "sha256:49cae022fa13f09be91b2c880e58e14b6da5d10639ed45ca69b85faf039f7a4e",
-                "sha256:56e01daca75eae420bce184edd8bb341c8eebb19dd3bce7266332258f9fb9dd7",
-                "sha256:5862975b45d451b6db51c2e654990c1820523a5b07100fc6903e9c86575202a0",
-                "sha256:6a8ce43923c518c24a2579fda49f093f1397dad5d18346211e46f134fc624e31",
-                "sha256:6c54ce4b5d61a7129bad5c5dc279e222afd00e721bf92f9ef09e4fae28755683",
-                "sha256:6e4b08c6f8daca7d8f07c8d24e4331ae7953333dbd09c648ed6ebd24db5a10ee",
-                "sha256:717881211f46de3ab130b58ec0908267961fadc06e44f974466d1887f865bd5b",
-                "sha256:749078d1eb89484db5f34b4012092ad14b327944ee7f1c4f74d6279a6e4d1884",
-                "sha256:7913bd25f4ab274ba37bc97ad0e21c31004224ccb02765ad984eef43e04acc6c",
-                "sha256:7a25fcbeae08f96a754b45bdc050e1fb94b95cab046bf56b016c25e9ab127b3e",
-                "sha256:83d6b356e116ca119db8e7c6fc2983289d87b27b3fac238cfe5dca529d884562",
-                "sha256:8b882a78c320478b12ff024e81dc7d43c1462aa4a3341c754ee65d857a521f85",
-                "sha256:8f6a2229e8ad946e36815f2a03386bb8353d4bde368fdf8ca5f0cb97264d3b5c",
-                "sha256:9801c4c1d9ae6a70aeb2128e5b4b68c45d4f0af0d1535500884d644fa9b768c6",
-                "sha256:a15f64ae3a027b64496a71ab1f722355e570c3fac5ba2801cafce846bf5af01d",
-                "sha256:a3d748383762e56337c39ab35c6ed4deb88df5326f97a38946ddd19028ecce6b",
-                "sha256:a63f1a07932c9686d2d416fb295ec2c01ab246e89b4d58e5fa468089cab44b70",
-                "sha256:b2b1a5ddae3677d89b686e5c625fc5547c6e492bd755b520de5332773a8af06b",
-                "sha256:b2f4007bff007c96a173e24dcda236e5e83bde4358a557f9ccf5e014439eae4b",
-                "sha256:baf378ba6151f6e272824b86a774326f692bc2ef4cc5ce8d5bc76e38c813a55f",
-                "sha256:bafb01b4688833e099d79e7efd23f99172f501a15c44f21ea2118681473fdba0",
-                "sha256:bba349276b126947b014e50ab3316c027cac1495992f10e5682dc677b3dfa0c5",
-                "sha256:c084582d4215593f2f1d28b65d2a2f3aceff8342aa85afd7be23a9cad74a0de5",
-                "sha256:d1ebb090a426db66dd80df8ca85adc4abfcbad8a7c2e9a5ec7513ede522e0a8f",
-                "sha256:d2d8ce12b7c12c87e41123997ebaf1a5767a5be3ec545f64675388970f415e2e",
-                "sha256:e32f5f3d1b1c663af7f9c4c1e72e6ffe9a78c03a31e149259f531e0fed826512",
-                "sha256:e3faaf10a0d1e8e23a9b51d1900b72e1635c2d5b0e1bea1c18022486a8e2e52d",
-                "sha256:f7d29a6fc4760300f86ae329e3b6ca28ea9c20823df123a2ea8693e967b29917",
-                "sha256:f8f295db00ef5f8bae530fc39af0b40486ca6068733fb860b42115052206466f"
-            ],
-            "version": "==2020.11.13"
-        },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "version": "==0.10.2"
-        },
-        "typed-ast": {
-            "hashes": [
-                "sha256:07d49388d5bf7e863f7fa2f124b1b1d89d8aa0e2f7812faff0a5658c01c59aa1",
-                "sha256:14bf1522cdee369e8f5581238edac09150c765ec1cb33615855889cf33dcb92d",
-                "sha256:240296b27397e4e37874abb1df2a608a92df85cf3e2a04d0d4d61055c8305ba6",
-                "sha256:36d829b31ab67d6fcb30e185ec996e1f72b892255a745d3a82138c97d21ed1cd",
-                "sha256:37f48d46d733d57cc70fd5f30572d11ab8ed92da6e6b28e024e4a3edfb456e37",
-                "sha256:4c790331247081ea7c632a76d5b2a265e6d325ecd3179d06e9cf8d46d90dd151",
-                "sha256:5dcfc2e264bd8a1db8b11a892bd1647154ce03eeba94b461effe68790d8b8e07",
-                "sha256:7147e2a76c75f0f64c4319886e7639e490fee87c9d25cb1d4faef1d8cf83a440",
-                "sha256:7703620125e4fb79b64aa52427ec192822e9f45d37d4b6625ab37ef403e1df70",
-                "sha256:8368f83e93c7156ccd40e49a783a6a6850ca25b556c0fa0240ed0f659d2fe496",
-                "sha256:84aa6223d71012c68d577c83f4e7db50d11d6b1399a9c779046d75e24bed74ea",
-                "sha256:85f95aa97a35bdb2f2f7d10ec5bbdac0aeb9dafdaf88e17492da0504de2e6400",
-                "sha256:8db0e856712f79c45956da0c9a40ca4246abc3485ae0d7ecc86a20f5e4c09abc",
-                "sha256:9044ef2df88d7f33692ae3f18d3be63dec69c4fb1b5a4a9ac950f9b4ba571606",
-                "sha256:963c80b583b0661918718b095e02303d8078950b26cc00b5e5ea9ababe0de1fc",
-                "sha256:987f15737aba2ab5f3928c617ccf1ce412e2e321c77ab16ca5a293e7bbffd581",
-                "sha256:9ec45db0c766f196ae629e509f059ff05fc3148f9ffd28f3cfe75d4afb485412",
-                "sha256:9fc0b3cb5d1720e7141d103cf4819aea239f7d136acf9ee4a69b047b7986175a",
-                "sha256:a2c927c49f2029291fbabd673d51a2180038f8cd5a5b2f290f78c4516be48be2",
-                "sha256:a38878a223bdd37c9709d07cd357bb79f4c760b29210e14ad0fb395294583787",
-                "sha256:b4fcdcfa302538f70929eb7b392f536a237cbe2ed9cba88e3bf5027b39f5f77f",
-                "sha256:c0c74e5579af4b977c8b932f40a5464764b2f86681327410aa028a22d2f54937",
-                "sha256:c1c876fd795b36126f773db9cbb393f19808edd2637e00fd6caba0e25f2c7b64",
-                "sha256:c9aadc4924d4b5799112837b226160428524a9a45f830e0d0f184b19e4090487",
-                "sha256:cc7b98bf58167b7f2db91a4327da24fb93368838eb84a44c472283778fc2446b",
-                "sha256:cf54cfa843f297991b7388c281cb3855d911137223c6b6d2dd82a47ae5125a41",
-                "sha256:d003156bb6a59cda9050e983441b7fa2487f7800d76bdc065566b7d728b4581a",
-                "sha256:d175297e9533d8d37437abc14e8a83cbc68af93cc9c1c59c2c292ec59a0697a3",
-                "sha256:d746a437cdbca200622385305aedd9aef68e8a645e385cc483bdc5e488f07166",
-                "sha256:e683e409e5c45d5c9082dc1daf13f6374300806240719f95dc783d1fc942af10"
+                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
+                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
             ],
-            "version": "==1.4.2"
+            "index": "pypi",
+            "version": "==67.7.2"
         },
-        "wcwidth": {
+        "wheel": {
             "hashes": [
-                "sha256:beb4802a9cebb9144e99086eff703a642a13d6a0052920003a230f3294bbe784",
-                "sha256:c4d647b99872929fdb7bdcaa4fbe7f01413ed3d98077df798530e5b04f116c83"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
-            "version": "==0.2.5"
+            "index": "pypi",
+            "version": "==0.40.0"
         }
     }
 }
```

### Comparing `django-markup-1.6/README.rst` & `django-markup-1.7/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 =============
 
 This app is a generic way to provide filters that convert text into html.
 
 Compatibility Matrix:
 =====================
 
-========= === === === ====
-Py/Dj     3.7 3.8 3.9 3.10
-========= === === === ====
-3.2 (LTS)  ✓   ✓   ✓   ✓
-4.1            ✓   ✓   ✓
-4.2            ✓   ✓   ✓
-========= === === === ====
+========= === === === ==== ====
+Py/Dj     3.7 3.8 3.9 3.10 3.11
+========= === === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓   ✓    ✓
+4.0            ✓   ✓   ✓    ✓
+4.1            ✓   ✓   ✓    ✓
+4.2 (LTS)      ✓   ✓   ✓    ✓
+========= === === === ==== ====
 
 Quickstart
 ==========
 
 Download and install the package from the python package index (pypi)::
 
     $ pip install django-markup
```

### Comparing `django-markup-1.6/django_markup/defaults.py` & `django-markup-1.7/django_markup/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from django_markup.filter.textile_filter import TextileMarkupFilter
 from django_markup.filter.widont_filter import WidontMarkupFilter
 
 # MarkupFilter that get's loaded automatically
 # You can override this list within your settings: MARKUP_FILTER
 
 DEFAULT_MARKUP_FILTER = {
-    'creole': CreoleMarkupFilter,
-    'linebreaks': LinebreaksMarkupFilter,
-    'markdown': MarkdownMarkupFilter,
-    'none': NoneMarkupFilter,
-    'restructuredtext': RstMarkupFilter,
-    'smartypants': SmartyPantsMarkupFilter,
-    'textile': TextileMarkupFilter,
-    'widont': WidontMarkupFilter,
+    "creole": CreoleMarkupFilter,
+    "linebreaks": LinebreaksMarkupFilter,
+    "markdown": MarkdownMarkupFilter,
+    "none": NoneMarkupFilter,
+    "restructuredtext": RstMarkupFilter,
+    "smartypants": SmartyPantsMarkupFilter,
+    "textile": TextileMarkupFilter,
+    "widont": WidontMarkupFilter,
 }
 
 # MarkupFilter that are the default value for choices, used in the MarkupField
 # You can override this list within your settings: MARKUP_CHOICES
 
-DEFAULT_MARKUP_CHOICES = ('none', 'linebreaks', 'markdown', 'restructuredtext')
+DEFAULT_MARKUP_CHOICES = ("none", "linebreaks", "markdown", "restructuredtext")
```

### Comparing `django-markup-1.6/django_markup/fields.py` & `django-markup-1.7/django_markup/fields.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/django_markup/filter/markdown_filter.py` & `django-markup-1.7/django_markup/filter/markdown_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 
 class MarkdownMarkupFilter(MarkupFilter):
     """
     Applies Markdown conversion to a string, and returns the HTML.
     """
 
-    title = 'Markdown'
-    kwargs = {'safe_mode': True}
+    title = "Markdown"
+    kwargs = {"safe_mode": True}
 
     def render(self, text, **kwargs):
         if kwargs:
             self.kwargs.update(kwargs)
 
         from markdown import markdown
 
         text = markdown(text, **self.kwargs)
 
         # Markdowns safe_mode is deprecated. We replace it with  Bleach
         # to keep it backwards compatible.
         # https://python-markdown.github.io/change_log/release-2.6/#safe_mode-deprecated
-        if self.kwargs.get('safe_mode') is True:
+        if self.kwargs.get("safe_mode") is True:
             from bleach import clean
 
             # fmt: off
             markdown_tags = [
                 "h1", "h2", "h3", "h4", "h5", "h6",
                 "b", "i", "strong", "em", "tt",
                 "p", "br",
```

### Comparing `django-markup-1.6/django_markup/filter/rst_filter.py` & `django-markup-1.7/django_markup/filter/rst_filter.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/django_markup/markup.py` & `django-markup-1.7/django_markup/markup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 
 class MarkupFormatter(object):
     def __init__(self, load_defaults=True):
         self.filter_list = {}
 
         if load_defaults:
-            filter_list = getattr(
-                settings, 'MARKUP_FILTER', DEFAULT_MARKUP_FILTER
-            )
+            filter_list = getattr(settings, "MARKUP_FILTER", DEFAULT_MARKUP_FILTER)
             for filter_name, filter_class in filter_list.items():
                 self.register(filter_name, filter_class)
 
     def _get_filter_title(self, filter_name):
         """
         Returns the human readable title of a given filter_name. If no title
         attribute is set, the filter_name is used, where underscores are
@@ -25,26 +23,24 @@
 
         >>> MarkupFormatter._get_title('markdown')
         'Markdown'
 
         >>> MarkupFormatter._get_title('a_cool_filter_name')
         'A Cool Filter Name'
         """
-        title = getattr(self.filter_list[filter_name], 'title', None)
+        title = getattr(self.filter_list[filter_name], "title", None)
         if not title:
-            title = ' '.join([w.title() for w in filter_name.split('_')])
+            title = " ".join([w.title() for w in filter_name.split("_")])
         return title
 
     def choices(self):
         """
         Returns the filter list as a tuple. Useful for model choices.
         """
-        choice_list = getattr(
-            settings, 'MARKUP_CHOICES', DEFAULT_MARKUP_CHOICES
-        )
+        choice_list = getattr(settings, "MARKUP_CHOICES", DEFAULT_MARKUP_CHOICES)
         return [(f, self._get_filter_title(f)) for f in choice_list]
 
     def register(self, filter_name, filter_class):
         """
         Register a new filter for use
         """
         self.filter_list[filter_name] = filter_class
@@ -72,29 +68,29 @@
         """
         Applies text-to-HTML conversion to a string, and returns the
         HTML.
 
         TODO: `filter` should either be a filter_name or a filter class.
         """
 
-        filter_fallback = getattr(settings, 'MARKUP_FILTER_FALLBACK', False)
+        filter_fallback = getattr(settings, "MARKUP_FILTER_FALLBACK", False)
         if not filter_name and filter_fallback:
             filter_name = filter_fallback
 
         # Check that the filter_name is a registered markup filter
         if filter_name not in self.filter_list:
             raise ValueError(
                 "'%s' is not a registered markup filter. Registered filters are: %s."
-                % (filter_name, ', '.join(self.filter_list.keys()))
+                % (filter_name, ", ".join(self.filter_list.keys()))
             )
         filter_class = self.filter_list[filter_name]
 
         # Read global filter settings and apply it
         filter_kwargs = {}
-        filter_settings = getattr(settings, 'MARKUP_SETTINGS', {})
+        filter_settings = getattr(settings, "MARKUP_SETTINGS", {})
         if filter_name in filter_settings:
             filter_kwargs.update(filter_settings[filter_name])
         filter_kwargs.update(**kwargs)
 
         # Apply the filter on text
         return filter_class().render(text, **filter_kwargs)
```

### Comparing `django-markup-1.6/django_markup/tests/markup_strings.py` & `django-markup-1.7/django_markup/tests/markup_strings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from __future__ import unicode_literals
 
 """
 Sample Markup strings and their expected pendant.
 """
 
-NONE = ('*This* is some text.', '*This* is some text.')
+NONE = ("*This* is some text.", "*This* is some text.")
 
 # Django's linebreaks filter
-LINEBREAKS = ('*This* is some text.', '<p>*This* is some text.</p>')
+LINEBREAKS = ("*This* is some text.", "<p>*This* is some text.</p>")
 
 # Simple Markdown
-MARKDOWN = ('*This* is some text.', '<p><em>This</em> is some text.</p>')
+MARKDOWN = ("*This* is some text.", "<p><em>This</em> is some text.</p>")
 
 # Markdown with PRE tag
 MARKDOWN_PRE = (
-    '    code line 1\n    code line 2\n',
-    '<pre><code>code line 1\ncode line 2\n</code></pre>',
+    "    code line 1\n    code line 2\n",
+    "<pre><code>code line 1\ncode line 2\n</code></pre>",
 )
 
 # Simple Markdown
 MARKDOWN_JS_LINK = (
     '[Javascript Link](javascript:alert("123");)',
     '<p><a title="123">Javascript Link</a>;)</p>',
 )
 
 # Simple Textile
 TEXTILE = (
-    '*This* is some text.',
-    '\t<p><strong>This</strong> is some text.</p>',
+    "*This* is some text.",
+    "\t<p><strong>This</strong> is some text.</p>",
 )
 
 # Simple RestructuredText
 RST = (
-    '*This* is some text.',
+    "*This* is some text.",
     '<div class="document">\n<p><em>This</em> is some text.</p>\n</div>\n',
 )
 
 # Creole Sntax
 CREOLE = (
-    'This is **some //text//**.',
-    '<p>This is <strong>some <i>text</i></strong>.</p>',
+    "This is **some //text//**.",
+    "<p>This is <strong>some <i>text</i></strong>.</p>",
 )
 # Smartypants
-SMARTYPANTS = ('This is "some" text.', 'This is &#8220;some&#8221; text.')
+SMARTYPANTS = ('This is "some" text.', "This is &#8220;some&#8221; text.")
 
 # Windont
 WIDONT = (
-    'Widont does not leave anyone alone.',
-    'Widont does not leave anyone&nbsp;alone.',
+    "Widont does not leave anyone alone.",
+    "Widont does not leave anyone&nbsp;alone.",
 )
```

### Comparing `django-markup-1.6/django_markup/tests/settings.py` & `django-markup-1.7/django_markup/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/django_markup/tests/test_custom_filter.py` & `django-markup-1.7/django_markup/tests/test_custom_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,77 +7,75 @@
 
 
 class UppercaseMarkupFilter(MarkupFilter):
     """
     Custom filter that makes all the text uppercase.
     """
 
-    title = 'UppercaseFilter'
+    title = "UppercaseFilter"
 
     def render(self, text, **kwargs):
         return text.upper()
 
 
 class LowercaseMarkupFilter(MarkupFilter):
     """
     Custom filter that makes all the text lowercase.
     """
 
-    title = 'LowercaseFilter'
+    title = "LowercaseFilter"
 
     def render(self, text, **kwargs):
         return text.lower()
 
 
 class CustomMarkupFilterTestCase(TestCase):
     """
     Test the registration/unregistration of a custom filter.
     """
 
     def test_register_filter(self):
         """
         Register the filter, and its wildly available.
         """
-        formatter.register('uppercase', UppercaseMarkupFilter)
+        formatter.register("uppercase", UppercaseMarkupFilter)
 
         # It's ready to be called
-        result = formatter('This is some text', filter_name='uppercase')
-        self.assertEqual(result, 'THIS IS SOME TEXT')
+        result = formatter("This is some text", filter_name="uppercase")
+        self.assertEqual(result, "THIS IS SOME TEXT")
 
     def test_update_filter(self):
         """
         You can update an existing filter, but keep the name.
         """
-        formatter.update('uppercase', LowercaseMarkupFilter)
+        formatter.update("uppercase", LowercaseMarkupFilter)
 
         # Despite its key name is still 'uppercase' we actually call the
         # LowercaseFilter.
-        result = formatter('This Is Some Text', filter_name='uppercase')
-        self.assertEqual(result, 'this is some text')
+        result = formatter("This Is Some Text", filter_name="uppercase")
+        self.assertEqual(result, "this is some text")
 
     def test_unregister_filter(self):
         # Unregistering a filter that does not exist is simply ignored
-        formatter.unregister('does-not-exist')
+        formatter.unregister("does-not-exist")
 
         # Unregistering an registered filter, and it no longer works and will
         # raise a ValueError.
-        formatter.register('uppercase', UppercaseMarkupFilter)
-        formatter.unregister('uppercase')
+        formatter.register("uppercase", UppercaseMarkupFilter)
+        formatter.unregister("uppercase")
 
         self.assertRaises(
-            ValueError, formatter, 'This is some text', filter_name='uppercase'
+            ValueError, formatter, "This is some text", filter_name="uppercase"
         )
 
     def test_fallback_filter(self):
         """
         You can call the formatter without a `filter_name` as long as a
         `MARKUP_FILTER_FALLBACK` setting is set.
         """
-        self.assertRaises(
-            ValueError, formatter, 'This is some text', filter_name=None
-        )
+        self.assertRaises(ValueError, formatter, "This is some text", filter_name=None)
 
-        formatter.register('uppercase', UppercaseMarkupFilter)
+        formatter.register("uppercase", UppercaseMarkupFilter)
 
-        with self.settings(MARKUP_FILTER_FALLBACK='uppercase'):
-            result = formatter('This is some text', filter_name=None)
-            self.assertEqual(result, 'THIS IS SOME TEXT')
+        with self.settings(MARKUP_FILTER_FALLBACK="uppercase"):
+            result = formatter("This is some text", filter_name=None)
+            self.assertEqual(result, "THIS IS SOME TEXT")
```

### Comparing `django-markup-1.6/django_markup/tests/test_filter.py` & `django-markup-1.7/django_markup/tests/test_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,118 +3,117 @@
 import os
 
 from django.test import TestCase
 
 from ..markup import formatter
 from . import markup_strings as s
 
-FILES_DIR = os.path.join(os.path.dirname(__file__), 'files')
+FILES_DIR = os.path.join(os.path.dirname(__file__), "files")
 
 
 class FormatterTestCase(TestCase):
     """
     Test the Formatter conversion done in Python of all shipped filters.
     """
 
     def test_unregistered_filter_fails_loud(self):
         """
         Trying to call a unregistered filter will raise a ValueError.
         """
         self.assertRaises(
-            ValueError, formatter, 'some text', filter_name='does-not-exist'
+            ValueError, formatter, "some text", filter_name="does-not-exist"
         )
 
     def test_none_filter(self):
         text, expected = s.NONE
-        result = formatter(text, filter_name='none')
+        result = formatter(text, filter_name="none")
         self.assertEqual(result, expected)
 
     def test_linebreaks_filter(self):
         text, expected = s.LINEBREAKS
-        result = formatter(text, filter_name='linebreaks')
+        result = formatter(text, filter_name="linebreaks")
         self.assertEqual(result, expected)
 
     def test_markdown_filter(self):
         text, expected = s.MARKDOWN
-        result = formatter(text, filter_name='markdown')
+        result = formatter(text, filter_name="markdown")
         self.assertEqual(result, expected)
 
     def test_markdown_filter_pre(self):
         text, expected = s.MARKDOWN_PRE
-        result = formatter(text, filter_name='markdown')
+        result = formatter(text, filter_name="markdown")
         self.assertEqual(result, expected)
 
     def test_markdown_safemode_enabled_by_default(self):
         """Safe mode is enabled by default."""
         text, expected = s.MARKDOWN_JS_LINK
-        result = formatter(text, filter_name='markdown')
+        result = formatter(text, filter_name="markdown")
         self.assertEqual(result, expected)
 
     def test_textile_filter(self):
         text, expected = s.TEXTILE
-        result = formatter(text, filter_name='textile')
+        result = formatter(text, filter_name="textile")
         self.assertEqual(result, expected)
 
     def test_rst_filter(self):
         text, expected = s.RST
-        result = formatter(text, filter_name='restructuredtext')
+        result = formatter(text, filter_name="restructuredtext")
         self.assertEqual(result, expected)
 
     def test_rst_header_levels(self):
         """
         Make sure the rST filter fetches the entire document rather just the
         document fragment.
 
         :see: https://github.com/bartTC/django-markup/issues/14
         """
-        text = open(os.path.join(FILES_DIR, 'rst_header.txt')).read()
-        expected = open(
-            os.path.join(FILES_DIR, 'rst_header_expected.txt')
-        ).read()
-        result = formatter(text, filter_name='restructuredtext')
+        text = open(os.path.join(FILES_DIR, "rst_header.txt")).read()
+        expected = open(os.path.join(FILES_DIR, "rst_header_expected.txt")).read()
+        result = formatter(text, filter_name="restructuredtext")
         self.assertEqual(result, expected)
 
     def test_rst_with_pygments(self):
         """
         Having Pygments installed will automatically provide a ``.. code-block``
         directive in reStructredText to highlight code snippets.
         """
-        text = open(os.path.join(FILES_DIR, 'rst_with_pygments.txt')).read()
+        text = open(os.path.join(FILES_DIR, "rst_with_pygments.txt")).read()
         expected = open(
-            os.path.join(FILES_DIR, 'rst_with_pygments_expected.txt')
+            os.path.join(FILES_DIR, "rst_with_pygments_expected.txt")
         ).read()
-        result = formatter(text, filter_name='restructuredtext')
+        result = formatter(text, filter_name="restructuredtext")
+
         self.assertEqual(result, expected)
 
     def test_rst_raw_default(self):
         """Raw file inclusion is disabled by default."""
-        text = open(os.path.join(FILES_DIR, 'rst_raw.txt')).read()
-        result = formatter(text, filter_name='restructuredtext')
-        self.assertIn('Other text', result)
-        self.assertNotIn('<script>', result)
+        text = open(os.path.join(FILES_DIR, "rst_raw.txt")).read()
+        result = formatter(text, filter_name="restructuredtext")
+        self.assertIn("Other text", result)
+        self.assertNotIn("<script>", result)
 
     def test_rst_include_default(self):
         """File inclusion is disabled by default."""
         # Build up dynamically in order to build absolute path
         text = (
             ".. include:: "
-            + os.path.join(FILES_DIR, 'rst_header.txt')
+            + os.path.join(FILES_DIR, "rst_header.txt")
             + "\n\nOther text\n"
         )
-        result = formatter(text, filter_name='restructuredtext')
-        self.assertIn('Other text', result)
+        result = formatter(text, filter_name="restructuredtext")
+        self.assertIn("Other text", result)
         self.assertNotIn("Header 1", result)
 
     def test_creole_filter(self):
         text, expected = s.CREOLE
-        result = formatter(text, filter_name='creole')
+        result = formatter(text, filter_name="creole")
         self.assertEqual(result, expected)
 
     def test_smartypants_filter(self):
         text, expected = s.SMARTYPANTS
-        result = formatter(text, filter_name='smartypants')
+        result = formatter(text, filter_name="smartypants")
         self.assertEqual(result, expected)
 
     def test_widont_filter(self):
         text, expected = s.WIDONT
-        result = formatter(text, filter_name='widont')
+        result = formatter(text, filter_name="widont")
         self.assertEqual(result, expected)
```

### Comparing `django-markup-1.6/django_markup/tests/test_templatetag.py` & `django-markup-1.7/django_markup/tests/test_templatetag.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
     No need to test all filters here, since their low level routines are
     covered in `test_filter`.
     """
 
     def test_none_filter(self):
         text, expected = s.NONE
-        result = apply_markup(text, 'none')
+        result = apply_markup(text, "none")
         self.assertEqual(result, expected)
 
     def test_markdown_filter(self):
         text, expected = s.MARKDOWN
-        result = apply_markup(text, 'markdown')
+        result = apply_markup(text, "markdown")
         self.assertEqual(result, expected)
 
 
 class TemplateTagTestCase(TestCase):
     """
     Test the proper markup conversion using the template tag in a template itself.
     """
@@ -35,15 +35,15 @@
         """
         Test usage as a template tag:
 
             {{ "some text"|apply_markup:"markdown" }}
         """
         text, expected = s.MARKDOWN
         result = render_to_string(
-            'test_templatetag.html', {'text': text, 'filter': 'markdown'}
+            "test_templatetag.html", {"text": text, "filter": "markdown"}
         )
 
         # Strip leading and trailing whitespace from the rendered HTL
         result = result.strip()
 
         self.assertEqual(result, expected)
 
@@ -53,15 +53,15 @@
 
             {% filter apply_markup:"markdown" %}
                 some text
             {% endfilter %}
         """
         text, expected = s.MARKDOWN
         result = render_to_string(
-            'test_templatetag_filterwrapper.html',
-            {'text': text, 'filter': 'markdown'},
+            "test_templatetag_filterwrapper.html",
+            {"text": text, "filter": "markdown"},
         )
 
         # Strip leading and trailing whitespace from the rendered HTL
         result = result.strip()
 
         self.assertEqual(result, expected)
```

### Comparing `django-markup-1.6/django_markup.egg-info/PKG-INFO` & `django-markup-1.7/django_markup.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,185 +1,192 @@
 Metadata-Version: 2.1
 Name: django-markup
-Version: 1.6
+Version: 1.7
 Summary: A generic Django application to convert text with specific markup to html.
 Home-page: https://github.com/bartTC/django-markup
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
-Description: .. image:: https://img.shields.io/pypi/v/django-markup.svg
-            :target: https://pypi.org/project/django-markup/
-        
-        .. image:: https://github.com/bartTC/django-markup/actions/workflows/push.yml/badge.svg?branch=main
-            :target: https://github.com/bartTC/django-markup/actions
-        
-        ----
-        
-        📖 Full documentation on https://django-markup.readthedocs.io/en/latest/
-        
-        =============
-        django-markup
-        =============
-        
-        This app is a generic way to provide filters that convert text into html.
-        
-        Compatibility Matrix:
-        =====================
-        
-        ========= === === === ====
-        Py/Dj     3.7 3.8 3.9 3.10
-        ========= === === === ====
-        3.2 (LTS)  ✓   ✓   ✓   ✓
-        4.1            ✓   ✓   ✓
-        4.2            ✓   ✓   ✓
-        ========= === === === ====
-        
-        Quickstart
-        ==========
-        
-        Download and install the package from the python package index (pypi)::
-        
-            $ pip install django-markup
-        
-        Note that `django-markup` ships with some filters ready to use, but the more
-        complex packages such as Markdown or ReStructuredText are not part of the code.
-        Please refer the docs which packages are used for the built-in filter.
-        
-        An alternative is to install django-markup with all filter dependencies
-        right away. Do so with::
-        
-            $ pip install django-markup[all_filter_dependencies]
-        
-        Then add it to the ``INSTALLED_APPS`` list::
-        
-            INSTALLED_APPS = (
-                ...
-                'django_markup',
-            )
-        
-        Use it in the template::
-        
-            {% load markup_tags %}
-            {{ the_text|apply_markup:"markdown" }}
-        
-        Or in Python code::
-        
-            from django_markup.markup import formatter
-            formatter('Some *Markdown* text.', filter_name='markdown')
-        
-        Testsuite
-        =========
-        
-        To run the testsuite install the project with pipenv and run it::
-        
-            % pipenv install --dev
-            $ pipenv run test
-        
-        You can also test against a variation of Django and Python versions
-        using tox::
-        
-            $ tox
-        
-        Changelog
-        =========
-        
-        v1.6 (2022-08-14):
-        ------------------
-        
-        - Dropped support for Django <3.2 and Python <3.7.
-        - Django 3.2 (LTS) compatibility and tests.
-        - Django 4.0 compatibility and tests.
-        - Django 4.1 compatibility and tests.
-        - Python 3.9 compatibility and tests.
-        - Python 3.10 compatibility and tests.
-        
-        
-        v1.5 (2020-06-12):
-        ------------------
-        
-        - Dropped support for Django <=1.11 and Python <=3.5.
-        - Python 3.8 compatibility and tests.
-        - Django 3.0 compatibility and tests.
-        - bleach-whitelist dependency is no longer necessary as tags are now shipped
-          with the built-in markdown filter.
-        - Uses pytest for testing.
-        
-        v1.4 (2019-03-15):
-        ------------------
-        
-        - Markdown's safe_mode was deprecated and no longer functional, it's behavior
-          was replaced with bleach_.
-        - Pipfile support for local development and general code cleanup.
-        
-        .. _bleach: https://github.com/mozilla/bleach
-        
-        v1.3 (2018-09-07):
-        ------------------
-        
-        - Python 3.6 and 3.7 compatibility and tests.
-        - Django 2.0 and 2.1 compatibility and tests.
-        - The package setup script now provides the ability to install all filter
-          dependencies automatically. See the installation Readme for details.
-        
-        v1.2 (2017-03-18):
-        ------------------
-        
-        - Django 1.10 compatibility and tests.
-        - Updated all filter dependencies. most notably SmartyPants to v2.0
-          which changed it's API, so your project dependencies need to update it
-          as well.
-        
-        v1.1 (2016-05-02):
-        ------------------
-        
-        - The Markdown filter has the ``safe_mode`` option enabled by default.
-        - The RestructuredText filter has the file and raw content inclusion
-          disabled by default.
-        
-        v1.0 (2016-01-02):
-        ------------------
-        
-        - Removed some 5 year old dust
-        - Django 1.8+ compatible
-        - Tests
-        
-        Backwards incompatible changes:
-        
-        - Removed Pygments highlighting in the Markdown and RestructuredText filter.
-        - Removed CreoleParser library in favor of a pypi package.
-        - Removed Lightbox filter.
-        - The RestructuredText filter now renders level 1 and 2 headers.
-          See Github `Issue 14`_ for details and a backwards compatible workaround.
-        
-        v0.4 (2011-06-01):
-        ------------------
-        
-        - Added a widont filter
-        - MarkupField is South compatible.
-        - Tested with Django 1.3
-        
-        v0.3 (2009-07-29):
-        ------------------
-        
-        django-markup now ships with a builtin creole parser. Advantage is, that
-        the recently used Creoleparser library needs the Genshi lib, which needs
-        a c-compiler and so on. The builtin creole parser is a pure python library
-        without any dependencies and follows the wikicreole.org specifications.
-        django-markup uses the `WikiCreole library`_.
-        
-        .. _WikiCreole library: http://devel.sheep.art.pl/creole/
-        .. _Issue 14: https://github.com/bartTC/django-markup/issues/14
-        
 Keywords: django,markup,markdown,restructuredtext,format,text
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Provides-Extra: all_filter_dependencies
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-markup.svg
+    :target: https://pypi.org/project/django-markup/
+
+.. image:: https://github.com/bartTC/django-markup/actions/workflows/push.yml/badge.svg?branch=main
+    :target: https://github.com/bartTC/django-markup/actions
+
+----
+
+📖 Full documentation on https://django-markup.readthedocs.io/en/latest/
+
+=============
+django-markup
+=============
+
+This app is a generic way to provide filters that convert text into html.
+
+Compatibility Matrix:
+=====================
+
+========= === === === ==== ====
+Py/Dj     3.7 3.8 3.9 3.10 3.11
+========= === === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓   ✓    ✓
+4.0            ✓   ✓   ✓    ✓
+4.1            ✓   ✓   ✓    ✓
+4.2 (LTS)      ✓   ✓   ✓    ✓
+========= === === === ==== ====
+
+Quickstart
+==========
+
+Download and install the package from the python package index (pypi)::
+
+    $ pip install django-markup
+
+Note that `django-markup` ships with some filters ready to use, but the more
+complex packages such as Markdown or ReStructuredText are not part of the code.
+Please refer the docs which packages are used for the built-in filter.
+
+An alternative is to install django-markup with all filter dependencies
+right away. Do so with::
+
+    $ pip install django-markup[all_filter_dependencies]
+
+Then add it to the ``INSTALLED_APPS`` list::
+
+    INSTALLED_APPS = (
+        ...
+        'django_markup',
+    )
+
+Use it in the template::
+
+    {% load markup_tags %}
+    {{ the_text|apply_markup:"markdown" }}
+
+Or in Python code::
+
+    from django_markup.markup import formatter
+    formatter('Some *Markdown* text.', filter_name='markdown')
+
+Testsuite
+=========
+
+To run the testsuite install the project with pipenv and run it::
+
+    % pipenv install --dev
+    $ pipenv run test
+
+You can also test against a variation of Django and Python versions
+using tox::
+
+    $ tox
+
+Changelog
+=========
+
+v1.7 (2023-04-25):
+------------------
+
+- Django 4.2 compatibility and tests.
+- Python 3.11 compatibility and tests.
+
+v1.6 (2022-08-14):
+------------------
+
+- Dropped support for Django <3.2 and Python <3.7.
+- Django 3.2 (LTS) compatibility and tests.
+- Django 4.0 compatibility and tests.
+- Django 4.1 compatibility and tests.
+- Python 3.9 compatibility and tests.
+- Python 3.10 compatibility and tests.
+
+
+v1.5 (2020-06-12):
+------------------
+
+- Dropped support for Django <=1.11 and Python <=3.5.
+- Python 3.8 compatibility and tests.
+- Django 3.0 compatibility and tests.
+- bleach-whitelist dependency is no longer necessary as tags are now shipped
+  with the built-in markdown filter.
+- Uses pytest for testing.
+
+v1.4 (2019-03-15):
+------------------
+
+- Markdown's safe_mode was deprecated and no longer functional, it's behavior
+  was replaced with bleach_.
+- Pipfile support for local development and general code cleanup.
+
+.. _bleach: https://github.com/mozilla/bleach
+
+v1.3 (2018-09-07):
+------------------
+
+- Python 3.6 and 3.7 compatibility and tests.
+- Django 2.0 and 2.1 compatibility and tests.
+- The package setup script now provides the ability to install all filter
+  dependencies automatically. See the installation Readme for details.
+
+v1.2 (2017-03-18):
+------------------
+
+- Django 1.10 compatibility and tests.
+- Updated all filter dependencies. most notably SmartyPants to v2.0
+  which changed it's API, so your project dependencies need to update it
+  as well.
+
+v1.1 (2016-05-02):
+------------------
+
+- The Markdown filter has the ``safe_mode`` option enabled by default.
+- The RestructuredText filter has the file and raw content inclusion
+  disabled by default.
+
+v1.0 (2016-01-02):
+------------------
+
+- Removed some 5 year old dust
+- Django 1.8+ compatible
+- Tests
+
+Backwards incompatible changes:
+
+- Removed Pygments highlighting in the Markdown and RestructuredText filter.
+- Removed CreoleParser library in favor of a pypi package.
+- Removed Lightbox filter.
+- The RestructuredText filter now renders level 1 and 2 headers.
+  See Github `Issue 14`_ for details and a backwards compatible workaround.
+
+v0.4 (2011-06-01):
+------------------
+
+- Added a widont filter
+- MarkupField is South compatible.
+- Tested with Django 1.3
+
+v0.3 (2009-07-29):
+------------------
+
+django-markup now ships with a builtin creole parser. Advantage is, that
+the recently used Creoleparser library needs the Genshi lib, which needs
+a c-compiler and so on. The builtin creole parser is a pure python library
+without any dependencies and follows the wikicreole.org specifications.
+django-markup uses the `WikiCreole library`_.
+
+.. _WikiCreole library: http://devel.sheep.art.pl/creole/
+.. _Issue 14: https://github.com/bartTC/django-markup/issues/14
```

### Comparing `django-markup-1.6/django_markup.egg-info/SOURCES.txt` & `django-markup-1.7/django_markup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/_static/basic.css` & `django-markup-1.7/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/_static/default.css` & `django-markup-1.7/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/_static/pygments.css` & `django-markup-1.7/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/bundled_filter/rst.rst` & `django-markup-1.7/docs/bundled_filter/rst.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/conf.py` & `django-markup-1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/filter.rst` & `django-markup-1.7/docs/filter.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/filter_settings.rst` & `django-markup-1.7/docs/filter_settings.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/formatter.rst` & `django-markup-1.7/docs/formatter.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/index.rst` & `django-markup-1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/installation.rst` & `django-markup-1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/usage_models.rst` & `django-markup-1.7/docs/usage_models.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/docs/usage_templates.rst` & `django-markup-1.7/docs/usage_templates.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.6/setup.cfg` & `django-markup-1.7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-markup
-version = 1.6
+version = 1.7
 description = A generic Django application to convert text with specific markup to html.
 long_description = file: README.rst, CHANGELOG.rst
 author = Martin Mahner
 author_email = martin@mahner.org
 url = https://github.com/bartTC/django-markup
 keywords = django, markup, markdown, restructuredtext, format, text
 license = MIT
@@ -33,15 +33,15 @@
 	textile>=2.3.16
 	smartypants>=2.0.0
 	docutils>=0.14
 	pygments>=2.2.0
 	markdown>=2.6.9
 	bleach>=3.0
 	python-creole>=1.3.1
-	pygments>=2.2.0
+	pygments>=2.10.0
 
 [isort]
 known_first_party = django_markup
 default_section = THIRDPARTY
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 multi_line_output = 5
 skip = migrations
```

### Comparing `django-markup-1.6/tox.ini` & `django-markup-1.7/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tox]
 toxworkdir=/tmp/tox/django-markup
 skip_missing_interpreters=True
 envlist=
     readme
     py{37,38,39,310}-django-{32}
-    py{38,39,310}-django-{40,41}
+    py{38,39,310,311}-django-{40,41}
 
 [gh-actions]
 python =
     readme: py37
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
+    3.11: py311
 
 
 [testenv]
 commands=
-    py.test --pyargs --cov={envsitepackagesdir}/django_markup django_markup 
+    py.test --pyargs --cov={envsitepackagesdir}/django_markup django_markup
 extras=all_filter_dependencies
 deps=
     # Django versions
     django-32: django==3.2.*
     django-40: django==4.0.*
     django-41: django==4.1.*
     coverage
-    pytest 
-    pytest-cov 
+    pytest
+    pytest-cov
     pytest-Django
 
 [testenv:readme]
 skip_install = True
 deps =
     docutils
     Pygments
```

