# Comparing `tmp/pdstools-3.1.6.tar.gz` & `tmp/pdstools-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.1.6.tar", last modified: Wed Apr 26 08:24:30 2023, max compression
+gzip compressed data, was "pdstools-3.1.7.tar", last modified: Wed Apr 26 09:20:18 2023, max compression
```

## Comparing `pdstools-3.1.6.tar` & `pdstools-3.1.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.245845 pdstools-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 08:24:21.000000 pdstools-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 08:24:30.241845 pdstools-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-26 08:24:21.000000 pdstools-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.237845 pdstools-3.1.6/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 08:24:30.000000 pdstools-3.1.6/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 08:24:30.000000 pdstools-3.1.6/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:24:30.000000 pdstools-3.1.6/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 08:24:30.000000 pdstools-3.1.6/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 08:24:30.000000 pdstools-3.1.6/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 08:24:30.000000 pdstools-3.1.6/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 08:24:21.000000 pdstools-3.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.237845 pdstools-3.1.6/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.237845 pdstools-3.1.6/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.237845 pdstools-3.1.6/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/table_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:30.241845 pdstools-3.1.6/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:24:21.000000 pdstools-3.1.6/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:24:30.245845 pdstools-3.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 09:20:06.000000 pdstools-3.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 09:20:18.192341 pdstools-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-26 09:20:06.000000 pdstools-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 09:20:18.000000 pdstools-3.1.7/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 09:20:06.000000 pdstools-3.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.188341 pdstools-3.1.7/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/table_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:18.192341 pdstools-3.1.7/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:20:06.000000 pdstools-3.1.7/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:20:18.192341 pdstools-3.1.7/setup.cfg
```

### Comparing `pdstools-3.1.6/LICENSE` & `pdstools-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/PKG-INFO` & `pdstools-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.6
+Version: 3.1.7
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.6 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.7 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.6/README.md` & `pdstools-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/pdstools.egg-info/PKG-INFO` & `pdstools-3.1.7/pdstools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.6
+Version: 3.1.7
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.6 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.7 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.6/pdstools.egg-info/SOURCES.txt` & `pdstools-3.1.7/pdstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/pyproject.toml` & `pdstools-3.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/__init__.py` & `pdstools-3.1.7/python/pdstools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python pdstools"""
 
-__version__ = "3.1.6"
+__version__ = "3.1.7"
 
 from polars import enable_string_cache
 
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
```

### Comparing `pdstools-3.1.6/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.1.7/python/pdstools/adm/ADMDatamart.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/adm/ADMTrees.py` & `pdstools-3.1.7/python/pdstools/adm/ADMTrees.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/adm/Tables.py` & `pdstools-3.1.7/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/app/cli.py` & `pdstools-3.1.7/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/app/pages/Health Check.py` & `pdstools-3.1.7/python/pdstools/app/pages/Health Check.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.1.7/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/ih/legacy_IH.py` & `pdstools-3.1.7/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/pega_io/API.py` & `pdstools-3.1.7/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/pega_io/File.py` & `pdstools-3.1.7/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/pega_io/S3.py` & `pdstools-3.1.7/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/plots/plot_base.py` & `pdstools-3.1.7/python/pdstools/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/plots/plots_plotly.py` & `pdstools-3.1.7/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.1.7/python/pdstools/reports/HealthCheck.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/reports/HealthCheckModel.qmd` & `pdstools-3.1.7/python/pdstools/reports/HealthCheckModel.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/utils/cdh_utils.py` & `pdstools-3.1.7/python/pdstools/utils/cdh_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/utils/datasets.py` & `pdstools-3.1.7/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/utils/hds_utils.py` & `pdstools-3.1.7/python/pdstools/utils/hds_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,38 +184,64 @@
             self.column_mapping,
         ) = self.get_predictors_mapping()
 
     def write_to_output(
         self,
         df: Optional[pl.DataFrame] = None,
         ext: Literal["ndjson", "parquet", "arrow", "csv"] = None,
+        mode: Literal["optimized", "robust"] = "optimized",
     ):
         """Write the processed dataframe to an output file.
 
         Parameters
         ----------
         df : Optional[pl.DataFrame]
             Dataframe to write.
             If not provided, runs `self.process()`
         ext : Literal["ndjson", "parquet", "arrow", "csv"]
             What extension to write the file to
