# Comparing `tmp/jsonrpc-py-3.0.4.tar.gz` & `tmp/jsonrpc-py-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.4.tar", last modified: Tue Apr 25 08:02:31 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.5.tar", last modified: Wed Apr 26 12:25:48 2023, max compression
```

## Comparing `jsonrpc-py-3.0.4.tar` & `jsonrpc-py-3.0.5.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.054547 jsonrpc-py-3.0.4/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/Makefile
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-25 08:02:31.054547 jsonrpc-py-3.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.032545 jsonrpc-py-3.0.4/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.025544 jsonrpc-py-3.0.4/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.035545 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.043546 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.045546 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1602 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.049546 jsonrpc-py-3.0.4/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5734 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.050547 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-25 08:02:30.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1889 2023-04-25 08:02:31.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 08:02:30.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-25 08:02:30.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 08:02:31.054547 jsonrpc-py-3.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.053547 jsonrpc-py-3.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.470396 jsonrpc-py-3.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-26 12:25:48.469396 jsonrpc-py-3.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.449395 jsonrpc-py-3.0.5/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.442394 jsonrpc-py-3.0.5/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.451395 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.459395 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.461395 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.465396 jsonrpc-py-3.0.5/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9483 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.466396 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:25:48.470396 jsonrpc-py-3.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.469396 jsonrpc-py-3.0.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13819 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.4/.gitlab-ci.yml` & `jsonrpc-py-3.0.5/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -21,49 +21,52 @@
 before_script:
   - python -VV
   - python -m venv --copies .venv
   - source .venv/bin/activate
 
 code quality:
   stage: testing
-  script: make install linting coverage
+  script:
+    - time make install
+    - time make linting
+    - time make coverage
   coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   artifacts:
     name: ${CI_JOB_NAME}-${CI_COMMIT_REF_NAME}-${CI_COMMIT_SHA}
     expire_in: 1 day
     reports:
       junit: pytest.xml
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
 
 build package:
   stage: building
-  script: make build
+  script: time make build
   artifacts:
+    expire_in: 1 day
     paths:
       - dist
-    expire_in: 1 day
   only:
     - tags
 
 deployment:
   stage: publishing
   dependencies:
     - build package
-  script: make release
+  script: time make release
   environment:
     name: PyPI
     url: https://pypi.org/project/jsonrpc-py
   only:
     - tags
 
 pages:
   stage: publishing
-  script: make docs
+  script: time make docs
   environment:
     name: GitLab Pages
     url: https://docs.jsonrpc.ru
   artifacts:
     paths:
       - public
     expire_in: 1 day
```

### Comparing `jsonrpc-py-3.0.4/LICENSE` & `jsonrpc-py-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/Makefile` & `jsonrpc-py-3.0.5/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .PHONY: all help install build release docs isort black mypy flake8 linting test coverage clean
 
 all: install clean
 
 help: ## Display this help screen
-	@grep -E '^[a-z.A-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-15s\033[0m %s\n", $$1, $$2}'
+	@grep -E '^[a-zA-Z0-9_]+:.*?## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-15s\033[0m %s\n", $$1, $$2}'
 
 install: ## Install a dependencies for development
 	@pip install --requirement requirements-dev.txt --upgrade
 
 build: ## Build a package
 	@python -m build --sdist
```

### Comparing `jsonrpc-py-3.0.4/PKG-INFO` & `jsonrpc-py-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.4
+Version: 3.0.5
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.4/README.md` & `jsonrpc-py-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/changelog.rst` & `jsonrpc-py-3.0.5/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/conf.py` & `jsonrpc-py-3.0.5/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 # A list of strings that are module names of extensions:
 extensions: Final[tuple[str, ...]] = (
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
 )
 
 # Highlighting of the code blocks:
-pygments_style: Final[str] = "trac"
+pygments_style: Final[str] = "stata-light"
 
 # This variable is Furo-specific at this time:
