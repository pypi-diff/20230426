# Comparing `tmp/climate_categories-0.7.1.tar.gz` & `tmp/climate_categories-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_categories-0.7.1.tar", last modified: Thu Nov 25 15:30:23 2021, max compression
+gzip compressed data, was "climate_categories-0.8.1.tar", last modified: Wed Apr 26 14:03:08 2023, max compression
```

## Comparing `climate_categories-0.7.1.tar` & `climate_categories-0.8.1.tar`

### file list

```diff
@@ -1,121 +1,134 @@
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.085100 climate_categories-0.7.1/
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.077100 climate_categories-0.7.1/.github/
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.077100 climate_categories-0.7.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      671 2021-03-09 10:15:39.000000 climate_categories-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      548 2021-03-09 10:20:59.000000 climate_categories-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      571 2021-03-09 10:20:19.000000 climate_categories-0.7.1/.github/ISSUE_TEMPLATE/new_categorization.md
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      375 2021-10-22 15:48:52.000000 climate_categories-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.077100 climate_categories-0.7.1/.github/workflows/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      964 2021-10-22 15:49:34.000000 climate_categories-0.7.1/.github/workflows/ci.yml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1283 2021-10-22 15:48:52.000000 climate_categories-0.7.1/.gitignore
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1277 2021-11-25 15:00:43.000000 climate_categories-0.7.1/.pre-commit-config.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      122 2021-01-06 18:41:35.000000 climate_categories-0.7.1/.readthedocs.yml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       38 2021-10-22 15:21:16.000000 climate_categories-0.7.1/.sourcery.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      210 2021-11-25 15:26:53.000000 climate_categories-0.7.1/AUTHORS.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     4050 2021-11-25 15:29:35.000000 climate_categories-0.7.1/CHANGELOG.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5450 2021-11-25 15:26:53.000000 climate_categories-0.7.1/CONTRIBUTING.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      651 2021-10-22 15:48:52.000000 climate_categories-0.7.1/LICENSE
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3052 2021-11-25 14:08:41.000000 climate_categories-0.7.1/Makefile
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8012 2021-11-25 15:30:23.085100 climate_categories-0.7.1/PKG-INFO
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2932 2021-11-25 15:30:08.000000 climate_categories-0.7.1/README.rst
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.077100 climate_categories-0.7.1/climate_categories/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2038 2021-11-25 15:26:57.000000 climate_categories-0.7.1/climate_categories/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    41525 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/_categories.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    46871 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/_conversions.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.081100 climate_categories-0.7.1/climate_categories/data/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    48820 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/BURDI.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    39603 2021-11-18 14:07:37.000000 climate_categories-0.7.1/climate_categories/data/BURDI.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    91320 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/BURDI_class.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    64321 2021-11-18 14:07:54.000000 climate_categories-0.7.1/climate_categories/data/BURDI_class.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    84030 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/CRF1999.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    69834 2021-11-18 14:04:06.000000 climate_categories-0.7.1/climate_categories/data/CRF1999.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    85443 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/CRFDI.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    68686 2021-11-18 14:04:40.000000 climate_categories-0.7.1/climate_categories/data/CRFDI.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)   252079 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/CRFDI_class.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)   172924 2021-11-18 14:05:36.000000 climate_categories-0.7.1/climate_categories/data/CRFDI_class.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2039 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/GCB.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1795 2021-10-22 15:48:52.000000 climate_categories-0.7.1/climate_categories/data/GCB.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    60150 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/IPCC1996.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    51928 2021-11-18 14:03:52.000000 climate_categories-0.7.1/climate_categories/data/IPCC1996.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)   146256 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/IPCC2006.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)   126862 2021-11-18 14:02:36.000000 climate_categories-0.7.1/climate_categories/data/IPCC2006.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)   149225 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/IPCC2006_PRIMAP.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)   128959 2021-11-18 14:03:08.000000 climate_categories-0.7.1/climate_categories/data/IPCC2006_PRIMAP.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    24805 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/RCMIP.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    18551 2021-11-18 14:02:19.000000 climate_categories-0.7.1/climate_categories/data/RCMIP.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3761 2021-11-25 15:20:07.000000 climate_categories-0.7.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    32498 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/data/gas.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    23635 2021-11-18 14:04:30.000000 climate_categories-0.7.1/climate_categories/data/gas.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      353 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/search.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.081100 climate_categories-0.7.1/climate_categories/tests/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       48 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3782 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/conftest.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.081100 climate_categories-0.7.1/climate_categories/tests/data/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/data/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      359 2021-11-25 15:20:07.000000 climate_categories-0.7.1/climate_categories/tests/data/broken_conversion_not_allowed.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      359 2021-11-25 15:20:07.000000 climate_categories-0.7.1/climate_categories/tests/data/broken_conversion_not_existing.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1387 2021-03-22 14:50:44.000000 climate_categories-0.7.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      705 2021-04-30 18:30:34.000000 climate_categories-0.7.1/climate_categories/tests/data/broken_simple_categorization.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      350 2021-11-25 15:20:07.000000 climate_categories-0.7.1/climate_categories/tests/data/good_conversion.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      650 2021-10-22 15:21:16.000000 climate_categories-0.7.1/climate_categories/tests/data/good_conversion_A.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      341 2021-10-22 15:48:52.000000 climate_categories-0.7.1/climate_categories/tests/data/good_conversion_B.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      372 2021-10-22 15:21:16.000000 climate_categories-0.7.1/climate_categories/tests/data/good_conversion_aux1.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      349 2021-10-22 15:21:16.000000 climate_categories-0.7.1/climate_categories/tests/data/good_conversion_aux2.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      350 2021-11-25 15:20:07.000000 climate_categories-0.7.1/climate_categories/tests/data/good_conversion_reversed.csv
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1387 2021-03-22 14:50:44.000000 climate_categories-0.7.1/climate_categories/tests/data/hierarchical_categorization.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      702 2021-03-22 14:50:44.000000 climate_categories-0.7.1/climate_categories/tests/data/simple_categorization.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1665 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/examples.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    21268 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_climate_categories.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    14197 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_conversions.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      769 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_di.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      508 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_gas.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1296 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_ipcc.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     7703 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_overcounting.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      596 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_primap.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      305 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_rcmip.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      462 2021-11-25 15:26:53.000000 climate_categories-0.7.1/climate_categories/tests/test_search.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.077100 climate_categories-0.7.1/climate_categories.egg-info/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8012 2021-11-25 15:30:23.000000 climate_categories-0.7.1/climate_categories.egg-info/PKG-INFO
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3523 2021-11-25 15:30:23.000000 climate_categories-0.7.1/climate_categories.egg-info/SOURCES.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        1 2021-11-25 15:30:23.000000 climate_categories-0.7.1/climate_categories.egg-info/dependency_links.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      299 2021-11-25 15:30:23.000000 climate_categories-0.7.1/climate_categories.egg-info/requires.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       19 2021-11-25 15:30:23.000000 climate_categories-0.7.1/climate_categories.egg-info/top_level.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      130 2021-10-22 15:21:16.000000 climate_categories-0.7.1/codecov.yml
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.081100 climate_categories-0.7.1/data_generation/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       62 2021-11-04 16:45:33.000000 climate_categories-0.7.1/data_generation/.gitignore
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5819 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/BURDI.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3177 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/BURDI_class.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    17598 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/CRF1999.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5318 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/CRFDI.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     5120 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/CRFDI_class.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    11573 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/IPCC1996.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8982 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/IPCC2006.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     4254 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/IPCC2006_PRIMAP.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8137 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/RCMIP.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      272 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/convert_yaml_to_python.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3344 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/gas.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1082 2021-11-25 15:26:53.000000 climate_categories-0.7.1/data_generation/utils.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2021-11-25 15:30:23.085100 climate_categories-0.7.1/docs/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      631 2021-01-21 11:13:36.000000 climate_categories-0.7.1/docs/Makefile
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      241 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/api.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       30 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/changelog.rst
--rwxrwxr-x   0 pflueger  (1000) pflueger  (1000)     5230 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/conf.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       33 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/contributing.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      337 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/credits.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     8178 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/data.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      325 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/index.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1209 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/installation.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      780 2021-01-18 17:21:51.000000 climate_categories-0.7.1/docs/make.bat
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       27 2021-11-25 15:26:53.000000 climate_categories-0.7.1/docs/readme.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       40 2021-10-22 15:21:16.000000 climate_categories-0.7.1/docs/requirements.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    18334 2021-10-22 15:48:52.000000 climate_categories-0.7.1/docs/usage.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      191 2021-03-22 14:50:44.000000 climate_categories-0.7.1/pyproject.toml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        2 2021-03-22 14:50:44.000000 climate_categories-0.7.1/requirements.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        7 2021-03-22 14:57:42.000000 climate_categories-0.7.1/requirements_dev.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1732 2021-11-25 15:30:23.085100 climate_categories-0.7.1/setup.cfg
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       61 2021-11-25 15:26:53.000000 climate_categories-0.7.1/setup.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1381 2021-11-25 15:26:41.000000 climate_categories-0.7.1/tbump.toml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      384 2021-11-04 16:33:47.000000 climate_categories-0.7.1/tox.ini
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      773 2021-11-25 15:26:53.000000 climate_categories-0.7.1/update_changelog.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1186 2021-11-25 15:26:53.000000 climate_categories-0.7.1/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.315656 climate_categories-0.8.1/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.github/ISSUE_TEMPLATE/new_categorization.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.8.1/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-04-26 12:34:31.000000 climate_categories-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.8.1/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.8.1/.sourcery.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      210 2023-04-26 09:04:13.000000 climate_categories-0.8.1/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4575 2023-04-26 14:01:13.000000 climate_categories-0.8.1/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      651 2023-04-26 09:04:13.000000 climate_categories-0.8.1/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3235 2023-04-26 12:32:41.000000 climate_categories-0.8.1/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8931 2023-04-26 14:03:08.315656 climate_categories-0.8.1/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3344 2023-04-26 14:02:09.000000 climate_categories-0.8.1/README.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/climate_categories/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1943 2023-04-26 14:01:00.000000 climate_categories-0.8.1/climate_categories/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    41200 2023-04-26 12:37:35.000000 climate_categories-0.8.1/climate_categories/_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.8.1/climate_categories/_conversions.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.311656 climate_categories-0.8.1/climate_categories/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.8.1/climate_categories/data/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.8.1/climate_categories/data/BURDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.8.1/climate_categories/data/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.8.1/climate_categories/data/BURDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.8.1/climate_categories/data/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.8.1/climate_categories/data/CRF1999.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2021.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2022.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/CRF2013_2023.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.8.1/climate_categories/data/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.8.1/climate_categories/data/CRFDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.8.1/climate_categories/data/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.8.1/climate_categories/data/CRFDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.8.1/climate_categories/data/GCB.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/data/GCB.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.8.1/climate_categories/data/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.8.1/climate_categories/data/IPCC1996.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.8.1/climate_categories/data/RCMIP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.8.1/climate_categories/data/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.8.1/climate_categories/data/gas.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.8.1/climate_categories/search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.311656 climate_categories-0.8.1/climate_categories/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.8.1/climate_categories/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.311656 climate_categories-0.8.1/climate_categories/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.8.1/climate_categories/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_conversion_not_allowed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_conversion_not_existing.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/broken_simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_A.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_B.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_aux1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_aux2.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/data/good_conversion_reversed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/data/simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21242 2023-04-26 12:40:48.000000 climate_categories-0.8.1/climate_categories/tests/test_climate_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.8.1/climate_categories/tests/test_conversions.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.8.1/climate_categories/tests/test_crf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_di.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_ipcc.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_overcounting.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.8.1/climate_categories/tests/test_primap.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.8.1/climate_categories/tests/test_rcmip.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.8.1/climate_categories/tests/test_search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.307656 climate_categories-0.8.1/climate_categories.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8931 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4001 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      326 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-04-26 14:03:08.000000 climate_categories-0.8.1/climate_categories.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.8.1/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.315656 climate_categories-0.8.1/data_generation/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.8.1/data_generation/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/convert_yaml_to_python.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.8.1/data_generation/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 14:03:08.315656 climate_categories-0.8.1/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5230 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/contributing.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8178 2023-04-26 09:06:11.000000 climate_categories-0.8.1/docs/data.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       40 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18334 2023-04-26 09:04:13.000000 climate_categories-0.8.1/docs/usage.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.8.1/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.8.1/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.8.1/requirements_dev.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1662 2023-04-26 14:03:08.315656 climate_categories-0.8.1/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.8.1/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-04-26 14:01:00.000000 climate_categories-0.8.1/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.8.1/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.8.1/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.8.1/update_citation_info.py
```

### Comparing `climate_categories-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `climate_categories-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `climate_categories-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/.github/ISSUE_TEMPLATE/new_categorization.md` & `climate_categories-0.8.1/.github/ISSUE_TEMPLATE/new_categorization.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/.github/workflows/ci.yml` & `climate_categories-0.8.1/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest, windows-latest ]
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [ 3.9, "3.10", "3.11"]
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `climate_categories-0.7.1/.gitignore` & `climate_categories-0.8.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -105,7 +105,10 @@
 
 # mypy
 .mypy_cache/
 
 # IDE settings
 .vscode/
 .idea/
+
+# Information on categorizations
+category_info
```