+        mode : Literal['optimized', 'robust'], default = 'optimized'
+            Whether to output a single file (optimized) or maintain
+            the same file structure as the original files (robust).
+            Optimized should be faster, but robust should allow for bigger
+            data as we don't need all data in memory at the same time.
 
         """
         out_filename = f"{self.config.output_folder}/hds"
         out_format = self.config.output_format if ext is None else ext
+
         if df is None:
-            df = self.process()
-        if out_format == "ndjson":
-            df.write_ndjson(f"{out_filename}.json")
-        elif out_format == "parquet":
-            df.write_parquet(f"{out_filename}.parquet")
-        elif out_format == "arrow":
-            df.write_ipc(f"{out_filename}.arrow")
-        else:
-            df.write_csv(f"{out_filename}.csv")
+            df = self.process(strategy="lazy")
+        if mode == "robust":
+            if "filename" not in df.columns:
+                mode = "optimized"
+            else:
+                for filename in (
+                    df.select(pl.col("filename").unique())
+                    .collect()
+                    .to_series()
+                    .to_list()
+                ):
+                    newName = Path(out_filename) / Path(filename).name
+                    df.filter(pl.col("filename") == filename).drop(
+                        "filename"
+                    ).collect().write_ndjson(newName)
+
+        if mode == "optimized":
+            if "filename" in df.columns:
+                df = df.drop(pl.col("filename"))
+            df = df.collect()
+            if out_format == "ndjson":
+                df.write_ndjson(f"{out_filename}.json")
+            elif out_format == "parquet":
+                df.write_parquet(f"{out_filename}.parquet")
+            elif out_format == "arrow":
+                df.write_ipc(f"{out_filename}.arrow")
+            else:
+                df.write_csv(f"{out_filename}.csv")
 
     def create_mapping_file(self):
         """Create a file to write the column mapping"""
         with open(self.config.mapping_file, "w") as wr:
             for key, mapped_val in self.column_mapping.items():
                 wr.write(f"{key}={mapped_val}")
                 wr.write("\n")
@@ -385,14 +411,16 @@
                 else:
                     numeric_predictors_to_mask.append(val)
             predictors[val] = (
                 f"PREDICTOR_{idx}" if self.config.mask_predictor_names else val
             )
 
         special_predictors = {x: x for x in special_predictors_t}
+        if "Decision_SubjectID" in special_predictors_t:
+            symbolic_predictors_to_mask.append("Decision_SubjectID")
 
         outcome_column[outcome_t] = (
             "OUTCOME" if self.config.mask_outcome_name else outcome_t
         )
 
         column_mapping = {
             **predictors,
@@ -428,15 +456,14 @@
 
         else:
             return pl.col(cols).apply(algorithm)
 
     def process(
         self,
         strategy="eager",
-        mode: Literal["optimized", "robust"] = "optimized",
         **kwargs,
     ):
         """Anonymize the dataset."""
 
         def to_hash(cols, **kwargs):
             hasher = self.getHasher(cols, **kwargs)
             return (
```

### Comparing `pdstools-3.1.6/python/pdstools/utils/pega_template.py` & `pdstools-3.1.7/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/utils/polars_ext.py` & `pdstools-3.1.7/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/utils/show_versions.py` & `pdstools-3.1.7/python/pdstools/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.1.7/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/utils/table_definitions.py` & `pdstools-3.1.7/python/pdstools/utils/table_definitions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.6/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.1.7/python/pdstools/valuefinder/ValueFinder.py`

 * *Files identical despite different names*

