# Comparing `tmp/hunter-3.6.0.tar.gz` & `tmp/hunter-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hunter-3.6.0.tar", last modified: Tue Apr 25 11:59:53 2023, max compression
+gzip compressed data, was "hunter-3.6.1.tar", last modified: Wed Apr 26 09:56:30 2023, max compression
```

## Comparing `hunter-3.6.0.tar` & `hunter-3.6.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.761536 hunter-3.6.0/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      654 2023-04-25 07:35:29.000000 hunter-3.6.0/.bumpversion.cfg
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1706 2023-04-24 11:28:35.000000 hunter-3.6.0/.cookiecutterrc
--rw-r--r--   0 ionel     (1000) ionel     (1000)      119 2023-04-24 09:46:45.000000 hunter-3.6.0/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2023-04-24 09:43:01.000000 hunter-3.6.0/.editorconfig
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.736536 hunter-3.6.0/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.739536 hunter-3.6.0/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)    32405 2023-04-24 11:28:35.000000 hunter-3.6.0/.github/workflows/github-actions.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      786 2023-04-24 11:28:35.000000 hunter-3.6.0/.gitignore
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1027 2023-04-24 11:28:35.000000 hunter-3.6.0/.pre-commit-config.yaml
--rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2022-10-28 12:27:32.000000 hunter-3.6.0/.python-version
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      231 2023-04-24 09:43:01.000000 hunter-3.6.0/.readthedocs.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      256 2023-04-24 09:46:45.000000 hunter-3.6.0/AUTHORS.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)    21724 2023-04-25 07:33:58.000000 hunter-3.6.0/CHANGELOG.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2341 2023-04-24 11:28:35.000000 hunter-3.6.0/CONTRIBUTING.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2023-04-24 11:28:35.000000 hunter-3.6.0/LICENSE
--rw-r--r--   0 ionel     (1000) ionel     (1000)    39977 2023-04-25 11:59:53.761536 hunter-3.6.0/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)    18784 2023-04-25 07:35:29.000000 hunter-3.6.0/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.739536 hunter-3.6.0/build_backend/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      144 2023-04-25 05:29:45.000000 hunter-3.6.0/build_backend/backend.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.739536 hunter-3.6.0/ci/
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2861 2023-04-24 11:28:35.000000 hunter-3.6.0/ci/bootstrap.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)       72 2023-04-24 09:46:45.000000 hunter-3.6.0/ci/requirements.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.737536 hunter-3.6.0/ci/templates/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.737536 hunter-3.6.0/ci/templates/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.739536 hunter-3.6.0/ci/templates/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     4037 2023-04-24 11:28:35.000000 hunter-3.6.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.741536 hunter-3.6.0/docs/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2023-04-24 09:43:01.000000 hunter-3.6.0/docs/authors.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2023-04-24 09:43:01.000000 hunter-3.6.0/docs/changelog.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    31085 2021-03-24 11:38:24.000000 hunter-3.6.0/docs/code-trace.png
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1514 2023-04-25 07:35:29.000000 hunter-3.6.0/docs/conf.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1100 2022-10-28 12:27:32.000000 hunter-3.6.0/docs/configuration.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2023-04-24 09:43:01.000000 hunter-3.6.0/docs/contributing.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)    16005 2022-10-28 12:27:32.000000 hunter-3.6.0/docs/cookbook.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3801 2022-10-28 12:27:32.000000 hunter-3.6.0/docs/filtering.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      297 2023-04-24 09:46:45.000000 hunter-3.6.0/docs/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       86 2023-04-24 09:43:01.000000 hunter-3.6.0/docs/installation.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     4208 2021-03-24 11:38:24.000000 hunter-3.6.0/docs/introduction.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2023-04-24 09:43:01.000000 hunter-3.6.0/docs/readme.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     5012 2022-10-28 12:27:32.000000 hunter-3.6.0/docs/reference.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1340 2022-10-28 12:27:32.000000 hunter-3.6.0/docs/remote.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)       48 2023-04-24 09:46:45.000000 hunter-3.6.0/docs/requirements.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    28581 2021-03-24 11:38:24.000000 hunter-3.6.0/docs/simple-trace.png
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2023-04-24 09:43:01.000000 hunter-3.6.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    11793 2018-11-08 02:40:37.000000 hunter-3.6.0/docs/tree-trace.png
--rw-rw-r--   0 ionel     (1000) ionel     (1000)    51251 2021-03-24 11:38:24.000000 hunter-3.6.0/docs/vars-trace.png
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1412 2023-04-25 05:26:11.000000 hunter-3.6.0/pyproject.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      916 2023-04-24 09:46:45.000000 hunter-3.6.0/pytest.ini
--rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2023-04-25 11:59:53.761536 hunter-3.6.0/setup.cfg
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     6490 2023-04-25 07:35:29.000000 hunter-3.6.0/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.742536 hunter-3.6.0/src/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.754536 hunter-3.6.0/src/hunter/
--rw-r--r--   0 ionel     (1000) ionel     (1000)    18383 2023-04-25 07:35:29.000000 hunter-3.6.0/src/hunter/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)   788614 2023-04-25 05:55:37.000000 hunter-3.6.0/src/hunter/_event.c
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1488 2023-04-24 11:28:35.000000 hunter-3.6.0/src/hunter/_event.pxd
--rw-r--r--   0 ionel     (1000) ionel     (1000)    15009 2023-04-24 14:41:11.000000 hunter-3.6.0/src/hunter/_event.pyx
--rw-r--r--   0 ionel     (1000) ionel     (1000)  1618683 2023-04-25 05:55:37.000000 hunter-3.6.0/src/hunter/_predicates.c
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1620 2023-04-24 11:28:35.000000 hunter-3.6.0/src/hunter/_predicates.pxd
--rw-r--r--   0 ionel     (1000) ionel     (1000)    24587 2023-04-25 04:25:41.000000 hunter-3.6.0/src/hunter/_predicates.pyx
--rw-r--r--   0 ionel     (1000) ionel     (1000)   478304 2023-04-25 05:55:37.000000 hunter-3.6.0/src/hunter/_tracer.c
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2023-04-24 11:28:35.000000 hunter-3.6.0/src/hunter/_tracer.pxd
--rw-r--r--   0 ionel     (1000) ionel     (1000)     5026 2023-04-24 13:32:00.000000 hunter-3.6.0/src/hunter/_tracer.pyx
--rw-r--r--   0 ionel     (1000) ionel     (1000)      176 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter/_version.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    32658 2023-04-24 13:56:33.000000 hunter-3.6.0/src/hunter/actions.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      506 2023-04-24 11:28:35.000000 hunter-3.6.0/src/hunter/config.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1310 2023-04-24 00:41:08.000000 hunter-3.6.0/src/hunter/const.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    14494 2023-04-24 14:29:30.000000 hunter-3.6.0/src/hunter/event.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    29272 2023-04-24 14:15:25.000000 hunter-3.6.0/src/hunter/predicates.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     6156 2023-04-24 13:42:13.000000 hunter-3.6.0/src/hunter/remote.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     4839 2023-04-24 13:40:10.000000 hunter-3.6.0/src/hunter/tracer.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7970 2023-04-24 15:02:07.000000 hunter-3.6.0/src/hunter/util.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.755536 hunter-3.6.0/src/hunter/vendor/
--rw-r--r--   0 ionel     (1000) ionel     (1000)        0 2022-10-28 12:27:32.000000 hunter-3.6.0/src/hunter/vendor/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    16063 2023-04-24 13:39:43.000000 hunter-3.6.0/src/hunter/vendor/_compat.h
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.757536 hunter-3.6.0/src/hunter/vendor/_cymem/
--rw-r--r--   0 ionel     (1000) ionel     (1000)        0 2022-10-28 12:27:32.000000 hunter-3.6.0/src/hunter/vendor/_cymem/__init__.pxd
--rw-r--r--   0 ionel     (1000) ionel     (1000)       21 2022-10-28 12:27:32.000000 hunter-3.6.0/src/hunter/vendor/_cymem/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      232 2023-04-24 00:45:28.000000 hunter-3.6.0/src/hunter/vendor/_cymem/about.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)   490603 2023-04-25 05:55:37.000000 hunter-3.6.0/src/hunter/vendor/_cymem/cymem.c
--rw-r--r--   0 ionel     (1000) ionel     (1000)      809 2022-10-28 12:27:32.000000 hunter-3.6.0/src/hunter/vendor/_cymem/cymem.pxd
--rw-r--r--   0 ionel     (1000) ionel     (1000)     5612 2022-10-28 12:27:32.000000 hunter-3.6.0/src/hunter/vendor/_cymem/cymem.pyx
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.759536 hunter-3.6.0/src/hunter/vendor/colorama/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      239 2023-04-24 00:45:28.000000 hunter-3.6.0/src/hunter/vendor/colorama/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2522 2023-04-24 00:45:28.000000 hunter-3.6.0/src/hunter/vendor/colorama/ansi.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    10517 2023-04-24 00:45:28.000000 hunter-3.6.0/src/hunter/vendor/colorama/ansitowin32.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1915 2023-04-24 00:45:28.000000 hunter-3.6.0/src/hunter/vendor/colorama/initialise.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     5404 2023-04-24 00:45:28.000000 hunter-3.6.0/src/hunter/vendor/colorama/win32.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     6438 2023-04-24 00:45:28.000000 hunter-3.6.0/src/hunter/vendor/colorama/winterm.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.755536 hunter-3.6.0/src/hunter.egg-info/
--rw-r--r--   0 ionel     (1000) ionel     (1000)    39977 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter.egg-info/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2398 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter.egg-info/SOURCES.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter.egg-info/dependency_links.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       52 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter.egg-info/entry_points.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter.egg-info/not-zip-safe
--rw-r--r--   0 ionel     (1000) ionel     (1000)       46 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter.egg-info/requires.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2023-04-25 11:59:53.000000 hunter-3.6.0/src/hunter.egg-info/top_level.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       47 2022-10-28 12:27:32.000000 hunter-3.6.0/src/hunter.pth
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-25 11:59:53.761536 hunter-3.6.0/tests/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      310 2023-04-24 00:41:08.000000 hunter-3.6.0/tests/conftest.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      475 2023-04-24 11:28:35.000000 hunter-3.6.0/tests/eviltracer.pxd
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1140 2023-04-24 11:28:35.000000 hunter-3.6.0/tests/eviltracer.pyx
--rw-r--r--   0 ionel     (1000) ionel     (1000)      138 2023-04-24 00:41:08.000000 hunter-3.6.0/tests/sample.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      518 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/sample2.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      247 2022-10-28 12:27:32.000000 hunter-3.6.0/tests/sample3.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       14 2018-11-08 02:40:37.000000 hunter-3.6.0/tests/sample4.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      102 2022-10-28 12:27:32.000000 hunter-3.6.0/tests/sample5.pyx
--rw-r--r--   0 ionel     (1000) ionel     (1000)      168 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/sample6.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      415 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/sample7.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1185 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/sample7args.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      648 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/sample8errors.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      211 2023-04-24 00:41:08.000000 hunter-3.6.0/tests/samplemanhole.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1062 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/samplepdb.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1210 2023-04-24 11:28:35.000000 hunter-3.6.0/tests/setup.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      327 2023-04-24 11:28:35.000000 hunter-3.6.0/tests/simple.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3125 2023-04-24 00:41:08.000000 hunter-3.6.0/tests/test_config.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     6557 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/test_cookbook.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    37557 2023-04-25 04:32:50.000000 hunter-3.6.0/tests/test_integration.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    15584 2023-04-24 11:28:35.000000 hunter-3.6.0/tests/test_predicates.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     5070 2023-04-24 11:28:35.000000 hunter-3.6.0/tests/test_remote.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    57014 2023-04-25 04:33:05.000000 hunter-3.6.0/tests/test_tracer.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     8038 2023-04-24 15:02:07.000000 hunter-3.6.0/tests/test_util.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      615 2023-04-24 01:23:08.000000 hunter-3.6.0/tests/utils.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2851 2023-04-25 05:55:47.000000 hunter-3.6.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.057405 hunter-3.6.1/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      654 2023-04-26 09:11:54.000000 hunter-3.6.1/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1706 2023-04-24 11:28:35.000000 hunter-3.6.1/.cookiecutterrc
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      119 2023-04-24 09:46:45.000000 hunter-3.6.1/.coveragerc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2023-04-24 09:43:01.000000 hunter-3.6.1/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.045405 hunter-3.6.1/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.047405 hunter-3.6.1/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    32405 2023-04-24 11:28:35.000000 hunter-3.6.1/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      786 2023-04-24 11:28:35.000000 hunter-3.6.1/.gitignore
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1027 2023-04-24 11:28:35.000000 hunter-3.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2022-10-28 12:27:32.000000 hunter-3.6.1/.python-version
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      231 2023-04-24 09:43:01.000000 hunter-3.6.1/.readthedocs.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      256 2023-04-24 09:46:45.000000 hunter-3.6.1/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    21811 2023-04-26 09:08:53.000000 hunter-3.6.1/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2341 2023-04-24 11:28:35.000000 hunter-3.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2023-04-24 11:28:35.000000 hunter-3.6.1/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    40064 2023-04-26 09:56:30.057405 hunter-3.6.1/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    18784 2023-04-26 09:11:54.000000 hunter-3.6.1/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.047405 hunter-3.6.1/build_backend/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      144 2023-04-25 05:29:45.000000 hunter-3.6.1/build_backend/backend.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.047405 hunter-3.6.1/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2861 2023-04-24 11:28:35.000000 hunter-3.6.1/ci/bootstrap.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       72 2023-04-24 09:46:45.000000 hunter-3.6.1/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.045405 hunter-3.6.1/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.045405 hunter-3.6.1/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.047405 hunter-3.6.1/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     4037 2023-04-24 11:28:35.000000 hunter-3.6.1/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.049405 hunter-3.6.1/docs/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2023-04-24 09:43:01.000000 hunter-3.6.1/docs/authors.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2023-04-24 09:43:01.000000 hunter-3.6.1/docs/changelog.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)    31085 2021-03-24 11:38:24.000000 hunter-3.6.1/docs/code-trace.png
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1514 2023-04-26 09:11:54.000000 hunter-3.6.1/docs/conf.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1100 2022-10-28 12:27:32.000000 hunter-3.6.1/docs/configuration.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2023-04-24 09:43:01.000000 hunter-3.6.1/docs/contributing.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    16005 2022-10-28 12:27:32.000000 hunter-3.6.1/docs/cookbook.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3801 2022-10-28 12:27:32.000000 hunter-3.6.1/docs/filtering.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      297 2023-04-24 09:46:45.000000 hunter-3.6.1/docs/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       86 2023-04-24 09:43:01.000000 hunter-3.6.1/docs/installation.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     4208 2021-03-24 11:38:24.000000 hunter-3.6.1/docs/introduction.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2023-04-24 09:43:01.000000 hunter-3.6.1/docs/readme.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5012 2022-10-28 12:27:32.000000 hunter-3.6.1/docs/reference.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1340 2022-10-28 12:27:32.000000 hunter-3.6.1/docs/remote.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       48 2023-04-24 09:46:45.000000 hunter-3.6.1/docs/requirements.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)    28581 2021-03-24 11:38:24.000000 hunter-3.6.1/docs/simple-trace.png
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2023-04-24 09:43:01.000000 hunter-3.6.1/docs/spelling_wordlist.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)    11793 2018-11-08 02:40:37.000000 hunter-3.6.1/docs/tree-trace.png
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)    51251 2021-03-24 11:38:24.000000 hunter-3.6.1/docs/vars-trace.png
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1412 2023-04-25 05:26:11.000000 hunter-3.6.1/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      916 2023-04-24 09:46:45.000000 hunter-3.6.1/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2023-04-26 09:56:30.057405 hunter-3.6.1/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     6490 2023-04-26 09:11:54.000000 hunter-3.6.1/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.050405 hunter-3.6.1/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.053405 hunter-3.6.1/src/hunter/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    18383 2023-04-26 09:11:54.000000 hunter-3.6.1/src/hunter/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)   788614 2023-04-25 20:01:55.000000 hunter-3.6.1/src/hunter/_event.c
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1488 2023-04-24 11:28:35.000000 hunter-3.6.1/src/hunter/_event.pxd
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    15009 2023-04-24 14:41:11.000000 hunter-3.6.1/src/hunter/_event.pyx
+-rw-r--r--   0 ionel     (1000) ionel     (1000)  1618683 2023-04-25 20:01:55.000000 hunter-3.6.1/src/hunter/_predicates.c
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1620 2023-04-24 11:28:35.000000 hunter-3.6.1/src/hunter/_predicates.pxd
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    24587 2023-04-25 04:25:41.000000 hunter-3.6.1/src/hunter/_predicates.pyx
+-rw-r--r--   0 ionel     (1000) ionel     (1000)   478304 2023-04-25 20:01:55.000000 hunter-3.6.1/src/hunter/_tracer.c
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2023-04-24 11:28:35.000000 hunter-3.6.1/src/hunter/_tracer.pxd
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5026 2023-04-24 13:32:00.000000 hunter-3.6.1/src/hunter/_tracer.pyx
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      176 2023-04-26 09:56:29.000000 hunter-3.6.1/src/hunter/_version.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    32658 2023-04-24 13:56:33.000000 hunter-3.6.1/src/hunter/actions.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      506 2023-04-24 11:28:35.000000 hunter-3.6.1/src/hunter/config.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1310 2023-04-24 00:41:08.000000 hunter-3.6.1/src/hunter/const.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    14494 2023-04-24 14:29:30.000000 hunter-3.6.1/src/hunter/event.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    29272 2023-04-24 14:15:25.000000 hunter-3.6.1/src/hunter/predicates.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     6156 2023-04-24 13:42:13.000000 hunter-3.6.1/src/hunter/remote.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     4839 2023-04-24 13:40:10.000000 hunter-3.6.1/src/hunter/tracer.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7981 2023-04-25 13:35:27.000000 hunter-3.6.1/src/hunter/util.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.054405 hunter-3.6.1/src/hunter/vendor/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        0 2022-10-28 12:27:32.000000 hunter-3.6.1/src/hunter/vendor/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    16063 2023-04-24 13:39:43.000000 hunter-3.6.1/src/hunter/vendor/_compat.h
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.054405 hunter-3.6.1/src/hunter/vendor/_cymem/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        0 2022-10-28 12:27:32.000000 hunter-3.6.1/src/hunter/vendor/_cymem/__init__.pxd
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       21 2022-10-28 12:27:32.000000 hunter-3.6.1/src/hunter/vendor/_cymem/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      232 2023-04-24 00:45:28.000000 hunter-3.6.1/src/hunter/vendor/_cymem/about.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)   490603 2023-04-25 20:01:55.000000 hunter-3.6.1/src/hunter/vendor/_cymem/cymem.c
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      809 2022-10-28 12:27:32.000000 hunter-3.6.1/src/hunter/vendor/_cymem/cymem.pxd
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5612 2022-10-28 12:27:32.000000 hunter-3.6.1/src/hunter/vendor/_cymem/cymem.pyx
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.055405 hunter-3.6.1/src/hunter/vendor/colorama/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      239 2023-04-24 00:45:28.000000 hunter-3.6.1/src/hunter/vendor/colorama/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2522 2023-04-24 00:45:28.000000 hunter-3.6.1/src/hunter/vendor/colorama/ansi.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    10517 2023-04-24 00:45:28.000000 hunter-3.6.1/src/hunter/vendor/colorama/ansitowin32.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1915 2023-04-24 00:45:28.000000 hunter-3.6.1/src/hunter/vendor/colorama/initialise.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5404 2023-04-24 00:45:28.000000 hunter-3.6.1/src/hunter/vendor/colorama/win32.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     6438 2023-04-24 00:45:28.000000 hunter-3.6.1/src/hunter/vendor/colorama/winterm.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.054405 hunter-3.6.1/src/hunter.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    40064 2023-04-26 09:56:29.000000 hunter-3.6.1/src/hunter.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2398 2023-04-26 09:56:30.000000 hunter-3.6.1/src/hunter.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-04-26 09:56:29.000000 hunter-3.6.1/src/hunter.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       52 2023-04-26 09:56:29.000000 hunter-3.6.1/src/hunter.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-04-26 09:56:29.000000 hunter-3.6.1/src/hunter.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       46 2023-04-26 09:56:29.000000 hunter-3.6.1/src/hunter.egg-info/requires.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2023-04-26 09:56:29.000000 hunter-3.6.1/src/hunter.egg-info/top_level.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       47 2022-10-28 12:27:32.000000 hunter-3.6.1/src/hunter.pth
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-04-26 09:56:30.057405 hunter-3.6.1/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      310 2023-04-24 00:41:08.000000 hunter-3.6.1/tests/conftest.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      475 2023-04-24 11:28:35.000000 hunter-3.6.1/tests/eviltracer.pxd
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1140 2023-04-24 11:28:35.000000 hunter-3.6.1/tests/eviltracer.pyx
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      138 2023-04-24 00:41:08.000000 hunter-3.6.1/tests/sample.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      518 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/sample2.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      247 2022-10-28 12:27:32.000000 hunter-3.6.1/tests/sample3.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       14 2018-11-08 02:40:37.000000 hunter-3.6.1/tests/sample4.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      102 2022-10-28 12:27:32.000000 hunter-3.6.1/tests/sample5.pyx
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      168 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/sample6.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      415 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/sample7.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1185 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/sample7args.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      648 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/sample8errors.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      211 2023-04-24 00:41:08.000000 hunter-3.6.1/tests/samplemanhole.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1062 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/samplepdb.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1210 2023-04-24 11:28:35.000000 hunter-3.6.1/tests/setup.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      327 2023-04-24 11:28:35.000000 hunter-3.6.1/tests/simple.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3125 2023-04-24 00:41:08.000000 hunter-3.6.1/tests/test_config.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     6557 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/test_cookbook.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    37557 2023-04-25 04:32:50.000000 hunter-3.6.1/tests/test_integration.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    15584 2023-04-24 11:28:35.000000 hunter-3.6.1/tests/test_predicates.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5070 2023-04-24 11:28:35.000000 hunter-3.6.1/tests/test_remote.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    57014 2023-04-25 04:33:05.000000 hunter-3.6.1/tests/test_tracer.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     8135 2023-04-25 13:39:12.000000 hunter-3.6.1/tests/test_util.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      615 2023-04-24 01:23:08.000000 hunter-3.6.1/tests/utils.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2851 2023-04-25 20:01:55.000000 hunter-3.6.1/tox.ini
```

### Comparing `hunter-3.6.0/.bumpversion.cfg` & `hunter-3.6.1/.bumpversion.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.6.0
+current_version = 3.6.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = 'fallback_version': '{current_version}'
 replace = 'fallback_version': '{new_version}'
