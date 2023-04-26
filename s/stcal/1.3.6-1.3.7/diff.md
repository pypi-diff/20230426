# Comparing `tmp/stcal-1.3.6.tar.gz` & `tmp/stcal-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stcal-1.3.6.tar", last modified: Wed Apr 19 18:19:23 2023, max compression
+gzip compressed data, was "stcal-1.3.7.tar", last modified: Wed Apr 26 13:59:59 2023, max compression
```

## Comparing `stcal-1.3.6.tar` & `stcal-1.3.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.778066 stcal-1.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.702065 stcal-1.3.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.702065 stcal-1.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/label_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-19 18:19:13.000000 stcal-1.3.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-19 18:19:13.000000 stcal-1.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-19 18:19:13.000000 stcal-1.3.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-19 18:19:13.000000 stcal-1.3.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-19 18:19:13.000000 stcal-1.3.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-19 18:19:13.000000 stcal-1.3.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-19 18:19:13.000000 stcal-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-19 18:19:23.778066 stcal-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-19 18:19:13.000000 stcal-1.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-19 18:19:13.000000 stcal-1.3.6/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-19 18:19:13.000000 stcal-1.3.6/benchmarks/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/stcal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/jump/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/jump/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/package_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/docs/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/ramp_fitting/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 18:19:13.000000 stcal-1.3.6/docs/stcal/ramp_fitting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-19 18:19:13.000000 stcal-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:19:23.778066 stcal-1.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.702065 stcal-1.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal/dark_current/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dark_current/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dark_current/dark_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dark_current/dark_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/dynamicdq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32158 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/jump/twopoint_difference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.710065 stcal-1.3.6/src/stcal/linearity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/linearity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/linearity/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.710065 stcal-1.3.6/src/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)   127072 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/ols_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/ramp_fitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.710065 stcal-1.3.6/src/stcal/saturation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/saturation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-19 18:19:13.000000 stcal-1.3.6/src/stcal/saturation/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.706065 stcal-1.3.6/src/stcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 18:19:23.000000 stcal-1.3.6/src/stcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:19:22.000000 stcal-1.3.6/src/stcal.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.746065 stcal-1.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/current_gdqfits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:19:23.778066 stcal-1.3.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/data/input_gdq_flarge.fits
--rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/data/large_event_input_dq_cube2.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/data/snowball1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    48432 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_ramp_fitting_gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43187 2023-04-19 18:19:13.000000 stcal-1.3.6/tests/test_twopoint_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-19 18:19:13.000000 stcal-1.3.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.752149 stcal-1.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/label_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-26 13:59:46.000000 stcal-1.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 13:59:46.000000 stcal-1.3.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-04-26 13:59:46.000000 stcal-1.3.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-26 13:59:46.000000 stcal-1.3.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-26 13:59:46.000000 stcal-1.3.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-26 13:59:46.000000 stcal-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-26 13:59:59.748149 stcal-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-26 13:59:46.000000 stcal-1.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-26 13:59:46.000000 stcal-1.3.7/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/docs/stcal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/docs/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/jump/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/jump/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/package_index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/docs/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/ramp_fitting/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/ramp_fitting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-26 13:59:46.000000 stcal-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:59:59.752149 stcal-1.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.668148 stcal-1.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dark_current/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dark_current/dark_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dark_current/dark_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dynamicdq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32158 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/twopoint_difference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/linearity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/linearity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/linearity/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127063 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/ols_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.680148 stcal-1.3.7/src/stcal/saturation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/saturation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/saturation/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:59:58.000000 stcal-1.3.7/src/stcal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.716149 stcal-1.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/current_gdqfits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.748149 stcal-1.3.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/data/input_gdq_flarge.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/data/large_event_input_dq_cube2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/data/snowball1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48431 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_ramp_fitting_gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43187 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_twopoint_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-26 13:59:46.000000 stcal-1.3.7/tox.ini
```

### Comparing `stcal-1.3.6/.github/labeler.yml` & `stcal-1.3.7/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/.github/pull_request_template.md` & `stcal-1.3.7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/.github/workflows/ci.yml` & `stcal-1.3.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/.github/workflows/publish-to-pypi.yml` & `stcal-1.3.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/.gitignore` & `stcal-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/.readthedocs.yaml` & `stcal-1.3.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/CHANGES.rst` & `stcal-1.3.7/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 1.4.0 (unreleased)
 ==================
 
 Bug Fixes
 ---------
 
--
+- 
 
 Changes to API
 --------------
 