### Comparing `climate_categories-0.7.1/.pre-commit-config.yaml` & `climate_categories-0.8.1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: 'v4.0.1'
+    rev: 'v4.4.0'
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: check-ast
       - id: fix-byte-order-marker
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: detect-private-key
       - id: mixed-line-ending
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: 'v0.0.263'
+    hooks:
+      - id: ruff
+        args: [ --fix, --exit-non-zero-on-fix ]
   - repo: https://github.com/psf/black
-    rev: '21.11b1'
+    rev: '23.3.0'
     hooks:
       - id: black
   - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.4
+    rev: v0.3.8
     hooks:
       - id: blackdoc
-  - repo: https://github.com/PyCQA/flake8
-    rev: '4.0.1'
-    hooks:
-      - id: flake8
   - repo: https://github.com/PyCQA/doc8
-    rev: '0.10.1'
+    rev: 'v1.1.1'
     hooks:
       - id: doc8
         additional_dependencies: ['pygments-csv-lexer']
-  - repo: https://github.com/PyCQA/isort
-    rev: '5.10.1'
-    hooks:
-      - id: isort
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: '1.2.1'
+    rev: '1.7.0'
     hooks:
       - id: nbqa-black
         args: [ --nbqa-mutate, --line-length=75 ]
       - id: nbqa-check-ast
   - repo: https://github.com/asottile/blacken-docs
-    rev: 'v1.12.0'
+    rev: '1.13.0'
     hooks:
       - id: blacken-docs
```

### Comparing `climate_categories-0.7.1/CHANGELOG.rst` & `climate_categories-0.8.1/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 =========
 Changelog
 =========
 
+0.8.1 (2023-04-26)
+------------------
+* regenerate data included in the package to benefit
+  from latest fixes in data generation scripts.
+
+0.8.0 (2023-04-26)
+------------------
+* Add updated CRF2013 terminologies for 2021, 2022, and 2023 submission rounds
+* The unfccc DI API recently returns unspecified measure IDs.
+  data_generation/CRFDI_class.py was fixed to ignore them.
+* Add CRF2013 terminology for data submitted by AnnexI countries to the UNFCCC
+* Drop support for Python 3.7 and 3.8, add support for Python 3.11
+
 0.7.1 (2021-11-25)
 ------------------
 * Change conversion metadata format to use comment chars and a YAML header.
 
 0.7.0 (2021-11-25)
 ------------------
 * Use Python files instead of pickle objects for caching
```

### Comparing `climate_categories-0.7.1/CONTRIBUTING.rst` & `climate_categories-0.8.1/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring and check the generated
    API documentation.
-3. The pull request will be tested on python 3.7, 3.8, 3.9, and 3.10.
+3. The pull request will be tested on python 3.9, 3.10, and 3.11.
 
 Deploying
 ---------
 
 .. highlight:: shell
 
 A reminder for the maintainers on how to deploy.
```

### Comparing `climate_categories-0.7.1/LICENSE` & `climate_categories-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/Makefile` & `climate_categories-0.8.1/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -73,14 +73,18 @@
 
 cache: climate_categories/data/RCMIP.py
 cache: climate_categories/data/GCB.py
 cache: climate_categories/data/IPCC2006.py
 cache: climate_categories/data/IPCC2006_PRIMAP.py
 cache: climate_categories/data/IPCC1996.py
 cache: climate_categories/data/CRF1999.py
+cache: climate_categories/data/CRF2013.py
+cache: climate_categories/data/CRF2013_2021.py
+cache: climate_categories/data/CRF2013_2022.py
+cache: climate_categories/data/CRF2013_2023.py
 cache: climate_categories/data/gas.py
 cache: climate_categories/data/CRFDI.py
 cache: climate_categories/data/CRFDI_class.py
 cache: climate_categories/data/BURDI.py
 cache: climate_categories/data/BURDI_class.py  ## Generate Python specs from YAML files
 
 climate_categories/data/%.yaml: data_generation/%.py data_generation/utils.py
```

### Comparing `climate_categories-0.7.1/PKG-INFO` & `climate_categories-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: climate_categories
-Version: 0.7.1
+Version: 0.8.1
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@pik-potsdam.de
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 ==================
 Climate categories
@@ -48,14 +47,21 @@
 ===============  ==================================================================
 Name             Title
 ---------------  ------------------------------------------------------------------
 IPCC1996         IPCC GHG emission categories (1996)
 IPCC2006         IPCC GHG emission categories (2006)
 IPCC2006_PRIMAP  IPCC GHG emission categories (2006) with additional categories
 CRF1999          Common Reporting Format GHG emissions categories (1999)
+CRF2013          Common Reporting Format GHG emissions categories (2013)
+CRF2013_2021     CRF categories extended with country specific categories from
+                 2021 submissions
+CRF2013_2022     CRF categories extended with country specific categories from
+                 2022 submissions
+CRF2013_2023     CRF categories extended with country specific categories from
+                 2023 submissions
 BURDI            BUR GHG emission categories (DI query interface)
 BURDI_class      BUR GHG emission categories (DI query interface) + classifications
 CRFDI            CRF GHG emission categories (DI query interface)
 CRFDI_class      CRF GHG emission categories (DI query interface) + classifications
 GCB              Global Carbon Budget CO2 emission categories
 RCMIP            RCMIP emissions categories
 gas              Gases and other climate-forcing substances
@@ -87,22 +93,35 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2021-11-25).
-pik-primap/climate_categories: climate_categories Version 0.7.1.
-Zenodo. https://doi.org/10.5281/zenodo.5727646
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-04-26).
+pik-primap/climate_categories: climate_categories Version 0.8.1.
+Zenodo. https://doi.org/10.5281/zenodo.7867951
 
 =========
 Changelog
 =========
 
+0.8.1 (2023-04-26)
+------------------
+* regenerate data included in the package to benefit
+  from latest fixes in data generation scripts.
+
+0.8.0 (2023-04-26)
+------------------
+* Add updated CRF2013 terminologies for 2021, 2022, and 2023 submission rounds
+* The unfccc DI API recently returns unspecified measure IDs.
+  data_generation/CRFDI_class.py was fixed to ignore them.
+* Add CRF2013 terminology for data submitted by AnnexI countries to the UNFCCC
+* Drop support for Python 3.7 and 3.8, add support for Python 3.11
+
 0.7.1 (2021-11-25)
 ------------------
 * Change conversion metadata format to use comment chars and a YAML header.
 
 0.7.0 (2021-11-25)
 ------------------
 * Use Python files instead of pickle objects for caching
@@ -222,9 +241,7 @@
 * Add IPCC2006 categorization and scripts to generate it from the source pdf.
 
 0.1.0 (2021-01-18)
 ------------------
 
 * First release on PyPI.
 * Contains documentation and a stub API for querying, but no working code yet.
-
-
```

### Comparing `climate_categories-0.7.1/README.rst` & `climate_categories-0.8.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 ===============  ==================================================================
 Name             Title
 ---------------  ------------------------------------------------------------------
 IPCC1996         IPCC GHG emission categories (1996)
 IPCC2006         IPCC GHG emission categories (2006)
 IPCC2006_PRIMAP  IPCC GHG emission categories (2006) with additional categories
 CRF1999          Common Reporting Format GHG emissions categories (1999)
+CRF2013          Common Reporting Format GHG emissions categories (2013)
+CRF2013_2021     CRF categories extended with country specific categories from
+                 2021 submissions
+CRF2013_2022     CRF categories extended with country specific categories from
+                 2022 submissions
+CRF2013_2023     CRF categories extended with country specific categories from
+                 2023 submissions
 BURDI            BUR GHG emission categories (DI query interface)
 BURDI_class      BUR GHG emission categories (DI query interface) + classifications
 CRFDI            CRF GHG emission categories (DI query interface)
 CRFDI_class      CRF GHG emission categories (DI query interface) + classifications
 GCB              Global Carbon Budget CO2 emission categories
 RCMIP            RCMIP emissions categories
 gas              Gases and other climate-forcing substances
@@ -62,10 +69,10 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2021-11-25).
-pik-primap/climate_categories: climate_categories Version 0.7.1.
-Zenodo. https://doi.org/10.5281/zenodo.5727646
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-04-26).
+pik-primap/climate_categories: climate_categories Version 0.8.1.
+Zenodo. https://doi.org/10.5281/zenodo.7867951
```

### Comparing `climate_categories-0.7.1/climate_categories/__init__.py` & `climate_categories-0.8.1/climate_categories/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Access to all categorizations is provided directly at the module level, using the
 names of categorizations. To access the example categorization `Excat`, simply use
 `climate_categories.Excat` .
 """
 
 __author__ = """Mika Pflüger"""
 __email__ = "mika.pflueger@pik-potsdam.de"
-__version__ = "0.7.1"
+__version__ = "0.8.1"
 
 import importlib
 import importlib.resources
-import typing
 
-from . import data  # noqa: F401
-from . import search
-from ._categories import Categorization  # noqa: F401
-from ._categories import Category  # noqa: F401
-from ._categories import HierarchicalCategory  # noqa: F401
-from ._categories import from_pickle  # noqa: F401
-from ._categories import from_python  # noqa: F401
-from ._categories import from_spec  # noqa: F401
-from ._categories import from_yaml  # noqa: F401
-from ._categories import HierarchicalCategorization
-from ._conversions import Conversion, ConversionRule  # noqa: F401
+from . import (
+    search,
+)
+from ._categories import (
+    Categorization,
+    Category,
+    HierarchicalCategorization,
+    HierarchicalCategory,
+    from_pickle,
+    from_python,
+    from_spec,
+    from_yaml,
+)
+from ._conversions import Conversion, ConversionRule
 
 cats = {}
 
 
 def _read_py_hier(name) -> HierarchicalCategorization:
     mod = importlib.import_module(f".data.{name}", package="climate_categories")
     cat = HierarchicalCategorization.from_spec(mod.spec)
@@ -35,24 +37,28 @@
 
 
 # do this explicitly to help static analysis tools
 IPCC1996 = _read_py_hier("IPCC1996")
 IPCC2006 = _read_py_hier("IPCC2006")
 IPCC2006_PRIMAP = _read_py_hier("IPCC2006_PRIMAP")
 CRF1999 = _read_py_hier("CRF1999")
+CRF2013 = _read_py_hier("CRF2013")
+CRF2013_2021 = _read_py_hier("CRF2013_2021")
+CRF2013_2022 = _read_py_hier("CRF2013_2022")
+CRF2013_2023 = _read_py_hier("CRF2013_2023")
 CRFDI = _read_py_hier("CRFDI")
 CRFDI_class = _read_py_hier("CRFDI_class")
 BURDI = _read_py_hier("BURDI")
 BURDI_class = _read_py_hier("BURDI_class")
 GCB = _read_py_hier("GCB")
 RCMIP = _read_py_hier("RCMIP")
 gas = _read_py_hier("gas")
 
 
-def find_code(code: str) -> typing.Set[Category]:
+def find_code(code: str) -> set[Category]:
     """Search for the given code in all included categorizations."""
     return search.search_code(code, cats.values())
 
 
 __all__ = [
     "cats",
     "Categorization",
@@ -61,8 +67,10 @@
     "HierarchicalCategory",
     "Conversion",
     "ConversionRule",
     "find_code",
     "from_pickle",
     "from_spec",
     "from_yaml",
-] + list(cats.keys())
+    "from_python",
+    *list(cats.keys()),
+]
```

### Comparing `climate_categories-0.7.1/climate_categories/_categories.py` & `climate_categories-0.8.1/climate_categories/_categories.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Classes to represent and query categorical systems."""
 
 import datetime
+import functools
 import importlib
 import importlib.resources
 import pathlib
 import pickle
 import typing
 
 import natsort
@@ -28,69 +29,69 @@
             sy.Optional("alternative_codes"): sy.Seq(sy.Str()),
             sy.Optional("info"): sy.MapPattern(sy.Str(), sy.Any()),
         }
     )
 
     def __init__(
         self,
-        codes: typing.Tuple[str],
+        codes: tuple[str, ...],
         categorization: "Categorization",
         title: str,
-        comment: typing.Optional[str] = None,
-        info: typing.Optional[dict] = None,
+        comment: typing.Union[None, str] = None,
+        info: typing.Union[None, dict] = None,
     ):
         self.codes = codes
         self.title = title
         self.comment = comment
         self.categorization = categorization
         if info is None:
             self.info = {}
         else:
             self.info = info
         self._hash = None
 
     @classmethod
