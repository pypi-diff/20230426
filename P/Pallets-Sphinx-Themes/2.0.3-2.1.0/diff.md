# Comparing `tmp/Pallets-Sphinx-Themes-2.0.3.tar.gz` & `tmp/Pallets-Sphinx-Themes-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pallets-Sphinx-Themes-2.0.3.tar", last modified: Sat Dec 24 17:13:29 2022, max compression
+gzip compressed data, was "Pallets-Sphinx-Themes-2.1.0.tar", last modified: Tue Apr 25 17:30:32 2023, max compression
```

## Comparing `Pallets-Sphinx-Themes-2.0.3.tar` & `Pallets-Sphinx-Themes-2.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/
--rw-r--r--   0 david     (1000) david     (1000)     5562 2022-12-24 17:12:26.000000 Pallets-Sphinx-Themes-2.0.3/CHANGES.rst
--rw-r--r--   0 david     (1000) david     (1000)     1475 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/LICENSE.rst
--rw-r--r--   0 david     (1000) david     (1000)      102 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)     1632 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      512 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/README.rst
--rw-r--r--   0 david     (1000) david     (1000)     2023 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      197 2022-12-24 16:25:44.000000 Pallets-Sphinx-Themes-2.0.3/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.119434 Pallets-Sphinx-Themes-2.0.3/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     1632 2022-12-24 17:13:29.000000 Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     1969 2022-12-24 17:13:29.000000 Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-12-24 17:13:29.000000 Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)      126 2022-12-24 17:13:29.000000 Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/entry_points.txt
--rw-r--r--   0 david     (1000) david     (1000)       63 2022-12-24 17:13:29.000000 Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       22 2022-12-24 17:13:29.000000 Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/top_level.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/
--rw-r--r--   0 david     (1000) david     (1000)     5932 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     1265 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/theme_check.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/babel/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/babel/static/
--rw-r--r--   0 david     (1000) david     (1000)      435 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/babel/static/babel.css
--rw-r--r--   0 david     (1000) david     (1000)       47 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/babel/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/
--rw-r--r--   0 david     (1000) david     (1000)      174 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     7842 2022-12-24 16:25:44.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/domain.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/static/
--rw-r--r--   0 david     (1000) david     (1000)      585 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/static/click.css
--rw-r--r--   0 david     (1000) david     (1000)       70 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/flask/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.122768 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/flask/static/
--rw-r--r--   0 david     (1000) david     (1000)      219 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/flask/static/flask.css
--rw-r--r--   0 david     (1000) david     (1000)       47 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/flask/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/
--rw-r--r--   0 david     (1000) david     (1000)     1548 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     8852 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/domain.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/static/
--rw-r--r--   0 david     (1000) david     (1000)      407 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/static/jinja.css
--rw-r--r--   0 david     (1000) david     (1000)       70 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/platter/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/platter/static/
--rw-r--r--   0 david     (1000) david     (1000)      449 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/platter/static/platter.css
--rw-r--r--   0 david     (1000) david     (1000)       49 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/platter/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/
--rw-r--r--   0 david     (1000) david     (1000)      391 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/404.html
--rw-r--r--   0 david     (1000) david     (1000)     4052 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)       38 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/ethicalads.html
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/layout.html
--rw-r--r--   0 david     (1000) david     (1000)       66 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/localtoc.html
--rw-r--r--   0 david     (1000) david     (1000)      173 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/project.html
--rw-r--r--   0 david     (1000) david     (1000)      645 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/relations.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/static/
--rw-r--r--   0 david     (1000) david     (1000)     7934 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css
--rw-r--r--   0 david     (1000) david     (1000)     1582 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js
--rw-r--r--   0 david     (1000) david     (1000)      181 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/theme.conf
--rw-r--r--   0 david     (1000) david     (1000)      253 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/versions.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/werkzeug/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-24 17:13:29.126101 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/werkzeug/static/
--rw-r--r--   0 david     (1000) david     (1000)      219 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/werkzeug/static/werkzeug.css
--rw-r--r--   0 david     (1000) david     (1000)       50 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/werkzeug/theme.conf
--rw-r--r--   0 david     (1000) david     (1000)     4580 2022-12-23 23:44:01.000000 Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/versions.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/
+-rw-r--r--   0 david     (1000) david     (1000)     5761 2023-04-25 17:28:30.000000 Pallets-Sphinx-Themes-2.1.0/CHANGES.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1475 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/LICENSE.rst
+-rw-r--r--   0 david     (1000) david     (1000)      102 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)     1578 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      512 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/README.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1980 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      145 2023-04-25 17:21:40.000000 Pallets-Sphinx-Themes-2.1.0/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     1578 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     1969 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)      126 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1000) david     (1000)       20 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       22 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/
+-rw-r--r--   0 david     (1000) david     (1000)     5359 2023-04-25 17:23:09.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     1265 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/theme_check.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/static/
+-rw-r--r--   0 david     (1000) david     (1000)      453 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/static/babel.css
+-rw-r--r--   0 david     (1000) david     (1000)       47 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/theme.conf
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/
+-rw-r--r--   0 david     (1000) david     (1000)      174 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     7785 2023-04-25 17:19:12.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/domain.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/static/
+-rw-r--r--   0 david     (1000) david     (1000)      585 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/static/click.css
+-rw-r--r--   0 david     (1000) david     (1000)       70 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/theme.conf
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/static/
+-rw-r--r--   0 david     (1000) david     (1000)      237 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/static/flask.css
+-rw-r--r--   0 david     (1000) david     (1000)       47 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/theme.conf
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/
+-rw-r--r--   0 david     (1000) david     (1000)     1548 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     8756 2023-04-25 17:21:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/domain.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/static/
+-rw-r--r--   0 david     (1000) david     (1000)      425 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/static/jinja.css
+-rw-r--r--   0 david     (1000) david     (1000)       70 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/theme.conf
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/static/
+-rw-r--r--   0 david     (1000) david     (1000)      449 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/static/platter.css
+-rw-r--r--   0 david     (1000) david     (1000)       49 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/theme.conf
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/
+-rw-r--r--   0 david     (1000) david     (1000)      391 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/404.html
+-rw-r--r--   0 david     (1000) david     (1000)     4052 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)       38 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/ethicalads.html
+-rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/layout.html
+-rw-r--r--   0 david     (1000) david     (1000)       66 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/localtoc.html
+-rw-r--r--   0 david     (1000) david     (1000)      173 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/project.html
+-rw-r--r--   0 david     (1000) david     (1000)      645 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/relations.html
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/
+-rw-r--r--   0 david     (1000) david     (1000)     8153 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css
+-rw-r--r--   0 david     (1000) david     (1000)     1582 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js
+-rw-r--r--   0 david     (1000) david     (1000)      181 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/theme.conf
+-rw-r--r--   0 david     (1000) david     (1000)      253 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/versions.html
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/static/
+-rw-r--r--   0 david     (1000) david     (1000)      237 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/static/werkzeug.css
+-rw-r--r--   0 david     (1000) david     (1000)       50 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/theme.conf
+-rw-r--r--   0 david     (1000) david     (1000)     4580 2022-12-23 23:44:01.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/versions.py
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/CHANGES.rst` & `Pallets-Sphinx-Themes-2.1.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Version 2.1.0
+-------------
+
+Released 2023-04-25
+
+-   Drop support for Python 3.6 and 3.7.
+-   Require Sphinx >= 3.
+-   Remove previously deprecated code.
+-   Fix table of contents overflow issue.
+
+
 Version 2.0.3
 -------------
 
 Released 2022-12-24
 
 -   Fix compatibility with ``packaging>=22``.
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/LICENSE.rst` & `Pallets-Sphinx-Themes-2.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/PKG-INFO` & `Pallets-Sphinx-Themes-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: Pallets-Sphinx-Themes
-Version: 2.0.3
+Version: 2.1.0
 Summary: Sphinx themes for Pallets and related projects.
 Home-page: https://github.com/pallets/pallets-sphinx-themes/
 Author: Pallets
 Author-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Source Code, https://github.com/pallets/pallets-sphinx-themes/
 Project-URL: Issue Tracker, https://github.com/pallets/pallets-sphinx-themes/issues/
-Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 Pallets Sphinx Themes
 =====================
 
 Themes for the Pallets projects. If you're writing an extension, use the
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/README.rst` & `Pallets-Sphinx-Themes-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/setup.cfg` & `Pallets-Sphinx-Themes-2.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [metadata]
 name = Pallets-Sphinx-Themes
-version = 2.0.3
+version = 2.1.0
 url = https://github.com/pallets/pallets-sphinx-themes/
 project_urls = 
 	Donate = https://palletsprojects.com/donate
 	Source Code = https://github.com/pallets/pallets-sphinx-themes/
 	Issue Tracker = https://github.com/pallets/pallets-sphinx-themes/issues/
-	Twitter = https://twitter.com/PalletsTeam
 	Chat = https://discord.gg/pallets
 license = BSD-3-Clause
 license_files = LICENSE.rst
 author = Pallets
 author_email = contact@palletsprojects.com
 description = Sphinx themes for Pallets and related projects.
 long_description = file: README.rst
@@ -27,15 +26,15 @@
 	Topic :: Documentation :: Sphinx
 	Topic :: Software Development :: Documentation
 
 [options]
 packages = find:
 package_dir = = src
 include_package_data = True
-python_requires = >= 3.6
+python_requires = >= 3.8
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 pygments.styles = 
 	pocoo = pallets_sphinx_themes.themes.pocoo:PocooStyle
