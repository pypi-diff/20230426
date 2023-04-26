# Comparing `tmp/cellxgene-1.1.1.tar.gz` & `tmp/cellxgene-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene-1.1.1.tar", last modified: Wed Sep 21 18:53:41 2022, max compression
+gzip compressed data, was "cellxgene-1.1.2.tar", last modified: Wed Apr 26 19:04:22 2023, max compression
```

## Comparing `cellxgene-1.1.1.tar` & `cellxgene-1.1.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.825168 cellxgene-1.1.1/
--rw-r--r--   0 atolopko   (503) staff       (20)      319 2022-09-21 18:53:41.000000 cellxgene-1.1.1/MANIFEST.in
--rw-r--r--   0 atolopko   (503) staff       (20)     8285 2022-09-21 18:53:41.825274 cellxgene-1.1.1/PKG-INFO
--rw-r--r--   0 atolopko   (503) staff       (20)     7268 2022-09-21 18:53:41.000000 cellxgene-1.1.1/README.md
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.799824 cellxgene-1.1.1/cellxgene.egg-info/
--rw-r--r--   0 atolopko   (503) staff       (20)     8285 2022-09-21 18:53:41.000000 cellxgene-1.1.1/cellxgene.egg-info/PKG-INFO
--rw-r--r--   0 atolopko   (503) staff       (20)     3517 2022-09-21 18:53:41.000000 cellxgene-1.1.1/cellxgene.egg-info/SOURCES.txt
--rw-r--r--   0 atolopko   (503) staff       (20)        1 2022-09-21 18:53:41.000000 cellxgene-1.1.1/cellxgene.egg-info/dependency_links.txt
--rw-r--r--   0 atolopko   (503) staff       (20)       50 2022-09-21 18:53:41.000000 cellxgene-1.1.1/cellxgene.egg-info/entry_points.txt
--rw-r--r--   0 atolopko   (503) staff       (20)        1 2022-09-21 18:53:41.000000 cellxgene-1.1.1/cellxgene.egg-info/not-zip-safe
--rw-r--r--   0 atolopko   (503) staff       (20)      477 2022-09-21 18:53:41.000000 cellxgene-1.1.1/cellxgene.egg-info/requires.txt
--rw-r--r--   0 atolopko   (503) staff       (20)        7 2022-09-21 18:53:41.000000 cellxgene-1.1.1/cellxgene.egg-info/top_level.txt
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.800525 cellxgene-1.1.1/server/
--rw-r--r--   0 atolopko   (503) staff       (20)      376 2022-09-21 18:52:47.000000 cellxgene-1.1.1/server/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)      339 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/__main__.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.800716 cellxgene-1.1.1/server/annotate/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-29 12:55:16.000000 cellxgene-1.1.1/server/annotate/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)       80 2022-07-29 12:55:16.000000 cellxgene-1.1.1/server/annotate/annotation_types.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.801007 cellxgene-1.1.1/server/app/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/app/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)     8328 2022-09-09 14:48:53.000000 cellxgene-1.1.1/server/app/app.py
--rw-r--r--   0 atolopko   (503) staff       (20)      354 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/app/session.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.802390 cellxgene-1.1.1/server/cli/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/cli/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)     9856 2022-09-20 15:31:57.000000 cellxgene-1.1.1/server/cli/annotate.py
--rw-r--r--   0 atolopko   (503) staff       (20)      908 2022-07-29 12:55:16.000000 cellxgene-1.1.1/server/cli/cli.py
--rw-r--r--   0 atolopko   (503) staff       (20)    14776 2022-07-26 13:01:50.000000 cellxgene-1.1.1/server/cli/launch.py
--rw-r--r--   0 atolopko   (503) staff       (20)     9838 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/cli/prepare.py
--rw-r--r--   0 atolopko   (503) staff       (20)     2991 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/cli/upgrade.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.803225 cellxgene-1.1.1/server/common/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/__init__.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.803511 cellxgene-1.1.1/server/common/annotations/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/annotations/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)     2929 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/annotations/annotations.py
--rw-r--r--   0 atolopko   (503) staff       (20)    11185 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/annotations/local_file_csv.py
--rw-r--r--   0 atolopko   (503) staff       (20)     7101 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/colors.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.803813 cellxgene-1.1.1/server/common/compute/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/compute/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)     6343 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/common/compute/diffexp_generic.py
--rw-r--r--   0 atolopko   (503) staff       (20)     3284 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/compute/estimate_distribution.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.813511 cellxgene-1.1.1/server/common/config/
--rw-r--r--   0 atolopko   (503) staff       (20)       76 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/common/config/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)     7222 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/config/app_config.py
--rw-r--r--   0 atolopko   (503) staff       (20)     3870 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/config/base_config.py
--rw-r--r--   0 atolopko   (503) staff       (20)     3234 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/config/client_config.py
--rw-r--r--   0 atolopko   (503) staff       (20)     9426 2022-07-29 11:44:18.000000 cellxgene-1.1.1/server/common/config/dataset_config.py
--rw-r--r--   0 atolopko   (503) staff       (20)     1833 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/config/external_config.py
--rw-r--r--   0 atolopko   (503) staff       (20)     7866 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/config/server_config.py
--rw-r--r--   0 atolopko   (503) staff       (20)      730 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/constants.py
--rw-r--r--   0 atolopko   (503) staff       (20)     2918 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/corpora.py
--rw-r--r--   0 atolopko   (503) staff       (20)     2400 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/errors.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.813705 cellxgene-1.1.1/server/common/fbs/
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.814959 cellxgene-1.1.1/server/common/fbs/NetEncoding/
--rw-r--r--   0 atolopko   (503) staff       (20)     1301 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/Column.py
--rw-r--r--   0 atolopko   (503) staff       (20)     1617 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/Float32Array.py
--rw-r--r--   0 atolopko   (503) staff       (20)     1617 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/Float64Array.py
--rw-r--r--   0 atolopko   (503) staff       (20)     1591 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/Int32Array.py
--rw-r--r--   0 atolopko   (503) staff       (20)     1657 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/JSONEncodedArray.py
--rw-r--r--   0 atolopko   (503) staff       (20)     3647 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/Matrix.py
--rw-r--r--   0 atolopko   (503) staff       (20)      242 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/TypedArray.py
--rw-r--r--   0 atolopko   (503) staff       (20)     1604 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/Uint32Array.py
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/NetEncoding/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/fbs/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)     9064 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/common/fbs/matrix.py
--rw-r--r--   0 atolopko   (503) staff       (20)     9183 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/common/genesets.py
--rw-r--r--   0 atolopko   (503) staff       (20)     1060 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/health.py
--rw-r--r--   0 atolopko   (503) staff       (20)    15782 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/rest.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.816619 cellxgene-1.1.1/server/common/utils/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/utils/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)      633 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/utils/corpora_constants.py
--rw-r--r--   0 atolopko   (503) staff       (20)     5378 2022-07-29 11:44:18.000000 cellxgene-1.1.1/server/common/utils/data_locator.py
--rw-r--r--   0 atolopko   (503) staff       (20)     6590 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/utils/type_conversion_utils.py
--rw-r--r--   0 atolopko   (503) staff       (20)     4268 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/common/utils/utils.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.816768 cellxgene-1.1.1/server/common/web/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/common/web/__init__.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.822401 cellxgene-1.1.1/server/common/web/static/
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.824342 cellxgene-1.1.1/server/common/web/static/assets/
--rw-r--r--   0 atolopko   (503) staff       (20)   169352 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/RobotoCondensed-Bold-89a396525c0de98da36505cb04eb9373.ttf
--rw-r--r--   0 atolopko   (503) staff       (20)   174736 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/RobotoCondensed-Italic-aca8cfe6a0fd2abecaa6e21a19f66eba.ttf
--rw-r--r--   0 atolopko   (503) staff       (20)   169848 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/RobotoCondensed-Regular-db6d916952fb988edac1e531d47ff83a.ttf
--rw-r--r--   0 atolopko   (503) staff       (20)     3124 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/icon-25c81dcb04bb17fa0e8ad26da31ac22b.png
--rw-r--r--   0 atolopko   (503) staff       (20)    98828 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/icons-16-13933033991f62d6bb641c7a19c8c431.ttf
--rw-r--r--   0 atolopko   (503) staff       (20)    98904 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/icons-16-1645f50fb7f7c109f64eedae92080228.woff
--rw-r--r--   0 atolopko   (503) staff       (20)    99032 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/icons-16-2368f88a078780d80145531133100823.eot
--rw-r--r--   0 atolopko   (503) staff       (20)   101580 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/icons-20-1ef633d3a28d0986f63e78a70178d06d.woff
--rw-r--r--   0 atolopko   (503) staff       (20)   101504 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/icons-20-57b3e708b232fdcb64f9cb115cdda7bb.ttf
--rw-r--r--   0 atolopko   (503) staff       (20)   101708 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/assets/icons-20-cde033c5d3f24283f7578120bb9dc288.eot
--rw-r--r--   0 atolopko   (503) staff       (20)  1722744 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/main-233225c0dceeaa635aef.js
--rw-r--r--   0 atolopko   (503) staff       (20)     4565 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/main-233225c0dceeaa635aef.js.LICENSE.txt
--rw-r--r--   0 atolopko   (503) staff       (20)  6267306 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/main-233225c0dceeaa635aef.js.map
--rw-r--r--   0 atolopko   (503) staff       (20)   324628 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/main-6835a9ad4754cf2ffc45.css
--rw-r--r--   0 atolopko   (503) staff       (20)    50432 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/main-6835a9ad4754cf2ffc45.css.map
--rw-r--r--   0 atolopko   (503) staff       (20)    15835 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js
--rw-r--r--   0 atolopko   (503) staff       (20)    56191 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js.map
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.824533 cellxgene-1.1.1/server/common/web/templates/
--rw-r--r--   0 atolopko   (503) staff       (20)     1741 2022-09-21 18:53:41.000000 cellxgene-1.1.1/server/common/web/templates/index.html
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.824732 cellxgene-1.1.1/server/data_anndata/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/data_anndata/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)    17431 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/data_anndata/anndata_adaptor.py
-drwxr-xr-x   0 atolopko   (503) staff       (20)        0 2022-09-21 18:53:41.825065 cellxgene-1.1.1/server/data_common/
--rw-r--r--   0 atolopko   (503) staff       (20)        0 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/data_common/__init__.py
--rw-r--r--   0 atolopko   (503) staff       (20)    15516 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/data_common/data_adaptor.py
--rw-r--r--   0 atolopko   (503) staff       (20)     2162 2022-09-09 14:49:09.000000 cellxgene-1.1.1/server/data_common/matrix_loader.py
--rw-r--r--   0 atolopko   (503) staff       (20)     2654 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/default_config.py
--rw-r--r--   0 atolopko   (503) staff       (20)       14 2022-07-29 12:55:16.000000 cellxgene-1.1.1/server/requirements-annotate.txt
--rw-r--r--   0 atolopko   (503) staff       (20)      125 2022-07-26 12:18:16.000000 cellxgene-1.1.1/server/requirements-prepare.txt
--rw-r--r--   0 atolopko   (503) staff       (20)      736 2022-07-29 12:55:16.000000 cellxgene-1.1.1/server/requirements.txt
--rw-r--r--   0 atolopko   (503) staff       (20)      168 2022-09-21 18:53:41.825547 cellxgene-1.1.1/setup.cfg
--rw-r--r--   0 atolopko   (503) staff       (20)     1738 2022-09-21 18:53:41.000000 cellxgene-1.1.1/setup.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.182692 cellxgene-1.1.2/
+-rw-r--r--   0 atarashansky   (503) staff       (20)      319 2023-04-26 19:04:21.000000 cellxgene-1.1.2/MANIFEST.in
+-rw-r--r--   0 atarashansky   (503) staff       (20)     8285 2023-04-26 19:04:22.182967 cellxgene-1.1.2/PKG-INFO
+-rw-r--r--   0 atarashansky   (503) staff       (20)     7268 2023-04-26 19:04:21.000000 cellxgene-1.1.2/README.md
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.153379 cellxgene-1.1.2/cellxgene.egg-info/
+-rw-r--r--   0 atarashansky   (503) staff       (20)     8285 2023-04-26 19:04:22.000000 cellxgene-1.1.2/cellxgene.egg-info/PKG-INFO
+-rw-r--r--   0 atarashansky   (503) staff       (20)     3517 2023-04-26 19:04:22.000000 cellxgene-1.1.2/cellxgene.egg-info/SOURCES.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)        1 2023-04-26 19:04:22.000000 cellxgene-1.1.2/cellxgene.egg-info/dependency_links.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)       50 2023-04-26 19:04:22.000000 cellxgene-1.1.2/cellxgene.egg-info/entry_points.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)        1 2023-04-26 19:04:22.000000 cellxgene-1.1.2/cellxgene.egg-info/not-zip-safe
+-rw-r--r--   0 atarashansky   (503) staff       (20)      484 2023-04-26 19:04:22.000000 cellxgene-1.1.2/cellxgene.egg-info/requires.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)        7 2023-04-26 19:04:22.000000 cellxgene-1.1.2/cellxgene.egg-info/top_level.txt
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.154736 cellxgene-1.1.2/server/
+-rw-r--r--   0 atarashansky   (503) staff       (20)      376 2023-04-26 19:02:23.000000 cellxgene-1.1.2/server/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)      339 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/__main__.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.155242 cellxgene-1.1.2/server/annotate/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/annotate/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)       80 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/annotate/annotation_types.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.155938 cellxgene-1.1.2/server/app/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/app/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     8328 2023-04-26 17:51:31.000000 cellxgene-1.1.2/server/app/app.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)      354 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/app/session.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.157298 cellxgene-1.1.2/server/cli/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/cli/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     9856 2023-01-09 13:34:09.000000 cellxgene-1.1.2/server/cli/annotate.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)      908 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/cli/cli.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)    14776 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/cli/launch.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     9838 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/cli/prepare.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     2991 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/cli/upgrade.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.159058 cellxgene-1.1.2/server/common/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/__init__.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.159916 cellxgene-1.1.2/server/common/annotations/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/annotations/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     2929 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/annotations/annotations.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)    11185 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/annotations/local_file_csv.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     7101 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/colors.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.160588 cellxgene-1.1.2/server/common/compute/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/compute/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     6343 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/compute/diffexp_generic.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     3284 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/compute/estimate_distribution.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.162156 cellxgene-1.1.2/server/common/config/
+-rw-r--r--   0 atarashansky   (503) staff       (20)       76 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/config/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     7222 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/config/app_config.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     3870 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/config/base_config.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     3234 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/config/client_config.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     9426 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/config/dataset_config.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1833 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/config/external_config.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     7866 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/config/server_config.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)      730 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/constants.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     2918 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/corpora.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     2400 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/errors.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.162623 cellxgene-1.1.2/server/common/fbs/
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.164741 cellxgene-1.1.2/server/common/fbs/NetEncoding/
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1301 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/Column.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1617 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/Float32Array.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1617 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/Float64Array.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1591 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/Int32Array.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1657 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/JSONEncodedArray.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     3647 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/Matrix.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)      242 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/TypedArray.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1604 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/Uint32Array.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/NetEncoding/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     9064 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/fbs/matrix.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     9183 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/genesets.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1060 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/health.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)    15782 2023-02-14 01:45:42.000000 cellxgene-1.1.2/server/common/rest.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.165775 cellxgene-1.1.2/server/common/utils/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/utils/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)      633 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/utils/corpora_constants.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     5378 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/utils/data_locator.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     6590 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/utils/type_conversion_utils.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     4268 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/utils/utils.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.165992 cellxgene-1.1.2/server/common/web/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/common/web/__init__.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.176059 cellxgene-1.1.2/server/common/web/static/
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.180770 cellxgene-1.1.2/server/common/web/static/assets/
+-rw-r--r--   0 atarashansky   (503) staff       (20)   169352 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/RobotoCondensed-Bold-89a396525c0de98da36505cb04eb9373.ttf
+-rw-r--r--   0 atarashansky   (503) staff       (20)   174736 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/RobotoCondensed-Italic-aca8cfe6a0fd2abecaa6e21a19f66eba.ttf
+-rw-r--r--   0 atarashansky   (503) staff       (20)   169848 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/RobotoCondensed-Regular-db6d916952fb988edac1e531d47ff83a.ttf
+-rw-r--r--   0 atarashansky   (503) staff       (20)     3124 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/icon-25c81dcb04bb17fa0e8ad26da31ac22b.png
+-rw-r--r--   0 atarashansky   (503) staff       (20)    98828 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/icons-16-13933033991f62d6bb641c7a19c8c431.ttf
+-rw-r--r--   0 atarashansky   (503) staff       (20)    98904 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/icons-16-1645f50fb7f7c109f64eedae92080228.woff
+-rw-r--r--   0 atarashansky   (503) staff       (20)    99032 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/icons-16-2368f88a078780d80145531133100823.eot
+-rw-r--r--   0 atarashansky   (503) staff       (20)   101580 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/icons-20-1ef633d3a28d0986f63e78a70178d06d.woff
+-rw-r--r--   0 atarashansky   (503) staff       (20)   101504 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/icons-20-57b3e708b232fdcb64f9cb115cdda7bb.ttf
+-rw-r--r--   0 atarashansky   (503) staff       (20)   101708 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/assets/icons-20-cde033c5d3f24283f7578120bb9dc288.eot
+-rw-r--r--   0 atarashansky   (503) staff       (20)  1722744 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/main-233225c0dceeaa635aef.js
+-rw-r--r--   0 atarashansky   (503) staff       (20)     4565 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/main-233225c0dceeaa635aef.js.LICENSE.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)  6267306 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/main-233225c0dceeaa635aef.js.map
+-rw-r--r--   0 atarashansky   (503) staff       (20)   324628 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/main-6835a9ad4754cf2ffc45.css
+-rw-r--r--   0 atarashansky   (503) staff       (20)    50432 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/main-6835a9ad4754cf2ffc45.css.map
+-rw-r--r--   0 atarashansky   (503) staff       (20)    15835 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js
+-rw-r--r--   0 atarashansky   (503) staff       (20)    56191 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js.map
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.181129 cellxgene-1.1.2/server/common/web/templates/
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1741 2023-04-26 19:04:21.000000 cellxgene-1.1.2/server/common/web/templates/index.html
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.181777 cellxgene-1.1.2/server/data_anndata/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/data_anndata/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)    17431 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/data_anndata/anndata_adaptor.py
+drwxr-xr-x   0 atarashansky   (503) staff       (20)        0 2023-04-26 19:04:22.182455 cellxgene-1.1.2/server/data_common/
+-rw-r--r--   0 atarashansky   (503) staff       (20)        0 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/data_common/__init__.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)    15516 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/data_common/data_adaptor.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     2162 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/data_common/matrix_loader.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)     2654 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/default_config.py
+-rw-r--r--   0 atarashansky   (503) staff       (20)       14 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/requirements-annotate.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)      125 2022-08-25 15:21:09.000000 cellxgene-1.1.2/server/requirements-prepare.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)      743 2023-04-26 18:59:55.000000 cellxgene-1.1.2/server/requirements.txt
+-rw-r--r--   0 atarashansky   (503) staff       (20)      168 2023-04-26 19:04:22.183529 cellxgene-1.1.2/setup.cfg
+-rw-r--r--   0 atarashansky   (503) staff       (20)     1738 2023-04-26 19:04:21.000000 cellxgene-1.1.2/setup.py
```

### Comparing `cellxgene-1.1.1/PKG-INFO` & `cellxgene-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene
-Version: 1.1.1
+Version: 1.1.2
 Summary: Web application for exploration of large scale scRNA-seq datasets
 Home-page: https://github.com/chanzuckerberg/cellxgene
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Flask
```

### Comparing `cellxgene-1.1.1/README.md` & `cellxgene-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/cellxgene.egg-info/PKG-INFO` & `cellxgene-1.1.2/cellxgene.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene
-Version: 1.1.1
+Version: 1.1.2
 Summary: Web application for exploration of large scale scRNA-seq datasets
 Home-page: https://github.com/chanzuckerberg/cellxgene
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Flask
```

### Comparing `cellxgene-1.1.1/cellxgene.egg-info/SOURCES.txt` & `cellxgene-1.1.2/cellxgene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/app/app.py` & `cellxgene-1.1.2/server/app/app.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/cli/annotate.py` & `cellxgene-1.1.2/server/cli/annotate.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/cli/cli.py` & `cellxgene-1.1.2/server/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/cli/launch.py` & `cellxgene-1.1.2/server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/cli/prepare.py` & `cellxgene-1.1.2/server/cli/prepare.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/cli/upgrade.py` & `cellxgene-1.1.2/server/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/annotations/annotations.py` & `cellxgene-1.1.2/server/common/annotations/annotations.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/annotations/local_file_csv.py` & `cellxgene-1.1.2/server/common/annotations/local_file_csv.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/colors.py` & `cellxgene-1.1.2/server/common/colors.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/compute/diffexp_generic.py` & `cellxgene-1.1.2/server/common/compute/diffexp_generic.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/compute/estimate_distribution.py` & `cellxgene-1.1.2/server/common/compute/estimate_distribution.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/config/app_config.py` & `cellxgene-1.1.2/server/common/config/app_config.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/config/base_config.py` & `cellxgene-1.1.2/server/common/config/base_config.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/config/client_config.py` & `cellxgene-1.1.2/server/common/config/client_config.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/config/dataset_config.py` & `cellxgene-1.1.2/server/common/config/dataset_config.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/config/external_config.py` & `cellxgene-1.1.2/server/common/config/external_config.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/config/server_config.py` & `cellxgene-1.1.2/server/common/config/server_config.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/constants.py` & `cellxgene-1.1.2/server/common/constants.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/corpora.py` & `cellxgene-1.1.2/server/common/corpora.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/errors.py` & `cellxgene-1.1.2/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/NetEncoding/Column.py` & `cellxgene-1.1.2/server/common/fbs/NetEncoding/Column.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/NetEncoding/Float32Array.py` & `cellxgene-1.1.2/server/common/fbs/NetEncoding/Float32Array.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/NetEncoding/Float64Array.py` & `cellxgene-1.1.2/server/common/fbs/NetEncoding/Float64Array.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/NetEncoding/Int32Array.py` & `cellxgene-1.1.2/server/common/fbs/NetEncoding/Int32Array.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/NetEncoding/JSONEncodedArray.py` & `cellxgene-1.1.2/server/common/fbs/NetEncoding/JSONEncodedArray.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/NetEncoding/Matrix.py` & `cellxgene-1.1.2/server/common/fbs/NetEncoding/Matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/NetEncoding/Uint32Array.py` & `cellxgene-1.1.2/server/common/fbs/NetEncoding/Uint32Array.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/fbs/matrix.py` & `cellxgene-1.1.2/server/common/fbs/matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/genesets.py` & `cellxgene-1.1.2/server/common/genesets.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/health.py` & `cellxgene-1.1.2/server/common/health.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/rest.py` & `cellxgene-1.1.2/server/common/rest.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/utils/corpora_constants.py` & `cellxgene-1.1.2/server/common/utils/corpora_constants.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/utils/data_locator.py` & `cellxgene-1.1.2/server/common/utils/data_locator.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/utils/type_conversion_utils.py` & `cellxgene-1.1.2/server/common/utils/type_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/utils/utils.py` & `cellxgene-1.1.2/server/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/RobotoCondensed-Bold-89a396525c0de98da36505cb04eb9373.ttf` & `cellxgene-1.1.2/server/common/web/static/assets/RobotoCondensed-Bold-89a396525c0de98da36505cb04eb9373.ttf`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/RobotoCondensed-Italic-aca8cfe6a0fd2abecaa6e21a19f66eba.ttf` & `cellxgene-1.1.2/server/common/web/static/assets/RobotoCondensed-Italic-aca8cfe6a0fd2abecaa6e21a19f66eba.ttf`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/RobotoCondensed-Regular-db6d916952fb988edac1e531d47ff83a.ttf` & `cellxgene-1.1.2/server/common/web/static/assets/RobotoCondensed-Regular-db6d916952fb988edac1e531d47ff83a.ttf`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/icon-25c81dcb04bb17fa0e8ad26da31ac22b.png` & `cellxgene-1.1.2/server/common/web/static/assets/icon-25c81dcb04bb17fa0e8ad26da31ac22b.png`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/icons-16-13933033991f62d6bb641c7a19c8c431.ttf` & `cellxgene-1.1.2/server/common/web/static/assets/icons-16-13933033991f62d6bb641c7a19c8c431.ttf`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/icons-16-1645f50fb7f7c109f64eedae92080228.woff` & `cellxgene-1.1.2/server/common/web/static/assets/icons-16-1645f50fb7f7c109f64eedae92080228.woff`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/icons-16-2368f88a078780d80145531133100823.eot` & `cellxgene-1.1.2/server/common/web/static/assets/icons-16-2368f88a078780d80145531133100823.eot`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/icons-20-1ef633d3a28d0986f63e78a70178d06d.woff` & `cellxgene-1.1.2/server/common/web/static/assets/icons-20-1ef633d3a28d0986f63e78a70178d06d.woff`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/icons-20-57b3e708b232fdcb64f9cb115cdda7bb.ttf` & `cellxgene-1.1.2/server/common/web/static/assets/icons-20-57b3e708b232fdcb64f9cb115cdda7bb.ttf`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/assets/icons-20-cde033c5d3f24283f7578120bb9dc288.eot` & `cellxgene-1.1.2/server/common/web/static/assets/icons-20-cde033c5d3f24283f7578120bb9dc288.eot`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/main-233225c0dceeaa635aef.js` & `cellxgene-1.1.2/server/common/web/static/main-233225c0dceeaa635aef.js`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/main-233225c0dceeaa635aef.js.LICENSE.txt` & `cellxgene-1.1.2/server/common/web/static/main-233225c0dceeaa635aef.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/main-233225c0dceeaa635aef.js.map` & `cellxgene-1.1.2/server/common/web/static/main-233225c0dceeaa635aef.js.map`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/main-6835a9ad4754cf2ffc45.css` & `cellxgene-1.1.2/server/common/web/static/main-6835a9ad4754cf2ffc45.css`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/main-6835a9ad4754cf2ffc45.css.map` & `cellxgene-1.1.2/server/common/web/static/main-6835a9ad4754cf2ffc45.css.map`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js` & `cellxgene-1.1.2/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js.map` & `cellxgene-1.1.2/server/common/web/static/obsolete-08e38608ad9cbdcbafda246111ad337d.js.map`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/common/web/templates/index.html` & `cellxgene-1.1.2/server/common/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/data_anndata/anndata_adaptor.py` & `cellxgene-1.1.2/server/data_anndata/anndata_adaptor.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/data_common/data_adaptor.py` & `cellxgene-1.1.2/server/data_common/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/data_common/matrix_loader.py` & `cellxgene-1.1.2/server/data_common/matrix_loader.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/default_config.py` & `cellxgene-1.1.2/server/default_config.py`

 * *Files identical despite different names*

