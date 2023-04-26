# Comparing `tmp/pyg2p-3.2.2.tar.gz` & `tmp/pyg2p-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyg2p-3.2.2.tar", last modified: Mon Feb 20 17:34:09 2023, max compression
+gzip compressed data, was "dist/pyg2p-3.2.3.tar", last modified: Wed Apr 26 09:40:42 2023, max compression
```

## Comparing `pyg2p-3.2.2.tar` & `pyg2p-3.2.3.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-02-15 12:18:09.000000 pyg2p-3.2.2/LICENSE
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-02-20 17:30:36.000000 pyg2p-3.2.2/MANIFEST.in
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    44072 2023-02-20 17:34:09.000000 pyg2p-3.2.2/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    43057 2023-02-15 12:18:09.000000 pyg2p-3.2.2/README.md
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/bin/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-02-15 12:18:09.000000 pyg2p-3.2.2/bin/pyg2p
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/configuration/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/geopotentials.json
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/configuration/global/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/global/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2946 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/global/geopotentials.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/global/global_conf.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    36594 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/global/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7000 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/global/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/global/test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-02-15 12:18:09.000000 pyg2p-3.2.2/configuration/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      214 2023-02-15 12:18:09.000000 pyg2p-3.2.2/requirements.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-02-20 17:34:09.000000 pyg2p-3.2.2/setup.cfg
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6305 2023-02-20 17:10:51.000000 pyg2p-3.2.2/setup.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-02-20 17:31:49.000000 pyg2p-3.2.2/src/pyg2p/VERSION
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7595 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/exceptions.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/main/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    15410 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/api.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/config.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    22535 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/context.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/controller.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/main/interpolation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    19605 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/interpolation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/interpolation/grib_interpolation_lib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1937 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/interpolation/latlong.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    50723 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/main/manipulation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/manipulation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    14068 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/manipulation/aggregator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/manipulation/conversion.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4830 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/manipulation/correction.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/main/readers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/readers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11707 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/readers/grib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3116 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/readers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/readers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/main/writers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6693 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/writers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     5603 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/writers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1952 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/main/writers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/util/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/util/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/util/files.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/util/generics.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/util/numeric.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p/util/profiling/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/util/profiling/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/util/profiling/profilehooks.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p/util/strings.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p.egg-info/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    44072 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p.egg-info/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4206 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p.egg-info/SOURCES.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p.egg-info/dependency_links.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      132 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p.egg-info/requires.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2023-02-20 17:34:09.000000 pyg2p-3.2.2/src/pyg2p.egg-info/top_level.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-02-20 16:19:14.000000 pyg2p-3.2.2/src/pyg2p.egg-info/zip-safe
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-02-15 12:18:09.000000 pyg2p-3.2.2/src/pyg2p.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-02-20 17:34:09.000000 pyg2p-3.2.2/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_cp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_lsp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_rg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_rn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_ta.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_td.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_wu.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/AFFS_wv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_15d.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_15d_glob.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_CV.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_CV_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_CV_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_CV_scipy_inv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_CV_scipy_nn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_agg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_december.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/EUE_RainAnim_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/UKMO_t24_LA.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/UKMO_t24_LA_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/UKMO_t24_LA_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cin.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_e06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_r06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_t24_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/cosmo_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_e06_2.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_e06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_e06_3.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_r06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_r06_efas.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_r06_gmi.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_t24_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwd_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/dwdl_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/efas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eud_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_e24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_e24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_r24_15days.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_r24_15days_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_r24_15days_noagg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_r24_15days_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/eue_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/glofas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/glofas_sro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/glofas_ssro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/glofas_ssro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test_scipy_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test_scipy_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/octahedral_test_scipy_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/rn_false_mv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_r06_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_r06_scipy_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_t24_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.2/templates/tigge_lam_t24_scipy_rotated.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-04-26 09:09:26.000000 pyg2p-3.2.3/LICENSE
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-04-26 09:09:26.000000 pyg2p-3.2.3/MANIFEST.in
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    47878 2023-04-26 09:40:42.000000 pyg2p-3.2.3/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    46863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/README.md
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/bin/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-04-26 09:09:26.000000 pyg2p-3.2.3/bin/pyg2p
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/configuration/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/geopotentials.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/configuration/global/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2946 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/geopotentials.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/global_conf.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    36594 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7000 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/global/test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-04-26 09:09:26.000000 pyg2p-3.2.3/configuration/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      214 2023-04-26 09:09:26.000000 pyg2p-3.2.3/requirements.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-04-26 09:40:42.000000 pyg2p-3.2.3/setup.cfg
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6305 2023-04-26 09:09:26.000000 pyg2p-3.2.3/setup.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/VERSION
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7644 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/exceptions.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    15678 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/api.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/config.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    22879 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/context.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/controller.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    19605 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/grib_interpolation_lib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2020 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/latlong.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    50993 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    14068 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/aggregator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/conversion.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4907 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/manipulation/correction.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/readers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11805 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/grib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3116 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/readers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/main/writers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6837 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/writers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8513 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/writers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1952 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/main/writers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/util/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/files.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/generics.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/numeric.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p/util/profiling/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/profiling/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/profiling/profilehooks.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p/util/strings.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    47878 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4206 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      132 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/requires.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2023-04-26 09:40:42.000000 pyg2p-3.2.3/src/pyg2p.egg-info/top_level.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-04-26 09:25:41.000000 pyg2p-3.2.3/src/pyg2p.egg-info/zip-safe
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-04-26 09:09:26.000000 pyg2p-3.2.3/src/pyg2p.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 09:40:42.000000 pyg2p-3.2.3/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_cp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_lsp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_rg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_rn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_ta.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_td.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_wu.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/AFFS_wv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_15d.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_15d_glob.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_inv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_nn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_agg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_december.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/EUE_RainAnim_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/UKMO_t24_LA.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/UKMO_t24_LA_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/UKMO_t24_LA_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cin.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_e06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_r06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_t24_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/cosmo_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_2.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_3.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_efas.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_gmi.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_t24_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwd_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/dwdl_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/efas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eud_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_e24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_e24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days_noagg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_15days_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/eue_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_sro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_ssro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/glofas_ssro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/octahedral_test_scipy_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/rn_false_mv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_r06_scipy_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-04-26 09:09:26.000000 pyg2p-3.2.3/templates/tigge_lam_t24_scipy_rotated.json
```

### Comparing `pyg2p-3.2.2/LICENSE` & `pyg2p-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/PKG-INFO` & `pyg2p-3.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg2p
-Version: 3.2.2
+Version: 3.2.3
 Summary: Convert GRIB files to netCDF or PCRaster
 Author: Domenico Nappo
 Author-email: domenico.nappo@gmail.com
 License: EUPL 1.2
 Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -32,20 +32,32 @@
 It can also manipulates GRIB messages (performing aggregation or simple unit conversion) before to apply format conversion.
 
 ## Installation
 
 To install package, you can use a python virtual environment or directly install dependencies and
 package at system level (executable script will be saved into /usr/local/bin in this case).
 