```

### Comparing `hunter-3.6.0/.cookiecutterrc` & `hunter-3.6.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/.github/workflows/github-actions.yml` & `hunter-3.6.1/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/.gitignore` & `hunter-3.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/.pre-commit-config.yaml` & `hunter-3.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/CHANGELOG.rst` & `hunter-3.6.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 
 Changelog
 =========
 
+3.6.1 (2023-04-26)
+------------------
+
+* Added safe repr support for Decimal objects.
+
 3.6.0 (2023-04-25)
 ------------------
 
 * Added C extension support for Python 3.11. This may come with up to 10% performance hit (depending on use-case) for all Pythons.
   Unfortunately some `compat shims <https://raw.githubusercontent.com/python/pythoncapi_compat/master/pythoncapi_compat.h>`_ are
   now used for getting frame details. This is necessary to be able to work with Python 3.11 and be more future-proof.
 * Added safe repr support for ZoneInfo objects.
```

### Comparing `hunter-3.6.0/CONTRIBUTING.rst` & `hunter-3.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/LICENSE` & `hunter-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/PKG-INFO` & `hunter-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hunter
-Version: 3.6.0
+Version: 3.6.1
 Summary: Hunter is a flexible code tracing toolkit.
 Home-page: https://github.com/ionelmc/python-hunter
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-hunter.readthedocs.io/
 Project-URL: Changelog, https://python-hunter.readthedocs.io/en/latest/changelog.html
