# Comparing `tmp/siibra-0.4a46.tar.gz` & `tmp/siibra-0.4a47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-0.4a46.tar", last modified: Wed Apr 26 10:27:10 2023, max compression
+gzip compressed data, was "siibra-0.4a47.tar", last modified: Wed Apr 26 11:04:32 2023, max compression
```

## Comparing `siibra-0.4a46.tar` & `siibra-0.4a47.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.445911 siibra-0.4a46/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 10:25:41.000000 siibra-0.4a46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 10:25:41.000000 siibra-0.4a46/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-26 10:27:10.445911 siibra-0.4a46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-04-26 10:25:41.000000 siibra-0.4a46/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:27:10.445911 siibra-0.4a46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 10:25:41.000000 siibra-0.4a46/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.433910 siibra-0.4a46/siibra/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.433910 siibra-0.4a46/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.433910 siibra-0.4a46/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.433910 siibra-0.4a46/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.437910 siibra-0.4a46/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/connectivity/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/connectivity/streamline_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.437910 siibra-0.4a46/siibra/features/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/dataset/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.437910 siibra-0.4a46/siibra/features/image/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/image/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/image/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.437910 siibra-0.4a46/siibra/features/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/layerwise_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/receptor_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/regional_timeseries_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/features/tabular/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.437910 siibra-0.4a46/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.441911 siibra-0.4a46/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.441911 siibra-0.4a46/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.441911 siibra-0.4a46/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.441911 siibra-0.4a46/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.445911 siibra-0.4a46/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/volumes/gifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/volumes/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/volumes/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/volumes/parcellationmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-26 10:25:41.000000 siibra-0.4a46/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.433910 siibra-0.4a46/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-26 10:27:10.000000 siibra-0.4a46/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 10:27:10.000000 siibra-0.4a46/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:27:10.000000 siibra-0.4a46/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 10:27:10.000000 siibra-0.4a46/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 10:27:10.000000 siibra-0.4a46/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:27:10.445911 siibra-0.4a46/test/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-26 10:25:41.000000 siibra-0.4a46/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.645815 siibra-0.4a47/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 11:03:14.000000 siibra-0.4a47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 11:03:14.000000 siibra-0.4a47/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-26 11:04:32.645815 siibra-0.4a47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-04-26 11:03:14.000000 siibra-0.4a47/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:04:32.645815 siibra-0.4a47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 11:03:14.000000 siibra-0.4a47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/connectivity/streamline_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/regional_timeseries_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.637815 siibra-0.4a47/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/parcellationmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-26 11:03:14.000000 siibra-0.4a47/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.633814 siibra-0.4a47/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 11:04:32.000000 siibra-0.4a47/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:04:32.641815 siibra-0.4a47/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-26 11:03:14.000000 siibra-0.4a47/test/test_siibra.py
```

### Comparing `siibra-0.4a46/LICENSE` & `siibra-0.4a47/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/PKG-INFO` & `siibra-0.4a47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a46
+Version: 0.4a47
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a46/README.rst` & `siibra-0.4a47/README.rst`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/setup.py` & `siibra-0.4a47/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/__init__.py` & `siibra-0.4a47/siibra/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/commons.py` & `siibra-0.4a47/siibra/commons.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/configuration/__init__.py` & `siibra-0.4a47/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/configuration/configuration.py` & `siibra-0.4a47/siibra/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/configuration/factory.py` & `siibra-0.4a47/siibra/configuration/factory.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/core/__init__.py` & `siibra-0.4a47/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/core/atlas.py` & `siibra-0.4a47/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/core/concept.py` & `siibra-0.4a47/siibra/core/concept.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/core/parcellation.py` & `siibra-0.4a47/siibra/core/parcellation.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/core/region.py` & `siibra-0.4a47/siibra/core/region.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/core/space.py` & `siibra-0.4a47/siibra/core/space.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/__init__.py` & `siibra-0.4a47/siibra/features/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/anchor.py` & `siibra-0.4a47/siibra/features/anchor.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/connectivity/__init__.py` & `siibra-0.4a47/siibra/features/connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/connectivity/functional_connectivity.py` & `siibra-0.4a47/siibra/features/connectivity/functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/connectivity/regional_connectivity.py` & `siibra-0.4a47/siibra/features/connectivity/regional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/connectivity/streamline_counts.py` & `siibra-0.4a47/siibra/features/connectivity/streamline_counts.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/connectivity/streamline_lengths.py` & `siibra-0.4a47/siibra/features/connectivity/streamline_lengths.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/dataset/__init__.py` & `siibra-0.4a47/siibra/features/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/dataset/ebrains.py` & `siibra-0.4a47/siibra/features/dataset/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/feature.py` & `siibra-0.4a47/siibra/features/feature.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/image/__init__.py` & `siibra-0.4a47/siibra/features/image/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/image/image.py` & `siibra-0.4a47/siibra/features/image/image.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/image/sections.py` & `siibra-0.4a47/siibra/features/image/sections.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/image/volume_of_interest.py` & `siibra-0.4a47/siibra/features/image/volume_of_interest.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/__init__.py` & `siibra-0.4a47/siibra/features/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/bigbrain_intensity_profile.py` & `siibra-0.4a47/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/cell_density_profile.py` & `siibra-0.4a47/siibra/features/tabular/cell_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/cortical_profile.py` & `siibra-0.4a47/siibra/features/tabular/cortical_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/gene_expression.py` & `siibra-0.4a47/siibra/features/tabular/gene_expression.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/layerwise_bigbrain_intensities.py` & `siibra-0.4a47/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/layerwise_cell_density.py` & `siibra-0.4a47/siibra/features/tabular/layerwise_cell_density.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/receptor_density_fingerprint.py` & `siibra-0.4a47/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/receptor_density_profile.py` & `siibra-0.4a47/siibra/features/tabular/receptor_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/features/tabular/regional_timeseries_activity.py` & `siibra-0.4a47/siibra/features/tabular/regional_timeseries_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,14 @@
         table = self.get_table(subject)
         return table.mean().plot(kind="bar", **kwargs)
 
 
 class RegionalBOLD(
     RegionalTimeseriesActivity,
     configuration_folder="features/tabular/activity_timeseries/bold",
-    category="activity_timeseries"
+    category="functional"
 ):
     """
     Blood-oxygen-level-dependent (BOLD) signals per region.
     """
 
     pass
```

