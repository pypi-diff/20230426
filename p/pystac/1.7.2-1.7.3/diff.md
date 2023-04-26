# Comparing `tmp/pystac-1.7.2.tar.gz` & `tmp/pystac-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-1.7.2.tar", last modified: Thu Apr  6 14:51:38 2023, max compression
+gzip compressed data, was "pystac-1.7.3.tar", last modified: Wed Apr 26 11:44:19 2023, max compression
```

## Comparing `pystac-1.7.2.tar` & `pystac-1.7.3.tar`

### file list

```diff
@@ -1,86 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.867306 pystac-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-06 14:51:26.000000 pystac-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-06 14:51:38.867306 pystac-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-06 14:51:26.000000 pystac-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.855306 pystac-1.7.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.855306 pystac-1.7.2/benchmarks/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/extensions/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/import_pystac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-06 14:51:26.000000 pystac-1.7.2/benchmarks/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.859306 pystac-1.7.2/pystac/
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    41568 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.867306 pystac-1.7.2/pystac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/datacube.py
--rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/eo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/item_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    28872 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/sat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/scientific.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/extensions/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.867306 pystac-1.7.2/pystac/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/Asset.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/Catalog.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/Collection.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/Item.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/ItemCollection.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/Link.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/Macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/Provider.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/html/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/item_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/rel_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.867306 pystac-1.7.2/pystac/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/serialization/common_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/serialization/identify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/serialization/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/stac_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/stac_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/summaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.867306 pystac-1.7.2/pystac/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/validation/schema_uri_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/validation/stac_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-06 14:51:26.000000 pystac-1.7.2/pystac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:51:38.863306 pystac-1.7.2/pystac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-06 14:51:38.000000 pystac-1.7.2/pystac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-06 14:51:38.000000 pystac-1.7.2/pystac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:51:38.000000 pystac-1.7.2/pystac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:51:38.000000 pystac-1.7.2/pystac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-06 14:51:38.000000 pystac-1.7.2/pystac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-06 14:51:38.000000 pystac-1.7.2/pystac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-06 14:51:38.867306 pystac-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-06 14:51:26.000000 pystac-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-26 11:44:09.000000 pystac-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-26 11:44:19.257161 pystac-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-26 11:44:09.000000 pystac-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.245160 pystac-1.7.3/pystac/
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41568 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.253161 pystac-1.7.3/pystac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/datacube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/eo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/item_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28872 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/sat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/scientific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/extensions/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/pystac/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Asset.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Catalog.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Collection.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Item.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/ItemCollection.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Link.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/Provider.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/html/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19333 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/item_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/rel_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/pystac/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/common_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/serialization/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/stac_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/stac_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.257161 pystac-1.7.3/pystac/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/validation/schema_uri_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/validation/stac_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-26 11:44:09.000000 pystac-1.7.3/pystac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:44:19.249160 pystac-1.7.3/pystac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 11:44:19.000000 pystac-1.7.3/pystac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 11:44:19.261160 pystac-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-26 11:44:09.000000 pystac-1.7.3/setup.py
```

### Comparing `pystac-1.7.2/LICENSE` & `pystac-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/PKG-INFO` & `pystac-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.7.2
+Version: 1.7.3
 Summary: Python library for working with Spatiotemporal Asset Catalog (STAC).
 Home-page: https://github.com/stac-utils/pystac
 Author: stac-utils
 Author-email: stac@radiant.earth
 License: Apache Software License 2.0
 Project-URL: Tracker, https://github.com/stac-utils/pystac/issues
 Project-URL: Documentation, https://pystac.readthedocs.io/en/latest/
```

### Comparing `pystac-1.7.2/README.md` & `pystac-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/__init__.py` & `pystac-1.7.3/pystac/__init__.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/asset.py` & `pystac-1.7.3/pystac/asset.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/cache.py` & `pystac-1.7.3/pystac/cache.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/catalog.py` & `pystac-1.7.3/pystac/catalog.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/collection.py` & `pystac-1.7.3/pystac/collection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/common_metadata.py` & `pystac-1.7.3/pystac/common_metadata.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/errors.py` & `pystac-1.7.3/pystac/errors.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/base.py` & `pystac-1.7.3/pystac/extensions/base.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/datacube.py` & `pystac-1.7.3/pystac/extensions/datacube.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/eo.py` & `pystac-1.7.3/pystac/extensions/eo.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/file.py` & `pystac-1.7.3/pystac/extensions/file.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/grid.py` & `pystac-1.7.3/pystac/extensions/grid.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/hooks.py` & `pystac-1.7.3/pystac/extensions/hooks.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/item_assets.py` & `pystac-1.7.3/pystac/extensions/item_assets.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/label.py` & `pystac-1.7.3/pystac/extensions/label.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/pointcloud.py` & `pystac-1.7.3/pystac/extensions/pointcloud.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/projection.py` & `pystac-1.7.3/pystac/extensions/projection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/raster.py` & `pystac-1.7.3/pystac/extensions/raster.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/sar.py` & `pystac-1.7.3/pystac/extensions/sar.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/sat.py` & `pystac-1.7.3/pystac/extensions/sat.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/scientific.py` & `pystac-1.7.3/pystac/extensions/scientific.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/storage.py` & `pystac-1.7.3/pystac/extensions/storage.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/table.py` & `pystac-1.7.3/pystac/extensions/table.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/timestamps.py` & `pystac-1.7.3/pystac/extensions/timestamps.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/version.py` & `pystac-1.7.3/pystac/extensions/version.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/extensions/view.py` & `pystac-1.7.3/pystac/extensions/view.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/html/Asset.jinja2` & `pystac-1.7.3/pystac/html/Asset.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/html/Catalog.jinja2` & `pystac-1.7.3/pystac/html/Catalog.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/html/Item.jinja2` & `pystac-1.7.3/pystac/html/Item.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/html/ItemCollection.jinja2` & `pystac-1.7.3/pystac/html/ItemCollection.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/html/Link.jinja2` & `pystac-1.7.3/pystac/html/Link.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/html/Macros.jinja2` & `pystac-1.7.3/pystac/html/Macros.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/html/jinja_env.py` & `pystac-1.7.3/pystac/html/jinja_env.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/item.py` & `pystac-1.7.3/pystac/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import warnings
 from copy import copy, deepcopy
 from html import escape
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union, cast
 
 import pystac
