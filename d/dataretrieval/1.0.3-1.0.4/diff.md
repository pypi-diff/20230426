# Comparing `tmp/dataretrieval-1.0.3.tar.gz` & `tmp/dataretrieval-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataretrieval-1.0.3.tar", last modified: Fri Mar 10 20:58:54 2023, max compression
+gzip compressed data, was "dataretrieval-1.0.4.tar", last modified: Wed Apr 26 21:39:09 2023, max compression
```

## Comparing `dataretrieval-1.0.3.tar` & `dataretrieval-1.0.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.244438 dataretrieval-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.160437 dataretrieval-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.164437 dataretrieval-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/.github/workflows/sphinx-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.160437 dataretrieval-1.0.3/.gitlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.164437 dataretrieval-1.0.3/.gitlab/issue_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/.gitlab/issue_templates/reviewer_checklist.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.164437 dataretrieval-1.0.3/.gitlab/merge_request_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/.gitlab/merge_request_templates/reviewer_checklist.md
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-03-10 20:58:54.240438 dataretrieval-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/code.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.164437 dataretrieval-1.0.3/dataretrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-10 20:58:53.000000 dataretrieval-1.0.3/dataretrieval/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.164437 dataretrieval-1.0.3/dataretrieval/codes/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/codes/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/codes/timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/nadp.py
--rw-r--r--   0 runner    (1001) docker     (123)    40358 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/nwis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/streamstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/waterwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/dataretrieval/wqp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.164437 dataretrieval-1.0.3/dataretrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-03-10 20:58:53.000000 dataretrieval-1.0.3/dataretrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-10 20:58:54.000000 dataretrieval-1.0.3/dataretrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:58:53.000000 dataretrieval-1.0.3/dataretrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-10 20:58:53.000000 dataretrieval-1.0.3/dataretrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-10 20:58:53.000000 dataretrieval-1.0.3/dataretrieval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.168437 dataretrieval-1.0.3/demos/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9869 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/NWIS_demo_1.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)    13027 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/R Python Vignette equivalents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.168437 dataretrieval-1.0.3/demos/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/datasets/peak_discharge_trends.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.168437 dataretrieval-1.0.3/demos/hydroshare/
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.168437 dataretrieval-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.168437 dataretrieval-1.0.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.172437 dataretrieval-1.0.3/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.172437 dataretrieval-1.0.3/docs/source/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/datasets/peak_discharge_trends.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/nwisdemo01.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/readme_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/rvignettes.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/examples/siteinfo_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.172437 dataretrieval-1.0.3/docs/source/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/meta/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/meta/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/meta/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.172437 dataretrieval-1.0.3/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/reference/nadp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/reference/nwis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/reference/streamstats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/reference/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/reference/waterwatch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/reference/wqp.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.176437 dataretrieval-1.0.3/docs/source/userguide/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/userguide/dataportals.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/userguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/docs/source/userguide/timeconventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 20:58:54.244438 dataretrieval-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.176437 dataretrieval-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:58:54.240438 dataretrieval-1.0.3/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22902 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/nwis_sites.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    48992 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/water_use_allegheny.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/water_use_national.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14065 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterdata_measurements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterdata_pmcodes.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)  5998995 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterdata_qwdata.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14869 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterservices_dv.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterservices_gwlevels.txt
--rwxr-xr-x   0 runner    (1001) docker     (123) 22180871 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterservices_iv.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4595 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterservices_peaks.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2323 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterservices_ratings.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1429 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterservices_site.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)   198769 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/waterservices_stats.txt
--rw-r--r--   0 runner    (1001) docker     (123) 21772141 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_activities.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_activity_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1442378 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_detection_limits.txt
--rw-r--r--   0 runner    (1001) docker     (123)   436730 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_habitat_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_organizations.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1029205 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_project_weights.txt
--rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_projects.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_results.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)  2276131 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/data/wqp_sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/nadp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/nwis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13631 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/waterservices_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7787 2023-03-10 20:58:33.000000 dataretrieval-1.0.3/tests/wqp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.772600 dataretrieval-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.688598 dataretrieval-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.github/workflows/sphinx-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.688598 dataretrieval-1.0.4/.gitlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/.gitlab/issue_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.gitlab/issue_templates/reviewer_checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/.gitlab/merge_request_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/.gitlab/merge_request_templates/reviewer_checklist.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-26 21:39:09.772600 dataretrieval-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/code.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/dataretrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/dataretrieval/codes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/codes/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/codes/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/nadp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40711 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/streamstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/waterwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/dataretrieval/wqp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/dataretrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 21:39:09.000000 dataretrieval-1.0.4/dataretrieval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.696598 dataretrieval-1.0.4/demos/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9869 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/NWIS_demo_1.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13027 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/R Python Vignette equivalents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/demos/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/datasets/peak_discharge_trends.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/demos/hydroshare/
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.700598 dataretrieval-1.0.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.704598 dataretrieval-1.0.4/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.704598 dataretrieval-1.0.4/docs/source/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)   535225 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/datasets/peak_discharge_trends.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/nwisdemo01.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/readme_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/rvignettes.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/examples/siteinfo_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.708598 dataretrieval-1.0.4/docs/source/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/meta/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/meta/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/meta/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.708598 dataretrieval-1.0.4/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/nadp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/nwis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/streamstats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/waterwatch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/reference/wqp.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.708598 dataretrieval-1.0.4/docs/source/userguide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/userguide/dataportals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/userguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/docs/source/userguide/timeconventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:39:09.772600 dataretrieval-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.712598 dataretrieval-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:09.768599 dataretrieval-1.0.4/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22902 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/nwis_sites.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48992 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/water_use_allegheny.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/water_use_national.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14065 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterdata_measurements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterdata_pmcodes.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5998995 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterdata_qwdata.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14869 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_dv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_gwlevels.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123) 22180871 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_iv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4595 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_peaks.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2323 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_ratings.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1429 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_site.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)   198769 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/waterservices_stats.txt
+-rw-r--r--   0 runner    (1001) docker     (123) 21772141 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_activities.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_activity_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1442378 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_detection_limits.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   436730 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_habitat_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_organizations.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1029205 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_project_weights.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_projects.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_results.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2276131 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/data/wqp_sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/nadp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/nwis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13455 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/waterservices_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7787 2023-04-26 21:38:52.000000 dataretrieval-1.0.4/tests/wqp_test.py
```

### Comparing `dataretrieval-1.0.3/.github/workflows/python-package.yml` & `dataretrieval-1.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/.github/workflows/python-publish.yml` & `dataretrieval-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/.github/workflows/sphinx-docs.yml` & `dataretrieval-1.0.4/.github/workflows/sphinx-docs.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/.gitignore` & `dataretrieval-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/.gitlab/issue_templates/reviewer_checklist.md` & `dataretrieval-1.0.4/.gitlab/issue_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/.gitlab/merge_request_templates/reviewer_checklist.md` & `dataretrieval-1.0.4/.gitlab/merge_request_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/CONTRIBUTING.md` & `dataretrieval-1.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/DISCLAIMER.md` & `dataretrieval-1.0.4/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/LICENSE.md` & `dataretrieval-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/PKG-INFO` & `dataretrieval-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.3
+Version: 1.0.4
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>, Jayaram Hariharan <jhariharan@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `dataretrieval-1.0.3/README.md` & `dataretrieval-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/code.json` & `dataretrieval-1.0.4/code.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval/codes/states.py` & `dataretrieval-1.0.4/dataretrieval/codes/states.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval/codes/timezones.py` & `dataretrieval-1.0.4/dataretrieval/codes/timezones.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval/nadp.py` & `dataretrieval-1.0.4/dataretrieval/nadp.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval/nwis.py` & `dataretrieval-1.0.4/dataretrieval/nwis.py`

 * *Files 1% similar despite different names*