@@ -64,15 +63,15 @@
 	E501
 	E722
 	W503
 max-line-length = 80
 
 [mypy]
 files = src/pallets_sphinx_themes
-python_version = 3.6
+python_version = 3.7
 disallow_subclassing_any = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 no_implicit_optional = True
 local_partial_types = True
 no_implicit_reexport = True
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO` & `Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: Pallets-Sphinx-Themes
-Version: 2.0.3
+Version: 2.1.0
 Summary: Sphinx themes for Pallets and related projects.
 Home-page: https://github.com/pallets/pallets-sphinx-themes/
 Author: Pallets
 Author-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Source Code, https://github.com/pallets/pallets-sphinx-themes/
 Project-URL: Issue Tracker, https://github.com/pallets/pallets-sphinx-themes/issues/
-Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 Pallets Sphinx Themes
 =====================
 
 Themes for the Pallets projects. If you're writing an extension, use the
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt` & `Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/__init__.py` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import inspect
 import os
 import re
 import sys
 import textwrap
 from collections import namedtuple
+from importlib import metadata as importlib_metadata
 
 from sphinx.application import Sphinx
 from sphinx.builders._epub_base import EpubBuilder
 from sphinx.builders.dirhtml import DirectoryHTMLBuilder
 from sphinx.builders.singlehtml import SingleFileHTMLBuilder
 from sphinx.errors import ExtensionError
 
 from .theme_check import only_pallets_theme
 from .theme_check import set_is_pallets_theme
 from .versions import load_versions
 
-try:
-    from importlib import metadata as importlib_metadata
-except ImportError:
-    # Python <3.8 compatibility
-    import importlib_metadata
-
 
 def setup(app):
     base = os.path.join(os.path.dirname(__file__), "themes")
 
     for name in os.listdir(base):
         path = os.path.join(base, name)
 
@@ -75,31 +70,17 @@
 
 @only_pallets_theme()
 def canonical_url(app: Sphinx, pagename, templatename, context, doctree):
     """Sphinx 1.8 builds a canonical URL if ``html_baseurl`` config is
     set. However, it builds a URL ending with ".html" when using the
     dirhtml builder, which is incorrect. Detect this and generate the
     correct URL for each page.
-
-    Also accepts the custom, deprecated ``canonical_url`` config as the
-    base URL. This will be removed in version 2.1.
     """
     base = app.config.html_baseurl
 
-    if not base and context.get("canonical_url"):
-        import warnings
-
-        warnings.warn(
-            "'canonical_url' config is deprecated and will be removed"
-            " in Pallets-Sphinx-Themes 2.1. Set Sphinx's 'html_baseurl'"
-            " config instead.",
-            DeprecationWarning,
-        )
-        base = context["canonical_url"]
-
     if (
         not base
         or not isinstance(app.builder, DirectoryHTMLBuilder)
         or not context["pageurl"]
         or not context["pageurl"].endswith(".html")
     ):
         return
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/theme_check.py` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/theme_check.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/domain.py` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,20 @@
         yield
     finally:
         subprocess.call = old_call
 
 
 class ExampleRunner(CliRunner):
     def __init__(self):
-        super(ExampleRunner, self).__init__(echo_stdin=True)
+        super().__init__(echo_stdin=True)
         self.namespace = {"click": click, "__file__": "dummy.py", "str": text_type}
 
     @contextlib.contextmanager
     def isolation(self, *args, **kwargs):
-        iso = super(ExampleRunner, self).isolation(*args, **kwargs)
+        iso = super().isolation(*args, **kwargs)
 
         with iso as streams:
             try:
                 buffer = sys.stdin.buffer
             except AttributeError:
                 buffer = sys.stdin
 
@@ -91,15 +91,15 @@
         cli,
         args=None,
         prog_name=None,
         input=None,
         terminate_input=False,
         env=None,
         _output_lines=None,
-        **extra
+        **extra,
     ):
         """Like :meth:`CliRunner.invoke` but displays what the user
         would enter in the terminal for env vars, command args, and
         prompts.
 
         :param terminate_input: Whether to display "^D" after a list of
             input.
@@ -107,15 +107,15 @@
             be displayed.
         """
         output_lines = _output_lines if _output_lines is not None else []
 
         if env:
             for key, value in sorted(env.items()):
                 value = shlex.quote(value)
-                output_lines.append("$ export {}={}".format(key, value))
+                output_lines.append(f"$ export {key}={value}")
 
         args = args or []
 
         if prog_name is None:
             prog_name = cli.name.replace("_", "-")
 
         output_lines.append(
@@ -126,15 +126,15 @@
 
         if isinstance(input, (tuple, list)):
             input = "\n".join(input) + "\n"
 
             if terminate_input:
                 input += "\x04"
 
-        result = super(ExampleRunner, self).invoke(
+        result = super().invoke(
             cli=cli, args=args, input=input, env=env, prog_name=prog_name, **extra
         )
         output_lines.extend(result.output.splitlines())
         return result
 
     def declare_example(self, source):
         """Execute the given code, adding it to the runner's namespace."""
@@ -238,15 +238,15 @@
 
         try:
             rv = runner.run_example("\n".join(self.content))
         except BaseException:
             runner.close()
             raise
 
-        doc.append(".. sourcecode:: text", "")
+        doc.append(".. sourcecode:: shell-session", "")
         doc.append("", "")
 
         for line in rv:
             doc.append(" " + line, "")
 
         node = nodes.section()
         self.state.nested_parse(doc, self.content_offset, node)
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/click/static/click.css` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/static/click.css`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/__init__.py` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/__init__.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/jinja/domain.py` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 
             if params[0].kind != inspect.Parameter.VAR_POSITIONAL:
                 # only remove it if it's not "*args"
                 del params[0]
 
             sig = sig.replace(parameters=params)
 
-    result = ["", ".. function:: {}{}".format(name, sig), ""]
-    result.extend(["    {}".format(x) for x in doc])
+    result = ["", f".. function:: {name}{sig}", ""]
+    result.extend([f"    {x}" for x in doc])
 
     if aliases:
         result.append("")
-        alias_str = ", ".join(["``{}``".format(x) for x in sorted(aliases)])
-        result.append("    :aliases: {}".format(alias_str))
+        alias_str = ", ".join([f"``{x}``" for x in sorted(aliases)])
+        result.append(f"    :aliases: {alias_str}")
 
     return result
 
 
 class MappedFunctionsDirective(SphinxDirective):
     """Take a dict of names to functions and produce rendered docs.
     Requires one argument, the import name of the dict to process.
@@ -144,29 +144,29 @@
 
         The table is hard coded to be 5 columns wide. Names are rendered
         in alphabetical order in columns.
 
         :return: A list of rendered nodes.
         """
         # the reference markup to link to each name
-        names = [":func:`{}`".format(name) for name, _, _ in self.funcs]
+        names = [f":func:`{name}`" for name, _, _ in self.funcs]
         # total number of rows, the number of names divided by the
         # number of columns, plus one in case of overflow
         row_size = (len(names) // 5) + bool(len(names) % 5)
         # pivot to rows so that names remain alphabetical in columns
         rows = [names[i::row_size] for i in range(row_size)]
 
         # render the names to CSV for the csv-table directive
         out = StringIO()
         writer = csv.writer(out)
         writer.writerows(rows)
 
         # generate the markup for the csv-table directive
         result = ["", ".. csv-table::", "    :align: left", ""]
-        result.extend(["    {}".format(line) for line in out.getvalue().splitlines()])
+        result.extend([f"    {line}" for line in out.getvalue().splitlines()])
 
         # parse the generated markup into nodes
         result = StringList(result, "<jinja>")
         node = nodes.Element()
         self.state.nested_parse(result, self.content_offset, node)
         return node.children
 
@@ -223,17 +223,15 @@
                 if members:
                     members.sort()
                     lines.append("    :members: " + ", ".join(members))
 
             # reference the parent node, except for the base node
             if cls.__base__ is not object:
                 lines.append("")
-                lines.append(
-                    "    :Node type: :class:`{}`".format(cls.__base__.__name__)
-                )
+                lines.append(f"    :Node type: :class:`{cls.__base__.__name__}`")
 
             lines.append("")
             children = cls.__subclasses__()
             children.sort(key=lambda x: x.__name__.lower())
 
             # render each child
             for child in children:
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/__init__.py` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/__init__.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/layout.html` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/layout.html`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/relations.html` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/relations.html`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,33 @@
 div.sphinxsidebar {
   width: 220px;
   font-size: 14px;
   line-height: 1.5;
   color: #444;
 }
 