-    def from_spec(cls, code: str, spec: typing.Dict, categorization: "Categorization"):
+    def from_spec(cls, code: str, spec: dict, categorization: "Categorization"):
         codes = [code]
         if "alternative_codes" in spec:
             codes += spec["alternative_codes"]
             del spec["alternative_codes"]
         return cls(
             codes=tuple(codes),
             categorization=categorization,
             title=spec["title"],
-            comment=spec.get("comment", None),
-            info=spec.get("info", None),
+            comment=spec.get("comment"),
+            info=spec.get("info"),
         )
 
-    def to_spec(self) -> (str, typing.Dict[str, typing.Union[str, dict, list]]):
+    def to_spec(self) -> tuple[str, dict[str, typing.Union[str, dict, list]]]:
         """Turn this category into a specification ready to be written to a yaml file.
 
         Returns
         -------
         (code: str, spec: dict)
             Primary code and specification dict
         """
         code = self.codes[0]
-        spec = {"title": self.title}
+        spec: dict[str, typing.Union[str, dict, list[str]]] = {"title": self.title}
         if self.comment is not None:
             spec["comment"] = self.comment
         if len(self.codes) > 1:
             spec["alternative_codes"] = list(self.codes[1:])
         if self.info:
             spec["info"] = self.info
         return code, spec
 
     def __str__(self) -> str:
         return f"{self.codes[0]} {self.title}"
 
-    def __eq__(self, other: "Category"):
+    def __eq__(self, other: object):
         if not isinstance(other, Category):
-            return False
-        return any((x in other.codes for x in self.codes)) and (
+            return NotImplemented
+        return any(x in other.codes for x in self.codes) and (
             self.categorization is other.categorization
             or self.categorization.name.startswith(f"{other.categorization.name}_")
             or other.categorization.name.startswith(f"{self.categorization.name}_")
             or self.categorization.name == other.categorization.name
         )
 
     def __repr__(self) -> str:
@@ -117,66 +118,66 @@
             sy.Optional("info"): sy.MapPattern(sy.Str(), sy.Any()),
             sy.Optional("children"): sy.Seq(sy.Seq(sy.Str())),
         }
     )
 
     def __init__(
         self,
-        codes: typing.Tuple[str],
+        codes: tuple[str],
         categorization: "HierarchicalCategorization",
         title: str,
-        comment: typing.Optional[str] = None,
-        info: typing.Optional[dict] = None,
+        comment: typing.Union[None, str] = None,
+        info: typing.Union[None, dict] = None,
     ):
         Category.__init__(self, codes, categorization, title, comment, info)
         self.categorization = categorization
 
-    def to_spec(self) -> (str, typing.Dict[str, typing.Union[str, dict, list]]):
+    def to_spec(self) -> tuple[str, dict[str, typing.Union[str, dict, list]]]:
         """Turn this category into a specification ready to be written to a yaml file.
 
         Returns
         -------
         (code: str, spec: dict)
             Primary code and specification dict
         """
         code, spec = Category.to_spec(self)
-        children = []
-        for child_set in self.children:
-            children.append(list(sorted((c.codes[0] for c in child_set))))
+        children = [
+            list(sorted(c.codes[0] for c in child_set)) for child_set in self.children
+        ]
         if children:
             spec["children"] = children
         return code, spec
 
     @property
-    def children(self) -> typing.List[typing.Set["HierarchicalCategory"]]:
+    def children(self) -> list[set["HierarchicalCategory"]]:
         """The sets of subcategories comprising this category.
 
         The first set is canonical, the other sets are alternative.
         Only the canonical sets are used to calculate the level of a category."""
         return self.categorization.children(self)
 
     @property
-    def parents(self) -> typing.Set["HierarchicalCategory"]:
+    def parents(self) -> set["HierarchicalCategory"]:
         """The super-categories where this category is a member of any set of children.
 
         Note that all possible parents are returned, not "canonical" parents.
         """
         return self.categorization.parents(self)
 
     @property
-    def ancestors(self) -> typing.Set["HierarchicalCategory"]:
+    def ancestors(self) -> set["HierarchicalCategory"]:
         """The super-categories where this category or any of its parents is a member
         of any set of children, transitively.
 
         Note that all possible ancestors are returned, not only "canonical" ones.
         """
         return self.categorization.ancestors(self)
 
     @property
-    def descendants(self) -> typing.Set["HierarchicalCategory"]:
+    def descendants(self) -> set["HierarchicalCategory"]:
         """The sets of subcategories comprising this category directly or indirectly.
 
         Note that all possible descendants are returned, not only "canonical" ones."""
         return self.categorization.descendants(self)
 
     @property
     def level(self) -> int:
@@ -234,48 +235,48 @@
             "last_update": sy.Str(),
             "hierarchical": sy.Bool(),
             sy.Optional("version"): sy.Str(),
             "categories": sy.MapPattern(sy.Str(), Category._strictyaml_schema),
         }
     )
 
-    def _add_categories(self, categories: typing.Dict[str, typing.Dict]):
+    def _add_categories(self, categories: dict[str, dict]):
         for code, spec in categories.items():
             cat = Category.from_spec(code=code, spec=spec, categorization=self)
 
             self._primary_code_map[code] = cat
             for icode in cat.codes:
                 self._all_codes_map[icode] = cat
 
     def __init__(
         self,
         *,
-        categories: typing.Dict[str, typing.Dict],
+        categories: dict[str, dict],
         name: str,
         title: str,
         comment: str,
         references: str,
         institution: str,
         last_update: datetime.date,
-        version: typing.Optional[str] = None,
+        version: typing.Union[None, str] = None,
     ):
-        self._primary_code_map = {}
-        self._all_codes_map = {}
+        self._primary_code_map: dict[str, Category] = {}
+        self._all_codes_map: dict[str, Category] = {}
         self.name = name
         self.references = references
         self.title = title
         self.comment = comment
         self.institution = institution
         self.last_update = last_update
         self.version = version
 
         self._add_categories(categories)
 
         # is filled in __init__.py to contain all categorizations
-        self._cats: typing.Dict[str, "Categorization"] = {}
+        self._cats: dict[str, "Categorization"] = {}
 
     def __hash__(self):
         return hash(self.name)
 
     @classmethod
     def from_yaml(
         cls, filepath: typing.Union[str, pathlib.Path, typing.IO[bytes]]
@@ -285,15 +286,15 @@
             yaml = sy.load(filepath.read(), schema=cls._strictyaml_schema)
         except AttributeError:
             with open(filepath) as fd:
                 yaml = sy.load(fd.read(), schema=cls._strictyaml_schema)
         return cls.from_spec(yaml.data)
 
     @classmethod
-    def from_spec(cls, spec: typing.Dict[str, typing.Any]) -> "Categorization":
+    def from_spec(cls, spec: dict[str, typing.Any]) -> "Categorization":
         """Create Categorization from a Dictionary specification."""
         if spec["hierarchical"] != cls.hierarchical:
             raise ValueError(
                 "Specification is for a hierarchical categorization, use"
                 "HierarchicalCategorization.from_spec."
             )
         last_update = datetime.date.fromisoformat(spec["last_update"])
@@ -301,15 +302,15 @@
             categories=spec["categories"],
             name=spec["name"],
             title=spec["title"],
             comment=spec["comment"],
             references=spec["references"],
             institution=spec["institution"],
             last_update=last_update,
-            version=spec.get("version", None),
+            version=spec.get("version"),
         )
 
     @staticmethod
     def from_pickle(
         filepath: typing.Union[str, pathlib.Path, typing.IO[bytes]]
     ) -> "Categorization":
         """De-serialize Categorization from a file written by to_pickle.
@@ -324,15 +325,15 @@
     ) -> "Categorization":
         """De-serialize Categorization from a file written by to_python.
 
         Note that this executes the python cache file. Only load from python cache files
         you trust."""
         return from_python(filepath)
 
-    def to_spec(self) -> typing.Dict[str, typing.Any]:
+    def to_spec(self) -> dict[str, typing.Any]:
         """Turn this categorization into a specification dictionary ready to be written
         to a yaml file.
 
         Returns
         -------
         spec: dict
             Specification dictionary understood by `from_spec`.
@@ -344,18 +345,19 @@
             "references": self.references,
             "institution": self.institution,
             "hierarchical": self.hierarchical,
             "last_update": self.last_update.isoformat(),
         }
         if self.version is not None:
             spec["version"] = self.version
-        spec["categories"] = {}
+        categories = {}
         for cat in self.values():
             code, cat_spec = cat.to_spec()
-            spec["categories"][code] = cat_spec
+            categories[code] = cat_spec
+        spec["categories"] = categories
 
         return spec
 
     def to_yaml(self, filepath: typing.Union[str, pathlib.Path]) -> None:
         """Write to a YAML file."""
         spec = self.to_spec()
         yaml = YAML()
@@ -425,32 +427,32 @@
         comments = []
         alternative_codes = []
         for cat in self.values():
             titles.append(cat.title)
             comments.append(cat.comment)
             alternative_codes.append(cat.codes[1:])
         return pandas.DataFrame(
-            index=self.keys(),
+            index=list(self.keys()),
             data={
                 "title": titles,
                 "comment": comments,
                 "alternative_codes": alternative_codes,
             },
         )
 
     def _extend_prepare(
         self,
         *,
-        categories: typing.Optional[typing.Dict[str, typing.Dict]] = None,
-        alternative_codes: typing.Optional[typing.Dict[str, str]] = None,
+        categories: typing.Union[None, dict[str, dict]] = None,
+        alternative_codes: typing.Union[None, dict[str, str]] = None,
         name: str,
-        title: typing.Optional[str] = None,
-        comment: typing.Optional[str] = None,
-        last_update: typing.Optional[datetime.date] = None,
-    ) -> typing.Dict[str, typing.Any]:
+        title: typing.Union[None, str] = None,
+        comment: typing.Union[None, str] = None,
+        last_update: typing.Union[None, datetime.date] = None,
+    ) -> dict[str, typing.Any]:
         spec = self.to_spec()
 
         spec["name"] = f"{self.name}_{name}"
         spec["references"] = ""
         spec["institution"] = ""
 
         if title is None:
@@ -479,20 +481,20 @@
                 spec["categories"][primary]["alternative_codes"].append(alias)
 
         return spec
 
     def extend(
         self,
         *,
-        categories: typing.Optional[typing.Dict[str, typing.Dict]] = None,
-        alternative_codes: typing.Optional[typing.Dict[str, str]] = None,
+        categories: typing.Union[None, dict[str, dict]] = None,
+        alternative_codes: typing.Union[None, dict[str, str]] = None,
         name: str,
-        title: typing.Optional[str] = None,
-        comment: typing.Optional[str] = None,
-        last_update: typing.Optional[datetime.date] = None,
+        title: typing.Union[None, str] = None,
+        comment: typing.Union[None, str] = None,
+        last_update: typing.Union[None, datetime.date] = None,
     ) -> "Categorization":
         """Extend the categorization with additional categories, yielding a new
         categorization.
 
         Metadata: the ``name``, ``title``, ``comment``, and ``last_update`` are updated
         automatically (see below), the ``institution`` and ``references`` are deleted
         and the values for ``version`` and ``hierarchical`` are kept.
@@ -550,22 +552,25 @@
         If conversion rules for this conversion are not included, raises
         NotImplementedError."""
         if isinstance(other, str):
             other_name = other
         else:
             other_name = other.name
 
-        forward_csv_name = f"conversion.{self.name}.{other_name}.csv"
-        if importlib.resources.is_resource(data, forward_csv_name):
-            fd = importlib.resources.open_text(data, forward_csv_name)
-            return ConversionSpec.from_csv(fd).hydrate(cats=self._cats)
-        reversed_csv_name = f"conversion.{other_name}.{self.name}.csv"
-        if importlib.resources.is_resource(data, reversed_csv_name):
-            fd = importlib.resources.open_text(data, reversed_csv_name)
-            return ConversionSpec.from_csv(fd).hydrate(cats=self._cats).reversed()
+        data_files = importlib.resources.files(data)
+        forward_file = data_files / f"conversion.{self.name}.{other_name}.csv"
+        if forward_file.is_file():
+            return ConversionSpec.from_csv(forward_file.open()).hydrate(cats=self._cats)
+        reverse_file = data_files / f"conversion.{other_name}.{self.name}.csv"
+        if reverse_file.is_file():
+            return (
+                ConversionSpec.from_csv(reverse_file.open())
+                .hydrate(cats=self._cats)
+                .reversed()
+            )
 
         raise NotImplementedError(
             f"Conversion between {self.name} and {other_name} not yet included."
         )
 
 
 class HierarchicalCategorization(Categorization):
@@ -605,15 +610,15 @@
             sy.Optional("canonical_top_level_category"): sy.Str(),
             "categories": sy.MapPattern(
                 sy.Str(), HierarchicalCategory._strictyaml_schema
             ),
         }
     )
 
-    def _add_categories(self, categories: typing.Dict[str, typing.Dict]):
+    def _add_categories(self, categories: dict[str, dict]):
         for code, spec in categories.items():
             cat = HierarchicalCategory.from_spec(
                 code=code, spec=spec, categorization=self
             )
 
             self._primary_code_map[code] = cat
             self._graph.add_node(cat)