-pygments_dark_style: Final[str] = "monokai"
+pygments_dark_style: Final[str] = "stata-dark"
 
 # Options for HTML Output
 # -----------------------
 
 # The "theme" that the HTML output should use:
 html_theme: Final[str] = "furo"
```

### Comparing `jsonrpc-py-3.0.4/docs/deployment.rst` & `jsonrpc-py-3.0.5/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/index.rst` & `jsonrpc-py-3.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/quickstart.rst` & `jsonrpc-py-3.0.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/docs/reference.rst` & `jsonrpc-py-3.0.5/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc/__init__.py` & `jsonrpc-py-3.0.5/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc/asgi.py` & `jsonrpc-py-3.0.5/jsonrpc/asgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from asyncio import CancelledError, Task, create_task, gather, wait_for
 from collections import UserDict
 from collections.abc import Generator, MutableSequence
 from http import HTTPMethod, HTTPStatus
 from io import DEFAULT_BUFFER_SIZE, BytesIO
 from typing import Any, ClassVar, Final, TypeAlias
 
@@ -14,14 +15,21 @@
 
 __all__: Final[tuple[str, ...]] = ("ASGIHandler",)
 
 AnyTask: TypeAlias = Task[Any]
 AnyRequest: TypeAlias = Request | Error | BatchRequest
 AnyResponse: TypeAlias = Response | BatchResponse | None
 
+#: ---
+#: Ensure that "Content-Type" is a valid JSON header.
+JSON_CTYPE_REGEXB: Final[re.Pattern[bytes]] = re.compile(
+    rb"(?:application/|[\w.-]+/[\w.+-]+?\+)json$",
+    flags=re.IGNORECASE,
+)
+
 
 class RequestAborted(Exception):
     """
     The request was closed before it was completed, or timed out.
     """
 
 
@@ -52,17 +60,19 @@
     ) -> None:
         self.scope: Final[HTTPConnectionScope] = scope
         self.receive: Final[ASGIReceiveCallable] = receive
         self.send: Final[ASGISendCallable] = send
         self.app: type[ASGIHandler] = app
 
     def __await__(self) -> Generator[Any, None, None]:
-        return self.dispatch().__await__()
+        #: ---
+        #: Create a suitable iterator by calling __await__ on a coroutine.
+        return self.__await_impl__().__await__()
 
-    async def dispatch(self) -> None:
+    async def __await_impl__(self) -> None:
         try:
             #: ---
             #: Might be "405 Method Not Allowed" or "415 Unsupported Media Type".
             self.negotiate_content()
 
             #: ---
             #: Might be "400 Bad Request" or abort.
@@ -89,15 +99,15 @@
         except (TimeoutError, CancelledError):
             await self.send_response(status=HTTPStatus.GATEWAY_TIMEOUT)
 
     def negotiate_content(self) -> None:
         if self.scope["method"] != HTTPMethod.POST:
             raise HTTPException(status=HTTPStatus.METHOD_NOT_ALLOWED)
         for key, value in self.scope["headers"]:
-            if key == b"content-type" and not value.startswith(self.app.content_type.encode("ascii")):
+            if key == b"content-type" and not JSON_CTYPE_REGEXB.match(value):
                 raise HTTPException(status=HTTPStatus.UNSUPPORTED_MEDIA_TYPE)
 
     async def read_request_body(self) -> bytes:
         with BytesIO() as raw_buffer:
             while True:
                 match await self.receive():
                     case {"type": "http.request", **kwargs}:
```

### Comparing `jsonrpc-py-3.0.4/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.5/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc/errors.py` & `jsonrpc-py-3.0.5/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc/request.py` & `jsonrpc-py-3.0.5/jsonrpc/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+import re
 from collections import UserList
 from collections.abc import Iterable, MutableMapping, MutableSequence
 from dataclasses import dataclass
 from numbers import Number
-from re import match as regex_match
 from typing import Any, Final, Self
 
 from .errors import Error, ErrorEnum
 from .utilities import Undefined, UndefinedType, make_hashable
 
 __all__: Final[tuple[str, ...]] = (
     "BatchRequest",
     "Request",
 )
 
