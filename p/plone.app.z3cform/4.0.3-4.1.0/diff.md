# Comparing `tmp/plone.app.z3cform-4.0.3.tar.gz` & `tmp/plone.app.z3cform-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.z3cform-4.0.3.tar", last modified: Thu Apr 13 22:51:53 2023, max compression
+gzip compressed data, was "plone.app.z3cform-4.1.0.tar", last modified: Wed Apr 26 21:55:46 2023, max compression
```

## Comparing `plone.app.z3cform-4.0.3.tar` & `plone.app.z3cform-4.1.0.tar`

### file list

```diff
@@ -1,90 +1,103 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.870687 plone.app.z3cform-4.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)    24821 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    48074 2023-04-13 22:51:53.870810 plone.app.z3cform-4.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.848336 plone.app.z3cform-4.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      749 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.848564 plone.app.z3cform-4.0.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.851131 plone.app.z3cform-4.0.3/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.856082 plone.app.z3cform-4.0.3/plone/app/z3cform/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4254 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      431 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2500 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      212 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)      152 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.845032 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.856946 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      163 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      635 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.865826 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/ajaxselect_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/checkbox_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      140 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/contentprovider-widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)      209 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/error.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/file_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/image_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      677 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3547 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/link_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9551 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/multi_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/object_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5486 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/orderedselect_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/password_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      650 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input_single.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/relateditems_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/select_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      976 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      765 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/submit_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/text_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textarea_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textfield_widget_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textlines_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/widget.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.868712 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)      907 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)     4554 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widget.py
--rw-r--r--   0 maurits    (501) staff       (20)    66068 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     3393 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/views.py
--rw-r--r--   0 maurits    (501) staff       (20)    33302 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/widget.py
--rw-r--r--   0 maurits    (501) staff       (20)     8895 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/widget.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.870334 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/
--rw-r--r--   0 maurits    (501) staff       (20)      919 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      639 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/widget.py
--rw-r--r--   0 maurits    (501) staff       (20)      601 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.850904 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    48074 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2876 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      735 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      242 2023-04-13 22:51:53.871275 plone.app.z3cform-4.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2881 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.671824 plone.app.z3cform-4.1.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    24989 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    48242 2023-04-26 21:55:46.671959 plone.app.z3cform-4.1.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.648920 plone.app.z3cform-4.1.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.649168 plone.app.z3cform-4.1.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.651481 plone.app.z3cform-4.1.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.656343 plone.app.z3cform-4.1.0/plone/app/z3cform/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2935 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1310 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/converters.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      431 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2500 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      212 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.645957 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.657138 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      635 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.664494 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/ajaxselect_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/checkbox_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/contentprovider-widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/error.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/file_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/image_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3547 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/link_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9551 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/multi_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/object_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5486 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/orderedselect_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/password_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      650 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input_single.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/relateditems_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/select_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      765 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/submit_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/text_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textarea_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textfield_widget_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textlines_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/widget.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.667203 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17512 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4554 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)    66963 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5619 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2959 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.669884 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1807 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4970 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/datetime.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9625 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2712 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/querystring.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8804 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/relateditems.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6381 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11155 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/select.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2962 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/singlecheckbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9303 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.671621 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/
+-rw-r--r--   0 maurits    (501) staff       (20)      919 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      639 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)      601 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.651230 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    48242 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3335 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      242 2023-04-26 21:55:46.672532 plone.app.z3cform-4.1.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2625 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/setup.py
```

### Comparing `plone.app.z3cform-4.0.3/CHANGES.rst` & `plone.app.z3cform-4.1.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2023-04-26)
+------------------
+
+New features:
+
+
+- Merge utils and base classes from  ``plone.app.widgets`` and do not depend
+  on it anymore. [petschki] (#19)
+
+
 4.0.3 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fixes transitive circular dependency to plone.schema.
```

### Comparing `plone.app.z3cform-4.0.3/PKG-INFO` & `plone.app.z3cform-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.0.3
+Version: 4.1.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -677,14 +677,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2023-04-26)
+------------------
+
+New features:
+
+
+- Merge utils and base classes from  ``plone.app.widgets`` and do not depend
+  on it anymore. [petschki] (#19)
+
+
 4.0.3 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fixes transitive circular dependency to plone.schema.
```

### Comparing `plone.app.z3cform-4.0.3/README.rst` & `plone.app.z3cform-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/docs/LICENSE.GPL` & `plone.app.z3cform-4.1.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/docs/LICENSE.txt` & `plone.app.z3cform-4.1.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/converters.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/csrf.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.rst` & `plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/interfaces.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/profiles.zcml` & `plone.app.z3cform-4.1.0/plone/app/z3cform/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/ajaxselect_display.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/ajaxselect_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/checkbox_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/file_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/file_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/form.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/image_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/image_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/layout.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/link_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/link_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/macros.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/multi_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/multi_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/object_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/object_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/orderedselect_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/orderedselect_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/password_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/password_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input_single.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input_single.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/relateditems_display.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/relateditems_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/select_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/select_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckbox.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_display.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/submit_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/submit_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/text_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/text_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textarea_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textarea_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textfield_widget_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textfield_widget_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textlines_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textlines_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/widget.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/widget.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/example.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/example.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/layer.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/layer.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_csrf.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_utils.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widget.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widgets.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from datetime import datetime
 from datetime import time
 from json import loads
 from lxml import html
 from plone.app.contentlisting.contentlisting import ContentListing
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
-from plone.app.widgets.utils import NotImplemented as PatternNotImplemented
 from plone.app.z3cform.tests.layer import PAZ3CForm_INTEGRATION_TESTING
-from plone.app.z3cform.widget import BaseWidget
-from plone.app.z3cform.widget import DateWidget
-from plone.app.z3cform.widget import RelatedItemsWidget
+from plone.app.z3cform.widgets.base import BaseWidget
+from plone.app.z3cform.widgets.base import PatternNotImplemented
+from plone.app.z3cform.widgets.datetime import DateWidget
+from plone.app.z3cform.widgets.relateditems import RelatedItemsWidget
 from plone.autoform.directives import widget
 from plone.autoform.form import AutoExtensibleForm
 from plone.base.interfaces import IMarkupSchema
 from plone.dexterity.fti import DexterityFTI
 from plone.registry.interfaces import IRegistry
 from plone.supermodel.model import Schema
 from plone.testing.zca import UNIT_TESTING
@@ -98,16 +98,16 @@
                 "pattern": "example",
                 "pattern_options": {},
             },
             widget._base_args(),
         )
 
     def test_widget_base_notimplemented(self):