@@ -628,24 +633,24 @@
                         self._graph.add_edge(
                             parent, self._all_codes_map[child_code], set=i
                         )
 
     def __init__(
         self,
         *,
-        categories: typing.Dict[str, typing.Dict],
+        categories: dict[str, dict],
         name: str,
         title: str,
         comment: str,
         references: str,
         institution: str,
         last_update: datetime.date,
-        version: typing.Optional[str] = None,
+        version: typing.Union[None, str] = None,
         total_sum: bool,
-        canonical_top_level_category: typing.Optional[str] = None,
+        canonical_top_level_category: typing.Union[None, str] = None,
     ):
         self._graph = nx.MultiDiGraph()
         Categorization.__init__(
             self,
             categories=categories,
             name=name,
             title=title,
@@ -653,16 +658,16 @@
             references=references,
             institution=institution,
             last_update=last_update,
             version=version,
         )
         self.total_sum = total_sum
         if canonical_top_level_category is None:
-            self.canonical_top_level_category: typing.Optional[
-                HierarchicalCategory
+            self.canonical_top_level_category: typing.Union[
+                None, HierarchicalCategory
             ] = None
         else:
             self.canonical_top_level_category = self._all_codes_map[
                 canonical_top_level_category
             ]
 
     def __getitem__(self, code: str) -> HierarchicalCategory:
@@ -674,17 +679,15 @@
         return self._primary_code_map.values()
 
     def items(self) -> typing.ItemsView[str, HierarchicalCategory]:
         """Iterate over (primary code, category) pairs."""
         return self._primary_code_map.items()
 
     @classmethod
-    def from_spec(
-        cls, spec: typing.Dict[str, typing.Any]
-    ) -> "HierarchicalCategorization":
+    def from_spec(cls, spec: dict[str, typing.Any]) -> "HierarchicalCategorization":
         """Create Categorization from a Dictionary specification."""
         if spec["hierarchical"] != cls.hierarchical:
             raise ValueError(
                 "Specification is for a non-hierarchical categorization, use"
                 "Categorization.from_spec."
             )
         last_update = datetime.date.fromisoformat(spec["last_update"])
@@ -692,20 +695,20 @@
             categories=spec["categories"],
             name=spec["name"],
             title=spec["title"],
             comment=spec["comment"],
             references=spec["references"],
             institution=spec["institution"],
             last_update=last_update,
-            version=spec.get("version", None),
+            version=spec.get("version"),
             total_sum=spec["total_sum"],
-            canonical_top_level_category=spec.get("canonical_top_level_category", None),
+            canonical_top_level_category=spec.get("canonical_top_level_category"),
         )
 
-    def to_spec(self) -> typing.Dict[str, typing.Any]:
+    def to_spec(self) -> dict[str, typing.Any]:
         """Turn this categorization into a specification dictionary ready to be written
         to a yaml file.
 
         Returns
         -------
         spec: dict
             Specification dictionary understood by `from_spec`.
@@ -732,46 +735,43 @@
         spec["categories"] = {}
         for cat in self.values():
             code, cat_spec = cat.to_spec()
             spec["categories"][code] = cat_spec
 
         return spec
 
-    @property
+    @functools.cached_property
     def _canonical_subgraph(self) -> nx.DiGraph:
-        # TODO: from python 3.8 on, there is functools.cached_property to
-        # automatically cache this - as soon as we drop python 3.7 support, we can
-        # easily add it.
         return nx.DiGraph(
             self._graph.edge_subgraph(
-                ((u, v, 0) for (u, v, s) in self._graph.edges(data="set") if s == 0)
+                (u, v, 0) for (u, v, s) in self._graph.edges(data="set") if s == 0
             )
         )
 
     def _show_subtree_children(
         self,
         children: typing.Iterable[HierarchicalCategory],
         format_func: typing.Callable,
         prefix: str,
-        maxdepth: typing.Optional[int],
+        maxdepth: typing.Union[None, int],
     ) -> str:
         children_sorted = natsort.natsorted(children, key=format_func)
         r = "".join(
             self._show_subtree(
                 node=child,
-                prefix=prefix + "│",
+                prefix=f"{prefix}│",
                 format_func=format_func,
                 maxdepth=maxdepth,
             )
             for child in children_sorted[:-1]
         )
         # Last child needs to be called slightly differently
         r += self._show_subtree(
             node=children_sorted[-1],
-            prefix=prefix + " ",
+            prefix=f"{prefix} ",
             last=True,
             format_func=format_func,
             maxdepth=maxdepth,
         )
         return r
 
     @staticmethod
@@ -793,15 +793,15 @@
     def _show_subtree(
         self,
         *,
         node: HierarchicalCategory,
         prefix="",
         last=False,
         format_func: typing.Callable[[HierarchicalCategory], str] = str,
-        maxdepth: typing.Optional[int],
+        maxdepth: typing.Union[None, int],
     ) -> str:
         """Recursively-called function to show a subtree starting at the given node."""
 
         r = self._render_node(node, last=last, prefix=prefix, format_func=format_func)
 
         if maxdepth is not None:
             maxdepth -= 1
@@ -846,16 +846,16 @@
 
         return r
 
     def show_as_tree(
         self,
         *,
         format_func: typing.Callable[[HierarchicalCategory], str] = str,
-        maxdepth: typing.Optional[int] = None,
-        root: typing.Optional[typing.Union[HierarchicalCategory, str]] = None,
+        maxdepth: typing.Union[None, int] = None,
+        root: typing.Union[None, HierarchicalCategory, str] = None,
     ) -> str:
         """Format the hierarchy as a tree.
 
         Starting from the given root, or - if no root is given - the top-level
         categories (i.e. categories without parents), the tree of categories that are
         transitive children of the root is show, with children connected to their
         parents using lines. If a parent category has one set of children, the children
@@ -899,21 +899,21 @@
             )
             for top_level_node in top_level_nodes
         )
 
     def extend(
         self,
         *,
-        categories: typing.Optional[typing.Dict[str, typing.Dict]] = None,
-        alternative_codes: typing.Optional[typing.Dict[str, str]] = None,
-        children: typing.Optional[typing.List[tuple]] = None,
+        categories: typing.Union[None, dict[str, dict]] = None,
+        alternative_codes: typing.Union[None, dict[str, str]] = None,
+        children: typing.Union[None, list[tuple]] = None,
         name: str,
-        title: typing.Optional[str] = None,
-        comment: typing.Optional[str] = None,
-        last_update: typing.Optional[datetime.date] = None,
+        title: typing.Union[None, str] = None,
+        comment: typing.Union[None, str] = None,
+        last_update: typing.Union[None, datetime.date] = None,
     ) -> "HierarchicalCategorization":
         """Extend the categorization with additional categories and relationships,
         yielding a new categorization.
 
         Metadata: the ``name``, ``title``, ``comment``, and ``last_update`` are updated
         automatically (see below), the ``institution`` and ``references`` are deleted
         and the values for ``version``, ``hierarchical``, ``total_sum``, and
@@ -1019,46 +1019,46 @@
                     self._graph, self.canonical_top_level_category, cat
                 )
             except (nx.NetworkXNoPath, nx.NodeNotFound):
                 raise ValueError(
                     f"{cat.codes[0]!r} is not a transitive child of the "
                     f"canonical top level "
                     f"{self.canonical_top_level_category.codes[0]!r}."
-                )
+                ) from None
 
         return sp + 1
 
     def parents(
         self, cat: typing.Union[str, HierarchicalCategory]
-    ) -> typing.Set[HierarchicalCategory]:
+    ) -> set[HierarchicalCategory]:
         """The direct parents of the given category."""
         if not isinstance(cat, HierarchicalCategory):
             return self.parents(self._all_codes_map[cat])
 
         return set(self._graph.predecessors(cat))
 
     def ancestors(
         self, cat: typing.Union[str, HierarchicalCategory]
-    ) -> typing.Set[HierarchicalCategory]:
+    ) -> set[HierarchicalCategory]:
         """All ancestors of the given category, i.e. the direct parents and their
         parents, etc."""
         if not isinstance(cat, HierarchicalCategory):
             return self.ancestors(self._all_codes_map[cat])
 
         return set(nx.ancestors(self._graph, cat))
 
     def children(
         self, cat: typing.Union[str, HierarchicalCategory]
-    ) -> typing.List[typing.Set[HierarchicalCategory]]:
+    ) -> list[set[HierarchicalCategory]]:
         """The list of sets of direct children of the given category."""
         if not isinstance(cat, HierarchicalCategory):
             return self.children(self._all_codes_map[cat])
 
         children_dict = {}
-        for (_, child, setno) in self._graph.edges(cat, "set"):
+        for _, child, setno in self._graph.edges(cat, "set"):
             if setno not in children_dict:
                 children_dict[setno] = []
             children_dict[setno].append(child)
 
         return [set(children_dict[x]) for x in sorted(children_dict.keys())]
 
     def descendants(self, cat: typing.Union[str, HierarchicalCategory]):
@@ -1094,28 +1094,27 @@
 
     Note that this executes the python cache file. Only load from python cache files
     you trust."""
     try:
         python_code = filepath.read()
         filepath.seek(0)
     except AttributeError:
-        with open(filepath) as fd:
-            python_code = fd.read()
+        python_code = pathlib.Path(filepath).read_text()
     variables = {}
     exec(python_code, variables)
     spec = variables["spec"]
     if spec["hierarchical"]:
         cls = HierarchicalCategorization
     else:
         cls = Categorization
     return cls.from_spec(spec)
 
 
 def from_spec(
-    spec: typing.Dict[str, typing.Any]
+    spec: dict[str, typing.Any]
 ) -> typing.Union[Categorization, HierarchicalCategorization]:
     """Create Categorization or HierarchicalCategorization from a dict specification."""
     if spec["hierarchical"]:
         return HierarchicalCategorization.from_spec(spec)
     else:
         return Categorization.from_spec(spec)
```

### Comparing `climate_categories-0.7.1/climate_categories/_conversions.py` & `climate_categories-0.8.1/climate_categories/_conversions.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import csv
 import dataclasses
 import datetime
 import pathlib
 import typing
 from typing import TYPE_CHECKING
 
+import immutables
 import pyparsing
 import strictyaml as sy
 
 if TYPE_CHECKING:
     from ._categories import Categorization, Category, HierarchicalCategory
 
 
@@ -42,26 +43,26 @@
         rule is only valid for the given category codes. If multiple auxiliary
         categorizations are given, the rule is only valid if all auxiliary
         categorizations match.
     comment : str
         A human-readable comment explaining the rule or adding additional information.
     """
 
-    factors_categories_a: typing.Dict[str, int]
-    factors_categories_b: typing.Dict[str, int]
-    auxiliary_categories: typing.Dict[str, typing.Set[str]]
+    factors_categories_a: dict[str, int]
+    factors_categories_b: dict[str, int]
+    auxiliary_categories: dict[str, set[str]]
     comment: str = ""
     csv_line_number: typing.Optional[int] = None
     csv_original_text: typing.Optional[str] = None
 
     def hydrate(
         self,
         categorization_a: "Categorization",
         categorization_b: "Categorization",
-        cats: typing.Dict[str, "Categorization"],
+        cats: dict[str, "Categorization"],
     ) -> "ConversionRule":
         """Convert this specification into a ConversionRule object with full
         functionality."""
 
         auxiliary_categories_hydrated = {}
         for aux_categorization_name, categories in self.auxiliary_categories.items():
             aux_categorization = cats[aux_categorization_name]
@@ -78,39 +79,51 @@
             ),
             auxiliary_categories=auxiliary_categories_hydrated,
             comment=self.comment,
             csv_line_number=self.csv_line_number,
             csv_original_text=self.csv_original_text,
         )
 
+    @typing.overload
+    def _hydrate_handle_errors(
+        self, to_hydrate: dict[str, int], categorization: "Categorization"
+    ) -> dict["Category", int]:
+        ...
+
+    @typing.overload
+    def _hydrate_handle_errors(
+        self, to_hydrate: set[str], categorization: "Categorization"
+    ) -> set["Category"]:
+        ...
+
     def _hydrate_handle_errors(
         self,
-        to_hydrate: typing.Union[typing.Dict[str, int], typing.Set[str]],
+        to_hydrate: typing.Union[dict[str, int], set[str]],
         categorization: "Categorization",
-    ) -> typing.Union[typing.Dict["Category", int], typing.Set["Category"]]:
+    ) -> typing.Union[dict["Category", int], set["Category"]]:
         """Hydrate a dict/set while nicely handling errors."""
         try:
             if isinstance(to_hydrate, dict):
                 return {
                     categorization[code]: factor for code, factor in to_hydrate.items()
                 }
             else:
                 return {categorization[code] for code in to_hydrate}
         except KeyError as err:
             code = err.args[0]
             raise ValueError(
                 f"Error in line {self.csv_line_number}: {code!r} not in"
                 f" {categorization}."
-            )
+            ) from None
 
     # Parsing rules for simple formulas from str
     # Supported operators at the moment are plus and minus
     _operator = pyparsing.Char("+") ^ pyparsing.Char("-")
-    _operator_factors = {"+": 1, "-": -1}
-    _factor_operators = {1: "+", -1: "-"}
+    _operator_factors = immutables.Map({"+": 1, "-": -1})
+    _factor_operators = immutables.Map({1: "+", -1: "-"})
     # alphanumeric category codes can be given directly, others have to be quoted
     _category_code = pyparsing.Word(pyparsing.alphanums + ".") ^ pyparsing.QuotedString(
         quoteChar='"', escChar="\\"
     )
     _formula = (
         pyparsing.StringStart()
         + pyparsing.Optional(_operator("unary_op"))
@@ -121,15 +134,15 @@
     _auxiliary_codes = (
         pyparsing.StringStart()
         + pyparsing.ZeroOrMore(_category_code("aux_category_code"))
         + pyparsing.StringEnd()
     )
 
     @classmethod
-    def _parse_aux_codes(cls, aux_codes_str: str) -> typing.List[str]:
+    def _parse_aux_codes(cls, aux_codes_str: str) -> list[str]:
         """Parse a whitespace-separated list of auxiliary codes.
 
         Parameters
         ----------
         aux_codes_str: str
             Category codes separated by whitespace. Alphanumeric category codes can be
             given directly, other category codes must be quoted using double quotes.
