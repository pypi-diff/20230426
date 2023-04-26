# Comparing `tmp/pywapor-3.3.3.tar.gz` & `tmp/pywapor-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywapor-3.3.3.tar", last modified: Wed Apr  5 09:01:31 2023, max compression
+gzip compressed data, was "pywapor-3.3.4.tar", last modified: Wed Apr 26 14:18:25 2023, max compression
```

## Comparing `pywapor-3.3.3.tar` & `pywapor-3.3.4.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:31.004777 pywapor-3.3.3/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2022-06-23 13:36:53.000000 pywapor-3.3.3/LICENSE
--rw-r--r--   0 hmcoerver   (501) staff       (20)      229 2022-08-29 07:22:20.000000 pywapor-3.3.3/MANIFEST.in
--rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-04-05 09:01:31.004646 pywapor-3.3.3/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11578 2023-04-05 08:06:25.000000 pywapor-3.3.3/README.md
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.958511 pywapor-3.3.3/pywapor/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      416 2023-04-05 08:59:47.000000 pywapor-3.3.3/pywapor/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.959983 pywapor-3.3.3/pywapor/collect/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2022-09-28 07:45:21.000000 pywapor-3.3.3/pywapor/collect/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13487 2023-01-25 04:36:11.000000 pywapor-3.3.3/pywapor/collect/accounts.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9150 2023-01-12 09:57:39.000000 pywapor-3.3.3/pywapor/collect/downloader.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.981876 pywapor-3.3.3/pywapor/collect/product/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5802 2023-01-05 11:26:49.000000 pywapor-3.3.3/pywapor/collect/product/CHIRPS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8172 2022-12-22 13:03:36.000000 pywapor-3.3.3/pywapor/collect/product/COPERNICUS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8387 2022-09-29 11:29:30.000000 pywapor-3.3.3/pywapor/collect/product/ERA5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6154 2022-12-22 11:50:32.000000 pywapor-3.3.3/pywapor/collect/product/GEOS5.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1110900 2022-08-24 12:33:55.000000 pywapor-3.3.3/pywapor/collect/product/GLO30.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1111950 2022-08-24 12:33:41.000000 pywapor-3.3.3/pywapor/collect/product/GLO90.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2023-01-06 12:00:32.000000 pywapor-3.3.3/pywapor/collect/product/GLOBCOVER.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    40234 2023-01-25 04:40:44.000000 pywapor-3.3.3/pywapor/collect/product/LANDSAT.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.983787 pywapor-3.3.3/pywapor/collect/product/Landsat/
--rw-r--r--   0 hmcoerver   (501) staff       (20)    25684 2022-09-28 09:16:32.000000 pywapor-3.3.3/pywapor/collect/product/Landsat/C2L2SP.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      250 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/collect/product/Landsat/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2023-01-05 10:39:18.000000 pywapor-3.3.3/pywapor/collect/product/MERRA2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2023-02-10 10:58:24.000000 pywapor-3.3.3/pywapor/collect/product/MODIS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/collect/product/MODIS_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11566 2023-01-04 09:31:52.000000 pywapor-3.3.3/pywapor/collect/product/PROBAV.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    23344 2023-03-17 16:53:56.000000 pywapor-3.3.3/pywapor/collect/product/SENTINEL2.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6543 2023-03-16 15:51:36.000000 pywapor-3.3.3/pywapor/collect/product/SENTINEL3.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7297 2022-12-22 13:02:32.000000 pywapor-3.3.3/pywapor/collect/product/SRTM.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/collect/product/SRTM30_tiles.geojson
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7204 2023-01-05 10:39:59.000000 pywapor-3.3.3/pywapor/collect/product/STATICS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    20115 2023-02-02 15:28:01.000000 pywapor-3.3.3/pywapor/collect/product/VIIRSL1.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      372 2023-01-10 14:54:30.000000 pywapor-3.3.3/pywapor/collect/product/__init__.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.985625 pywapor-3.3.3/pywapor/collect/protocol/
--rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/collect/protocol/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9062 2023-01-03 17:06:31.000000 pywapor-3.3.3/pywapor/collect/protocol/cds.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3928 2023-01-04 14:25:33.000000 pywapor-3.3.3/pywapor/collect/protocol/cog.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9848 2023-02-02 13:46:25.000000 pywapor-3.3.3/pywapor/collect/protocol/crawler.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9398 2023-02-02 12:46:35.000000 pywapor-3.3.3/pywapor/collect/protocol/opendap.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/collect/protocol/projections.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12012 2023-03-17 16:51:06.000000 pywapor-3.3.3/pywapor/collect/protocol/sentinelapi.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.988101 pywapor-3.3.3/pywapor/enhancers/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2022-09-30 08:36:06.000000 pywapor-3.3.3/pywapor/enhancers/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      886 2022-09-28 11:29:36.000000 pywapor-3.3.3/pywapor/enhancers/apply_enhancers.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2577 2023-01-04 13:41:38.000000 pywapor-3.3.3/pywapor/enhancers/dem.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.989355 pywapor-3.3.3/pywapor/enhancers/dms/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2022-09-30 08:43:00.000000 pywapor-3.3.3/pywapor/enhancers/dms/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    35799 2022-09-29 14:57:21.000000 pywapor-3.3.3/pywapor/enhancers/dms/pyDMS.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2022-09-16 14:57:12.000000 pywapor-3.3.3/pywapor/enhancers/dms/pyDMS_utils.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15442 2023-01-03 17:06:31.000000 pywapor-3.3.3/pywapor/enhancers/dms/thermal_sharpener.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2023-01-11 15:57:27.000000 pywapor-3.3.3/pywapor/enhancers/gap_fill.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2023-01-04 14:25:21.000000 pywapor-3.3.3/pywapor/enhancers/lulc.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2022-09-28 11:32:40.000000 pywapor-3.3.3/pywapor/enhancers/other.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2022-09-28 11:33:29.000000 pywapor-3.3.3/pywapor/enhancers/pressure.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.991566 pywapor-3.3.3/pywapor/enhancers/smooth/
--rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2023-03-02 12:28:19.000000 pywapor-3.3.3/pywapor/enhancers/smooth/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2023-04-04 12:24:13.000000 pywapor-3.3.3/pywapor/enhancers/smooth/archive.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5737 2023-04-04 12:36:23.000000 pywapor-3.3.3/pywapor/enhancers/smooth/core.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10591 2023-04-05 08:45:20.000000 pywapor-3.3.3/pywapor/enhancers/smooth/plotters.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12465 2023-04-05 08:45:08.000000 pywapor-3.3.3/pywapor/enhancers/smooth/whittaker.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2022-09-28 11:37:26.000000 pywapor-3.3.3/pywapor/enhancers/temperature.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2022-09-28 11:39:56.000000 pywapor-3.3.3/pywapor/enhancers/wind.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    18917 2023-01-17 16:22:18.000000 pywapor-3.3.3/pywapor/et_look.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.995456 pywapor-3.3.3/pywapor/et_look_dev/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7291 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1221 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/biomass.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12699 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/clear_sky_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3840 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/constants.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5939 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/evapotranspiration.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     6371 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/et_look_dev/leaf.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    28680 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/et_look_dev/meteo.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7133 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/neutral.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13821 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     4357 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_dev/resistance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7562 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/et_look_dev/roughness.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    31961 2022-08-23 08:30:34.000000 pywapor-3.3.3/pywapor/et_look_dev/soil_moisture.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    33779 2022-09-19 16:03:01.000000 pywapor-3.3.3/pywapor/et_look_dev/solar_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5671 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/et_look_dev/stress.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    21516 2023-01-26 11:30:09.000000 pywapor-3.3.3/pywapor/et_look_dev/unstable.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:31.000485 pywapor-3.3.3/pywapor/et_look_v2_v3/
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2022-08-23 08:57:05.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2022-06-23 15:01:24.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/biomass.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2022-08-30 08:32:15.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/clear_sky_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/constants.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2022-08-23 08:57:03.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/evapotranspiration.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2022-08-23 07:31:32.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/leaf.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2022-08-30 08:24:51.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/meteo.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2022-08-23 08:57:00.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/neutral.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2022-08-23 08:56:51.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2022-06-23 13:36:53.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/resistance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7345 2023-01-05 10:38:52.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/roughness.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2022-08-30 08:22:31.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/soil_moisture.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2022-09-19 16:35:35.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/solar_radiation.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/stress.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    23799 2022-08-31 14:11:30.000000 pywapor-3.3.3/pywapor/et_look_v2_v3/unstable.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:31.004253 pywapor-3.3.3/pywapor/general/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      294 2022-09-21 12:21:59.000000 pywapor-3.3.3/pywapor/general/__init__.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     8550 2023-04-05 08:51:56.000000 pywapor-3.3.3/pywapor/general/aligner.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2022-06-30 13:24:46.000000 pywapor-3.3.3/pywapor/general/bitmasks.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12833 2023-04-04 12:14:45.000000 pywapor-3.3.3/pywapor/general/compositer.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7399 2022-10-18 09:02:44.000000 pywapor-3.3.3/pywapor/general/curvilinear.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2023-01-05 09:12:37.000000 pywapor-3.3.3/pywapor/general/lazifier.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    28510 2023-04-04 12:34:47.000000 pywapor-3.3.3/pywapor/general/levels.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1589 2022-12-20 11:10:00.000000 pywapor-3.3.3/pywapor/general/logger.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    11401 2022-09-28 10:51:57.000000 pywapor-3.3.3/pywapor/general/network.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2352 2022-09-28 10:56:25.000000 pywapor-3.3.3/pywapor/general/performance.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2023-01-06 12:39:34.000000 pywapor-3.3.3/pywapor/general/pre_defaults.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    16701 2023-04-04 09:46:53.000000 pywapor-3.3.3/pywapor/general/processing_functions.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    12556 2023-02-02 12:48:00.000000 pywapor-3.3.3/pywapor/general/reproject.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2022-06-23 13:41:57.000000 pywapor-3.3.3/pywapor/general/units.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2023-01-05 08:22:50.000000 pywapor-3.3.3/pywapor/general/variables.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2022-08-26 10:45:16.000000 pywapor-3.3.3/pywapor/post_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7145 2023-01-10 14:36:33.000000 pywapor-3.3.3/pywapor/pre_et_look.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)     7018 2023-01-06 12:34:19.000000 pywapor-3.3.3/pywapor/pre_se_root.py
--rw-r--r--   0 hmcoerver   (501) staff       (20)    14976 2023-01-04 08:27:07.000000 pywapor-3.3.3/pywapor/se_root.py
-drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-05 09:01:30.959288 pywapor-3.3.3/pywapor.egg-info/
--rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-04-05 09:01:30.000000 pywapor-3.3.3/pywapor.egg-info/PKG-INFO
--rw-r--r--   0 hmcoerver   (501) staff       (20)     3495 2023-04-05 09:01:30.000000 pywapor-3.3.3/pywapor.egg-info/SOURCES.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2023-04-05 09:01:30.000000 pywapor-3.3.3/pywapor.egg-info/dependency_links.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)      280 2023-04-05 09:01:30.000000 pywapor-3.3.3/pywapor.egg-info/requires.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2023-04-05 09:01:30.000000 pywapor-3.3.3/pywapor.egg-info/top_level.txt
--rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2023-04-05 09:01:31.004818 pywapor-3.3.3/setup.cfg
--rw-r--r--   0 hmcoerver   (501) staff       (20)     2001 2023-04-05 08:59:44.000000 pywapor-3.3.3/setup.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.185048 pywapor-3.3.4/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11323 2022-06-23 13:36:53.000000 pywapor-3.3.4/LICENSE
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      229 2022-08-29 07:22:20.000000 pywapor-3.3.4/MANIFEST.in
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-04-26 14:18:25.184918 pywapor-3.3.4/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11246 2023-04-05 09:03:16.000000 pywapor-3.3.4/README.md
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.139938 pywapor-3.3.4/pywapor/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      416 2023-04-26 10:51:30.000000 pywapor-3.3.4/pywapor/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.141391 pywapor-3.3.4/pywapor/collect/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      241 2022-09-28 07:45:21.000000 pywapor-3.3.4/pywapor/collect/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13487 2023-01-25 04:36:11.000000 pywapor-3.3.4/pywapor/collect/accounts.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9150 2023-01-12 09:57:39.000000 pywapor-3.3.4/pywapor/collect/downloader.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.159371 pywapor-3.3.4/pywapor/collect/product/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5802 2023-01-05 11:26:49.000000 pywapor-3.3.4/pywapor/collect/product/CHIRPS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8172 2023-04-14 12:52:07.000000 pywapor-3.3.4/pywapor/collect/product/COPERNICUS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8387 2022-09-29 11:29:30.000000 pywapor-3.3.4/pywapor/collect/product/ERA5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6154 2023-04-19 09:01:02.000000 pywapor-3.3.4/pywapor/collect/product/GEOS5.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1110900 2022-08-24 12:33:55.000000 pywapor-3.3.4/pywapor/collect/product/GLO30.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1111950 2022-08-24 12:33:41.000000 pywapor-3.3.4/pywapor/collect/product/GLO90.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5808 2023-01-06 12:00:32.000000 pywapor-3.3.4/pywapor/collect/product/GLOBCOVER.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    40234 2023-01-25 04:40:44.000000 pywapor-3.3.4/pywapor/collect/product/LANDSAT.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.164824 pywapor-3.3.4/pywapor/collect/product/Landsat/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    25684 2022-09-28 09:16:32.000000 pywapor-3.3.4/pywapor/collect/product/Landsat/C2L2SP.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      250 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/product/Landsat/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8549 2023-01-05 10:39:18.000000 pywapor-3.3.4/pywapor/collect/product/MERRA2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13898 2023-02-10 10:58:24.000000 pywapor-3.3.4/pywapor/collect/product/MODIS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  1232314 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/product/MODIS_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11566 2023-01-04 09:31:52.000000 pywapor-3.3.4/pywapor/collect/product/PROBAV.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    23350 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/collect/product/SENTINEL2.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6555 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/collect/product/SENTINEL3.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7297 2022-12-22 13:02:32.000000 pywapor-3.3.4/pywapor/collect/product/SRTM.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)  3610761 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/product/SRTM30_tiles.geojson
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7204 2023-01-05 10:39:59.000000 pywapor-3.3.4/pywapor/collect/product/STATICS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    20125 2023-04-13 12:04:14.000000 pywapor-3.3.4/pywapor/collect/product/VIIRSL1.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      372 2023-01-10 14:54:30.000000 pywapor-3.3.4/pywapor/collect/product/__init__.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.166393 pywapor-3.3.4/pywapor/collect/protocol/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       33 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/protocol/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9062 2023-01-03 17:06:31.000000 pywapor-3.3.4/pywapor/collect/protocol/cds.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3904 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/collect/protocol/cog.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9912 2023-04-19 08:49:47.000000 pywapor-3.3.4/pywapor/collect/protocol/crawler.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9446 2023-04-19 09:02:03.000000 pywapor-3.3.4/pywapor/collect/protocol/opendap.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1572 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/collect/protocol/projections.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12012 2023-03-17 16:51:06.000000 pywapor-3.3.4/pywapor/collect/protocol/sentinelapi.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.168783 pywapor-3.3.4/pywapor/enhancers/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      223 2022-09-30 08:36:06.000000 pywapor-3.3.4/pywapor/enhancers/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      886 2022-09-28 11:29:36.000000 pywapor-3.3.4/pywapor/enhancers/apply_enhancers.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2577 2023-01-04 13:41:38.000000 pywapor-3.3.4/pywapor/enhancers/dem.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.170422 pywapor-3.3.4/pywapor/enhancers/dms/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      175 2022-09-30 08:43:00.000000 pywapor-3.3.4/pywapor/enhancers/dms/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    36143 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/enhancers/dms/pyDMS.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10174 2022-09-16 14:57:12.000000 pywapor-3.3.4/pywapor/enhancers/dms/pyDMS_utils.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15479 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/enhancers/dms/thermal_sharpener.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2066 2023-01-11 15:57:27.000000 pywapor-3.3.4/pywapor/enhancers/gap_fill.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8897 2023-01-04 14:25:21.000000 pywapor-3.3.4/pywapor/enhancers/lulc.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      616 2022-09-28 11:32:40.000000 pywapor-3.3.4/pywapor/enhancers/other.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      348 2022-09-28 11:33:29.000000 pywapor-3.3.4/pywapor/enhancers/pressure.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.171934 pywapor-3.3.4/pywapor/enhancers/smooth/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        0 2023-03-02 12:28:19.000000 pywapor-3.3.4/pywapor/enhancers/smooth/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    17945 2023-04-04 12:24:13.000000 pywapor-3.3.4/pywapor/enhancers/smooth/archive.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6710 2023-04-26 10:49:45.000000 pywapor-3.3.4/pywapor/enhancers/smooth/core.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10601 2023-04-25 10:30:52.000000 pywapor-3.3.4/pywapor/enhancers/smooth/plotters.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13564 2023-04-25 12:17:43.000000 pywapor-3.3.4/pywapor/enhancers/smooth/whittaker.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    10210 2022-09-28 11:37:26.000000 pywapor-3.3.4/pywapor/enhancers/temperature.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1003 2022-09-28 11:39:56.000000 pywapor-3.3.4/pywapor/enhancers/wind.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    18917 2023-01-17 16:22:18.000000 pywapor-3.3.4/pywapor/et_look.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.176347 pywapor-3.3.4/pywapor/et_look_dev/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7291 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1221 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/biomass.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12699 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/clear_sky_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3840 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/constants.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5939 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/evapotranspiration.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     6371 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/leaf.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    28680 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/meteo.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7133 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/neutral.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13821 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     4357 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_dev/resistance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7562 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/roughness.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    31961 2022-08-23 08:30:34.000000 pywapor-3.3.4/pywapor/et_look_dev/soil_moisture.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    33779 2022-09-19 16:03:01.000000 pywapor-3.3.4/pywapor/et_look_dev/solar_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5671 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_dev/stress.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    21516 2023-01-26 11:30:09.000000 pywapor-3.3.4/pywapor/et_look_dev/unstable.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.180328 pywapor-3.3.4/pywapor/et_look_v2_v3/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7216 2022-08-23 08:57:05.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     9037 2022-06-23 15:01:24.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/biomass.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12950 2022-08-30 08:32:15.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/clear_sky_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3891 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/constants.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5008 2022-08-23 08:57:03.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/evapotranspiration.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5403 2022-08-23 07:31:32.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/leaf.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    31410 2022-08-30 08:24:51.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/meteo.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7248 2022-08-23 08:57:00.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/neutral.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    13996 2022-08-23 08:56:51.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3833 2022-06-23 13:36:53.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/resistance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7345 2023-01-05 10:38:52.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/roughness.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32038 2022-08-30 08:22:31.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/soil_moisture.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    15852 2022-09-19 16:35:35.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/solar_radiation.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     5011 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/stress.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    23799 2022-08-31 14:11:30.000000 pywapor-3.3.4/pywapor/et_look_v2_v3/unstable.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.184538 pywapor-3.3.4/pywapor/general/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      294 2022-09-21 12:21:59.000000 pywapor-3.3.4/pywapor/general/__init__.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     8550 2023-04-14 09:51:55.000000 pywapor-3.3.4/pywapor/general/aligner.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    22239 2022-06-30 13:24:46.000000 pywapor-3.3.4/pywapor/general/bitmasks.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12818 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/general/compositer.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7414 2023-04-13 13:02:47.000000 pywapor-3.3.4/pywapor/general/curvilinear.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3065 2023-01-05 09:12:37.000000 pywapor-3.3.4/pywapor/general/lazifier.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    28534 2023-04-13 09:53:40.000000 pywapor-3.3.4/pywapor/general/levels.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2103 2023-04-13 09:40:27.000000 pywapor-3.3.4/pywapor/general/logger.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    11401 2022-09-28 10:51:57.000000 pywapor-3.3.4/pywapor/general/network.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2352 2022-09-28 10:56:25.000000 pywapor-3.3.4/pywapor/general/performance.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     1885 2023-01-06 12:39:34.000000 pywapor-3.3.4/pywapor/general/pre_defaults.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    16701 2023-04-04 09:46:53.000000 pywapor-3.3.4/pywapor/general/processing_functions.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    12552 2023-04-12 12:40:20.000000 pywapor-3.3.4/pywapor/general/reproject.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2538 2022-06-23 13:41:57.000000 pywapor-3.3.4/pywapor/general/units.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    32644 2023-01-05 08:22:50.000000 pywapor-3.3.4/pywapor/general/variables.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    18087 2022-08-26 10:45:16.000000 pywapor-3.3.4/pywapor/post_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7145 2023-01-10 14:36:33.000000 pywapor-3.3.4/pywapor/pre_et_look.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     7014 2023-04-14 09:20:37.000000 pywapor-3.3.4/pywapor/pre_se_root.py
+-rw-r--r--   0 hmcoerver   (501) staff       (20)    14976 2023-01-04 08:27:07.000000 pywapor-3.3.4/pywapor/se_root.py
+drwxr-xr-x   0 hmcoerver   (501) staff       (20)        0 2023-04-26 14:18:25.140725 pywapor-3.3.4/pywapor.egg-info/
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      457 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/PKG-INFO
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     3495 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/SOURCES.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        1 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/dependency_links.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)      280 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/requires.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)        8 2023-04-26 14:18:25.000000 pywapor-3.3.4/pywapor.egg-info/top_level.txt
+-rw-r--r--   0 hmcoerver   (501) staff       (20)       38 2023-04-26 14:18:25.185086 pywapor-3.3.4/setup.cfg
+-rw-r--r--   0 hmcoerver   (501) staff       (20)     2001 2023-04-26 10:51:26.000000 pywapor-3.3.4/setup.py
```

### Comparing `pywapor-3.3.3/LICENSE` & `pywapor-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/README.md` & `pywapor-3.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,24 +69,19 @@
       <tr class="row-odd">
          <td>3.</td>
          <td>Composites</td>
          <td style="text-align:center"><a href="https://colab.research.google.com/github/bertcoerver/pywapor_notebooks/blob/main/3_composites.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"/></a></td>
       </tr>
       <tr class="row-even">
          <td>4.</td>