-        from plone.app.widgets.base import InputWidget
-        from plone.app.z3cform.widget import BaseWidget
+        from plone.app.z3cform.widgets.base import BaseWidget
+        from plone.app.z3cform.widgets.patterns import InputWidget
 
         widget = BaseWidget(self.request)
         widget.field = self.field
         widget.pattern = "example"
 
         self.assertRaises(
             PatternNotImplemented,
@@ -118,31 +118,31 @@
 
         self.assertEqual(
             '<input class="pat-example" type="text"/>',
             widget.render(),
         )
 
     def test_widget_base_custom_css(self):
-        from plone.app.widgets.base import InputWidget
-        from plone.app.z3cform.widget import BaseWidget
+        from plone.app.z3cform.widgets.base import BaseWidget
+        from plone.app.z3cform.widgets.patterns import InputWidget
 
         widget = BaseWidget(self.request)
         widget.field = self.field
         widget.pattern = "example"
         widget.klass = "very-custom-class"
         widget._base = InputWidget
 
         self.assertEqual(
             '<input class="pat-example very-custom-class" type="text"/>',
             widget.render(),
         )
 
     def test_widget_base_pattern_options_with_functions(self):
-        from plone.app.widgets.base import InputWidget
-        from plone.app.z3cform.widget import BaseWidget
+        from plone.app.z3cform.widgets.base import BaseWidget
+        from plone.app.z3cform.widgets.patterns import InputWidget
 
         widget = BaseWidget(self.request)
         widget.context = "testcontext"
         widget.field = self.field
         widget.pattern = "example"
         widget._base = InputWidget
         widget.pattern_options = {
@@ -179,15 +179,15 @@
                 },
             },
         )
 
 
 class DateWidgetTests(unittest.TestCase):
     def setUp(self):
-        from plone.app.z3cform.widget import DateWidget
+        from plone.app.z3cform.widgets.datetime import DateWidget
 
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
         self.field = Date(__name__="datefield")
         self.field.required = False
         self.widget = DateWidget(self.request)
         self.widget.field = self.field
         self.widget.pattern_options = {"date": {"firstDay": 0}}
@@ -213,15 +213,15 @@
     def test_widget_required(self):
         """Required fields should not have a "Clear" button."""
         self.field.required = True
         base_args = self.widget._base_args()
         self.assertEqual(base_args["pattern_options"]["clear"], False)
 
     def test_data_converter(self):
-        from plone.app.z3cform.widget import DateWidgetConverter
+        from plone.app.z3cform.widgets.datetime import DateWidgetConverter
 
         converter = DateWidgetConverter(self.field, self.widget)
 
         self.assertEqual(
             converter.field.missing_value,
             converter.toFieldValue(""),
         )
@@ -248,16 +248,16 @@
 
         self.assertEqual(
             "21-10-30",
             converter.toWidgetValue(date(21, 10, 30)),
         )
 
     def test_fieldwidget(self):
-        from plone.app.z3cform.widget import DateFieldWidget
-        from plone.app.z3cform.widget import DateWidget
+        from plone.app.z3cform.widgets.datetime import DateFieldWidget
+        from plone.app.z3cform.widgets.datetime import DateWidget
 
         field = Mock(__name__="field", title="", required=True)
         request = Mock()
         widget = DateFieldWidget(field, request)
         self.assertTrue(isinstance(widget, DateWidget))
         self.assertIs(widget.field, field)
         self.assertIs(widget.request, request)
@@ -282,15 +282,15 @@
         self.widget._formater_length = "foo"
         with self.assertRaises(ValueError):
             self.widget.render()
 
 
 class DatetimeWidgetTests(unittest.TestCase):
     def setUp(self):
-        from plone.app.z3cform.widget import DatetimeWidget
+        from plone.app.z3cform.widgets.datetime import DatetimeWidget
 
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
         self.field = Datetime(__name__="datetimefield")
         self.field.required = False
         self.widget = DatetimeWidget(self.request)
         self.widget.field = self.field
         self.widget.pattern_options = {
@@ -320,15 +320,15 @@
     def test_widget_required(self):
         """Required fields should not have a "Clear" button."""
         self.field.required = True
         base_args = self.widget._base_args()
         self.assertEqual(base_args["pattern_options"]["clear"], False)
 
     def test_data_converter(self):
-        from plone.app.z3cform.widget import DatetimeWidgetConverter
+        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
 
         converter = DatetimeWidgetConverter(self.field, self.widget)
 
         self.assertEqual(
             converter.toFieldValue(""),
             converter.field.missing_value,
         )
@@ -356,15 +356,15 @@
         self.assertEqual(
             converter.toWidgetValue(datetime(21, 10, 30, 15, 40)),
             "21-10-30T15:40",
         )
 
     def test_data_converter__no_timezone(self):
         """When no timezone is set, don't apply one."""
-        from plone.app.z3cform.widget import DatetimeWidgetConverter
+        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
 
         context = Mock()
 
         dt = datetime(2013, 11, 13, 10, 20)
         setattr(context, self.field.getName(), dt)
         self.widget.context = context
         self.widget.default_timezone = None
@@ -377,15 +377,15 @@
 
         # cleanup
         self.widget.context = None
         self.widget.default_timezone = None
 
     def test_data_converter__timezone_id(self):
         """When a (pytz) timezone id is set, use that."""
-        from plone.app.z3cform.widget import DatetimeWidgetConverter
+        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
 
         context = Mock()
 
         dt = datetime(2013, 11, 13, 10, 20)
         setattr(context, self.field.getName(), dt)
         self.widget.context = context
         self.widget.default_timezone = "Europe/Amsterdam"
@@ -401,15 +401,15 @@
         self.widget.context = None
         self.widget.default_timezone = None
 
     def test_data_converter__timezone_callback(self):
         """When a timezone callback is set, returning a (pytz) timezone id,
         use that.
         """
-        from plone.app.z3cform.widget import DatetimeWidgetConverter
+        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
 
         context = Mock()
 
         dt = datetime(2013, 11, 13, 10, 20)
         setattr(context, self.field.getName(), dt)
         self.widget.context = context
         self.widget.default_timezone = lambda context: "Europe/Amsterdam"
@@ -422,16 +422,16 @@
         )
 
         # cleanup
         self.widget.context = None
         self.widget.default_timezone = None
 
     def test_fieldwidget(self):
-        from plone.app.z3cform.widget import DatetimeFieldWidget
-        from plone.app.z3cform.widget import DatetimeWidget
+        from plone.app.z3cform.widgets.datetime import DatetimeFieldWidget
+        from plone.app.z3cform.widgets.datetime import DatetimeWidget
 
         field = Mock(__name__="field", title="", required=True)
         request = Mock()
         widget = DatetimeFieldWidget(field, request)
         self.assertTrue(isinstance(widget, DatetimeWidget))
         self.assertIs(widget.field, field)
         self.assertIs(widget.request, request)