+### Using miniconda:
+
+
+* Install [miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+* Create a conda env named "pyg2penv" and install dependencies:
+
+  ```bash
+  conda create --name pyg2penv python=3.7 -c conda-forge
+  conda activate pyg2penv
+  ```
+
 >IMPORTANT: Before to launch setup, you need the following steps:
 
->Install eccodes: this can be done compiling from source code or using the available conda virtual environment package by running 
+>Install eccodes (and GDAL): this can be done compiling from source code or using the available conda virtual environment package by running 
 
 ```bash
-$ conda install -c conda-forge eccodes
+$ conda install -c conda-forge eccodes gdal
 ```
 
 >Configure geopotentials and intertables paths in
 configuration/global/global_conf.json. These paths are used by pyg2p to read
 geopotentials and intertables already configured. You may need to download files from FTP (launch `pyg2p -W` for this). 
 Users running pyg2p installed by a different user (ie. root) will configure similar paths for their own intertables 
 and geopotentials under his home folder. These paths will need write permissions.
@@ -53,15 +65,16 @@
 
 
 Grab last archive and extract it in a folder (or clone this repository) and follow these steps:
 
 ```bash
 $ cd pyg2p
 $ vim configuration/global/global_conf.json # to edit shared paths !!!
-$ python setup.py install
+$ pip install -r requirements.txt
+$ pip install .
 ```
 
 After installation, you will have all dependencies installed and an executable script 'pyg2p' (in a
 virtual environment, script is located under <VIRTUALENV_PATH>/bin folder otherwise under
 /usr/local/bin). To check correct installation of eccodes run the following command: 
 
 ```bash
@@ -225,15 +238,15 @@
 
 There are four sections of configuration.
 
 #### Aggregation
 Defines the aggregation method and step. Method can be `accumulation`, `average` or `instantaneous`.
 
 #### OutMaps
-Here you define interpolation method and paths to coordinates PCRaster maps, output unit time, the clone map etc.
+Here you define interpolation method and paths to coordinates netCDF/PCRaster maps, output unit time, the clone map etc.
 
 #### Interpolation
 This is a subelement of OutMaps. Here you define interpolation method (see later for details), paths
 to coordinates maps.
 
 #### Parameter
 In this section, you configure the parameter to select by using its shortName, as stored in GRIB file.
@@ -301,15 +314,23 @@
         </tr> 
     </thead>
     <tbody>
         <tr>
         <td><b>Execution</b></td>
         <td>name</td>
         <td>Descriptive name of the execution configuration.</td>
-        </tr>
+        </tr>        
+        <tr>
+        <td>&nbsp;</td><td>intertableDir</td><td>Alternative home folder for interpolation lookup
+tables, where pyg2p will load/save intertables. Folder must be existing. If not set, pyg2p will use intertables from ~/.pyg2p/intertables/</td>
+        </tr>    
+        <tr>
+        <td>&nbsp;</td><td>geopotentialDir</td><td>Alternative home folder for geopotential lookup
+tables. Folder must be existing. If not set, pyg2p will use geopotentials from ~/.pyg2p/geopotentials/</td>
+        </tr>    
         <tr>
         <td></td><td><b>Parameter</b></td><td>See relative table</td>
         </tr>
         <tr>
         <td></td><td><b>OutMaps</b></td><td>See relative table</td>
         </tr>
         <tr>
@@ -361,33 +382,52 @@
         <tr>
         <td><b>OutMaps</b></td><td>cloneMap</td><td>The clone map with area (must have a REAL cell
 type and missing values for points outside area
 of interest. A dem map works fine. A typical area boolean map will not).</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>unitTime</b></td><td>Time unit in hours of output maps. Tipical value
-is 24 (daily maps).</td>
+is 24 (daily maps). Used in "accumulation" operation</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>format</b></td><td>Output file format. Default 'pcraster'. Available
 formats are 'pcraster', 'netcdf'.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>namePrefix</b></td><td>Prefix for maps. Default is parameter
 shortName.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>fmap</b></td><td>First PCRaster map number. Default 1.</td>
+        <td>&nbsp;</td><td><b>scaleFactor</b></td><td>Scale factor of the output netCDF map. Default 1.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>Interpolation</b></td><td>See relative table.</td>
+        <td>&nbsp;</td><td><b>offset</b></td><td>Offset of the output netCDF map. Default 0.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>validMin</b></td><td>Minimum value of the output netCDF map. Values below will be set to nodata.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>validMax</b></td><td>Maximum value of the output netCDF map. Values above will be set to nodata.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>valueFormat</b></td><td>Variable type to use in the output netCDF map. Deafult f8. Available formats are: i1,i2,i4,i8,u1,u2,u4,u8,f4,f8 where i is integer, u is unsigned integer, f if float and the number corresponds to the number of bytes used (e.g. i4 is integer 32bits = 4 bytes)</td>
+        </tr>  
+        <tr>
+        <td>&nbsp;</td><td><b>outputStepUnits</b></td><td>Step units to use in output map. If not specified, it will use the stepUnits of the source Grib file. Available values are: 's': seconds, 'm': minutes, 'h': hours, '3h': 3h steps, '6h': 6h steps, '12h': 12h steps, 'D': days</td>
+        </tr>
+        <tr>      
+        <tr>
+        <td>&nbsp;</td><td><b>fmap</b></td><td>First PCRaster map number. Default 1.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>ext</b></td><td>Extension mode. It's the integer number
-defining the step numbers to skip when writing maps. Same as old grib2pcraster. Default 1.</td>
+defining the step numbers to skip when writing PCRaster maps. Same as old grib2pcraster. Default 1.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>Interpolation</b></td><td>See relative table.</td>
         </tr>
         <tr>
         <td colspan="3"><hr/></td>
         </tr>
         <tr>
         <td><b>Aggregation</b></td><td><b>step</b></td><td>Step of aggregation in hours.</td>
         </tr>
@@ -410,19 +450,15 @@
 “grib_invdist”</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>latMap</b></td><td>PCRaster map of target latitudes.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>lonMap</b></td><td>PCRaster map of target longitudes.</td>
-        </tr>
-        <tr>
-        <td>&nbsp;</td><td>intertableDir</td><td>Alternative home folder for interpolation lookup
-tables, where pyg2p will load/save intertables. Folder must be existing. If not set, pyg2p will use intertables from ~/.pyg2p/intertables/</td>
-        </tr>
+        </tr>        
     </tbody>
 </table>
 
 ## Usage
 
 To use the application, after the main configuration you need to configure a template JSON file for
 each type of extraction you need to perform.
@@ -451,78 +487,86 @@
 
 ### Input arguments
 
 If you run pyg2p without arguments, it shows help of all input arguments.
 
 ```console
 usage: pyg2p [-h] [-c json_file] [-o out_dir] [-i input_file]
-[-I input_file_2nd] [-s tstart] [-e tend] [-m eps_member]
-[-T data_time] [-D data_date] [-f fmap] [-F format] [-x extension_step]
-[-n outfiles_prefix] [-l log_level] [-N intertable_dir] [-B] [-X]
-[-t cmds_file] [-g geopotential] [-C path] [-z path] [-W dataset]
+             [-I input_file_2nd] [-s tstart] [-e tend] [-m eps_member]
+             [-T data_time] [-D data_date] [-f fmap] [-F format]
+             [-x extension_step] [-n outfiles_prefix] [-O offset]
+             [-S scale_factor] [-vM valid_max] [-vm valid_min]
+             [-vf value_format] [-U output_step_units] [-l log_level]
+             [-N intertable_dir] [-G geopotential_dir] [-B] [-X]
+             [-g geopotential] [-W dataset]
 
-Execute the grib to pcraster conversion using parameters from the input json configuration.
-Read user manual.
+Pyg2p: Execute the grib to netCDF/PCRaster conversion, using parameters
+from CLI/json configuration.
 
 optional arguments:
--h, --help show this help message and exit
--c json_file, --commandsFile json_file
-Path to json command file
--o out_dir, --outDir out_dir
-Path where output maps will be created.
--i input_file, --inputFile input_file
-Path to input grib.
--I input_file_2nd, --inputFile2 input_file_2nd
-Path to 2nd resolution input grib.
--s tstart, --start tstart
-Grib timestep start. It overwrites the tstart in json
-execution file.
--e tend, --end tend Grib timestep end. It overwrites the tend in json
-execution file.
--m eps_member, --perturbationNumber eps_member
-eps member number
--T data_time, --dataTime data_time
-To select messages by dataTime key value
--D data_date, --dataDate data_date
-<YYYYMMDD> to select messages by dataDate key value
--f fmap, --fmap fmap First map number
--F format, --format format
-Output format. Available options: netcdf, pcraster.
-Default pcraster
--x extension_step, --ext extension_step
-Extension number step
--n outfiles_prefix, --namePrefix outfiles_prefix
-Prefix name for maps
--l log_level, --loggerLevel log_level
-Console logging level
--N intertable_dir, --intertableDir intertable_dir
-interpolation tables dir
--B, --createIntertable
-create intertable file
--X, --interpolationParallel
-Use parallelization tools to make interpolation
-faster.If -B option is not passed or intertable
-already exists it does not have any effect.
--t cmds_file, --test cmds_file
-Path to a text file containing list of commands,
-defining a battery of tests. Then it will create diff
-pcraster maps and log alerts if differences are higher
-than a threshold (edit configuration in test.json)
--g geopotential, --addGeopotential geopotential
-Add the file to geopotentials.json configuration file, to use for correction. The file will be copied into
-the right folder (configuration/geopotentials) Note:
-shortName of geopotential must be "fis" or "z"
--C path, --convertConf path
-Convert old xml configuration to new json format
--z path, --convertIntertables path
-Convert old pyg2p intertables to new version and copy
-to user folders
--W dataset, --downloadConf dataset
-Download intertables and geopotentials (FTP settings
-defined in ftp.json)
+  -h, --help            show this help message and exit
+  -c json_file, --commandsFile json_file
+                        Path to json command file
+  -o out_dir, --outDir out_dir
+                        Path where output maps will be created.
+  -i input_file, --inputFile input_file
+                        Path to input grib.
+  -I input_file_2nd, --inputFile2 input_file_2nd
+                        Path to 2nd resolution input grib.
+  -s tstart, --start tstart
+                        Grib timestep start. It overwrites the tstart in json
+                        execution file.
+  -e tend, --end tend   Grib timestep end. It overwrites the tend in json
+                        execution file.
+  -m eps_member, --perturbationNumber eps_member
+                        eps member number
+  -T data_time, --dataTime data_time
+                        To select messages by dataTime key value
+  -D data_date, --dataDate data_date
+                        <YYYYMMDD> to select messages by dataDate key value
+  -f fmap, --fmap fmap  First map number
+  -F format, --format format
+                        Output format. Available options: netcdf, pcraster.
+                        Default pcraster
+  -x extension_step, --ext extension_step
+                        Extension number step
+  -n outfiles_prefix, --namePrefix outfiles_prefix
+                        Prefix name for maps
+  -O offset, --offset offset
+                        Map offset
+  -S scale_factor, --scaleFactor scale_factor
+                        Map scale factor
+  -vM valid_max, --validMax valid_max
+                        Max valid value
+  -vm valid_min, --validMin valid_min
+                        Min valid value
+  -vf value_format, --valueFormat value_format
+                        output value format (default f8)
+  -U output_step_units, --outputStepUnits output_step_units
+                        output step units
+  -l log_level, --loggerLevel log_level
+                        Console logging level
+  -N intertable_dir, --intertableDir intertable_dir
+                        Alternate interpolation tables dir
+  -G geopotential_dir, --geopotentialDir geopotential_dir
+                        Alternate geopotential dir
+  -B, --createIntertable
+                        Flag to create intertable file
+  -X, --interpolationParallel
+                        Use parallelization tools to make interpolation
+                        faster.If -B option is not passed or intertable
+                        already exists it does not have any effect.
+  -g geopotential, --addGeopotential geopotential
+                        Add the file to geopotentials.json configuration file,
+                        to use for correction. The file will be copied into
+                        the right folder (configuration/geopotentials) Note:
+                        shortName of geopotential must be "fis" or "z"
+  -W dataset, --downloadConf dataset
+                        Download intertables and geopotentials (FTP settings
+                        defined in ftp.json)
 ```
 #### Usage examples:
 
 ```bash
 pyg2p -c ./exec1.json -i ./input.grib -o /out/dir -s 12 -e 36 -F netcdf
 pyg2p -c ./exec2.json -i ./input.grib -o /out/dir -m 10 -l INFO --format netcdf
 pyg2p -c ./exec3.json -i ./input.grib -I /input2ndres.grib -o /out/dir -m 10 -l DEBUG
@@ -686,24 +730,30 @@
   "@mode": "bilinear_delaunay"}
 }
 ```
 
 ## OutMaps configuration
 
 Interpolation is configured under the OutMaps tag. With additional attributes, you also configure
-resulting PCRaster maps. Output dir is ./ by default or you can set it via command line using the
+resulting PCRaster or netCDF maps. Output dir is ./ by default or you can set it via command line using the
 option -o (--outDir).
 
 | Attribute      | Details                                                                                                                           |
 |----------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | namePrefix     | Prefix name for output map files. Default is the value of shortName key.                                                          |
-| **unitTime**   | Unit time in hours for results. This is used during aggregation operations.                                                       |
+| unitTime       | Unit time in hours for results. This is used during aggregation operations.                                                       |
 | fmap           | Extension number for the first map. Default 1.                                                                                    |
 | ext            | Extension mode. It's the integer number defining the step numbers to skip when writing maps. Same as old grib2pcraster. Default 1.|
-| **cloneMap**   | Path to a PCRaster clone map, needed by PCRaster libraries to write a new map on disk.                                            |
+| cloneMap       | Path to a PCRaster clone map, needed by PCRaster libraries to write a new map on disk.                                            |
+| scaleFactor    | Scale factor of the output netCDF map. Default 1. |
+| offset         | Offset of the output netCDF map. Default 0. |
+| validMin       | Minimum value of the output netCDF map. Values below will be set to nodata. |
+| validMax       | Maximum value of the output netCDF map. Values above will be set to nodata. |
+| valueFormat    | Variable type to use in the output netCDF map. Deafult f8. Available formats are: i1,i2,i4,i8,u1,u2,u4,u8,f4,f8 where i is integer, u is unsigned integer, f if float and the number corresponds to the number of bytes used (e.g. i4 is integer 32bits = 4 bytes) | 
+| outputStepUnits | Step units to use in output map. If not specified, it will use the stepUnits of the source Grib file. Available values are: 's': seconds, 'm': minutes, 'h': hours, '3h': 3h steps, '6h': 6h steps, '12h': 12h steps, 'D': days |
 
 ## Aggregation
 
 Values from grib files can be aggregated before to write the final PCRaster maps. There are two kinds of aggregation available: average and accumulation. 
 The JSON configuration in the execution file will look like:
 
 ```json