+#: ---
+#: Method names that begin with the word rpc followed by a
+#: period character (U+002E or ASCII 46) are reserved for
+#: rpc-internal methods and extensions and MUST NOT be used
+#: for anything else.
+INTERNAL_METHOD_REGEX: Final[re.Pattern[str]] = re.compile(r"^rpc\.", flags=re.IGNORECASE)
+
 
 @dataclass(kw_only=True, slots=True)
 class Request:
     """
     Base JSON-RPC request object.
     """
 
@@ -35,15 +42,15 @@
         self._validate_params()
         self._validate_request_id()
 
     def __hash__(self) -> int:
         return hash((self.method, make_hashable(self.params), self.request_id))
 
     def _validate_method(self) -> None:
-        if not isinstance(self.method, str) or regex_match("\x5e\x72\x70\x63\x5c\x2e", self.method):
+        if not isinstance(self.method, str) or INTERNAL_METHOD_REGEX.match(self.method):
             raise Error(
                 code=ErrorEnum.INVALID_REQUEST,
                 message="Request method must be a string and should not have a 'rpc.' prefix",
             )
 
     def _validate_params(self) -> None:
         if not isinstance(self.params, MutableSequence | MutableMapping | UndefinedType):
```

### Comparing `jsonrpc-py-3.0.4/jsonrpc/response.py` & `jsonrpc-py-3.0.5/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc/serializer.py` & `jsonrpc-py-3.0.5/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.5/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc/utilities.py` & `jsonrpc-py-3.0.5/jsonrpc/utilities.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.5/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.4
+Version: 3.0.5
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.4/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.5/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 docs/changelog/v2.x.x/v2.5.1.rst
 docs/changelog/v3.x.x/index.rst
 docs/changelog/v3.x.x/v3.0.0.rst
 docs/changelog/v3.x.x/v3.0.1.rst
 docs/changelog/v3.x.x/v3.0.2.rst
 docs/changelog/v3.x.x/v3.0.3.rst
 docs/changelog/v3.x.x/v3.0.4.rst
+docs/changelog/v3.x.x/v3.0.5.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
```

### Comparing `jsonrpc-py-3.0.4/pyproject.toml` & `jsonrpc-py-3.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/tests/test_asgi.py` & `jsonrpc-py-3.0.5/tests/test_asgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     async def asyncSetUp(self) -> None:
         await self.enterAsyncContext(self.client)
 
     async def test_negotiate_content_405(self) -> None:
         for request in (
             self.client.build_request(HTTPMethod.HEAD, "/testHead"),
             self.client.build_request(HTTPMethod.GET, "/testGet"),
-            self.client.build_request(HTTPMethod.PATCH, "/testPatch", content=b""),
-            self.client.build_request(HTTPMethod.DELETE, "/testDelete", content=b""),
+            self.client.build_request(HTTPMethod.PATCH, "/testPatch"),
+            self.client.build_request(HTTPMethod.DELETE, "/testDelete"),
             self.client.build_request(HTTPMethod.OPTIONS, "/testOptions"),
             self.client.build_request(HTTPMethod.TRACE, "/testTrace"),
         ):
             with self.subTest(request=request):
                 response: Response = await self.client.send(request)
                 self.assertEqual(response.status_code, HTTPStatus.METHOD_NOT_ALLOWED)
                 self.assertEqual(response.headers["Allow"], HTTPMethod.POST)
```

### Comparing `jsonrpc-py-3.0.4/tests/test_dispatcher.py` & `jsonrpc-py-3.0.5/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/tests/test_errors.py` & `jsonrpc-py-3.0.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/tests/test_request.py` & `jsonrpc-py-3.0.5/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/tests/test_response.py` & `jsonrpc-py-3.0.5/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/tests/test_serializer.py` & `jsonrpc-py-3.0.5/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.4/tests/test_utilities.py` & `jsonrpc-py-3.0.5/tests/test_utilities.py`

 * *Files identical despite different names*

