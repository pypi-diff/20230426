# Comparing `tmp/django-markup-1.7.tar.gz` & `tmp/django-markup-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-markup-1.7.tar", last modified: Wed Apr 26 19:23:31 2023, max compression
+gzip compressed data, was "django-markup-1.7.1.tar", last modified: Wed Apr 26 19:28:29 2023, max compression
```

## Comparing `django-markup-1.7.tar` & `django-markup-1.7.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.108317 django-markup-1.7/
--rw-r--r--   0 martin     (501) staff       (20)     2776 2023-04-26 19:19:16.000000 django-markup-1.7/CHANGELOG.rst
--rw-r--r--   0 martin     (501) staff       (20)     1534 2022-08-14 08:39:58.000000 django-markup-1.7/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)      266 2022-08-14 08:39:58.000000 django-markup-1.7/MANIFEST.in
--rw-r--r--   0 martin     (501) staff       (20)     5564 2023-04-26 19:23:31.108415 django-markup-1.7/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      582 2023-04-26 19:09:41.000000 django-markup-1.7/Pipfile
--rw-r--r--   0 martin     (501) staff       (20)    21963 2023-04-26 19:09:52.000000 django-markup-1.7/Pipfile.lock
--rw-r--r--   0 martin     (501) staff       (20)     1888 2023-04-26 19:18:12.000000 django-markup-1.7/README.rst
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.100173 django-markup-1.7/django_markup/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1259 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/defaults.py
--rw-r--r--   0 martin     (501) staff       (20)     1053 2022-08-14 08:44:22.000000 django-markup-1.7/django_markup/fields.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.102571 django-markup-1.7/django_markup/filter/
--rw-r--r--   0 martin     (501) staff       (20)      288 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      235 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/creole_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      475 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/linebreaks_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     1360 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/markdown_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      237 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/none_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      897 2022-08-14 08:44:39.000000 django-markup-1.7/django_markup/filter/rst_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      246 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/smartypants_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      226 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/textile_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      206 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/filter/widont_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     3534 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/markup.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.102853 django-markup-1.7/django_markup/templatetags/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/templatetags/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      255 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/templatetags/markup_tags.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.103725 django-markup-1.7/django_markup/tests/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/__init__.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.104496 django-markup-1.7/django_markup/tests/files/
--rw-r--r--   0 martin     (501) staff       (20)       85 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_header.txt
--rw-r--r--   0 martin     (501) staff       (20)      212 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_header_expected.txt
--rw-r--r--   0 martin     (501) staff       (20)       64 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_raw.txt
--rw-r--r--   0 martin     (501) staff       (20)       87 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/files/rst_with_pygments.txt
--rw-r--r--   0 martin     (501) staff       (20)      352 2023-04-26 19:13:49.000000 django-markup-1.7/django_markup/tests/files/rst_with_pygments_expected.txt
--rw-r--r--   0 martin     (501) staff       (20)     1213 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/tests/markup_strings.py
--rw-r--r--   0 martin     (501) staff       (20)      756 2022-08-14 08:48:00.000000 django-markup-1.7/django_markup/tests/settings.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.104805 django-markup-1.7/django_markup/tests/templates/
--rw-r--r--   0 martin     (501) staff       (20)       54 2022-08-14 08:39:58.000000 django-markup-1.7/django_markup/tests/templates/test_templatetag.html
--rw-r--r--   0 martin     (501) staff       (20)       81 2023-04-26 19:13:10.000000 django-markup-1.7/django_markup/tests/templates/test_templatetag_filterwrapper.html
--rw-r--r--   0 martin     (501) staff       (20)     2478 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/tests/test_custom_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     4169 2023-04-26 19:14:13.000000 django-markup-1.7/django_markup/tests/test_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     1960 2023-02-26 22:47:46.000000 django-markup-1.7/django_markup/tests/test_templatetag.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.101155 django-markup-1.7/django_markup.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     5564 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1939 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 18:45:56.000000 django-markup-1.7/django_markup.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)      171 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       14 2023-04-26 19:23:31.000000 django-markup-1.7/django_markup.egg-info/top_level.txt
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.106434 django-markup-1.7/docs/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.106951 django-markup-1.7/docs/_static/
--rw-r--r--   0 martin     (501) staff       (20)     6488 2022-08-14 08:39:58.000000 django-markup-1.7/docs/_static/basic.css
--rw-r--r--   0 martin     (501) staff       (20)     3791 2022-08-14 08:39:58.000000 django-markup-1.7/docs/_static/default.css
--rw-r--r--   0 martin     (501) staff       (20)     2717 2022-08-14 08:39:58.000000 django-markup-1.7/docs/_static/pygments.css
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:23:31.108175 django-markup-1.7/docs/bundled_filter/
--rw-r--r--   0 martin     (501) staff       (20)      252 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/creole.rst
--rw-r--r--   0 martin     (501) staff       (20)      300 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/linebreaks.rst
--rw-r--r--   0 martin     (501) staff       (20)      418 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/markdown.rst
--rw-r--r--   0 martin     (501) staff       (20)      126 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/none.rst
--rw-r--r--   0 martin     (501) staff       (20)     2263 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/rst.rst
--rw-r--r--   0 martin     (501) staff       (20)      314 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/smartypants.rst
--rw-r--r--   0 martin     (501) staff       (20)      500 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/textile.rst
--rw-r--r--   0 martin     (501) staff       (20)      208 2022-08-14 08:39:58.000000 django-markup-1.7/docs/bundled_filter/widont.rst
--rw-r--r--   0 martin     (501) staff       (20)     6322 2022-08-14 08:39:58.000000 django-markup-1.7/docs/conf.py
--rw-r--r--   0 martin     (501) staff       (20)      384 2022-08-14 08:39:58.000000 django-markup-1.7/docs/configuration.rst
--rw-r--r--   0 martin     (501) staff       (20)     1211 2022-08-14 08:39:58.000000 django-markup-1.7/docs/filter.rst
--rw-r--r--   0 martin     (501) staff       (20)     1351 2022-08-14 08:39:58.000000 django-markup-1.7/docs/filter_settings.rst
--rw-r--r--   0 martin     (501) staff       (20)     2689 2022-08-14 08:39:58.000000 django-markup-1.7/docs/formatter.rst
--rw-r--r--   0 martin     (501) staff       (20)     1183 2022-08-14 08:39:58.000000 django-markup-1.7/docs/index.rst
--rw-r--r--   0 martin     (501) staff       (20)      773 2022-08-14 08:39:58.000000 django-markup-1.7/docs/installation.rst
--rw-r--r--   0 martin     (501) staff       (20)      759 2022-08-14 08:39:58.000000 django-markup-1.7/docs/usage_models.rst
--rw-r--r--   0 martin     (501) staff       (20)      107 2022-08-14 08:39:58.000000 django-markup-1.7/docs/usage_python.rst
--rw-r--r--   0 martin     (501) staff       (20)     1137 2022-08-14 08:39:58.000000 django-markup-1.7/docs/usage_templates.rst
--rw-r--r--   0 martin     (501) staff       (20)     1691 2023-04-26 19:23:31.108852 django-markup-1.7/setup.cfg
--rwxr-xr-x   0 martin     (501) staff       (20)       59 2023-04-26 19:06:37.000000 django-markup-1.7/setup.py
--rw-r--r--   0 martin     (501) staff       (20)      793 2023-04-26 19:21:41.000000 django-markup-1.7/tox.ini
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.711862 django-markup-1.7.1/
+-rw-r--r--   0 martin     (501) staff       (20)     2776 2023-04-26 19:19:16.000000 django-markup-1.7.1/CHANGELOG.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1534 2022-08-14 08:39:58.000000 django-markup-1.7.1/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)      266 2022-08-14 08:39:58.000000 django-markup-1.7.1/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     5617 2023-04-26 19:28:29.711967 django-markup-1.7.1/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      582 2023-04-26 19:09:41.000000 django-markup-1.7.1/Pipfile
+-rw-r--r--   0 martin     (501) staff       (20)    21963 2023-04-26 19:09:52.000000 django-markup-1.7.1/Pipfile.lock
+-rw-r--r--   0 martin     (501) staff       (20)     1888 2023-04-26 19:18:12.000000 django-markup-1.7.1/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.703019 django-markup-1.7.1/django_markup/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1259 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/defaults.py
+-rw-r--r--   0 martin     (501) staff       (20)     1053 2022-08-14 08:44:22.000000 django-markup-1.7.1/django_markup/fields.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.705373 django-markup-1.7.1/django_markup/filter/
+-rw-r--r--   0 martin     (501) staff       (20)      288 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      235 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/creole_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      475 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/linebreaks_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     1360 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/markdown_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      237 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/none_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      897 2022-08-14 08:44:39.000000 django-markup-1.7.1/django_markup/filter/rst_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      246 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/smartypants_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      226 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/textile_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      206 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/widont_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     3534 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/markup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.705645 django-markup-1.7.1/django_markup/templatetags/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/templatetags/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      255 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/templatetags/markup_tags.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.706674 django-markup-1.7.1/django_markup/tests/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/__init__.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.707537 django-markup-1.7.1/django_markup/tests/files/
+-rw-r--r--   0 martin     (501) staff       (20)       85 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_header.txt
+-rw-r--r--   0 martin     (501) staff       (20)      212 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_header_expected.txt
+-rw-r--r--   0 martin     (501) staff       (20)       64 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_raw.txt
+-rw-r--r--   0 martin     (501) staff       (20)       87 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_with_pygments.txt
+-rw-r--r--   0 martin     (501) staff       (20)      352 2023-04-26 19:13:49.000000 django-markup-1.7.1/django_markup/tests/files/rst_with_pygments_expected.txt
+-rw-r--r--   0 martin     (501) staff       (20)     1213 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/tests/markup_strings.py
+-rw-r--r--   0 martin     (501) staff       (20)      756 2022-08-14 08:48:00.000000 django-markup-1.7.1/django_markup/tests/settings.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.707851 django-markup-1.7.1/django_markup/tests/templates/
+-rw-r--r--   0 martin     (501) staff       (20)       54 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/templates/test_templatetag.html
+-rw-r--r--   0 martin     (501) staff       (20)       81 2023-04-26 19:13:10.000000 django-markup-1.7.1/django_markup/tests/templates/test_templatetag_filterwrapper.html
+-rw-r--r--   0 martin     (501) staff       (20)     2478 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/tests/test_custom_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     4169 2023-04-26 19:14:13.000000 django-markup-1.7.1/django_markup/tests/test_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     1960 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/tests/test_templatetag.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.703979 django-markup-1.7.1/django_markup.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     5617 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1939 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 18:45:56.000000 django-markup-1.7.1/django_markup.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)      171 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       14 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.709463 django-markup-1.7.1/docs/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.710383 django-markup-1.7.1/docs/_static/
+-rw-r--r--   0 martin     (501) staff       (20)     6488 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/_static/basic.css
+-rw-r--r--   0 martin     (501) staff       (20)     3791 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/_static/default.css
+-rw-r--r--   0 martin     (501) staff       (20)     2717 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/_static/pygments.css
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.711710 django-markup-1.7.1/docs/bundled_filter/
+-rw-r--r--   0 martin     (501) staff       (20)      252 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/creole.rst
+-rw-r--r--   0 martin     (501) staff       (20)      300 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/linebreaks.rst
+-rw-r--r--   0 martin     (501) staff       (20)      418 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/markdown.rst
+-rw-r--r--   0 martin     (501) staff       (20)      126 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/none.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2263 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/rst.rst
+-rw-r--r--   0 martin     (501) staff       (20)      314 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/smartypants.rst
+-rw-r--r--   0 martin     (501) staff       (20)      500 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/textile.rst
+-rw-r--r--   0 martin     (501) staff       (20)      208 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/widont.rst
+-rw-r--r--   0 martin     (501) staff       (20)     6322 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/conf.py
+-rw-r--r--   0 martin     (501) staff       (20)      384 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/configuration.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1211 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/filter.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1351 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/filter_settings.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2689 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/formatter.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1183 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/index.rst
+-rw-r--r--   0 martin     (501) staff       (20)      773 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/installation.rst
+-rw-r--r--   0 martin     (501) staff       (20)      759 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/usage_models.rst
+-rw-r--r--   0 martin     (501) staff       (20)      107 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/usage_python.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1137 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/usage_templates.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1733 2023-04-26 19:28:29.712429 django-markup-1.7.1/setup.cfg
+-rwxr-xr-x   0 martin     (501) staff       (20)       59 2023-04-26 19:06:37.000000 django-markup-1.7.1/setup.py
+-rw-r--r--   0 martin     (501) staff       (20)      800 2023-04-26 19:24:59.000000 django-markup-1.7.1/tox.ini
```

### Comparing `django-markup-1.7/CHANGELOG.rst` & `django-markup-1.7.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/LICENSE` & `django-markup-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/PKG-INFO` & `django-markup-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-markup
-Version: 1.7
+Version: 1.7.1
 Summary: A generic Django application to convert text with specific markup to html.
 Home-page: https://github.com/bartTC/django-markup
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
 Keywords: django,markup,markdown,restructuredtext,format,text
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Provides-Extra: all_filter_dependencies
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/django-markup.svg
     :target: https://pypi.org/project/django-markup/