@@ -458,15 +458,15 @@
         self.widget._formater_length = "foo"
         with self.assertRaises(ValueError):
             self.widget.render()
 
 
 class TimeWidgetTests(unittest.TestCase):
     def setUp(self):
-        from plone.app.z3cform.widget import TimeWidget
+        from plone.app.z3cform.widgets.datetime import TimeWidget
 
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
         self.field = Time(__name__="timefield")
         self.field.required = False
         self.widget = TimeWidget(self.request)
         self.widget.field = self.field
 
@@ -495,16 +495,16 @@
 
         self.assertEqual(
             converter.toWidgetValue(time(15, 40)),
             "15:40",
         )
 
     def test_fieldwidget(self):
-        from plone.app.z3cform.widget import TimeFieldWidget
-        from plone.app.z3cform.widget import TimeWidget
+        from plone.app.z3cform.widgets.datetime import TimeFieldWidget
+        from plone.app.z3cform.widgets.datetime import TimeWidget
 
         field = Mock(__name__="field", title="", required=True)
         request = Mock()
         widget = TimeFieldWidget(field, request)
         self.assertTrue(isinstance(widget, TimeWidget))
         self.assertIs(widget.field, field)
         self.assertIs(widget.request, request)
@@ -528,15 +528,15 @@
         from z3c.form import term
 
         base.unregisterAdapter(term.CollectionTerms)
         base.unregisterAdapter(term.CollectionTermsVocabulary)
         base.unregisterAdapter(term.CollectionTermsSource)
 
     def test_widget(self):
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         widget = SelectWidget(self.request)
         widget.id = "test-widget"
         widget.field = Choice(
             __name__="selectfield",
             values=["one", "two", "three"],
         )
@@ -626,15 +626,15 @@
                     ("three", "three"),
                 ],
             },
             widget._base_args(),
         )
 
     def test_widget_list_orderable(self):
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         widget = SelectWidget(self.request)
         widget.id = "test-widget"
         widget.separator = "."
         widget.field = List(
             __name__="selectfield",
             value_type=Choice(values=["one", "two", "three"]),
@@ -653,15 +653,15 @@
                     ("three", "three"),
                 ],
             },
             widget._base_args(),
         )
 
     def test_widget_tuple_orderable(self):
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         widget = SelectWidget(self.request)
         widget.id = "test-widget"
         widget.field = Tuple(
             __name__="selectfield",
             value_type=Choice(values=["one", "two", "three"]),
         )
@@ -679,15 +679,15 @@
                     ("three", "three"),
                 ],
             },
             widget._base_args(),
         )
 
     def test_widget_set_not_orderable(self):
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         widget = SelectWidget(self.request)
         widget.id = "test-widget"
         # A set is not orderable
         widget.field = Set(
             __name__="selectfield",
             value_type=Choice(values=["one", "two", "three"]),
@@ -706,15 +706,15 @@
                     ("three", "three"),
                 ],
             },
             widget._base_args(),
         )
 
     def test_widget_extract(self):
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         widget = SelectWidget(self.request)
         widget.field = Choice(
             __name__="selectfield",
             values=["one", "two", "three"],
         )
         widget.name = "selectfield"