@@ -154,19 +167,19 @@
         """
         try:
             tokens = cls._auxiliary_codes.parseString(aux_codes_str)
         except pyparsing.ParseException as exc:
             raise ValueError(
                 f"Could not parse: {aux_codes_str!r}, error: {exc.msg},"
                 f" error at char {exc.loc}"
-            )
+            ) from None
         return list(tokens)
 
     @classmethod
-    def _parse_formula(cls, formula: str) -> typing.Dict[str, int]:
+    def _parse_formula(cls, formula: str) -> dict[str, int]:
         """Parse a formula into factors for categories.
 
         Parameters
         ----------
         formula: str
             Formula comprising category codes connected with + or - . Alphanumeric
             category codes can be given directly, other category codes must be quoted
@@ -202,38 +215,37 @@
         """
         try:
             tokens = cls._formula.parseString(formula)
         except pyparsing.ParseException as exc:
             raise ValueError(
                 f"Could not parse: {formula!r}, error: {exc.msg},"
                 f" error at char {exc.loc}"
-            )
-        code_factors = {}
+            ) from None
         # first operator is implicitly a plus, have to handle it specially
         if "unary_op" in tokens:
             op = tokens.pop(0)
         else:
             op = "+"
         code = tokens.pop(0)
-        code_factors[code] = cls._operator_factors[op]
+        code_factors = {code: cls._operator_factors[op]}
         while len(tokens):
             op = tokens.pop(0)
             code = tokens.pop(0)
             if code in code_factors:
                 code_factors[code] += cls._operator_factors[op]
             else:
                 code_factors[code] = cls._operator_factors[op]
 
         return code_factors
 
     @classmethod
     def from_csv_row(
         cls,
         irow: typing.Iterator[str],
-        aux_names: typing.List[str],
+        aux_names: list[str],
         line_number: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> "ConversionRuleSpec":
         """Parse a ConversionRuleSpec from a row in a CSV file.
 
         Parameters
         ----------
@@ -275,17 +287,15 @@
             auxiliary_categories=auxiliary_categories,
             comment=comment,
             csv_line_number=line_number,
             csv_original_text=",".join(row),
         )
 
     @classmethod
-    def _factors_categories_formula(
-        cls, factors_categories: typing.Dict[str, int]
-    ) -> str:
+    def _factors_categories_formula(cls, factors_categories: dict[str, int]) -> str:
         """Serialize a dict mapping categories to factors to a formula string.
 
         Parameters
         ----------
         factors_categories: dict
             Mapping of categories to factors.
 
@@ -332,21 +342,25 @@
             return code
         # replace:
         # \ -> \\
         # " -> \"
         esc = code.replace("\\", "\\\\").replace('"', '\\"')
         return f'"{esc}"'
 
-    def to_csv_row(self) -> typing.List[str]:
+    def to_csv_row(self) -> list[str]:
         """Return a representation of this rule suitable for writing to a CSV file."""
         row = [self._factors_categories_formula(self.factors_categories_a)]
         for aux_categories in self.auxiliary_categories.values():
             row.append(" ".join(sorted(map(self._escape_code, aux_categories))))
-        row.append(self._factors_categories_formula(self.factors_categories_b))
-        row.append(self.comment)
+        row.extend(
+            (
+                self._factors_categories_formula(self.factors_categories_b),
+                self.comment,
+            )
+        )
         return row
 
     def __str__(self) -> str:
         if self.csv_original_text is not None:
             return self.csv_original_text
         return ",".join(self.to_csv_row())
 
@@ -390,17 +404,17 @@
     is_restricted : bool
         The rule is restricted if and only if for at least one auxiliary categorization
         at least one category is specified, so that the rule is only valid for a
         subset of cases. Otherwise, the rule is unrestricted and valid for all
         cases.
     """
 
-    factors_categories_a: typing.Dict["Category", int]
-    factors_categories_b: typing.Dict["Category", int]
-    auxiliary_categories: typing.Dict["Categorization", typing.Set["Category"]]
+    factors_categories_a: dict["Category", int]
+    factors_categories_b: dict["Category", int]
+    auxiliary_categories: dict["Categorization", set["Category"]]
     comment: str = ""
     csv_line_number: typing.Optional[int] = None
     csv_original_text: typing.Optional[str] = None
     cardinality_a: str = dataclasses.field(init=False)
     cardinality_b: str = dataclasses.field(init=False)
     is_restricted: bool = dataclasses.field(init=False)
 
@@ -417,15 +431,17 @@
             "cardinality_b",
             "one" if len(self.factors_categories_b) == 1 else "many",
         )
         object.__setattr__(
             self, "is_restricted", any(self.auxiliary_categories.values())
         )
 
-    def __eq__(self, other: "ConversionRule"):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, ConversionRule):
+            return NotImplemented
         return (
             self.factors_categories_a == other.factors_categories_a
             and self.factors_categories_b == other.factors_categories_b
             and self.auxiliary_categories == other.auxiliary_categories
             and self.comment == other.comment
         )
 
@@ -559,16 +575,16 @@
     """
 
     def __init__(
         self,
         *,
         categorization_a_name: str,
         categorization_b_name: str,
-        rule_specs: typing.List[ConversionRuleSpec],
-        auxiliary_categorizations_names: typing.Optional[typing.List[str]] = None,
+        rule_specs: list[ConversionRuleSpec],
+        auxiliary_categorizations_names: typing.Optional[list[str]] = None,
         comment: typing.Optional[str] = None,
         references: typing.Optional[str] = None,
         institution: typing.Optional[str] = None,
         last_update: typing.Optional[datetime.date] = None,
         version: typing.Optional[str] = None,
     ):
         self.categorization_a_name = categorization_a_name
@@ -626,16 +642,16 @@
     )
 
     def __init__(
         self,
         *,
         categorization_a_name: str,
         categorization_b_name: str,
-        rule_specs: typing.List[ConversionRuleSpec],
-        auxiliary_categorizations_names: typing.Optional[typing.List[str]] = None,
+        rule_specs: list[ConversionRuleSpec],
+        auxiliary_categorizations_names: typing.Optional[list[str]] = None,
         comment: typing.Optional[str] = None,
         references: typing.Optional[str] = None,
         institution: typing.Optional[str] = None,
         last_update: typing.Optional[datetime.date] = None,
         version: typing.Optional[str] = None,
     ):
         ConversionBase.__init__(
@@ -668,15 +684,14 @@
         Returns
         -------
         meta_data: dict
             Mapping of meta data keys to values.
         linecount: int
             Count of lines of the metadata block
         """
-        meta_data = {}
         yaml_header = ""
         last_pos = fd.tell()
         line = fd.readline()
         while line.startswith("#"):
             # remove leading comment and whitespace
             yaml_header += line[1:].lstrip()
             last_pos = fd.tell()
@@ -685,15 +700,15 @@
         meta_data = sy.load(yaml_header, schema=cls._strictyaml_metadata_schema).data
 
         return meta_data, yaml_header.count("\n")
 
     @classmethod
     def _read_csv_rules(
         cls, reader: csv.reader, offset: int
-    ) -> typing.Tuple[str, str, typing.List[str], typing.List[ConversionRuleSpec]]:
+    ) -> tuple[str, str, list[str], list[ConversionRuleSpec]]:
         """Read the data section of a CSV specification file. It consists of a header,
         followed by rules, with each rule on one line.
 
         Parameters
         ----------
         reader: CSV reader object as returned by csv.reader
             The reader object must already be advanced to the rules section, so that
@@ -704,15 +719,15 @@
         Returns
         -------
         a_name, b_name, aux_names, rule_specs: str, str, list, list
            The name of categorizations A and B, the names of the auxiliary categories,
            and the parsed rules.
         """
         rule_specs = []
-        header = next(reader)
+        header: list[str] = next(reader)
         a_name = header[0]
         b_name = header[-2]
         if header[-1] != "comment":
             raise ValueError("Last column must be 'comment', but isn't.")
         aux_names = header[1:-2]
         for row in reader:
             line_num = reader.line_num + offset
@@ -720,20 +735,23 @@
             try:
                 rule_specs.append(
                     ConversionRuleSpec.from_csv_row(
                         irow, aux_names=aux_names, line_number=line_num
                     )
                 )
             except ValueError as err:
-                raise ValueError(f"Error in line {line_num}: {err}")
+                raise ValueError(f"Error in line {line_num}: {err}") from None
 
         return a_name, b_name, aux_names, rule_specs
 
     @classmethod
-    def _from_csv(cls, fd: typing.TextIO) -> "ConversionSpec":
+    def _from_csv(
+        cls,
+        fd: typing.TextIO,
+    ) -> "ConversionSpec":
         meta_data, len_meta_data = cls._read_csv_meta(fd)
         reader = csv.reader(fd, quoting=csv.QUOTE_NONE, escapechar="\\")
         a_name, b_name, aux_names, rule_specs = cls._read_csv_rules(
             reader, len_meta_data
         )
 
         return cls(
@@ -743,15 +761,15 @@
             auxiliary_categorizations_names=aux_names or None,
             **meta_data,
         )
 
     @classmethod
     def from_csv(
         cls,
-        filepath: typing.Union[str, pathlib.Path, typing.TextIO, typing.Iterable[str]],
+        filepath: typing.Union[str, pathlib.Path, typing.TextIO],
     ) -> "ConversionSpec":
         """Read conversion from comma-separated-values file."""
         if not isinstance(filepath, (str, pathlib.Path)):
             return cls._from_csv(filepath)
         fp = pathlib.Path(filepath)
         with fp.open(newline="") as fd:
             return cls._from_csv(fd)