```

### Comparing `django-markup-1.7/Pipfile` & `django-markup-1.7.1/Pipfile`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/Pipfile.lock` & `django-markup-1.7.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/README.rst` & `django-markup-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/defaults.py` & `django-markup-1.7.1/django_markup/defaults.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/fields.py` & `django-markup-1.7.1/django_markup/fields.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/filter/markdown_filter.py` & `django-markup-1.7.1/django_markup/filter/markdown_filter.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/filter/rst_filter.py` & `django-markup-1.7.1/django_markup/filter/rst_filter.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/markup.py` & `django-markup-1.7.1/django_markup/markup.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/tests/markup_strings.py` & `django-markup-1.7.1/django_markup/tests/markup_strings.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/tests/settings.py` & `django-markup-1.7.1/django_markup/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/tests/test_custom_filter.py` & `django-markup-1.7.1/django_markup/tests/test_custom_filter.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/tests/test_filter.py` & `django-markup-1.7.1/django_markup/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup/tests/test_templatetag.py` & `django-markup-1.7.1/django_markup/tests/test_templatetag.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/django_markup.egg-info/PKG-INFO` & `django-markup-1.7.1/django_markup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-markup
-Version: 1.7
+Version: 1.7.1
 Summary: A generic Django application to convert text with specific markup to html.
 Home-page: https://github.com/bartTC/django-markup
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
 Keywords: django,markup,markdown,restructuredtext,format,text
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Provides-Extra: all_filter_dependencies
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/django-markup.svg
     :target: https://pypi.org/project/django-markup/
```