@@ -456,14 +456,19 @@
 
 More projects using it at https://github.com/ionelmc/python-hunter/network/dependents
 
 
 Changelog
 =========
 
+3.6.1 (2023-04-26)
+------------------
+
+* Added safe repr support for Decimal objects.
+
 3.6.0 (2023-04-25)
 ------------------
 
 * Added C extension support for Python 3.11. This may come with up to 10% performance hit (depending on use-case) for all Pythons.
   Unfortunately some `compat shims <https://raw.githubusercontent.com/python/pythoncapi_compat/master/pythoncapi_compat.h>`_ are
   now used for getting frame details. This is necessary to be able to work with Python 3.11 and be more future-proof.
 * Added safe repr support for ZoneInfo objects.
```

### Comparing `hunter-3.6.0/README.rst` & `hunter-3.6.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/hunter
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/hunter.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/hunter
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-hunter/v3.6.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-hunter/v3.6.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/ionelmc/python-hunter/compare/v3.6.0...master
+    :target: https://github.com/ionelmc/python-hunter/compare/v3.6.1...master
 
 
 
 .. end-badges
 
 Hunter is a flexible code tracing toolkit, not for measuring coverage, but for debugging, logging, inspection and other
 nefarious purposes. It has a `simple Python API <https://python-hunter.readthedocs.io/en/latest/introduction.html>`_,