```diff
@@ -935,14 +935,15 @@
         - 'site' : site description
         - 'measurements' : discharge measurements
         - 'peaks': discharge peaks
         - 'gwlevels': groundwater levels
         - 'pmcodes': get parameter codes
         - 'water_use': get water use data
         - 'ratings': get rating table
+        - 'stat': get statistics
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
         ``pandas.DataFrame`` containing requested data
 
@@ -984,14 +985,19 @@
         >>> df = dataretrieval.nwis.get_record(
         ...     service='water_use', years='2010', categories='L')
 
         >>> # Get rating table for USGS streamgage 01585200
         >>> df = dataretrieval.nwis.get_record(
         ...     sites='01585200', service='ratings')
 
+        >>> # Get annual statistics for USGS station 01646500
+        >>> df = dataretrieval.nwis.get_record(
+        ...     sites='01646500', service='stat', statReportType='annual',
+        ...     statYearType='water')
+
     """
     if service not in WATERSERVICES_SERVICES + WATERDATA_SERVICES:
         raise TypeError('Unrecognized service: {}'.format(service))
 
     if service == 'iv':
         df, _ = get_iv(sites=sites, startDT=start, endDT=end,
                        multi_index=multi_index, **kwargs)
@@ -1037,14 +1043,18 @@
         df, _ = get_water_use(state=state, **kwargs)
         return df
 
     elif service == 'ratings':
         df, _ = get_ratings(site=sites, **kwargs)
         return df
 
+    elif service == 'stat':
+        df, _ = get_stats(sites=sites, **kwargs)
+        return df
+
     else:
         raise TypeError('{} service not yet implemented'.format(service))
 
 
 def _read_json(json):
     """
     Reads a NWIS Water Services formatted JSON into a ``pandas.DataFrame``.
```