-         <td>Sideloading</td>
-         <td style="text-align:center"><a href="https://colab.research.google.com/github/bertcoerver/pywapor_notebooks/blob/main/4_sideloading.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"/></a></td>
-      </tr>
-      <tr class="row-odd">
-         <td>5.</td>
          <td>Enhancers</td>
          <td style="text-align:center"><a href="https://colab.research.google.com/github/bertcoerver/pywapor_notebooks/blob/main/5_enhancers.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"/></a></td>
       </tr>
-      <tr class="row-even">
-         <td>6.</td>
+      <tr class="row-odd">
+         <td>5.</td>
          <td>pyWaPOR vs. WaPOR</td>
          <td style="text-align:center"><a href="https://colab.research.google.com/github/bertcoerver/pywapor_notebooks/blob/main/6_wapor_vs_pywapor.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"/></a></td>
       </tr>
    </tbody>
 </table>
 
 #### WaPOR v3
```

#### html2text {}

```diff
@@ -29,17 +29,16 @@
 the notebooks below to learn more! ### Documentation Go [here](https://
 www.fao.org/aquastat/py-wapor/) for the full pyWaPOR documentation. ####
 Notebooks
    Name              Colab
 1. Introduction      [colab]
 2. Levels            [colab]
 3. Composites        [colab]