@@ -1221,12 +1271,12 @@
 Dimensions:
         xc: Number of rows of area/clone map
         yc: Number of cols of area/clone map
         time: Unlimited dimension for time steps
 Variables:
         lon: 2D array with shape (yc, xc)
         lat: 2D array with shape (yc, xc)
-        time_nc: 1D array of values representing hours since dataDate of first grib message (endStep)
+        time_nc: 1D array of values representing hours/days since dataDate of first grib message (endStep)
         values_nc: a 3D array of dimensions (time, yc, xc), with coordinates set to 'lon, lat'.
 ```
```

### Comparing `pyg2p-3.2.2/README.md` & `pyg2p-3.2.3/src/pyg2p.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,63 @@
+Metadata-Version: 2.1
+Name: pyg2p
+Version: 3.2.3
+Summary: Convert GRIB files to netCDF or PCRaster
+Author: Domenico Nappo
+Author-email: domenico.nappo@gmail.com
+License: EUPL 1.2
+Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [ChangeLog](CHANGE_LOG.rst)
 
 
 # pyg2p
 pyg2p is a converter between GRIB and netCDF4/PCRaster files. 
 It can also manipulates GRIB messages (performing aggregation or simple unit conversion) before to apply format conversion.
 
 ## Installation
 
 To install package, you can use a python virtual environment or directly install dependencies and
 package at system level (executable script will be saved into /usr/local/bin in this case).
 
+### Using miniconda:
+
+
+* Install [miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+* Create a conda env named "pyg2penv" and install dependencies:
+
+  ```bash
+  conda create --name pyg2penv python=3.7 -c conda-forge
+  conda activate pyg2penv
+  ```
+
 >IMPORTANT: Before to launch setup, you need the following steps:
 
->Install eccodes: this can be done compiling from source code or using the available conda virtual environment package by running 
+>Install eccodes (and GDAL): this can be done compiling from source code or using the available conda virtual environment package by running 
 
 ```bash
-$ conda install -c conda-forge eccodes
+$ conda install -c conda-forge eccodes gdal
 ```
 
 >Configure geopotentials and intertables paths in
 configuration/global/global_conf.json. These paths are used by pyg2p to read
 geopotentials and intertables already configured. You may need to download files from FTP (launch `pyg2p -W` for this). 
 Users running pyg2p installed by a different user (ie. root) will configure similar paths for their own intertables 
 and geopotentials under his home folder. These paths will need write permissions.
@@ -27,15 +65,16 @@
 
 
 Grab last archive and extract it in a folder (or clone this repository) and follow these steps:
 
 ```bash
 $ cd pyg2p
 $ vim configuration/global/global_conf.json # to edit shared paths !!!
-$ python setup.py install
+$ pip install -r requirements.txt
+$ pip install .
 ```
 
 After installation, you will have all dependencies installed and an executable script 'pyg2p' (in a
 virtual environment, script is located under <VIRTUALENV_PATH>/bin folder otherwise under
 /usr/local/bin). To check correct installation of eccodes run the following command: 
 
 ```bash
@@ -199,15 +238,15 @@
 
 There are four sections of configuration.
 
 #### Aggregation
 Defines the aggregation method and step. Method can be `accumulation`, `average` or `instantaneous`.
 
 #### OutMaps
-Here you define interpolation method and paths to coordinates PCRaster maps, output unit time, the clone map etc.
+Here you define interpolation method and paths to coordinates netCDF/PCRaster maps, output unit time, the clone map etc.
 
 #### Interpolation
 This is a subelement of OutMaps. Here you define interpolation method (see later for details), paths
 to coordinates maps.
 
 #### Parameter
 In this section, you configure the parameter to select by using its shortName, as stored in GRIB file.
@@ -275,15 +314,23 @@
         </tr> 
     </thead>
     <tbody>
         <tr>
         <td><b>Execution</b></td>
         <td>name</td>
         <td>Descriptive name of the execution configuration.</td>
-        </tr>
+        </tr>        
+        <tr>
+        <td>&nbsp;</td><td>intertableDir</td><td>Alternative home folder for interpolation lookup
+tables, where pyg2p will load/save intertables. Folder must be existing. If not set, pyg2p will use intertables from ~/.pyg2p/intertables/</td>
+        </tr>    
+        <tr>
+        <td>&nbsp;</td><td>geopotentialDir</td><td>Alternative home folder for geopotential lookup
+tables. Folder must be existing. If not set, pyg2p will use geopotentials from ~/.pyg2p/geopotentials/</td>
+        </tr>    
         <tr>
         <td></td><td><b>Parameter</b></td><td>See relative table</td>
         </tr>
         <tr>
         <td></td><td><b>OutMaps</b></td><td>See relative table</td>
         </tr>
         <tr>
@@ -335,33 +382,52 @@
         <tr>
         <td><b>OutMaps</b></td><td>cloneMap</td><td>The clone map with area (must have a REAL cell
 type and missing values for points outside area
 of interest. A dem map works fine. A typical area boolean map will not).</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>unitTime</b></td><td>Time unit in hours of output maps. Tipical value
-is 24 (daily maps).</td>
+is 24 (daily maps). Used in "accumulation" operation</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>format</b></td><td>Output file format. Default 'pcraster'. Available
 formats are 'pcraster', 'netcdf'.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>namePrefix</b></td><td>Prefix for maps. Default is parameter
 shortName.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>fmap</b></td><td>First PCRaster map number. Default 1.</td>
+        <td>&nbsp;</td><td><b>scaleFactor</b></td><td>Scale factor of the output netCDF map. Default 1.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>Interpolation</b></td><td>See relative table.</td>
+        <td>&nbsp;</td><td><b>offset</b></td><td>Offset of the output netCDF map. Default 0.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>validMin</b></td><td>Minimum value of the output netCDF map. Values below will be set to nodata.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>validMax</b></td><td>Maximum value of the output netCDF map. Values above will be set to nodata.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>valueFormat</b></td><td>Variable type to use in the output netCDF map. Deafult f8. Available formats are: i1,i2,i4,i8,u1,u2,u4,u8,f4,f8 where i is integer, u is unsigned integer, f if float and the number corresponds to the number of bytes used (e.g. i4 is integer 32bits = 4 bytes)</td>
+        </tr>  
+        <tr>
+        <td>&nbsp;</td><td><b>outputStepUnits</b></td><td>Step units to use in output map. If not specified, it will use the stepUnits of the source Grib file. Available values are: 's': seconds, 'm': minutes, 'h': hours, '3h': 3h steps, '6h': 6h steps, '12h': 12h steps, 'D': days</td>
+        </tr>
+        <tr>      
+        <tr>
+        <td>&nbsp;</td><td><b>fmap</b></td><td>First PCRaster map number. Default 1.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>ext</b></td><td>Extension mode. It's the integer number
-defining the step numbers to skip when writing maps. Same as old grib2pcraster. Default 1.</td>
+defining the step numbers to skip when writing PCRaster maps. Same as old grib2pcraster. Default 1.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>Interpolation</b></td><td>See relative table.</td>
         </tr>
         <tr>
         <td colspan="3"><hr/></td>
         </tr>
         <tr>
         <td><b>Aggregation</b></td><td><b>step</b></td><td>Step of aggregation in hours.</td>
         </tr>
@@ -384,19 +450,15 @@
 “grib_invdist”</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>latMap</b></td><td>PCRaster map of target latitudes.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>lonMap</b></td><td>PCRaster map of target longitudes.</td>
-        </tr>
-        <tr>
-        <td>&nbsp;</td><td>intertableDir</td><td>Alternative home folder for interpolation lookup
-tables, where pyg2p will load/save intertables. Folder must be existing. If not set, pyg2p will use intertables from ~/.pyg2p/intertables/</td>
-        </tr>
+        </tr>        
     </tbody>
 </table>
 
 ## Usage
 
 To use the application, after the main configuration you need to configure a template JSON file for
 each type of extraction you need to perform.
@@ -425,78 +487,86 @@
 
 ### Input arguments
 
 If you run pyg2p without arguments, it shows help of all input arguments.
 
 ```console
 usage: pyg2p [-h] [-c json_file] [-o out_dir] [-i input_file]
-[-I input_file_2nd] [-s tstart] [-e tend] [-m eps_member]
-[-T data_time] [-D data_date] [-f fmap] [-F format] [-x extension_step]
-[-n outfiles_prefix] [-l log_level] [-N intertable_dir] [-B] [-X]
-[-t cmds_file] [-g geopotential] [-C path] [-z path] [-W dataset]
+             [-I input_file_2nd] [-s tstart] [-e tend] [-m eps_member]
+             [-T data_time] [-D data_date] [-f fmap] [-F format]
+             [-x extension_step] [-n outfiles_prefix] [-O offset]
+             [-S scale_factor] [-vM valid_max] [-vm valid_min]
+             [-vf value_format] [-U output_step_units] [-l log_level]
+             [-N intertable_dir] [-G geopotential_dir] [-B] [-X]
+             [-g geopotential] [-W dataset]
 
-Execute the grib to pcraster conversion using parameters from the input json configuration.
-Read user manual.
+Pyg2p: Execute the grib to netCDF/PCRaster conversion, using parameters
+from CLI/json configuration.
 
 optional arguments:
--h, --help show this help message and exit
--c json_file, --commandsFile json_file
-Path to json command file
--o out_dir, --outDir out_dir
-Path where output maps will be created.
--i input_file, --inputFile input_file
-Path to input grib.
--I input_file_2nd, --inputFile2 input_file_2nd
-Path to 2nd resolution input grib.
--s tstart, --start tstart
-Grib timestep start. It overwrites the tstart in json
-execution file.
--e tend, --end tend Grib timestep end. It overwrites the tend in json
-execution file.
--m eps_member, --perturbationNumber eps_member
-eps member number
--T data_time, --dataTime data_time
-To select messages by dataTime key value
--D data_date, --dataDate data_date
-<YYYYMMDD> to select messages by dataDate key value
--f fmap, --fmap fmap First map number
--F format, --format format
-Output format. Available options: netcdf, pcraster.
-Default pcraster
--x extension_step, --ext extension_step
-Extension number step
--n outfiles_prefix, --namePrefix outfiles_prefix
-Prefix name for maps
--l log_level, --loggerLevel log_level
-Console logging level
--N intertable_dir, --intertableDir intertable_dir
-interpolation tables dir
--B, --createIntertable
-create intertable file
--X, --interpolationParallel
-Use parallelization tools to make interpolation
-faster.If -B option is not passed or intertable
-already exists it does not have any effect.
--t cmds_file, --test cmds_file
-Path to a text file containing list of commands,
-defining a battery of tests. Then it will create diff
-pcraster maps and log alerts if differences are higher
-than a threshold (edit configuration in test.json)
--g geopotential, --addGeopotential geopotential
-Add the file to geopotentials.json configuration file, to use for correction. The file will be copied into
-the right folder (configuration/geopotentials) Note:
-shortName of geopotential must be "fis" or "z"
--C path, --convertConf path
-Convert old xml configuration to new json format
--z path, --convertIntertables path
-Convert old pyg2p intertables to new version and copy
-to user folders
--W dataset, --downloadConf dataset
-Download intertables and geopotentials (FTP settings
-defined in ftp.json)
+  -h, --help            show this help message and exit
+  -c json_file, --commandsFile json_file
+                        Path to json command file
+  -o out_dir, --outDir out_dir
+                        Path where output maps will be created.
+  -i input_file, --inputFile input_file
+                        Path to input grib.
+  -I input_file_2nd, --inputFile2 input_file_2nd
+                        Path to 2nd resolution input grib.
+  -s tstart, --start tstart
+                        Grib timestep start. It overwrites the tstart in json
+                        execution file.
+  -e tend, --end tend   Grib timestep end. It overwrites the tend in json
+                        execution file.
+  -m eps_member, --perturbationNumber eps_member
+                        eps member number
+  -T data_time, --dataTime data_time
+                        To select messages by dataTime key value
+  -D data_date, --dataDate data_date
+                        <YYYYMMDD> to select messages by dataDate key value
+  -f fmap, --fmap fmap  First map number
+  -F format, --format format
+                        Output format. Available options: netcdf, pcraster.
+                        Default pcraster
+  -x extension_step, --ext extension_step
+                        Extension number step
+  -n outfiles_prefix, --namePrefix outfiles_prefix
+                        Prefix name for maps
+  -O offset, --offset offset
+                        Map offset
+  -S scale_factor, --scaleFactor scale_factor
+                        Map scale factor
+  -vM valid_max, --validMax valid_max
+                        Max valid value
+  -vm valid_min, --validMin valid_min
+                        Min valid value
+  -vf value_format, --valueFormat value_format
+                        output value format (default f8)
+  -U output_step_units, --outputStepUnits output_step_units
+                        output step units
+  -l log_level, --loggerLevel log_level
+                        Console logging level
+  -N intertable_dir, --intertableDir intertable_dir
+                        Alternate interpolation tables dir
+  -G geopotential_dir, --geopotentialDir geopotential_dir
+                        Alternate geopotential dir
+  -B, --createIntertable
+                        Flag to create intertable file
+  -X, --interpolationParallel
+                        Use parallelization tools to make interpolation
+                        faster.If -B option is not passed or intertable
+                        already exists it does not have any effect.
+  -g geopotential, --addGeopotential geopotential
+                        Add the file to geopotentials.json configuration file,
+                        to use for correction. The file will be copied into
+                        the right folder (configuration/geopotentials) Note:
+                        shortName of geopotential must be "fis" or "z"
+  -W dataset, --downloadConf dataset
+                        Download intertables and geopotentials (FTP settings
+                        defined in ftp.json)
 ```
 #### Usage examples:
 
 ```bash
 pyg2p -c ./exec1.json -i ./input.grib -o /out/dir -s 12 -e 36 -F netcdf
 pyg2p -c ./exec2.json -i ./input.grib -o /out/dir -m 10 -l INFO --format netcdf
 pyg2p -c ./exec3.json -i ./input.grib -I /input2ndres.grib -o /out/dir -m 10 -l DEBUG
@@ -660,24 +730,30 @@
   "@mode": "bilinear_delaunay"}
 }
 ```
 
 ## OutMaps configuration
 
 Interpolation is configured under the OutMaps tag. With additional attributes, you also configure
-resulting PCRaster maps. Output dir is ./ by default or you can set it via command line using the
+resulting PCRaster or netCDF maps. Output dir is ./ by default or you can set it via command line using the
 option -o (--outDir).
 
 | Attribute      | Details                                                                                                                           |
 |----------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | namePrefix     | Prefix name for output map files. Default is the value of shortName key.                                                          |
-| **unitTime**   | Unit time in hours for results. This is used during aggregation operations.                                                       |
+| unitTime       | Unit time in hours for results. This is used during aggregation operations.                                                       |
 | fmap           | Extension number for the first map. Default 1.                                                                                    |
 | ext            | Extension mode. It's the integer number defining the step numbers to skip when writing maps. Same as old grib2pcraster. Default 1.|
-| **cloneMap**   | Path to a PCRaster clone map, needed by PCRaster libraries to write a new map on disk.                                            |
+| cloneMap       | Path to a PCRaster clone map, needed by PCRaster libraries to write a new map on disk.                                            |
+| scaleFactor    | Scale factor of the output netCDF map. Default 1. |
+| offset         | Offset of the output netCDF map. Default 0. |
+| validMin       | Minimum value of the output netCDF map. Values below will be set to nodata. |
+| validMax       | Maximum value of the output netCDF map. Values above will be set to nodata. |
+| valueFormat    | Variable type to use in the output netCDF map. Deafult f8. Available formats are: i1,i2,i4,i8,u1,u2,u4,u8,f4,f8 where i is integer, u is unsigned integer, f if float and the number corresponds to the number of bytes used (e.g. i4 is integer 32bits = 4 bytes) | 
+| outputStepUnits | Step units to use in output map. If not specified, it will use the stepUnits of the source Grib file. Available values are: 's': seconds, 'm': minutes, 'h': hours, '3h': 3h steps, '6h': 6h steps, '12h': 12h steps, 'D': days |
 
 ## Aggregation
 
 Values from grib files can be aggregated before to write the final PCRaster maps. There are two kinds of aggregation available: average and accumulation. 
 The JSON configuration in the execution file will look like:
 
 ```json