+div.sphinxsidebar li {
+  overflow: hidden;
+  text-overflow: ellipsis;
+}
+
+div.sphinxsidebar li:hover {
+  overflow: visible;
+}
+
 div.sphinxsidebar a,
 div.sphinxsidebar a code {
   color: #444;
   border-color: #444;
 }
 
+div.sphinxsidebar a:hover {
+  background-color:#fff;
+}
+
 div.sphinxsidebar p.logo {
   margin: 0;
   text-align: center;
 }
 
 div.sphinxsidebar h3,
 div.sphinxsidebar h4 {
@@ -163,20 +176,21 @@
   color: #fff;
   border-color: #fff;
 }
 
 /* -- body styles --------------------------------------------------- */
 
 a {
-  text-decoration: none;
-  border-bottom: 1px dotted #000;
+  text-decoration: underline;
+  text-decoration-style: dotted;
+  text-decoration-color: #000;
 }
 
 a:hover {
-  border-bottom-style: solid;
+  text-decoration-style: solid;
 }
 
 h1, h2, h3, h4, h5, h6 {
   font-weight: normal;
   margin: 30px 0 10px;
   padding: 0;
   color: black;
```

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.0.3/src/pallets_sphinx_themes/versions.py` & `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/versions.py`

 * *Files identical despite different names*

