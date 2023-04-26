# Comparing `tmp/invenio-workflows-tugraz-0.1.7.tar.gz` & `tmp/invenio-workflows-tugraz-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-workflows-tugraz-0.1.7.tar", last modified: Thu Jan 26 08:48:08 2023, max compression
+gzip compressed data, was "invenio-workflows-tugraz-0.1.8.tar", last modified: Tue Apr 25 21:13:08 2023, max compression
```

## Comparing `invenio-workflows-tugraz-0.1.7.tar` & `invenio-workflows-tugraz-0.1.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.370847 invenio-workflows-tugraz-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.370847 invenio-workflows-tugraz-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/data/
--rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/data/iso6393.json
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/theses.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-26 08:48:08.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-26 08:48:08.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 08:48:08.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-26 08:48:08.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 08:48:08.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-26 08:48:08.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-26 08:48:08.000000 invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-26 08:48:08.378847 invenio-workflows-tugraz-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 08:48:08.374847 invenio-workflows-tugraz-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-26 08:48:03.000000 invenio-workflows-tugraz-0.1.7/tests/test_invenio_workflows_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.615503 invenio-workflows-tugraz-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.615503 invenio-workflows-tugraz-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.615503 invenio-workflows-tugraz-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/data/iso6393.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/theses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/tests/test_invenio_workflows_tugraz.py
```

### Comparing `invenio-workflows-tugraz-0.1.7/.editorconfig` & `invenio-workflows-tugraz-0.1.8/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/.github/workflows/tests.yml` & `invenio-workflows-tugraz-0.1.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/CHANGES.rst` & `invenio-workflows-tugraz-0.1.8/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.8 (release 2023-04-25)
+
+- theses: add necessary need to import
+
+
 Version v0.1.7 (release 2023-01-26)
 
 - theses: change alma import size
 - theses: change import start date
 
 
 Version v0.1.6 (release 2023-01-23)
```

### Comparing `invenio-workflows-tugraz-0.1.7/CONTRIBUTING.rst` & `invenio-workflows-tugraz-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/LICENSE` & `invenio-workflows-tugraz-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/MANIFEST.in` & `invenio-workflows-tugraz-0.1.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/PKG-INFO` & `invenio-workflows-tugraz-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.1.7
+Version: 0.1.8
 Summary: "This package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
@@ -26,14 +26,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.8 (release 2023-04-25)
+
+- theses: add necessary need to import
+
+
 Version v0.1.7 (release 2023-01-26)
 
 - theses: change alma import size
 - theses: change import start date
 
 
 Version v0.1.6 (release 2023-01-23)
```

### Comparing `invenio-workflows-tugraz-0.1.7/babel.ini` & `invenio-workflows-tugraz-0.1.8/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/docs/Makefile` & `invenio-workflows-tugraz-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/docs/conf.py` & `invenio-workflows-tugraz-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/docs/index.rst` & `invenio-workflows-tugraz-0.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/docs/make.bat` & `invenio-workflows-tugraz-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/config.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/data/iso6393.json` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/data/iso6393.json`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/ext.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/convert.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/convert.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/utils.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/openaccess/workflow.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/workflow.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/__init__.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/convert.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/convert.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/decorators.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/theses.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/theses.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 """Theses Workflows."""
 
 from collections import namedtuple
 from typing import Callable
 from xml.etree.ElementTree import Element
 
+from invenio_access.permissions import system_process
 from invenio_campusonline.types import (
     CampusOnlineConfigs,
     CampusOnlineID,
     ThesesFilter,
     ThesesState,
 )
 from invenio_config_tugraz import get_identity_from_user_by_email
@@ -161,14 +162,15 @@
 
     marc21_record = Marc21Metadata()
     convert = CampusOnlineToMarc21(marc21_record)
 
     convert.visit(thesis, marc21_record)
 
     identity = get_identity_from_user_by_email(email=configs.user_email)
+    identity.provides.add(system_process)
     service = current_records_marc21.records_service
     data = marc21_record.json
     data["access"] = {
         "record": "restricted",
         "files": "restricted",
     }
```

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz/theses/views.py` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/views.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/PKG-INFO` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.1.7
+Version: 0.1.8
 Summary: "This package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
@@ -26,14 +26,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.8 (release 2023-04-25)
+
+- theses: add necessary need to import
+
+
 Version v0.1.7 (release 2023-01-26)
 
 - theses: change alma import size
 - theses: change import start date
 
 
 Version v0.1.6 (release 2023-01-23)
```

### Comparing `invenio-workflows-tugraz-0.1.7/invenio_workflows_tugraz.egg-info/SOURCES.txt` & `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/setup.cfg` & `invenio-workflows-tugraz-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/tests/conftest.py` & `invenio-workflows-tugraz-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.7/tests/test_invenio_workflows_tugraz.py` & `invenio-workflows-tugraz-0.1.8/tests/test_invenio_workflows_tugraz.py`

 * *Files identical despite different names*