### Comparing `dataretrieval-1.0.3/dataretrieval/streamstats.py` & `dataretrieval-1.0.4/dataretrieval/streamstats.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval/utils.py` & `dataretrieval-1.0.4/dataretrieval/utils.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval/waterwatch.py` & `dataretrieval-1.0.4/dataretrieval/waterwatch.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval/wqp.py` & `dataretrieval-1.0.4/dataretrieval/wqp.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/dataretrieval.egg-info/PKG-INFO` & `dataretrieval-1.0.4/dataretrieval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.3
+Version: 1.0.4
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>, Jayaram Hariharan <jhariharan@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `dataretrieval-1.0.3/dataretrieval.egg-info/SOURCES.txt` & `dataretrieval-1.0.4/dataretrieval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/NWIS_demo_1.ipynb` & `dataretrieval-1.0.4/demos/NWIS_demo_1.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/R Python Vignette equivalents.ipynb` & `dataretrieval-1.0.4/demos/R Python Vignette equivalents.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.4/demos/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb` & `dataretrieval-1.0.4/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/docs/Makefile` & `dataretrieval-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/docs/source/conf.py` & `dataretrieval-1.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/docs/source/examples/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.4/docs/source/examples/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/docs/source/examples/index.rst` & `dataretrieval-1.0.4/docs/source/examples/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 We provide executed versions of these notebooks below; to download the
 ``.ipynb`` files for your own use, either visit the `Hydroshare`_ repository,
 or navigate to the `demos/hydroshare`_ subdirectory of the ``dataretrieval``
 project repository.
 
 .. _Hydroshare: https://www.hydroshare.org/resource/c97c32ecf59b4dff90ef013030c54264/
 
-.. _demos/hydroshare: https://github.com/USGS-python/dataretrieval/tree/master/demos/hydroshare
+.. _demos/hydroshare: https://github.com/DOI-USGS/dataretrieval-python/tree/master/demos/hydroshare
 
 .. toctree::
     :maxdepth: 1
 
     USGS_dataretrieval_DailyValues_Examples
     USGS_dataretrieval_GroundwaterLevels_Examples
     USGS_dataretrieval_Measurements_Examples
```

### Comparing `dataretrieval-1.0.3/docs/source/examples/readme_examples.rst` & `dataretrieval-1.0.4/docs/source/examples/readme_examples.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/docs/source/examples/siteinfo_examples.rst` & `dataretrieval-1.0.4/docs/source/examples/siteinfo_examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 `NWIS water services documentation`_ for additional information. The below
 example illustrates the use of the ``seriesCatalogOutput`` switch and displays
 the resulting column names for the output dataframes (example prompted by
 `GitHub Issue #34`_).
 
 .. _NWIS water services documentation: https://nwis.waterservices.usgs.gov/rest/Site-Service.html
 
-.. _GitHub Issue #34: https://github.com/USGS-python/dataretrieval/issues/34
+.. _GitHub Issue #34: https://github.com/DOI-USGS/dataretrieval-python/issues/34
 
 .. doctest::
 
     # first import the functions for downloading data from NWIS
     >>> import dataretrieval.nwis as nwis
 
     # fetch data from a major HUC basin with seriesCatalogOutput set to True