@@ -722,15 +722,15 @@
         self.assertEqual(widget.extract(), "one")
         widget.multiple = True
         self.request.form["selectfield"] = "one;two"
         self.assertEqual(widget.extract(), "one;two")
 
     def test_data_converter_list(self):
         from plone.app.z3cform.converters import SelectWidgetConverter
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         field = List(
             __name__="listfield",
             value_type=Choice(
                 __name__="selectfield",
                 values=["one", "two", "three"],
             ),
@@ -769,15 +769,15 @@
         self.assertEqual(
             converter.toWidgetValue(["one", "two", "three"]),
             ["one", "two", "three"],
         )
 
     def test_data_converter_tuple(self):
         from plone.app.z3cform.converters import SelectWidgetConverter
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         field = Tuple(
             __name__="tuplefield",
             value_type=Choice(
                 __name__="selectfield",
                 values=["one", "two", "three"],
             ),
@@ -805,15 +805,15 @@
         self.assertEqual(
             converter.toWidgetValue(("one", "two", "three")),
             ["one", "two", "three"],
         )
 
     def test_data_converter_handles_empty_value(self):
         from plone.app.z3cform.converters import SelectWidgetConverter
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
 
         field = Tuple(
             __name__="tuplefield",
             value_type=Choice(__name__="selectfield", values=["one", "two", "three"]),
         )
         widget = SelectWidget(self.request)
         widget.field = field
@@ -825,15 +825,15 @@
             field.missing_value,
         )
 
     def test_widget_optgroup(self):
         """
         If the widget vocabulary is a mapping <optgroup>'s are rendered.
         """
-        from plone.app.z3cform.widget import SelectWidget
+        from plone.app.z3cform.widgets.select import SelectWidget
         from z3c.form import term
 
         widget = SelectWidget(self.request)
         widget.field = Choice(
             vocabulary=vocabulary.TreeVocabulary.fromDict(
                 {
                     ("foo_group", "Foo Group"): {
@@ -881,15 +881,15 @@
     maxDiff = None
 
     def setUp(self):
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
         provideUtility(example_vocabulary_factory, name="example")
 
     def test_widget(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         widget = AjaxSelectWidget(self.request)
         widget.update()
         self.assertEqual(
             {
                 "name": None,
                 "value": "",
@@ -928,45 +928,45 @@
                     "separator": ";",
                 },
             },
             widget._base_args(),
         )
 
     def test_widget_list_orderable(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         widget = AjaxSelectWidget(self.request)
         widget.field = List(__name__="selectfield")
         self.assertEqual(
             {
                 "name": None,
                 "value": "",
                 "pattern": "select2",
                 "pattern_options": {"orderable": True, "separator": ";"},
             },
             widget._base_args(),
         )
 
     def test_widget_tuple_orderable(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         widget = AjaxSelectWidget(self.request)
         widget.field = Tuple(__name__="selectfield")
         self.assertEqual(
             {
                 "name": None,
                 "value": "",
                 "pattern": "select2",
                 "pattern_options": {"orderable": True, "separator": ";"},
             },
             widget._base_args(),
         )
 
     def test_widget_set_not_orderable(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         widget = AjaxSelectWidget(self.request)
         # A set is not orderable
         widget.field = Set(__name__="selectfield")
         self.assertEqual(
             {
                 "name": None,
@@ -974,15 +974,15 @@
                 "pattern": "select2",
                 "pattern_options": {"separator": ";"},
             },
             widget._base_args(),
         )
 
     def test_widget_choice(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
         from zope.schema.interfaces import ISource
 
         widget = AjaxSelectWidget(self.request)
         source = Mock()
         alsoProvides(source, ISource)
         widget.field = Choice(__name__="choicefield", source=source)
         widget.name = "choicefield"
@@ -998,15 +998,15 @@
                     "vocabularyUrl": "http://127.0.0.1/++widget++choicefield/@@getSource",
                 },
             },
             widget._base_args(),
         )
 
     def test_widget_addform_url_on_addform(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         widget = AjaxSelectWidget(self.request)
         form = Mock(parentForm=None)
         from z3c.form.interfaces import IAddForm
         from zope.interface import directlyProvides  # noqa
 
         directlyProvides(form, IAddForm)  # noqa
@@ -1033,15 +1033,15 @@
                 },
             },
             widget._base_args(),
         )
 
     def test_data_converter_list(self):
         from plone.app.z3cform.converters import AjaxSelectWidgetConverter
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         field = List(__name__="listfield", value_type=TextLine())
         widget = AjaxSelectWidget(self.request)
         widget.field = field
         converter = AjaxSelectWidgetConverter(field, widget)
 
         self.assertEqual(
@@ -1062,15 +1062,15 @@
         self.assertEqual(
             converter.toWidgetValue(["123", "456", "789"]),
             "123;456;789",
         )
 
     def test_data_converter_collection_with_vocabulary(self):
         from plone.app.z3cform.converters import AjaxSelectWidgetConverter
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         field = Tuple(
             __name__="listfield",
             value_type=Choice(
                 vocabulary="example",
             ),
         )
@@ -1096,15 +1096,15 @@
         self.assertEqual(
             converter.toWidgetValue(["123", "456", "789"]),
             "123;456;789",
         )
 
     def test_data_converter_tuple(self):
         from plone.app.z3cform.converters import AjaxSelectWidgetConverter
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         field = Tuple(__name__="tuplefield", value_type=TextLine())
         widget = AjaxSelectWidget(self.request)
         widget.field = field
         converter = AjaxSelectWidgetConverter(field, widget)
 
         self.assertEqual(
@@ -1124,27 +1124,27 @@
 
         self.assertEqual(
             converter.toWidgetValue(("123", "456", "789")),
             "123;456;789",
         )
 
     def test_fieldwidget(self):
-        from plone.app.z3cform.widget import AjaxSelectFieldWidget
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectFieldWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         field = Mock(__name__="field", title="", required=True)
         request = Mock()
         widget = AjaxSelectFieldWidget(field, request)
         self.assertTrue(isinstance(widget, AjaxSelectWidget))
         self.assertIs(widget.field, field)
         self.assertIs(widget.request, request)
 
     def test_fieldwidget_sequence(self):
-        from plone.app.z3cform.widget import AjaxSelectFieldWidget
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectFieldWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         field = Mock(__name__="field", title="", required=True)
         vocabulary = Mock()
         request = Mock()
         widget = AjaxSelectFieldWidget(field, vocabulary, request)
         self.assertTrue(isinstance(widget, AjaxSelectWidget))
         self.assertIs(widget.field, field)
@@ -1154,39 +1154,50 @@
 class AjaxSelectWidgetIntegrationTests(unittest.TestCase):
     layer = PAZ3CForm_INTEGRATION_TESTING
 
     def setUp(self):
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
 
     def test_keywords_can_add(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         portal = self.layer["portal"]
         setRoles(portal, TEST_USER_ID, ["Manager"])
         widget = AjaxSelectWidget(self.request)
         widget.context = portal
         widget.vocabulary = "plone.app.vocabularies.Keywords"
         self.assertEqual(
             widget._base_args()["pattern_options"]["allowNewItems"],
             "true",
         )
 
     def test_keywords_cannot_add(self):
-        from plone.app.z3cform.widget import AjaxSelectWidget
+        from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
         portal = self.layer["portal"]
         widget = AjaxSelectWidget(self.request)
         widget.context = portal
         widget.vocabulary = "plone.app.vocabularies.Keywords"
         self.assertEqual(
             widget._base_args()["pattern_options"]["allowNewItems"],
             "false",
         )
 
 
+def mock_querystring_options(context, querystring_view):
+    return {
+        "indexOptionsUrl": f"/{querystring_view}",
+        "previewURL": "/@@querybuilder_html_results",
+        "previewCountURL": "/@@querybuildernumberofresults",
+        "patternDateOptions": None,
+        "patternAjaxSelectOptions": {"separator": ";"},
+        "patternRelateditemsOptions": None,
+    }
+
+
 class QueryStringWidgetTests(unittest.TestCase):
     def setUp(self):
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
 
     def test_converter_toWidgetValue(self):
         from plone.app.z3cform.converters import QueryStringDataConverter
 
@@ -1198,23 +1209,19 @@
         from plone.app.z3cform.converters import QueryStringDataConverter
 
         converter = QueryStringDataConverter(List(), None)
         self.assertEqual(converter.toFieldValue(""), None)
         self.assertEqual(converter.toFieldValue("[]"), None)
 
     @mock.patch(
-        "plone.app.widgets.utils.get_date_options",
-        new=lambda *args, **kwargs: None,
-    )
-    @mock.patch(
-        "plone.app.widgets.utils.get_relateditems_options",
-        new=lambda *args, **kwargs: None,
+        "plone.app.z3cform.widgets.querystring.get_querystring_options",
+        new=mock_querystring_options,
     )
     def test_widget(self):
-        from plone.app.z3cform.widget import QueryStringWidget
+        from plone.app.z3cform.widgets.querystring import QueryStringWidget
 
         widget = QueryStringWidget(self.request)
         self.assertEqual(
             {
                 "name": None,
                 "value": "",
                 "pattern": "querystring",
@@ -1245,15 +1252,15 @@
         https://bugs.python.org/issue9424
         To not introduce a forward incompatibility, here is a replacement based
         on: http://stackoverflow.com/a/21058312
         """
         return set(expected.items()).issubset(set(actual.items()))
 
     def test_related_items_widget(self):
-        from plone.app.z3cform.widget import RelatedItemsWidget
+        from plone.app.z3cform.widgets.relateditems import RelatedItemsWidget
 
         EXPECTED_ROOT_PATH = "/plone"
         EXPECTED_ROOT_URL = "http://nohost/plone"
         EXPECTED_BASE_PATH = "/plone"
         EXPECTED_VOCAB_URL = "http://nohost/plone/@@getVocabulary?name=plone.app.vocabularies.Catalog"  # noqa
 
         widget = RelatedItemsWidget(self.request)
@@ -1277,15 +1284,15 @@
         self.assertEqual(
             EXPECTED_VOCAB_URL,
             result["pattern_options"]["vocabularyUrl"],
         )
 
     def test_related_items_widget_nav_root(self):
         from plone.app.layout.navigation.interfaces import INavigationRoot
-        from plone.app.z3cform.widget import RelatedItemsWidget
+        from plone.app.z3cform.widgets.relateditems import RelatedItemsWidget
 
         EXPECTED_ROOT_PATH = "/plone"
         EXPECTED_ROOT_URL = "http://nohost/plone"
         EXPECTED_BASE_PATH = "/plone/subfolder"
         EXPECTED_VOCAB_URL = "http://nohost/plone/@@getVocabulary?name=plone.app.vocabularies.Catalog"  # noqa
 
         self.portal.invokeFactory("Folder", "subfolder")
@@ -1401,21 +1408,21 @@
 
 
 class RelatedItemsWidgetTests(unittest.TestCase):
     def setUp(self):
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
 
     @mock.patch(
-        "plone.app.widgets.utils.getToolByName",
+        "Products.CMFCore.utils.getToolByName",
         new=Mock(return_value=Mock(return_value="testuser")),
     )
     def test_single_selection(self):
         """The pattern_options value for maximumSelectionSize should
         be 1 when the field only allows a single selection."""
-        from plone.app.z3cform.widget import RelatedItemsFieldWidget
+        from plone.app.z3cform.widgets.relateditems import RelatedItemsFieldWidget
 
         context = Mock(
             absolute_url=lambda: "fake_url", getPhysicalPath=lambda: ["", "site"]
         )
         field = Choice(
             __name__="selectfield",
             values=["one", "two", "three"],
@@ -1424,21 +1431,21 @@
         widget.context = context
         widget.update()
         base_args = widget._base_args()
         pattern_options = base_args["pattern_options"]
         self.assertEqual(pattern_options.get("maximumSelectionSize", 0), 1)
 
     @mock.patch(
-        "plone.app.widgets.utils.getToolByName",
+        "Products.CMFCore.utils.getToolByName",
         new=Mock(return_value=Mock(return_value="testuser")),
     )
     def test_multiple_selection(self):
         """The pattern_options key maximumSelectionSize shouldn't be
         set when the field allows multiple selections"""
-        from plone.app.z3cform.widget import RelatedItemsFieldWidget
+        from plone.app.z3cform.widgets.relateditems import RelatedItemsFieldWidget
         from zope.schema.interfaces import ISource
         from zope.schema.vocabulary import VocabularyRegistry
 
         context = Mock(
             absolute_url=lambda: "fake_url", getPhysicalPath=lambda: ["", "site"]
         )
         field = List(
@@ -1558,16 +1565,16 @@
             self.assertEqual(converter.toFieldValue(None), None)
             self.assertEqual(
                 type(converter.toFieldValue("id1;id2")[0]),
                 expected_value_type,
             )
 
     def test_fieldwidget(self):
-        from plone.app.z3cform.widget import RelatedItemsFieldWidget
-        from plone.app.z3cform.widget import RelatedItemsWidget
+        from plone.app.z3cform.widgets.relateditems import RelatedItemsFieldWidget
+        from plone.app.z3cform.widgets.relateditems import RelatedItemsWidget
 
         field = Mock(__name__="field", title="", required=True)
         vocabulary = Mock()
         request = Mock()
         widget = RelatedItemsFieldWidget(field, vocabulary, request)
         self.assertTrue(isinstance(widget, RelatedItemsWidget))
         self.assertIs(widget.field, field)
@@ -1575,21 +1582,21 @@
 
 
 def add_mock_fti(portal):
     # Fake DX Type
     fti = DexterityFTI("dx_mock")
     portal.portal_types._setObject("dx_mock", fti)
     fti.klass = "plone.dexterity.content.Item"
-    fti.schema = "plone.app.widgets.tests.test_dx.IMockSchema"
+    fti.schema = "plone.dexterity.tests.schemata.ITestSchema"
     fti.filter_content_types = False
     fti.behaviors = ("plone.app.dexterity.behaviors.metadata.IBasic",)
 
 
 def _custom_field_widget(field, request):
-    from plone.app.z3cform.widget import AjaxSelectWidget
+    from plone.app.z3cform.widgets.select import AjaxSelectWidget
 
     widget = FieldWidget(field, AjaxSelectWidget(request))
     widget.vocabulary = "plone.app.vocabularies.PortalTypes"
     return widget
 
 
 class RichTextWidgetTests(unittest.TestCase):
@@ -1607,15 +1614,15 @@
 
         class IWithText(Interface):
             text = RichTextField(title="Text")
 
         self.field = IWithText["text"]
 
     def test_widget_params(self):
-        from plone.app.z3cform.widget import RichTextWidget
+        from plone.app.z3cform.widgets.richtext import RichTextWidget
 
         widget = FieldWidget(self.field, RichTextWidget(self.request))
         # set the context so we can get tinymce settings
         widget.context = self.portal
         widget.update()
         base_args = widget._base_args()
         self.assertEqual(base_args["name"], "text")
@@ -1629,15 +1636,15 @@
         )
         self.assertEqual(
             base_args["pattern_options"]["upload"]["relativePath"],
             "@@fileUpload",
         )
 
     def test_widget_params_different_contexts(self):
-        from plone.app.z3cform.widget import RichTextWidget
+        from plone.app.z3cform.widgets.richtext import RichTextWidget
 
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
 
         widget = FieldWidget(self.field, RichTextWidget(self.request))
         self.portal.invokeFactory("Folder", "sub")
         sub = self.portal.sub
         form = Form(sub, self.request)
@@ -1680,15 +1687,15 @@
         self.assertEqual(
             base_args["pattern_options"]["relatedItems"]["basePath"],
             "/plone",
         )
 
     def test_widget_values(self):
         from plone.app.textfield.value import RichTextValue
-        from plone.app.z3cform.widget import RichTextWidget
+        from plone.app.z3cform.widgets.richtext import RichTextWidget
 
         widget = FieldWidget(self.field, RichTextWidget(self.request))
         # set the context so we can get tinymce settings
         widget.context = self.portal
         widget.value = RichTextValue("Lorem ipsum \u2026")
         base_args = widget._base_args()
         self.assertEqual(base_args["value"], "Lorem ipsum \u2026")
@@ -1707,15 +1714,15 @@
     def test_dx_tinymcewidget_single_mimetype(self):
         """A RichTextWidget with only one available mimetype should render the
         pattern class directly on itself.
         """
         if IMarkupSchema:
             # if not, don't run this test
             self._set_mimetypes(allowed=("text/html",))
-            from plone.app.z3cform.widget import RichTextWidget
+            from plone.app.z3cform.widgets.richtext import RichTextWidget
 
             widget = FieldWidget(self.field, RichTextWidget(self.request))
             # set the context so we can get tinymce settings
             widget.context = self.portal
             rendered = widget.render()
 
             self.assertTrue("<select" not in rendered)
@@ -1726,15 +1733,15 @@
         """A RichTextWidget with multiple available mimetypes should render a
         mimetype selection widget along with the textfield. When there is no
         field value, the default mimetype should be preselected.
         """
         if IMarkupSchema:
             # if not, don't run this test
             self._set_mimetypes(allowed=("text/html", "text/plain"))
-            from plone.app.z3cform.widget import RichTextWidget
+            from plone.app.z3cform.widgets.richtext import RichTextWidget
 
             widget = FieldWidget(self.field, RichTextWidget(self.request))
             # set the context so we can get tinymce settings
             widget.context = self.portal
             rendered = widget.render()
 
             self.assertTrue("<select" in rendered)
@@ -1750,15 +1757,15 @@
         mimetype selection widget along with the textfield. When there is
         already a RichTextValue, it's mimetype should be preselected.
         """
         if IMarkupSchema:
             # if not, don't run this test
             self._set_mimetypes(allowed=("text/html", "text/plain"))
             from plone.app.textfield.value import RichTextValue
-            from plone.app.z3cform.widget import RichTextWidget
+            from plone.app.z3cform.widgets.richtext import RichTextWidget
 
             widget = FieldWidget(self.field, RichTextWidget(self.request))
             # set the context so we can get tinymce settings
             widget.context = self.portal
             widget.value = RichTextValue("Hello world", mimeType="text/plain")
             rendered = widget.render()
 
@@ -1777,23 +1784,23 @@
             self._set_mimetypes(allowed=("text/html",))
             registry = getUtility(IRegistry)
             from plone.base.interfaces import IEditingSchema
 
             proxy = registry.forInterface(IEditingSchema, check=False, prefix="plone")
             proxy.available_editors = ["dummy", "TinyMCE"]
             proxy.default_editor = "dummy"
-            from plone.app.z3cform.widget import RichTextWidget
+            from plone.app.z3cform.widgets.richtext import RichTextWidget
 
             widget = FieldWidget(self.field, RichTextWidget(self.request))
             widget.context = self.portal
             rendered = widget.render()
             self.assertTrue("<p>dummy</p>" in rendered)
 
             proxy.default_editor = "TinyMCE"
-            from plone.app.z3cform.widget import RichTextWidget
+            from plone.app.z3cform.widgets.richtext import RichTextWidget
 
             widget = FieldWidget(self.field, RichTextWidget(self.request))
             widget.context = self.portal
             rendered = widget.render()
             self.assertTrue("pat-tinymce" in rendered)
 
 
@@ -1803,84 +1810,84 @@
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
         setRequest(self.request)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
     def test_link_widget__pattern_options(self):
-        from plone.app.z3cform.widget import LinkWidget
+        from plone.app.z3cform.widgets.link import LinkWidget
 
         widget = LinkWidget(self.request)
 
         pattern_data = json.loads(widget.pattern_data())
         self.assertEqual(
             pattern_data["vocabularyUrl"],
             "http://nohost/plone/@@getVocabulary?name=plone.app.vocabularies.Catalog",  # noqa
         )
         self.assertEqual(pattern_data["maximumSelectionSize"], 1)
 
     def test_link_widget__extract_internal(self):
-        from plone.app.z3cform.widget import LinkWidget
+        from plone.app.z3cform.widgets.link import LinkWidget
 
         widget = LinkWidget(self.request)
         widget.context = self.portal
         widget.name = "testlinkwidget"
         widget.update()
 
         self.request.form["testlinkwidget.internal"] = "abc"
         self.assertEqual(
             widget.extract(),
             "${portal_url}/resolveuid/abc",
         )
 
     def test_link_widget__extract_external(self):
-        from plone.app.z3cform.widget import LinkWidget
+        from plone.app.z3cform.widgets.link import LinkWidget
 
         widget = LinkWidget(self.request)
         widget.context = self.portal
         widget.name = "testlinkwidget"
         widget.update()
 
         self.request.form["testlinkwidget.external"] = "https://plone.org"
         self.assertEqual(
             widget.extract(),
             "https://plone.org",
         )
 
     def test_link_widget__extract_email(self):
-        from plone.app.z3cform.widget import LinkWidget
+        from plone.app.z3cform.widgets.link import LinkWidget
 
         widget = LinkWidget(self.request)
         widget.context = self.portal
         widget.name = "testlinkwidget"
         widget.update()
 
         self.request.form["testlinkwidget.email"] = "dev@plone.org"
         self.assertEqual(
             widget.extract(),
             "mailto:dev@plone.org",
         )
 
     def test_link_widget__extract_email_including_mailto(self):
-        from plone.app.z3cform.widget import LinkWidget
+        from plone.app.z3cform.widgets.link import LinkWidget
 
         widget = LinkWidget(self.request)
         widget.context = self.portal
         widget.name = "testlinkwidget"
         widget.update()
 
         self.request.form["testlinkwidget.email"] = "mailto:dev@plone.org"
         self.assertEqual(
             widget.extract(),
             "mailto:dev@plone.org",
         )
 
     def test_link_widget__data_converter(self):
         from plone.app.z3cform.converters import LinkWidgetDataConverter
-        from plone.app.z3cform.widget import LinkWidget
+        from plone.app.z3cform.widgets.link import LinkWidget
 
         field = TextLine(__name__="linkfield")
         widget = LinkWidget(self.request)
         converter = LinkWidgetDataConverter(field, widget)
 
         self.portal.invokeFactory("Folder", "test")
         portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/testing.zcml` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/tests.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/views.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/views.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/widget.zcml` & `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:z3c="http://namespaces.zope.org/z3c"
-    i18n_domain="plone"
     >
 
   <!-- Make the default widget for sequence-of-text-lines a textlines
        widget; the default is too confusing -->
 
   <adapter
       factory="plone.z3cform.textlines.textlines.TextLinesFieldWidgetFactory"
       provides="z3c.form.interfaces.IFieldWidget"
       for="zope.schema.interfaces.IList
            zope.schema.interfaces.ITextLine
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
+
   <adapter
       factory="plone.z3cform.textlines.textlines.TextLinesFieldWidgetFactory"
       provides="z3c.form.interfaces.IFieldWidget"
       for="zope.schema.interfaces.ITuple
            zope.schema.interfaces.ITextLine
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
+
   <adapter
       factory="plone.z3cform.textlines.textlines.TextLinesFieldWidgetFactory"
       provides="z3c.form.interfaces.IFieldWidget"
       for="zope.schema.interfaces.IAbstractSet
            zope.schema.interfaces.ITextLine
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
@@ -32,14 +33,15 @@
   <adapter
       factory="plone.z3cform.textlines.textlines.TextLinesFieldWidgetFactory"
       provides="z3c.form.interfaces.IFieldWidget"
       for="zope.schema.interfaces.IList
            zope.schema.interfaces.IASCIILine
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
+
   <adapter
       factory="plone.z3cform.textlines.textlines.TextLinesFieldWidgetFactory"
       provides="z3c.form.interfaces.IFieldWidget"
       for="zope.schema.interfaces.ITuple
            zope.schema.interfaces.IASCIILine
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
@@ -47,156 +49,167 @@
       factory="plone.z3cform.textlines.textlines.TextLinesFieldWidgetFactory"
       provides="z3c.form.interfaces.IFieldWidget"
       for="zope.schema.interfaces.IAbstractSet
            zope.schema.interfaces.IASCIILine
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
+  <!-- single checkbox boolean -->
   <adapter
-      factory=".widget.SingleCheckBoxBoolFieldWidget"
+      factory=".widgets.singlecheckbox.SingleCheckBoxBoolFieldWidget"
       for="zope.schema.interfaces.IBool
            .interfaces.IPloneFormLayer"
       />
-  <adapter factory=".converters.BoolSingleCheckboxDataConverter" />
 
   <z3c:widgetTemplate
       field="zope.schema.interfaces.IBool"
       widget=".interfaces.ISingleCheckBoxBoolWidget"
       template="templates/singlecheckboxbool_display.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="display"
       />
+
   <z3c:widgetTemplate
       field="zope.schema.interfaces.IBool"
       widget=".interfaces.ISingleCheckBoxBoolWidget"
       template="templates/singlecheckboxbool_input.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="input"
       />
+
+  <!-- ajaxselect -->
   <z3c:widgetTemplate
       field="*"
       widget=".interfaces.IAjaxSelectWidget"
       template="templates/ajaxselect_display.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="display"
       />
+
   <z3c:widgetTemplate
       field="zope.schema.interfaces.IBool"
       widget=".interfaces.ISingleCheckBoxBoolWidget"
       template="templates/singlecheckboxbool_hidden.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="hidden"
       />
 
+  <!-- multi -->
   <z3c:widgetTemplate
       widget="z3c.form.interfaces.IMultiWidget"
       template="templates/multi_input.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="input"
       />
 
+  <!-- object -->
   <z3c:widgetTemplate
       widget="z3c.form.interfaces.IObjectWidget"
       template="templates/object_input.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="input"
       />
 
-  <z3c:widgetTemplate
-      widget=".interfaces.ILinkWidget"
-      template="templates/link_input.pt"
-      layer=".interfaces.IPloneFormLayer"
-      mode="input"
-      />
-
-  <z3c:widgetTemplate
-      widget=".interfaces.IRelatedItemsWidget"
-      template="templates/relateditems_display.pt"
-      layer=".interfaces.IPloneFormLayer"
-      mode="display"
-      />
-
-  <!-- widget registration stuff -->
-  <class class=".widget.DateWidget">
+  <!-- date/time -->
+  <class class=".widgets.datetime.DateWidget">
     <require
         permission="zope.Public"
         interface=".interfaces.IDateWidget"
         />
   </class>
 
   <adapter
-      factory=".widget.DateFieldWidget"
+      factory=".widgets.datetime.DateFieldWidget"
       for="zope.schema.interfaces.IDate
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
-  <class class=".widget.DatetimeWidget">
+  <class class=".widgets.datetime.DatetimeWidget">
     <require
         permission="zope.Public"
         interface=".interfaces.IDatetimeWidget"
         />
   </class>
 
   <adapter
-      factory=".widget.DatetimeFieldWidget"
+      factory=".widgets.datetime.DatetimeFieldWidget"
       for="zope.schema.interfaces.IDatetime
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
-  <class class=".widget.TimeWidget">
+  <class class=".widgets.datetime.TimeWidget">
     <require
         permission="zope.Public"
         interface=".interfaces.ITimeWidget"
         />
   </class>
 
   <adapter
-      factory=".widget.TimeFieldWidget"
+      factory=".widgets.datetime.TimeFieldWidget"
       for="zope.schema.interfaces.ITime
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
+  <!-- relateditems -->
+
   <adapter
-      factory=".widget.RelatedItemsFieldWidget"
+      factory=".widgets.relateditems.RelatedItemsFieldWidget"
       for="z3c.relationfield.interfaces.IRelationChoice
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
   <adapter
-      factory=".widget.RelatedItemsFieldWidget"
+      factory=".widgets.relateditems.RelatedItemsFieldWidget"
       for="z3c.relationfield.interfaces.IRelationList
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
   <adapter
-      factory=".widget.RelatedItemsFieldWidget"
+      factory=".widgets.relateditems.RelatedItemsFieldWidget"
       for="zope.schema.interfaces.IChoice
            plone.app.vocabularies.catalog.CatalogSource
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
+  <z3c:widgetTemplate
+      widget=".interfaces.IRelatedItemsWidget"
+      template="templates/relateditems_display.pt"
+      layer=".interfaces.IPloneFormLayer"
+      mode="display"
+      />
+
+  <!-- querystring -->
   <adapter
-      factory=".widget.QueryStringFieldWidget"
+      factory=".widgets.querystring.QueryStringFieldWidget"
       for="zope.schema.interfaces.IList
            zope.schema.interfaces.IDict
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
+  <!-- richtext -->
   <adapter
-      factory=".widget.RichTextFieldWidget"
+      factory=".widgets.richtext.RichTextFieldWidget"
       for="plone.app.textfield.interfaces.IRichText
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
+  <!-- link -->
   <adapter
-      factory=".widget.LinkFieldWidget"
+      factory=".widgets.link.LinkFieldWidget"
       for="z3c.form.interfaces.ITextWidget
            plone.app.z3cform.interfaces.IPloneFormLayer"
       />
 
+  <z3c:widgetTemplate
+      widget=".interfaces.ILinkWidget"
+      template="templates/link_input.pt"
+      layer=".interfaces.IPloneFormLayer"
+      mode="input"
+      />
+
   <!-- z3c.form overrides -->
 
   <z3c:widgetTemplate
       widget="z3c.form.interfaces.ITextWidget"
       template="templates/text_input.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="input"
@@ -293,8 +306,14 @@
   <z3c:widgetTemplate
       widget="plone.app.textfield.widget.IRichTextWidget"
       template="templates/textfield_widget_input.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="input"
       />
 
+  <utility
+      provides="plone.app.z3cform.interfaces.IRichTextWidgetInputModeRenderer"
+      name="tinymce"
+      component=".widgets.richtext.tinymce_richtextwidget_render"
+      />
+
 </configure>
```

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/README.rst` & `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/configure.zcml` & `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/widget.py` & `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_display.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_input.pt` & `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/PKG-INFO` & `plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.0.3
+Version: 4.1.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -677,14 +677,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2023-04-26)
+------------------
+
+New features:
+
+
+- Merge utils and base classes from  ``plone.app.widgets`` and do not depend
+  on it anymore. [petschki] (#19)
+
+
 4.0.3 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fixes transitive circular dependency to plone.schema.
```

### Comparing `plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/SOURCES.txt` & `plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 plone.app.z3cform.egg-info/not-zip-safe
 plone.app.z3cform.egg-info/requires.txt
 plone.app.z3cform.egg-info/top_level.txt
 plone/app/__init__.py
 plone/app/z3cform/__init__.py
 plone/app/z3cform/configure.zcml
 plone/app/z3cform/converters.py
+plone/app/z3cform/converters.zcml
 plone/app/z3cform/csrf.py
 plone/app/z3cform/factories.py
 plone/app/z3cform/inline_validation.py
 plone/app/z3cform/inline_validation.rst
 plone/app/z3cform/interfaces.py
 plone/app/z3cform/layout.py
 plone/app/z3cform/overrides.zcml
 plone/app/z3cform/profiles.zcml
 plone/app/z3cform/utils.py
 plone/app/z3cform/views.py
 plone/app/z3cform/widget.py
-plone/app/z3cform/widget.zcml
+plone/app/z3cform/widgets.zcml
 plone/app/z3cform/profiles/default/browserlayer.xml
 plone/app/z3cform/profiles/default/metadata.xml
 plone/app/z3cform/templates/ajaxselect_display.pt
 plone/app/z3cform/templates/checkbox_input.pt
 plone/app/z3cform/templates/contentprovider-widget.pt
 plone/app/z3cform/templates/error.pt
 plone/app/z3cform/templates/file_input.pt
@@ -61,18 +62,29 @@
 plone/app/z3cform/templates/textfield_widget_input.pt
 plone/app/z3cform/templates/textlines_input.pt
 plone/app/z3cform/templates/widget.pt
 plone/app/z3cform/tests/__init__.py
 plone/app/z3cform/tests/example.py
 plone/app/z3cform/tests/layer.py
 plone/app/z3cform/tests/test_csrf.py
+plone/app/z3cform/tests/test_patterns.py
 plone/app/z3cform/tests/test_utils.py
 plone/app/z3cform/tests/test_widget.py
 plone/app/z3cform/tests/test_widgets.py
 plone/app/z3cform/tests/testing.zcml
 plone/app/z3cform/tests/tests.py
+plone/app/z3cform/widgets/__init__.py
+plone/app/z3cform/widgets/base.py
+plone/app/z3cform/widgets/datetime.py
+plone/app/z3cform/widgets/link.py
+plone/app/z3cform/widgets/patterns.py
+plone/app/z3cform/widgets/querystring.py
+plone/app/z3cform/widgets/relateditems.py
+plone/app/z3cform/widgets/richtext.py
+plone/app/z3cform/widgets/select.py
+plone/app/z3cform/widgets/singlecheckbox.py
 plone/app/z3cform/wysiwyg/README.rst
 plone/app/z3cform/wysiwyg/__init__.py
 plone/app/z3cform/wysiwyg/configure.zcml
 plone/app/z3cform/wysiwyg/widget.py
 plone/app/z3cform/wysiwyg/wysiwyg_display.pt
 plone/app/z3cform/wysiwyg/wysiwyg_input.pt
```

### Comparing `plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/requires.txt` & `plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-lxml
-plone.app.contentlisting
-plone.app.vocabularies
 plone.app.textfield>=1.3.6
-plone.app.widgets>=2.4.2
 plone.base
-plone.dexterity
-plone.i18n
-plone.namedfile
 plone.protect
 plone.registry
 plone.schema
 plone.uuid
 plone.z3cform
 Products.GenericSetup
 pytz
 setuptools
 z3c.form>=4.0
-z3c.relationfield
-zope.browserpage
-zope.contentprovider
+z3c.formwidget.query
+zope.deprecation
 zope.globalrequest
-zope.pagetemplate
 Zope
 
 [test]
 plone.app.contenttypes[test]
 plone.app.layout
 plone.app.testing
 plone.autoform
```

### Comparing `plone.app.z3cform-4.0.3/pyproject.toml` & `plone.app.z3cform-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.3/setup.py` & `plone.app.z3cform-4.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
-version = "4.0.3"
+version = "4.1.0"
 
 long_description = (
     read("README.rst")
     + "\n"
     + read("plone", "app", "z3cform", "wysiwyg", "README.rst")
     + "\n"
     + read("plone", "app", "z3cform", "inline_validation.rst")
@@ -61,37 +61,28 @@
     license="GPL",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
-        "lxml",
-        "plone.app.contentlisting",
-        "plone.app.vocabularies",
         "plone.app.textfield>=1.3.6",
-        "plone.app.widgets>=2.4.2",
         "plone.base",
-        "plone.dexterity",
-        "plone.i18n",
-        "plone.namedfile",
         "plone.protect",
         "plone.registry",
         "plone.schema",
         "plone.uuid",
         "plone.z3cform",
         "Products.GenericSetup",
         "pytz",
         "setuptools",
         "z3c.form >= 4.0",
-        "z3c.relationfield",
-        "zope.browserpage",
-        "zope.contentprovider",
+        "z3c.formwidget.query",
+        "zope.deprecation",
         "zope.globalrequest",
-        "zope.pagetemplate",
         "Zope",
     ],
     extras_require={
         # Until plone.app.z3cform 4.0.2 we only had the 'tests' extra.
         # In 4.0.3 we introduced the 'test' extra.
         # Keep 'tests' for backwards compatibility.
         # Remove it in Plone 7.
```