@@ -1195,10 +1271,12 @@
 Dimensions:
         xc: Number of rows of area/clone map
         yc: Number of cols of area/clone map
         time: Unlimited dimension for time steps
 Variables:
         lon: 2D array with shape (yc, xc)
         lat: 2D array with shape (yc, xc)
-        time_nc: 1D array of values representing hours since dataDate of first grib message (endStep)
+        time_nc: 1D array of values representing hours/days since dataDate of first grib message (endStep)
         values_nc: a 3D array of dimensions (time, yc, xc), with coordinates set to 'lon, lat'.
 ```
+
+
```

### Comparing `pyg2p-3.2.2/configuration/global/geopotentials.json` & `pyg2p-3.2.3/configuration/global/geopotentials.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/configuration/global/intertables.json` & `pyg2p-3.2.3/configuration/global/intertables.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/configuration/global/parameters.json` & `pyg2p-3.2.3/configuration/global/parameters.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/setup.py` & `pyg2p-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/__init__.py` & `pyg2p-3.2.3/src/pyg2p/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,19 +141,20 @@
 
     def __str__(self):
         return str(self._geo_keys)
 
 
 class Messages(Loggable):
 
-    def __init__(self, values, mv, unit, type_of_level, type_of_step, grid_details, val_2nd=None, data_date=None):
+    def __init__(self, values, mv, unit, type_of_level, type_of_step, step_units, grid_details, val_2nd=None, data_date=None):
         super().__init__()
         self.values_first_or_single_res = values
         self.values_second_res = val_2nd or {}
         self.step_type = type_of_step
+        self.step_units = step_units
         self.type_of_level = type_of_level
         self.unit = unit
         self.missing_value = mv
         self.data_date = datetime.strptime(str(data_date), '%Y%m%d')
 
         self.grid_details = grid_details
         # order key list to get first step