```

### Comparing `dataretrieval-1.0.3/docs/source/index.rst` & `dataretrieval-1.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/docs/source/meta/contributing.rst` & `dataretrieval-1.0.4/docs/source/meta/contributing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Ways to contribute
 ------------------
 
 Reporting Bugs:
 ^^^^^^^^^^^^^^^
 
-Report bugs at https://github.com/USGS-python/dataretrieval/issues
+Report bugs at https://github.com/DOI-USGS/dataretrieval-python/issues
 
 When reporting a bug, please include:
 
     - Detailed steps to reproduce the bug
     - Your operating system name and version.
     - Any details about your local setup that might be helpful in troubleshooting.
 
@@ -40,15 +40,15 @@
 ``dataretrieval`` could always use more documentation, whether as part of the
 official docs, in docstrings, or even in blog posts or articles.
 
 Submitting Feedback:
 ^^^^^^^^^^^^^^^^^^^^
 
 The best way to send feedback is to file an issue at
-https://github.com/USGS-python/dataretrieval/issues
+https://github.com/DOI-USGS/dataretrieval-python/issues
 
 If you are proposing a feature:
 
     - Explain in detail how it would work.
     - Keep the scope as narrow as possible, to make it easier to implement.
 
 Contributor Guidelines
```

### Comparing `dataretrieval-1.0.3/docs/source/meta/installing.rst` & `dataretrieval-1.0.4/docs/source/meta/installing.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 Whether you are a user or developer we recommend installing ``dataretrieval``
 in a virtual environment. This can be done using something like ``virtualenv``
 or ``conda``. Package dependencies are listed in the `requirements.txt`_ file,
 a full list of dependencies necessary for development are listed in the
 `requirements-dev.txt`_ file.
 
-.. _requirements.txt: https://github.com/USGS-python/dataretrieval/blob/master/requirements.txt
+.. _requirements.txt: https://github.com/DOI-USGS/dataretrieval-python/blob/master/requirements.txt
 
-.. _requirements-dev.txt: https://github.com/USGS-python/dataretrieval/blob/master/requirements-dev.txt
+.. _requirements-dev.txt: https://github.com/DOI-USGS/dataretrieval-python/blob/master/requirements-dev.txt
 
 
 User Installation
 -----------------
 
 Via ``pip``:
 ^^^^^^^^^^^^
@@ -47,15 +47,15 @@
 feature branch, and propose changes as pull requests to the main branch of
 the repository.
 
 The first step is to clone your fork of the repository:
 
 .. code-block:: bash
 
-    $ git clone https://github.com/USGS-python/dataretrieval.git
+    $ git clone https://github.com/DOI-USGS/dataretrieval-python.git
 
 Then, set the cloned repository as your current working directory in your
 terminal and run the following commands to get an "editable" installation of
 the package for development:
 
 .. code-block:: bash
 
@@ -70,15 +70,15 @@
     $ pytest
 
 In order to fetch the latest version of ``dataretrieval``, we recommend
 defining the main repository as a remote `upstream` repository:
 
 .. code-block:: bash
 
-    $ git remote add upstream https://github.com/USGS-python/dataretrieval.git
+    $ git remote add upstream https://github.com/DOI-USGS/dataretrieval-python.git
 
 You can also build the documentation locally by running the following commands:
 
 .. code-block:: bash
 
     $ cd docs
     $ make docs
```

### Comparing `dataretrieval-1.0.3/docs/source/meta/license.rst` & `dataretrieval-1.0.4/docs/source/meta/license.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 
 Unless otherwise noted, this project is in the public domain in the United
 States because it contains materials that originally came from the United
 States Geological Survey, an agency of the United States Department of
 Interior. For more information, see the `LICENSE.md`_ file. See the
 `Disclaimer.md`_ file for more information about the disclaimer.
 
-.. _LICENSE.md: https://github.com/USGS-python/dataretrieval/blob/master/LICENSE.md
+.. _LICENSE.md: https://github.com/DOI-USGS/dataretrieval-python/blob/master/LICENSE.md
 