-4. Sideloading       [colab]
-5. Enhancers         [colab]
-6. pyWaPOR vs. WaPOR [colab]
+4. Enhancers         [colab]
+5. pyWaPOR vs. WaPOR [colab]
 #### WaPOR v3
     * WaPOR-ETLook_Online_Manual_(v3)
 #### WaPOR v2
     * WaPOR-ETLook_Data_Manual_(v2)
     * WaPOR-Biomass_Data_Manual_(v2)
 #### WaPOR v1
     * WaPOR-ETLook_Data_Manual_(v1)
```

### Comparing `pywapor-3.3.3/pywapor/collect/accounts.py` & `pywapor-3.3.4/pywapor/collect/accounts.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/downloader.py` & `pywapor-3.3.4/pywapor/collect/downloader.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/CHIRPS.py` & `pywapor-3.3.4/pywapor/collect/product/CHIRPS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/COPERNICUS.py` & `pywapor-3.3.4/pywapor/collect/product/COPERNICUS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/ERA5.py` & `pywapor-3.3.4/pywapor/collect/product/ERA5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/GEOS5.py` & `pywapor-3.3.4/pywapor/collect/product/GEOS5.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/GLO30.txt` & `pywapor-3.3.4/pywapor/collect/product/GLO30.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/GLO90.txt` & `pywapor-3.3.4/pywapor/collect/product/GLO90.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/GLOBCOVER.py` & `pywapor-3.3.4/pywapor/collect/product/GLOBCOVER.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/LANDSAT.py` & `pywapor-3.3.4/pywapor/collect/product/LANDSAT.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/Landsat/C2L2SP.py` & `pywapor-3.3.4/pywapor/collect/product/Landsat/C2L2SP.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/MERRA2.py` & `pywapor-3.3.4/pywapor/collect/product/MERRA2.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/MODIS.py` & `pywapor-3.3.4/pywapor/collect/product/MODIS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/MODIS_tiles.geojson` & `pywapor-3.3.4/pywapor/collect/product/MODIS_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/PROBAV.py` & `pywapor-3.3.4/pywapor/collect/product/PROBAV.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/SENTINEL2.py` & `pywapor-3.3.4/pywapor/collect/product/SENTINEL2.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
         Filename.
 
     Returns
     -------
     np.datetime64
         Date as described in the filename.
     """
-    dtime = np.datetime64(dt.strptime(fn.split("_")[2], "%Y%m%dT%H%M%S"))
+    dtime = np.datetime64(dt.strptime(fn.split("_")[2], "%Y%m%dT%H%M%S"), "ns")
     return dtime
 
 def s2_processor(scene_folder, variables):
 
     dss = [open_ds(glob.glob(os.path.join(scene_folder, "**", "*" + k), recursive = True)[0], decode_coords=None).isel(band=0).rename({"band_data": v[1]}) for k, v in variables.items()]
     ds = xr.merge(dss).drop_vars("band")
```

### Comparing `pywapor-3.3.3/pywapor/collect/product/SENTINEL3.py` & `pywapor-3.3.4/pywapor/collect/product/SENTINEL3.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         Filename.
 
     Returns
     -------
     np.datetime64
         Date as described in the filename.
     """
