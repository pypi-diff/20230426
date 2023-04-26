# Comparing `tmp/adafruit-circuitpython-lsm6ds-4.5.7.tar.gz` & `tmp/adafruit-circuitpython-lsm6ds-4.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lsm6ds-4.5.7.tar", last modified: Mon Nov 28 18:10:30 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-lsm6ds-4.5.8.tar", last modified: Tue Apr 25 22:50:29 2023, max compression
```

## Comparing `adafruit-circuitpython-lsm6ds-4.5.7.tar` & `adafruit-circuitpython-lsm6ds-4.5.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.903739 adafruit-circuitpython-lsm6ds-4.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.891739 adafruit-circuitpython-lsm6ds-4.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.895739 adafruit-circuitpython-lsm6ds-4.5.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.895739 adafruit-circuitpython-lsm6ds-4.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.899739 adafruit-circuitpython-lsm6ds-4.5.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3853 2022-11-28 18:10:30.899739 adafruit-circuitpython-lsm6ds-4.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.899739 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3853 2022-11-28 18:10:30.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2022-11-28 18:10:30.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:10:30.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:10:30.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:10:30.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.899739 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/
--rw-r--r--   0 runner    (1001) docker     (122)    15238 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/ism330dhcx.py
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6ds3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1376 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6ds33.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6ds3trc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2103 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6dso32.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6dsox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.899739 adafruit-circuitpython-lsm6ds-4.5.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.899739 adafruit-circuitpython-lsm6ds-4.5.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      579 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5918 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:30.899739 adafruit-circuitpython-lsm6ds-4.5.7/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1377 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_full_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_ism330dhcx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      553 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6ds33_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      518 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6ds3_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6ds3trc_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      556 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6dso32_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2227 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6dsox_mlc_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      553 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6dsox_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_pedometer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_rate_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2022-11-28 18:10:23.000000 adafruit-circuitpython-lsm6ds-4.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:10:16.000000 adafruit-circuitpython-lsm6ds-4.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:10:30.903739 adafruit-circuitpython-lsm6ds-4.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.094131 adafruit-circuitpython-lsm6ds-4.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.094131 adafruit-circuitpython-lsm6ds-4.5.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/ism330dhcx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3trc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dso32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dsox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_full_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_ism330dhcx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds33_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3trc_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dso32_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_mlc_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_pedometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_rate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/setup.cfg
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lsm6ds-4.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/.gitignore` & `adafruit-circuitpython-lsm6ds-4.5.8/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/.pre-commit-config.yaml` & `adafruit-circuitpython-lsm6ds-4.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/.pylintrc` & `adafruit-circuitpython-lsm6ds-4.5.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lsm6ds-4.5.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/LICENSE` & `adafruit-circuitpython-lsm6ds-4.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/LICENSES/MIT.txt` & `adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/PKG-INFO` & `adafruit-circuitpython-lsm6ds-4.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm6ds
-Version: 4.5.7
+Version: 4.5.8
 Summary: CircuitPython helper library for the LSM6DS family of motion sensors from ST
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS
 Keywords: adafruit,blinka,circuitpython,micropython,lsm6ds,lsm6dsox,lsmds33,lsm6dso32,st,imu,gyro,accelerometer,ism330dhcx,imu,gyro,gyroscope,inemo
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/README.rst` & `adafruit-circuitpython-lsm6ds-4.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm6ds
-Version: 4.5.7
+Version: 4.5.8
 Summary: CircuitPython helper library for the LSM6DS family of motion sensors from ST
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS
 Keywords: adafruit,blinka,circuitpython,micropython,lsm6ds,lsm6dsox,lsmds33,lsm6dso32,st,imu,gyro,accelerometer,ism330dhcx,imu,gyro,gyroscope,inemo
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/__init__.py` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 * Adafruit's Bus Device library:
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
-__version__ = "4.5.7"
+__version__ = "4.5.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS.git"
 
 import struct
 from time import sleep
 from math import radians
 from micropython import const
 from adafruit_bus_device import i2c_device
@@ -111,17 +111,17 @@
         ("RATE_12_5_HZ", 1, 12.5, None),
         ("RATE_26_HZ", 2, 26.0, None),
         ("RATE_52_HZ", 3, 52.0, None),
         ("RATE_104_HZ", 4, 104.0, None),
         ("RATE_208_HZ", 5, 208.0, None),
         ("RATE_416_HZ", 6, 416.0, None),
         ("RATE_833_HZ", 7, 833.0, None),
-        ("RATE_1_66K_HZ", 8, 1066.0, None),
-        ("RATE_3_33K_HZ", 9, 3033.0, None),
-        ("RATE_6_66K_HZ", 10, 6066.0, None),
+        ("RATE_1_66K_HZ", 8, 1666.0, None),
+        ("RATE_3_33K_HZ", 9, 3332.0, None),
+        ("RATE_6_66K_HZ", 10, 6664.0, None),
         ("RATE_1_6_HZ", 11, 1.6, None),
     )
 )
 
 
 class AccelHPF(CV):
     """Options for the accelerometer high pass filter"""
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/ism330dhcx.py` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/ism330dhcx.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6ds3.py` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6ds33.py` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds33.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6ds3trc.py` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3trc.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6dso32.py` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dso32.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/adafruit_lsm6ds/lsm6dsox.py` & `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dsox.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/docs/_static/favicon.ico` & `adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/docs/api.rst` & `adafruit-circuitpython-lsm6ds-4.5.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/docs/conf.py` & `adafruit-circuitpython-lsm6ds-4.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/docs/examples.rst` & `adafruit-circuitpython-lsm6ds-4.5.8/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/docs/index.rst` & `adafruit-circuitpython-lsm6ds-4.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_full_test.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_full_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_ism330dhcx_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_ism330dhcx_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6ds33_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds33_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6ds3_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6ds3trc_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3trc_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6dso32_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dso32_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6dsox_mlc_test.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_mlc_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_lsm6dsox_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_pedometer.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_pedometer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/examples/lsm6ds_rate_test.py` & `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_rate_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.7/pyproject.toml` & `adafruit-circuitpython-lsm6ds-4.5.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-lsm6ds"
 description = "CircuitPython helper library for the LSM6DS family of motion sensors from ST"
-version = "4.5.7"
+version = "4.5.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS"}
 keywords = [
     "adafruit",
```