@@ -760,15 +778,15 @@
         return (
             f"<ConversionSpec {self.categorization_a_name!r} <->"
             f" {self.categorization_b_name!r} with {len(self.rule_specs)} rules>"
         )
 
     def hydrate(
         self,
-        cats: typing.Dict[str, "Categorization"],
+        cats: dict[str, "Categorization"],
     ) -> "Conversion":
         """Convert this Specification into a Conversion object with full
         functionality."""
         categorization_a = cats[self.categorization_a_name]
         categorization_b = cats[self.categorization_b_name]
         auxiliary_categorizations = (
             [cats[x] for x in self.auxiliary_categorizations_names]
@@ -796,21 +814,19 @@
 
 
 @dataclasses.dataclass(frozen=True)
 class OverCountingProblem:
     """A suspected over counting problem."""
 
     category: "HierarchicalCategory"
-    leave_node_groups: typing.List[typing.Set["HierarchicalCategory"]]
-    rules: typing.List[ConversionRule]
+    leave_node_groups: list[set["HierarchicalCategory"]]
+    rules: list[ConversionRule]
 
     def __str__(self):
-        involved_rules_str = ", ".join(
-            (rule.format_with_lineno() for rule in self.rules)
-        )
+        involved_rules_str = ", ".join(rule.format_with_lineno() for rule in self.rules)
         sorted_leave_node_groups = [sorted(g) for g in self.leave_node_groups]
         return (
             f"{self.category!r} is possibly counted multiple times"
             f"\ninvolved leave groups categories: {sorted_leave_node_groups!r}"
             f"\ninvolved rules: {involved_rules_str}."
         )
 
@@ -845,18 +861,16 @@
     """
 
     def __init__(
         self,
         *,
         categorization_a: "Categorization",
         categorization_b: "Categorization",
-        rules: typing.List[ConversionRule],
-        auxiliary_categorizations: typing.Optional[
-            typing.List["Categorization"]
-        ] = None,
+        rules: list[ConversionRule],
+        auxiliary_categorizations: typing.Optional[list["Categorization"]] = None,
         comment: typing.Optional[str] = None,
         references: typing.Optional[str] = None,
         institution: typing.Optional[str] = None,
         last_update: typing.Optional[datetime.date] = None,
         version: typing.Optional[str] = None,
     ):
         ConversionBase.__init__(
@@ -908,16 +922,16 @@
         -1 * IPCC1996 4 Agriculture
         to indicate that category 4 should be subtracted.
         """
         one_to_one = []
         one_to_many = []
         many_to_one = []
         many_to_many = []
-        cats_a = set()
-        cats_b = set()
+        cats_a: set["Category"] = set()
+        cats_b: set["Category"] = set()
         for rule in self.rules:
             cats_a.update(rule.factors_categories_a.keys())
             cats_b.update(rule.factors_categories_b.keys())
             if rule.cardinality_a == "one" and rule.cardinality_b == "one":
                 one_to_one.append(rule)
             elif rule.cardinality_a == "one":
                 one_to_many.append(rule)
@@ -945,42 +959,42 @@
         r += "\n".join((rule.format_human_readable()) for rule in many_to_many)
         r += "\n\n"
 
         r += "## Unmapped categories\n\n"
         cats_missing_a = set(self.categorization_a.values()) - cats_a
         cats_missing_b = set(self.categorization_b.values()) - cats_b
         r += f"### {cat_a}\n"
-        r += "\n".join(sorted((str(x) for x in cats_missing_a))) + "\n\n"
+        r += "\n".join(sorted(str(x) for x in cats_missing_a)) + "\n\n"
         r += f"### {cat_b}\n"
-        r += "\n".join(sorted((str(x) for x in cats_missing_b))) + "\n\n"
+        r += "\n".join(sorted(str(x) for x in cats_missing_b)) + "\n\n"
 
         return r
 
     def find_unmapped_categories(
         self,
-    ) -> (typing.Set["Category"], typing.Set["Category"]):
+    ) -> tuple[set["Category"], set["Category"]]:
         """Find categories for which no rule exists to map them.
 
         Returns
         -------
         missing_categories_a, missing_categories_b: set, set
             A list of categories missing from categorization_a and categorization_b,
             respectively.
         """
-        cats_a = set()
-        cats_b = set()
+        cats_a: set["Category"] = set()
+        cats_b: set["Category"] = set()
         for rule in self.rules:
             cats_a.update(rule.factors_categories_a.keys())
             cats_b.update(rule.factors_categories_b.keys())
 
         cats_missing_a = set(self.categorization_a.values()) - cats_a
         cats_missing_b = set(self.categorization_b.values()) - cats_b
         return cats_missing_a, cats_missing_b
 
-    def find_over_counting_problems(self) -> typing.List[OverCountingProblem]:
+    def find_over_counting_problems(self) -> list[OverCountingProblem]:
         """Check if any category from one side is counted more than once on the
         other side.
 
         Note that the algorithm at the moment can't reliably detect all over counting
         problems and also some suspected problems might be fine under closer
         examination, so use this function only to generate hints for possible problems.
 
@@ -991,38 +1005,39 @@
         """
         for categorization in self.categorization_a, self.categorization_b:
             if not categorization.hierarchical:
                 raise ValueError(
                     f"{categorization} is not hierarchical, without "
                     f"a hierarchy, over counting can not be evaluated."
                 )
-            if not categorization.total_sum:
+            if not categorization.total_sum:  # type: ignore
                 raise ValueError(
                     f"For {categorization} it is not specified that the "
                     f"sum of a set of children equals the parent, so "
                     f"over counting can not be evaluated."
                 )
 
         problems = []
         for categorization in self.categorization_a, self.categorization_b:
-            descendants = {}  # used to cache costly descendant evaluation
+            # used to cache costly descendant evaluation
+            descendants: dict[str, set[str]] = {}
             for category in categorization.values():
                 prob = self._check_over_counting_category(
-                    category, categorization, descendants
+                    category, categorization, descendants  # type: ignore
                 )
                 if prob:
                     problems.append(prob)
 
         return problems
 
     @staticmethod
     def _leave_node_group(
         categories: typing.Iterable["HierarchicalCategory"],
-        hull: typing.Set[str],
-        descendants: typing.Dict[str, typing.Iterable[str]],
+        hull: set[str],
+        descendants: dict[str, set[str]],
     ) -> bool:
         """Are all of the given categories leave nodes of the given hull?
 
         Parameters
         ----------
         categories: list of HierarchicalCategory objects
             Categories that will be checked. If any of the categories has descendants
@@ -1053,18 +1068,18 @@
             for d in desc:
                 if d in hull:
                     return False
         return True
 
     def relevant_rules(
         self,
-        categories: typing.Set["HierarchicalCategory"],
+        categories: set["HierarchicalCategory"],
         source_categorization: typing.Optional["Categorization"] = None,
         simple_sums_only: bool = False,
-    ) -> typing.List[ConversionRule]:
+    ) -> list[ConversionRule]:
         """Returns all rules which involve the given categories.
 
         Parameters
         ----------
         categories: set of HierarchicalCategory
             The categories to limit the rules to.
         source_categorization: Categorization, optional
@@ -1075,15 +1090,15 @@
             summands (i.e. with a factor of 1).
 
         Returns
         -------
         relevant_rules:
             All rules which touch the given categories.
         """
-        relevant_rules = []
+        relevant_rules: list[ConversionRule] = []
         if not categories:
             return relevant_rules
 
         if source_categorization is None:
             source_categorization = next(iter(categories)).categorization
 
         for rule in self.rules:
@@ -1104,15 +1119,15 @@
 
         return relevant_rules
 
     def _check_over_counting_category(
         self,
         category: "HierarchicalCategory",
         source_categorization: "Categorization",
-        descendants: typing.Dict[str, typing.Set[str]],
+        descendants: dict[str, set[str]],
     ) -> typing.Optional[OverCountingProblem]:
         """Finds possible over counting problems for the specified category.
 
         Parameters
         ----------
         category: HierarchicalCategory
             The category to check.
@@ -1182,34 +1197,34 @@
         relevant_rules = self.relevant_rules(
             categories=ancestral_set,
             source_categorization=source_categorization,
             simple_sums_only=True,
         )
         # TODO: for now, only use rules that don't have aux categories
         relevant_rules = [rule for rule in relevant_rules if not rule.is_restricted]
-        projected_ancestral_set: typing.List[typing.Set["HierarchicalCategory"]] = []
+        projected_ancestral_set: list[set["HierarchicalCategory"]] = []
         for rule in relevant_rules:
             if source_categorization == self.categorization_a:
                 fc = rule.factors_categories_b
             else:
                 fc = rule.factors_categories_a
             target_categories = {cat for cat, factor in fc.items() if factor == 1}
-            projected_ancestral_set.append(target_categories)
+            projected_ancestral_set.append(target_categories)  # type: ignore
 
         if not projected_ancestral_set:  # trivial
-            return
+            return None
 
         # for performance, use codes (which are guaranteed to be unique within a
         # categorization) for the comparisons here
         projected_ancestral_set_codes = [
             {c.codes[0] for c in group} for group in projected_ancestral_set
         ]
 
         # hull(PA_S(c))
-        hull: typing.Set[str] = set().union(*projected_ancestral_set_codes)
+        hull: set[str] = set().union(*projected_ancestral_set_codes)
 
         # L(PA_S(c))
         leave_node_groups = [
             m
             for m in projected_ancestral_set
             if self._leave_node_group(m, hull, descendants)
         ]
@@ -1219,14 +1234,16 @@
 
         if len(leave_hull) != len(largest):
             return OverCountingProblem(
                 category=category,
                 rules=relevant_rules,
                 leave_node_groups=leave_node_groups,
             )