-.. _Disclaimer.md: https://github.com/USGS-python/dataretrieval/blob/master/Disclaimer.md
+.. _Disclaimer.md: https://github.com/DOI-USGS/dataretrieval-python/blob/master/DISCLAIMER.md
```

### Comparing `dataretrieval-1.0.3/docs/source/userguide/dataportals.rst` & `dataretrieval-1.0.4/docs/source/userguide/dataportals.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/docs/source/userguide/timeconventions.rst` & `dataretrieval-1.0.4/docs/source/userguide/timeconventions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 conversion, or :obj:`pandas.DataFrame.tz_localize()` if the datetime objects
 exist but are not UTC-localized. In most cases (single-site and multi-site),
 ``dataretrieval`` assigns the datetime information as the dataframe *index*,
 the exception to this is when incomplete datetime information is available, in
 these cases integers are used as the dataframe index (see `PR#58`_ for more
 details).
 
-.. _PR#58: https://github.com/USGS-python/dataretrieval/pull/58
+.. _PR#58: https://github.com/DOI-USGS/dataretrieval-python/pull/58
 
 
 Inspecting Timestamps
 *********************
 
 For single sites, the index of the returned dataframe contains pandas
 timestamps.
```

### Comparing `dataretrieval-1.0.3/pyproject.toml` & `dataretrieval-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/nwis_sites.txt` & `dataretrieval-1.0.4/tests/data/nwis_sites.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/water_use_allegheny.txt` & `dataretrieval-1.0.4/tests/data/water_use_allegheny.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/water_use_national.txt` & `dataretrieval-1.0.4/tests/data/water_use_national.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterdata_measurements.txt` & `dataretrieval-1.0.4/tests/data/waterdata_measurements.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterdata_qwdata.txt` & `dataretrieval-1.0.4/tests/data/waterdata_qwdata.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterservices_dv.txt` & `dataretrieval-1.0.4/tests/data/waterservices_dv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterservices_gwlevels.txt` & `dataretrieval-1.0.4/tests/data/waterservices_gwlevels.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterservices_iv.txt` & `dataretrieval-1.0.4/tests/data/waterservices_iv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterservices_peaks.txt` & `dataretrieval-1.0.4/tests/data/waterservices_peaks.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterservices_ratings.txt` & `dataretrieval-1.0.4/tests/data/waterservices_ratings.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterservices_site.txt` & `dataretrieval-1.0.4/tests/data/waterservices_site.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/waterservices_stats.txt` & `dataretrieval-1.0.4/tests/data/waterservices_stats.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_activities.txt` & `dataretrieval-1.0.4/tests/data/wqp_activities.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_activity_metrics.txt` & `dataretrieval-1.0.4/tests/data/wqp_activity_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_detection_limits.txt` & `dataretrieval-1.0.4/tests/data/wqp_detection_limits.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_habitat_metrics.txt` & `dataretrieval-1.0.4/tests/data/wqp_habitat_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_organizations.txt` & `dataretrieval-1.0.4/tests/data/wqp_organizations.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_project_weights.txt` & `dataretrieval-1.0.4/tests/data/wqp_project_weights.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_projects.txt` & `dataretrieval-1.0.4/tests/data/wqp_projects.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_results.txt` & `dataretrieval-1.0.4/tests/data/wqp_results.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/data/wqp_sites.txt` & `dataretrieval-1.0.4/tests/data/wqp_sites.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/nadp_test.py` & `dataretrieval-1.0.4/tests/nadp_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/nwis_test.py` & `dataretrieval-1.0.4/tests/nwis_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/utils_test.py` & `dataretrieval-1.0.4/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.3/tests/waterservices_test.py` & `dataretrieval-1.0.4/tests/waterservices_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,14 @@
 
 def test_get_record_validation():
     """Tests the validation parameters of the get_record method"""
     with pytest.raises(TypeError) as type_error:
         get_record(sites=['01491000'], service='not_a_service')
     assert 'Unrecognized service: not_a_service' == str(type_error.value)
 
-    with pytest.raises(TypeError) as type_error:
-        get_record(sites=['01491000'], service='stat')
-    assert 'stat service not yet implemented' == str(type_error.value)
-
 
 def test_get_dv(requests_mock):
     """Tests get_dv method correctly generates the request url and returns the result in a DataFrame"""
     format = "json"
     site = '01491000%2C01645000'
     request_url = 'https://waterservices.usgs.gov/nwis/dv?format={}' \
                   '&startDT=2020-02-14&endDT=2020-02-15&sites={}'.format(format, site)
```

### Comparing `dataretrieval-1.0.3/tests/wqp_test.py` & `dataretrieval-1.0.4/tests/wqp_test.py`

 * *Files identical despite different names*