-- drop support for Python 3.8 [#162]
+- 
 
 Other
 -----
 
--
+- 
+
+1.3.7 (unreleased)
+==================
+
+Bug Fixes
+---------
+
+ramp_fitting
+~~~~~~~~~~~~
+
+- Correctly compute the number of groups in a segment to properly compute the
+  optimal weights for the OLS ramp fitting algorithm.  Originally, this
+  computation had the potential to include groups not in the segment being
+  computed. [#163]
+
+Changes to API
+--------------
+
+- Drop support for Python 3.8 [#162]
 
 1.3.6 (2023-04-19)
 ==================
 
 Bug Fixes
 ---------
```

### Comparing `stcal-1.3.6/CODE_OF_CONDUCT.md` & `stcal-1.3.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/CONTRIBUTING.md` & `stcal-1.3.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/LICENSE` & `stcal-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/PKG-INFO` & `stcal-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.3.6
+Version: 1.3.7
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.3.6/README.md` & `stcal-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/benchmarks/dark_current.py` & `stcal-1.3.7/benchmarks/dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/benchmarks/linearity.py` & `stcal-1.3.7/benchmarks/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/benchmarks/ramp_fitting.py` & `stcal-1.3.7/benchmarks/ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/benchmarks/saturation.py` & `stcal-1.3.7/benchmarks/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/docs/Makefile` & `stcal-1.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/docs/conf.py` & `stcal-1.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/docs/stcal/jump/description.rst` & `stcal-1.3.7/docs/stcal/jump/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/docs/stcal/ramp_fitting/description.rst` & `stcal-1.3.7/docs/stcal/ramp_fitting/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/pyproject.toml` & `stcal-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/dark_current/dark_class.py` & `stcal-1.3.7/src/stcal/dark_current/dark_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/dark_current/dark_sub.py` & `stcal-1.3.7/src/stcal/dark_current/dark_sub.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/dqflags.py` & `stcal-1.3.7/src/stcal/dqflags.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/jump/jump.py` & `stcal-1.3.7/src/stcal/jump/jump.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/jump/twopoint_difference.py` & `stcal-1.3.7/src/stcal/jump/twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/linearity/linearity.py` & `stcal-1.3.7/src/stcal/linearity/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/ramp_fitting/gls_fit.py` & `stcal-1.3.7/src/stcal/ramp_fitting/gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/ramp_fitting/ols_fit.py` & `stcal-1.3.7/src/stcal/ramp_fitting/ols_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,14 +916,15 @@
     #   each segment are also calculated here.
 
     med_rates = utils.compute_median_rates(ramp_data)
 
     # Loop over data integrations:
     for num_int in range(0, n_int):
         # Loop over data sections
+        ramp_data.current_integ = num_int
         for rlo in range(0, cubeshape[1], nrows):
             rhi = rlo + nrows
 
             if rhi > cubeshape[1]:
                 rhi = cubeshape[1]
 
             # Skip data section if it is all NaNs
@@ -2837,15 +2838,15 @@
 
     c_mask_2d = c_mask_2d[:, good_pix]
     nreads_1d = nreads_1d[good_pix]
 
     if weighting.lower() == 'optimal':  # fit using optimal weighting
         # get sums from optimal weighting
         sumx, sumxx, sumxy, sumy, nreads_wtd, xvalues = calc_opt_sums(
-            rn_sect, gain_sect, data_masked, c_mask_2d, xvalues, good_pix)
+            ramp_data, rn_sect, gain_sect, data_masked, c_mask_2d, xvalues, good_pix)
 
         slope, intercept, sig_slope, sig_intercept = \
             calc_opt_fit(nreads_wtd, sumxx, sumx, sumxy, sumy)
 
         variance = sig_slope**2.  # variance due to fit values
 
     elif weighting.lower() == 'unweighted':  # fit using unweighted weighting
@@ -3496,15 +3497,15 @@
     sumxx = (xvalues**2).sum(axis=0)
     sumy = (np.reshape(data_masked.sum(axis=0), sumx.shape))
     sumxy = (xvalues * np.reshape(data_masked, xvalues.shape)).sum(axis=0)
 
     return sumx, sumxx, sumxy, sumy
 
 
-def calc_opt_sums(rn_sect, gain_sect, data_masked, mask_2d, xvalues, good_pix):
+def calc_opt_sums(ramp_data, rn_sect, gain_sect, data_masked, mask_2d, xvalues, good_pix):
     """
     Calculate the sums needed to determine the slope and intercept (and sigma of
     each) using the optimal weights.  For each good pixel's segment, from the
     initial and final indices and the corresponding number of counts, calculate
     the SNR. From the SNR, calculate the weighting exponent using the formulation
     by Fixsen (Fixsen et al, PASP, 112, 1350). Using this exponent and the gain
     and the readnoise, the weights are calculated from which the sums are
@@ -3567,24 +3568,26 @@
     mask_2d_sum = c_mask_2d.sum(axis=0)   # number of valid groups/pixel
 
     # get final valid group for each pixel for this semiramp
     ind_lastnz = fnz + mask_2d_sum - 1
 
     # get SCI value of initial good group for semiramp
     data_zero = data_masked[fnz, range(data_masked.shape[1])]
+    fnz = 0
 
     # get SCI value of final good group for semiramp
     data_final = data_masked[(ind_lastnz), range(data_masked.shape[1])]
     data_diff = data_final - data_zero  # correctly does *NOT* have nans
 
     ind_lastnz = 0
 
     # Use the readnoise and gain for good pixels only
     rn_sect_rav = rn_sect.flatten()[good_pix]
     rn_2_r = rn_sect_rav * rn_sect_rav
+    rn_sect = 0
 
     gain_sect_r = gain_sect.flatten()[good_pix]
 
     # Calculate the sigma for nonzero gain values
     sigma_ir = data_final.copy() * 0.0
     numer_ir = data_final.copy() * 0.0
 
@@ -3606,32 +3609,26 @@
     del wh_pos
 
     gain_sect_r = 0
     numer_ir = 0
     data_diff = 0
     sigma_ir = 0
 
-    power_wt_r = calc_power(snr)  # Get the interpolated power for this SNR
     # Make array of number of good groups, and exponents for each pixel
-    num_nz = (data_masked != 0.).sum(0)  # number of nonzero groups per pixel
-    nrd_data_a = num_nz.copy()
+    power_wt_r = calc_power(snr)  # Get the interpolated power for this SNR
+    num_nz = c_mask_2d.sum(0)  # number of groups in segment
+    nrd_prime = (num_nz - 1) / 2.
     num_nz = 0
 
-    nrd_prime = (nrd_data_a - 1) / 2.
-    nrd_data_a = 0
-
     # Calculate inverse read noise^2 for use in weights
     # Suppress, then re-enable, harmless arithmetic warning
     warnings.filterwarnings("ignore", ".*divide by zero.*", RuntimeWarning)
     invrdns2_r = 1. / rn_2_r
     warnings.resetwarnings()
 
-    rn_sect = 0
-    fnz = 0
-
     # Set optimal weights for each group of each pixel;
     #    for all pixels at once, loop over the groups
     wt_h = np.zeros(data_masked.shape, dtype=np.float32)
 
     for jj_rd in range(data_masked.shape[0]):
         wt_h[jj_rd, :] = \
             abs((abs(jj_rd - nrd_prime) / nrd_prime) ** power_wt_r) * invrdns2_r
```

### Comparing `stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit.py` & `stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/ramp_fitting/ramp_fit_class.py` & `stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/ramp_fitting/utils.py` & `stcal-1.3.7/src/stcal/ramp_fitting/utils.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal/saturation/saturation.py` & `stcal-1.3.7/src/stcal/saturation/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/src/stcal.egg-info/PKG-INFO` & `stcal-1.3.7/src/stcal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.3.6
+Version: 1.3.7
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.3.6/src/stcal.egg-info/SOURCES.txt` & `stcal-1.3.7/src/stcal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/current_gdqfits` & `stcal-1.3.7/tests/current_gdqfits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/data/input_gdq_flarge.fits` & `stcal-1.3.7/tests/data/input_gdq_flarge.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/data/large_event_input_dq_cube2.fits` & `stcal-1.3.7/tests/data/large_event_input_dq_cube2.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/data/snowball1.fits` & `stcal-1.3.7/tests/data/snowball1.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/test_dark_current.py` & `stcal-1.3.7/tests/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/test_dq.py` & `stcal-1.3.7/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/test_jump.py` & `stcal-1.3.7/tests/test_jump.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/test_linearity.py` & `stcal-1.3.7/tests/test_linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/test_ramp_fitting.py` & `stcal-1.3.7/tests/test_ramp_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1152,15 +1152,15 @@
         ramp, bufsize, save_opt, rnoise, gain, algo,"optimal", ncores, dqflags)
 
     tol = 1.e-5
 
     # Check slopes information
     sdata, sdq, svp, svr, serr = slopes
 
-    check = np.array([[2.797567 , 2.8022935, np.nan]])
+    check = np.array([[2.795187 , 2.795632, np.nan]])
     np.testing.assert_allclose(sdata, check, tol, tol)
 
     check = np.array([[JUMP, JUMP, DNU | SAT]])
     np.testing.assert_allclose(sdq, check, tol, tol)
 
     check = np.array([[0.00033543, 0.00043342, 0.]])
     np.testing.assert_allclose(svp, check, tol, tol)
@@ -1170,16 +1170,16 @@
 
     check = np.array([[0.01847528, 0.02225729, 0.]])
     np.testing.assert_allclose(serr, check, tol, tol)
 
     # Check slopes information
     cdata, cdq, cvp, cvr, cerr = cube
 
-    check = np.array([[[2.7949152, 2.8022935, np.nan]],
-                      [[2.8020892, np.nan, np.nan]]])
+    check = np.array([[[2.7949152, 2.7956316, np.nan]],
+                      [[2.7956493, np.nan, np.nan]]])
     np.testing.assert_allclose(cdata, check, tol, tol)
 
     check = np.array([[[GOOD, JUMP, DNU | SAT]],
                       [[JUMP, DNU | SAT, DNU | SAT]]])
     np.testing.assert_allclose(cdq, check, tol, tol)
 
     check = np.array([[[0.00054729, 0.00043342, 0.]],
```

### Comparing `stcal-1.3.6/tests/test_ramp_fitting_gls_fit.py` & `stcal-1.3.7/tests/test_ramp_fitting_gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/test_saturation.py` & `stcal-1.3.7/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tests/test_twopoint_difference.py` & `stcal-1.3.7/tests/test_twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.6/tox.ini` & `stcal-1.3.7/tox.ini`

 * *Files identical despite different names*

