# Comparing `tmp/collective.z3cform.jsonwidget-1.1.1.tar.gz` & `tmp/collective.z3cform.jsonwidget-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.z3cform.jsonwidget-1.1.1.tar", last modified: Fri Apr 21 08:41:25 2023, max compression
+gzip compressed data, was "collective.z3cform.jsonwidget-1.1.2.tar", last modified: Wed Apr 26 20:41:38 2023, max compression
```

## Comparing `collective.z3cform.jsonwidget-1.1.1.tar` & `collective.z3cform.jsonwidget-1.1.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.672797 collective.z3cform.jsonwidget-1.1.1/
--rw-r--r--   0 cekk       (501) staff       (20)      376 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/.eslintrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      278 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/.prettierrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      131 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/.stylelintrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      895 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       70 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      673 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      234 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     6632 2023-04-21 08:41:25.673022 collective.z3cform.jsonwidget-1.1.1/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2967 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/constraints_plone51.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.657861 collective.z3cform.jsonwidget-1.1.1/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7935 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)      110 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)     3013 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/package.json
--rw-r--r--   0 cekk       (501) staff       (20)      256 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/postcss.config.js
--rw-r--r--   0 cekk       (501) staff       (20)       50 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      321 2023-04-21 08:41:25.673479 collective.z3cform.jsonwidget-1.1.1/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2603 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.648833 collective.z3cform.jsonwidget-1.1.1/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.658110 collective.z3cform.jsonwidget-1.1.1/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.660573 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.662167 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/
--rw-r--r--   0 cekk       (501) staff       (20)      146 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.663119 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      847 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      366 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/json_widget_input.pt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.649751 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.649612 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.664465 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/
--rw-r--r--   0 cekk       (501) staff       (20)     2520 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css
--rw-r--r--   0 cekk       (501) staff       (20)     2879 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map
--rw-r--r--   0 cekk       (501) staff       (20)   330486 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js
--rw-r--r--   0 cekk       (501) staff       (20)      198 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.664760 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.665010 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/
--rw-r--r--   0 cekk       (501) staff       (20)      494 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.665514 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     1523 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.665708 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     3839 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.666197 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     4726 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js
--rw-r--r--   0 cekk       (501) staff       (20)     1006 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.667954 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/
--rw-r--r--   0 cekk       (501) staff       (20)     2790 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js
--rw-r--r--   0 cekk       (501) staff       (20)      370 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.less
--rw-r--r--   0 cekk       (501) staff       (20)     8758 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js
--rw-r--r--   0 cekk       (501) staff       (20)     1335 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less
--rw-r--r--   0 cekk       (501) staff       (20)     1324 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js
--rw-r--r--   0 cekk       (501) staff       (20)      354 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextAreaField.js
--rw-r--r--   0 cekk       (501) staff       (20)      961 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js
--rw-r--r--   0 cekk       (501) staff       (20)      767 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.668436 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/
--rw-r--r--   0 cekk       (501) staff       (20)      953 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js
--rw-r--r--   0 cekk       (501) staff       (20)      274 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/widgetContext.js
--rw-r--r--   0 cekk       (501) staff       (20)     2482 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/widget.py
--rw-r--r--   0 cekk       (501) staff       (20)     1432 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      277 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.669830 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1328 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.651121 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.670317 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      988 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1541 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po
--rw-r--r--   0 cekk       (501) staff       (20)     1027 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/manual.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1701 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      543 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      260 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.651538 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.671559 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      212 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      195 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)     1084 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.672086 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      139 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      478 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      630 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1724 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.672509 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2678 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/test_setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.660332 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     6632 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3950 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      154 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       30 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      173 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)     2795 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/webpack.config.js
--rw-r--r--   0 cekk       (501) staff       (20)   471705 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/yarn.lock
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.604354 collective.z3cform.jsonwidget-1.1.2/
+-rw-r--r--   0 cekk       (501) staff       (20)      376 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/.eslintrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      278 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/.prettierrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      131 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/.stylelintrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      960 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       70 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      673 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      234 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     6746 2023-04-26 20:41:38.604532 collective.z3cform.jsonwidget-1.1.2/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2967 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.587634 collective.z3cform.jsonwidget-1.1.2/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7935 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)      110 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     3013 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)      256 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/postcss.config.js
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      321 2023-04-26 20:41:38.605007 collective.z3cform.jsonwidget-1.1.2/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2618 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.577853 collective.z3cform.jsonwidget-1.1.2/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.587877 collective.z3cform.jsonwidget-1.1.2/src/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.590431 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.592279 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/
+-rw-r--r--   0 cekk       (501) staff       (20)      146 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.593327 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      847 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      366 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/json_widget_input.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.578888 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.578726 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.594739 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/
+-rw-r--r--   0 cekk       (501) staff       (20)     2520 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css
+-rw-r--r--   0 cekk       (501) staff       (20)     2879 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)   330486 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)      198 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.595034 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.595286 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)      494 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.595814 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     1523 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.596075 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     3839 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.596746 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     4726 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1006 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.598827 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/
+-rw-r--r--   0 cekk       (501) staff       (20)     2790 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      370 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     8758 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1335 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     1324 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      354 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextAreaField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      961 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      767 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.599336 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/utils/
+-rw-r--r--   0 cekk       (501) staff       (20)      953 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js
+-rw-r--r--   0 cekk       (501) staff       (20)      274 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/utils/widgetContext.js
+-rw-r--r--   0 cekk       (501) staff       (20)     2482 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/widget.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1432 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      277 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.601007 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1328 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.580428 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.601664 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      988 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1541 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1027 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1701 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      543 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      260 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.580861 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.603124 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      212 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      195 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     1084 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.603619 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      139 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      478 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      630 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1724 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.604141 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2678 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-26 20:41:38.590184 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     6746 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3950 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      154 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       30 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      173 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-26 20:41:38.000000 collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)     2795 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/webpack.config.js
+-rw-r--r--   0 cekk       (501) staff       (20)   471705 2023-04-26 20:41:37.000000 collective.z3cform.jsonwidget-1.1.2/yarn.lock
```

### Comparing `collective.z3cform.jsonwidget-1.1.1/CHANGES.rst` & `collective.z3cform.jsonwidget-1.1.2/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.1.2 (2023-04-26)
+------------------
+
+- Fix release.
+  [cekk]
+
+
 1.1.1 (2023-04-21)
 ------------------
 
 - Handle integer fields.
   [cekk]
 
 1.1.0 (2022-07-18)