-    start_dtime = np.datetime64(dt.strptime(fn.split("_")[7], "%Y%m%dT%H%M%S"))
-    end_dtime = np.datetime64(dt.strptime(fn.split("_")[8], "%Y%m%dT%H%M%S"))
+    start_dtime = np.datetime64(dt.strptime(fn.split("_")[7], "%Y%m%dT%H%M%S"), "ns")
+    end_dtime = np.datetime64(dt.strptime(fn.split("_")[8], "%Y%m%dT%H%M%S"), "ns")
     dtime = start_dtime + (end_dtime - start_dtime)/2
     return dtime
 
 def s3_processor(scene_folder, variables, bb = None, **kwargs):
 
     ncs = [glob.glob(os.path.join(scene_folder, "**", "*" + k), recursive = True)[0] for k in variables.keys()]
```

### Comparing `pywapor-3.3.3/pywapor/collect/product/SRTM.py` & `pywapor-3.3.4/pywapor/collect/product/SRTM.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/SRTM30_tiles.geojson` & `pywapor-3.3.4/pywapor/collect/product/SRTM30_tiles.geojson`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/STATICS.py` & `pywapor-3.3.4/pywapor/collect/product/STATICS.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/product/VIIRSL1.py` & `pywapor-3.3.4/pywapor/collect/product/VIIRSL1.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         buffer = 0.2
         mask = ((ds.y >= bb[1] - buffer) &
                 (ds.y <= bb[3] + buffer) & 
                 (ds.x >= bb[0] - buffer) & 
                 (ds.x <= bb[2] + buffer))
 
         # Apply the mask.
-        ds = ds.where(mask, drop = True)
+        ds = ds.where(mask.compute(), drop = True)
 
         # Stop with scene if no valid data is found inside bb.
         if ds.bt.count().values == 0:
             log.warning(f"--> ({i+1}/{len(scenes)}) Skipping scene `{os.path.split(fp)[-1]}`, no valid data found inside bounding-box.")
             continue
 
         # Save intermediate file.
```

### Comparing `pywapor-3.3.3/pywapor/collect/protocol/cds.py` & `pywapor-3.3.4/pywapor/collect/protocol/cds.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/protocol/cog.py` & `pywapor-3.3.4/pywapor/collect/protocol/cog.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,19 +82,19 @@
 
     # Check if path is free.
     temp_path = fp.replace(".nc", "_temp.nc")
     while os.path.isfile(temp_path):
         temp_path = temp_path.replace(".nc", "_.nc")
 
     # Run gdal.Translate.
-    ds = gdal.Translate(temp_path, url, options = options)
+    ds_ = gdal.Translate(temp_path, url, options = options)
 
     # Reset the gdal.Dataset.
-    ds.FlushCache()
-    ds = None
+    ds_.FlushCache()
+    ds_ = None
 
     # Process the new netCDF.
     ds = open_ds(temp_path)
 
     # TODO Also check COPERNICUS and GLOBCOVER...
     if int(gdal.__version__.split(".")[0]) < 3 and "WaPOR" in product_name:
         # NOTE this is terrible, but Google Colab uses a 7 year old GDAL version in 
@@ -112,11 +112,10 @@
             ds, label = apply_enhancer(ds, var, func)
             # log.info(label)
 
     # Save final output.
     out = save_ds(ds, fp, encoding = "initiate", label = f"Saving {fn}.")
 
     # Remove the temporary file.
