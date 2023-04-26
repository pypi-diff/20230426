# Comparing `tmp/pytest-remote-response-2.1.1.tar.gz` & `tmp/pytest-remote-response-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-remote-response-2.1.1.tar", last modified: Fri Apr 21 01:14:26 2023, max compression
+gzip compressed data, was "pytest-remote-response-2.1.2.tar", last modified: Wed Apr 26 13:49:43 2023, max compression
```

## Comparing `pytest-remote-response-2.1.1.tar` & `pytest-remote-response-2.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.805803 pytest-remote-response-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-21 01:14:26.805803 pytest-remote-response-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.801802 pytest-remote-response-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/2.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.801802 pytest-remote-response-2.1.1/docs/code_ref/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/code_ref/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/how_it_works.rst
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/docs/why.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.801802 pytest-remote-response-2.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/examples/block_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/examples/capture_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/examples/insert_get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/examples/response_decorator_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/examples/response_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.801802 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_remote_response.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.801802 pytest-remote-response-2.1.1/pytest_response/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 01:14:26.000000 pytest-remote-response-2.1.1/pytest_response/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.801802 pytest-remote-response-2.1.1/pytest_response/interceptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/interceptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/interceptors/_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/interceptors/_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/interceptors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/interceptors/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/interceptors/urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/interceptors/urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/pytest_response/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-21 01:14:26.805803 pytest-remote-response-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:26.805803 pytest-remote-response-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tests/test_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-21 01:14:06.000000 pytest-remote-response-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/docs/code_ref/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/code_ref/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/how_it_works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/docs/why.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/examples/block_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/examples/capture_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/examples/insert_get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/examples/response_decorator_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/examples/response_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-26 13:49:42.000000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 13:49:43.000000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:49:42.000000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 13:49:42.000000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:49:42.000000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 13:49:42.000000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 13:49:42.000000 pytest-remote-response-2.1.2/pytest_remote_response.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/pytest_response/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 13:49:42.000000 pytest-remote-response-2.1.2/pytest_response/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/pytest_response/interceptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/interceptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/interceptors/_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/interceptors/_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/interceptors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/interceptors/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/interceptors/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/interceptors/urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/pytest_response/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-26 13:49:43.362000 pytest-remote-response-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:43.358000 pytest-remote-response-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tests/test_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-26 13:49:29.000000 pytest-remote-response-2.1.2/tox.ini
```

### Comparing `pytest-remote-response-2.1.1/LICENSE` & `pytest-remote-response-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/PKG-INFO` & `pytest-remote-response-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-remote-response
-Version: 2.1.1
+Version: 2.1.2
 Summary: Pytest plugin for capturing and mocking connection requests.
 Home-page: https://github.com/devanshshukla99/pytest-remote-response
 Author: devanshshukla99
 Author-email: devanshshukla99@outlook.com
 License: MIT
 Description: ======================
         pytest-remote-response
@@ -152,15 +152,15 @@
             :target: https://pypi.org/project/pytest-remote-response/
             :alt: Package stability
         
         .. |versions| image:: https://img.shields.io/pypi/pyversions/pytest-remote-response.svg?logo=python&logoColor=FBE072
             :target: https://pypi.org/project/pytest-remote-response/
             :alt: Python versions supported
         
-        .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg 
+        .. |license| image:: https://img.shields.io/pypi/l/pytest-remote-response 
             :target: https://pypi.org/project/pytest-remote-response/
             :alt: License
         
         .. |codestyle| image:: https://img.shields.io/badge/code%20style-black-000000.svg
            :target: https://github.com/psf/black
         
         .. |docs| image:: https://readthedocs.org/projects/pytest-remote-response/badge/?version=latest
```

### Comparing `pytest-remote-response-2.1.1/README.rst` & `pytest-remote-response-2.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     :target: https://pypi.org/project/pytest-remote-response/
     :alt: Package stability
 
 .. |versions| image:: https://img.shields.io/pypi/pyversions/pytest-remote-response.svg?logo=python&logoColor=FBE072
     :target: https://pypi.org/project/pytest-remote-response/
     :alt: Python versions supported
 
-.. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg 
+.. |license| image:: https://img.shields.io/pypi/l/pytest-remote-response 
     :target: https://pypi.org/project/pytest-remote-response/
     :alt: License
 
 .. |codestyle| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |docs| image:: https://readthedocs.org/projects/pytest-remote-response/badge/?version=latest