```

### Comparing `collective.z3cform.jsonwidget-1.1.1/DEVELOP.rst` & `collective.z3cform.jsonwidget-1.1.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/LICENSE.GPL` & `collective.z3cform.jsonwidget-1.1.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/LICENSE.rst` & `collective.z3cform.jsonwidget-1.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/PKG-INFO` & `collective.z3cform.jsonwidget-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.z3cform.jsonwidget
-Version: 1.1.1
+Version: 1.1.2
 Summary: Custom widget to manage complex json data stored into a text field
 Home-page: https://github.com/collective/collective.z3cform.jsonwidget
 Author: Andrea Cecchi
 Author-email: andrea.cecchi85@gmail.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.z3cform.jsonwidget
 Project-URL: Source, https://github.com/collective/collective.z3cform.jsonwidget
@@ -140,14 +140,21 @@
         - Andrea Cecchi, andrea.cecchi85@gmail.com
         
         
         Changelog
         =========
         
         
+        1.1.2 (2023-04-26)
+        ------------------
+        
+        - Fix release.
+          [cekk]
+        
+        
         1.1.1 (2023-04-21)
         ------------------
         
         - Handle integer fields.
           [cekk]
         
         1.1.0 (2022-07-18)
@@ -214,9 +221,9 @@
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7, >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
```

### Comparing `collective.z3cform.jsonwidget-1.1.1/README.rst` & `collective.z3cform.jsonwidget-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/docs/conf.py` & `collective.z3cform.jsonwidget-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/package.json` & `collective.z3cform.jsonwidget-1.1.2/package.json`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/setup.py` & `collective.z3cform.jsonwidget-1.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 """Installer for the collective.z3cform.jsonwidget package."""
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-long_description = '\n\n'.join([
-    open('README.rst').read(),
-    open('CONTRIBUTORS.rst').read(),
-    open('CHANGES.rst').read(),
-])
+long_description = "\n\n".join(
+    [
+        open("README.rst").read(),
+        open("CONTRIBUTORS.rst").read(),
+        open("CHANGES.rst").read(),
+    ]
+)
 
 
 setup(
-    name='collective.z3cform.jsonwidget',
-    version='1.1.1',
+    name="collective.z3cform.jsonwidget",
+    version="1.1.2",
     description="Custom widget to manage complex json data stored into a text field",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -26,48 +28,48 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
-    keywords='Python Plone',
-    author='Andrea Cecchi',
-    author_email='andrea.cecchi85@gmail.com',
-    url='https://github.com/collective/collective.z3cform.jsonwidget',
+    keywords="Python Plone",
+    author="Andrea Cecchi",
+    author_email="andrea.cecchi85@gmail.com",
+    url="https://github.com/collective/collective.z3cform.jsonwidget",
     project_urls={
-        'PyPI': 'https://pypi.python.org/pypi/collective.z3cform.jsonwidget',
-        'Source': 'https://github.com/collective/collective.z3cform.jsonwidget',
-        'Tracker': 'https://github.com/collective/collective.z3cform.jsonwidget/issues',
+        "PyPI": "https://pypi.python.org/pypi/collective.z3cform.jsonwidget",
+        "Source": "https://github.com/collective/collective.z3cform.jsonwidget",
+        "Tracker": "https://github.com/collective/collective.z3cform.jsonwidget/issues",
         # 'Documentation': 'https://collective.z3cform.jsonwidget.readthedocs.io/en/latest/',
     },
-    license='GPL version 2',
-    packages=find_packages('src', exclude=['ez_setup']),
-    namespace_packages=['collective', 'collective.z3cform'],
-    package_dir={'': 'src'},
+    license="GPL version 2",
+    packages=find_packages("src", exclude=["ez_setup"]),
+    namespace_packages=["collective", "collective.z3cform"],
+    package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7, >=3.6",
+    python_requires=">=3.7",
     install_requires=[
-        'setuptools',
+        "setuptools",
         # -*- Extra requirements: -*-
-        'z3c.jbot',
-        'plone.api>=1.8.4',
-        'plone.restapi',
-        'plone.app.dexterity',
+        "z3c.jbot",
+        "plone.api>=1.8.4",
+        "plone.restapi",
+        "plone.app.dexterity",
     ],
     extras_require={
-        'test': [
-            'plone.app.testing',
+        "test": [
+            "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
-            'plone.testing>=5.0.0',
-            'plone.app.contenttypes',
-            'plone.app.robotframework[debug]',
+            "plone.testing>=5.0.0",
+            "plone.app.contenttypes",
+            "plone.app.robotframework[debug]",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = collective.z3cform.jsonwidget.locales.update:update_locale
```

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/configure.zcml` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/index.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/index.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/widget.py` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/browser/widget.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/configure.zcml` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/README.rst` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/manual.pot` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.py` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.sh` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/registry.xml` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/setuphandlers.py` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/testing.py` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/testing.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/test_setup.py` & `collective.z3cform.jsonwidget-1.1.2/src/collective/z3cform/jsonwidget/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO` & `collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.z3cform.jsonwidget
-Version: 1.1.1
+Version: 1.1.2
 Summary: Custom widget to manage complex json data stored into a text field
 Home-page: https://github.com/collective/collective.z3cform.jsonwidget
 Author: Andrea Cecchi
 Author-email: andrea.cecchi85@gmail.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.z3cform.jsonwidget
 Project-URL: Source, https://github.com/collective/collective.z3cform.jsonwidget
@@ -140,14 +140,21 @@
         - Andrea Cecchi, andrea.cecchi85@gmail.com
         
         
         Changelog
         =========
         
         
+        1.1.2 (2023-04-26)
+        ------------------
+        
+        - Fix release.
+          [cekk]
+        
+        
         1.1.1 (2023-04-21)
         ------------------
         
         - Handle integer fields.
           [cekk]
         
         1.1.0 (2022-07-18)
@@ -214,9 +221,9 @@
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7, >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
```

### Comparing `collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt` & `collective.z3cform.jsonwidget-1.1.2/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/webpack.config.js` & `collective.z3cform.jsonwidget-1.1.2/webpack.config.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.1/yarn.lock` & `collective.z3cform.jsonwidget-1.1.2/yarn.lock`

 * *Files identical despite different names*

