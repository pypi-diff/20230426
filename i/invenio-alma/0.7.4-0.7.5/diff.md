# Comparing `tmp/invenio-alma-0.7.4.tar.gz` & `tmp/invenio-alma-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-alma-0.7.4.tar", last modified: Thu Jan 26 21:47:27 2023, max compression
+gzip compressed data, was "invenio-alma-0.7.5.tar", last modified: Wed Apr 26 15:28:19 2023, max compression
```

## Comparing `invenio-alma-0.7.4.tar` & `invenio-alma-0.7.5.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/invenio_alma/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/click_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/invenio_alma/services/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/services/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/services/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/invenio_alma/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/invenio_alma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-01-26 21:47:27.000000 invenio-alma-0.7.4/invenio_alma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-26 21:47:27.000000 invenio-alma-0.7.4/invenio_alma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 21:47:27.000000 invenio-alma-0.7.4/invenio_alma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-26 21:47:27.000000 invenio-alma-0.7.4/invenio_alma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 21:47:27.000000 invenio-alma-0.7.4/invenio_alma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-26 21:47:27.000000 invenio-alma-0.7.4/invenio_alma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-26 21:47:27.000000 invenio-alma-0.7.4/invenio_alma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:47:27.733244 invenio-alma-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/tests/test_invenio_alma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-01-26 21:47:23.000000 invenio-alma-0.7.4/tests/test_invenio_alma_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.851810 invenio-alma-0.7.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.855810 invenio-alma-0.7.5/invenio_alma/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/click_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.855810 invenio-alma-0.7.5/invenio_alma/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/invenio_alma/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/invenio_alma/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.855810 invenio-alma-0.7.5/invenio_alma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 15:28:19.000000 invenio-alma-0.7.5/invenio_alma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:28:19.859810 invenio-alma-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/tests/test_invenio_alma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 15:28:07.000000 invenio-alma-0.7.5/tests/test_invenio_alma_service.py
```

### Comparing `invenio-alma-0.7.4/.editorconfig` & `invenio-alma-0.7.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/CHANGES.rst` & `invenio-alma-0.7.5/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.5 (release 2023-04-26)
+
+- create: add read permission
+- feature: add item api
+
+
 Version v0.7.4 (release 2023-01-26)
 
 - fix: handle read timeout
 
 
 Version v0.7.3 (release 2023-01-26)
```

### Comparing `invenio-alma-0.7.4/CONTRIBUTING.rst` & `invenio-alma-0.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/LICENSE` & `invenio-alma-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/MANIFEST.in` & `invenio-alma-0.7.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/PKG-INFO` & `invenio-alma-0.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.7.4
+Version: 0.7.5
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.5 (release 2023-04-26)
+
+- create: add read permission
+- feature: add item api
+
+
 Version v0.7.4 (release 2023-01-26)
 
 - fix: handle read timeout
 
 
 Version v0.7.3 (release 2023-01-26)
```

### Comparing `invenio-alma-0.7.4/README.rst` & `invenio-alma-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/docs/Makefile` & `invenio-alma-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/docs/conf.py` & `invenio-alma-0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/docs/index.rst` & `invenio-alma-0.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/docs/make.bat` & `invenio-alma-0.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/api.py` & `invenio-alma-0.7.5/invenio_alma/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """API functions of the alma connector."""
 
 from csv import DictReader
 from time import sleep
 
 from flask import current_app
 from flask_principal import Identity
+from invenio_access.permissions import system_process
 from invenio_records_marc21 import (
     DuplicateRecordError,
     Marc21Metadata,
     Marc21RecordService,
     MarcDraftProvider,
     check_about_duplicate,
     convert_json_to_marc21xml,
@@ -38,14 +39,15 @@
     cms_id: str = "",
 ) -> None:
     """Create a record in alma.
 
     Normally - depending on the API_KEY - the record will be created in
     the Institution Zone (IZ).
     """
+    identity.provides.add(system_process)
     record = records_service.read_draft(identity, marc_id)
     marc21_record_etree = convert_json_to_marc21xml(record.to_dict()["metadata"])
 
     if is_duplicate_in_alma(cms_id):
         return
 
     try:
```

### Comparing `invenio-alma-0.7.4/invenio_alma/cli.py` & `invenio-alma-0.7.5/invenio_alma/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/click_param_type.py` & `invenio-alma-0.7.5/invenio_alma/click_param_type.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/config.py` & `invenio-alma-0.7.5/invenio_alma/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/services/base.py` & `invenio-alma-0.7.5/invenio_alma/services/base.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/services/config.py` & `invenio-alma-0.7.5/invenio_alma/services/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 class AlmaRESTConfig:
     """Alma service configuration class."""
 
     api_key: str = ""
     api_host: str = ""
 
 
-@dataclass(frozen=True)
+@dataclass
 class AlmaSRUConfig:
     """Alma sru service config."""
 
     search_key: str = ""
     domain: str = ""
     institution_code: str = ""
```

### Comparing `invenio-alma-0.7.4/invenio_alma/services/errors.py` & `invenio-alma-0.7.5/invenio_alma/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/services/rest.py` & `invenio-alma-0.7.5/invenio_alma/services/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/services/sru.py` & `invenio-alma-0.7.5/invenio_alma/services/sru.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/tasks.py` & `invenio-alma-0.7.5/invenio_alma/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma/utils.py` & `invenio-alma-0.7.5/invenio_alma/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/invenio_alma.egg-info/PKG-INFO` & `invenio-alma-0.7.5/invenio_alma.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.7.4
+Version: 0.7.5
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.5 (release 2023-04-26)
+
+- create: add read permission
+- feature: add item api
+
+
 Version v0.7.4 (release 2023-01-26)
 
 - fix: handle read timeout
 
 
 Version v0.7.3 (release 2023-01-26)
```

### Comparing `invenio-alma-0.7.4/invenio_alma.egg-info/SOURCES.txt` & `invenio-alma-0.7.5/invenio_alma.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -29,21 +29,25 @@
 invenio_alma/cli.py
 invenio_alma/click_param_type.py
 invenio_alma/config.py
 invenio_alma/ext.py
 invenio_alma/proxies.py
 invenio_alma/tasks.py
 invenio_alma/utils.py
+invenio_alma/views.py
 invenio_alma.egg-info/PKG-INFO
 invenio_alma.egg-info/SOURCES.txt
 invenio_alma.egg-info/dependency_links.txt
 invenio_alma.egg-info/entry_points.txt
 invenio_alma.egg-info/not-zip-safe
 invenio_alma.egg-info/requires.txt
 invenio_alma.egg-info/top_level.txt
+invenio_alma/resources/__init__.py
+invenio_alma/resources/config.py
+invenio_alma/resources/resources.py
 invenio_alma/services/__init__.py
 invenio_alma/services/base.py
 invenio_alma/services/config.py
 invenio_alma/services/errors.py
 invenio_alma/services/rest.py
 invenio_alma/services/sru.py
 invenio_alma/services/utils.py
```

### Comparing `invenio-alma-0.7.4/run-tests.sh` & `invenio-alma-0.7.5/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/setup.cfg` & `invenio-alma-0.7.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 [options.entry_points]
 flask.commands = 
 	alma = invenio_alma.cli:alma
 console_scripts = 
 	alma = invenio_alma.cli:alma
 invenio_base.apps = 
 	invenio_alma = invenio_alma:InvenioAlma
+invenio_base.api_apps = 
+	invenio_alma = invenio_alma:InvenioAlma
+invenio_base.api_blueprints = 
+	invenio_alma_records = invenio_alma.views:create_record_bp
 invenio_celery.tasks = 
 	invenio_alma = invenio_alma.tasks
 
 [aliases]
 test = pytest
 
 [build_sphinx]
```

### Comparing `invenio-alma-0.7.4/tests/conftest.py` & `invenio-alma-0.7.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/tests/test_invenio_alma.py` & `invenio-alma-0.7.5/tests/test_invenio_alma.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.4/tests/test_invenio_alma_service.py` & `invenio-alma-0.7.5/tests/test_invenio_alma_service.py`

 * *Files identical despite different names*

