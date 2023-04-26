# Comparing `tmp/gnssrefl-1.3.6.tar.gz` & `tmp/gnssrefl-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.3.6.tar", last modified: Sat Apr 22 16:09:35 2023, max compression
+gzip compressed data, was "gnssrefl-1.3.7.tar", last modified: Wed Apr 26 08:55:56 2023, max compression
```

## Comparing `gnssrefl-1.3.6.tar` & `gnssrefl-1.3.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.203649 gnssrefl-1.3.6/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.203649 gnssrefl-1.3.6/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/felipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   174790 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-22 16:09:21.000000 gnssrefl-1.3.6/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/nmea2snr_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34303 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5871 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickPhase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickPhase_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58967 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.203649 gnssrefl-1.3.6/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 16:09:35.000000 gnssrefl-1.3.6/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:09:35.223649 gnssrefl-1.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-22 16:09:22.000000 gnssrefl-1.3.6/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.971593 gnssrefl-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 08:55:56.971593 gnssrefl-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.947593 gnssrefl-1.3.7/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.947593 gnssrefl-1.3.7/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/felipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   174790 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/nmea2snr_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34303 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5882 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickPhase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickPhase_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58967 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.947593 gnssrefl-1.3.7/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:55:56.971593 gnssrefl-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.967593 gnssrefl-1.3.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.3.6/LICENSE` & `gnssrefl-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/PKG-INFO` & `gnssrefl-1.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.6
+Version: 1.3.7
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.7** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.6/README.md` & `gnssrefl-1.3.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gnssrefl
 
-**github version: 1.3.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.7** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.6/gnssrefl/EGM96.py` & `gnssrefl-1.3.7/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/check_rinex_file.py` & `gnssrefl-1.3.7/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/computemp1mp2.py` & `gnssrefl-1.3.7/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/daily_avg.py` & `gnssrefl-1.3.7/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.3.7/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.3.7/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_ioc.py` & `gnssrefl-1.3.7/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_noaa.py` & `gnssrefl-1.3.7/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_orbits.py` & `gnssrefl-1.3.7/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_psmsl.py` & `gnssrefl-1.3.7/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_rinex.py` & `gnssrefl-1.3.7/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_teqc.py` & `gnssrefl-1.3.7/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_tides.py` & `gnssrefl-1.3.7/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_unr.py` & `gnssrefl-1.3.7/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/download_wsv.py` & `gnssrefl-1.3.7/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/felipe.py` & `gnssrefl-1.3.7/gnssrefl/felipe.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/filesizes.py` & `gnssrefl-1.3.7/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gnssir.py` & `gnssrefl-1.3.7/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gnssir_cl.py` & `gnssrefl-1.3.7/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gnsssnr.f` & `gnssrefl-1.3.7/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.3.7/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gps.py` & `gnssrefl-1.3.7/gnssrefl/gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gpssnr.f` & `gnssrefl-1.3.7/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gpsweek.py` & `gnssrefl-1.3.7/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.3.7/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/highrate.py` & `gnssrefl-1.3.7/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/installexe_cl.py` & `gnssrefl-1.3.7/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/invsnr_cl.py` & `gnssrefl-1.3.7/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/invsnr_input.py` & `gnssrefl-1.3.7/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/karnak_libraries.py` & `gnssrefl-1.3.7/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/kelly.py` & `gnssrefl-1.3.7/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/llh2xyz.py` & `gnssrefl-1.3.7/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/make_json_input.py` & `gnssrefl-1.3.7/gnssrefl/make_json_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,25 @@
     parser.add_argument("long", help="longitude (degrees)", type=float)
     parser.add_argument("height", help="ellipsoidal height (meters)", type=float)
     # optional inputs
     parser.add_argument("-e1", default=None, type=int, help="lower limit elevation angle (deg)")
     parser.add_argument("-e2", default=None, type=int, help="upper limit elevation angle (deg)")
     parser.add_argument("-h1", default=None, type=float, help="lower limit reflector height (m)")
     parser.add_argument("-h2", default=None, type=float, help="upper limit reflector height (m)")