+        else:
+            return None
 
     def __eq__(self, other):
         return (
             isinstance(other, Conversion)
             and self.categorization_a == other.categorization_a
             and self.categorization_b == other.categorization_b
             and self.rules == other.rules
```

### Comparing `climate_categories-0.7.1/climate_categories/data/BURDI.py` & `climate_categories-0.8.1/climate_categories/data/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/BURDI.yaml` & `climate_categories-0.8.1/climate_categories/data/BURDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/BURDI_class.py` & `climate_categories-0.8.1/climate_categories/data/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/BURDI_class.yaml` & `climate_categories-0.8.1/climate_categories/data/BURDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/CRF1999.py` & `climate_categories-0.8.1/climate_categories/data/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/CRF1999.yaml` & `climate_categories-0.8.1/climate_categories/data/CRF1999.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/CRFDI.py` & `climate_categories-0.8.1/climate_categories/data/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/CRFDI.yaml` & `climate_categories-0.8.1/climate_categories/data/CRFDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/CRFDI_class.py` & `climate_categories-0.8.1/climate_categories/data/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/CRFDI_class.yaml` & `climate_categories-0.8.1/climate_categories/data/CRFDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/GCB.py` & `climate_categories-0.8.1/climate_categories/data/GCB.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/GCB.yaml` & `climate_categories-0.8.1/climate_categories/data/GCB.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/IPCC1996.py` & `climate_categories-0.8.1/climate_categories/data/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/IPCC1996.yaml` & `climate_categories-0.8.1/climate_categories/data/IPCC1996.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/IPCC2006.py` & `climate_categories-0.8.1/climate_categories/data/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/IPCC2006.yaml` & `climate_categories-0.8.1/climate_categories/data/IPCC2006.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/IPCC2006_PRIMAP.py` & `climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/IPCC2006_PRIMAP.yaml` & `climate_categories-0.8.1/climate_categories/data/IPCC2006_PRIMAP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/RCMIP.py` & `climate_categories-0.8.1/climate_categories/data/RCMIP.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Do not edit this file. It was auto-generated from the
 # corresponding YAML file.
 spec = {
     "name": "RCMIP",
     "title": "Emissions categories from the Reduced Complexity Model Intercomparison Project (RCMIP)",
     "comment": "AFOLU in the SSPDb is AFOLU minus any agriculture\nrelated fossil fuel based emissions hence is not the same as the\nWG3 AFOLU definition. Rather AFOLU in the SSPDb is AFOLU as expected by\nMAGICC (i.e. exluding agriculture related fossil fuel use), hence\nwe call it MAGICC AFOLU.",
-    "references": "Nicholls, Z. R. J., Meinshausen, M., Lewis, J., Gieseke, R., Dommenget, D., Dorheim, K., Fan, C.-S., Fuglestvedt, J. S., Gasser, T., Golüke, U., Goodwin, P., Hartin, C., Hope, A. P., Kriegler, E., Leach, N. J., Marchegiani, D., McBride, L. A., Quilcaille, Y., Rogelj, J., Salawitch, R. J., Samset, B. H., Sandstad, M., Shiklomanov, A. N., Skeie, R. B., Smith, C. J., Smith, S., Tanaka, K., Tsutsui, J., and Xie, Z.: Reduced Complexity Model Intercomparison Project Phase 1: introduction and evaluation of global-mean temperature response, Geosci. Model Dev., 13, 5175–5190, https://doi.org/10.5194/gmd-13-5175-2020, 2020.",
+    "references": "Nicholls, Z. R. J., Meinshausen, M., Lewis, J., Gieseke, R., Dommenget, D., Dorheim, K., Fan, C.-S., Fuglestvedt, J. S., Gasser, T., Golüke, U., Goodwin, P., Hartin, C., Hope, A. P., Kriegler, E., Leach, N. J., Marchegiani, D., McBride, L. A., Quilcaille, Y., Rogelj, J., Salawitch, R. J., Samset, B. H., Sandstad, M., Shiklomanov, A. N., Skeie, R. B., Smith, C. J., Smith, S., Tanaka, K., Tsutsui, J., and Xie, Z.: Reduced Complexity Model Intercomparison Project Phase 1: introduction and evaluation of global-mean temperature response, Geosci. Model Dev., 13, 5175-5190, https://doi.org/10.5194/gmd-13-5175-2020, 2020.",
     "institution": "RCMIP",
     "hierarchical": True,
     "last_update": "2020-09-21",
     "version": "v5.1.0",
     "total_sum": True,
     "canonical_top_level_category": "Emissions",
     "categories": {
```

### Comparing `climate_categories-0.7.1/climate_categories/data/RCMIP.yaml` & `climate_categories-0.8.1/climate_categories/data/RCMIP.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   \ fuel use), hence\nwe call it MAGICC AFOLU."
 references: 'Nicholls, Z. R. J., Meinshausen, M., Lewis, J., Gieseke, R., Dommenget,
   D., Dorheim, K., Fan, C.-S., Fuglestvedt, J. S., Gasser, T., Golüke, U., Goodwin,
   P., Hartin, C., Hope, A. P., Kriegler, E., Leach, N. J., Marchegiani, D., McBride,
   L. A., Quilcaille, Y., Rogelj, J., Salawitch, R. J., Samset, B. H., Sandstad, M.,
   Shiklomanov, A. N., Skeie, R. B., Smith, C. J., Smith, S., Tanaka, K., Tsutsui,
   J., and Xie, Z.: Reduced Complexity Model Intercomparison Project Phase 1: introduction
-  and evaluation of global-mean temperature response, Geosci. Model Dev., 13, 5175–5190,
+  and evaluation of global-mean temperature response, Geosci. Model Dev., 13, 5175-5190,
   https://doi.org/10.5194/gmd-13-5175-2020, 2020.'
 institution: RCMIP
 hierarchical: true
 last_update: '2020-09-21'
 version: v5.1.0
 total_sum: true
 canonical_top_level_category: Emissions
```

### Comparing `climate_categories-0.7.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv` & `climate_categories-0.8.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/gas.py` & `climate_categories-0.8.1/climate_categories/data/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/data/gas.yaml` & `climate_categories-0.8.1/climate_categories/data/gas.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/conftest.py` & `climate_categories-0.8.1/climate_categories/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import climate_categories
 import climate_categories.tests
 import climate_categories.tests.data
 
 
 def read_cat(fragment):
     return climate_categories.from_yaml(
-        importlib.resources.open_text(
-            climate_categories.tests.data, f"{fragment}_categorization.yaml"
-        )
+        importlib.resources.files("climate_categories.tests.data")
+        .joinpath(f"{fragment}_categorization.yaml")
+        .open("r")
     )
 
 
 @pytest.fixture
 def SimpleCat():
     return read_cat("simple")
```

### Comparing `climate_categories-0.7.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml` & `climate_categories-0.8.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/data/broken_simple_categorization.yaml` & `climate_categories-0.8.1/climate_categories/tests/data/broken_simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/data/good_conversion_A.yaml` & `climate_categories-0.8.1/climate_categories/tests/data/good_conversion_A.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/data/hierarchical_categorization.yaml` & `climate_categories-0.8.1/climate_categories/tests/data/hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/data/simple_categorization.yaml` & `climate_categories-0.8.1/climate_categories/tests/data/simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/examples.py` & `climate_categories-0.8.1/climate_categories/tests/examples.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/test_climate_categories.py` & `climate_categories-0.8.1/climate_categories/tests/test_climate_categories.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,16 @@
         assert list(sorted(SimpleCat.values())) == [
             SimpleCat["1"],
             SimpleCat["2"],
             SimpleCat["3"],
             SimpleCat["unnumbered"],
         ]
 
-        assert not SimpleCat["1"] == "1"
-        assert not SimpleCat["1"] == SimpleCat["2"]
+        assert SimpleCat["1"] != "1"
+        assert SimpleCat["1"] != SimpleCat["2"]
         assert SimpleCat["1"] == SimpleCat["1"]
         ext = SimpleCat.extend(
             name="ext",
             categories={"10": {"title": "ten"}},
             alternative_codes={"yksi": "1"},
         )
         assert SimpleCat["1"] == ext["1"]
@@ -447,15 +447,15 @@
             assert key in ReRead
             assert HierCat[key] == ReRead[key]
         assert HierCat == ReRead
 
     def test_level_error(self, HierCat: climate_categories.HierarchicalCategorization):
         HierCat.canonical_top_level_category = None
         with pytest.raises(ValueError, match="Can not calculate the level"):
-            HierCat["1"].level
+            _ = HierCat["1"].level
 
     def test_parents_code(self, HierCat):
         assert HierCat.parents(HierCat["1"]) == HierCat.parents("1")
 
     def test_children_code(self, HierCat):
         assert HierCat.children(HierCat["1"]) == HierCat.children("1")
 
@@ -639,21 +639,19 @@
 
     def test_broken(self):
         with pytest.raises(
             strictyaml.YAMLValidationError,
             match="unexpected key not in schema 'reefrences'",
         ):
             climate_categories.HierarchicalCategorization.from_yaml(
-                importlib.resources.open_text(
-                    climate_categories.tests.data,
-                    "broken_hierarchical_categorization.yaml",
-                )
+                importlib.resources.files("climate_categories.tests.data")
+                .joinpath("broken_hierarchical_categorization.yaml")
+                .open()
             )
 
     def test_broken_hierarchical(self):
         with pytest.raises(ValueError, match="'hierarchical' must be "):
             climate_categories.from_yaml(
-                importlib.resources.open_text(
-                    climate_categories.tests.data,
-                    "broken_simple_categorization.yaml",
-                )
+                importlib.resources.files("climate_categories.tests.data")
+                .joinpath("broken_simple_categorization.yaml")
+                .open()
             )
```

### Comparing `climate_categories-0.7.1/climate_categories/tests/test_conversions.py` & `climate_categories-0.8.1/climate_categories/tests/test_conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,21 +123,22 @@
         assert not unrestricted.is_restricted
         assert restricted.is_restricted
 
 
 class TestConversionSpec:
     def test_good_csv(self, tmp_path):
         # write CSV resource to file to test also file opening path
-        fd = importlib.resources.open_text(
-            climate_categories.tests.data,
-            "good_conversion.csv",
+        good_csv = (
+            importlib.resources.files("climate_categories.tests.data")
+            .joinpath("good_conversion.csv")
+            .open()
         )
         temp_csv = tmp_path / "gc.csv"
         with temp_csv.open("w") as fd2:
-            fd2.write(fd.read())
+            fd2.write(good_csv.read())
 
         # Now actually read from the file
         conv = conversions.ConversionSpec.from_csv(temp_csv)
         assert conv.categorization_a_name == "A"
         assert conv.categorization_b_name == "B"
         assert conv.comment == "A correct conversion specification file"
         assert conv.version == "1.2.3.4"
@@ -237,26 +238,26 @@
         with pytest.raises(
             ValueError, match="Last column must be 'comment', but isn't."
         ):
             climate_categories._conversions.ConversionSpec.from_csv(csv)
 
 
 def load_conversion_from_csv(fname: str):
-    fd = importlib.resources.open_text(
-        climate_categories.tests.data,
-        fname,
+    fd = (
+        importlib.resources.files("climate_categories.tests.data")
+        .joinpath(fname)
+        .open()
     )
-
     gc = conversions.ConversionSpec.from_csv(fd)
 
     cats = {
         cat_name: climate_categories.Categorization.from_yaml(
-            importlib.resources.open_text(
-                climate_categories.tests.data, f"good_conversion_{cat_name}.yaml"
-            )
+            importlib.resources.files("climate_categories.tests.data")
+            .joinpath(f"good_conversion_{cat_name}.yaml")
+            .open()
         )
         for cat_name in ("A", "B", "aux1", "aux2")
     }
 
     return gc.hydrate(cats)
 
 
@@ -309,15 +310,14 @@
     def test_not_existing(self):
         with pytest.raises(
             ValueError, match="Error in line 10: 'notexisting' not in A"
         ):
             load_conversion_from_csv("broken_conversion_not_existing.csv")
 
     def test_describe(self, good_conversion: conversions.Conversion):
-
         assert (
             good_conversion.describe_detailed()
             == """# Mapping between A and B
 
 ## Simple direct mappings
 
 Only for aux1 in ['3', '4', 'A', 'argl-5'] and aux2 in ['A', 'B', 'B A']
```

### Comparing `climate_categories-0.7.1/climate_categories/tests/test_di.py` & `climate_categories-0.8.1/climate_categories/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/test_ipcc.py` & `climate_categories-0.8.1/climate_categories/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/test_overcounting.py` & `climate_categories-0.8.1/climate_categories/tests/test_overcounting.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories/tests/test_primap.py` & `climate_categories-0.8.1/climate_categories/tests/test_primap.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/climate_categories.egg-info/PKG-INFO` & `climate_categories-0.8.1/climate_categories.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: climate-categories
-Version: 0.7.1
+Version: 0.8.1
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@pik-potsdam.de
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 ==================
 Climate categories
@@ -48,14 +47,21 @@
 ===============  ==================================================================
 Name             Title
 ---------------  ------------------------------------------------------------------
 IPCC1996         IPCC GHG emission categories (1996)
 IPCC2006         IPCC GHG emission categories (2006)
 IPCC2006_PRIMAP  IPCC GHG emission categories (2006) with additional categories
 CRF1999          Common Reporting Format GHG emissions categories (1999)
+CRF2013          Common Reporting Format GHG emissions categories (2013)
+CRF2013_2021     CRF categories extended with country specific categories from
+                 2021 submissions
+CRF2013_2022     CRF categories extended with country specific categories from
+                 2022 submissions
+CRF2013_2023     CRF categories extended with country specific categories from
+                 2023 submissions
 BURDI            BUR GHG emission categories (DI query interface)
 BURDI_class      BUR GHG emission categories (DI query interface) + classifications
 CRFDI            CRF GHG emission categories (DI query interface)
 CRFDI_class      CRF GHG emission categories (DI query interface) + classifications
 GCB              Global Carbon Budget CO2 emission categories
 RCMIP            RCMIP emissions categories
 gas              Gases and other climate-forcing substances
@@ -87,22 +93,35 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2021-11-25).
-pik-primap/climate_categories: climate_categories Version 0.7.1.
-Zenodo. https://doi.org/10.5281/zenodo.5727646
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-04-26).
+pik-primap/climate_categories: climate_categories Version 0.8.1.
+Zenodo. https://doi.org/10.5281/zenodo.7867951
 
 =========
 Changelog
 =========
 
+0.8.1 (2023-04-26)
+------------------
+* regenerate data included in the package to benefit
+  from latest fixes in data generation scripts.
+
+0.8.0 (2023-04-26)
+------------------
+* Add updated CRF2013 terminologies for 2021, 2022, and 2023 submission rounds
+* The unfccc DI API recently returns unspecified measure IDs.
+  data_generation/CRFDI_class.py was fixed to ignore them.
+* Add CRF2013 terminology for data submitted by AnnexI countries to the UNFCCC
+* Drop support for Python 3.7 and 3.8, add support for Python 3.11
+
 0.7.1 (2021-11-25)
 ------------------
 * Change conversion metadata format to use comment chars and a YAML header.
 
 0.7.0 (2021-11-25)
 ------------------
 * Use Python files instead of pickle objects for caching
@@ -222,9 +241,7 @@
 * Add IPCC2006 categorization and scripts to generate it from the source pdf.
 
 0.1.0 (2021-01-18)
 ------------------
 
 * First release on PyPI.
 * Contains documentation and a stub API for querying, but no working code yet.
-
-
```

### Comparing `climate_categories-0.7.1/climate_categories.egg-info/SOURCES.txt` & `climate_categories-0.8.1/climate_categories.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -34,14 +34,22 @@
 climate_categories.egg-info/top_level.txt
 climate_categories/data/BURDI.py
 climate_categories/data/BURDI.yaml
 climate_categories/data/BURDI_class.py
 climate_categories/data/BURDI_class.yaml
 climate_categories/data/CRF1999.py
 climate_categories/data/CRF1999.yaml
+climate_categories/data/CRF2013.py
+climate_categories/data/CRF2013.yaml
+climate_categories/data/CRF2013_2021.py
+climate_categories/data/CRF2013_2021.yaml
+climate_categories/data/CRF2013_2022.py
+climate_categories/data/CRF2013_2022.yaml
+climate_categories/data/CRF2013_2023.py
+climate_categories/data/CRF2013_2023.yaml
 climate_categories/data/CRFDI.py
 climate_categories/data/CRFDI.yaml
 climate_categories/data/CRFDI_class.py
 climate_categories/data/CRFDI_class.yaml
 climate_categories/data/GCB.py
 climate_categories/data/GCB.yaml
 climate_categories/data/IPCC1996.py
@@ -57,14 +65,15 @@
 climate_categories/data/gas.py
 climate_categories/data/gas.yaml
 climate_categories/tests/__init__.py
 climate_categories/tests/conftest.py
 climate_categories/tests/examples.py
 climate_categories/tests/test_climate_categories.py
 climate_categories/tests/test_conversions.py
+climate_categories/tests/test_crf.py
 climate_categories/tests/test_di.py
 climate_categories/tests/test_gas.py
 climate_categories/tests/test_ipcc.py
 climate_categories/tests/test_overcounting.py
 climate_categories/tests/test_primap.py
 climate_categories/tests/test_rcmip.py
 climate_categories/tests/test_search.py
@@ -81,14 +90,18 @@
 climate_categories/tests/data/good_conversion_reversed.csv
 climate_categories/tests/data/hierarchical_categorization.yaml
 climate_categories/tests/data/simple_categorization.yaml
 data_generation/.gitignore
 data_generation/BURDI.py
 data_generation/BURDI_class.py
 data_generation/CRF1999.py
+data_generation/CRF2013.py
+data_generation/CRF2013_2021.py
+data_generation/CRF2013_2022.py
+data_generation/CRF2013_2023.py
 data_generation/CRFDI.py
 data_generation/CRFDI_class.py
 data_generation/IPCC1996.py
 data_generation/IPCC2006.py
 data_generation/IPCC2006_PRIMAP.py
 data_generation/RCMIP.py
 data_generation/convert_yaml_to_python.py
```

### Comparing `climate_categories-0.7.1/data_generation/BURDI.py` & `climate_categories-0.8.1/data_generation/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/data_generation/BURDI_class.py` & `climate_categories-0.8.1/data_generation/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/data_generation/CRF1999.py` & `climate_categories-0.8.1/data_generation/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/data_generation/CRFDI.py` & `climate_categories-0.8.1/data_generation/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/data_generation/CRFDI_class.py` & `climate_categories-0.8.1/data_generation/CRFDI_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Run this via `make climate_categories/data/CRFDI_class.yaml` in the main directory.
 """
 import datetime
 import pathlib
 
 import numpy as np
+import treelib
 import unfccc_di_api
 
 import climate_categories
 
 OUTPATH = pathlib.Path("./climate_categories/data/CRFDI_class.yaml")
 
 
@@ -76,15 +77,18 @@
                 ),
                 "measureId",
             ]
         )
 
         new_children_for_category = []
         for mid in sorted(measure_ids):
-            measure = rao.measure_tree[mid].tag
+            try:
+                measure = rao.measure_tree[mid].tag
+            except treelib.tree.NodeIDAbsentError:
+                continue
             if measure not in refrigerant_emission_measures:
                 continue
             short_mid = refrigerant_emission_measures[measure]
             code = f"{parent_category.codes[0]}-m{short_mid}"
             altcodes = [f"{parent_category.codes[0]}-m{mid}"]
             numerical_altcodes = [
                 f"{nid}-m{mid}" for nid in parent_category.info["numerical_ids"]
```

### Comparing `climate_categories-0.7.1/data_generation/IPCC1996.py` & `climate_categories-0.8.1/data_generation/IPCC1996.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 def combine_rows(ts):
     rows = []
     for table in ts:
         code_name_previously_empty = True
         definition_previously_empty = True
         current_code_name = None
         current_definition = None
-        for i, (code_name, definition) in table.df.iterrows():
+        for _, (code_name, definition) in table.df.iterrows():
             if (
                 code_name.startswith("Time period is an important element in")
                 or code_name.startswith("categories.  For example, the IPCC default")
                 or code_name.startswith("years for biomass decay.")
             ):
                 continue
             code_name_empty = not code_name.strip()
@@ -142,15 +142,15 @@
 
 def parse_codes(rows):
     cats_raw = []
     roman_numerals = ("i", "ii", "iii", "iv", "v", "vi", "vii")
     parent_code = ""
     parent_roman_code = ""
     running_number = 1
-    for (code_title, definition) in rows:
+    for code_title, definition in rows:
         if code_title.startswith(" 1 A 2\nb "):
             code_raw = code_title[:8]
             title = code_title[9:]
         elif code_title == " 1 A 2\ne":
             code_raw = code_title
             title = definition
             definition = ""
@@ -217,15 +217,15 @@
         cats_raw.append((code, title, definition))
 
     return cats_raw
 
 
 def parse_categories(cats_raw):
     cats = {}
-    for (code, title, definition) in cats_raw:
+    for code, title, definition in cats_raw:
         if "(" in title and "ISIC" in title and not definition:
             title, definition = title.split("(")
             definition = definition[:-1]
 
         title = title_case(" ".join(title.split()))
         definition = " ".join(definition.split()).replace("- ", "")
         if len(definition) > 2 and definition[0] == "(" and definition[-1] == ")":
@@ -246,15 +246,15 @@
         cats[code] = spec
 
     return cats
 
 
 def add_relationships(categories):
     for parent_code in categories:
-        prefix = parent_code + "."
+        prefix = f"{parent_code}."
         children = []
         for child_code in categories:
             if child_code.startswith(prefix) and "." not in child_code[len(prefix) :]:
                 children.append(child_code)
         if children:
             categories[parent_code]["children"] = [children]
 
@@ -262,15 +262,15 @@
 def main():
     download_cached(URL, INPATH)
     ts = read_pdf(INPATH)
     rows = combine_rows(ts)
     cats_raw = parse_codes(rows)
 
     # Widely used and very useful, even though not included in the official spec
-    categories: typing.Dict[str, typing.Any] = {
+    categories: dict[str, typing.Any] = {
         "0": {
             "title": "National Total",
             "comment": "All emissions and removals",
             "children": [["1", "2", "3", "4", "5", "6", "7"]],
         }
     }
```

### Comparing `climate_categories-0.7.1/data_generation/IPCC2006.py` & `climate_categories-0.8.1/data_generation/IPCC2006.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             code_parts.append(si)
         else:
             code_ended = True
             name_parts.append(si)
     return code_parts, " ".join(name_parts)
 
 
-def parse_pdfs(inpath: str) -> typing.List[typing.Tuple[str, str, str, str]]:
+def parse_pdfs(inpath: str) -> list[tuple[str, str, str, str]]:
     t = camelot.read_pdf(
         inpath,
         pages="10-33",
         flavor="stream",
         table_areas=["74,744,527,35"],
         columns=["251,468,498"],
         row_tol=3,
@@ -52,15 +52,15 @@
     )
     cats_raw = []
     full_code_name = None
     full_definition = None
     full_code_96 = None
     full_gases = None
     for table in itertools.chain(t, tend):
-        for i, row in table.df.iterrows():
+        for _, row in table.df.iterrows():
             code_name, definition, code_96, gases = row
             if code_name and code_name[0].isnumeric():
                 # store current and start new category
                 if full_gases is not None:
                     cats_raw.append(
                         (full_code_name, full_definition, full_code_96, full_gases)
                     )
@@ -80,16 +80,16 @@
                     full_gases = f"{full_gases}{gases}"
                 else:
                     full_gases = f"{full_gases} {gases}"
     cats_raw.append((full_code_name, full_definition, full_code_96, full_gases))
     return cats_raw
 
 
-def parse_categories(cats_raw) -> typing.Dict[str, typing.Any]:
-    categories: typing.Dict[str, typing.Any] = {}
+def parse_categories(cats_raw) -> dict[str, typing.Any]:
+    categories: dict[str, typing.Any] = {}
     for code_name, definition, code_96, gases in cats_raw:
         code_parts, title = split_code_name(code_name)
         # error in pdf
         if code_parts == ["1", "B", "2", "a", "iii", "I"]:
             code_parts = ["1", "B", "2", "a", "iii", "1"]
         code = ".".join(code_parts)
         altcode = "".join(code_parts)
@@ -135,15 +135,15 @@
 
 
 def main():
     download_cached(URL, INPATH)
     cats_raw = parse_pdfs(str(INPATH))
 
     # Widely used and very useful, even though not included in the official spec
-    categories: typing.Dict[str, typing.Any] = {
+    categories: dict[str, typing.Any] = {
         "0": {
             "title": "National Total",
             "comment": "All emissions and removals",
             "children": [["1", "2", "3", "4", "5"]],
         }
     }
```

### Comparing `climate_categories-0.7.1/data_generation/IPCC2006_PRIMAP.py` & `climate_categories-0.8.1/data_generation/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/data_generation/RCMIP.py` & `climate_categories-0.8.1/data_generation/RCMIP.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
     categories = {}
 
     categories["Emissions"] = {"title": "RCMIP Emissions", "children": [[]]}
 
     definitions = pd.read_excel(INPATH, sheet_name="variable_definitions")
 
     for _, item in definitions[definitions.Category == "Emissions"].iterrows():
-
         species = item.Variable
         print(species)
         parent = item.Variable.rsplit("|", maxsplit=1)[0]
         print(parent)
         item_comment = item.Definition.replace(
             "(please provide a definition of other sources in this category in the "
             "'comments' tab)",
@@ -160,15 +159,15 @@
             "Dommenget, D., Dorheim, K., Fan, C.-S., Fuglestvedt, J. S., Gasser, T., "
             "Golüke, U., Goodwin, P., Hartin, C., Hope, A. P., Kriegler, E., Leach, "
             "N. J., Marchegiani, D., McBride, L. A., Quilcaille, Y., Rogelj, J., "
             "Salawitch, R. J., Samset, B. H., Sandstad, M., Shiklomanov, A. N., "
             "Skeie, R. B., Smith, C. J., Smith, S., Tanaka, K., Tsutsui, J., "
             "and Xie, Z.: Reduced Complexity Model Intercomparison Project Phase 1:"
             " introduction and evaluation of global-mean temperature response, "
-            "Geosci. Model Dev., 13, 5175–5190, "
+            "Geosci. Model Dev., 13, 5175-5190, "
             "https://doi.org/10.5194/gmd-13-5175-2020, 2020."
         ),
         "institution": "RCMIP",
         "last_update": "2020-09-21",
         "hierarchical": True,
         "version": "v5.1.0",
         "total_sum": True,
```

### Comparing `climate_categories-0.7.1/data_generation/gas.py` & `climate_categories-0.8.1/data_generation/gas.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,15 @@
 
 
 def openscm_mixtures():
     categories = {}
     m = openscm_units.data.mixtures.MIXTURES
 
     for code, constituents in m.items():
-        cstr = ", ".join(
-            (f"{constituents[const][0]}% {const}" for const in constituents)
-        )
+        cstr = ", ".join(f"{constituents[const][0]}% {const}" for const in constituents)
         categories[code] = {
             "title": code,
             "comment": f"The refrigerant {code}, which is a mixture " f"of {cstr}.",
         }
 
     categories["mixtures"] = {
         "title": "refrigerant mixtures",
@@ -62,15 +60,15 @@
 
 
 def openscm_standard_gases():
     categories = {}
     # This is not public API, will have to fix it when openscm_units changes
     sg = openscm_units._unit_registry._STANDARD_GASES
 
-    for (oscm_gas_code, oscm_gas_spec) in sg.items():
+    for oscm_gas_code, oscm_gas_spec in sg.items():
         if isinstance(oscm_gas_spec, str):  # base entity
             code = oscm_gas_code
             title = oscm_gas_spec.replace("_", " ")
             categories[code] = {
                 "title": title,
             }
             if code != oscm_gas_spec and " " not in oscm_gas_spec:
```

### Comparing `climate_categories-0.7.1/data_generation/utils.py` & `climate_categories-0.8.1/data_generation/utils.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/docs/Makefile` & `climate_categories-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/docs/conf.py` & `climate_categories-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/docs/data.rst` & `climate_categories-0.8.1/docs/data.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/docs/installation.rst` & `climate_categories-0.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/docs/make.bat` & `climate_categories-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/docs/usage.ipynb` & `climate_categories-0.8.1/docs/usage.ipynb`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/setup.cfg` & `climate_categories-0.8.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climate_categories
-version = 0.7.1
+version = 0.8.1
 author = Mika Pflüger
 author_email = mika.pflueger@pik-potsdam.de
 description = Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/climate_categories
 project_urls = 
@@ -12,77 +12,72 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 license = Apache Software License 2.0
 license_file = LICENSE
 
 [options]
 packages = 
 	climate_categories
 	climate_categories.data
 	climate_categories.tests
 	climate_categories.tests.data
-python_requires = >=3.7
+python_requires = >=3.9
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	networkx
 	pandas
 	strictyaml
 	natsort
 	ruamel.yaml
 	pyparsing
+	immutables
 	black
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	xdoctest
 dev = 
 	pip
 	tbump
 	wheel
 	build
-	flake8
+	ruff
 	coverage
 	Sphinx
 	twine
 	pytest
 	pre-commit
 	sphinx_rtd_theme
 	ipykernel
 	nbsphinx
 	networkx
 	xdoctest
-	camelot-py[plot,cv]
+	camelot-py[plot] >= 0.11.0
 	tox
-	unfccc_di_api
+	unfccc_di_api >= 3.0.1
 	pygments-csv-lexer
 	openscm-units
+	black
 
 [options.package_data]
 * = 
 	*.yaml
 	*.csv
 
-[flake8]
-exclude = 
-	docs
-	climate_categories/data/*.py
-max-line-length = 88
-extend-ignore = E203, W503
-
 [doc8]
 max-line-length = 88
 ignore-path-errors = docs/data.rst;D001
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `climate_categories-0.7.1/tbump.toml` & `climate_categories-0.8.1/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/climate_categories/"
 
 [version]
-current = "0.7.1"
+current = "0.8.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `climate_categories-0.7.1/update_changelog.py` & `climate_categories-0.8.1/update_changelog.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.7.1/update_citation_info.py` & `climate_categories-0.8.1/update_citation_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 If you use this library and want to cite it, please cite it as:
 
 Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. ({new_date}).
 {new_title}.
 Zenodo. {new_link}
 """
 
-with open("README.rst", "r") as fd:
+with open("README.rst") as fd:
     old_content = fd.read().splitlines(keepends=True)
 
 with open("README.rst", "w") as fd:
     skip_to_next_section = False
     i = 0
     while True:
         try:
```