-from pystac import STACError, STACObjectType
+from pystac import RelType, STACError, STACObjectType
 from pystac.asset import Asset
 from pystac.catalog import Catalog
 from pystac.collection import Collection
 from pystac.errors import DeprecatedWarning, ExtensionNotImplemented
 from pystac.html.jinja_env import get_jinja_env
 from pystac.link import Link
 from pystac.serialization import (
@@ -472,21 +472,17 @@
             datetime=datetime,
             properties=properties,
             extra_fields=extra_fields,
             href=href,
             assets={k: Asset.from_dict(v) for k, v in assets.items()},
         )
 
-        has_self_link = False
         for link in links:
-            has_self_link |= link["rel"] == pystac.RelType.SELF
-            item.add_link(Link.from_dict(link))
-
-        if not has_self_link and href is not None:
-            item.add_link(Link.self_href(href))
+            if href is None or link.get("rel", None) != RelType.SELF:
+                item.add_link(Link.from_dict(link))
 
         if root:
             item.set_root(root)
 
         try:
             version = ItemVersionExtension.ext(item)
             if version.deprecated:
```

### Comparing `pystac-1.7.2/pystac/item_collection.py` & `pystac-1.7.3/pystac/item_collection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/layout.py` & `pystac-1.7.3/pystac/layout.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/link.py` & `pystac-1.7.3/pystac/link.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/media_type.py` & `pystac-1.7.3/pystac/media_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/provider.py` & `pystac-1.7.3/pystac/provider.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/rel_type.py` & `pystac-1.7.3/pystac/rel_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/serialization/common_properties.py` & `pystac-1.7.3/pystac/serialization/common_properties.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/serialization/identify.py` & `pystac-1.7.3/pystac/serialization/identify.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/serialization/migrate.py` & `pystac-1.7.3/pystac/serialization/migrate.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/stac_io.py` & `pystac-1.7.3/pystac/stac_io.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/stac_object.py` & `pystac-1.7.3/pystac/stac_object.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/summaries.py` & `pystac-1.7.3/pystac/summaries.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/utils.py` & `pystac-1.7.3/pystac/utils.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/validation/__init__.py` & `pystac-1.7.3/pystac/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/validation/schema_uri_map.py` & `pystac-1.7.3/pystac/validation/schema_uri_map.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/validation/stac_validator.py` & `pystac-1.7.3/pystac/validation/stac_validator.py`

 * *Files identical despite different names*

### Comparing `pystac-1.7.2/pystac/version.py` & `pystac-1.7.3/pystac/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import Optional
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 """Library version"""
 
 
 class STACVersion:
     DEFAULT_STAC_VERSION = "1.0.0"
     """Latest STAC version supported by PySTAC"""
```

### Comparing `pystac-1.7.2/pystac.egg-info/PKG-INFO` & `pystac-1.7.3/pystac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.7.2
+Version: 1.7.3
 Summary: Python library for working with Spatiotemporal Asset Catalog (STAC).
 Home-page: https://github.com/stac-utils/pystac
 Author: stac-utils
 Author-email: stac@radiant.earth
 License: Apache Software License 2.0
 Project-URL: Tracker, https://github.com/stac-utils/pystac/issues
 Project-URL: Documentation, https://pystac.readthedocs.io/en/latest/
```

### Comparing `pystac-1.7.2/pystac.egg-info/SOURCES.txt` & `pystac-1.7.3/pystac.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,11 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-benchmarks/__init__.py
-benchmarks/_base.py
-benchmarks/_util.py
-benchmarks/catalog.py
-benchmarks/collection.py
-benchmarks/import_pystac.py
-benchmarks/item.py
-benchmarks/extensions/__init__.py
-benchmarks/extensions/projection.py
 pystac/__init__.py
 pystac/asset.py
 pystac/cache.py
 pystac/catalog.py
 pystac/collection.py
 pystac/common_metadata.py
 pystac/errors.py
```

### Comparing `pystac-1.7.2/setup.py` & `pystac-1.7.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "Python library for working with Spatiotemporal Asset Catalog (STAC)."
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="stac-utils",
     author_email="stac@radiant.earth",
     url="https://github.com/stac-utils/pystac",
-    packages=find_packages(exclude=["tests*"]),
+    packages=find_packages(exclude=["tests*", "benchmarks*"]),
     package_data={"": ["py.typed", "*.jinja2"]},
     py_modules=[splitext(basename(path))[0] for path in glob("pystac/*.py")],
     python_requires=">=3.8",
     install_requires=["python-dateutil>=2.7.0"],
     extras_require={
         "validation": ["jsonschema>=4.0.1"],
         "orjson": ["orjson>=3.5"],
```