-    parser.add_argument("-nr1",default=None, type=float, help="lower limit noise region for QC(m)")
-    parser.add_argument("-nr2",default=None, type=float, help="upper limit noise region for QC(m)")
+    parser.add_argument("-nr1",default=None, type=float, help="lower limit RH used for noise region in QC(m)")
+    parser.add_argument("-nr2",default=None, type=float, help="upper limit RH used for noise region in QC(m)")
     parser.add_argument("-peak2noise", default=None, type=float, help="peak to noise ratio used for QC")
     parser.add_argument("-ampl", default=None, type=float, help="required spectral peak amplitude for QC")
     parser.add_argument("-allfreq", default=None, type=str, help="set to True to include all GNSS")
     parser.add_argument("-l1", default=None, type=str, help="set to True to only use GPS L1")
     parser.add_argument("-l2c", default=None, type=str, help="set to True to only use GPS L2C")
     parser.add_argument("-xyz", default=None, type=str, help="set to True if using Cartesian coordinates")
     parser.add_argument("-refraction", default=None, type=str, help="Set to False to turn off refraction correction")
     parser.add_argument("-extension", type=str, help="Provide extension name so you can try different strategies")
-    parser.add_argument("-ediff", default=None, type=str, help="ediff (degrees) default is 2")
+    parser.add_argument("-ediff", default=None, type=str, help="Allowed min/max elevation diff from obs min/max elev angle (degrees) default is 2")
     parser.add_argument("-delTmax", default=None, type=float, help="max arc length (min) default is 75. Shorten for tides.")
     parser.add_argument('-azlist', nargs="*",type=float,  help='User defined azimuth zones, i.e. 0 90 90 180 would mean only the east. Must be an even number of values.')
     parser.add_argument('-frlist', nargs="*",type=int,  help='User defined frequencies using our nomenclature.')
 
 
     args = parser.parse_args().__dict__
 
@@ -54,15 +54,16 @@
 def make_json(station: str, lat: float, long: float, height: float, e1: int = 5, e2: int = 25,
               h1: float = 0.5, h2: float = 8.0, nr1: float = None, nr2: float = None,
               peak2noise: float = 2.8, ampl: float = 5.0, allfreq: bool = False,
               l1: bool = False, l2c: bool = False, xyz: bool = False, refraction: bool = True,
               extension: str = '', ediff: float=2.0, delTmax: float=75.0, azlist: float=[], frlist: float=[] ):
 
     """
-    Saves the lomb scargle analysis strategy you will use in gnssrefl. Store in a json file which by default is saved
+    Saves the lomb scargle analysis strategy you will use in gnssrefl. Store in 
+    a json file which by default is saved
     in REFL_CODE/<station>.json.
 
     Examples
     --------
 
     make_json_input p041 0 0 0 
         uses only GPS frequencies and all azimuths and the coordinates in the UNR database
@@ -72,14 +73,17 @@
 
     make_json_input p041 39.9494 -105.19426 1728.85  -l2c T -e1 5 -e2 15
         uses only L2C GPS data between elevation angles of 5 and 15 degrees.
 
     make_json_input p041 39.9494 -105.19426 1728.85  -h1 0.5 -h2 10 -e1 5 -e2 25
         uses only GPS data between elevation angles of 5-25 degrees and reflector heights of 0.5-10 meters
 
+    make_json_input p041 0 0 0 -ediff 2
+        uses only GPS data, default station coordinates, enforces elevation angles to be 
+        within 2 degrees of default limits (5-25)
 
     Parameters
     ----------
     station : str
         4 character station ID.
     lat : float
         latitude in degrees.
@@ -118,28 +122,24 @@
     refraction : bool, optional
         set to False to turn off refraction correction.
         default is True.
     extension : str, optional
         provide extension name so you can try different strategies. 
         Results will then go into $REFL_CODE/YYYY/results/ssss/extension
         Default is '' 
-
     ediff : float
         quality control parameter (Degrees)
         default is 2
-
     delTmax : float
         maximum allowed arc length (minutes)
         default is 75, which is a bit long for tides
-
     azlist : list of floats
         lets the user set the azimuth regions, in degrees
         each region must be < 100 degrees! e.g. 0 90 90 180 would be all the east
         90 180 180 270 would be all the south
-
     frlist : list of integers
         avoids all the booleans - if you know the frequencies, enter them.
         e.g. 1 2 or 1 20 5 or 1 20 101 102
 
     """
 
     # make sure environment variables exist