```

### Comparing `pyg2p-3.2.2/src/pyg2p/exceptions.py` & `pyg2p-3.2.3/src/pyg2p/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/__init__.py` & `pyg2p-3.2.3/src/pyg2p/main/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/api.py` & `pyg2p-3.2.3/src/pyg2p/main/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     c = Command()
     c = c.with_cmdpath('average.json').with_inputfile('rain.grb').with_outdir('./')
     c = c.with_create_intertable().with_parallel().with_out_format('netcdf')  # boolean args are created without args
     """
     cmds_map = {'cmdpath': '-c', 'inputfile': '-i', 'second_input_file': '-I',
                 'eps': '-m', 'tend': '-e', 'tstart': '-s', 'datatime': '-T', 'datadate': '-D',
                 'ext': '-x', 'fmap': '-f', 'outdir': '-o', 'nameprefix': '-n', 
-                'scalefactor': '-S', 'offset': '-O', 
+                'scaleFactor': '-S', 'offset': '-O', 
                 'validMax': '-vM', 'validMin': '-vm', 'valueFormat': '-vf',
-                'log_level': '-l', 'log_dir': '-d', 'out_format': '-F',
+                'log_level': '-l', 'log_dir': '-d', 'out_format': '-F', 'outputStepUnits': '-U',
                 'create_intertable': '-B', 'parallel': '-X', 'intertable_dir': '-N'}
 
     def _a(self, opt, param=''):
         self._d[opt] = param
         return self
 
     def __init__(self, cmd_string=None, **params):
@@ -111,14 +111,15 @@
         self._vars['outMaps.ext'] = self.api_conf.get('ext')
         self._vars['outMaps.namePrefix'] = self.api_conf.get('namePrefix')
         self._vars['outMaps.scaleFactor'] = self.api_conf.get('scaleFactor')
         self._vars['outMaps.offset'] = self.api_conf.get('offset')
         self._vars['outMaps.validMin'] = self.api_conf.get('validMin')
         self._vars['outMaps.validMax'] = self.api_conf.get('validMax')
         self._vars['outMaps.valueFormat'] = self.api_conf.get('valueFormat')
+        self._vars['outMaps.outputStepUnits'] = self.api_conf.get('outputStepUnits')
         self._vars['outMaps.offset'] = self.api_conf.get('offset')
         self._vars['outMaps.outDir'] = './'  # not used
         self._vars['parameter.perturbationNumber'] = self.api_conf.get('perturbationNumber')
         self._vars['input.file2'] = self.api_conf.get('inputFile2')
         self._vars['input.two_resolution'] = bool(self._vars['input.file2'])
         self._vars['geopotential'] = self.api_conf.get('addGeopotential')
         self._to_add_geopotential = bool(self._vars['geopotential'])
@@ -184,14 +185,16 @@
             self._vars['outMaps.offset'] = self.api_conf['OutMaps'].get('offset') or 0.0
         if self._vars['outMaps.validMin'] is None:
             self._vars['outMaps.validMin'] = self.api_conf['OutMaps'].get('validMin')
         if self._vars['outMaps.validMax'] is None:
             self._vars['outMaps.validMax'] = self.api_conf['OutMaps'].get('validMax')
         if self._vars['outMaps.valueFormat'] is None:
             self._vars['outMaps.valueFormat'] = self.api_conf['OutMaps'].get('valueFormat')
+        if self._vars['outMaps.outputStepUnits'] is None:
+            self._vars['outMaps.outputStepUnits'] = self.api_conf['OutMaps'].get('outputStepUnits')
         if self._vars['outMaps.fmap'] == 1:
             self._vars['outMaps.fmap'] = self.api_conf['OutMaps'].get('fmap') or 1
         if self._vars['outMaps.ext'] == 1:
             self._vars['outMaps.ext'] = self.api_conf['OutMaps'].get('ext') or 1
 
         # if start, end and dataTime are defined via command line input args, these are ignored.
         # if missing, GribReader will read all timesteps for the parameter
```

### Comparing `pyg2p-3.2.2/src/pyg2p/main/config.py` & `pyg2p-3.2.3/src/pyg2p/main/config.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/context.py` & `pyg2p-3.2.3/src/pyg2p/main/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,15 @@
         self._vars['outMaps.ext'] = parsed_args['ext']
         self._vars['outMaps.namePrefix'] = parsed_args['namePrefix']
         self._vars['outMaps.scaleFactor'] = parsed_args['scaleFactor']
         self._vars['outMaps.offset'] = parsed_args['offset']
         self._vars['outMaps.validMin'] = parsed_args['validMin']
         self._vars['outMaps.validMax'] = parsed_args['validMax']
         self._vars['outMaps.valueFormat'] = parsed_args['valueFormat']
+        self._vars['outMaps.outputStepUnits'] = parsed_args['outputStepUnits']
         self._vars['outMaps.outDir'] = parsed_args['outDir']
         self._vars['parameter.perturbationNumber'] = parsed_args['perturbationNumber']
         self._vars['input.file2'] = parsed_args['inputFile2']
         self._vars['input.two_resolution'] = bool(self._vars['input.file2'])
         self._vars['geopotential'] = parsed_args['addGeopotential']
         self._to_add_geopotential = bool(self._vars['geopotential'])
         self._vars['download_configuration'] = parsed_args['downloadConf']
@@ -280,14 +281,15 @@
         parser.add_argument('-x', '--ext', help='Extension number step', type=int, default=1, metavar='extension_step')
         parser.add_argument('-n', '--namePrefix', help='Prefix name for maps', metavar='outfiles_prefix')
         parser.add_argument('-O', '--offset', help='Map offset', metavar='offset')
         parser.add_argument('-S', '--scaleFactor', help='Map scale factor', metavar='scale_factor')
         parser.add_argument('-vM', '--validMax', help='Max valid value', metavar='valid_max')
         parser.add_argument('-vm', '--validMin', help='Min valid value', metavar='valid_min')
         parser.add_argument('-vf', '--valueFormat', help='output value format (default f8)', metavar='value_format')
+        parser.add_argument('-U', '--outputStepUnits', help='output step units', metavar='output_step_units')
 
         # logging
         parser.add_argument('-l', '--loggerLevel', help='Console logging level', default='INFO',
                             choices=['ERROR', 'WARNING', 'INFO', 'DEBUG'], metavar='log_level')
 
         # interpolation lookup tables reading/writing
         parser.add_argument('-N', '--intertableDir', help='Alternate interpolation tables dir',
@@ -380,14 +382,16 @@
             self._vars['outMaps.offset'] = exec_conf['OutMaps'].get('@offset') or 0.0
         if self._vars['outMaps.validMin'] is None:
             self._vars['outMaps.validMin'] = exec_conf['OutMaps'].get('@validMin')
         if self._vars['outMaps.validMax'] is None:
             self._vars['outMaps.validMax'] = exec_conf['OutMaps'].get('@validMax')
         if self._vars['outMaps.valueFormat'] is None:
             self._vars['outMaps.valueFormat'] = exec_conf['OutMaps'].get('@valueFormat')
+        if self._vars['outMaps.outputStepUnits'] is None:
+            self._vars['outMaps.outputStepUnits'] = exec_conf['OutMaps'].get('@outputStepUnits')
         if self._vars['outMaps.fmap'] == 1:
             self._vars['outMaps.fmap'] = exec_conf['OutMaps'].get('@fmap') or 1
         if self._vars['outMaps.ext'] == 1:
             self._vars['outMaps.ext'] = exec_conf['OutMaps'].get('@ext') or 1
         if self._vars['outMaps.format'] == 'notset':
             # default out format to pcraster if not set from commandline nor in execution command json
             self._vars['outMaps.format'] = exec_conf['OutMaps'].get('@format') or 'pcraster'
```

### Comparing `pyg2p-3.2.2/src/pyg2p/main/controller.py` & `pyg2p-3.2.3/src/pyg2p/main/controller.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/interpolation/__init__.py` & `pyg2p-3.2.3/src/pyg2p/main/interpolation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/interpolation/grib_interpolation_lib.py` & `pyg2p-3.2.3/src/pyg2p/main/interpolation/grib_interpolation_lib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/interpolation/scipy_interpolation_lib.py` & `pyg2p-3.2.3/src/pyg2p/main/interpolation/scipy_interpolation_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from math import radians
 from sys import stdout
+import time
 
 import eccodes
 import numexpr as ne
 import numpy as np
 import math 
 import scipy.optimize as opt  
 from scipy.spatial import cKDTree as KDTree, Delaunay
@@ -318,14 +319,15 @@
 
     def interpolate(self, target_lons, target_lats):
         # Target coordinates  HAVE to be rotated coords in case GRIB grid is rotated
         # Example of target rotated coords are COSMO lat/lon/dem PCRASTER maps
         self.target_latsOR=target_lats
         self.target_lonsOR=target_lons
 
+        start = time.time()
         if self.mode != 'triangulation' and self.mode != 'bilinear_delaunay':
             stdout.write('Finding indexes for {} interpolation k={}\n'.format(self.mode, self.nnear))
             x, y, z = self.to_3d(target_lons, target_lats, to_regular=self.target_grid_is_rotated)
             efas_locations = np.vstack((x.ravel(), y.ravel(), z.ravel())).T
             distances, indexes = self.tree.query(efas_locations, k=self.nnear, n_jobs=self.njobs) 
         
         if self.mode == 'nearest' and self.nnear == 1:
@@ -350,14 +352,17 @@
                             result, weights, indexes = self._build_weights_triangulation(use_bilinear=True) 
                         else:
                             raise ApplicationException.get_exc(INVALID_INTERPOL_METHOD, 
                                         f"interpolation method not supported (mode = {self.mode}, nnear = {self.nnear})")
                     
                
         stdout.write('End scipy interpolation: {}\n'.format(now_string()))
+        end = time.time()
+        stdout.write('Interpolation time (sec): {}\n'.format(end - start))
+
         return result, weights, indexes
 
     def to_3d(self, lons, lats, rotate=False, to_regular=False):
         # these variables are used. Do NOT remove as they are used by numexpr
         lons = np.radians(lons)
         lats = np.radians(lats)
         x_formula = 'cos(lons) * cos(lats)'
@@ -410,53 +415,51 @@
             result[jinterpol] = wz
             jinterpol += 1
         stdout.write('{}{:>100}'.format(back_char, ' '))
         stdout.write('{}Building coeffs: {}/{} [outs: {}] (100%)\n'.format(back_char, jinterpol, num_cells, outs))
         stdout.flush()
         return result, idxs
 
+    # Invdist Optimized version (using broadcast)
     def _build_weights_invdist(self, distances, indexes, nnear):
         z = self.z
         result = mask_it(np.empty((len(distances),) + np.shape(z[0])), self._mv_target, 1)
-        jinterpol = 0
+        weights = empty((len(distances),) + (nnear,))
+        idxs = empty((len(indexes),) + (nnear,), fill_value=z.size, dtype=int)
         num_cells = result.size
-        back_char, progress_step = progress_step_and_backchar(num_cells)
+        back_char, _ = progress_step_and_backchar(num_cells)
 
         stdout.write('Skipping neighbors at distance > {}\n'.format(self.min_upper_bound))
-        stdout.write('{}Building coeffs: 0/{} [outs: 0] (0%)'.format(back_char, num_cells))
+        stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 0, 5, 0, 0))
         stdout.flush()
 
-        # weights will be saved in intertable along with indexes
-        weights = empty((len(distances),) + (nnear,))
-        idxs = empty((len(indexes),) + (nnear,), fill_value=z.size, dtype=int)
-        empty_array = empty(z[0].shape, self._mv_target)
-        outs = 0
-        for dist, ix in zip(distances, indexes):
-            if jinterpol % progress_step == 0:
-                stdout.write('{}Building coeffs: {}/{} [outs: {}] ({:.2f}%)'.format(back_char, jinterpol, num_cells, outs, jinterpol * 100. / num_cells))
-                stdout.flush()
-            if dist[0] <= 1e-10:
-                wz = z[ix[0]]  # take exactly the point, weight = 1
-                idxs[jinterpol] = ix
-                weights[jinterpol] = np.array([1., 0., 0., 0.])
-            elif dist[0] <= self.min_upper_bound:
-                w = ne.evaluate('1 / dist ** 2')
-                sums = ne.evaluate('sum(w)')
-                ne.evaluate('w/sums', out=w)
-                wz = np.dot(w, z[ix])  # weighted values (result)
-                weights[jinterpol] = w
-                idxs[jinterpol] = ix
-            else:
-                outs += 1
-                weights[jinterpol] = np.array([1., 0., 0., 0.])
-                wz = empty_array
-            result[jinterpol] = wz
-            jinterpol += 1
-        stdout.write('{}{:>100}'.format(back_char, ' '))
-        stdout.write('{}Building coeffs: {}/{} [outs: {}] (100%)\n'.format(back_char, jinterpol, num_cells, outs))
+        dist_leq_1e_10 = distances[:, 0] <= 1e-10
+        dist_leq_min_upper_bound = np.logical_and(~dist_leq_1e_10, distances[:, 0] <= self.min_upper_bound)
+        
+        # distances <= 1e-10 : take exactly the point, weight = 1
+        weights[dist_leq_1e_10] = np.array([1., 0., 0., 0.])
+        idxs[dist_leq_1e_10] = indexes[dist_leq_1e_10]
+        result[dist_leq_1e_10] = z[indexes[dist_leq_1e_10][:, 0]]
+
+        w = np.zeros_like(distances)
+        w[dist_leq_min_upper_bound] = 1. / distances[dist_leq_min_upper_bound] ** 2
+        stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 1, 5, 100/5))
+        stdout.flush()
+        sums = np.sum(w[dist_leq_min_upper_bound], axis=1, keepdims=True)
+        stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 2, 5, 2*100/5))
+        stdout.flush()
+        weights[dist_leq_min_upper_bound] = w[dist_leq_min_upper_bound] / sums
+        stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 3, 5, 3*100/5))
+        stdout.flush()
+        wz = np.einsum('ij,ij->i', weights, z[indexes])
+        stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 4, 5, 4*100/5))
+        stdout.flush()
+        idxs[dist_leq_min_upper_bound] = indexes[dist_leq_min_upper_bound]
+        result[dist_leq_min_upper_bound] = wz[dist_leq_min_upper_bound]
+        stdout.write('{}Building coeffs: {}/{} (100%)\n'.format(back_char, 5, 5))
         stdout.flush()
         return result, weights, idxs
 
     # take additional points from the KDTree close to the current point and replace the wrong ones with a new ones
     def replaceIndex(self, indexes_to_replace, indexes, nn, additional_points):
         additional_points += len(indexes_to_replace)
         # replace the unwanted index with next one:
```

### Comparing `pyg2p-3.2.2/src/pyg2p/main/manipulation/aggregator.py` & `pyg2p-3.2.3/src/pyg2p/main/manipulation/aggregator.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/manipulation/conversion.py` & `pyg2p-3.2.3/src/pyg2p/main/manipulation/conversion.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/manipulation/correction.py` & `pyg2p-3.2.3/src/pyg2p/main/manipulation/correction.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pyg2p.main.interpolation import Interpolator
 from pyg2p.main.interpolation.latlong import Dem
 from pyg2p.main.readers.grib import GRIBReader
 
 from pyg2p.main.config import GeopotentialsConfiguration
 import pyg2p.util.numeric
-from pyg2p.util.numeric import int_fill_value
+from netCDF4 import default_fillvals
 
 from ..interpolation.scipy_interpolation_lib import DEBUG_BILINEAR_INTERPOLATION, \
                                         DEBUG_MIN_LAT, DEBUG_MIN_LON, DEBUG_MAX_LAT, DEBUG_MAX_LON
 
 class Corrector(Loggable):
 
     instances = {}
@@ -71,15 +71,15 @@
                     assert(False)
             else:
                 dem = self._dem_values
             p = values
             gem = self._gem_values
             dem_mv = self._dem_missing_value
             gem_mv = self._gem_missing_value
-            mv = int_fill_value
+            mv = default_fillvals[values.dtype.str[1:]] # take missing values from the default netCDF fillvals values
             values = ne.evaluate(self._numexpr_eval)
             # mask out values (here is already output values with destination shape)
             values = ma.masked_where(pyg2p.util.numeric.get_masks(p), values)
         return values
 
     def _read_geo(self, grib_file, ctx):
         is_grib_interpolation = ctx.is_with_grib_interpolation
```

### Comparing `pyg2p-3.2.2/src/pyg2p/main/readers/grib.py` & `pyg2p-3.2.3/src/pyg2p/main/readers/grib.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,17 @@
             # cumulated rainfall rates could have the step zero instant message as kg/m^2, instead of kg/(m^2*s)
             if len(self._selected_grbs) > 1:
                 unit = codes_get(self._selected_grbs[1], 'units')
                 type_of_step = codes_get(self._selected_grbs[1], 'stepType')
             else:
                 type_of_step = codes_get(self._selected_grbs[0], 'stepType')
                 unit = codes_get(self._selected_grbs[0], 'units')
+
+            step_units = codes_get(self._selected_grbs[0], 'stepUnits', ktype=str) 
+
             type_of_level = codes_get(self._selected_grbs[0], 'levelType')
 
             missing_value = codes_get(self._selected_grbs[0], 'missingValue')
             data_date = codes_get(self._selected_grbs[0], 'dataDate')
             all_values = {}
             all_values_second_res = {}
             grid2 = None
@@ -200,15 +203,15 @@
                     all_values[step_key] = values
                 elif points_meridian != grid.num_points_along_meridian:
                     all_values_second_res[step_key] = values
 
             if grid2:
                 key_2nd_spatial_res = min(all_values_second_res.keys())
                 grid.set_2nd_resolution(grid2, key_2nd_spatial_res)
-            return Messages(all_values, missing_value, unit, type_of_level, type_of_step, grid, all_values_second_res, data_date=data_date)
+            return Messages(all_values, missing_value, unit, type_of_level, type_of_step, step_units, grid, all_values_second_res, data_date=data_date)
         # no messages found
         else:
             raise ApplicationException.get_exc(NO_MESSAGES, details=f'using {kwargs}')
 
     @staticmethod
     def _find_start_end_steps(gribs):
         # return input_steps,
```

### Comparing `pyg2p-3.2.2/src/pyg2p/main/readers/netcdf.py` & `pyg2p-3.2.3/src/pyg2p/main/readers/netcdf.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/readers/pcr.py` & `pyg2p-3.2.3/src/pyg2p/main/readers/pcr.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/main/writers/__init__.py` & `pyg2p-3.2.3/src/pyg2p/main/writers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         time_values = np.array(time_values, dtype=np.int32)
         out_values = np.array(out_values, dtype=np.float64)
         out_filename = self._name_netcdf_file()
         var_args = dict(prefix=self.ctx.get('outMaps.namePrefix'),
                         unit=self.ctx.get('parameter.conversionUnit'),
                         var_long_name=self.ctx.get('parameter.description'),
                         data_date=messages.data_date,
+                        grib_step_units=messages.step_units,
+                        output_step_units=self.ctx.get('outMaps.outputStepUnits'),
                         valid_max=self.ctx.get('outMaps.validMax'),
                         valid_min=self.ctx.get('outMaps.validMin'),
                         value_format=self.ctx.get('outMaps.valueFormat'),
                         offset=self.ctx.get('outMaps.offset'),
                         scale_factor=self.ctx.get('outMaps.scaleFactor'))
         self.writer.init_dataset(out_filename)
```

### Comparing `pyg2p-3.2.2/src/pyg2p/main/writers/pcr.py` & `pyg2p-3.2.3/src/pyg2p/main/writers/pcr.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/util/files.py` & `pyg2p-3.2.3/src/pyg2p/util/files.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/util/generics.py` & `pyg2p-3.2.3/src/pyg2p/util/generics.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/util/numeric.py` & `pyg2p-3.2.3/src/pyg2p/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/util/profiling/profilehooks.py` & `pyg2p-3.2.3/src/pyg2p/util/profiling/profilehooks.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p/util/strings.py` & `pyg2p-3.2.3/src/pyg2p/util/strings.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/src/pyg2p.egg-info/PKG-INFO` & `pyg2p-3.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,37 @@
-Metadata-Version: 2.1
-Name: pyg2p
-Version: 3.2.2
-Summary: Convert GRIB files to netCDF or PCRaster
-Author: Domenico Nappo
-Author-email: domenico.nappo@gmail.com
-License: EUPL 1.2
-Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Other Audience
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Physics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [ChangeLog](CHANGE_LOG.rst)
 
 
 # pyg2p
 pyg2p is a converter between GRIB and netCDF4/PCRaster files. 
 It can also manipulates GRIB messages (performing aggregation or simple unit conversion) before to apply format conversion.
 
 ## Installation
 
 To install package, you can use a python virtual environment or directly install dependencies and
 package at system level (executable script will be saved into /usr/local/bin in this case).
 
+### Using miniconda:
+
+
+* Install [miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+* Create a conda env named "pyg2penv" and install dependencies:
+
+  ```bash
+  conda create --name pyg2penv python=3.7 -c conda-forge
+  conda activate pyg2penv
+  ```
+
 >IMPORTANT: Before to launch setup, you need the following steps:
 
->Install eccodes: this can be done compiling from source code or using the available conda virtual environment package by running 
+>Install eccodes (and GDAL): this can be done compiling from source code or using the available conda virtual environment package by running 
 
 ```bash
-$ conda install -c conda-forge eccodes
+$ conda install -c conda-forge eccodes gdal
 ```
 
 >Configure geopotentials and intertables paths in
 configuration/global/global_conf.json. These paths are used by pyg2p to read
 geopotentials and intertables already configured. You may need to download files from FTP (launch `pyg2p -W` for this). 
 Users running pyg2p installed by a different user (ie. root) will configure similar paths for their own intertables 
 and geopotentials under his home folder. These paths will need write permissions.
@@ -53,15 +39,16 @@
 
 
 Grab last archive and extract it in a folder (or clone this repository) and follow these steps:
 
 ```bash
 $ cd pyg2p
 $ vim configuration/global/global_conf.json # to edit shared paths !!!
-$ python setup.py install
+$ pip install -r requirements.txt
+$ pip install .
 ```
 
 After installation, you will have all dependencies installed and an executable script 'pyg2p' (in a
 virtual environment, script is located under <VIRTUALENV_PATH>/bin folder otherwise under
 /usr/local/bin). To check correct installation of eccodes run the following command: 
 
 ```bash
@@ -225,15 +212,15 @@
 
 There are four sections of configuration.
 
 #### Aggregation
 Defines the aggregation method and step. Method can be `accumulation`, `average` or `instantaneous`.
 
 #### OutMaps
-Here you define interpolation method and paths to coordinates PCRaster maps, output unit time, the clone map etc.
+Here you define interpolation method and paths to coordinates netCDF/PCRaster maps, output unit time, the clone map etc.
 
 #### Interpolation
 This is a subelement of OutMaps. Here you define interpolation method (see later for details), paths
 to coordinates maps.
 
 #### Parameter
 In this section, you configure the parameter to select by using its shortName, as stored in GRIB file.
@@ -301,15 +288,23 @@
         </tr> 
     </thead>
     <tbody>
         <tr>
         <td><b>Execution</b></td>
         <td>name</td>
         <td>Descriptive name of the execution configuration.</td>
-        </tr>
+        </tr>        
+        <tr>
+        <td>&nbsp;</td><td>intertableDir</td><td>Alternative home folder for interpolation lookup
+tables, where pyg2p will load/save intertables. Folder must be existing. If not set, pyg2p will use intertables from ~/.pyg2p/intertables/</td>
+        </tr>    
+        <tr>
+        <td>&nbsp;</td><td>geopotentialDir</td><td>Alternative home folder for geopotential lookup
+tables. Folder must be existing. If not set, pyg2p will use geopotentials from ~/.pyg2p/geopotentials/</td>
+        </tr>    
         <tr>
         <td></td><td><b>Parameter</b></td><td>See relative table</td>
         </tr>
         <tr>
         <td></td><td><b>OutMaps</b></td><td>See relative table</td>
         </tr>
         <tr>
@@ -361,33 +356,52 @@
         <tr>
         <td><b>OutMaps</b></td><td>cloneMap</td><td>The clone map with area (must have a REAL cell
 type and missing values for points outside area
 of interest. A dem map works fine. A typical area boolean map will not).</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>unitTime</b></td><td>Time unit in hours of output maps. Tipical value
-is 24 (daily maps).</td>
+is 24 (daily maps). Used in "accumulation" operation</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>format</b></td><td>Output file format. Default 'pcraster'. Available
 formats are 'pcraster', 'netcdf'.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>namePrefix</b></td><td>Prefix for maps. Default is parameter
 shortName.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>fmap</b></td><td>First PCRaster map number. Default 1.</td>
+        <td>&nbsp;</td><td><b>scaleFactor</b></td><td>Scale factor of the output netCDF map. Default 1.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>Interpolation</b></td><td>See relative table.</td>
+        <td>&nbsp;</td><td><b>offset</b></td><td>Offset of the output netCDF map. Default 0.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>validMin</b></td><td>Minimum value of the output netCDF map. Values below will be set to nodata.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>validMax</b></td><td>Maximum value of the output netCDF map. Values above will be set to nodata.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>valueFormat</b></td><td>Variable type to use in the output netCDF map. Deafult f8. Available formats are: i1,i2,i4,i8,u1,u2,u4,u8,f4,f8 where i is integer, u is unsigned integer, f if float and the number corresponds to the number of bytes used (e.g. i4 is integer 32bits = 4 bytes)</td>
+        </tr>  
+        <tr>
+        <td>&nbsp;</td><td><b>outputStepUnits</b></td><td>Step units to use in output map. If not specified, it will use the stepUnits of the source Grib file. Available values are: 's': seconds, 'm': minutes, 'h': hours, '3h': 3h steps, '6h': 6h steps, '12h': 12h steps, 'D': days</td>
+        </tr>
+        <tr>      
+        <tr>
+        <td>&nbsp;</td><td><b>fmap</b></td><td>First PCRaster map number. Default 1.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>ext</b></td><td>Extension mode. It's the integer number
-defining the step numbers to skip when writing maps. Same as old grib2pcraster. Default 1.</td>
+defining the step numbers to skip when writing PCRaster maps. Same as old grib2pcraster. Default 1.</td>
+        </tr>
+        <tr>
+        <td>&nbsp;</td><td><b>Interpolation</b></td><td>See relative table.</td>
         </tr>
         <tr>
         <td colspan="3"><hr/></td>
         </tr>
         <tr>
         <td><b>Aggregation</b></td><td><b>step</b></td><td>Step of aggregation in hours.</td>
         </tr>
@@ -410,19 +424,15 @@
 “grib_invdist”</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>latMap</b></td><td>PCRaster map of target latitudes.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>lonMap</b></td><td>PCRaster map of target longitudes.</td>
-        </tr>
-        <tr>
-        <td>&nbsp;</td><td>intertableDir</td><td>Alternative home folder for interpolation lookup
-tables, where pyg2p will load/save intertables. Folder must be existing. If not set, pyg2p will use intertables from ~/.pyg2p/intertables/</td>
-        </tr>
+        </tr>        
     </tbody>
 </table>
 
 ## Usage
 
 To use the application, after the main configuration you need to configure a template JSON file for
 each type of extraction you need to perform.
@@ -451,78 +461,86 @@
 
 ### Input arguments
 
 If you run pyg2p without arguments, it shows help of all input arguments.
 
 ```console
 usage: pyg2p [-h] [-c json_file] [-o out_dir] [-i input_file]
-[-I input_file_2nd] [-s tstart] [-e tend] [-m eps_member]
-[-T data_time] [-D data_date] [-f fmap] [-F format] [-x extension_step]
-[-n outfiles_prefix] [-l log_level] [-N intertable_dir] [-B] [-X]
-[-t cmds_file] [-g geopotential] [-C path] [-z path] [-W dataset]
+             [-I input_file_2nd] [-s tstart] [-e tend] [-m eps_member]
+             [-T data_time] [-D data_date] [-f fmap] [-F format]
+             [-x extension_step] [-n outfiles_prefix] [-O offset]
+             [-S scale_factor] [-vM valid_max] [-vm valid_min]
+             [-vf value_format] [-U output_step_units] [-l log_level]
+             [-N intertable_dir] [-G geopotential_dir] [-B] [-X]
+             [-g geopotential] [-W dataset]
 
-Execute the grib to pcraster conversion using parameters from the input json configuration.
-Read user manual.
+Pyg2p: Execute the grib to netCDF/PCRaster conversion, using parameters
+from CLI/json configuration.
 
 optional arguments:
--h, --help show this help message and exit
--c json_file, --commandsFile json_file
-Path to json command file
--o out_dir, --outDir out_dir
-Path where output maps will be created.
--i input_file, --inputFile input_file
-Path to input grib.
--I input_file_2nd, --inputFile2 input_file_2nd
-Path to 2nd resolution input grib.
--s tstart, --start tstart
-Grib timestep start. It overwrites the tstart in json
-execution file.
--e tend, --end tend Grib timestep end. It overwrites the tend in json
-execution file.
--m eps_member, --perturbationNumber eps_member
-eps member number
--T data_time, --dataTime data_time
-To select messages by dataTime key value
--D data_date, --dataDate data_date
-<YYYYMMDD> to select messages by dataDate key value
--f fmap, --fmap fmap First map number
--F format, --format format
-Output format. Available options: netcdf, pcraster.
-Default pcraster
--x extension_step, --ext extension_step
-Extension number step
--n outfiles_prefix, --namePrefix outfiles_prefix
-Prefix name for maps
--l log_level, --loggerLevel log_level
-Console logging level
--N intertable_dir, --intertableDir intertable_dir
-interpolation tables dir
--B, --createIntertable
-create intertable file
--X, --interpolationParallel
-Use parallelization tools to make interpolation
-faster.If -B option is not passed or intertable
-already exists it does not have any effect.
--t cmds_file, --test cmds_file
-Path to a text file containing list of commands,
-defining a battery of tests. Then it will create diff
-pcraster maps and log alerts if differences are higher
-than a threshold (edit configuration in test.json)
--g geopotential, --addGeopotential geopotential
-Add the file to geopotentials.json configuration file, to use for correction. The file will be copied into
-the right folder (configuration/geopotentials) Note:
-shortName of geopotential must be "fis" or "z"
--C path, --convertConf path
-Convert old xml configuration to new json format
--z path, --convertIntertables path
-Convert old pyg2p intertables to new version and copy
-to user folders
--W dataset, --downloadConf dataset
-Download intertables and geopotentials (FTP settings
-defined in ftp.json)
+  -h, --help            show this help message and exit
+  -c json_file, --commandsFile json_file
+                        Path to json command file
+  -o out_dir, --outDir out_dir
+                        Path where output maps will be created.
+  -i input_file, --inputFile input_file
+                        Path to input grib.
+  -I input_file_2nd, --inputFile2 input_file_2nd
+                        Path to 2nd resolution input grib.
+  -s tstart, --start tstart
+                        Grib timestep start. It overwrites the tstart in json
+                        execution file.
+  -e tend, --end tend   Grib timestep end. It overwrites the tend in json
+                        execution file.
+  -m eps_member, --perturbationNumber eps_member
+                        eps member number
+  -T data_time, --dataTime data_time
+                        To select messages by dataTime key value
+  -D data_date, --dataDate data_date
+                        <YYYYMMDD> to select messages by dataDate key value
+  -f fmap, --fmap fmap  First map number
+  -F format, --format format
+                        Output format. Available options: netcdf, pcraster.
+                        Default pcraster
+  -x extension_step, --ext extension_step
+                        Extension number step
+  -n outfiles_prefix, --namePrefix outfiles_prefix
+                        Prefix name for maps
+  -O offset, --offset offset
+                        Map offset
+  -S scale_factor, --scaleFactor scale_factor
+                        Map scale factor
+  -vM valid_max, --validMax valid_max
+                        Max valid value
+  -vm valid_min, --validMin valid_min
+                        Min valid value
+  -vf value_format, --valueFormat value_format
+                        output value format (default f8)
+  -U output_step_units, --outputStepUnits output_step_units
+                        output step units
+  -l log_level, --loggerLevel log_level
+                        Console logging level
+  -N intertable_dir, --intertableDir intertable_dir
+                        Alternate interpolation tables dir
+  -G geopotential_dir, --geopotentialDir geopotential_dir
+                        Alternate geopotential dir
+  -B, --createIntertable
+                        Flag to create intertable file
+  -X, --interpolationParallel
+                        Use parallelization tools to make interpolation
+                        faster.If -B option is not passed or intertable
+                        already exists it does not have any effect.
+  -g geopotential, --addGeopotential geopotential
+                        Add the file to geopotentials.json configuration file,
+                        to use for correction. The file will be copied into
+                        the right folder (configuration/geopotentials) Note:
+                        shortName of geopotential must be "fis" or "z"
+  -W dataset, --downloadConf dataset
+                        Download intertables and geopotentials (FTP settings
+                        defined in ftp.json)
 ```
 #### Usage examples:
 
 ```bash
 pyg2p -c ./exec1.json -i ./input.grib -o /out/dir -s 12 -e 36 -F netcdf
 pyg2p -c ./exec2.json -i ./input.grib -o /out/dir -m 10 -l INFO --format netcdf
 pyg2p -c ./exec3.json -i ./input.grib -I /input2ndres.grib -o /out/dir -m 10 -l DEBUG
@@ -686,24 +704,30 @@
   "@mode": "bilinear_delaunay"}
 }
 ```
 
 ## OutMaps configuration
 
 Interpolation is configured under the OutMaps tag. With additional attributes, you also configure
-resulting PCRaster maps. Output dir is ./ by default or you can set it via command line using the
+resulting PCRaster or netCDF maps. Output dir is ./ by default or you can set it via command line using the
 option -o (--outDir).
 
 | Attribute      | Details                                                                                                                           |
 |----------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | namePrefix     | Prefix name for output map files. Default is the value of shortName key.                                                          |
-| **unitTime**   | Unit time in hours for results. This is used during aggregation operations.                                                       |
+| unitTime       | Unit time in hours for results. This is used during aggregation operations.                                                       |
 | fmap           | Extension number for the first map. Default 1.                                                                                    |
 | ext            | Extension mode. It's the integer number defining the step numbers to skip when writing maps. Same as old grib2pcraster. Default 1.|
-| **cloneMap**   | Path to a PCRaster clone map, needed by PCRaster libraries to write a new map on disk.                                            |
+| cloneMap       | Path to a PCRaster clone map, needed by PCRaster libraries to write a new map on disk.                                            |
+| scaleFactor    | Scale factor of the output netCDF map. Default 1. |
+| offset         | Offset of the output netCDF map. Default 0. |
+| validMin       | Minimum value of the output netCDF map. Values below will be set to nodata. |
+| validMax       | Maximum value of the output netCDF map. Values above will be set to nodata. |
+| valueFormat    | Variable type to use in the output netCDF map. Deafult f8. Available formats are: i1,i2,i4,i8,u1,u2,u4,u8,f4,f8 where i is integer, u is unsigned integer, f if float and the number corresponds to the number of bytes used (e.g. i4 is integer 32bits = 4 bytes) | 
+| outputStepUnits | Step units to use in output map. If not specified, it will use the stepUnits of the source Grib file. Available values are: 's': seconds, 'm': minutes, 'h': hours, '3h': 3h steps, '6h': 6h steps, '12h': 12h steps, 'D': days |
 
 ## Aggregation
 
 Values from grib files can be aggregated before to write the final PCRaster maps. There are two kinds of aggregation available: average and accumulation. 
 The JSON configuration in the execution file will look like:
 
 ```json
@@ -1221,12 +1245,10 @@
 Dimensions:
         xc: Number of rows of area/clone map
         yc: Number of cols of area/clone map
         time: Unlimited dimension for time steps
 Variables:
         lon: 2D array with shape (yc, xc)
         lat: 2D array with shape (yc, xc)
-        time_nc: 1D array of values representing hours since dataDate of first grib message (endStep)
+        time_nc: 1D array of values representing hours/days since dataDate of first grib message (endStep)
         values_nc: a 3D array of dimensions (time, yc, xc), with coordinates set to 'lon, lat'.
 ```
-
-
```

### Comparing `pyg2p-3.2.2/src/pyg2p.egg-info/SOURCES.txt` & `pyg2p-3.2.3/src/pyg2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_cp.json` & `pyg2p-3.2.3/templates/AFFS_cp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_lsp.json` & `pyg2p-3.2.3/templates/AFFS_lsp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_rg.json` & `pyg2p-3.2.3/templates/AFFS_rg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_rn.json` & `pyg2p-3.2.3/templates/AFFS_rn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_ta.json` & `pyg2p-3.2.3/templates/AFFS_ta.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_td.json` & `pyg2p-3.2.3/templates/AFFS_td.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_wu.json` & `pyg2p-3.2.3/templates/AFFS_wu.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/AFFS_wv.json` & `pyg2p-3.2.3/templates/AFFS_wv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_15d.json` & `pyg2p-3.2.3/templates/EUE_15d.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_15d_glob.json` & `pyg2p-3.2.3/templates/EUE_15d_glob.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim.json` & `pyg2p-3.2.3/templates/EUE_RainAnim.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_CV.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_CV.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_CV_g.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_CV_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_CV_scipy.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_CV_scipy_inv.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_inv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_CV_scipy_nn.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_CV_scipy_nn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_agg.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_agg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_december.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_december.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_g.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/EUE_RainAnim_scipy.json` & `pyg2p-3.2.3/templates/EUE_RainAnim_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/UKMO_t24_LA.json` & `pyg2p-3.2.3/templates/UKMO_t24_LA.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/UKMO_t24_LA_g.json` & `pyg2p-3.2.3/templates/UKMO_t24_LA_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/UKMO_t24_LA_scipy.json` & `pyg2p-3.2.3/templates/UKMO_t24_LA_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cin.json` & `pyg2p-3.2.3/templates/cin.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_e06.json` & `pyg2p-3.2.3/templates/cosmo_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_e06_newmaps.json` & `pyg2p-3.2.3/templates/cosmo_e06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_e06_scipy.json` & `pyg2p-3.2.3/templates/cosmo_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_r06.json` & `pyg2p-3.2.3/templates/cosmo_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_r06_newmaps.json` & `pyg2p-3.2.3/templates/cosmo_r06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_r06_scipy.json` & `pyg2p-3.2.3/templates/cosmo_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_t24.json` & `pyg2p-3.2.3/templates/cosmo_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_t24_newmaps.json` & `pyg2p-3.2.3/templates/cosmo_t24_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/cosmo_t24_scipy.json` & `pyg2p-3.2.3/templates/cosmo_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_e06.json` & `pyg2p-3.2.3/templates/dwd_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_e06_2.json` & `pyg2p-3.2.3/templates/dwd_e06_2.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_e06_2nd.json` & `pyg2p-3.2.3/templates/dwd_e06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_e06_3.json` & `pyg2p-3.2.3/templates/dwd_e06_3.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_e06_scipy.json` & `pyg2p-3.2.3/templates/dwd_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_r06.json` & `pyg2p-3.2.3/templates/dwd_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_r06_2nd.json` & `pyg2p-3.2.3/templates/dwd_r06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_r06_efas.json` & `pyg2p-3.2.3/templates/dwd_r06_efas.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_r06_gmi.json` & `pyg2p-3.2.3/templates/dwd_r06_gmi.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_r06_scipy.json` & `pyg2p-3.2.3/templates/dwd_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_t24.json` & `pyg2p-3.2.3/templates/dwd_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_t24_2nd.json` & `pyg2p-3.2.3/templates/dwd_t24_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwd_t24_scipy.json` & `pyg2p-3.2.3/templates/dwd_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/dwdl_r06.json` & `pyg2p-3.2.3/templates/dwdl_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/efas_sro.json` & `pyg2p-3.2.3/templates/efas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_e06.json` & `pyg2p-3.2.3/templates/eud_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_e06_scipy.json` & `pyg2p-3.2.3/templates/eud_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_r06.json` & `pyg2p-3.2.3/templates/eud_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_r06_scipy.json` & `pyg2p-3.2.3/templates/eud_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_r24.json` & `pyg2p-3.2.3/templates/eud_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_r24_scipy.json` & `pyg2p-3.2.3/templates/eud_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_t24.json` & `pyg2p-3.2.3/templates/eud_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eud_t24_scipy.json` & `pyg2p-3.2.3/templates/eud_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_e24.json` & `pyg2p-3.2.3/templates/eue_e24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_e24_scipy.json` & `pyg2p-3.2.3/templates/eue_e24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_r24.json` & `pyg2p-3.2.3/templates/eue_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_r24_15days.json` & `pyg2p-3.2.3/templates/eue_r24_15days.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_r24_15days_g.json` & `pyg2p-3.2.3/templates/eue_r24_15days_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_r24_15days_noagg.json` & `pyg2p-3.2.3/templates/eue_r24_15days_noagg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_r24_15days_scipy.json` & `pyg2p-3.2.3/templates/eue_r24_15days_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_r24_scipy.json` & `pyg2p-3.2.3/templates/eue_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_t24.json` & `pyg2p-3.2.3/templates/eue_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/eue_t24_scipy.json` & `pyg2p-3.2.3/templates/eue_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/glofas_sro.json` & `pyg2p-3.2.3/templates/glofas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/glofas_sro_scipy.json` & `pyg2p-3.2.3/templates/glofas_sro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/glofas_ssro.json` & `pyg2p-3.2.3/templates/glofas_ssro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/glofas_ssro_scipy.json` & `pyg2p-3.2.3/templates/glofas_ssro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test.json` & `pyg2p-3.2.3/templates/octahedral_test.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test_global.json` & `pyg2p-3.2.3/templates/octahedral_test_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test_global_invdist.json` & `pyg2p-3.2.3/templates/octahedral_test_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test_invdist.json` & `pyg2p-3.2.3/templates/octahedral_test_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test_scipy.json` & `pyg2p-3.2.3/templates/octahedral_test_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test_scipy_global.json` & `pyg2p-3.2.3/templates/octahedral_test_scipy_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test_scipy_global_invdist.json` & `pyg2p-3.2.3/templates/octahedral_test_scipy_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/octahedral_test_scipy_invdist.json` & `pyg2p-3.2.3/templates/octahedral_test_scipy_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/rn_false_mv.json` & `pyg2p-3.2.3/templates/rn_false_mv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_r06.json` & `pyg2p-3.2.3/templates/tigge_lam_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_r06_rotated.json` & `pyg2p-3.2.3/templates/tigge_lam_r06_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_r06_scipy.json` & `pyg2p-3.2.3/templates/tigge_lam_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_r06_scipy_rotated.json` & `pyg2p-3.2.3/templates/tigge_lam_r06_scipy_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_t24.json` & `pyg2p-3.2.3/templates/tigge_lam_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_t24_rotated.json` & `pyg2p-3.2.3/templates/tigge_lam_t24_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_t24_scipy.json` & `pyg2p-3.2.3/templates/tigge_lam_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.2/templates/tigge_lam_t24_scipy_rotated.json` & `pyg2p-3.2.3/templates/tigge_lam_t24_scipy_rotated.json`

 * *Files identical despite different names*