### Comparing `siibra-0.4a46/siibra/features/tabular/tabular.py` & `siibra-0.4a47/siibra/features/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/livequeries/__init__.py` & `siibra-0.4a47/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/livequeries/allen.py` & `siibra-0.4a47/siibra/livequeries/allen.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/livequeries/bigbrain.py` & `siibra-0.4a47/siibra/livequeries/bigbrain.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/livequeries/ebrains.py` & `siibra-0.4a47/siibra/livequeries/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/livequeries/query.py` & `siibra-0.4a47/siibra/livequeries/query.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/locations/__init__.py` & `siibra-0.4a47/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/locations/boundingbox.py` & `siibra-0.4a47/siibra/locations/boundingbox.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/locations/location.py` & `siibra-0.4a47/siibra/locations/location.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/locations/point.py` & `siibra-0.4a47/siibra/locations/point.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/locations/pointset.py` & `siibra-0.4a47/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/retrieval/__init__.py` & `siibra-0.4a47/siibra/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/retrieval/cache.py` & `siibra-0.4a47/siibra/retrieval/cache.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/retrieval/datasets.py` & `siibra-0.4a47/siibra/retrieval/datasets.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/retrieval/repositories.py` & `siibra-0.4a47/siibra/retrieval/repositories.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/retrieval/requests.py` & `siibra-0.4a47/siibra/retrieval/requests.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/vocabularies/__init__.py` & `siibra-0.4a47/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/vocabularies/gene_names.json` & `siibra-0.4a47/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/vocabularies/receptor_symbols.json` & `siibra-0.4a47/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/vocabularies/region_aliases.json` & `siibra-0.4a47/siibra/vocabularies/region_aliases.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/volumes/__init__.py` & `siibra-0.4a47/siibra/volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/volumes/gifti.py` & `siibra-0.4a47/siibra/volumes/gifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/volumes/neuroglancer.py` & `siibra-0.4a47/siibra/volumes/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/volumes/nifti.py` & `siibra-0.4a47/siibra/volumes/nifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/volumes/parcellationmap.py` & `siibra-0.4a47/siibra/volumes/parcellationmap.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/volumes/sparsemap.py` & `siibra-0.4a47/siibra/volumes/sparsemap.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra/volumes/volume.py` & `siibra-0.4a47/siibra/volumes/volume.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/siibra.egg-info/PKG-INFO` & `siibra-0.4a47/siibra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a46
+Version: 0.4a47
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a46/siibra.egg-info/SOURCES.txt` & `siibra-0.4a47/siibra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siibra-0.4a46/test/test_siibra.py` & `siibra-0.4a47/test/test_siibra.py`

 * *Files identical despite different names*

