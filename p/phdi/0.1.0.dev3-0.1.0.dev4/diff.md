# Comparing `tmp/phdi-0.1.0.dev3.tar.gz` & `tmp/phdi-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-0.1.0.dev3.tar", max compression
+gzip compressed data, was "phdi-0.1.0.dev4.tar", max compression
```

## Comparing `phdi-0.1.0.dev3.tar` & `phdi-0.1.0.dev4.tar`

### file list

```diff
@@ -1,54 +1,68 @@
--rw-r--r--   0        0        0     7048 2022-07-27 10:50:01.771632 phdi-0.1.0.dev3/LICENSE.md
--rw-r--r--   0        0        0     8741 2022-10-06 21:54:13.403270 phdi-0.1.0.dev3/README.md
--rw-r--r--   0        0        0       27 2022-10-06 22:06:38.445374 phdi-0.1.0.dev3/phdi/__init__.py
--rw-r--r--   0        0        0      223 2022-09-14 18:15:47.189114 phdi-0.1.0.dev3/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2022-08-31 21:43:21.734173 phdi-0.1.0.dev3/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     7871 2022-10-06 22:03:11.746293 phdi-0.1.0.dev3/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/cloud/core.py
--rw-r--r--   0        0        0     5766 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/cloud/gcp.py
--rw-r--r--   0        0        0        0 2022-09-01 15:01:27.448486 phdi-0.1.0.dev3/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2022-09-14 18:15:47.189114 phdi-0.1.0.dev3/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2022-08-31 21:43:21.735173 phdi-0.1.0.dev3/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2022-09-14 18:15:47.190114 phdi-0.1.0.dev3/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2022-08-31 21:43:21.735173 phdi-0.1.0.dev3/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     6934 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2022-09-14 18:15:47.190114 phdi-0.1.0.dev3/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3508 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2022-08-31 21:43:21.735173 phdi-0.1.0.dev3/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      158 2022-08-31 21:43:21.735173 phdi-0.1.0.dev3/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0     6520 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2022-09-14 18:15:47.190114 phdi-0.1.0.dev3/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2022-09-14 18:15:47.190114 phdi-0.1.0.dev3/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      235 2022-08-31 21:43:21.736173 phdi-0.1.0.dev3/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0     6787 2022-10-06 22:03:11.747293 phdi-0.1.0.dev3/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2022-09-14 18:15:47.190114 phdi-0.1.0.dev3/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2022-08-31 21:43:21.736173 phdi-0.1.0.dev3/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7384 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     6822 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     3816 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2022-09-14 18:15:47.191114 phdi-0.1.0.dev3/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2022-10-05 13:04:20.797257 phdi-0.1.0.dev3/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5917 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2022-08-31 21:43:21.736173 phdi-0.1.0.dev3/phdi/harmonization/README.md
--rw-r--r--   0        0        0      587 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    10909 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0     6718 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0      255 2022-08-31 21:43:21.737173 phdi-0.1.0.dev3/phdi/linkage/README.md
--rw-r--r--   0        0        0       69 2022-08-31 21:43:21.737173 phdi-0.1.0.dev3/phdi/linkage/__init__.py
--rw-r--r--   0        0        0      763 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/linkage/link.py
--rw-r--r--   0        0        0      286 2022-09-14 18:15:47.191114 phdi-0.1.0.dev3/phdi/tabulation/README.md
--rw-r--r--   0        0        0      148 2022-08-31 21:43:21.737173 phdi-0.1.0.dev3/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0     3948 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/tabulation/tables.py
--rw-r--r--   0        0        0      225 2022-09-14 18:15:47.191114 phdi-0.1.0.dev3/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2022-08-31 21:43:21.737173 phdi-0.1.0.dev3/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2299 2022-10-06 22:03:11.748293 phdi-0.1.0.dev3/phdi/transport/http.py
--rw-r--r--   0        0        0     1183 2022-10-06 22:06:46.330414 phdi-0.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0    10324 2022-10-06 22:06:48.965523 phdi-0.1.0.dev3/setup.py
--rw-r--r--   0        0        0    10025 2022-10-06 22:06:48.965943 phdi-0.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-04-26 17:41:55.912057 phdi-0.1.0.dev4/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-04-26 17:41:55.912057 phdi-0.1.0.dev4/README.md
+-rw-r--r--   0        0        0       27 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     8647 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2150 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3587 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     6822 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5911 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     1948 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     2288 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/core.py
+-rw-r--r--   0        0        0    56895 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/link.py
+-rw-r--r--   0        0        0    10945 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2667 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11839 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2881 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1449 2023-04-26 17:41:56.400037 phdi-0.1.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0    13606 1970-01-01 00:00:00.000000 phdi-0.1.0.dev4/PKG-INFO
```

### Comparing `phdi-0.1.0.dev3/LICENSE.md` & `phdi-0.1.0.dev4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/README.md` & `phdi-0.1.0.dev4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,116 @@
-# PRIME Public Health Data Infrastructure
+# PRIME Public Health Data Infrastructure (PHDI)
 [![Test github badge](https://github.com/CDCgov/phdi/actions/workflows/test.yaml/badge.svg)](https://github.com/CDCgov/phdi/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/CDCgov/phdi/branch/main/graph/badge.svg)](https://codecov.io/gh/CDCgov/phdi)
 - [PRIME Public Health Data Infrastructure](#prime-public-health-data-infrastructure)
-  - [Getting Started](#getting-started)
-    - [How to import PHDI](#how-to-import-phdi)
   - [Overview](#overview)
     - [Problem Scope](#problem-scope)
+  - [Getting Started](#getting-started)
+  - [Main Features](#main-features)
+  - [Where to Get PHDI](#where-to-get-phdi)
+  - [Documentation](#documentation)
   - [Standard Notices](#standard-notices)
     - [Public Domain Standard Notice](#public-domain-standard-notice)
     - [License Standard Notice](#license-standard-notice)
     - [Privacy Standard Notice](#privacy-standard-notice)
     - [Contributing Standard Notice](#contributing-standard-notice)
     - [Records Management Standard Notice](#records-management-standard-notice)
     - [Related documents](#related-documents)
     - [Additional Standard Notices](#additional-standard-notices)
 
 **General disclaimer** This repository was created for use by CDC programs to collaborate on public health related projects in support of the [CDC mission](https://www.cdc.gov/about/organization/mission.htm). GitHub is not hosted by the CDC, but is a third party website used by CDC and its partners to share information and collaborate on software. CDC use of GitHub does not imply an endorsement of any one particular service, product, or enterprise.
 
-## Getting Started
+## Overview
+
+This repository is a part of the CDC/USDS [PHDI project](https://cdcgov.github.io/phdi-site/) and has two components: 
+1. PHDI Python Package
+2. PHDI containerized Building Blocks 
+
+The PHDI Python package contains source code for a platform to help public health authorities (PHAs) ingest and report on public health data. This platform is composed of **Building Blocks**, which are modular software tools that, when composed together, can improve data quality and reduce data cleaning workloads by providing analysis-ready data to downstream public health surveillance systems and other analytical and reporting applications. 
+
+PHDI contains: 
+- Our SDK — the Python library containing Building Block source code
+  - [Repository](https://github.com/CDCgov/phdi/tree/main/phdi)
+  - [API documentation](https://cdcgov.github.io/phdi/sdk/phdi.html)
+- Containerized web services exposing Building Block functionality as HTTP endpoints
+  - [Repository](https://github.com/CDCgov/phdi/tree/main/containers)
+  - [User guide](https://cdcgov.github.io/phdi/) (under Building Blocks)
+- Cloud Starter Kit — Repositories that implement a complete cloud-based pipeline composed of Building Blocks
+  - [Azure](https://github.com/CDCgov/phdi-azure)
+  - [Google Cloud Platform](https://github.com/CDCgov/phdi-google-cloud)
 
-In order to use the PHDI Building Blocks library, you need [Python 3.9 or higher](https://www.python.org/downloads/) and [pip python package manager](https://pip.pypa.io/en/stable/installation/) (or any python package manager)
+### Problem Scope
+
+Current public health systems that digest, analyze, and respond to data are siloed. Lacking access to actionable data, our national, as well as state, local, and territorial infrastructure, isn’t pandemic-ready. Our objective is to help the CDC best support PHAs in moving towards a modern public health data infrastructure. See our [public website](https://cdcgov.github.io/phdi-site/) for more details.
+
+PHDI is a sibling project to [PRIME ReportStream](https://reportstream.cdc.gov), which focuses on improving the delivery of COVID-19 test data to public health departments, and [PRIME SimpleReport](https://simplereport.gov), which provides a better way for organizations and testing facilities to report COVID-19 rapid tests to public health departments.
+
+## Getting Started
 
+In order to use the PHDI library, you need [Python 3.9 or higher](https://www.python.org/downloads/) and [pip python package manager](https://pip.pypa.io/en/stable/installation/) (or any python package manager).
 
 To install using pip:
 ```
 pip install phdi
 ```
 
-### How to import PHDI
+## Main Features
 
-Our project is split up into two parts. Our FHIR supporting version and our generic version.
+Here are the current tools that PHDI offers:
+- **Containerized Building Blocks**
+  -   **[Alerts](https://cdcgov.github.io/phdi/containers/alerts.html)** - Provides the ability to send alerts via SMS, Slack, or Microsoft Teams
+  -   **[FHIR Converter](https://cdcgov.github.io/phdi/containers/fhir-converter.html)** - Enables conversion of health data from legacy formats (e.g., HL7 version 2, CCDA) to [FHIR](https://hl7.org/FHIR/), a standard for health care data exchange
+  -   **[Data Ingestion](https://cdcgov.github.io/phdi/containers/ingestion.html)** - Includes the entire pipeline of Building Blocks below
+      -  **[Harmonization](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirharmonization)** - Standardizes input data (e.g., patient names and phone numbers) to streamline the process of cleaning data and improve data quality
+      - **[Geospatial](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirgeospatial)** - Provides a common interface for obtaining precise geographic locations based on street addresses from input data
+      - **[Linkage](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirlinkage)** - Assigns a common identifier to patient records in order to link and deduplicate patient records seen across data contributors
+      - **[Transport](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirtransport)** - Offers functionality for reading and writing data from storage resources (e.g,. FHIR servers)  
+  -   **[Message Parser](https://cdcgov.github.io/phdi/containers/message_parser.html)** - Extracts desired fields from a given message
+  -   **[Tabulation](https://cdcgov.github.io/phdi/containers/tabulation.html)** - Extracts data from a FHIR server, converts it to a tabular representation, and stores it to a user-defined tabular storage file type (e.g., Parquet or CSV)
+  -   **[Record Linkage](https://cdcgov.github.io/phdi/containers/record_linkage.html)** - Links new health care messages to existing records if a connection exists
+  -   **[Validation](https://cdcgov.github.io/phdi/containers/validation.html)** - Checks whether health care messages are in the proper format and contain user-defined fields of interest 
+- **Implementation Support** - Resources to help users implement PHDI tools to manage their data and analysis workflows
+  - **[Examples](https://github.com/CDCgov/phdi/tree/main/examples)** - Sample data that simulates how a Building Block could be used 
+  - **[Tutorials](https://github.com/CDCgov/phdi/tree/main/tutorials)** - Step-by-step instructions to implement Building Blocks source code
 
-Example import for FHIR:
+## Where to Get PHDI 
+
+The source code is hosted on GitHub at: https://github.com/CDCgov/phdi.
+
+The latest released version is available at the [Python Package Index (PyPI)](https://pypi.org/project/phdi/).
+
+**Python modules**
 ```
- from phdi.fhir.geospatial.census import CensusFhirGeocodeClient
+pip install phdi
 ```
 
-Example import for generic:
+**Containerized services**
 ```
- from phdi.geospatial.census import CensusGeocodeClient
+build from source
+build Docker locally
+pull down Docker images from GitHub
 ```
 
-Every building block has a FHIR counterpart that works well with FHIR bundles as inputs. The generic version is used for all other non-FHIR inputs.
+## Documentation
 
-For further information on the tutorial: [Geospatial Tutorial](tutorials/geospatial-tutorial.md)
+PHDI documentation is currently hosted on GitHub Pages: https://cdcgov.github.io/phdi/ 
 
-## Overview
+There, you can find our: 
+- SDK API reference documentation
+- User guide for containerized Building Blocks
 
-The PRIME Public Health Data Infrastructure projects are part of the Pandemic-Ready Interoperability Modernization Effort, a multi-year collaboration between CDC and the U.S. Digital Service (USDS) to strengthen data quality and information technology systems in state and local health departments.
+## Additional Acknowledgments 
 
-This repository contains source code for a platform to help state, tribal, local and territorial (STLT) public health departments ingest and report on public health data.  It contains the following components:
-
-- **Data Ingestion** - Data ingestion tools provide a common framework to prepare data for storage, and store the data in a common standard data model ([FHIR](https://hl7.org/FHIR/)). 
-  - __Harmonization__ - Data harmonization tools can operate on raw input data (HL7 version 2, CCDA) and convert to the common data model format (FHIR).
-  - __Geospatial__ - Geospatial tools provide a common interface for obtaining precise geographic locations based on street addresses from input data.
-  - __Linkage__ - Linkage tools assign a common identifier to patient records to link and deduplicate patients seen across data contributors.
-  - __Transport__ - Transport tools provide a mechanism to store and interact with data stored to a central repostory (FHIR server). 
-- **Reporting** - Reporting tools define a dynamic framework for building custom data models in an analysis-ready output format.
-  - __Tabluation__ - Tabulation provides tools to retrieve data dynamically-defined records and data fields from the common data platform (FHIR server), extract, convert it to a tabular representation, and store to a user-defined tabular storage file type (Parquet or CSV).
-- **Implementation Support** - Implemetnation resources support implementing STLTs to configure a PHDI-driven workflow to manage their data and analysis workflows.
-  - __Cloud-agnostic tools__ - A common PHDI programming interface supports STLTs interacting with cloud-based data storage (containers/buckets), and FHIR servers in a common way.
-  - __Examples and Tutorials__ - Example and tutorial materials help STLTs implement the PHDI solution more quickly by providing easy-to-follow examples and tutorials.
-
-The PRIME Public Health Data Infrastructure prototype a sibling project to [PRIME ReportStream](https://reportstream.cdc.gov), focusing on delivering COVID-19 test data to public health departments, and [PRIME SimpleReport](https://simplereport.gov), working on a better way to report COVID-19 rapid tests.
-
-### Problem Scope
+We mapped the rootnames of the PHDI database to nicknames produced by the aggregation and synthesis of open source work from a number of projects. While we do not employ the packages and wrappers used by the various projects (merely their open source data), we wish to give credit to their various works building collections of nickname mappings. These projects are:
 
-Long-term Vision: Current public health systems to digest, analyze, and respond to data are siloed. Lacking access to actionable data, our national, as well as state, local, and territorial infrastructure, isn’t pandemic-ready. Our objective is to help the CDC best support STLTs in moving towards a modern public health data infrastructure.
+* [Secure Enterprise Master Patient Index](https://github.com/MrCsabaToth/SOEMPI), based on OpenEMPI, conducted by Vanderbilt University
+* [Curated Nicknames](https://github.com/carltonnorthern/nicknames), scraped from genealogy webpages and run by Old Dominion University Web Science and Digital Libraries Research Group
+* [Simple Public Domain Nickname Mappings](https://github.com/onyxrev/common_nickname_csv), hand collected using various sources
+* [Lingua En Nickname](https://github.com/brianary/Lingua-EN-Nickname), collected from a series of GenWeb projects
+* [diminutives.db](https://github.com/HaJongler/diminutives.db), compiled via a nickname extract using Wikipedia and Wiktionary
 
 ## Standard Notices
 
 ### Public Domain Standard Notice
 
 This repository constitutes a work of the United States Government and is not
 subject to domestic copyright protection under 17 USC § 105. This repository is in
```

### Comparing `phdi-0.1.0.dev3/phdi/cloud/azure.py` & `phdi-0.1.0.dev4/phdi/cloud/azure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 from phdi.cloud.core import BaseCredentialManager, BaseCloudStorageConnection
 from azure.core.credentials import AccessToken
+from azure.keyvault.secrets import SecretClient
 from azure.identity import DefaultAzureCredential
 from azure.storage.blob import ContainerClient, BlobServiceClient
 from datetime import datetime, timezone
 from typing import List, Union
 
 
 class AzureCredentialManager(BaseCredentialManager):
@@ -21,15 +22,15 @@
     def scope(self) -> str:
         return self.__scope
 
     @property
     def access_token(self) -> AccessToken:
         return self.__access_token
 
-    def __init__(self, resource_location: str, scope: str = None):
+    def __init__(self, resource_location: str = None, scope: str = None):
         """
         Creates a new AzureCredentialManager object.
 
         :param resource_location: The URL or other location of the requested resource.
         :param scope: A space-delimited list of scopes to limit access to resource.
           Default: `None`
         """
@@ -75,14 +76,31 @@
         try:
             current_time_utc = datetime.now(timezone.utc).timestamp()
             return self.access_token.expires_on < current_time_utc
         except AttributeError:
             # access_token not set
             return True
 
+    def get_secret(self, secret_name: str, key_vault_name: str) -> str:
+        """
+        Get the value of a secret from an Azure key vault given the names of the vault
+        and the secret.
+
+        :param secret_name: The name of the secret whose value should be retrieved from
+            the key vault.
+        :param key_vault_name: The name of the key vault where the secret is stored.
+        :return: The value of the secret specified by secret_name.
+        """
+
+        vault_url = f"https://{key_vault_name}.vault.azure.net"
+        secret_client = SecretClient(
+            vault_url=vault_url, credential=self.get_credential_object()
+        )
+        return secret_client.get_secret(secret_name).value
+
 
 class AzureCloudContainerConnection(BaseCloudStorageConnection):
     """
     Defines a connection used for interacting with cloud storage in Azure.
     """
 
     @property
```

### Comparing `phdi-0.1.0.dev3/phdi/cloud/core.py` & `phdi-0.1.0.dev4/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/cloud/gcp.py` & `phdi-0.1.0.dev4/phdi/cloud/gcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List
+from typing import List, Union
+import json
 from .core import BaseCredentialManager, BaseCloudStorageConnection
 import google.auth
 import google.auth.transport.requests
 from google.auth.credentials import Credentials
 from google.cloud import storage
 
 
@@ -90,14 +91,21 @@
     Defines a connection used for interacting with cloud storage in GCP.
     """
 
     @property
     def storage_client(self) -> storage.Client:
         return self.__storage_client
 
+    def __init__(self):
+        """
+        Creates a new GcpCloudContainerConnection object.
+        """
+
+        self.__storage_client = None
+
     def _get_storage_client(self) -> storage.Client:
         """
         Obtains a client connected to an GCP storage container by
         utilizing the first valid credentials GCP can find. Credential validation
         is handeled by GCP.
 
         :return: The GCP storage client.
@@ -121,33 +129,37 @@
         """
         storage_client = self._get_storage_client()
         blob = storage_client.bucket(container_name).blob(filename)
         return blob.download_as_text(encoding=encoding)
 
     def upload_object(
         self,
-        message: str,
+        message: Union[str, dict],
         container_name: str,
         filename: str,
         content_type="application/json",
     ) -> None:
         """
         Uploads the content of a given message to GCP blob storage.
         The message can be passed either as a raw string or as JSON.
 
         :param message: The contents of a message, encoded either as a
-          string or in a JSON format.
+          string or in a JSON-formatted dictionary.
         :param container_name: The name of the target bucket for upload.
         :param filename: The location of file within GCP blob storage.
         """
 
         storage_client = self._get_storage_client()
         bucket = storage_client.bucket(container_name)
 
         blob = bucket.blob(filename)
+
+        if isinstance(message, dict):
+            message = json.dumps(message).encode("utf-8")
+
         blob.upload_from_string(data=message, content_type=content_type)
 
     def list_containers(self) -> List[str]:
         """
         Lists bucket names in storage.
 
         :return: A list of bucket names in storage.
```

### Comparing `phdi-0.1.0.dev3/phdi/fhir/cloud/azure.py` & `phdi-0.1.0.dev4/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/fhir/conversion/convert.py` & `phdi-0.1.0.dev4/phdi/fhir/conversion/convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import hl7
+import requests
 
 import xml.etree.ElementTree as et
 
 from phdi.harmonization import standardize_hl7_datetimes
 from phdi.cloud.core import BaseCredentialManager
 from phdi.fhir.transport import http_request_with_reauth
+from phdi.transport.http import http_request_with_retry
 
 
 CCDA_CODES_TO_CONVERSION_RESOURCE = {
     "34133-9": "CCD",
     "11488-4": "ConsultationNote",
     "18842-5": "DischargeSummary",
     "34117-2": "HistoryandPhysical",
@@ -18,79 +20,85 @@
     "57133-1": "ReferralNote",
     "18761-7": "TransferSummary",
 }
 
 
 def convert_to_fhir(
     message: str,
-    cred_manager: BaseCredentialManager,
-    fhir_url: str,
+    url: str,
+    cred_manager: BaseCredentialManager = None,
+    headers: dict = {},
     use_default_ccda=False,
 ):
     """
-    Converts a given message from either HL7v2 (pipe-delimited flat file) or CCDA (XML)
+    Converts a given message from either HL7 v2 (pipe-delimited flat file) or CCDA (XML)
     into FHIR format (JSON) for further processing using the FHIR server. Standardizes
     datetimes in HL7v2 messages before conversion.
 
-    The FHIR server may respond with a status code of 400 if the
-    message itself is invalid, such as containing improperly
-    formatted data. Otherwise, the FHIR server will respond
-    with a status code of 200 along with the converted FHIR data.
-
-    :param message: The raw message that needs to be converted to FHIR.
-      Must be HL7v2 or CCDA.
-    :param cred_manager: The credential manager used to authenticate to the FHIR server.
-    :param fhir_url: A URL that points to the location of the FHIR server.
-    :param use_default_ccda: If true, default to the base "CCD" template
-      if a resources's LOINC code doesn't map to a specific supported template.
-      Default: `False`
-    :return: A `requests.Response` object containing the response from
-      the FHIR converter.
+    This function uses a containerized version of the
+    [Azure FHIR Converter](https://github.com/microsoft/FHIR-Converter).
+
+    If conversion succeeds, a `requests.Response` object will be returned with the
+    conversion response. Otherwise, a `ConversionError` is raised, with the
+    `requests.Response` available as a property for troubleshooting and reporting
+    purposes.
+
+    :param message: The raw message that needs to be converted to
+      FHIR. Currently, only HL7v2 or CCDA are supported.
+    :param url: A URL that points to the location of the converter API.
+    :param cred_manager: Service used to get an access token used to
+      make a request.
+    :param headers: JSON-type dictionary of headers to make the request with.
+    :param use_default_ccda: Whether to default to the
+      base "CCD" root template if a resource's LOINC code doesn't
+      map to a specific supported template (Optional, default is No)
+    :raises requests.HttpError: If the HTTP request was unsuccessful.
+    :raises ConversionError: If the message could not be converted.
+    :return: A requests.Response object
 
     """
+    # TODO Update documentation with a link to the containerized FHIR converter, once
+    # it's been ported over to the phdi repository.
+
     conversion_settings = _get_fhir_conversion_settings(message, use_default_ccda)
-    if conversion_settings.get("input_data_type") == "HL7v2":
+    if conversion_settings.get("input_type") == "hl7v2":
         message = standardize_hl7_datetimes(message)
 
-    url = f"{fhir_url}/$convert-data"
+    url = f"{url}"
     data = {
-        "resourceType": "Parameters",
-        "parameter": [
-            {"name": "inputData", "valueString": message},
-            {
-                "name": "inputDataType",
-                "valueString": conversion_settings.get("input_data_type"),
-            },
-            {
-                "name": "templateCollectionReference",
-                "valueString": conversion_settings.get("template_collection"),
-            },
-            {
-                "name": "rootTemplate",
-                "valueString": conversion_settings.get("root_template"),
-            },
-        ],
+        "input_data": message,
+        "input_type": conversion_settings.get("input_type"),
+        "root_template": conversion_settings.get("root_template"),
     }
-    access_token = cred_manager.get_access_token().token
-    headers = {"Authorization": f"Bearer {access_token}"}
 
-    response = http_request_with_reauth(
-        cred_manager=cred_manager,
-        url=url,
-        retry_count=3,
-        request_type="POST",
-        allowed_methods=["POST"],
-        headers=headers,
-        data=data,
-    )
+    if cred_manager:
+        access_token = cred_manager.get_access_token()
+        headers["Authorization"] = f"Bearer {access_token}"
+        response = http_request_with_reauth(
+            cred_manager=cred_manager,
+            url=url,
+            retry_count=3,
+            request_type="POST",
+            allowed_methods=["POST"],
+            headers=headers,
+            data=data,
+        )
+    else:
+        response = http_request_with_retry(
+            url=url,
+            retry_count=3,
+            request_type="POST",
+            allowed_methods=["POST"],
+            headers=headers,
+            data=data,
+        )
 
     if response.status_code != 200:
-        raise Exception(
-            f"HTTP {str(response.status_code)} code encountered in $convert-data for a message"  # noqa
-        )
+        raise ConversionError(response)
+
     return response
 
 
 def _get_fhir_conversion_settings(message: str, use_default_ccda=False) -> dict:
     """
     Determines which settings to use with the FHIR server to facilitate message
     conversion by attempting to identify which data type the input has (HL7 or XML)
@@ -103,14 +111,15 @@
 
     https://docs.microsoft.com/en-us/azure/healthcare-apis/azure-api-for-fhir/convert-data
 
     :param message: The incoming message.
     :param use_default_ccda: Whether to default to the
       base "CCD" root template if a resource's LOINC code doesn't
       map to a specific supported template. Default: `False`
+    :raises ConversionError: If conversion settings cannot be derived.
     :return: A dictionary holding the settings of parameters to-be
       set when converting the input to FHIR.
     """
     # Some streams (e.g. ELR, VXU) are HL7v2 encoded
     if message[:3] == "MSH":
         parsed_msg = hl7.parse(message)
         extracted_code = str(parsed_msg.segment("MSH")[9])
@@ -124,20 +133,19 @@
             formatted_code = extracted_code_tokenized[2]
         elif len(extracted_code_tokenized) == 2:
             formatted_code = (
                 f"{extracted_code_tokenized[0]}_{extracted_code_tokenized[1]}"
             )
 
         if formatted_code == "":
-            raise Exception("Could not determine HL7 message structure")
+            raise ConversionError(message="Could not determine HL7 message structure")
 
         return {
             "root_template": formatted_code,
-            "input_data_type": "HL7v2",
-            "template_collection": "microsofthealth/fhirconverter:default",
+            "input_type": "hl7v2",
         }
 
     # Others conform to C-CDA standards (e.g. ECR)
     else:
         try:
             root = et.fromstring(message)
 
@@ -152,26 +160,56 @@
                         break
                 ccda_code = child.attrib.get("code")
 
                 try:
                     root_template = CCDA_CODES_TO_CONVERSION_RESOURCE[ccda_code]
                     return {
                         "root_template": root_template,
-                        "input_data_type": "Ccda",
-                        "template_collection": "microsofthealth/ccdatemplates:default",
+                        "input_type": "ccda",
                     }
                 except KeyError:
                     if use_default_ccda:
                         return {
                             "root_template": "CCD",
-                            "input_data_type": "Ccda",
-                            "template_collection": "microsofthealth/ccdatemplates:default",  # noqa
+                            "input_type": "ccda",
                         }
                     else:
                         raise KeyError(
                             "Resource code does not match any provided input template"
                         )
 
-        except et.ParseError:
-            raise Exception(
-                "Input message has unrecognized data type, should be HL7v2 or XML"
+        except et.ParseError as ex:
+            raise ConversionError(
+                message=(
+                    "Input message has unrecognized data type, "
+                    + "should be HL7v2 or XML."
+                )
+            ) from ex
+
+
+class ConversionError(Exception):
+    """
+    Exception raised for errors that occur during conversion.
+    """
+
+    @property
+    def http_response(self):
+        return self.__http_response
+
+    def __init__(self, http_response: requests.Response = None, message: str = None):
+        """
+        Creates a new ConversionError object.
+
+        :param http_response: HTTP response returned by the converter service.
+          Default: `None`
+        :param message: Error message. Default: `None`
+        """
+        self.__http_response = http_response
+
+        if (message is None) and not (http_response is None):
+            message = (
+                "Conversion exception occurred with status code"
+                + f" {http_response.status_code} returned from the converter service."
             )
+        self.message = message
+
+        super().__init__(self.message)
```

### Comparing `phdi-0.1.0.dev3/phdi/fhir/geospatial/README.md` & `phdi-0.1.0.dev4/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/fhir/geospatial/census.py` & `phdi-0.1.0.dev4/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/fhir/geospatial/core.py` & `phdi-0.1.0.dev4/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/fhir/geospatial/smarty.py` & `phdi-0.1.0.dev4/phdi/fhir/geospatial/smarty.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     """
     Implementation of a geocoding client designed to handle FHIR-
     formatted data using the SmartyStreets API.
     Requires an authorization ID as well as an authentication token
     in order to build a street lookup client.
     """
 
-    def __init__(self, auth_id, auth_token):
-        self.__client = SmartyGeocodeClient(auth_id, auth_token)
+    def __init__(
+        self, auth_id: str, auth_token: str, licenses: list[str] = ["us-standard-cloud"]
+    ):
+        self.__client = SmartyGeocodeClient(auth_id, auth_token, licenses)
 
     @property
     def geocode_client(self) -> us_street.Client:
         """
         An instance of the underlying Smarty client.
         Allows the FHIR wrapper to access a SmartyStreets-
         specific connection client without instantiating its own
```

### Comparing `phdi-0.1.0.dev3/phdi/fhir/harmonization/README.md` & `phdi-0.1.0.dev4/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/fhir/harmonization/standardization.py` & `phdi-0.1.0.dev4/phdi/fhir/harmonization/standardization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,99 @@
 import copy
 from typing import List, Literal, Union
 from phdi.harmonization import (
+    DoubleMetaphone,
+    double_metaphone_string,
     standardize_name,
     standardize_country_code,
     standardize_phone,
+    standardize_birth_date,
 )
 
 
+def double_metaphone_bundle(bundle: dict, overwrite=True) -> dict:
+    """
+    Performs the double metaphone algorithm on each name of each patient in a
+    given FHIR bundle.
+
+    :param bundle: A FHIR bundle of data containing one or more patient
+      resources.
+    :param overwrite: If true, `data` is modified in-place; if false, a
+      copy of `data` modified and returned.  Default: `True`.
+    :return: A dictionary mapping the FHIR IDs of patients in the bundle
+      to lists holding the double metaphone representations of their
+      names for each FHIR use case their resource includes.
+    """
+    if not overwrite:
+        bundle = copy.deepcopy(bundle)
+
+    dmeta = DoubleMetaphone()
+    for entry in bundle.get("entry", []):
+        resource = entry.get("resource", {})
+        if resource.get("resourceType", "") == "Patient":
+            double_metaphone_patient(resource, dmeta, overwrite=True)
+    return bundle
+
+
+def double_metaphone_patient(patient: dict, dmeta=None, overwrite=True) -> dict:
+    """
+    Performs the double metaphone algorithm for each name in a given patient
+    resource. The algorithm is performed on each component of the name (first,
+    middle, last), and the resulting representations are ordered in a list
+    such that the first element is first name, the last element is last name,
+    and all other elements are one or more middle names in the order of
+    name presentation. These lists of phonetic representations are stored as
+    the values of dictionaries whose keys are the FHIR uses of the name in
+    the patient resource (e.g. "official"), and all such dictionaries are
+    returned to the caller in a list ordered the same as the names within
+    the given resource.
+
+    :param patient: A FHIR-formatted JSON dictionary representing a patient
+      resource.
+    :param dmeta: An optional existing instantiation of a double metaphone
+      object for use in bulk processing.
+    :param overwrite: If true, `data` is modified in-place; if false, a
+      copy of `data` modified and returned.  Default: `True`.
+    :return: A list of dictionaries mapping FHIR uses to the phonetic
+      representations of names associated with those uses, in presentation
+      order (first, middle, last).
+    """
+
+    if not overwrite:
+        patient = copy.deepcopy(patient)
+
+    for name in patient.get("name", []):
+        # Processing last name separately allows us to note in the result
+        # whether last name wasn't present ( = [None, None])
+        dm_last = double_metaphone_string(name.get("family", ""), dmeta)
+        dm_givens = []
+
+        # Each name is processed sequentially because FHIR expects given
+        # names to already follow proper presentation order
+        for given in name.get("given", []):
+            dm_givens.append(double_metaphone_string(given, dmeta))
+
+        # Cleanest way to store computed encodings is as an extension directly
+        # within the HumanName objects of the patient's `name` field
+        if name.get("extension", []) == []:
+            name["extension"] = []
+
+        name.get("extension").append(
+            {
+                "url": "https://xlinux.nist.gov/dads/HTML/doubleMetaphone.html",
+                "extension": [
+                    {"url": "familyName", "valueString": dm_last},
+                    {"url": "givenName", "valueString": dm_givens},
+                ],
+            }
+        )
+
+    return patient
+
+
 def standardize_names(
     data: dict,
     trim: bool = True,
     case: Literal["upper", "lower", "title"] = "upper",
     remove_numbers: bool = True,
     overwrite: bool = True,
 ) -> dict:
@@ -48,16 +131,16 @@
         return bundle.get("entry", [{}])[0].get("resource", {})
     return bundle
 
 
 def standardize_phones(data: dict, overwrite=True) -> dict:
     """
     Standardizes all phone numbers in a given FHIR bundle or a FHIR resource.
-    Standardization is done according to the underlying `standardize_phone` function in
-    `phdi.harmonization`.
+    Standardization is done according to the underlying `standardize_phone`
+    function in `phdi.harmonization`.
 
     :param data: A FHIR bundle or FHIR-formatted JSON dict.
     :param overwrite: If true, `data` is modified in-place;
       if false, a copy of `data` modified and returned.  Default: `True`
     :return: The bundle or resource with phones appropriately standardized.
     """
 
@@ -94,28 +177,29 @@
 
     The parameters to this function match the standardization flags
     used by the underlying `standardize_name` function found in
     `phdi.harmonization`. For more information, see the docstring for
     that function.
 
     :param resource: A FHIR-formatted JSON dictionary.
-    :param trim: Whether leading/trailing whitespace should be removed. Default: `True`
+    :param trim: Whether leading/trailing whitespace should be removed.
+      Default: `True`
     :param case: The type of casing that should be used. Default: `upper`
-    :param remove_numbers: Whether to delete numeric characters. Default: `True`
+    :param remove_numbers: Whether to delete numeric characters.
+      Default: `True`
     :param overwrite: Whether to replace the original names in the input
       data with the standardized names. Default: `True`
     :return: The resource with appropriately standardized names.
     """
 
     if not overwrite:
         resource = copy.deepcopy(resource)
 
     if resource.get("resourceType", "") == "Patient":
         for name in resource.get("name", []):
-
             # Handle family names
             if "family" in name:
                 transformed_name = standardize_name(
                     name.get("family", ""), trim, case, remove_numbers
                 )
                 name["family"] = transformed_name
 
@@ -129,15 +213,14 @@
                 name["given"] = transformed_names
     return resource
 
 
 def _standardize_phones_in_resource(
     resource: dict, overwrite=True
 ) -> Union[dict, None]:
-
     if not overwrite:
         resource = copy.deepcopy(resource)
 
     if resource.get("resourceType", "") == "Patient":
         for telecom in resource.get("telecom", []):
             if telecom.get("system") == "phone" and "value" in telecom:
                 countries = _extract_countries_from_resource(resource)
@@ -170,7 +253,52 @@
     resource_type = resource.get("resourceType")
     if resource_type == "Patient":
         for address in resource.get("address"):
             country = address.get("country")
             if country:
                 countries.append(standardize_country_code(country, code_type))
     return countries
+
+
+def _standardize_dob_in_resource(
+    resource: dict, format: str = "%Y-%m-%d", overwrite=True
+) -> Union[dict, None]:
+    if not overwrite:
+        resource = copy.deepcopy(resource)
+
+    if resource.get("resourceType", "") == "Patient":
+        birth_date = resource.get("birthDate")
+        transformed_birth_date = standardize_birth_date(birth_date, format)
+        resource["birthDate"] = transformed_birth_date
+    return resource
+
+
+def standardize_dob(data: dict, format: str = "%Y-%m-%d", overwrite=True) -> dict:
+    """
+    Standardizes all birth dates in a given FHIR bundle or a FHIR resource.
+    Standardization is done according to the underlying `standardize_dob` function in
+    `phdi.harmonization`.  The final birthDate will follow the FHIR STu3/R4 format
+    of YYYY-MM-DD which will be stored in the Patient resource.
+
+    :param data: A FHIR bundle or FHIR-formatted JSON dict.
+    :param format: A python DateTime format used to parse the birthDate within
+      the Patient resource.  Default: `%Y-%m-%d` (also known as YYYY-MM-DD)
+    :param overwrite: If true, `data` is modified in-place;
+      if false, a copy of `data` modified and returned.  Default: `True`
+    :return: The bundle or resource with bith dates appropriately standardized.
+    """
+
+    if not overwrite:
+        data = copy.deepcopy(data)
+
+    # Allow users to pass in either a resource or a bundle
+    bundle = data
+    if "entry" not in data:
+        bundle = {"entry": [{"resource": data}]}
+
+    for entry in bundle.get("entry"):
+        resource = entry.get("resource", {})
+        resource = _standardize_dob_in_resource(resource, format, overwrite)
+
+    if "entry" not in data:
+        return bundle.get("entry", [{}])[0].get("resource", {})
+    return bundle
```

### Comparing `phdi-0.1.0.dev3/phdi/fhir/linkage/link.py` & `phdi-0.1.0.dev4/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/fhir/transport/export.py` & `phdi-0.1.0.dev4/phdi/fhir/transport/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
             "Accept": "application/fhir+json",
             "Prefer": "respond-async",
         },
     )
 
     # TODO handle export failure conditions and timeouts.
     if response.status_code == 202:
-
         # Repeatedly poll the endpoint the FHIR server creates for us
         # until either the connection times out (as we configured) or
         # we have the response in hand
         poll_response = export_from_fhir_server_poll(
             poll_url=response.headers.get("Content-Location"),
             cred_manager=cred_manager,
             poll_step=poll_step,
```

### Comparing `phdi-0.1.0.dev3/phdi/fhir/transport/http.py` & `phdi-0.1.0.dev4/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/geospatial/README.md` & `phdi-0.1.0.dev4/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/geospatial/census.py` & `phdi-0.1.0.dev4/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/geospatial/core.py` & `phdi-0.1.0.dev4/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/geospatial/smarty.py` & `phdi-0.1.0.dev4/phdi/geospatial/smarty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import Union
 from smartystreets_python_sdk import StaticCredentials, ClientBuilder
 from smartystreets_python_sdk import us_street
 from smartystreets_python_sdk.us_street.lookup import Lookup
 
 from phdi.geospatial.core import BaseGeocodeClient, GeocodeResult
 
 
@@ -10,15 +10,15 @@
     """
     Represents a PHDI-supplied geocoding client using the Smarty API.
     Requires an authorization ID as well as an authentication token
     in order to build a street lookup client.
     """
 
     def __init__(
-        self, auth_id: str, auth_token: str, licenses: List[str] = ["us-standard-cloud"]
+        self, auth_id: str, auth_token: str, licenses: list[str] = ["us-standard-cloud"]
     ):
         self.auth_id = auth_id
         self.auth_token = auth_token
         creds = StaticCredentials(auth_id, auth_token)
         self.__client = (
             ClientBuilder(creds).with_licenses(licenses).build_us_street_api_client()
         )
```

### Comparing `phdi-0.1.0.dev3/phdi/harmonization/README.md` & `phdi-0.1.0.dev4/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/harmonization/hl7.py` & `phdi-0.1.0.dev4/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev3/phdi/transport/http.py` & `phdi-0.1.0.dev4/phdi/transport/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     retry_strategy = Retry(
         total=retry_count,
         status_forcelist=[429, 500, 502, 503, 504],
         allowed_methods=allowed_methods,
     )
     adapter = HTTPAdapter(max_retries=retry_strategy)
     http = requests.Session()
+    http.mount("http://", adapter)
     http.mount("https://", adapter)
 
     # Now, actually try to complete the API request
     # TODO: Condense this down to make a single call using
     # http.request(method=request_type, url=url, headers=headers, json=data)
     if request_type == "POST":
         response = http.post(
```

### Comparing `phdi-0.1.0.dev3/pyproject.toml` & `phdi-0.1.0.dev4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 [tool.poetry]
 name = "phdi"
-version = "0.1.0.dev3"
+version = "0.1.0.dev4"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi/v0.1.0-dev/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 smartystreets-python-sdk = "^4.10.6"
 pydantic = "^1.9.0"
+fastapi = "^0.95.0"
+httpx = "^0.23.3"
 hl7 = "^0.4.5"
 azure-identity = "^1.10.0"
 azure-storage-blob = "^12.12.0"
 polling = "^0.3.2"
 phonenumbers = "^8.12.48"
 pycountry = "^22.3.5"
 PyYAML = "^6.0"
 pyarrow = "^8.0.0"
 pandas = "^1.4.2"
 coverage = "^6.4.1"
-fhirpathpy = "0.1.0"
+fhirpathpy = "^0.1.0"
 google-auth = "^2.10.0"
 google-cloud-storage = "^2.5.0"
+jsonschema = "4.16.0"
+rapidfuzz = "^2.13.6"
+lxml = "^4.9.2"
+detect-delimiter = "^0.1.1"
+psycopg2-binary = "^2.9.5" 
+sqlalchemy = "^2.0.0"
+matplotlib = "^3.7.1"
+azure-keyvault-secrets = "^4.7.0"
+faker = "^18.4.0"
 
 [tool.poetry.dev-dependencies]
-Sphinx = "^4.4.0"
-black = "^22.1.0"
+pdoc = "^13.0.0"
+black = "^23.1.0"
 pytest = "^7.1.0"
 flake8 = "^4.0.1"
 pytest-cov = "^3.0.0"
+toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = 6.0
-addopts = "--doctest-modules"
+addopts = "--doctest-modules"
```

### Comparing `phdi-0.1.0.dev3/PKG-INFO` & `phdi-0.1.0.dev4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,158 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
+Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
 Requires-Dist: azure-storage-blob (>=12.12.0,<13.0.0)
 Requires-Dist: coverage (>=6.4.1,<7.0.0)
-Requires-Dist: fhirpathpy (==0.1.0)
+Requires-Dist: detect-delimiter (>=0.1.1,<0.2.0)
+Requires-Dist: faker (>=18.4.0,<19.0.0)
+Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: fhirpathpy (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth (>=2.10.0,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0)
 Requires-Dist: hl7 (>=0.4.5,<0.5.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: jsonschema (==4.16.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: phonenumbers (>=8.12.48,<9.0.0)
 Requires-Dist: polling (>=0.3.2,<0.4.0)
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: rapidfuzz (>=2.13.6,<3.0.0)
 Requires-Dist: smartystreets-python-sdk (>=4.10.6,<5.0.0)
+Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Project-URL: Documentation, https://cdcgov.github.io/phdi/v0.1.0-dev/
 Project-URL: Repository, https://github.com/CDCgov/phdi
 Description-Content-Type: text/markdown
 
-# PRIME Public Health Data Infrastructure
+# PRIME Public Health Data Infrastructure (PHDI)
 [![Test github badge](https://github.com/CDCgov/phdi/actions/workflows/test.yaml/badge.svg)](https://github.com/CDCgov/phdi/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/CDCgov/phdi/branch/main/graph/badge.svg)](https://codecov.io/gh/CDCgov/phdi)
 - [PRIME Public Health Data Infrastructure](#prime-public-health-data-infrastructure)
-  - [Getting Started](#getting-started)
-    - [How to import PHDI](#how-to-import-phdi)
   - [Overview](#overview)
     - [Problem Scope](#problem-scope)
+  - [Getting Started](#getting-started)
+  - [Main Features](#main-features)
+  - [Where to Get PHDI](#where-to-get-phdi)
+  - [Documentation](#documentation)
   - [Standard Notices](#standard-notices)
     - [Public Domain Standard Notice](#public-domain-standard-notice)
     - [License Standard Notice](#license-standard-notice)
     - [Privacy Standard Notice](#privacy-standard-notice)
     - [Contributing Standard Notice](#contributing-standard-notice)
     - [Records Management Standard Notice](#records-management-standard-notice)
     - [Related documents](#related-documents)
     - [Additional Standard Notices](#additional-standard-notices)
 
 **General disclaimer** This repository was created for use by CDC programs to collaborate on public health related projects in support of the [CDC mission](https://www.cdc.gov/about/organization/mission.htm). GitHub is not hosted by the CDC, but is a third party website used by CDC and its partners to share information and collaborate on software. CDC use of GitHub does not imply an endorsement of any one particular service, product, or enterprise.
 
-## Getting Started
+## Overview
 
-In order to use the PHDI Building Blocks library, you need [Python 3.9 or higher](https://www.python.org/downloads/) and [pip python package manager](https://pip.pypa.io/en/stable/installation/) (or any python package manager)
+This repository is a part of the CDC/USDS [PHDI project](https://cdcgov.github.io/phdi-site/) and has two components: 
+1. PHDI Python Package
+2. PHDI containerized Building Blocks 
+
+The PHDI Python package contains source code for a platform to help public health authorities (PHAs) ingest and report on public health data. This platform is composed of **Building Blocks**, which are modular software tools that, when composed together, can improve data quality and reduce data cleaning workloads by providing analysis-ready data to downstream public health surveillance systems and other analytical and reporting applications. 
+
+PHDI contains: 
+- Our SDK — the Python library containing Building Block source code
+  - [Repository](https://github.com/CDCgov/phdi/tree/main/phdi)
+  - [API documentation](https://cdcgov.github.io/phdi/sdk/phdi.html)
+- Containerized web services exposing Building Block functionality as HTTP endpoints
+  - [Repository](https://github.com/CDCgov/phdi/tree/main/containers)
+  - [User guide](https://cdcgov.github.io/phdi/) (under Building Blocks)
+- Cloud Starter Kit — Repositories that implement a complete cloud-based pipeline composed of Building Blocks
+  - [Azure](https://github.com/CDCgov/phdi-azure)
+  - [Google Cloud Platform](https://github.com/CDCgov/phdi-google-cloud)
 
+### Problem Scope
+
+Current public health systems that digest, analyze, and respond to data are siloed. Lacking access to actionable data, our national, as well as state, local, and territorial infrastructure, isn’t pandemic-ready. Our objective is to help the CDC best support PHAs in moving towards a modern public health data infrastructure. See our [public website](https://cdcgov.github.io/phdi-site/) for more details.
+
+PHDI is a sibling project to [PRIME ReportStream](https://reportstream.cdc.gov), which focuses on improving the delivery of COVID-19 test data to public health departments, and [PRIME SimpleReport](https://simplereport.gov), which provides a better way for organizations and testing facilities to report COVID-19 rapid tests to public health departments.
+
+## Getting Started
+
+In order to use the PHDI library, you need [Python 3.9 or higher](https://www.python.org/downloads/) and [pip python package manager](https://pip.pypa.io/en/stable/installation/) (or any python package manager).
 
 To install using pip:
 ```
 pip install phdi
 ```
 
-### How to import PHDI
+## Main Features
+
+Here are the current tools that PHDI offers:
+- **Containerized Building Blocks**
+  -   **[Alerts](https://cdcgov.github.io/phdi/containers/alerts.html)** - Provides the ability to send alerts via SMS, Slack, or Microsoft Teams
+  -   **[FHIR Converter](https://cdcgov.github.io/phdi/containers/fhir-converter.html)** - Enables conversion of health data from legacy formats (e.g., HL7 version 2, CCDA) to [FHIR](https://hl7.org/FHIR/), a standard for health care data exchange
+  -   **[Data Ingestion](https://cdcgov.github.io/phdi/containers/ingestion.html)** - Includes the entire pipeline of Building Blocks below
+      -  **[Harmonization](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirharmonization)** - Standardizes input data (e.g., patient names and phone numbers) to streamline the process of cleaning data and improve data quality
+      - **[Geospatial](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirgeospatial)** - Provides a common interface for obtaining precise geographic locations based on street addresses from input data
+      - **[Linkage](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirlinkage)** - Assigns a common identifier to patient records in order to link and deduplicate patient records seen across data contributors
+      - **[Transport](https://cdcgov.github.io/phdi/containers/ingestion.html#tag/fhirtransport)** - Offers functionality for reading and writing data from storage resources (e.g,. FHIR servers)  
+  -   **[Message Parser](https://cdcgov.github.io/phdi/containers/message_parser.html)** - Extracts desired fields from a given message
+  -   **[Tabulation](https://cdcgov.github.io/phdi/containers/tabulation.html)** - Extracts data from a FHIR server, converts it to a tabular representation, and stores it to a user-defined tabular storage file type (e.g., Parquet or CSV)
+  -   **[Record Linkage](https://cdcgov.github.io/phdi/containers/record_linkage.html)** - Links new health care messages to existing records if a connection exists
+  -   **[Validation](https://cdcgov.github.io/phdi/containers/validation.html)** - Checks whether health care messages are in the proper format and contain user-defined fields of interest 
+- **Implementation Support** - Resources to help users implement PHDI tools to manage their data and analysis workflows
+  - **[Examples](https://github.com/CDCgov/phdi/tree/main/examples)** - Sample data that simulates how a Building Block could be used 
+  - **[Tutorials](https://github.com/CDCgov/phdi/tree/main/tutorials)** - Step-by-step instructions to implement Building Blocks source code
+
+## Where to Get PHDI 
 
-Our project is split up into two parts. Our FHIR supporting version and our generic version.
+The source code is hosted on GitHub at: https://github.com/CDCgov/phdi.
 
-Example import for FHIR:
+The latest released version is available at the [Python Package Index (PyPI)](https://pypi.org/project/phdi/).
+
+**Python modules**
 ```
- from phdi.fhir.geospatial.census import CensusFhirGeocodeClient
+pip install phdi
 ```
 
-Example import for generic:
+**Containerized services**
 ```
- from phdi.geospatial.census import CensusGeocodeClient
+build from source
+build Docker locally
+pull down Docker images from GitHub
 ```
 
-Every building block has a FHIR counterpart that works well with FHIR bundles as inputs. The generic version is used for all other non-FHIR inputs.
+## Documentation
 
-For further information on the tutorial: [Geospatial Tutorial](tutorials/geospatial-tutorial.md)
+PHDI documentation is currently hosted on GitHub Pages: https://cdcgov.github.io/phdi/ 
 
-## Overview
-
-The PRIME Public Health Data Infrastructure projects are part of the Pandemic-Ready Interoperability Modernization Effort, a multi-year collaboration between CDC and the U.S. Digital Service (USDS) to strengthen data quality and information technology systems in state and local health departments.
-
-This repository contains source code for a platform to help state, tribal, local and territorial (STLT) public health departments ingest and report on public health data.  It contains the following components:
+There, you can find our: 
+- SDK API reference documentation
+- User guide for containerized Building Blocks
 
-- **Data Ingestion** - Data ingestion tools provide a common framework to prepare data for storage, and store the data in a common standard data model ([FHIR](https://hl7.org/FHIR/)). 
-  - __Harmonization__ - Data harmonization tools can operate on raw input data (HL7 version 2, CCDA) and convert to the common data model format (FHIR).
-  - __Geospatial__ - Geospatial tools provide a common interface for obtaining precise geographic locations based on street addresses from input data.
-  - __Linkage__ - Linkage tools assign a common identifier to patient records to link and deduplicate patients seen across data contributors.
-  - __Transport__ - Transport tools provide a mechanism to store and interact with data stored to a central repostory (FHIR server). 
-- **Reporting** - Reporting tools define a dynamic framework for building custom data models in an analysis-ready output format.
-  - __Tabluation__ - Tabulation provides tools to retrieve data dynamically-defined records and data fields from the common data platform (FHIR server), extract, convert it to a tabular representation, and store to a user-defined tabular storage file type (Parquet or CSV).
-- **Implementation Support** - Implemetnation resources support implementing STLTs to configure a PHDI-driven workflow to manage their data and analysis workflows.
-  - __Cloud-agnostic tools__ - A common PHDI programming interface supports STLTs interacting with cloud-based data storage (containers/buckets), and FHIR servers in a common way.
-  - __Examples and Tutorials__ - Example and tutorial materials help STLTs implement the PHDI solution more quickly by providing easy-to-follow examples and tutorials.
+## Additional Acknowledgments 
 
-The PRIME Public Health Data Infrastructure prototype a sibling project to [PRIME ReportStream](https://reportstream.cdc.gov), focusing on delivering COVID-19 test data to public health departments, and [PRIME SimpleReport](https://simplereport.gov), working on a better way to report COVID-19 rapid tests.
-
-### Problem Scope
+We mapped the rootnames of the PHDI database to nicknames produced by the aggregation and synthesis of open source work from a number of projects. While we do not employ the packages and wrappers used by the various projects (merely their open source data), we wish to give credit to their various works building collections of nickname mappings. These projects are:
 
-Long-term Vision: Current public health systems to digest, analyze, and respond to data are siloed. Lacking access to actionable data, our national, as well as state, local, and territorial infrastructure, isn’t pandemic-ready. Our objective is to help the CDC best support STLTs in moving towards a modern public health data infrastructure.
+* [Secure Enterprise Master Patient Index](https://github.com/MrCsabaToth/SOEMPI), based on OpenEMPI, conducted by Vanderbilt University
+* [Curated Nicknames](https://github.com/carltonnorthern/nicknames), scraped from genealogy webpages and run by Old Dominion University Web Science and Digital Libraries Research Group
+* [Simple Public Domain Nickname Mappings](https://github.com/onyxrev/common_nickname_csv), hand collected using various sources
+* [Lingua En Nickname](https://github.com/brianary/Lingua-EN-Nickname), collected from a series of GenWeb projects
+* [diminutives.db](https://github.com/HaJongler/diminutives.db), compiled via a nickname extract using Wikipedia and Wiktionary
 
 ## Standard Notices
 
 ### Public Domain Standard Notice
 
 This repository constitutes a work of the United States Government and is not
 subject to domestic copyright protection under 17 USC § 105. This repository is in
```