```

### Comparing `hunter-3.6.0/ci/bootstrap.py` & `hunter-3.6.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/ci/templates/.github/workflows/github-actions.yml` & `hunter-3.6.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/code-trace.png` & `hunter-3.6.1/docs/code-trace.png`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/conf.py` & `hunter-3.6.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 copyright = f'{year}, {author}'
 try:
     from pkg_resources import get_distribution
 
     version = release = get_distribution('hunter').version
 except Exception:
     traceback.print_exc()
-    version = release = '3.6.0'
+    version = release = '3.6.1'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/ionelmc/python-hunter/issues/%s', '#'),
     'pr': ('https://github.com/ionelmc/python-hunter/pull/%s', 'PR #'),
 }
```

### Comparing `hunter-3.6.0/docs/configuration.rst` & `hunter-3.6.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/cookbook.rst` & `hunter-3.6.1/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/filtering.rst` & `hunter-3.6.1/docs/filtering.rst`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/introduction.rst` & `hunter-3.6.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/reference.rst` & `hunter-3.6.1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/remote.rst` & `hunter-3.6.1/docs/remote.rst`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/simple-trace.png` & `hunter-3.6.1/docs/simple-trace.png`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/tree-trace.png` & `hunter-3.6.1/docs/tree-trace.png`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/docs/vars-trace.png` & `hunter-3.6.1/docs/vars-trace.png`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/pyproject.toml` & `hunter-3.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/pytest.ini` & `hunter-3.6.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/setup.py` & `hunter-3.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 
 setup(
     name='hunter',
     use_scm_version={
         'local_scheme': 'dirty-tag',
         'write_to': 'src/hunter/_version.py',
-        'fallback_version': '3.6.0',
+        'fallback_version': '3.6.1',
     },
     license='BSD-2-Clause',
     description='Hunter is a flexible code tracing toolkit.',
     long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
```

### Comparing `hunter-3.6.0/src/hunter/__init__.py` & `hunter-3.6.1/src/hunter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     from .predicates import Query
     from .predicates import When
     from .tracer import Tracer
 
 try:
     from ._version import version as __version__
 except ImportError:
-    __version__ = '3.6.0'
+    __version__ = '3.6.1'
 
 __all__ = (
     'And',
     'Backlog',
     'CallPrinter',
     'CodePrinter',
     'Debugger',
```

### Comparing `hunter-3.6.0/src/hunter/_event.c` & `hunter-3.6.1/src/hunter/_event.c`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_event.pxd` & `hunter-3.6.1/src/hunter/_event.pxd`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_event.pyx` & `hunter-3.6.1/src/hunter/_event.pyx`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_predicates.c` & `hunter-3.6.1/src/hunter/_predicates.c`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_predicates.pxd` & `hunter-3.6.1/src/hunter/_predicates.pxd`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_predicates.pyx` & `hunter-3.6.1/src/hunter/_predicates.pyx`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_tracer.c` & `hunter-3.6.1/src/hunter/_tracer.c`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_tracer.pxd` & `hunter-3.6.1/src/hunter/_tracer.pxd`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/_tracer.pyx` & `hunter-3.6.1/src/hunter/_tracer.pyx`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/actions.py` & `hunter-3.6.1/src/hunter/actions.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/const.py` & `hunter-3.6.1/src/hunter/const.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/event.py` & `hunter-3.6.1/src/hunter/event.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/predicates.py` & `hunter-3.6.1/src/hunter/predicates.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/remote.py` & `hunter-3.6.1/src/hunter/remote.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/tracer.py` & `hunter-3.6.1/src/hunter/tracer.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/util.py` & `hunter-3.6.1/src/hunter/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             name = obj.__name__
         return f'<{"un" if self is None else ""}bound method {name} of {safe_repr(self, newdepth)}>'
     elif obj_type_type is type and BaseException in obj_type.__mro__:
         return f'{obj_type.__name__}({", ".join(safe_repr(i, newdepth) for i in obj.args)})'
     elif (
         obj_type_type is type
         and obj_type is not InstanceType
-        and obj_type.__module__ in (builtins.__name__, 'io', 'socket', '_socket', 'zoneinfo')
+        and obj_type.__module__ in (builtins.__name__, 'io', 'socket', '_socket', 'zoneinfo', 'decimal')
     ):
         # hardcoded list of safe things. note that isinstance ain't used
         # (we don't trust subclasses to do the right thing in __repr__)
         return repr(obj)
     else:
         # if the object has a __dict__ then it's probably an instance of a pure python class, assume bad things
         #  with side-effects will be going on in __repr__ - use the default instead (object.__repr__)
```

### Comparing `hunter-3.6.0/src/hunter/vendor/_compat.h` & `hunter-3.6.1/src/hunter/vendor/_compat.h`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/_cymem/cymem.c` & `hunter-3.6.1/src/hunter/vendor/_cymem/cymem.c`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/_cymem/cymem.pxd` & `hunter-3.6.1/src/hunter/vendor/_cymem/cymem.pxd`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/_cymem/cymem.pyx` & `hunter-3.6.1/src/hunter/vendor/_cymem/cymem.pyx`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/colorama/ansi.py` & `hunter-3.6.1/src/hunter/vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/colorama/ansitowin32.py` & `hunter-3.6.1/src/hunter/vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/colorama/initialise.py` & `hunter-3.6.1/src/hunter/vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/colorama/win32.py` & `hunter-3.6.1/src/hunter/vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter/vendor/colorama/winterm.py` & `hunter-3.6.1/src/hunter/vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/src/hunter.egg-info/PKG-INFO` & `hunter-3.6.1/src/hunter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hunter
-Version: 3.6.0
+Version: 3.6.1
 Summary: Hunter is a flexible code tracing toolkit.
 Home-page: https://github.com/ionelmc/python-hunter
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-hunter.readthedocs.io/
 Project-URL: Changelog, https://python-hunter.readthedocs.io/en/latest/changelog.html
@@ -456,14 +456,19 @@
 
 More projects using it at https://github.com/ionelmc/python-hunter/network/dependents
 
 
 Changelog
 =========
 
+3.6.1 (2023-04-26)
+------------------
+
+* Added safe repr support for Decimal objects.
+
 3.6.0 (2023-04-25)
 ------------------
 
 * Added C extension support for Python 3.11. This may come with up to 10% performance hit (depending on use-case) for all Pythons.
   Unfortunately some `compat shims <https://raw.githubusercontent.com/python/pythoncapi_compat/master/pythoncapi_compat.h>`_ are
   now used for getting frame details. This is necessary to be able to work with Python 3.11 and be more future-proof.
 * Added safe repr support for ZoneInfo objects.
```

### Comparing `hunter-3.6.0/src/hunter.egg-info/SOURCES.txt` & `hunter-3.6.1/src/hunter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/eviltracer.pyx` & `hunter-3.6.1/tests/eviltracer.pyx`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/sample2.py` & `hunter-3.6.1/tests/sample2.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/sample7args.py` & `hunter-3.6.1/tests/sample7args.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/sample8errors.py` & `hunter-3.6.1/tests/sample8errors.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/samplepdb.py` & `hunter-3.6.1/tests/samplepdb.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/setup.py` & `hunter-3.6.1/tests/setup.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/test_config.py` & `hunter-3.6.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/test_cookbook.py` & `hunter-3.6.1/tests/test_cookbook.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/test_integration.py` & `hunter-3.6.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/test_predicates.py` & `hunter-3.6.1/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/test_remote.py` & `hunter-3.6.1/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/test_tracer.py` & `hunter-3.6.1/tests/test_tracer.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tests/test_util.py` & `hunter-3.6.1/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,18 @@
     zoneinfo = pytest.importorskip("zoneinfo")
     assert (
         safe_repr(datetime(2000, 2, 2, tzinfo=zoneinfo.ZoneInfo('Europe/Bucharest')))
         == "datetime(2000, 2, 2, 0, 0, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Bucharest'), fold=0)"
     )
 
 
+def test_safe_repr_decimal():
+    assert safe_repr(Decimal('1.23456')) == "Decimal('1.23456')"
+
+
 def test_reliable_primitives():
     # establish a baseline for primitives that cannot be messed with descriptors and metaclasses
     side_effects = []
 
     class MetaMeta(type):
         @property
         def __mro__(self):
```

### Comparing `hunter-3.6.0/tests/utils.py` & `hunter-3.6.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hunter-3.6.0/tox.ini` & `hunter-3.6.1/tox.ini`

 * *Files identical despite different names*