```

### Comparing `pytest-remote-response-2.1.1/docs/1.0.rst` & `pytest-remote-response-2.1.2/docs/1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/2.0.rst` & `pytest-remote-response-2.1.2/docs/2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/Makefile` & `pytest-remote-response-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/code_ref/index.rst` & `pytest-remote-response-2.1.2/docs/code_ref/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/conf.py` & `pytest-remote-response-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/how_it_works.rst` & `pytest-remote-response-2.1.2/docs/how_it_works.rst`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/index.rst` & `pytest-remote-response-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/make.bat` & `pytest-remote-response-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/user_guide.rst` & `pytest-remote-response-2.1.2/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/docs/why.rst` & `pytest-remote-response-2.1.2/docs/why.rst`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/examples/block_urllib.py` & `pytest-remote-response-2.1.2/examples/block_urllib.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/examples/capture_requests.py` & `pytest-remote-response-2.1.2/examples/capture_requests.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/examples/insert_get_database.py` & `pytest-remote-response-2.1.2/examples/insert_get_database.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/examples/response_decorator_urllib3.py` & `pytest-remote-response-2.1.2/examples/response_decorator_urllib3.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/examples/response_urllib3.py` & `pytest-remote-response-2.1.2/examples/response_urllib3.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pyproject.toml` & `pytest-remote-response-2.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [build-system]
 requires = [
-         "setuptools",
          "setuptools_scm",
          "wheel"
          ]
-build-backend = 'setuptools.build_meta'
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
+write_to = "pytest_response/_version.py"
 
 [tool.black]
 line-length = 110
 
 [tool.towncrier]
     package = "pytest_response"
     filename = "CHANGELOG.rst"
```

### Comparing `pytest-remote-response-2.1.1/pytest_remote_response.egg-info/PKG-INFO` & `pytest-remote-response-2.1.2/pytest_remote_response.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-remote-response
-Version: 2.1.1
+Version: 2.1.2
 Summary: Pytest plugin for capturing and mocking connection requests.
 Home-page: https://github.com/devanshshukla99/pytest-remote-response
 Author: devanshshukla99
 Author-email: devanshshukla99@outlook.com
 License: MIT
 Description: ======================
         pytest-remote-response
@@ -152,15 +152,15 @@
             :target: https://pypi.org/project/pytest-remote-response/
             :alt: Package stability
         
         .. |versions| image:: https://img.shields.io/pypi/pyversions/pytest-remote-response.svg?logo=python&logoColor=FBE072
             :target: https://pypi.org/project/pytest-remote-response/
             :alt: Python versions supported
         
-        .. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg 
+        .. |license| image:: https://img.shields.io/pypi/l/pytest-remote-response 
             :target: https://pypi.org/project/pytest-remote-response/
             :alt: License
         
         .. |codestyle| image:: https://img.shields.io/badge/code%20style-black-000000.svg
            :target: https://github.com/psf/black
         
         .. |docs| image:: https://readthedocs.org/projects/pytest-remote-response/badge/?version=latest
```

### Comparing `pytest-remote-response-2.1.1/pytest_remote_response.egg-info/SOURCES.txt` & `pytest-remote-response-2.1.2/pytest_remote_response.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/app.py` & `pytest-remote-response-2.1.2/pytest_response/app.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/database.py` & `pytest-remote-response-2.1.2/pytest_response/database.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/exceptions.py` & `pytest-remote-response-2.1.2/pytest_response/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/interceptors/_urllib.py` & `pytest-remote-response-2.1.2/pytest_response/interceptors/_urllib.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/interceptors/_urllib3.py` & `pytest-remote-response-2.1.2/pytest_response/interceptors/_urllib3.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/interceptors/aiohttp.py` & `pytest-remote-response-2.1.2/pytest_response/interceptors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/interceptors/requests.py` & `pytest-remote-response-2.1.2/pytest_response/interceptors/requests.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/interceptors/urllib.py` & `pytest-remote-response-2.1.2/pytest_response/interceptors/urllib.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/interceptors/urllib3.py` & `pytest-remote-response-2.1.2/pytest_response/interceptors/urllib3.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/logger.py` & `pytest-remote-response-2.1.2/pytest_response/logger.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/pytest_response/plugin.py` & `pytest-remote-response-2.1.2/pytest_response/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/setup.cfg` & `pytest-remote-response-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tests/test_aiohttp.py` & `pytest-remote-response-2.1.2/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tests/test_app.py` & `pytest-remote-response-2.1.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tests/test_database.py` & `pytest-remote-response-2.1.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tests/test_examples.py` & `pytest-remote-response-2.1.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tests/test_requests.py` & `pytest-remote-response-2.1.2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tests/test_urllib.py` & `pytest-remote-response-2.1.2/tests/test_urllib.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tests/test_urllib3.py` & `pytest-remote-response-2.1.2/tests/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `pytest-remote-response-2.1.1/tox.ini` & `pytest-remote-response-2.1.2/tox.ini`

 * *Files identical despite different names*