-    ds = ds.close()
-    remove_ds(temp_path)
+    remove_ds(ds)
 
     return out
```

### Comparing `pywapor-3.3.3/pywapor/collect/protocol/crawler.py` & `pywapor-3.3.4/pywapor/collect/protocol/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,30 +219,30 @@
             log.info(f"--> Retrying to download {len(urls)} remaining urls.")
 
     if len(urls) > 0:
         log.warning(f"--> Didn't succeed to download {len(urls)} files.")
     return relevant_fps
 
 
-def _download_url(url, fp, session = None, waitbar = True, headers = None):
+def _download_url(url, fp, session = None, waitbar = True, headers = None, verify = True):
 
     if os.path.isfile(fp):
         return fp
 
     folder, fn = os.path.split(fp)
     if not os.path.exists(folder):
         os.makedirs(folder)
 
     ext = os.path.splitext(fp)[-1]
     temp_fp = fp.replace(ext, "_temp")
 
     if isinstance(session, type(None)):
         session = requests.Session()
 
-    file_object = session.get(url, stream = True, headers = headers)
+    file_object = session.get(url, stream = True, headers = headers, verify = verify)
     file_object.raise_for_status()
 
     if "Content-Length" in file_object.headers.keys():
         tot_size = int(file_object.headers["Content-Length"])
     else:
         tot_size = None
 
@@ -257,15 +257,15 @@
                 wb.update(size)
 
     os.rename(temp_fp, fp)
 
     return fp
 
 def download_url(url, fp, session = None, waitbar = True, headers = None, 
-                    max_tries = 3, wait_sec = 15):
+                    max_tries = 3, wait_sec = 15, verify = True):
     """Download a URL to a file.
 
     Parameters
     ----------
     url : str
         URL to download.
     fp : str
@@ -295,15 +295,15 @@
     succes = False
     while try_n <= max_tries-1 and not succes:
         if try_n > 0:
             waiter = int((try_n**1.2) * wait_sec)
             log.info(f"--> Trying to download {fp}, attempt {try_n+1} of {max_tries} in {waiter} seconds.")
             time.sleep(waiter)
         try:
-            fp = _download_url(url, fp, session = session, waitbar = waitbar, headers = headers)
+            fp = _download_url(url, fp, session = session, waitbar = waitbar, headers = headers, verify = verify)
             succes = True
         except socket.timeout as e:
             log.info(f"--> Server connection timed out.")
         except HTTPError as e:
             error_body = getattr(getattr(e, "response", ""), "text", "")
             log.info(f"--> Server error {e} [{error_body}].")
         else:
```

### Comparing `pywapor-3.3.3/pywapor/collect/protocol/opendap.py` & `pywapor-3.3.4/pywapor/collect/protocol/opendap.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,21 +113,21 @@
     # Remove temporary files.
     if not isinstance(dss, type(None)):
         for x in dss:
             remove_ds(x)
 
     return ds
 
-def find_idxs(base_url, selection, session):
+def find_idxs(base_url, selection, session, verify = True):
     def _find_idxs(ds, k, search_range):
         all_idxs = np.where((ds[k] >= search_range[0]) & (ds[k] <= search_range[1]))[0]
         return [np.min(all_idxs), np.max(all_idxs)]
     fp = tempfile.NamedTemporaryFile(suffix=".nc").name
     url_coords = base_url + urllib.parse.quote(",".join(selection.keys()))
-    fp = download_url(url_coords, fp, session, waitbar = False)
+    fp = download_url(url_coords, fp, session, waitbar = False, verify = verify)
     ds = xr.open_dataset(fp, decode_coords = "all")
     idxs = {k: _find_idxs(ds, k, v) for k, v in selection.items()}
     return idxs
 
 def create_url(base_url, idxs, variables, request_dims = True):
     if request_dims:
         dims = [f"{k}[{v[0]}:{v[1]}]" for k, v in idxs.items()]
@@ -137,15 +137,15 @@
     url = base_url + urllib.parse.quote(",".join(dims + varis))
     return url
 
 def start_session(base_url, selection, un_pw = [None, None]):
     if un_pw == [None, None]:
         warnings.filterwarnings("ignore", "password was not set. ")
     url_coords = base_url + urllib.parse.quote(",".join(selection.keys()))
-    session = setup_session(*un_pw, check_url = url_coords)
+    session = setup_session(*un_pw, check_url = url_coords, verify = False)
     return session
 
 def download_xarray(url, fp, coords, variables, post_processors, 
                     data_source_crs = None, timedelta = None):
     """Download a OPENDaP dataset using xarray directly.
 
     Parameters
```

### Comparing `pywapor-3.3.3/pywapor/collect/protocol/projections.py` & `pywapor-3.3.4/pywapor/collect/protocol/projections.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/collect/protocol/sentinelapi.py` & `pywapor-3.3.4/pywapor/collect/protocol/sentinelapi.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/apply_enhancers.py` & `pywapor-3.3.4/pywapor/enhancers/apply_enhancers.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/dem.py` & `pywapor-3.3.4/pywapor/enhancers/dem.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/dms/pyDMS.py` & `pywapor-3.3.4/pywapor/enhancers/dms/pyDMS.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import math
 import os
 import numpy as np
 from osgeo import gdal
 from sklearn import tree, linear_model, ensemble
 import pywapor.enhancers.dms.pyDMS_utils as utils
 from pywapor.general.logger import log