### Comparing `django-markup-1.7/django_markup.egg-info/SOURCES.txt` & `django-markup-1.7.1/django_markup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/_static/basic.css` & `django-markup-1.7.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/_static/default.css` & `django-markup-1.7.1/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/_static/pygments.css` & `django-markup-1.7.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/bundled_filter/rst.rst` & `django-markup-1.7.1/docs/bundled_filter/rst.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/conf.py` & `django-markup-1.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/filter.rst` & `django-markup-1.7.1/docs/filter.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/filter_settings.rst` & `django-markup-1.7.1/docs/filter_settings.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/formatter.rst` & `django-markup-1.7.1/docs/formatter.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/index.rst` & `django-markup-1.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/installation.rst` & `django-markup-1.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/usage_models.rst` & `django-markup-1.7.1/docs/usage_models.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/docs/usage_templates.rst` & `django-markup-1.7.1/docs/usage_templates.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7/setup.cfg` & `django-markup-1.7.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-markup
-version = 1.7
+version = 1.7.1
 description = A generic Django application to convert text with specific markup to html.
 long_description = file: README.rst, CHANGELOG.rst
 author = Martin Mahner
 author_email = martin@mahner.org
 url = https://github.com/bartTC/django-markup
 keywords = django, markup, markdown, restructuredtext, format, text
 license = MIT
@@ -15,22 +15,23 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Framework :: Django
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
-	django>=3.2
+	django>=3.7
 
 [options.extras_require]
 all_filter_dependencies = 
 	textile>=2.3.16
 	smartypants>=2.0.0
 	docutils>=0.14
 	pygments>=2.2.0
```

### Comparing `django-markup-1.7/tox.ini` & `django-markup-1.7.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tox]
 toxworkdir=/tmp/tox/django-markup
 skip_missing_interpreters=True
 envlist=
     readme
-    py{37,38,39,310}-django-{32}
-    py{38,39,310,311}-django-{40,41}
+    py{37,38,39,310,311}-django-{32}
+    py{38,39,310,311}-django-{40,41,42}
 
 [gh-actions]
 python =
     readme: py37
     3.7: py37
     3.8: py38
     3.9: py39
```