```

### Comparing `gnssrefl-1.3.6/gnssrefl/nmea2snr.py` & `gnssrefl-1.3.7/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.3.7/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/phase_functions.py` & `gnssrefl-1.3.7/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/prn2gps.py` & `gnssrefl-1.3.7/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/query_unr.py` & `gnssrefl-1.3.7/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/quickLook_cl.py` & `gnssrefl-1.3.7/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/quickLook_function.py` & `gnssrefl-1.3.7/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/quickPhase.py` & `gnssrefl-1.3.7/gnssrefl/quickPhase.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,32 @@
     parser.add_argument("station", help="station", type=str)
     parser.add_argument("year", help="year", type=int)
     parser.add_argument("doy", help="doy", type=int)
     parser.add_argument("-snr", default=None, help="snr file ending", type=int)
     parser.add_argument("-fr", default=None, help="frequency (use all if you want both 1 and 20)", type=str)
     parser.add_argument("-doy_end", "-doy_end", default=None, type=int, help="doy end")
     parser.add_argument("-year_end", "-year_end", default=None, type=int, help="year end")
-    parser.add_argument("-e1", default=None, type=int),
-    parser.add_argument("-e2", default=None, type=int),
-    parser.add_argument("-plot", default=None, type=str)
+    parser.add_argument("-e1", default=None, type=float),
+    parser.add_argument("-e2", default=None, type=float),
+    parser.add_argument("-plt", default=None, type=str, help="plots come to the screen - which you do not want!")
     parser.add_argument("-screenstats", default=None, type=str, help="stats come to the screen")
     parser.add_argument("-gzip", default=None, type=str, help="gzip SNR files" )
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['plot', 'screenstats', 'gzip']
+    boolean_args = ['plt', 'screenstats', 'gzip']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def quickphase(station: str, year: int, doy: int, year_end: int = None, doy_end: int = None, snr: int = 66, 
-        fr: str = '20', e1: int = 5, e2: int = 30, plot: bool = False, screenstats: bool = False, gzip:bool=False):
+        fr: str = '20', e1: float = 5, e2: float = 30, plt: bool = False, screenstats: bool = False, gzip:bool=False):
     """
     quickphase computes phase for the given inputs (station, years, doy, elevation angles)
     These phase results are subquently used in vwc. The command line call is phase
     (which maybe we should change).
     
     Examples
     --------
@@ -50,57 +50,56 @@
 
     Parameters
     ----------
     station: str
         4 character ID of the station.
 
     year: int
-        Year to evaluate.
+        full Year to evaluate.
 
-    doy: integer
+    doy: int
         day of year to evaluate.
-        Default is None.
 
-    year_end: integer, optional
+    year_end: int, optional
         year to end analysis. Using this option will create a range from year-year_end.
         Default is None.
 
-    doy_end: integer, optional
+    doy_end: int, optional
         Day of year to end analysis. Using this option will create a range of doy-doy_end.
         If also using year_end, then this will be the day to end analysis in the year_end requested.
         Default is None.
 
-    snr : integer, optional
+    snr : int, optional
         SNR format. This tells the code what elevation angles are in the SNR file
         value options:
             66 (default) : data with elevation angles less than 30 degrees
 
             99 : data with elevation angles between 5 and 30 degrees
 
             88 : data with all elevation angles 
 
             50 : data with elevation angles less than 10 degrees
 
-    fr : string, optional
+    fr : str, optional
         GNSS frequency. Currently only supports L2C.
         Default is 20 (l2c)
 
-    e1 : integer, optional
+    e1 : float, optional
         Elevation angle lower limit in degrees for the LSP.
         default is 5
 
-    e2: integer, optional
+    e2: float, optional
         Elevation angle upper limit in degrees for the LSP.
         default is 30
 
-    plot: boolean, optional
+    plt: bool, optional
         Whether to plot results.
         Default is False
 
-    screenstats: boolean, optional
+    screenstats: bool, optional
         Whether to print stats to the screen.
         Default is False
 
     Returns
     -------
     Saves a file for each day in the doy-doy_end range: $REFL_CODE/<year>/phase/<station>/<doy>.txt
 
@@ -150,18 +149,18 @@
                 date_range = np.arange(1, doy_end+1)
             # If year within multi-year range then do whole year start to finish.
             else:
                 date_range = np.arange(1, 366)
 
             for d in date_range:
                 print('Analyzing year/day of year ' + str(y) + '/' + str(d))
-                qp.phase_tracks(station, y, d, snr, fr_list, e1, e2, pele, plot, screenstats, compute_lsp, gzip)
+                qp.phase_tracks(station, y, d, snr, fr_list, e1, e2, pele, plt, screenstats, compute_lsp, gzip)
     else:
         for d in np.arange(doy, doy_end + 1):
-            qp.phase_tracks(station, year, d, snr, fr_list, e1, e2, pele, plot, screenstats, compute_lsp, gzip)
+            qp.phase_tracks(station, year, d, snr, fr_list, e1, e2, pele, plt, screenstats, compute_lsp, gzip)
 
 
 def main():
     args = parse_arguments()
     quickphase(**args)
```

### Comparing `gnssrefl-1.3.6/gnssrefl/quickPhase_function.py` & `gnssrefl-1.3.7/gnssrefl/quickPhase_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/quickplt.py` & `gnssrefl-1.3.7/gnssrefl/quickplt.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     parser.add_argument("-ymdhm", help="if True/T, columns 1-4 are year mon day hour minute", type=str,default=None)
     parser.add_argument("-xlabel", type=str, help="optional x-axis label", default=None)
     parser.add_argument("-ylabel", type=str, help="optional y-axis label", default=None)
     parser.add_argument("-symbol", help="plot symbol ", type=str,default=None)
     parser.add_argument("-title", help="optional title", type=str,default=None)
     parser.add_argument("-outfile", help="optional filename for plot", type=str,default=None)
     parser.add_argument("-ylimits", nargs="*",type=float, help="optional ylimits", default=None)
+    parser.add_argument("-ydoy", help="if True/T, columns 1-2 are year and doy", type=str,default=None)
 
     args = parser.parse_args()
 
     filename = args.filename
     # change column numbers to pythonese
     xcol = int(args.xcol) - 1
     ycol = int(args.ycol) - 1
@@ -92,14 +93,18 @@
         reverse_sign = True
 
     # was previously ymdh
     ymd = False
     if (args.ymdhm == 'True') or (args.ymdhm == 'T'):
         ymd = True
 
+    ydoy = False
+    if (args.ydoy == 'True') or (args.ydoy == 'T'):
+        ydoy = True
+
     convert_mjd = False
     if (args.mjd== 'True') or (args.mjd == 'T'):
         convert_mjd = True
 
     commentsign = '%'
 
     if os.path.isfile(filename):
@@ -136,14 +141,19 @@
     else:
         if convert_mjd:
             t1 = Time(tvd[:,xcol],format='mjd')
             t1_utc = t1.utc # change to UTC
             # probably can be done in one step!
             tval =  t1_utc.datetime # change to datetime
             yval = tvd[:,ycol] # save the y values
+        elif ydoy:
+            tval = tvd[:,0]  + tvd[:,1]/365.25
+            yval = tvd[:,ycol]
+            ii = np.argsort( tval)
+            tval = tval[ii]; yval=yval[ii]
         else:
             tval = tvd[:,xcol] ; yval = tvd[:,ycol]
             x1 = min(tval) ; x2 = max(tval)
             if secondFile:
                 tval2 = tvd2[:,xcol] ; yval2 = tvd2[:,ycol]
 
     fig,ax=plt.subplots()
```

### Comparing `gnssrefl-1.3.6/gnssrefl/read_snr_files.py` & `gnssrefl-1.3.7/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/refl_zones.py` & `gnssrefl-1.3.7/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.3.7/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/refraction.py` & `gnssrefl-1.3.7/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/rh_plot.py` & `gnssrefl-1.3.7/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/rinex2snr.py` & `gnssrefl-1.3.7/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.3.7/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.3.7/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/rinex3_snr.py` & `gnssrefl-1.3.7/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/rinpy.py` & `gnssrefl-1.3.7/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.3.7/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/snow_functions.py` & `gnssrefl-1.3.7/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.3.7/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/spline_functions.py` & `gnssrefl-1.3.7/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/subdaily.py` & `gnssrefl-1.3.7/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/subdaily_cl.py` & `gnssrefl-1.3.7/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/utils.py` & `gnssrefl-1.3.7/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/veg_multiyr.py` & `gnssrefl-1.3.7/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/vwc.py` & `gnssrefl-1.3.7/gnssrefl/vwc.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     Examples
     --------
     vwc p038 2017
         one year for station p038 
     vwc p038 2015 -year_end 2017
         three years  for station p038 
     vwc p038 2015 -year_end 2017 -warning_value 6
-        warns you about tracks greater than 6 %
+        warns you about tracks greater than 6 degrees rms 
     vwc p038 2015 -year_end 2017 -warning_value 6 -auto_removal
         makes new list of tracks based on your new warning value
 
     Parameters
     ----------
     station : str
         4 character ID of the station
@@ -93,15 +93,15 @@
     subdir: str
         subdirectory in $REFL_CODE/Files for plots and text file outputs
     tmin: str
         minimum soil texture value, e.g. 0.05
     tmax: str
         maximum soil texture value, e.g. 0.45
     warning_value : float
-         screen warning about bad tracks (percent VWC).
+         screen warning about bad tracks (phase rms, in degrees).
          default is 5.5 
     auto_removal : boolean, optional
          whether to automatically remove tracks that hit your bad track threshold
          default value is false
 
     Returns
     -------
```

### Comparing `gnssrefl-1.3.6/gnssrefl/vwc_input.py` & `gnssrefl-1.3.7/gnssrefl/vwc_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,29 @@
     Picks up reflector height (RH) results for a given station and year-year end range and 
     computes the RH mean values and writes them to a file. These will be used to compute a consistent
     set of phase estimates.
 
     Examples
     --------
     vwc_input p038 2018
+        standard usage, station and year inputs
          
-    vwc_input p038 2018 -min_tracks 10
+    vwc_input p038 2018 -min_tracks 50
         allow fewer values to accept a satellite track
+        default is 100
 
     Parameters
     ----------
-    station : string
+    station : str
         4 character ID of the station
-    year : integer
-        Year
-    fr : integer, optional
+    year : int
+        full year
+    fr : int, optional
         GPS frequency. Currently only supports l2c, which is frequency 20.
-    min_tracks : integer, optional
+    min_tracks : int, optional
         number of minimum tracks needed in order to keep the average RH
 
     Returns
     -------
     File with columns
     index, mean reflector_heights, satellite, average_azimuth, number of reflector heights in average, min azimuth, max azimuth
```

### Comparing `gnssrefl-1.3.6/gnssrefl/xyz2llh.py` & `gnssrefl-1.3.7/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/ydoy.py` & `gnssrefl-1.3.7/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl/ymd.py` & `gnssrefl-1.3.7/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.3.7/gnssrefl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.6
+Version: 1.3.7
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.6** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.7** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.6/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.3.7/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.3.7/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/pyproject.toml` & `gnssrefl-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.6/setup.py` & `gnssrefl-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.3.6",
+    version="1.3.7",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.3.6/test/test_gps.py` & `gnssrefl-1.3.7/test/test_gps.py`

 * *Files identical despite different names*