+import warnings
 
 REG_sknn_ann = 0
 REG_sklearn_ann = 1
 
 class DecisionTreeRegressorWithLinearLeafRegression(tree.DecisionTreeRegressor):
     ''' Decision tree regressor with added linear (bayesian ridge) regression
     for all the data points falling within each decision tree leaf node.
@@ -591,24 +592,28 @@
         else:
             quality_LR = None
 
         residual_HR, residual_LR, gt_res = self._calculateResidual(scene_HR, scene_LR, quality_LR)
 
         if self.disaggregatingTemperature:
             if doCorrection:
-                corrected = (residual_HR + scene_HR.GetRasterBand(1).ReadAsArray()**4)**0.25
+                with warnings.catch_warnings():
+                    warnings.filterwarnings("ignore", message="invalid value encountered in power")                    
+                    corrected = (residual_HR + scene_HR.GetRasterBand(1).ReadAsArray()**4)**0.25
                 correctedImage = utils.saveImg(corrected,
                                                scene_HR.GetGeoTransform(),
                                                scene_HR.GetProjection(),
                                                "MEM",
                                                noDataValue=np.nan)
             else:
                 correctedImage = None
             # Convert residual back to temperature for easier visualisation
-            residual_LR = (residual_LR + 273.15**4)**0.25 - 273.15
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore", message="invalid value encountered in power")            
+                residual_LR = (residual_LR + 273.15**4)**0.25 - 273.15
         else:
             if doCorrection:
                 corrected = residual_HR + scene_HR.GetRasterBand(1).ReadAsArray()
                 correctedImage = utils.saveImg(corrected,
                                                scene_HR.GetGeoTransform(),
                                                scene_HR.GetProjection(),
                                                "MEM",
```

### Comparing `pywapor-3.3.3/pywapor/enhancers/dms/pyDMS_utils.py` & `pywapor-3.3.4/pywapor/enhancers/dms/pyDMS_utils.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/dms/thermal_sharpener.py` & `pywapor-3.3.4/pywapor/enhancers/dms/thermal_sharpener.py`

 * *Files 3% similar despite different names*

```diff
@@ -273,31 +273,32 @@
             os.remove(highResFilename)
             os.remove(lowResFilename)
         except PermissionError as e:
             ... # NOTE windows...
 
     log.sub()
 
-    ds = xr.open_mfdataset(out_fns, preprocess = preprocess, decode_coords = "all")
-    ds = ds.rename_dims({"lat": "y", "lon": "x"})
-    ds = ds.transpose("time", "y", "x")
-    ds = ds.rename_vars({"crs": "spatial_ref", "Band1": var, "lat": "y", "lon": "x"})
-    ds = ds.rio.write_grid_mapping("spatial_ref")
-    ds = ds.sortby("y", ascending = False)
-    ds = ds.sortby("x")
-    ds.attrs = {}
+    dss_ = [preprocess(open_ds(x)) for x in out_fns]
+    ds_ = xr.concat(dss_, dim = "time").sortby("time")
+    ds_ = ds_.rename_dims({"lat": "y", "lon": "x"})
+    ds_ = ds_.transpose("time", "y", "x")
+    ds_ = ds_.rename_vars({"crs": "spatial_ref", "Band1": var, "lat": "y", "lon": "x"})
+    ds_ = ds_.rio.write_grid_mapping("spatial_ref")
+    ds_ = ds_.sortby("y", ascending = False)
+    ds_ = ds_.sortby("x")
+    ds_.attrs = {}
 
     fp = os.path.join(workdir, f"{var}_i.nc")
 
-    ds = save_ds(ds, fp, encoding = "initiate", label = f"Merging sharpened `{var}` files.")
+    ds = save_ds(ds_, fp, encoding = "initiate", label = f"Merging sharpened `{var}` files.")
 
-    ds = ds.close()
+    ds_ = ds_.close()
     dss[var] = fp
 
-    for x in out_fns:
+    for x in dss_:
         remove_ds(x)
     
     if 'cos_solar_zangle' in dss.keys() and remove_cos_solar_zangle:
         remove_ds(dss['cos_solar_zangle'])
 
     for x in vars_for_sharpening:
         if x in dss.keys():
```

### Comparing `pywapor-3.3.3/pywapor/enhancers/gap_fill.py` & `pywapor-3.3.4/pywapor/enhancers/gap_fill.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/lulc.py` & `pywapor-3.3.4/pywapor/enhancers/lulc.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/other.py` & `pywapor-3.3.4/pywapor/enhancers/other.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/smooth/archive.py` & `pywapor-3.3.4/pywapor/enhancers/smooth/archive.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/smooth/core.py` & `pywapor-3.3.4/pywapor/enhancers/smooth/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,18 +90,21 @@
 def dist_to_finite(y, x, axis = -1, extrapolate = False):
     def _dtf(y, x, extrapolate = False):
         # NOTE could also use `xarray.core.missing._get_nan_block_lengths instead` (similar, but not exactly the same)
         # NOTE can use numba when this is resolved https://github.com/numba/numba/issues/1269
         part1 = np.expand_dims(np.extract(np.isfinite(y), x), 1)
         part2 = np.expand_dims(x, 0)
         distances = part2 - part1
-        dist = np.min(np.abs(distances), axis = 0, initial = x[-1]-x[0])
+        dist = np.min(np.abs(distances), axis = 0, initial = np.timedelta64(365, "D"))
         if not extrapolate and distances.size != 0:
-            mask = np.ptp(np.sign(distances), axis = 0).astype(int) > 0
-            dist = np.where(mask, dist, x[-1]-x[0])
+            if distances.shape[0] > 1:
+                mask = np.ptp(np.sign(distances), axis = 0).astype(int) > 0
+            else:
+                mask = np.isfinite(y)
+            dist = np.where(mask, dist, np.timedelta64(365, "D"))
         return dist
     out = np.apply_along_axis(_dtf, axis, y, x, extrapolate = extrapolate)
     return out
 
 def cve0(lmbdas, Y, A):
     def _cve(lmbdas, Y, A):
         assert len(Y.shape) == 1
@@ -124,7 +127,38 @@
     W = np.diag(w*u)
     Y_ = np.where(w == 0, 0, Y)
     for i, lmbda in enumerate(lmbdas):
         H = np.linalg.solve(W + lmbda * A, W) # Eq. 13
         y_hat = np.dot(H, Y_) # Eq. 10
         hii = np.diag(H)
         cves[i,...] = np.sqrt(np.nanmean(((Y - y_hat)/(1 - hii))**2)) # Eq. 9 + 11
+
+# if __name__ == "__main__":
+
+#     import xarray as xr
+#     from pywapor.general.processing_functions import open_ds
+
+#     # fh = r"/Users/hmcoerver/Local/tests/test_22/SENTINEL2/S2MSI2A_R60m.nc"
+#     fh = r"/Users/hmcoerver/Local/tests/test_22/VIIRSL1/VNP02IMG.nc"
+#     ds = open_ds(fh)
+
+#     y = ds.isel(y=30, x= 30).bt.values
+#     x = ds.time.values
+
+#     # Normalize x-coordinates
+#     x_ = (x - x.min()) / (x.max() - x.min()) * x.size
+
+#     # Create x-aware delta matrix.
+#     A = second_order_diff_matrix(x_)
+
+#     lmbdas = 100.
+#     min_drange = -np.inf
+#     max_drange = np.inf
+#     # min_drange = -1.
+#     # max_drange = 1.
+#     max_iter = 10
+#     u = np.ones(x.shape)
+#     a = 0.5
+
+#     z = wt(y, A, lmbdas, u, a, min_drange, max_drange, max_iter)
+
+#     xdist = dist_to_finite(y, x, axis = -1, extrapolate = False)
```

### Comparing `pywapor-3.3.3/pywapor/enhancers/smooth/plotters.py` & `pywapor-3.3.4/pywapor/enhancers/smooth/plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     fig.colorbar(im1)
     fig.colorbar(im2)
     fig.subplots_adjust(left=None, bottom=None, right=None, top=0.91, wspace=None, hspace=0.3)
     fig.suptitle(np.datetime_as_string(ds.time[t_idx], unit='m'))
     fig.savefig(os.path.join(folder, f"{t_idx:>06}.png"))
     plt.close(fig)
 
-def make_overview(ds, var, plot_folder, points = None, point_method = "equally_spaced", n = 3, offset = 0.1):
+def make_overview(ds, var, plot_folder, points = None, point_method = "equally_spaced", n = 3, offset = 0.1, **kwargs):
 
     if isinstance(points, type(None)):
         if point_method == "equally_spaced":
             points = create_points(ds, n = n, offset = offset)
         elif point_method == "worst":
             points = create_worst_points(ds, f"{var}_smoothed", "time", n = n)
```

### Comparing `pywapor-3.3.3/pywapor/enhancers/smooth/whittaker.py` & `pywapor-3.3.4/pywapor/enhancers/smooth/whittaker.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         log.warning(f"--> Adjusting chunks to (`{chunks}`), to avoid chunks along core dimension ({xdim}).")
 
     # Chunk dataset.
     ds = ds.chunk(chunks)
 
     # Add new x values.
     if not isinstance(new_x, type(None)) and getattr(xdim, '__len__', lambda: 0)() > 0:
-        ds = xr.concat([ds, xr.Dataset({xdim: new_x})], dim = xdim).drop_duplicates(xdim).chunk(chunks).sortby(xdim).chunk(chunks)
+        ds = xr.merge([ds, xr.Dataset({xdim: new_x})]).drop_duplicates(xdim).chunk(chunks).sortby(xdim).chunk(chunks)
         if "sensor" in ds.data_vars:
             sensor_id = np.nanmax(np.unique(ds["sensor"])) + 1
             ds["sensor"] = ds["sensor"].fillna(sensor_id).assign_attrs({str(int(sensor_id)): "Interp."})
             if not isinstance(weights, type(None)):
                 weights["Interp."] = 0.0
 
     # Add lmbdas as coordinate.
@@ -266,14 +266,17 @@
 
     # Drop irrelevant data.
     if not export_all:
         ds = ds[[f"{var}_smoothed"]]
         if not isinstance(new_x, type(None)) and getattr(xdim, '__len__', lambda: 0)() > 0:
             ds = ds.sel({xdim: new_x})
 
+    # Make sure the dimensions are in the correct order. TODO Maybe move this inside `save_ds`.
+    ds = ds.transpose("time", "y", "x", ...)
+
     if not isinstance(out_fh, type(None)):
         ds = save_ds(ds, out_fh, encoding = "initiate", label = f"Applying whittaker smoothing ({var}).")
 
     # Give warnings if data is outside of defined range.
     if not np.isinf(valid_drange[0]):
         min_bound = float(ds[f"{var}_smoothed"].min().values)
         if min_bound < valid_drange[0]:
@@ -286,22 +289,43 @@
 
     return ds
 
 if __name__ == "__main__":
 
     import matplotlib.pyplot as plt
 
-    ds = open_ds(r"/Users/hmcoerver/Desktop/test.nc")[["ndvi"]].drop_vars("lmbda")
+    ds = open_ds(r"/Users/hmcoerver/Local/poster_whit_data/consolidated_data.nc")
 
-    var = "ndvi"
+    ds.sensor.attrs["3"] = 'MOD13Q1.061'
+    ds.sensor.attrs["4"] = 'MYD13Q1.061'
 
+    _new_x = ds["new_x"].values
+    ds = ds.drop_vars("new_x").unify_chunks()
+
+    var = "ndvi"
     lmbdas = 100.
     weights = None
     a = 0.5
     max_iter = 10
-    out_fh = None
+    out_fh = r"/Users/hmcoerver/Local/poster_whit_data/out_data.nc"
     xdim = "time"
     max_dist = None
     new_x = None
-    export_all = False
+    export_all = True
     chunks = {}
-    valid_drange = [-np.inf, np.inf]
+    valid_drange = [-1.0, 1.0]
+    kwargs = {
+        "plot_folder": r"/Users/hmcoerver/Local/poster_whit_data/graphs",
+    }
+
+    out = whittaker_smoothing(ds, var, lmbdas = lmbdas, weights = weights, a = a, 
+                        max_iter = max_iter, out_fh = out_fh, xdim = xdim, max_dist = max_dist,
+                        new_x = new_x, export_all = export_all, chunks = chunks, make_plots = None,
+                        valid_drange = valid_drange, **kwargs)
+
+    import matplotlib.pyplot as plt
+    from pywapor.enhancers.smooth.plotters import plot_point
+
+    fig = plt.figure(figsize = (10, 5))
+    ax = fig.gca()
+    point_ds = out.sel(x = 30.725, y = 29.410, method = "nearest")
+    plot_point(ax, point_ds.compute(), var, ylim = [-0.2, 1], t_idx = None, title = True, xtick = True)
```

### Comparing `pywapor-3.3.3/pywapor/enhancers/temperature.py` & `pywapor-3.3.4/pywapor/enhancers/temperature.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/enhancers/wind.py` & `pywapor-3.3.4/pywapor/enhancers/wind.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look.py` & `pywapor-3.3.4/pywapor/et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/__init__.py` & `pywapor-3.3.4/pywapor/et_look_dev/__init__.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/biomass.py` & `pywapor-3.3.4/pywapor/et_look_dev/biomass.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/clear_sky_radiation.py` & `pywapor-3.3.4/pywapor/et_look_dev/clear_sky_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/constants.py` & `pywapor-3.3.4/pywapor/et_look_dev/constants.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/evapotranspiration.py` & `pywapor-3.3.4/pywapor/et_look_dev/evapotranspiration.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/leaf.py` & `pywapor-3.3.4/pywapor/et_look_dev/leaf.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/meteo.py` & `pywapor-3.3.4/pywapor/et_look_dev/meteo.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/neutral.py` & `pywapor-3.3.4/pywapor/et_look_dev/neutral.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/radiation.py` & `pywapor-3.3.4/pywapor/et_look_dev/radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/resistance.py` & `pywapor-3.3.4/pywapor/et_look_dev/resistance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/roughness.py` & `pywapor-3.3.4/pywapor/et_look_dev/roughness.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/soil_moisture.py` & `pywapor-3.3.4/pywapor/et_look_dev/soil_moisture.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/solar_radiation.py` & `pywapor-3.3.4/pywapor/et_look_dev/solar_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/stress.py` & `pywapor-3.3.4/pywapor/et_look_dev/stress.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_dev/unstable.py` & `pywapor-3.3.4/pywapor/et_look_dev/unstable.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/__init__.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/biomass.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/biomass.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/clear_sky_radiation.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/clear_sky_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/constants.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/constants.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/evapotranspiration.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/evapotranspiration.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/leaf.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/leaf.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/meteo.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/meteo.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/neutral.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/neutral.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/radiation.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/resistance.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/resistance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/roughness.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/roughness.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/soil_moisture.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/soil_moisture.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/solar_radiation.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/solar_radiation.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/stress.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/stress.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/et_look_v2_v3/unstable.py` & `pywapor-3.3.4/pywapor/et_look_v2_v3/unstable.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/aligner.py` & `pywapor-3.3.4/pywapor/general/aligner.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/bitmasks.py` & `pywapor-3.3.4/pywapor/general/bitmasks.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/compositer.py` & `pywapor-3.3.4/pywapor/general/compositer.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             empty_bins = xr.DataArray(x, {"time_bins": x})
         else:
             raise e
 
     new_t = determine_new_x(empty_bins.values, composite_type, bins = None, dtype = None)
 
     if len(new_t) > 0:
-        ds = xr.concat([ds, xr.Dataset({"time": new_t})], dim = "time").sortby("time")
+        ds = xr.merge([ds, xr.Dataset({"time": new_t})]).sortby("time")
 
     return ds
 
 def determine_new_x(intervals, composite_type, bins = None, dtype = None):
     
     if not isinstance(bins, type(None)):
         intervals = [pd.Interval(left = pd.Timestamp(l), right = pd.Timestamp(r)) for l, r in zip(bins[:-1], bins[1:])]
```

### Comparing `pywapor-3.3.3/pywapor/general/curvilinear.py` & `pywapor-3.3.4/pywapor/general/curvilinear.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     # Create output dataset
     output_ds = grid_ds.stack({"grid_pixel": ("y", "x")})
     no_pixel = output_ds.grid_pixel.size
 
     # Create intermediate dataset without multi-index
     grid_adj_ds = output_ds.assign_coords({"i": ("grid_pixel", range(no_pixel))}).set_index(grid_pixel="i")
-    grid_adj_ds = grid_adj_ds.drop(["x", "y"]).assign({"x": ("grid_pixel", grid_adj_ds.x.values),
+    grid_adj_ds = grid_adj_ds.drop_vars(["x", "y"]).assign({"x": ("grid_pixel", grid_adj_ds.x.values),
                                                        "y": ("grid_pixel", grid_adj_ds.y.values)})
 
     # Determine bounding box of current chunk.
     bb = [grid_adj_ds.x.min(), grid_adj_ds.y.min(), grid_adj_ds.x.max(), grid_adj_ds.y.max()]
 
     # Determine pixel size.
     dx = np.median(np.unique(np.diff(grid_ds.x)))
@@ -147,20 +147,20 @@
     # Wrap vertices and weights in xr.DataArray.
     kwargs = {"dims": ("grid_pixel", "j"), 
               "coords": {"j": range(3), "grid_pixel": grid_adj_ds.grid_pixel}}
     wts_da = xr.DataArray(wts, **kwargs)
     vtx_da = xr.DataArray(vtx, **kwargs)
 
     # --heavy-> Select relevant input data.
-    vls = data_pixel.drop(["x", "y"]).isel(pixel = vtx_da)
+    vls = data_pixel.drop_vars(["x", "y"]).isel(pixel = vtx_da)
 
     # Apply weights to input data.
     for var in vls.data_vars:
         da = xr.dot(vls[var], wts_da, dims = "j").where((wts_da > 0).all("j"))
-        output_ds[var] = da.reindex(grid_pixel = dists_pixel.grid_pixel).drop("grid_pixel")
+        output_ds[var] = da.reindex(grid_pixel = dists_pixel.grid_pixel).drop_vars("grid_pixel")
 
     return output_ds.unstack()
 
 if __name__ == "__main__":
 
     ...
     # Small test.
```

### Comparing `pywapor-3.3.3/pywapor/general/lazifier.py` & `pywapor-3.3.4/pywapor/general/lazifier.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/levels.py` & `pywapor-3.3.4/pywapor/general/levels.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     Returns
     -------
     list
         List of `source.product`s that contain `setting_str` in their nested dictionary.
     """
     example_sources = list()
     for var, x in sources.items():
-        prod = [product for product in x["products"] if setting_str in product.keys()]
+        x_ = x.get("products", [])
+        prod = [product for product in x_ if setting_str in product.keys()]
         if len(prod) >= 1:
             for pro in prod:
                 if pro[setting_str]:
                     example_source = (pro["source"], pro["product_name"])
                     if isinstance(example_source[0], types.FunctionType):
                         example_source = (example_source[0].__name__, example_source[1])
                     elif isinstance(example_source[0], partial):
```

### Comparing `pywapor-3.3.3/pywapor/general/logger.py` & `pywapor-3.3.4/pywapor/general/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 """Importing `log` from this module starts a logging handler, which can be logged to 
 with `log.info("log this info")` etc.
 """
 from python_log_indenter import IndentedLoggerAdapter
 import logging
 import os
 from tqdm.contrib.logging import logging_redirect_tqdm
+import warnings
 
 log_settings = logging.getLogger(__name__)
 __formatter__ = logging.Formatter(fmt='%(message)s', datefmt = '%Y/%m/%d %H:%M:%S')
 __handler__ = logging.StreamHandler()
 __handler__.setFormatter(__formatter__)
 __handler__.setLevel("INFO")
 log_settings.addHandler(__handler__)
 log = IndentedLoggerAdapter(log_settings)
-# logging_redirect_tqdm(loggers = [log_settings])
 
-def adjust_logger(log_write, folder, log_level):
+def adjust_logger(log_write, folder, log_level, testing = False):
     """Function to adjust the default logging settings that get initiated by
     importing this module.
 
     Parameters
     ----------
     log_write : bool
         Stop or start writing to log.
     folder : str
         Path to folder in which to store `"log.txt"`.
     log_level : str
         Set the log level.
     """
+    if log_write and any([isinstance(x, logging.FileHandler) for x in log_settings.handlers]):
+        handlers_to_remove = [x for x in log_settings.handlers if isinstance(x, logging.FileHandler)]
+        for handler in handlers_to_remove:
+            log_settings.removeHandler(handler)
+
     if log_write and not any([isinstance(x, logging.FileHandler) for x in log_settings.handlers]):
         if not os.path.isdir(folder):
             os.makedirs(folder)
         handler = logging.FileHandler(filename = os.path.join(folder, "log.txt"))
         formatter = logging.Formatter('{asctime} {levelname:>9s}: {message}', style='{')
         handler.setFormatter(formatter)
         handler.setLevel("DEBUG")
         log_settings.addHandler(handler)
         logging_redirect_tqdm(loggers = log_settings.handlers)
         log_settings.propagate = False
+
+    if testing:
+        log_settings.propagate = True
+        def fancy_warning(message):
+            IndentedLoggerAdapter(log_settings).warning(message)
+            warnings.warn(message, stacklevel=2)
+        log.warning = fancy_warning
+
     log_settings.setLevel(log_level)
```

### Comparing `pywapor-3.3.3/pywapor/general/network.py` & `pywapor-3.3.4/pywapor/general/network.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/performance.py` & `pywapor-3.3.4/pywapor/general/performance.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/pre_defaults.py` & `pywapor-3.3.4/pywapor/general/pre_defaults.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/processing_functions.py` & `pywapor-3.3.4/pywapor/general/processing_functions.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/reproject.py` & `pywapor-3.3.4/pywapor/general/reproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
     ncs = list()
 
     if has_changed(src_ds) or not has_geotransform(src_ds):
         src_path = src_ds.encoding.get("source", dst_path).replace(".nc", "_fixed.nc")
         new_src_ds = src_ds.sortby("y", ascending = False)
         new_src_ds = new_src_ds.rio.write_transform(new_src_ds.rio.transform(recalc=True))
         src_ds = save_ds(new_src_ds, src_path, encoding = "initiate", label = "Correcting src_ds.")
-        ncs.append(src_path)
+        ncs.append(src_ds)
     else:
         src_path = src_ds.encoding["source"]
 
     resampling = {
                     'nearest': 0,
                     'bilinear': 1,
                     'cubic': 2,
@@ -336,15 +336,15 @@
 
         if stack_dim in src_ds.coords:
             da = ds_part.to_array(stack_dim, name = var).assign_coords({stack_dim: src_ds[stack_dim]})
         else:
             da = ds_part[var]
 
         das.append(da)
-        ncs.append(part_path)
+        ncs.append(ds_part)
         variables[var] = (None, var)
 
     ds = xr.merge(das)
 
     if "spatial_ref" not in ds.coords:
         ds = ds.assign_coords({"spatial_ref": ds.crs})
```

### Comparing `pywapor-3.3.3/pywapor/general/units.py` & `pywapor-3.3.4/pywapor/general/units.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/general/variables.py` & `pywapor-3.3.4/pywapor/general/variables.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/post_et_look.py` & `pywapor-3.3.4/pywapor/post_et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/pre_et_look.py` & `pywapor-3.3.4/pywapor/pre_et_look.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor/pre_se_root.py` & `pywapor-3.3.4/pywapor/pre_se_root.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     dss= {**example_dss, **other_dss}
 
     ds = aligner.main(dss, sources, folder, general_enhancers, example_t_vars = example_t_vars)
 
     t2 = datetime.datetime.now()
     log.sub().info(f"< PRE_SE_ROOT ({str(t2 - t1)})")
 
-    files = remove_temp_files(folder)
+    _ = remove_temp_files(folder)
 
     return ds
 
 if __name__ == "__main__":
 
     # from pywapor.se_root import main as se_root
```

### Comparing `pywapor-3.3.3/pywapor/se_root.py` & `pywapor-3.3.4/pywapor/se_root.py`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/pywapor.egg-info/SOURCES.txt` & `pywapor-3.3.4/pywapor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywapor-3.3.3/setup.py` & `pywapor-3.3.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pywapor',
-    version = '3.3.3',
+    version = '3.3.4',
     url = 'https://www.fao.org/aquastat/py-wapor/',
     author = "FAO",
     author_email = "bert.coerver@fao.org",
     license = "Apache",
     packages = find_packages(include = ['pywapor', 'pywapor.*']),
     include_package_data=True,
     python_requires='>=3.7',
```