### Comparing `cellxgene-1.1.1/server/requirements.txt` & `cellxgene-1.1.2/server/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # NOTE: If you update 'anndata' min version, also update the 'anndata_version'
 # matrix value in .github/workflows/compatibility_tests.yml
 anndata>=0.7.6 # we need to_memory(), added in 0.7.6
 boto3>=1.12.18
 click>=7.1.2
-Flask>=1.0.2
+Flask>=1.0.2,<2.3.0
 Flask-Compress>=1.4.0
 Flask-Cors>=3.0.9  # CVE-2020-25032
 Flask-RESTful>=0.3.6
 flask-server-timing>=0.1.2
 flask-talisman>=0.7.0
 flatbuffers>=1.11.0,<2.0.0 # cellxgene is not compatible with 2.0.0. Requires migration
 flatten-dict>=0.2.0
```

### Comparing `cellxgene-1.1.1/setup.py` & `cellxgene-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     requirements_prepare = fh.read().splitlines()
 
 with open("server/requirements-annotate.txt") as fh:
     requirements_annotate = fh.read().splitlines()
 
 setup(
     name="cellxgene",
-    version="1.1.1",
+    version="1.1.2",
     packages=find_packages(),
     url="https://github.com/chanzuckerberg/cellxgene",
     license="MIT",
     author="Chan Zuckerberg Initiative",
     author_email="cellxgene@chanzuckerberg.com",
     description="Web application for exploration of large scale scRNA-seq datasets",
     long_description=long_description,
```

