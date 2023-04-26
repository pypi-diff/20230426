# Comparing `tmp/invenio-alma-0.7.5.tar.gz` & `tmp/invenio-alma-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-alma-0.7.5.tar", last modified: Wed Apr 26 15:28:19 2023, max compression
+gzip compressed data, was "invenio-alma-0.7.6.tar", last modified: Wed Apr 26 16:24:09 2023, max compression
```

## Comparing `invenio-alma-0.7.5.tar` & `invenio-alma-0.7.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.851810 invenio-alma-0.7.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.855810 invenio-alma-0.7.5/invenio_alma/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/click_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.855810 invenio-alma-0.7.5/invenio_alma/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/invenio_alma/services/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.855810 invenio-alma-0.7.5/invenio_alma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/tests/test_invenio_alma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/tests/test_invenio_alma_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.905268 invenio-alma-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-26 16:24:09.905268 invenio-alma-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/click_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-26 16:24:09.905268 invenio-alma-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/tests/test_invenio_alma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/tests/test_invenio_alma_service.py
```

### Comparing `invenio-alma-0.7.5/.editorconfig` & `invenio-alma-0.7.6/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/CHANGES.rst` & `invenio-alma-0.7.6/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.6 (release 2023-04-26)
+
+- fix: remove variable check
+
+
 Version v0.7.5 (release 2023-04-26)
 
 - create: add read permission
 - feature: add item api
 
 
 Version v0.7.4 (release 2023-01-26)
```

### Comparing `invenio-alma-0.7.5/CONTRIBUTING.rst` & `invenio-alma-0.7.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/LICENSE` & `invenio-alma-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/MANIFEST.in` & `invenio-alma-0.7.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/PKG-INFO` & `invenio-alma-0.7.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.7.5
+Version: 0.7.6
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.6 (release 2023-04-26)
+
+- fix: remove variable check
+
+
 Version v0.7.5 (release 2023-04-26)
 
 - create: add read permission
 - feature: add item api
 
 
 Version v0.7.4 (release 2023-01-26)
```

### Comparing `invenio-alma-0.7.5/README.rst` & `invenio-alma-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/docs/Makefile` & `invenio-alma-0.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/docs/conf.py` & `invenio-alma-0.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/docs/index.rst` & `invenio-alma-0.7.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/docs/make.bat` & `invenio-alma-0.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/api.py` & `invenio-alma-0.7.6/invenio_alma/api.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/cli.py` & `invenio-alma-0.7.6/invenio_alma/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/click_param_type.py` & `invenio-alma-0.7.6/invenio_alma/click_param_type.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/config.py` & `invenio-alma-0.7.6/invenio_alma/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/ext.py` & `invenio-alma-0.7.6/invenio_alma/ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,12 +33,11 @@
         self.alma_rest_service = AlmaRESTService.build(api_key, api_host)
 
     def init_resources(self, app):
         """Initialize resources."""
         search_key = "local_control_field_009"  # ac_number
         domain = app.config.get("ALMA_SRU_DOMAIN")
         institution_code = app.config.get("ALMA_SRU_INSTITUTION_CODE")
-        if domain and institution_code:
-            self.alma_resource = AlmaResource(
-                service=AlmaSRUService.build(search_key, domain, institution_code),
-                config=AlmaResourceConfig,
-            )
+        self.alma_resource = AlmaResource(
+            service=AlmaSRUService.build(search_key, domain, institution_code),
+            config=AlmaResourceConfig,
+        )
```

### Comparing `invenio-alma-0.7.5/invenio_alma/resources/config.py` & `invenio-alma-0.7.6/invenio_alma/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/resources/resources.py` & `invenio-alma-0.7.6/invenio_alma/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/services/base.py` & `invenio-alma-0.7.6/invenio_alma/services/base.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/services/config.py` & `invenio-alma-0.7.6/invenio_alma/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/services/errors.py` & `invenio-alma-0.7.6/invenio_alma/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/services/rest.py` & `invenio-alma-0.7.6/invenio_alma/services/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/services/sru.py` & `invenio-alma-0.7.6/invenio_alma/services/sru.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/tasks.py` & `invenio-alma-0.7.6/invenio_alma/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma/utils.py` & `invenio-alma-0.7.6/invenio_alma/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/invenio_alma.egg-info/PKG-INFO` & `invenio-alma-0.7.6/invenio_alma.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.7.5
+Version: 0.7.6
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.6 (release 2023-04-26)
+
+- fix: remove variable check
+
+
 Version v0.7.5 (release 2023-04-26)
 
 - create: add read permission
 - feature: add item api
 
 
 Version v0.7.4 (release 2023-01-26)
```

### Comparing `invenio-alma-0.7.5/invenio_alma.egg-info/SOURCES.txt` & `invenio-alma-0.7.6/invenio_alma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/run-tests.sh` & `invenio-alma-0.7.6/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/setup.cfg` & `invenio-alma-0.7.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/tests/conftest.py` & `invenio-alma-0.7.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/tests/test_invenio_alma.py` & `invenio-alma-0.7.6/tests/test_invenio_alma.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.5/tests/test_invenio_alma_service.py` & `invenio-alma-0.7.6/tests/test_invenio_alma_service.py`

 * *Files identical despite different names*

