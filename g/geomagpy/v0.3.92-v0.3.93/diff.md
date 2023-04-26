# Comparing `tmp/GeomagPy-v0.3.92.tar.gz` & `tmp/GeomagPy-v0.3.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GeomagPy-v0.3.92.tar", last modified: Fri Apr  7 17:32:24 2017, max compression
+gzip compressed data, was "dist/GeomagPy-v0.3.93.tar", last modified: Thu Jun 22 12:11:42 2017, max compression
```

## Comparing `GeomagPy-v0.3.92.tar` & `GeomagPy-v0.3.93.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/GeomagPy.egg-info/
--rw-rw-r--   0 leon      (1000) leon      (1000)   102748 2017-04-07 17:32:23.000000 GeomagPy-v0.3.92/GeomagPy.egg-info/PKG-INFO
--rw-rw-r--   0 leon      (1000) leon      (1000)       49 2017-04-07 17:32:23.000000 GeomagPy-v0.3.92/GeomagPy.egg-info/requires.txt
--rw-rw-r--   0 leon      (1000) leon      (1000)        6 2017-04-07 17:32:23.000000 GeomagPy-v0.3.92/GeomagPy.egg-info/top_level.txt
--rw-rw-r--   0 leon      (1000) leon      (1000)     2402 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/GeomagPy.egg-info/SOURCES.txt
--rw-rw-r--   0 leon      (1000) leon      (1000)        1 2017-04-07 17:32:23.000000 GeomagPy-v0.3.92/GeomagPy.egg-info/dependency_links.txt
--rw-rw-r--   0 leon      (1000) leon      (1000)   102748 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/PKG-INFO
--rw-rw-r--   0 leon      (1000) leon      (1000)    82357 2017-04-05 22:56:52.000000 GeomagPy-v0.3.92/README.txt
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/magpy/
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/magpy/gui/
--rw-rw-r--   0 leon      (1000) leon      (1000)    55259 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/gui/magpy128.xpm
--rwxrwxr-x   0 leon      (1000) leon      (1000)    10276 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/gui/monitorpage.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)   172671 2017-04-07 16:03:26.000000 GeomagPy-v0.3.92/magpy/gui/magpy_gui.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     4887 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/metapage.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)     6994 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/streampage.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)       99 2016-10-10 15:39:07.000000 GeomagPy-v0.3.92/magpy/gui/xmagpy.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)     5019 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/absolutespage.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     1315 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/reportpage.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)      327 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/magpy_gui_test.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)     5932 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/analysispage.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)    22295 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/developpage.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)       99 2016-09-03 07:23:37.000000 GeomagPy-v0.3.92/magpy/gui/xmagpy
--rw-rw-r--   0 leon      (1000) leon      (1000)     5823 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/gui/magpy.png
--rw-rw-r--   0 leon      (1000) leon      (1000)      541 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/gui/__init__.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)   173242 2017-04-07 15:17:15.000000 GeomagPy-v0.3.92/magpy/gui/dialogclasses.py
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/magpy/collector/
--rw-rw-r--   0 leon      (1000) leon      (1000)     8244 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/collector/collector-martas.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     1423 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/collector/collector-marcos.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    24760 2017-03-14 15:28:23.000000 GeomagPy-v0.3.92/magpy/collector/subscribe2client.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    11402 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/collector/subscribe2marcos.py
--rw-rw-r--   0 leon      (1000) leon      (1000)      319 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/collector/__init__.py
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/magpy/opt/
--rw-rw-r--   0 leon      (1000) leon      (1000)    15552 2017-04-05 21:40:03.000000 GeomagPy-v0.3.92/magpy/opt/analysismonitor.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)     7284 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/opt/cred.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)    56136 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/opt/stormdet.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     8524 2016-06-23 06:04:52.000000 GeomagPy-v0.3.92/magpy/opt/Table.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     1988 2016-10-10 15:39:07.000000 GeomagPy-v0.3.92/magpy/opt/mails.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     9263 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/opt/emd.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     4745 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/opt/sigfig.py
--rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/opt/__init__.py
--rw-rw-r--   0 leon      (1000) leon      (1000)       24 2017-04-07 17:27:30.000000 GeomagPy-v0.3.92/magpy/version.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)    98764 2017-03-30 12:34:58.000000 GeomagPy-v0.3.92/magpy/absolutes.py
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/magpy/lib/
--rw-rw-r--   0 leon      (1000) leon      (1000)     8699 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_latex.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    10725 2017-03-10 07:43:33.000000 GeomagPy-v0.3.92/magpy/lib/format_gdas.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    33242 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_wdc.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     1157 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_rcs.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     2338 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_iono.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     4436 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_neic.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     7184 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_didd.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     3452 2016-10-10 15:39:07.000000 GeomagPy-v0.3.92/magpy/lib/format_autodif_fread.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    13452 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_gsm19.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    15930 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/magpy_formats.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     4672 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_gfz.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     5996 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_sfs.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     2876 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_json.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    18698 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_lemi.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    41282 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_wic.py
--rw-rw-r--   0 leon      (1000) leon      (1000)        0 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_autodif.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     4651 2016-06-23 06:04:52.000000 GeomagPy-v0.3.92/magpy/lib/format_bdv.py
--rw-rw-r--   0 leon      (1000) leon      (1000)   112295 2017-04-05 21:26:16.000000 GeomagPy-v0.3.92/magpy/lib/format_imf.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    10861 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_wik.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    20402 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_iaga02.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     1703 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_env05.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     5567 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_dtu.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     5555 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_cr800.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    22380 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_abs_magpy.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    16518 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_noaa.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     4587 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/format_pos1.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    53288 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/lib/format_magpy.py
--rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/__init__.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     1020 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/lib/magpy_absformats.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)    14332 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/transfer.py
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/magpy/examples/
--rw-rw-r--   0 leon      (1000) leon      (1000)  1097714 2016-06-02 14:51:17.000000 GeomagPy-v0.3.92/magpy/examples/example1.cdf
--rw-r--r--   0 leon      (1000) leon      (1000)  4850331 2016-05-19 01:18:30.000000 GeomagPy-v0.3.92/magpy/examples/example5.cdf
--rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-10-10 15:39:07.000000 GeomagPy-v0.3.92/magpy/examples/__init__.py
--rw-rw-r--   0 leon      (1000) leon      (1000)   110762 2017-04-07 14:42:14.000000 GeomagPy-v0.3.92/magpy/mpplot.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)   492749 2017-04-07 16:12:57.000000 GeomagPy-v0.3.92/magpy/stream.py
-drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/magpy/acquisition/
--rw-rw-r--   0 leon      (1000) leon      (1000)     5937 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/acquisition/csprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     6260 2017-01-30 15:11:40.000000 GeomagPy-v0.3.92/magpy/acquisition/bm35protocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    14536 2016-10-07 12:09:58.000000 GeomagPy-v0.3.92/magpy/acquisition/pos1protocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     6432 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/acquisition/gsm90protocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     6917 2016-10-07 12:09:58.000000 GeomagPy-v0.3.92/magpy/acquisition/envprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    13909 2016-10-07 12:09:58.000000 GeomagPy-v0.3.92/magpy/acquisition/gsmp20protocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    13871 2016-10-10 15:39:07.000000 GeomagPy-v0.3.92/magpy/acquisition/arduinoprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     6827 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/acquisition/gsm19protocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    11684 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/acquisition/acquisition.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     5912 2016-10-07 12:09:58.000000 GeomagPy-v0.3.92/magpy/acquisition/kernprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     7670 2016-10-07 12:09:58.000000 GeomagPy-v0.3.92/magpy/acquisition/cobs_ws_protocols.py
--rw-rw-r--   0 leon      (1000) leon      (1000)     2578 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/acquisition/STANDARD_KEYS.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    15879 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/acquisition/callprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    14898 2016-10-07 12:09:58.000000 GeomagPy-v0.3.92/magpy/acquisition/lemiprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/acquisition/__init__.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    11129 2016-10-07 12:09:58.000000 GeomagPy-v0.3.92/magpy/acquisition/palmacqprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)    15665 2017-02-15 21:12:22.000000 GeomagPy-v0.3.92/magpy/acquisition/owprotocol.py
--rw-rw-r--   0 leon      (1000) leon      (1000)      614 2016-05-13 21:38:32.000000 GeomagPy-v0.3.92/magpy/__init__.py
--rwxrwxr-x   0 leon      (1000) leon      (1000)   141418 2017-02-18 11:00:40.000000 GeomagPy-v0.3.92/magpy/database.py
--rw-rw-r--   0 leon      (1000) leon      (1000)       59 2017-04-07 17:32:24.000000 GeomagPy-v0.3.92/setup.cfg
--rw-rw-r--   0 leon      (1000) leon      (1000)      860 2016-10-10 15:39:07.000000 GeomagPy-v0.3.92/setup.py
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/GeomagPy.egg-info/
+-rw-rw-r--   0 leon      (1000) leon      (1000)   102748 2017-06-22 12:11:38.000000 GeomagPy-v0.3.93/GeomagPy.egg-info/PKG-INFO
+-rw-rw-r--   0 leon      (1000) leon      (1000)       49 2017-06-22 12:11:38.000000 GeomagPy-v0.3.93/GeomagPy.egg-info/requires.txt
+-rw-rw-r--   0 leon      (1000) leon      (1000)        6 2017-06-22 12:11:38.000000 GeomagPy-v0.3.93/GeomagPy.egg-info/top_level.txt
+-rw-rw-r--   0 leon      (1000) leon      (1000)     2410 2017-06-22 12:11:41.000000 GeomagPy-v0.3.93/GeomagPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 leon      (1000) leon      (1000)        1 2017-06-22 12:11:38.000000 GeomagPy-v0.3.93/GeomagPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 leon      (1000) leon      (1000)   102748 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/PKG-INFO
+-rw-rw-r--   0 leon      (1000) leon      (1000)    82357 2017-04-05 22:56:52.000000 GeomagPy-v0.3.93/README.txt
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/magpy/
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/magpy/gui/
+-rw-rw-r--   0 leon      (1000) leon      (1000)    55259 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/gui/magpy128.xpm
+-rwxrwxr-x   0 leon      (1000) leon      (1000)    10276 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/gui/monitorpage.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)   174515 2017-05-11 14:18:38.000000 GeomagPy-v0.3.93/magpy/gui/magpy_gui.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     4887 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/metapage.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)     6994 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/streampage.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)       99 2016-10-10 15:39:07.000000 GeomagPy-v0.3.93/magpy/gui/xmagpy.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)     5019 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/absolutespage.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     1315 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/reportpage.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)      327 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/magpy_gui_test.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)     5932 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/analysispage.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)    22295 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/developpage.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)       99 2016-09-03 07:23:37.000000 GeomagPy-v0.3.93/magpy/gui/xmagpy
+-rw-rw-r--   0 leon      (1000) leon      (1000)     5823 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/gui/magpy.png
+-rw-rw-r--   0 leon      (1000) leon      (1000)      541 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/gui/__init__.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)   173242 2017-05-11 14:19:04.000000 GeomagPy-v0.3.93/magpy/gui/dialogclasses.py
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/magpy/collector/
+-rw-rw-r--   0 leon      (1000) leon      (1000)     8244 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/collector/collector-martas.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     1423 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/collector/collector-marcos.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    24760 2017-03-14 15:28:23.000000 GeomagPy-v0.3.93/magpy/collector/subscribe2client.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    11402 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/collector/subscribe2marcos.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)      319 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/collector/__init__.py
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/magpy/opt/
+-rw-rw-r--   0 leon      (1000) leon      (1000)    15552 2017-04-05 21:40:03.000000 GeomagPy-v0.3.93/magpy/opt/analysismonitor.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)     7284 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/opt/cred.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)    56136 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/opt/stormdet.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     8524 2016-06-23 06:04:52.000000 GeomagPy-v0.3.93/magpy/opt/Table.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     1988 2016-10-10 15:39:07.000000 GeomagPy-v0.3.93/magpy/opt/mails.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     9263 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/opt/emd.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     4745 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/opt/sigfig.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/opt/__init__.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)       24 2017-05-15 18:49:33.000000 GeomagPy-v0.3.93/magpy/version.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)    98764 2017-03-30 12:34:58.000000 GeomagPy-v0.3.93/magpy/absolutes.py
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/magpy/lib/
+-rw-rw-r--   0 leon      (1000) leon      (1000)     8699 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/format_latex.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    10725 2017-03-10 07:43:33.000000 GeomagPy-v0.3.93/magpy/lib/format_gdas.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    33242 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_wdc.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     1157 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/format_rcs.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     2338 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_iono.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     4436 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_neic.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     7184 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_didd.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     3452 2016-10-10 15:39:07.000000 GeomagPy-v0.3.93/magpy/lib/format_autodif_fread.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    13452 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/format_gsm19.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    16346 2017-05-11 11:55:16.000000 GeomagPy-v0.3.93/magpy/lib/magpy_formats.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     4672 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_gfz.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     5996 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_sfs.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     2871 2017-04-28 10:03:30.000000 GeomagPy-v0.3.93/magpy/lib/format_json.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    18698 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_lemi.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     4014 2017-04-28 10:03:30.000000 GeomagPy-v0.3.93/magpy/lib/format_nc.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    41282 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_wic.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)        0 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/format_autodif.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     4651 2016-06-23 06:04:52.000000 GeomagPy-v0.3.93/magpy/lib/format_bdv.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)   112925 2017-04-28 10:03:30.000000 GeomagPy-v0.3.93/magpy/lib/format_imf.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    10861 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_wik.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    20402 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_iaga02.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     5567 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/format_dtu.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     5555 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_cr800.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    22380 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/lib/format_abs_magpy.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    16518 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/format_noaa.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     4587 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/format_pos1.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    53301 2017-05-15 15:55:18.000000 GeomagPy-v0.3.93/magpy/lib/format_magpy.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/__init__.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     1020 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/lib/magpy_absformats.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)    14397 2017-04-28 10:03:30.000000 GeomagPy-v0.3.93/magpy/transfer.py
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/magpy/examples/
+-rw-rw-r--   0 leon      (1000) leon      (1000)  1097714 2016-06-02 14:51:17.000000 GeomagPy-v0.3.93/magpy/examples/example1.cdf
+-rw-r--r--   0 leon      (1000) leon      (1000)  4850331 2016-05-19 01:18:30.000000 GeomagPy-v0.3.93/magpy/examples/example5.cdf
+-rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-10-10 15:39:07.000000 GeomagPy-v0.3.93/magpy/examples/__init__.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)   110686 2017-04-28 10:03:30.000000 GeomagPy-v0.3.93/magpy/mpplot.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)   495667 2017-06-19 08:21:13.000000 GeomagPy-v0.3.93/magpy/stream.py
+drwxrwxr-x   0 leon      (1000) leon      (1000)        0 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/magpy/acquisition/
+-rw-rw-r--   0 leon      (1000) leon      (1000)     5937 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/acquisition/csprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     6260 2017-01-30 15:11:40.000000 GeomagPy-v0.3.93/magpy/acquisition/bm35protocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    14813 2017-04-13 08:18:10.000000 GeomagPy-v0.3.93/magpy/acquisition/pos1protocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     6432 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/acquisition/gsm90protocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     6917 2016-10-07 12:09:58.000000 GeomagPy-v0.3.93/magpy/acquisition/envprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    13909 2016-10-07 12:09:58.000000 GeomagPy-v0.3.93/magpy/acquisition/gsmp20protocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    13871 2016-10-10 15:39:07.000000 GeomagPy-v0.3.93/magpy/acquisition/arduinoprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     6827 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/acquisition/gsm19protocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    11684 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/acquisition/acquisition.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     5912 2016-10-07 12:09:58.000000 GeomagPy-v0.3.93/magpy/acquisition/kernprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     7670 2016-10-07 12:09:58.000000 GeomagPy-v0.3.93/magpy/acquisition/cobs_ws_protocols.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)     2578 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/acquisition/STANDARD_KEYS.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    15879 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/acquisition/callprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    14898 2016-10-07 12:09:58.000000 GeomagPy-v0.3.93/magpy/acquisition/lemiprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)      318 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/acquisition/__init__.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    11129 2016-10-07 12:09:58.000000 GeomagPy-v0.3.93/magpy/acquisition/palmacqprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)    15665 2017-02-15 21:12:22.000000 GeomagPy-v0.3.93/magpy/acquisition/owprotocol.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)      614 2016-05-13 21:38:32.000000 GeomagPy-v0.3.93/magpy/__init__.py
+-rwxrwxr-x   0 leon      (1000) leon      (1000)   144933 2017-05-29 14:40:56.000000 GeomagPy-v0.3.93/magpy/database.py
+-rw-rw-r--   0 leon      (1000) leon      (1000)   723842 2017-05-02 19:16:14.000000 GeomagPy-v0.3.93/README.rst
+-rw-rw-r--   0 leon      (1000) leon      (1000)       59 2017-06-22 12:11:42.000000 GeomagPy-v0.3.93/setup.cfg
+-rw-rw-r--   0 leon      (1000) leon      (1000)      860 2016-10-10 15:39:07.000000 GeomagPy-v0.3.93/setup.py
```

### Comparing `GeomagPy-v0.3.92/GeomagPy.egg-info/PKG-INFO` & `GeomagPy-v0.3.93/GeomagPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: GeomagPy
-Version: v0.3.92
+Version: v0.3.93
 Summary: Geomagnetic analysis tools.
 Home-page: http://pypi.python.org/pypi/GeomagPy/
 Author: R. Leonhardt, R. Bailey, M. Miklavec
 Author-email: roman.leonhardt@zamg.ac.at
 License: LICENSE.txt
 Description: ===========
         MagPy
```

### Comparing `GeomagPy-v0.3.92/GeomagPy.egg-info/SOURCES.txt` & `GeomagPy-v0.3.93/GeomagPy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.rst
 README.txt
 setup.py
 GeomagPy.egg-info/PKG-INFO
 GeomagPy.egg-info/SOURCES.txt
 GeomagPy.egg-info/dependency_links.txt
 GeomagPy.egg-info/requires.txt
 GeomagPy.egg-info/top_level.txt
@@ -56,25 +57,25 @@
 magpy/lib/format_abs_magpy.py
 magpy/lib/format_autodif.py
 magpy/lib/format_autodif_fread.py
 magpy/lib/format_bdv.py
 magpy/lib/format_cr800.py
 magpy/lib/format_didd.py
 magpy/lib/format_dtu.py
-magpy/lib/format_env05.py
 magpy/lib/format_gdas.py
 magpy/lib/format_gfz.py
 magpy/lib/format_gsm19.py
 magpy/lib/format_iaga02.py
 magpy/lib/format_imf.py
 magpy/lib/format_iono.py
 magpy/lib/format_json.py
 magpy/lib/format_latex.py
 magpy/lib/format_lemi.py
 magpy/lib/format_magpy.py
+magpy/lib/format_nc.py
 magpy/lib/format_neic.py
 magpy/lib/format_noaa.py
 magpy/lib/format_pos1.py
 magpy/lib/format_rcs.py
 magpy/lib/format_sfs.py
 magpy/lib/format_wdc.py
 magpy/lib/format_wic.py
```

### Comparing `GeomagPy-v0.3.92/PKG-INFO` & `GeomagPy-v0.3.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: GeomagPy
-Version: v0.3.92
+Version: v0.3.93
 Summary: Geomagnetic analysis tools.
 Home-page: http://pypi.python.org/pypi/GeomagPy/
 Author: R. Leonhardt, R. Bailey, M. Miklavec
 Author-email: roman.leonhardt@zamg.ac.at
 License: LICENSE.txt
 Description: ===========
         MagPy
```

### Comparing `GeomagPy-v0.3.92/README.txt` & `GeomagPy-v0.3.93/README.txt`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/magpy128.xpm` & `GeomagPy-v0.3.93/magpy/gui/magpy128.xpm`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/monitorpage.py` & `GeomagPy-v0.3.93/magpy/gui/monitorpage.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/magpy_gui.py` & `GeomagPy-v0.3.93/magpy/gui/magpy_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,14 +257,63 @@
         #    msubs.output = 'file'
         #    #sensorid = row[0]
         #    #module = row[1]
         #    #line = row[2]
         #    #msubs.storeData(li,parameterstring.split(','))
 
 
+    def startMQTTMonitor(self,**kwargs):
+        """
+        DEFINITION:
+            embbed matplotlib figure in canvas for mointoring
+
+        PARAMETERS:
+            kwargs:  - all plot args
+        """
+
+        dataid = self.datavars[0]
+        parameter = self.datavars[1]
+        period = self.datavars[2]
+        pad = self.datavars[3]
+        currentdate = self.datavars[4]
+        unitlist = self.datavars[5]
+        coverage = self.datavars[6]  # coverage
+        updatetime = self.datavars[7]
+        db = self.datavars[8]
+
+        """
+        # convert parameter list to a dbselect sql format
+        parameterstring = 'time,'+parameter
+
+        # Test whether data is available at all with selected keys and dataid
+        li = sorted(dbselect(db, parameterstring, dataid, expert='ORDER BY time DESC LIMIT {}'.format(int(coverage))))
+
+        if not len(li) > 0:
+            print("Parameter", parameterstring, dataid, coverage)
+            print("Did not find any data to display - aborting")
+            return
+        else:
+            valkeys = ['time']
+            valkeys = parameterstring.split(',')
+            for i,elem in enumerate(valkeys):
+                idx = KEYLIST.index(elem)
+                if elem == 'time':
+                    self.array[idx] = [datetime.strptime(el[0],"%Y-%m-%d %H:%M:%S.%f") for el in li]
+                else:
+                    self.array[idx] = [float(el[i]) for el in li]
+        """
+        self.datavars = {0: dataid, 1: parameter, 2: period, 3: pad, 4: currentdate, 5: unitlist, 6: coverage, 7: updatetime, 8: db}
+
+        self.figure.clear()
+        t1 = threading.Thread(target=self.timer, args=(1,self.t1_stop))
+        t1.start()
+        # Display the plot
+        self.canvas.draw()
+
+
     def startMARCOSMonitor(self,**kwargs):
         """
         DEFINITION:
             embbed matplotlib figure in canvas for mointoring
 
         PARAMETERS:
             kwargs:  - all plot args
@@ -1993,14 +2042,16 @@
             dipath = dipathlist[0]
             if os.path.isfile(dipath):
                 dipath = os.path.split(dipath)[0]
             self.options['dipathlist'] = [dipath]
             order=dlg.sheetorderTextCtrl.GetValue()
             double=dlg.sheetdoubleCheckBox.GetValue()
             scalevalue=dlg.sheetscaleCheckBox.GetValue()
+            self.options['double'] = 'True'
+            self.options['scalevalue'] = 'True'
             if not double:
                 self.options['double'] = 'False'
             if not scalevalue:
                 self.options['scalevalue'] = 'False'
             self.options['order'] = order
 
             saveini(self.options)
```

### Comparing `GeomagPy-v0.3.92/magpy/gui/metapage.py` & `GeomagPy-v0.3.93/magpy/gui/metapage.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/streampage.py` & `GeomagPy-v0.3.93/magpy/gui/streampage.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/absolutespage.py` & `GeomagPy-v0.3.93/magpy/gui/absolutespage.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/reportpage.py` & `GeomagPy-v0.3.93/magpy/gui/reportpage.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/analysispage.py` & `GeomagPy-v0.3.93/magpy/gui/analysispage.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/developpage.py` & `GeomagPy-v0.3.93/magpy/gui/developpage.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/magpy.png` & `GeomagPy-v0.3.93/magpy/gui/magpy.png`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/__init__.py` & `GeomagPy-v0.3.93/magpy/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/gui/dialogclasses.py` & `GeomagPy-v0.3.93/magpy/gui/dialogclasses.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/collector/collector-martas.py` & `GeomagPy-v0.3.93/magpy/collector/collector-martas.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/collector/collector-marcos.py` & `GeomagPy-v0.3.93/magpy/collector/collector-marcos.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/collector/subscribe2client.py` & `GeomagPy-v0.3.93/magpy/collector/subscribe2client.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/collector/subscribe2marcos.py` & `GeomagPy-v0.3.93/magpy/collector/subscribe2marcos.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/opt/analysismonitor.py` & `GeomagPy-v0.3.93/magpy/opt/analysismonitor.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/opt/cred.py` & `GeomagPy-v0.3.93/magpy/opt/cred.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/opt/stormdet.py` & `GeomagPy-v0.3.93/magpy/opt/stormdet.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/opt/Table.py` & `GeomagPy-v0.3.93/magpy/opt/Table.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/opt/mails.py` & `GeomagPy-v0.3.93/magpy/opt/mails.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/opt/emd.py` & `GeomagPy-v0.3.93/magpy/opt/emd.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/opt/sigfig.py` & `GeomagPy-v0.3.93/magpy/opt/sigfig.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/absolutes.py` & `GeomagPy-v0.3.93/magpy/absolutes.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_latex.py` & `GeomagPy-v0.3.93/magpy/lib/format_latex.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_gdas.py` & `GeomagPy-v0.3.93/magpy/lib/format_gdas.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_wdc.py` & `GeomagPy-v0.3.93/magpy/lib/format_wdc.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_rcs.py` & `GeomagPy-v0.3.93/magpy/lib/format_rcs.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_iono.py` & `GeomagPy-v0.3.93/magpy/lib/format_iono.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_neic.py` & `GeomagPy-v0.3.93/magpy/lib/format_neic.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_didd.py` & `GeomagPy-v0.3.93/magpy/lib/format_didd.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_autodif_fread.py` & `GeomagPy-v0.3.93/magpy/lib/format_autodif_fread.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_gsm19.py` & `GeomagPy-v0.3.93/magpy/lib/format_gsm19.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/magpy_formats.py` & `GeomagPy-v0.3.93/magpy/lib/magpy_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 DEPENDENCIES:
         magpy.lib...
                 .format_gsm19
                 .format_didd
                 .format_gdas
                 .format_lemi
                 .format_pos1
-                .format_env05
+                #.format_env05
                 .format_cr800
                 .format_iono
                 .format_iaga02
                 .format_wdc
                 .format_magpy
                 .format_noaa
                 .format_latex
@@ -40,29 +40,33 @@
         magpy.stream.read()
         magpy.stream.write()
 '''
 from __future__ import print_function
 
 from magpy.stream import *
 
+import logging
+logger = logging.getLogger(__name__)
+
 # IMPORT INSTRUMENT SPECIFIC DATA FORMATS:
 from magpy.lib.format_gsm19 import *
 from magpy.lib.format_didd import *
 from magpy.lib.format_gdas import *
 from magpy.lib.format_lemi import *
 from magpy.lib.format_pos1 import *
-from magpy.lib.format_env05 import *
+#from magpy.lib.format_env05 import *
 from magpy.lib.format_cr800 import *
 from magpy.lib.format_iono import *
 
 # IMPORT GENERAL PURPOSE FORMATS:
 from magpy.lib.format_iaga02 import *
 from magpy.lib.format_wdc import *
 from magpy.lib.format_magpy import *
 from magpy.lib.format_noaa import *
+from magpy.lib.format_nc import isNETCDF, readNETCDF
 from magpy.lib.format_latex import *
 from magpy.lib.format_json import *
 
 # IMPORT OBSERVATORY/GROUP SPECIFIC FORMATS:
 from magpy.lib.format_wik import *
 from magpy.lib.format_wic import *
 from magpy.lib.format_sfs import *
@@ -205,17 +209,17 @@
             pass
     elif (format_type == "AUTODIF_FREAD"): # Text AUTODIF F for baseline (0.2 Hz, from POS1)
         try:
             if (isAUTODIF_FREAD(filename)):
                 return True
         except:
             pass
-    elif (format_type == "ENV05"): # Binary Environmental data (1 Hz)
-        if (isENV05(filename)):
-            return True
+    #elif (format_type == "ENV05"): # Binary Environmental data (1 Hz)
+    #    if (isENV05(filename)):
+    #        return True
     elif (format_type == "SFDMI"): # San Fernando DMI(FGE) format
         if (isSFDMI(filename)):
             return True
     elif (format_type == "SFGSM"): # San Fernando GSM format
         if (isSFGSM(filename)):
             return True
     elif (format_type == "BDV1"): # Budkov format
@@ -223,26 +227,29 @@
             return True
     elif (format_type == "GFZKP"): # GFZ Kp
         if (isGFZKP(filename)):
             return True
     elif (format_type == "NOAAACE"): # NOAA ACE Satellite data
         if (isNOAAACE(filename)):
             return True
+    elif (format_type == "NETCDF"): # NetCDF format, NOAA DSCOVR satellite data
+        if (isNETCDF(filename)):
+            return True
     elif (format_type == "NEIC"): # NEIC USGS data
         if (isNEIC(filename)):
             return True
     elif (format_type == "USBLOG"): # Data from the USB temperature logger
         if (isUSBLOG(filename)):
             return True
     elif (format_type in ["PYNC", "AUTODIF", "SERMUL", "SERSIN", "LATEX"]): # Not yet supported
         return False
     elif (format_type == "UNKOWN"): # Unkown
         return False
     else:
-        print ("Could not identify data format", filename,format_type)
+        logger.warning("isFormat: Could not identify data format for file {}. Is {} a valid type?".format(filename, format_type))
         return False
 
 
 def readFormat(filename, format_type, headonly=False, **kwargs):
     empty = DataStream()
     if (format_type == "IAGA"):
         return readIAGA(filename, headonly, **kwargs)
@@ -294,16 +301,16 @@
         return readLEMIBIN1(filename, headonly, **kwargs)
     elif (format_type == "POS1"):
         return readPOS1(filename, headonly, **kwargs)
     elif (format_type == "POS1TXT"):
         return readPOS1TXT(filename, headonly, **kwargs)
     elif (format_type == "AUTODIF_FREAD"):
         return readAUTODIF_FREAD(filename, headonly, **kwargs)
-    elif (format_type == "ENV05"):
-        return readENV05(filename, headonly, **kwargs)
+    #elif (format_type == "ENV05"):
+    #    return readENV05(filename, headonly, **kwargs)
     elif (format_type == "USBLOG"):
         return readUSBLOG(filename, headonly, **kwargs)
     elif (format_type == "GRAVSG"):
         return readGRAVSG(filename, headonly, **kwargs)
     elif (format_type == "IWT"):
         return readIWT(filename, headonly, **kwargs)
     elif (format_type == "LIPPGRAV"):
@@ -331,17 +338,20 @@
         return readSFGSM(filename, headonly, **kwargs)
     elif (format_type == "BDV1"):
         return readBDV1(filename, headonly, **kwargs)
     elif (format_type == "GFZKP"):
         return readGFZKP(filename, headonly, **kwargs)
     elif (format_type == "NOAAACE"):
         return readNOAAACE(filename, headonly, **kwargs)
+    elif (format_type == "NETCDF"):
+        return readNETCDF(filename, headonly, **kwargs)
     elif (format_type == "NEIC"):
         return readNEIC(filename, headonly, **kwargs)
     else:
+        logger.info("No valid format found ({}). Returning empty stream.".format(format_type))
         return DataStream(empty,empty.header)
 
 
 def writeFormat(datastream, filename, format_type, **kwargs):
     """
     calls the format specific write functions
     if the selceted dir is not existing, it is created
@@ -376,9 +386,8 @@
     elif (format_type == "AUTODIF_FREAD"):
         return writeAUTODIF_FREAD(datastream, filename, **kwargs)
     elif (format_type == "CR800"):
         return writeCR800(datastream, filename, **kwargs)
     elif (format_type == "LATEX"):
         return writeLATEX(datastream, filename, **kwargs)
     else:
-        print("magpy-formats: Writing not succesful - format not recognized")
-        logging.warning("magpy-formats: Writing not succesful - format not recognized")
+        logging.warning("writeFormat: Writing not succesful - format not recognized")
```

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_gfz.py` & `GeomagPy-v0.3.93/magpy/lib/format_gfz.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_sfs.py` & `GeomagPy-v0.3.93/magpy/lib/format_sfs.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_json.py` & `GeomagPy-v0.3.93/magpy/lib/format_json.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 def readJSON(filename, headonly=False, **kwargs):
     """
     Reading JSON format data.
     """
     stream = DataStream()
+    header = {}
     array = [[] for key in KEYLIST]
 
     with open(filename, 'r') as jsonfile:
         dataset = json.load(jsonfile)
         loggerlib.info('Read: %s, Format: %s ' % (filename, "JSON"))
         
         fillkeys = ['var1', 'var2', 'var3', 'var4', 'var5', 'x', 'y', 'z', 'f']
@@ -72,16 +73,16 @@
                     
             if 'time' in key:
                 data = [date2num(testTimeString(str(x[i]))) for x in dataset[1:]]
             else:
 
                 data = [np.nan if x[i] is None else float(x[i]) for x in dataset[1:]]
             array[KEYLIST.index(keydict[i])] = data
-            stream.header['col-'+keydict[i]] = key
-            stream.header['unit-col-'+keydict[i]] = ''
+            header['col-'+keydict[i]] = key
+            header['unit-col-'+keydict[i]] = ''
                 
     for idx, elem in enumerate(array):
         array[idx] = np.asarray(array[idx])
 
-    stream = DataStream([],stream.header,np.asarray(array))
+    stream = DataStream([],header,np.asarray(array))
 
     return stream
```

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_lemi.py` & `GeomagPy-v0.3.93/magpy/lib/format_lemi.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_wic.py` & `GeomagPy-v0.3.93/magpy/lib/format_wic.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_bdv.py` & `GeomagPy-v0.3.93/magpy/lib/format_bdv.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_imf.py` & `GeomagPy-v0.3.93/magpy/lib/format_imf.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from __future__ import unicode_literals
 from __future__ import absolute_import
 from __future__ import division
 from io import open
 
 from magpy.stream import *
 
+import logging
+logger = logging.getLogger(__name__)
+
 def isIMF(filename):
     """
     Checks whether a file is ASCII IMF 1.22,1.23 minute format.
     """
     try:
         temp = open(filename, 'rt').readline()
     except:
@@ -32,15 +35,15 @@
         if temp[3] == ' ' and temp[11] == ' ' and temp[29] == ' ' and temp[45] == ' ' and temp[46] == 'R':
             pass
         else:
             return False
     except:
         return False
 
-    print("Found IMF data")
+    logger.debug("isIMF: Found IMF data")
     return True
 
 
 def isIMAGCDF(filename):
     """
     Checks whether a file is ImagCDF format.
     """
@@ -50,14 +53,16 @@
         return False
     try:
         form = temp.attrs['FormatDescription']
         if not form[0].startswith('INTERMAGNET'):
             return False
     except:
         return False
+    
+    logger.debug("isIMAGCDF: Found INTERMAGNET CDF data")
     return True
 
 
 def isIAF(filename):
     """
     Checks whether a file is BIN IAF INTERMAGNET Archive format.
     """
@@ -106,14 +111,16 @@
     #        return False
     #    if temp1[3] == ' ' and temp1[11] == ' ' and temp1[29] == ' ' and temp1[45] == ' ' and temp1[46] == 'R':
     #        pass
     #    else:
     #        return False
     #except:
     #    return False
+    
+    logger.debug("isBLV: Found BLV data")
     return True
 
 
 def isIYFV(filename):
     """
     Checks whether a file is ASCII IYFV 1.01 yearly mean format.
 
@@ -123,14 +130,15 @@
         temp = open(filename, 'rt').readline()
     except:
         return False
     try:
         searchstr = ['ANNUAL MEAN VALUES', 'Annual Mean Values', 'annual mean values']
         for elem in searchstr:
             if temp.find(elem) > 0:
+                logger.debug("isIYFV: Found IYFV data")
                 return True
     except:
         return False
     return False
 
 
 def isDKA(filename):
@@ -160,14 +168,15 @@
             if temp2.find(elem) > 0:
                 ok = True
         if not ok:
             return False
         searchstr = ['K-index values', 'K-INDEX VALUES']
         for elem in searchstr:
             if temp5.find(elem) > 0:
+                logger.debug("isDKA: Found DKA data")
                 return True
     except:
         return False
     return False
 
 
 def readIAF(filename, headonly=False, **kwargs):
@@ -351,15 +360,15 @@
     elif resolution in ['hour','hours','Hour','Hours','HOUR','HOURS']:
         ndarray = data2array([xho,yho,zho,fho],keystr.split(','),min(datelist)+timedelta(minutes=30),sr=3600)
         headers['DataSamplingRate'] = '3600 sec'
     elif resolution in ['k','K']:
         ndarray = data2array([k,ir],['var1','var2'],min(datelist)+timedelta(minutes=90),sr=10800)
         headers['DataSamplingRate'] = '10800 sec'
     else:
-        print (keystr, min(datelist))
+        logger.debug("Key and minimum: {} {}".format(keystr, min(datelist)))
         ndarray = data2array([x,y,z,f],keystr.split(','),min(datelist),sr=60)
         headers['DataSamplingRate'] = '60 sec'
 
     stream = DataStream([LineStruct()], headers, ndarray)
     #if 'df' in keystr:
     #    stream = stream.f_from_df()
 
@@ -374,35 +383,35 @@
     kvals = kwargs.get('kvals')
     mode = kwargs.get('mode')
     debug = kwargs.get('debug')
 
     df=False
     # Check whether data is present at all
     if not len(datastream.ndarray[0]) > 0:
-        print("writeIAF: No data found - check ndarray")
+        logger.error("writeIAF: No data found - check ndarray")
         return False
     # Check whether minute file
     sr = datastream.samplingrate()
     if not int(sr) == 60:
-        print("writeIAF: Minute data needs to be provided")
+        logger.error("writeIAF: Minute data needs to be provided")
         return False
     # check whether data covers one month
     tdiff = int(np.round(datastream.ndarray[0][-1]-datastream.ndarray[0][0]))
     if not tdiff >= 28:
-        print("writeIAF: Data needs to cover one month")
+        logger.error("writeIAF: Data needs to cover one month")
         return False
 
     try:
         # Convert data to XYZ if HDZ
         if not datastream.header.get('DataComponents','').startswith('XYZ'):
-            print ("Data contains: {}".format(datastream.header.get('DataComponents','')))
+            logger.indo("Data contains: {}".format(datastream.header.get('DataComponents','')))
         if datastream.header['DataComponents'].startswith('HDZ'):
             datastream = datastream.hdz2xyz()
     except:
-        print("writeIAF: HeaderInfo on DataComponents seems to be missing")
+        logger.error("writeIAF: HeaderInfo on DataComponents seems to be missing")
         return False
 
     dsf = datastream.header.get('DataSamplingFilter','')
 
     # Check whether f is contained (or delta f)
     # if f calc delta f
     dfpos = KEYLIST.index('df')
@@ -454,15 +463,15 @@
     tmpstream = datastream.copy()
     hourvals = tmpstream.filter(filter_width=timedelta(minutes=60), resampleoffset=timedelta(minutes=30), filter_type='flat',missingdata='mean')
     hourvals = hourvals.get_gaps()
 
     for i in range(tdiff):
         dayar = datastream._select_timerange(starttime=t0+i,endtime=t0+i+1)
         if not len(dayar[0]) == 1440:
-            print ("format_IMF: found {} datapoints (expected are 1440) - assuming last value(s) to represent next month".format(len(dayar[0])))
+            logger.info("format_IMF: found {} datapoints (expected are 1440) - assuming last value(s) to represent next month".format(len(dayar[0])))
             dayar = np.asarray([elem[:1440] for elem in dayar])
         # get all indicies
         #minutest = DataStream([LineStruct],datastream.header,dayar)
         #temp = minutest.copy() ### Necessary so that dayar is not modified by the filtering process
         #temp = temp.filter(filter_width=timedelta(minutes=60), resampleoffset=timedelta(minutes=30), filter_type='flat')
         tempvals = hourvals._select_timerange(starttime=t0+i,endtime=t0+i+1)
         temp = DataStream([LineStruct],datastream.header,tempvals)
@@ -477,15 +486,15 @@
                     if value == '':
                         misslist.append(elem)
                 elif elem == 'StartDate':
                     
                     value = int(datetime.strftime(num2date(dayar[0][0]),'%Y%j'))
                 elif elem == 'DataAcquisitionLatitude':
                     if not float(datastream.header.get('DataAcquisitionLatitude',0)) < 90 and float(datastream.header.get('DataAcquisitionLatitude','')) > -90:
-                        print("Latitude and Longitude need to be provided in Degree")
+                        print("Latitude and Longitude need to be provided in degrees")
                         x=1/0
                     value = int(np.round((90-float(datastream.header.get('DataAcquisitionLatitude',0)))*1000))
                     if value == 0:
                         misslist.append(elem)
                 elif elem == 'DataAcquisitionLongitude':
                     value = int(np.round(float(datastream.header.get('DataAcquisitionLongitude',0))*1000))
                     if value == 0:
@@ -518,15 +527,15 @@
                 elif elem == 'DataDigitalSampling':
                     try:
                         value = int(datastream.header.get('DataDigitalSampling',0)*1000)
                         if value == 0:
                             misslist.append(elem)
                     except:
                         value = datastream.header.get('DataDigitalSampling','')
-                        print ("writeIAF: DataDigitialSampling info needs to be integer")
+                        print ("writeIAF: DataDigitialSampling info needs to be an integer")
                         print ("          - extracting integers from provided string")
                         valtmp = re.findall(r'\d+', value)
                         value = int(valtmp[-1])*1000
                         print ("          extracted: {}".format(value))
                 elif elem == 'Reserved':
                     value = 0
                 else:
@@ -681,15 +690,15 @@
         station=datastream.header['StationIAGAcode']
         k9=datastream.header['StationK9']
         lat=np.round(float(datastream.header.get('DataAcquisitionLatitude')),3)
         lon=np.round(float(datastream.header.get('DataAcquisitionLongitude')),3)
         year=str(int(datetime.strftime(num2date(datastream.ndarray[0][1]),'%y')))
         ye=str(int(datetime.strftime(num2date(datastream.ndarray[0][1]),'%Y')))
         kfile = os.path.join(path[0],station.upper()+year+'K.DKA')
-        print("Writing k summary file:", kfile)
+        logger.info("Writing k summary file: {}".format(kfile))
         head = []
         if not os.path.isfile(kfile):
             head.append("{0:^66}".format(station.upper()))
             head2 = '                  Geographical latitude: {:>10.3f} N'.format(lat)
             head3 = '                  Geographical longitude:{:>10.3f} E'.format(lon)
             head4 = '            K-index values for {0}     (K9-limit = {1:>4} nT)'.format(ye, k9)
             head5 = '  DA-MON-YR  DAY #    1    2    3    4      5    6    7    8       SK'
@@ -707,42 +716,41 @@
                 #print elem
         # write data
         with open(kfile, "a") as myfile:
             for elem in kstr:
                 myfile.write(elem+'\r\n')
                 #print elem
 
-    print("Writing monthly IAF data format:", path[1].upper())
+    logger.info("Writing monthly IAF data format to {}".format(path[1].upper()))
     if os.path.isfile(filename):
         if mode == 'append':
             with open(filename, "a") as myfile:
                 myfile.write(output)
         else: # overwrite mode
             os.remove(filename)
             myfile = open(filename, "wb")
             myfile.write(output)
             myfile.close()
     else:
         myfile = open(filename, "wb")
         myfile.write(output)
         myfile.close()
 
-    print("Creating README from header info:", path[1].upper())
+    logger.info("Creating README from header info in {}".format(path[1].upper()))
     readme = True
     if readme:
         requiredhead = ['StationName','StationInstitution', 'StationStreet','StationCity','StationPostalCode','StationCountry','StationWebInfo', 'StationEmail','StationK9']
         acklist = ['StationName','StationInstitution', 'StationStreet','StationCity','StationPostalCode','StationCountry','StationWebInfo' ]
         conlist = ['StationName','StationInstitution', 'StationStreet','StationCity','StationPostalCode','StationCountry', 'StationEmail']
 
         for h in requiredhead:
             try:
                 test = datastream.header[h]
             except:
-                print ("README file could not be generated")
-                print ("Info on {0} is missing".format(h))
+                logger.error("README file could not be generated. Info on {0} is missing".format(h))
                 return True
         ack = []
         contact = []
         for a in acklist:
             try:
                 ack.append("               {0}".format(datastream.header[a]))
             except:
@@ -758,15 +766,15 @@
         stationname = datastream.header['StationName']
         k9=datastream.header['StationK9']
         lat=np.round(float(datastream.header.get('DataAcquisitionLatitude')),3)
         lon=np.round(float(datastream.header.get('DataAcquisitionLongitude')),3)
         ye=str(int(datetime.strftime(num2date(datastream.ndarray[0][1]),'%Y')))
         rfile = os.path.join(path[0],"README."+station.upper())
         head = []
-        print("Writing README file:", rfile)
+        logger.info("Writing README file: {}".format(rfile))
 
         dummy = "please insert manually"
         if not os.path.isfile(rfile):
             emptyline = ''
             head.append("{0:^66}".format(station.upper()))
             head.append("{0:<50}".format(emptyline))
             head.append("{0:>23} OBSERVATORY INFOMATION {1:>5}".format(stationname.upper(), ye))
@@ -812,15 +820,15 @@
 
 
 def readIMAGCDF(filename, headonly=False, **kwargs):
     """
     Reading Intermagnet CDF format (1.0,1.1,1.2)
     """
 
-    print("FOUND IMAGCDF")
+    logger.info("readIMAGCDF: FOUND IMAGCDF file")
 
     cdfdat = cdf.CDF(filename)
     # get Attribute list
     attrslist = [att for att in cdfdat.attrs]
     # get Data list
     datalist = [att for att in cdfdat]
     headers={}
@@ -915,28 +923,28 @@
         #print "No time column identified"
         # Check for starttime and sampling rate in header
         if 'StartTime' in attrslist and 'SamplingPeriod' in attrslist:
             # TODO Write that function
             st = str(cdfdat.attrs['StartTime'])
             sr = str(cdfdat.attrs['SamplingPeriod'])
         else:
-            print("readIMAGCDF: No Time information available - aborting")
+            logger.error("readIMAGCDF: No Time information available - aborting")
             return
     elif len(tllist) > 1:
         tl = [el[0] for el in tllist]
         if not max(tl) == min(tl):
-            print("readIMAGCDF: Time columns of different length. Choosing longest as basis")
+            logger.warning("readIMAGCDF: Time columns of different length. Choosing longest as basis")
             newdatalist.append(['time',max(tllist)[1]])
             try:
                 indexarray = np.nonzero(np.in1d(date2num(cdfdat[max(tllist)[1]][...]),date2num(cdfdat[min(tllist)[1]][...])))[0]
             except:
                 indexarray = np.asarray([])
             mutipletimerange = True
         else:
-            print("readIMAGCDF: Equal length time axes found - assuming identical time")
+            logger.info("readIMAGCDF: Equal length time axes found - assuming identical time")
             if 'GeomagneticVectorTimes' in datalist:
                 newdatalist.append(['time','GeomagneticVectorTimes'])
             else:
                 newdatalist.append(['time',tllist[0][1]]) # Take the first one
     else:
         #print "Single time axis found in file"
         newdatalist.append(['time',tllist[0][1]])
@@ -948,18 +956,18 @@
                 flaglisttmp = []
                 for elem in flagcolsconrad:
                     flaglisttmp.append(cdfdat[elem][...])
                 flaglist = np.transpose(flaglisttmp)
                 flaglist = [list(elem) for elem in flaglist]
                 return list(flaglist)
         else:
-            print ("readIMAGCDF: Could  not interprete Ruleset")
+            logger.warning("readIMAGCDF: Could  not interprete Ruleset")
 
     if not flagruletype == '':
-        print ("readIMAGCDF: Found flagging ruleset {} vers.{} - extracting flagging information".format(flagruletype,flagruleversion))
+        logger.info("readIMAGCDF: Found flagging ruleset {} vers.{} - extracting flagging information".format(flagruletype,flagruleversion))
         flagginglist = [elem for elem in datalist if elem.startswith('Flag')]
         flaglist = Ruleset2Flaglist(flagginglist,flagruletype,flagruleversion)
 
     datalist = [elem for elem in datalist if not elem.endswith('Times') and not elem.startswith('Flag')]
 
     # #########################################################
     # 2. Sort the datalist according to KEYLIST
@@ -979,15 +987,15 @@
                 label = cdfdat[elem].attrs['LABLAXIS'].lower()
                 if label in possvals:
                     newdatalist.append([key,elem])
             except:
                 pass # for lines which have no Label
 
     if not len(datalist) == len(newdatalist)-1:
-        print("readIMAGCDF: error encountered in key assignment - please check")
+        logger.warning("readIMAGCDF: error encountered in key assignment - please check")
 
     # 3. Create equal length array reducing all data to primary Times and filling nans for non-exist
     # (4. eventually completely drop time cols and just store start date and sampling period in header)
     # Deal with scalar data (independent or whatever
 
     for elem in newdatalist:
         #print ("Here", elem)
@@ -1037,15 +1045,15 @@
 
 def writeIMAGCDF(datastream, filename, **kwargs):
     """
     Writing Intermagnet CDF format (currently: vers1.2) + optional flagging info
     
     """
 
-    print("Writing IMAGCDF Format", filename)
+    logger.info("Writing IMAGCDF Format", filename)
     mode = kwargs.get('mode')
     addflags = kwargs.get('addflags')
     skipcompression = kwargs.get('skipcompression')
 
     cdf.lib.set_backward(False) ## necessary for time_tt2000 support
 
     testname = str(filename+'.cdf')
@@ -1307,29 +1315,29 @@
             if ndarray and len(datastream.ndarray[ind])>0:
                 col = datastream.ndarray[ind]
             else:
                 col = datastream._get_column(key)
             col = col.astype(float)
 
             if not False in checkEqual3(col):
-                print("Found identical values only:", key)
+                logger.warning("Found identical values only for {}".format(key))
                 col = col[:1]
             if key == 'time':
                 key = 'GeomagneticVectorTimes'
                 try: ## requires spacepy >= 1.5
                     mycdf.new(key, type=cdf.const.CDF_TIME_TT2000)
                     mycdf[key] = cdf.lib.v_datetime_to_tt2000(np.asarray([num2date(elem).replace(tzinfo=None) for elem in col]))
                     #print("writeIMAGCDF: Datetimes successfully converted to TT2000")
                     if useScalarTimes:
                         key = 'GeomagneticScalarTimes'
                         mycdf.new(key, type=cdf.const.CDF_TIME_TT2000)
                         if len(naninds) > 0:
-                            print ("{}: removing nan values from scalar times".format(datetime.utcnow()))
+                            logger.info("writeIMAGCDF: ({}) removing nan values from scalar times".format(datetime.utcnow()))
                             mycdf[key] = np.delete(mycdf['GeomagneticVectorTimes'], naninds)
-                            print ("{}: done".format(datetime.utcnow()))
+                            logger.info("writeIMAGCDF: ({}) finished".format(datetime.utcnow()))
                         else:
                             mycdf[key] = mycdf['GeomagneticVectorTimes']
                 except:
                     mycdf[key] = np.asarray([num2date(elem).replace(tzinfo=None) for elem in col])
             elif len(col) > 0:
                 #if len(col) > 1000000:
                 #    print ("Starting with {}".format(key))
@@ -1416,66 +1424,66 @@
                                     unit = headers.get('unit-col-'+key,'')
                                 mycdf[cdfkey].attrs['UNITS'] = unit
                             except:
                                 pass
             success = True
 
     if len(flaglist) > 0 and addflags == True:
-            flagstart = 'FlagBeginTimes'
-            flagend = 'FlagEndTimes'
-            flagcomponents = 'FlagComponents'
-            flagcode = 'FlagCode'
-            flagcomment = 'FlagDescription'
-            flagmodification = 'FlagModificationTimes'
-            flagsystemreference = 'FlagSystemReference'
-            flagobserver = 'FlagObserver'
-
-            trfl = np.transpose(flaglist)
-            #print ("Transposed flaglist", trfl)
-            ok =True
-            if ok:
-            #try:
-                mycdf.new(flagstart, type=cdf.const.CDF_TIME_TT2000)
-                mycdf[flagstart] = cdf.lib.v_datetime_to_tt2000(trfl[0])
-                mycdf.new(flagend, type=cdf.const.CDF_TIME_TT2000)
-                mycdf[flagend] = cdf.lib.v_datetime_to_tt2000(trfl[1])
-                mycdf.new(flagmodification, type=cdf.const.CDF_TIME_TT2000)
-                mycdf[flagmodification] = cdf.lib.v_datetime_to_tt2000(trfl[-1])
-
-                # Here we can select between different content
-                if len(flaglist[0]) == 7:
-                    #[st,et,key,flagnumber,commentarray[idx],sensorid,now]
-                    # eventually change flagcomponent in the future
-                    fllist = [flagcomponents,flagcode,flagcomment, flagsystemreference] # , flagobserver]
-                elif len(flaglist[0]) == 8:  
-                    # Future version ??
-                    fllist = [flagcomponents,flagcode,flagcomment, flagsystemreference, flagobserver]
-                for idx, cdfkey in enumerate(fllist):
-                    if not cdfkey == flagcode:
-                        ll = [el.encode('UTF8') for el in trfl[idx+2]]
-                    else:
-                        ll = trfl[idx+2]
-                    mycdf[cdfkey] = ll
-                    mycdf[cdfkey].attrs['DEPEND_0'] = "FlagBeginTimes"
-                    mycdf[cdfkey].attrs['DISPLAY_TYPE'] = "time_series"
-                    mycdf[cdfkey].attrs['LABLAXIS'] = cdfkey.strip('Flag')
-                    mycdf[cdfkey].attrs['FILLVAL'] = np.nan
-                    mycdf[cdfkey].attrs['FIELDNAM'] = cdfkey
-                    if cdfkey in ['flagcode']:
-                        mycdf[cdfkey].attrs['VALIDMIN'] = 0
-                        mycdf[cdfkey].attrs['VALIDMAX'] = 9
-            #except:
-            #    print ("writeIMAGCDF: error when adding flags. skipping this part")
-            print ("writeIMAGCDF: Flagging information added to file")
+        flagstart = 'FlagBeginTimes'
+        flagend = 'FlagEndTimes'
+        flagcomponents = 'FlagComponents'
+        flagcode = 'FlagCode'
+        flagcomment = 'FlagDescription'
+        flagmodification = 'FlagModificationTimes'
+        flagsystemreference = 'FlagSystemReference'
+        flagobserver = 'FlagObserver'
+
+        trfl = np.transpose(flaglist)
+        #print ("Transposed flaglist", trfl)
+        ok =True
+        if ok:
+        #try:
+            mycdf.new(flagstart, type=cdf.const.CDF_TIME_TT2000)
+            mycdf[flagstart] = cdf.lib.v_datetime_to_tt2000(trfl[0])
+            mycdf.new(flagend, type=cdf.const.CDF_TIME_TT2000)
+            mycdf[flagend] = cdf.lib.v_datetime_to_tt2000(trfl[1])
+            mycdf.new(flagmodification, type=cdf.const.CDF_TIME_TT2000)
+            mycdf[flagmodification] = cdf.lib.v_datetime_to_tt2000(trfl[-1])
+
+            # Here we can select between different content
+            if len(flaglist[0]) == 7:
+                #[st,et,key,flagnumber,commentarray[idx],sensorid,now]
+                # eventually change flagcomponent in the future
+                fllist = [flagcomponents,flagcode,flagcomment, flagsystemreference] # , flagobserver]
+            elif len(flaglist[0]) == 8:  
+                # Future version ??
+                fllist = [flagcomponents,flagcode,flagcomment, flagsystemreference, flagobserver]
+            for idx, cdfkey in enumerate(fllist):
+                if not cdfkey == flagcode:
+                    ll = [el.encode('UTF8') for el in trfl[idx+2]]
+                else:
+                    ll = trfl[idx+2]
+                mycdf[cdfkey] = ll
+                mycdf[cdfkey].attrs['DEPEND_0'] = "FlagBeginTimes"
+                mycdf[cdfkey].attrs['DISPLAY_TYPE'] = "time_series"
+                mycdf[cdfkey].attrs['LABLAXIS'] = cdfkey.strip('Flag')
+                mycdf[cdfkey].attrs['FILLVAL'] = np.nan
+                mycdf[cdfkey].attrs['FIELDNAM'] = cdfkey
+                if cdfkey in ['flagcode']:
+                    mycdf[cdfkey].attrs['VALIDMIN'] = 0
+                    mycdf[cdfkey].attrs['VALIDMAX'] = 9
+        #except:
+        #    print ("writeIMAGCDF: error when adding flags. skipping this part")
+        logger.info("writeIMAGCDF: Flagging information added to file")
 
     if not skipcompression:
         try:
             mycdf.compress(cdf.const.GZIP_COMPRESSION, 5)
         except:
-            print ("writeIMAGCDF: Compression failed for unknown reason - storing uncompresed data")
+            logger.warning("writeIMAGCDF: Compression failed for unknown reason - storing uncompresed data")
             pass
     mycdf.close()
     return success
 
 
 def readIMF(filename, headonly=False, **kwargs):
     """
@@ -1601,15 +1609,15 @@
     version = kwargs.get('version')
     gin = kwargs.get('gin')
     datatype = kwargs.get('datatype')
 
     success = False
     # 1. check whether datastream corresponds to minute file
     if not 0.9 < datastream.get_sampling_period()*60*24 < 1.1:
-        print ("format-imf: Data needs to be minute data for Intermagent - filter it accordingly")
+        logger.error("writeIMF: Data needs to be minute data for Intermagnet - filter it accordingly")
         return False
 
     # 2. check whether file exists and according to mode either create, append, replace
     if os.path.isfile(filename):
         if mode == 'skip': # skip existing inputs
             exst = read(path_or_url=filename)
             datastream = joinStreams(exst,datastream)
@@ -1631,29 +1639,29 @@
     if not gin:
         gin = 'EDI'
     if not datatype:
         datatype = 'R' # reported; can also be 'A', 'Q', 'D'
     try:
         idc = header['StationID']
     except:
-        print ("format-imf: No station code specified. Setting to XYZ ...")
+        logger.warning("writeIMF: No station code specified. Setting to XYZ ...")
         idc = 'XYZ'
         #return False
     try:
         colat = 90 - float(header['DataAcquisitionLatitude'])
         longi = float(header['DataAcquisitionLongitude'])
     except:
-        print ("format-imf: No location specified. Setting 99,999 ...")
+        logger.warning("writeIMF: No location specified. Setting 99,999 ...")
         colat = 99.9
         longi = 999.9
         #return False
     try:
         decbas = float(header['DataSensorAzimuth'])
     except:
-        print ("format-imf: No orientation angle specified. Setting 999.9 ...")
+        logger.warning("writeIMF: No orientation angle specified. Setting 999.9 ...")
         decbas = 999.9
         #return False
 
     # 4. Data
     dataline,blockline = '',''
     minuteprev = 0
 
@@ -1672,24 +1680,24 @@
     xlen = len(datastream.ndarray[KEYLIST.index('x')])
     ylen = len(datastream.ndarray[KEYLIST.index('y')])
     zlen = len(datastream.ndarray[KEYLIST.index('z')])
     flen = len(datastream.ndarray[KEYLIST.index('f')])
     dflen = len(datastream.ndarray[KEYLIST.index('df')])
 
     if not xlen > 0 or not ylen > 0 or not zlen > 0:
-        print ("writeIMF: vector data seems to be missing or incomplete - aborting")
+        logger.error("writeIMF: vector data seems to be missing or incomplete - aborting")
         return False
  
     if not flen > 0 and not dflen > 0:
-        print ("writeIMF: required information on f is missing - aborting")
+        logger.error("writeIMF: required information on f is missing - aborting")
         return False
 
     if not flen > 0 and dflen > 0:
-        print ("writeIMF: delta F provided, but no F values")
-        print ("writeIMF: calcualting F ...")
+        logger.warning("writeIMF: delta F provided, but no F values")
+        logger.warning("writeIMF: calcualting F ...")
         datastream = datastream.calc_f()
 
     flen = len(datastream.ndarray[KEYLIST.index('f')])
 
     xind = KEYLIST.index('x')
     yind = KEYLIST.index('y')
     zind = KEYLIST.index('z')
@@ -1878,15 +1886,15 @@
                     else:
                         array[2].append(float(block[2]))
                     array[3].append(float(block[3]))
                 #print block
             elif line.startswith('*'):  # comment block startsnow
                 # data info
                 starfound.append('*')
-                print ("Found comment section", starfound)
+                logger.debug("Found comment section", starfound)
                 block = line.split()
                 #print block
             else:
                 pass
     fh.close()
 
     array = [np.asarray(el) for el in array]
@@ -1937,15 +1945,15 @@
         t2 = date2num(datetime.strptime(str(int(year)+1)+'-01-01','%Y-%m-%d'))
 
     absinfoline = []
     if diff:
         if diff.length()[0] > 1:
             absinfo = diff.header.get('DataAbsInfo','')
             if not absinfo == '':
-                print("writeBLV: Getting Absolute info from header of provided dailymean file") 
+                logger.info("writeBLV: Getting Absolute info from header of provided dailymean file") 
                 absinfoline = absinfo.split('_')
                 extradays= int(absinfoline[2])
                 fitfunc = absinfoline[3]
                 fitdegree = int(absinfoline[4])
                 knotstep = float(absinfoline[5])
                 keys = ['dx','dy','dz']#,'df'] # absinfoline[6]
 
@@ -1974,26 +1982,26 @@
             myFile= open( filename, "ab" )
         else: # overwrite mode
             #os.remove(filename)  ?? necessary ??
             myFile= open( filename, "wb" )
     else:
         myFile= open( filename, "wb" )
 
-    print("writeBLV: file:", filename)
+    logger.info("writeBLV: file:", filename)
 
     # 3. check whether datastream corresponds to an absolute file and remove unreasonable inputs
     #     - check whether F measurements were performed at the main pier - delta F's are available
 
     try:
         if not datastream.header['DataFormat'] == 'MagPyDI':
-            print("writeBLV: Format not recognized - needs to be MagPyDI")
+            logger.error("writeBLV: Format not recognized - needs to be MagPyDI")
             return False
     except:
-        print("writeBLV: Format not recognized - should be MagPyDI")
-        print("writeBLV: is not yet assigned during database access")
+        logger.error("writeBLV: Format not recognized - should be MagPyDI")
+        logger.error("writeBLV: is not yet assigned during database access")
         #return False
 
     indf = KEYLIST.index('df')
     if len([elem for elem in datastream.ndarray[indf] if not np.isnan(float(elem))]) > 0:
         keys = ['dx','dy','dz','df']
     else:
         if not deltaF:
@@ -2089,27 +2097,26 @@
     #print "Mean df", meandf, mean(dfl)
 
     # 7. Get essential header info
     header = datastream.header
     try:
         idc = header['StationID']
     except:
-        print("formatBLV: No station code specified. Aborting ...")
         logging.error("formatBLV: No station code specified. Aborting ...")
         return False
     headerline = '%s %5.f %5.f %s %s' % (comps.upper(),meanh,meanf,idc,year)
     myFile.writelines( headerline+'\r\n'.encode('utf-8') )
 
     #print "writeBLV:", headerline
 
     # 8. Basevalues
     if len(datastream.ndarray[0]) > 0:
-        print ("writeBLV:", datastream.ndarray[indFtype])
-        print ("writeBLV:", datastream.ndarray)
-        print ("writeBLV:", datastream.length())
+        logger.debug("writeBLV: {}".format(datastream.ndarray[indFtype]))
+        logger.debug("writeBLV: {}".format(datastream.ndarray))
+        logger.debug("writeBLV: {}".format(datastream.length()))
         for idx, elem in enumerate(datastream.ndarray[0]):
             if t2 >= elem >= t1:
                 day = datetime.strftime(num2date(elem),'%j')
                 x = float(datastream.ndarray[indx][idx])
                 y = float(datastream.ndarray[indy][idx])*60.
                 z = float(datastream.ndarray[indz][idx])
                 df = float(datastream.ndarray[indf][idx])
@@ -2201,15 +2208,15 @@
         line = '%s %9.2f %9.2f %9.2f %9.2f %7.2f %s\r\n' % (day,x,y,z,f,df,parameter)
         myFile.writelines( line.encode('utf-8') )
 
     # 9. comments
     myFile.writelines( '*\r\n'.encode('utf-8') )
     myFile.writelines( 'Comments:\r\n'.encode('utf-8') )
     absinfoline = dummystream.header.get('DataAbsInfo','').split('_')
-    print ("Infoline", absinfoline)
+    logger.info("Infoline {}".format(absinfoline))
     funcline1 = 'Baselinefunction: %s\r\n' % absinfoline[3]
     funcline2 = 'Degree: %s, Knots: %s\r\n' % (absinfoline[4],absinfoline[5])
     funcline3 = 'For adopted values the fit has been applied between\r\n'
     funcline4 = '%s and %s\r\n' % (str(num2date(float(absinfoline[0])).replace(tzinfo=None)),str(num2date(float(absinfoline[1])).replace(tzinfo=None)))
     # get some data:
     infolist = [] # contains all provided information for comment section
     db = False
@@ -2325,15 +2332,15 @@
                 if not headonly:
                     # get data
                     data = line.split()
                     test = True
                     if test:
                         #try:
                         if not len(data) >= 12:
-                            print("readIYFV: inconsistency of file format - ", len(data))
+                            logger.warning("readIYFV: inconsistency of file format - ", len(data))
                         ye = data[0].split('.')
                         dat = ye[0]+'-06-01'
                         row = []
                         ti = date2num(datetime.strptime(dat,"%Y-%m-%d"))
                         row.append(dms2d(data[1]+':'+data[2]))
                         row.append(dms2d(data[3]+':'+data[4]))
                         row.append(float(data[5]))
@@ -2389,17 +2396,17 @@
                                 if idx in [0,1]: ## Angular values
                                     if el > 0.008:
                                         goodval = False
                                 else:
                                     if el > 0.8:
                                         goodval = False
                             if not goodval:
-                                print("readIYFV: verify conversions between components !")
-                                print("readIYFV: found:", np.array(row))
-                                print("readIYFV: expected:", np.array(checklist))
+                                logger.warning("readIYFV: verify conversions between components !")
+                                logger.warning("readIYFV: found: {}".format(np.array(row)))
+                                logger.warning("readIYFV: expected: {}".format(np.array(checklist)))
                         elif t == 'J' and tprev == tsel:
                             jumpx = jumpx + row[para.index('x')]
                             jumpy = jumpy + row[para.index('y')]
                             jumpz = jumpz + row[para.index('z')]
                             jumpf = jumpf + row[para.index('f')]
                         tprev = tsel
     fh.close()
@@ -2433,77 +2440,77 @@
     comment = kwargs.get('comment')
 
     if not kind in ['A','Q','D','q','d']:
         kind = 'A'
     else:
         kind = kind.upper()
     if comment:
-        print (" writeIYFV: Comments not yet supported")
+        logger.info("writeIYFV: Comments not yet supported")
         #identify next note and add comment at the send of the file
         pass
     else:
         note = 0
 
     # check datastream
     if not datastream.length()[0] > 1:
-        print (" writeIYFV: Datastream does not contain data")
+        logger.error(" writeIYFV: Datastream does not contain data")
         return False
     if not len(datastream.ndarray[1]) > 1:
-        print (" writeIYFV: Datastream does not contain data")
+        logger.error(" writeIYFV: Datastream does not contain data")
         return False
     # check time range
     tmin, tmax = datastream._find_t_limits()
     tmin = date2num(tmin)
     tmax = date2num(tmax)
     meant = mean([tmin,tmax])
     if tmax-tmin < 365*0.9: # 90% of one year
-        print (" writeIYFV: Datastream does not cover at least 90% of one year")
+        logger.error(" writeIYFV: Datastream does not cover at least 90% of one year")
         return False
     # if timerange covers more than one year ??????
     # should be automatically called with coverage='year' and filenamebegins='yearmean',
     # filenameends=Obscode
 
     header = datastream.header
     comp = header.get('DataComponents','')
     comp = comp.lower()
-    print(("writeIYFV: components found: ", comp))
+    logger.info(("writeIYFV: components found: {}".format(comp)))
     if not comp in ['hdz','xyz','idf','hez', 'hdzf','xyzf','idff','hezf', 'hdzg','xyzg','idfg','hezg']:
-        print (" writeIYFV: valid DataComponents could not be read from header - assuming xyz data")
+        logger.warning(" writeIYFV: valid DataComponents could not be read from header - assuming xyz data")
         comp = 'xyz'
     elif comp.startswith('hdz'):
         datastream = datastream.hdz2xyz()
     elif comp.startswith('idf'):
         datastream = datastream.idf2xyz()
     elif comp.startswith('hez'):
         alpha = header.get('DataSensorAzimuth','')
         if not is_number(alpha):
-            print (" writeIYFV: hez provided but no DataSensorAzimuth (usually the declination while sensor installation - aborting")
+            logger.error(" writeIYFV: hez provided but no DataSensorAzimuth (usually the declination while sensor installation - aborting")
             return False
         datastream = datastream.rotation(alpha=alpha)
 
     # Obtain means   ( drop nans ):
     meanx = datastream.mean('x',percentage=90)
     meany = datastream.mean('y',percentage=90)
     meanz = datastream.mean('z',percentage=90)
     if isnan(meanx) or isnan(meany) or isnan(meanz):
-        print (" writeIYFV: found more then 10% of NaN values - setting minimum requirement to 40% data recovery and change kind to I (incomplete)")
+        logger.warning(" writeIYFV: found more then 10% of NaN values - setting minimum requirement to 40% data recovery and change kind to I (incomplete)")
         meanx = datastream.mean('x',percentage=40)
         meany = datastream.mean('y',percentage=40)
         meanz = datastream.mean('z',percentage=40)
         kind = 'I'
         if isnan(meanx) or isnan(meany) or isnan(meanz):
-            print (" writeIYFV: less then 40% of data - skipping")
+            logger.error(" writeIYFV: less then 40% of data - aborting")
             return False
     meanyear = int(datetime.strftime(num2date(meant),"%Y"))
     # create datalist
     datalist = [meanyear]
     reslist = coordinatetransform(meanx,meany,meanz,'xyz')
     datalist.extend(reslist)
 
-    print ( "writeIYFV means:", meanx, meany, meanz )
+    logger.info( "writeIYFV means: {}, {}, {}".format(meanx, meany, meanz ))
     #print ( "writeIYFV: kind", kind )
     #print ( "writeIYFV: comment", comment )
     #kind = 'Q'
     #meanyear = '2011'
 
     #_YYYY.yyy_DDD_dd.d_III_ii.i_HHHHHH_XXXXXX_YYYYYY_ZZZZZZ_FFFFFF_A_EEEE_NNNCrLf
     decsep= str(datalist[1]).split('.')
@@ -2513,15 +2520,15 @@
     # create dummy header (check for existing values) and add data
     # inform observer to modify/check head
     def createhead(filename, locationname,coordlist,newline):
         """
         internal method to create header info for yearmean file
         """
         if not len(coordlist) == 3:
-            print ("writeIYFV: Coordinates missing")
+            logger.warning("writeIYFV: Coordinates missing")
             if len(coordlist) == 2:
                 coordlist.append(np.nan)
             else:
                 return False
 
         empty = "\r\n"
         content = []
```

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_wik.py` & `GeomagPy-v0.3.93/magpy/lib/format_wik.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_iaga02.py` & `GeomagPy-v0.3.93/magpy/lib/format_iaga02.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_dtu.py` & `GeomagPy-v0.3.93/magpy/lib/format_dtu.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_cr800.py` & `GeomagPy-v0.3.93/magpy/lib/format_cr800.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_abs_magpy.py` & `GeomagPy-v0.3.93/magpy/lib/format_abs_magpy.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_noaa.py` & `GeomagPy-v0.3.93/magpy/lib/format_noaa.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_pos1.py` & `GeomagPy-v0.3.93/magpy/lib/format_pos1.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/lib/format_magpy.py` & `GeomagPy-v0.3.93/magpy/lib/format_magpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from __future__ import absolute_import
 from __future__ import division
 from io import open
 
 # Specify what methods are really needed
 from magpy.stream import *
 
+import logging
+logger = logging.getLogger(__name__)
+
 import gc
 
 
 # K0 (Browsing - not for Serious Science) ACE-EPAM data from the OMNI database:
 k0_epm_KEYDICT = {#'H_lo',                      # H (0.48-0.97 MeV)     (UNUSED)
                 'Ion_very_lo': 'var1',          # Ion (47-65 keV) 1/(cm2 s ster MeV)
                 'Ion_lo': 'var2',               # Ion (310-580 keV) 1/(cm2 s ster MeV)
@@ -65,60 +68,60 @@
     try:
         if not 'Epoch' in temp:
             if not 'time' in temp:
                 return False
     except:
         return False
 
-    #loggerlib.debug("format_magpy: Found PYCDF file %s" % filename)
+    logger.debug("format_magpy: Found PYCDF file %s" % filename)
     return True
 
 
 def isPYSTR(filename):
     """
     Checks whether a file is ASCII PyStr format.
     """
     try:
         temp = open(filename, 'rt').readline()
     except:
         return False
     if not temp.startswith(' # MagPy - ASCII'):
         return False
 
-    #loggerlib.debug("format_magpy: Found PYSTR file %s" % filename)
+    logger.debug("format_magpy: Found PYSTR file %s" % filename)
     return True
 
 
 def isPYASCII(filename):
     """
     Checks whether a file is ASCII PyStr format.
     """
     try:
         temp = open(filename, 'rt').readline()
     except:
         return False
     if not temp.startswith(' # MagPy ASCII'):
         return False
 
-    #loggerlib.debug("format_magpy: Found PYSTR file %s" % filename)
+    logger.debug("format_magpy: Found PYASCII file %s" % filename)
     return True
 
 
 def isPYBIN(filename):
     """
     Checks whether a file is binary PyStr format.
     """
     try:
         temp = open(filename, 'r', encoding='utf-8', newline='', errors='ignore').readline()
     except:
         return False
     if not temp.startswith('# MagPyBin'):
         return False
 
-    #loggerlib.debug("format_magpy: Found PYBIN file %s" % filename)
+    logger.debug("format_magpy: Found PYBIN file %s" % filename)
     return True
 
 
 def readPYASCII(filename, headonly=False, **kwargs):
     """
     Reading basic ASCII format data.
     Should look like:
@@ -129,15 +132,15 @@
     """
     stream = DataStream([],{})
 
     array = [[] for key in KEYLIST]
 
     headers = {}
 
-    loggerlib.info('readPYASCII: Reading %s' % (filename))
+    logger.info('readPYASCII: Reading %s' % (filename))
 
     qFile= open( filename, "r", newline='' )
 
     csvReader= csv.reader( qFile )
     keylst = []
     timeconv = False
     timecol = -1
@@ -226,15 +229,15 @@
     stream = DataStream([],{})
 
     array = [[] for key in KEYLIST]
 
     # Check whether header infromation is already present
     headers={}
 
-    loggerlib.info('readPYSTR: Reading %s' % (filename))
+    logger.info('readPYSTR: Reading %s' % (filename))
     #qFile= file( filename, "rb" )
     qFile= open( filename, "rt", newline='' )
     csvReader= csv.reader( qFile )
 
     for elem in csvReader:
         if elem==[]:
             # blank line
@@ -363,15 +366,15 @@
         try:
             cdf_file = cdf.CDF(filename)
         except:
             return stream
         try:
             cdfformat = cdf_file.attrs['DataFormat']
         except:
-            logging.info("No format specification in CDF - passing")
+            logger.info("readPYCDF: No format specification in CDF - passing")
             cdfformat = 'Unknown'
             pass
         OMNIACE = False
         try:
             title = str(cdf_file.attrs['TITLE'])
             if 'ACE' in title:
                 OMNIACE = True
@@ -379,26 +382,26 @@
             pass
 
         if headskip:
             for key in cdf_file.attrs:
                 if not key in ['DataAbsFunctionObject','DataBaseValues', 'DataFlagList']:
                     stream.header[key] = str(cdf_file.attrs[key])
                 else:
-                    print("Found Object - loading and unpickling")
+                    logger.debug("readPYCDF: Found object - loading and unpickling")
                     try:
                         func = pickle.loads(str(cdf_file.attrs[key]))
                         stream.header[key] = func
                     except:
-                        print("Failed to load Object - constructed before v0.2.000?")
+                        logger.debug("readPYCDF: Failed to load Object - constructed before v0.2.000?")
 
         #if headonly:
         #    cdf_file.close()
         #    return DataStream(stream, stream.header)
 
-        loggerlib.info('Read: %s Format: %s ' % (filename, cdfformat))
+        logger.info('readPYCDF: %s Format: %s ' % (filename, cdfformat))
 
         for key in cdf_file:
             #print key
             #try:
             #    print key, cdf_file[key].attrs['LABLAXIS'], cdf_file[key].attrs['UNITS']
             #except:
             #    print key
@@ -726,134 +729,126 @@
                 getfile = False
     except:
         # Date format not recognized. Need to read all files
         getfile = True
     logbaddata = False
 
     if getfile:
-        loggerlib.info("read: %s Format: PYCDF" % filename)
-        if debug:
-            print ("PYBIN: Found pybin files")
+        logger.info("readPYBIN: %s Format: PYCDF" % filename)
 
         fh = open(filename, 'rb')
         #fh = open(filename, 'r', encoding='utf-8', newline='', errors='ignore')
         #infile = open(filename, 'r', encoding='utf-8', newline='')
         # read header line and extract packing format
         header = fh.readline()
         header = header.decode('utf-8')
         # some cleaning actions for false header inputs
         header = header.replace(', ',',')
         header = header.replace('deg C','deg')
         h_elem = header.strip().split()
-        if debug:
-            print ("PYBIN: Header {}".format(header))
+        logger.debug("PYBIN: Header {}".format(header))
 
-        if debug:
-            print('readPYBIN- debug header type (len should be 9): ', h_elem, len(h_elem))
+        logger.debug('readPYBIN- debug header type (len should be 9): {}, {}'.format(h_elem, len(h_elem)))
 
         if not h_elem[1] == 'MagPyBin':
-            print('readPYBIN: No MagPyBin format - aborting')
+            logger.error('readPYBIN: No MagPyBin format - aborting')
             return
         #print "Length ", len(h_elem), h_elem[2]
 
         #Test whether element 3,4,5 (and 6) are lists of equal length
         if len(h_elem) == 8:
             #print "Very old import format"
             nospecial = True
             try:
                 if not keylist:
-                    loggerlib.error('readPYBIN: keylist of length(elemlist) needs to be specified')
+                    logger.error('readPYBIN: keylist of length(elemlist) needs to be specified')
                     return stream
                 elemlist = h_elem[3].strip('[').strip(']').split(',')
                 unitlist = h_elem[4].strip('[').strip(']').split(',')
                 multilist = list(map(float,h_elem[5].strip('[').strip(']').split(',')))
             except:
-                print("readPYBIN: Could not extract lists from header - check format - aborting...")
+                logger.error("readPYBIN: Could not extract lists from header - check format - aborting...")
                 return stream
             if not len(keylist) == len(elemlist) or not len(keylist) == len(unitlist) or not  len(keylist) == len(multilist):
-                loggerlib.error("readPYBIN: Provided lists from header of differenet lengths - check format - aborting...")
+                logger.error("readPYBIN: Provided lists from header of differenet lengths - check format - aborting...")
                 return stream
         elif len(h_elem) == 9:
             #print "The current format"
             nospecial = True
             try:
                 keylist = h_elem[3].strip('[').strip(']').split(',')
                 elemlist = h_elem[4].strip('[').strip(']').split(',')
                 unitlist = h_elem[5].strip('[').strip(']').split(',')
                 multilist = list(map(float,h_elem[6].strip('[').strip(']').split(',')))
             except:
-                loggerlib.error("readPYBIN: Could not extract lists from header - check format - aborting...")
+                logger.error("readPYBIN: Could not extract lists from header - check format - aborting...")
                 return stream
             if not len(keylist) == len(elemlist) or not len(keylist) == len(unitlist) or not  len(keylist) == len(multilist):
                 if debug:
                     print('readPYBIN- header list error:', len(keylist), len(elemlist), len(unitlist), len(multilist))
-                loggerlib.error("readPYBIN: Provided lists from header of differenet lengths - check format - aborting...")
+                logger.error("readPYBIN: Provided lists from header of differenet lengths - check format - aborting...")
                 return stream
         elif len(h_elem) == 10:
-            #print "Special format"
-            loggerlib.debug("readPYBIN: Special format detected. May not be able to read file.")
+            logger.info("readPYBIN: Special format detected. May not be able to read file.")
             nospecial = False
             if h_elem[2][:5] == 'ENV05' or h_elem[2] == 'Env05':
                 keylist = h_elem[3].strip('[').strip(']').split(',')
                 elemlist = h_elem[4].strip('[').strip(']').split(',')
                 unitlist = h_elem[5].strip('[').strip(']').split(',')
                 multilist = list(map(float,h_elem[7].strip('[').strip(']').split(',')))
                 nospecial = True
         else:
-            loggerlib.error('readPYBIN: No valid MagPyBin format, inadequate header length - aborting')
+            logger.error('readPYBIN: No valid MagPyBin format, inadequate header length - aborting')
             return stream
 
-        if debug:
-            print('readPYBIN- checking code')
+        logger.debug('readPYBIN: checking code')
 
         packstr = '<'+h_elem[-2]+'B'
         packstr = packstr.encode('ascii','ignore')
         lengthcode = struct.calcsize(packstr)
         lengthgiven = int(h_elem[-1])+1
         length = lengthgiven
         if not lengthcode == lengthgiven:
-            loggerlib.debug("readPYBIN: Check your packing code!")
+            logger.debug("readPYBIN: Check your packing code!")
             if lengthcode < lengthgiven:
                 missings = lengthgiven-lengthcode
                 for i in range(missings):
                     packstr += 'B'
                     length = lengthgiven
             else:
                 length = lengthcode
 
-        if debug:
-            print('readPYBIN- unpack info:', packstr, lengthcode, lengthgiven)
+        logger.debug('readPYBIN: unpack info: {}, {}, {}'.format(packstr, lengthcode, lengthgiven))
 
         #fh = open(filename, 'rb')
         line = fh.read(length)
         stream.header['SensorID'] = h_elem[2]
         stream.header['SensorElements'] = ','.join(elemlist)
         stream.header['SensorKeys'] = ','.join(keylist)
         lenel = len([el for el in elemlist if el in KEYLIST]) # If elemlist and Keylist are disorderd
         lenke = len([el for el in keylist if el in KEYLIST])
         if lenel > lenke:
             keylist = elemlist
 
         array = [[] for key in KEYLIST]
         if nospecial:
-            if debug:
-                print('readPYBIN- debug found line')
+            logger.debug('readPYBIN- debug found line')
 
             for idx, elem in enumerate(keylist):
                 stream.header['col-'+elem] = elemlist[idx]
                 stream.header['unit-col-'+elem] = unitlist[idx]
                 # Header info
                 pass
             while not len(line) == 0:
                 lastdata = 'None'
                 data = 'None'
                 try:
                     data= struct.unpack(packstr, line)
                 except:
-                    print("readPYBIN: struct error", filename, len(line))
+                    logger.error("readPYBIN: struct error {} {}".format(filename, len(line)))
                 try:
                     time = datetime(data[0],data[1],data[2],data[3],data[4],data[5],data[6])
                     if not oldtype:
                         array[0].append(date2num(stream._testtime(time)))
                         # check elemlist and keylist
                         for idx, elem in enumerate(keylist):
                             try:
@@ -880,61 +875,60 @@
                     else:
                         row = LineStruct()
                         row.time = date2num(stream._testtime(time))
                         for idx, elem in enumerate(keylist):
                             exec('row.'+keylist[idx]+' = data[idx+7]/float(multilist[idx])')
                         stream.add(row)
                     if logbaddata == True:
-                        loggerlib.error("readPYBIN: Good data resumes with: %s" % str(data))
+                        logger.error("readPYBIN: Good data resumes with: %s" % str(data))
                         logbaddata = False
                 except:
-                    loggerlib.error("readPYBIN: Error in line while reading data file. Last line at: %s" % str(lastdata))
+                    logger.error("readPYBIN: Error in line while reading data file. Last line at: %s" % str(lastdata))
                     logbaddata = True
                 lastdata = data
                 line = fh.read(length)
         else:
-            print("To be done ...")
+            print("Not implemented")
             pass
 
         array = np.asarray([np.asarray(el).astype(object) for el in array])
         stream.ndarray = array
         if len(stream.ndarray[0]) > 0:
-            if debug:
-                print("readPYBIN: Imported bin as ndarray")
+            logger.debug("readPYBIN: Imported bin as ndarray")
             stream.container = [LineStruct()]
             # if unequal lengths are found, then usually txt and bin files are loaded together
 
     return stream
 
 
 def writePYSTR(datastream, filename, **kwargs):
     """
     Function to write structural ASCII data
     """
 
     mode = kwargs.get('mode')
-    loggerlib.info("writePYSTR: Writing file to %s" % filename)
+    logger.info("writePYSTR: Writing file to %s" % filename)
 
     if os.path.isfile(filename):
         if mode == 'skip': # skip existing inputs
             try:
                 exst = read(path_or_url=filename)
                 datastream = joinStreams(exst,datastream)
             except:
-                loggerlib.info("writePYSTR: Could not interprete existing file - replacing" % filename)
+                logger.info("writePYSTR: Could not interprete existing file - replacing %s" % filename)
             if sys.version_info >= (3,0,0):
                 myFile= open( filename, "w", newline='' )
             else:
                 myFile= open( filename, "wb")
         elif mode == 'replace': # replace existing inputs
             try:
                 exst = read(path_or_url=filename)
                 datastream = joinStreams(datastream,exst)
             except:
-                loggerlib.info("writePYSTR: Could not interprete existing file - replacing" % filename)
+                logger.info("writePYSTR: Could not interprete existing file - replacing %s" % filename)
             if sys.version_info >= (3,0,0):
                 myFile= open( filename, "w", newline='' )
             else:
                 myFile= open( filename, "wb")
         elif mode == 'append':
             if sys.version_info >= (3,0,0):
                 myFile= open( filename, "a", newline='' )
@@ -1053,15 +1047,15 @@
             #### If memory issues appear then please overwrite existing data
             #### TODO Optimze sorting
             #### !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
             try:
                 exst = read(path_or_url=filename+'.cdf')
                 datastream = joinStreams(datastream,exst,extend=True)
             except:
-                print("Could not interprete existing data set - aborting")
+                logger.error("writePYCDF: Could not interprete existing data set - aborting")
                 sys.exit()
             os.remove(filename+'.cdf')
             mycdf = cdf.CDF(filename, '')
         elif mode == 'append':
             #print filename
             exst = read(path_or_url=filename+'.cdf')
             datastream = joinStreams(exst,datastream,extend=True)
@@ -1093,15 +1087,15 @@
     if not mode == 'append':
         for key in headdict:
             if not key.find('col') >= 0:
                 #print key, headdict[key]
                 if not key in ['DataAbsFunctionObject','DataBaseValues', 'DataFlagList']:
                     mycdf.attrs[key] = headdict[key]
                 else:
-                    print("Found Object in header - pickle and dump ")
+                    logger.info("writePYCDF: Found Object in header - pickle and dump ")
                     pfunc = pickle.dumps(headdict[key])
                     mycdf.attrs[key] = pfunc
 
     mycdf.attrs['DataFormat'] = 'MagPyCDF'
 
     #def checkEqualIvo(lst):
     #    # http://stackoverflow.com/questions/3844801/check-if-all-elements-in-a-list-are-identical
@@ -1134,15 +1128,15 @@
         try:
             test = [elem for elem in col if not isnan(elem)]
             if not len(test) > 0:
                 col = np.asarray([])
         except:
             pass
         if not False in checkEqual3(col) and len(col) > 0:
-            print("Found identical values only: %s" % key)
+            logger.warning("writePYCDF: Found identical values only for key: %s" % key)
             col = col[:1]
             #if not col[0] in ['nan', float('nan'),NaN,'-',None,'']: #remove place holders
             #- better not!!! 2015-10-14 --- if two files are loaded, one with flags, one without, then column lengths will not fit
             #    col = col[:1]
             #else:
             #    col = np.asarray([])
 
@@ -1185,42 +1179,42 @@
     if compression == 0: ## temporary solution until all refs to skipcomression are eliminated
         skipcompression = True
 
     if isinstance(compression, int) and not compression == 0 and compression in range(0,10) and not skipcompression and len(mycdf['Epoch']) > 0:
         try:
             mycdf.compress(cdf.const.GZIP_COMPRESSION, compression)
         except:
-            print("format_magypy: compression of CDF failed - Trying to store uncompressed data")
-            print("format_magypy: please use option skipcompression=True if unreadable")
-            print("format_magypy: CDF: {}".format(mycdf))
-            print("format_magypy: attrs: {}".format(mycdf.attrs))
-            pass
+            logger.warning("writePYCDF: : compression of CDF failed - Trying to store uncompressed data")
+            logger.warning("writePYCDF: please use option skipcompression=True if unreadable")
+            #logger.info("writePYCDF: : CDF: {}".format(mycdf))
+            #logger.info("writePYCDF: attrs: {}".format(mycdf.attrs))
+            #pass
 
     mycdf.close()
     return True
 
 
 def writePYASCII(datastream, filename, **kwargs):
     """
     Function to write basic ASCII data
     """
 
     mode = kwargs.get('mode')
-    loggerlib.info("writePYASCII: Writing file to %s" % filename)
+    logger.info("writePYASCII: Writing file to %s" % filename)
 
     if os.path.isfile(filename):
         if mode == 'skip': # skip existing inputs
             exst = read(path_or_url=filename)
             datastream = joinStreams(exst,datastream,extend=True)
             if sys.version_info >= (3,0,0):
                 myFile = open(filename, 'w', newline='')
             else:
                 myFile = open(filename, 'wb')
         elif mode == 'replace': # replace existing inputs
-            print("write ascii filename", filename)
+            logger.debug("write ascii filename", filename)
             exst = read(path_or_url=filename)
             datastream = joinStreams(datastream,exst,extend=True)
             if sys.version_info >= (3,0,0):
                 myFile = open(filename, 'w', newline='')
             else:
                 myFile = open(filename, 'wb')
         elif mode == 'append':
```

### Comparing `GeomagPy-v0.3.92/magpy/lib/magpy_absformats.py` & `GeomagPy-v0.3.93/magpy/lib/magpy_absformats.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/transfer.py` & `GeomagPy-v0.3.93/magpy/transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from __future__ import absolute_import
 from __future__ import unicode_literals
 from __future__ import division
 
 from magpy.stream import *
 import ftplib
 import subprocess
+import logging
+logger = logging.getLogger(__name__)
 
 try:
     import pexpect
     ssh = True
 except:
-    print("SSH support not active - please install package pexpect to use this functionality")
+    logger.warning("SSH support not active - please install the pexpect package to use this functionality")
     ssh = False
 
 # Define defaults:
 
 # ####################
 # Check log files
 # ####################
```

### Comparing `GeomagPy-v0.3.92/magpy/examples/example1.cdf` & `GeomagPy-v0.3.93/magpy/examples/example1.cdf`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/examples/example5.cdf` & `GeomagPy-v0.3.93/magpy/examples/example5.cdf`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/mpplot.py` & `GeomagPy-v0.3.93/magpy/mpplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 '''
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import unicode_literals
 from __future__ import division
 
 from magpy.stream import *
+
+import logging
+logger = logging.getLogger(__name__)
 '''
 try:
     import matplotlib
     if not os.isatty(sys.stdout.fileno()):   # checks if stdout is connected to a terminal (if not, cron is starting the job)
         print "No terminal connected - assuming cron job and using Agg for matplotlib"
         matplotlib.use('Agg') # For using cron
 except:
@@ -66,16 +69,16 @@
     from matplotlib.colors import Normalize
     from matplotlib import mlab
     from matplotlib.dates import date2num, num2date
     import matplotlib.cm as cm
     from pylab import *
     from datetime import datetime, timedelta
 except ImportError as e:
-    loggerplot.error("plot package: Matplotlib import error. If missing, please install to proceed.")
-    loggerplot.error("Error string: %s" % e)
+    logger.error("plot package: Matplotlib import error. If missing, please install to proceed.")
+    logger.error("Error string: %s" % e)
     raise Exception("CRITICAL IMPORT ERROR FOR PLOT PACKAGE: Matplotlib import error.")
 '''
 
 # TODO:
 # - Move all plotting functions over from stream.
 #       STILL TO FIX:
 #       spectrogram()
@@ -127,15 +130,15 @@
         sensorid = ''
     try:
         datadate = datetime.strftime(num2date(stream[0].time),'%Y-%m-%d')
     except:
         datadate = datetime.strftime(num2date(stream.ndarray[0][0]),'%Y-%m-%d')
 
     plottitle = "%s (%s)" % (sensorid,datadate)
-    print("Plotting keys:", keys)
+    logger.info("Plotting keys:", keys)
     plot_new(stream, keys,
                 confinex = True,
                 plottitle = plottitle)
 
 #####################################################################
 #                                                                   #
 #       MAIN PLOTTING FUNCTIONS                                     #
@@ -213,27 +216,25 @@
         >>>
 
     APPLICATION:
 
     '''
 
     # Test whether columns really contain data or whether only nans are present:
-    #print stream.ndarray
     stream = stream._remove_nancolumns()
     availablekeys = stream._get_key_headers(numerical=True)
     logger = logging.getLogger(__name__+".plot")
-    #print stream.ndarray
 
     # if no variables are given, use all available:
     if len(variables) < 1:
         variables = availablekeys
     else:
         variables = [var for var in variables if var in availablekeys]
     if len(variables) > 9:
-        logger.info("More than 9 variables available - plotting only the first nine:", end=' ')
+        logger.info("More than 9 variables available - plotting only the first nine!")
         logger.info("Available: "+ str(variables))
         variables = variables[:9]
         logger.info("Plotting: "+ str(variables))
     else:
         logger.info("Plotting: "+ str(variables))
 
     # Check lists for variables have correct length:
@@ -393,23 +394,23 @@
 
     # Preselect only numerical values
     variables = [[el for el in lst if el in NUMKEYLIST] for lst in variables]
     num_of_var = 0
     for item in variables:
         num_of_var += len(item)
     if num_of_var > 9:
-        logger.error("plotStreams: Can't plot more than 9 variables, sorry.")
+        logger.error("Can't plot more than 9 variables, sorry.")
         raise Exception("Can't plot more than 9 variables!")
 
     # Check lists for variables have correct length:
     if len(symbollist) < num_of_var:
-        logger.error("plotStreams: Length of symbol list does not match number of variables.")
+        logger.error("Length of symbol list does not match number of variables.")
         raise Exception("Length of symbol list does not match number of variables.")
     if len(colorlist) < num_of_var:
-        logger.error("plotStreams: Length of color list does not match number of variables.")
+        logger.error("Length of color list does not match number of variables.")
         raise Exception("Length of color list does not match number of variables.")
 
     plot_dict = []
     count = 0
 
     if not resolution:
         resolution = 5000000  # 40 days of 1 second data can be maximaly shown in detail, 5 days of 10 Hz
@@ -466,15 +467,15 @@
             if dropflagged:
                 flagind = KEYLIST.index('flag')
                 flags = stream.ndarray[flagind]
                 ind = KEYLIST.index(key)
                 flagarray =  np.asarray([list(el)[ind] for el in flags])
                 print("Flagarray", flagarray)
                 indicies = np.where(flagarray == '1')
-                print("Indicies", indicies)
+                print("Indicis", indicis)
                 #for index in indicies:
                 #    y[index] = NaN
                     #y[index] = float('nan')
                     #newflag = flags[0][ind]
                     #newflag[indexflag] = '0'
                     #data[i]['flags'][0][ind] == newflag
                 #y = np.delete(np.asarray(y),indicies)
@@ -701,15 +702,15 @@
         self.axes = False
 
         self.orgkeylist = self.data._get_key_headers()
         if not variables: #or variables == ['x','y','z','f'] or variables == ['x','y','z']:
             try:
                 self.data = self.analyzeData(self.orgkeylist)
             except:
-                print("plotFlag: You have to provide variables for this data set")
+                logger.warning("figFlagger.__init__: You have to provide variables for this data set")
 
 
         keylist = self.data._get_key_headers(numerical=True)
         #print keylist
         if variables:
             keylist = variables
         if len(keylist) > 9:
@@ -728,16 +729,16 @@
             self.axes = self.fig.axes
         else:
             plt.show()
 
     def analyzeData(self,keylist):
         #keylist = self.data._get_key_headers()
         if not len(self.data.ndarray[0]) > 0:
-            print("No ndarrayfound:")
-            print(" -- stream will be converted to ndarray type")
+            logger.warning("figFlagger.analyzeData: No ndarray found:")
+            logger.warning("figFlagger.analyzeData: stream will be converted to ndarray type")
             self.data = self.data.linestruct2ndarray()
 
         if 'x' in keylist and 'y' in keylist and 'z' in keylist:
             self.data = self.data.differentiate(keys=['x','y','z'],put2keys = ['dx','dy','dz'])
             if 'f' in keylist:
                 self.data = self.data.delta_f()
         return self.data
@@ -1062,27 +1063,24 @@
 
     # TODO:
     # - make axes easier to read
     # - add a amplitude statistic (histogram)
     # - add a haeufigkeit plot perpendicular to the diagrams
     import magpy.opt.emd as emd # XXX: add this into main program when method is finalised
 
-    loggerplot.info("plotEMD: Starting EMD calculation.")
+    logger.info("plotEMD: Starting EMD calculation.")
 
     col = stream._get_column(key)
     timecol = stream._get_column('time')
-    if verbose:
-        print("Amount of values and standard deviation:", len(col), np.std(col))
+    logger.debug("plotEMD: Amount of values and standard deviation:", len(col), np.std(col))
 
     res = emd.emd(col,max_modes=max_modes)
-    if verbose:
-        print("Found the following amount of decomposed modes:", len(res))
+    logger.debug("plotEMD: Found the following amount of decomposed modes:", len(res))
     separate = int(np.round(len(res)*sratio,0))
-    if verbose:
-        print("Separating the last N curves as smooth. N =",separate)
+    logger.debug("plotEMD: Separating the last N curves as smooth. N =",separate)
     stdarray = []
     newcurve = [0]*len(res[0])
     noisecurve = [0]*len(res[0])
     midcurve = [0]*len(res[0])
     smoothcurve = [0]*len(res[0])
     f, axarr = plt.subplots(len(res), sharex=True)
 
@@ -1101,24 +1099,21 @@
             smoothcurve = [x + y for x, y in zip(smoothcurve, elem)]
         if i < len(res)-separate:
             if verbose:
                 print "Noise:", i
             noisecurve = [x + y for x, y in zip(noisecurve, elem)]
         """
         if i > stackvals[2]: # 14 - add stackvals = [2,8,14]
-            if verbose:
-                print("Smooth:", i)
+            logger.debug("plotEMD: Smooth: {}".format(i))
             smoothcurve = [x + y for x, y in zip(smoothcurve, elem)]
         if stackvals[1] <= i <= stackvals[2]:
-            if verbose:
-                print("Mid:", i)
+            logger.debug("plotEMD: Mid: {}".format(i))
             midcurve = [x + y for x, y in zip(midcurve, elem)]
         if stackvals[0] < i < stackvals[1]:
-            if verbose:
-                print("Noise:", i)
+            logger.debug("plotEMD: Noise: {}".format(i))
             noisecurve = [x + y for x, y in zip(noisecurve, elem)]
 
     plt.show()
 
     plt.plot(smoothcurve)
     #plt.plot(newcurve)
     plt.title("Variation of IMF 14 to 17 component - low frequency content")
@@ -1204,25 +1199,25 @@
     fig = plt.figure()
     ax = fig.add_subplot(1,1,1)
 
     arraylist = []
 
     if labels:
         if len(labels) != len(streamlist):
-            loggerplot.warning("plotNormStreams: Number of labels does not match number of streams!")
+            logger.warning("plotNormStreams: Number of labels does not match number of streams!")
 
     for i, stream in enumerate(streamlist):
-        loggerplot.info("plotNormStreams: Adding stream %s of %s..." % ((i+1),len(streamlist)))
+        logger.info("plotNormStreams: Adding stream %s of %s..." % ((i+1),len(streamlist)))
         y = stream._get_column(key)
         t = stream._get_column('time')
         xlabel = "Time (UTC)"
         color = colorlist[i]
 
         if len(y) == 0:
-            loggerplot.error("plotNormStreams: stream with empty array!")
+            logger.error("plotNormStreams: stream with empty array!")
             return
         try:
             yunit = stream.header['unit-col-'+key]
         except:
             yunit = ''
         #ylabel = stream.header['col-'+key].upper()+' $['+re.sub('[#$%&~_^\{}]', '', yunit)+']$'
         ylabel = stream.header['col-'+key].upper()+' $['+re.sub('[#$%&~_\{}]', '', yunit)+']$'
@@ -1343,55 +1338,51 @@
                         endtime='2013-06-11 00:00:00')
         2. Call for data stream:
         >>> data.powerspectrum('f',
                         plottitletitle='PSD of f', marks={'day':0.000011574},
                         outfile='ps.png')
     """
 
-    logger = logging.getLogger(__name__+".plotPS")
-    logger.info("Starting powerspectrum calculation.")
+    logger.info("plotPS: Starting power spectrum calculation")
 
     if noshow == True:
         show = False
     elif noshow == False:
         show = True
     else:
-        logger.error("Incorrect value ({:s}) for variable noshow.".format(noshow))
-        raise ValueError("Incorrect value ({:s}) for variable noshow.".format(noshow))
+        logger.error("plotPS: Incorrect value ({:s}) for variable noshow.".format(noshow))
+        raise ValueError("plotPS: Incorrect value ({:s}) for variable noshow.".format(noshow))
 
     dt = stream.get_sampling_period()*24*3600
 
     if not stream.length()[0] > 0:
-        logger.error("Stream of zero length -- aborting.")
-        raise Exception("Can't analyse power spectrum of stream of zero length!")
+        logger.error("plotPS: Stream of zero length -- aborting.")
+        raise Exception("plotPS: Can't analyse power spectrum of stream of zero length!")
 
     t_new, val_new, nfft = _extract_data_for_PSD(stream, key)
 
-    if debugmode:
-        print("Extracted data for powerspectrum at %s" % datetime.utcnow())
+    logger.debug("plotPS: Extracted data for powerspectrum at %s" % datetime.utcnow())
 
     if not axes:
         fig = plt.figure()
         ax = fig.add_subplot(111)
     else:
         ax = axes
 
     psdm = mlab.psd(val_new, nfft, 1/dt)
     asdm = np.sqrt(psdm[0])
     freqm = psdm[1]
 
     ax.loglog(freqm, asdm,'b-')
 
-    if debugmode:
-        print("Maximum frequency:", max(freqm))
+    logger.debug("Maximum frequency: {}".format(max(freqm)))
 
     if freqlevel:
         val, idx = find_nearest(freqm, freqlevel)
-        if debugmode:
-            print("Maximum Noise Level at %s Hz: %s" % (val,asdm[idx]))
+        logger.debug("Maximum Noise Level at %s Hz: %s" % (val,asdm[idx]))
 
     if not marks:
         pass
     else:
         for elem in marks:
             ax.annotate(elem, xy=(marks[elem],min(asdm)),
                         xytext=(marks[elem],max(asdm)-(max(asdm)-min(asdm))*0.3),
@@ -1467,15 +1458,15 @@
     EXAMPLE:
         >>> plotSatMag(LEMI_data, ACE_data, ['x','y'])
 
     APPLICATION:
         >>>
     """
 
-    loggerplot.info("plotSatMag - Starting plotting of satellite and magnetic data...")
+    logger.info("plotSatMag - Starting plotting of satellite and magnetic data...")
 
     key_mag, key_sat = keys[0], keys[1]
     ind_mag, ind_sat, ind_t = KEYLIST.index(key_mag), KEYLIST.index(key_sat), KEYLIST.index('time')
 
     if len(mag_stream.ndarray) > 0.:
         t_mag = mag_stream.ndarray[ind_t]
         t_sat = sat_stream.ndarray[ind_t]
@@ -1506,15 +1497,15 @@
         nans, test = nan_helper(y_sat)
         newt_sat = [t_sat[idx] for idx, el in enumerate(y_sat) if not nans[idx]]
         t_sat = newt_sat
         y_sat = [el for idx, el in enumerate(y_sat) if not nans[idx]]
 
 
     if (len(y_sat) == 0 or len(y_mag)) == 0:
-        loggerplot.error("plotSatMag - Can't plot empty column! Full of nans?")
+        logger.error("plotSatMag - Can't plot empty column! Full of nans?")
         raise Exception("plotSatMag - Empty column!")
 
     # Define y-labels:
     try:
         ylabel_mag = mag_stream.header['col-'+key_mag].upper()
     except:
         ylabel_mag = ''
@@ -1628,18 +1619,18 @@
 
     if returnfig == True:
         fig = plt.gcf()
         return fig
 
     if outfile:
         plt.savefig(outfile,savedpi=80)
-        loggerplot.info("plotSatMag - Plot saved to %s." % outfile)
+        logger.info("plotSatMag - Plot saved to %s." % outfile)
     else:
         plt.show()
-        loggerplot.info("plotSatMag - Plot completed.")
+        logger.info("plotSatMag - Plot completed.")
 
 
 def plotSpectrogram(stream, keys, NFFT=1024, detrend=mlab.detrend_none,
              window=mlab.window_hanning, noverlap=900,
              cmap=cm.Accent, cbar=False, xextent=None, pad_to=None, sides='default',
              scale_by_freq=None, minfreq = None, maxfreq = None, plottitle=False, **kwargs):
     """
@@ -1686,15 +1677,15 @@
 
     t = stream._get_column('time')
 
     if not minfreq:
         minfreq = 0.0001
 
     if not len(t) > 0:
-        loggerplot.error('plotSpectrogram: stream of zero length -- aborting')
+        logger.error('plotSpectrogram: stream of zero length -- aborting')
         return
 
     for key in keys:
         val = stream._get_column(key)
         val = maskNAN(val)
         dt = stream.get_sampling_period()*(samp_rate_multiplicator)
         Fs = float(1.0/dt)
@@ -1906,32 +1897,32 @@
     EXAMPLE:
         >>> stream.stereoplot(focus='data',groups='str2')
 
     APPLICATION:
         >>>
     """
 
-    loggerplot.info('plotStereoplot: Starting plot of stereoplot.')
+    logger.info('plotStereoplot: Starting plot of stereoplot.')
 
     if not stream[0].typ == 'idff':
-        loggerplot.error('plotStereoplot: idf data required for stereoplot.')
+        logger.error('plotStereoplot: idf data required for stereoplot.')
         raise Exception("Idf data required for plotting a stereoplot!")
 
     inc = stream._get_column('x')
     dec = stream._get_column('y')
 
     col = ['']
     if groups:
         sel = stream._get_column(groups)
         col = list(set(list(sel)))
         if len(col) > 7:
             col = col[:7]
 
     if not len(dec) == len(inc):
-        loggerplot.error('plotStereoplot: Check input file - unequal inc and dec data?')
+        logger.error('plotStereoplot: Check input file - unequal inc and dec data?')
         return
 
     if not figure:
         fig = plt.figure()
     else:
         fig = figure
     ax = plt.gca()
```

### Comparing `GeomagPy-v0.3.92/magpy/stream.py` & `GeomagPy-v0.3.93/magpy/stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sys
 import tempfile
 
 # ----------------------------------------------------------------------------
 # Part 1: Import routines for packages
 # ----------------------------------------------------------------------------
 
-logpygen = ''           # temporary loggerstream variable
+logpygen = ''           # temporary logger variable
 badimports = []         # List of missing packages
 nasacdfdir = "c:\CDF Distribution\cdf33_1-dist\lib"
 
 # Logging
 # ---------
 # Select the home directory of the user (platform independent)
 from os.path import expanduser
@@ -46,29 +46,30 @@
     console = logging.StreamHandler()
     console.setLevel(warninglevel)
     logger.addHandler(console)
     
     return logger
 
 # Package loggers to identify info/problem source
-basiclogger = setup_logger(__name__)
+logger = setup_logger(__name__)
+# DEPRECATED: replaced by individual module loggers, delete these when sure they're no longer needed:
 loggerabs = logging.getLogger('abs')
 loggertransfer = logging.getLogger('transf')
 loggerdatabase = logging.getLogger('db')
 loggerstream = logging.getLogger('stream')
 loggerlib = logging.getLogger('lib')
 loggerplot = logging.getLogger('plot')
 
 # Special loggers for event notification
 stormlogger = logging.getLogger('stream')
 
-basiclogger.info("Initiating MagPy...")
+logger.info("Initiating MagPy...")
 
 from magpy.version import __version__
-basiclogger.info("MagPy version "+str(__version__))
+logger.info("MagPy version "+str(__version__))
 magpyversion = __version__
 
 # Standard packages
 # -----------------
 try:
     import csv
     import pickle
@@ -118,32 +119,32 @@
 
 # Matplotlib
 # ----------
 try:
     import matplotlib
     try:
         if not os.isatty(sys.stdout.fileno()):   # checks if stdout is connected to a terminal (if not, cron is starting the job)
-            basiclogger.info("No terminal connected - assuming cron job and using Agg for matplotlib")
+            logger.info("No terminal connected - assuming cron job and using Agg for matplotlib")
             matplotlib.use('Agg') # For using cron
     except:
-        basiclogger.warning("Problems with identfying cron job - windows system?")
+        logger.warning("Problems with identfying cron job - windows system?")
         pass
 except ImportError as e:
     logpygen += "CRITICAL MagPy initiation ImportError: problem with matplotlib.\n"
     badimports.append(e)
 
 try:
     version = matplotlib.__version__.replace('svn', '')
     try:
         version = map(int, version.replace("rc","").split("."))
         MATPLOTLIB_VERSION = list(version)
     except:
         version = version.strip("rc")
         MATPLOTLIB_VERSION = version
-    basiclogger.info("Loaded Matplotlib - Version %s" % str(MATPLOTLIB_VERSION))
+    logger.info("Loaded Matplotlib - Version %s" % str(MATPLOTLIB_VERSION))
     try:
         import matplotlib.pyplot as plt
     except: ## Workaround for anaconda PYQT4 patch error
         matplotlib.use('qt5agg')
         import matplotlib.pyplot as plt
     from matplotlib.colors import Normalize
     from matplotlib.widgets import RectangleSelector, RadioButtons
@@ -157,15 +158,15 @@
     logpygen += "CRITICAL MagPy initiation ImportError with matplotlib package. Please install to proceed.\n"
     logpygen += " ... if installed please check the permissions on .matplotlib in your homedirectory.\n"
     badimports.append(e)
 
 # Numpy & SciPy
 # -------------
 try:
-    basiclogger.info("Loading Numpy and SciPy...")
+    logger.info("Loading Numpy and SciPy...")
     import numpy as np
     import scipy as sp
     from scipy import interpolate
     from scipy import stats
     from scipy import signal
     from scipy.interpolate import UnivariateSpline
     from scipy.ndimage import filters
@@ -189,57 +190,57 @@
 # NASACDF - SpacePy
 # -----------------
 def findpath(name, path):
     for root, dirs, files in os.walk(path):
         if name in files:
             return root
 try:
-    basiclogger.info("Loading SpacePy package cdf support ...")
+    logger.info("Loading SpacePy package cdf support ...")
     try:
         # check for windows
         nasacdfdir = findpath('libcdf.dll','C:\CDF_Distribution') ## new path since nasaCDF3.6
         if not nasacdfdir:
             nasacdfdir = findpath('libcdf.dll','C:\CDF Distribution')
         #print nasacdfdir
         os.putenv("CDF_LIB", nasacdfdir)
-        basiclogger.info("Using CDF lib in %s" % nasacdfdir)
+        logger.info("Using CDF lib in %s" % nasacdfdir)
         try:
             import spacepy.pycdf as cdf
-            basiclogger.info("... success")
+            logger.info("... success")
         except KeyError as e:
             # Probably running at boot time - spacepy HOMEDRIVE cannot be detected
             badimports.append(e)
         except:
-            basiclogger.info("... Could not import spacepy")
+            logger.info("... Could not import spacepy")
             pass
     except:
         os.putenv("CDF_LIB", "/usr/local/cdf/lib")
-        basiclogger.info("using CDF lib in /usr/local/cdf")
+        logger.info("using CDF lib in /usr/local/cdf")
         try:
             import spacepy.pycdf as cdf
-            basiclogger.info("... success")
+            logger.info("... success")
         except KeyError as e:
             # Probably running at boot time - spacepy HOMEDRIVE cannot be detected
             badimports.append(e)
         except:
-            basiclogger.info("... Could not import spacepy")
+            logger.info("... Could not import spacepy")
             pass
 except ImportError as e:
     logpygen += "MagPy initiation ImportError: NASA cdf not available.\n"
     logpygen += "... if you want to use NASA CDF format support please install a current version.\n"
     badimports.append(e)
 
 if logpygen == '':
     logpygen = "OK"
 else:
-    basiclogger.info(logpygen)
-    basiclogger.info("Missing packages:")
+    logger.info(logpygen)
+    logger.info("Missing packages:")
     for item in badimports:
-        basiclogger.info(item)
-    basiclogger.info("Moving on anyway...")
+        logger.info(item)
+    logger.info("Moving on anyway...")
 
 ### Some Python3/2 compatibility code
 ### taken from http://www.rfk.id.au/blog/entry/preparing-pyenchant-for-python-3/
 try:
     unicode = unicode
     # 'unicode' exists, must be Python 2
     str = str
@@ -363,14 +364,15 @@
                 'POS1TXT':['r', 'POS-1 text format output data'],
                 'POS1':['r', 'POS-1 binary output at WIC'],
                 #'PYNC':['r', 'MagPy NetCDF variant (too be developed)'],
                 #'DTU1':['r', 'ASCII Data from the DTUs FGE systems'],
                 #'BDV1':['r', 'Budkov GDAS data variant'],
                 'GFZKP':['r', 'GeoForschungsZentrum KP-Index format'],
                 'NOAAACE':['r', 'NOAA ACE satellite data format'],
+                'NETCDF':['r', 'NetCDF4 format, NOAA DSCOVR satellite data archive format'],
                 'LATEX':['w','LateX data'],
                 'CS':['r','Cesium G823'],
                 #'SFDMI':['r', 'San Fernando variometer'],
                 #'SFGSM':['r', 'San Fernando GSM90'],
                 'UNKOWN':['-','Unknown']
                         }
 """
@@ -665,14 +667,40 @@
         + paths of all MagPy package dependencies.
 
 CALLED BY:
         Path to magpy packages that call this part, e.g. magpy.bin.acquisition
 
 *********************************************************************
     """
+    
+    KEYLIST = [ 'time',         # Timestamp (date2num object)
+                'x',            # X or I component of magnetic field (float)
+                'y',            # Y or D component of magnetic field (float)
+                'z',            # Z component of magnetic field (float)
+                'f',            # Magnetic field strength (float)
+                't1',           # Temperature variable (e.g. ambient temp) (float)
+                't2',           # Secondary temperature variable (e.g. sensor temp) (float)
+                'var1',         # Extra variable #1 (float)
+                'var2',         # Extra variable #2 (float)
+                'var3',         # Extra variable #3 (float)
+                'var4',         # Extra variable #4 (float)
+                'var5',         # Extra variable #5 (float)
+                'dx',           # Errors in X (float)
+                'dy',           # Errors in Y (float)
+                'dz',           # Errors in Z (float)
+                'df',           # Errors in F (float)
+                'str1',         # Extra string variable #1 (str)
+                'str2',         # Extra string variable #2 (str)
+                'str3',         # Extra string variable #3 (str)
+                'str4',         # Extra string variable #4 (str)
+                'flag',         # Variable for flags. (str='0000000000000000-')
+                'comment',      # Space for comments on flags (str)
+                'typ',          # Type of data (str='xyzf')
+                'sectime'       # Secondary time variable (date2num)
+                ]
 
     def __init__(self, container=None, header={},ndarray=None):
         if container is None:
             container = []
         self.container = container
         if ndarray is None:
             ndarray = np.array([np.asarray([]) for elem in KEYLIST])
@@ -707,15 +735,18 @@
 
     def length(self):
         #try:
         if len(self.ndarray[0]) > 0:
             ll = [len(elem) for elem in self.ndarray]
             return ll
         else:
-            return [len(self)]
+            if len(self) == 1 and np.isnan(self[0].time):
+                return [0]
+            else:
+                return [len(self)]
 
     def replace(self, datlst):
         # Replace in stream
         # - replace value with existing data
         # Method was used by K calc - replaced by internal method there
         newself = DataStream()
         assert isinstance(self.container, (list, tuple))
@@ -773,16 +804,22 @@
 
     def __str__(self):
         return str(self.container)
 
     def __repr__(self):
         return str(self.container)
 
-    def __getitem__(self, index):
-        return self.container.__getitem__(index)
+    def __getitem__(self, var):
+        try:
+            return self.ndarray[self.KEYLIST.index(var)]
+        except:
+            return self.container.__getitem__(var)
+        
+    def __setitem__(self, var, value):
+        self.ndarray[self.KEYLIST.index(var)] = value
 
     def __len__(self):
         return len(self.container)
 
     def clear_header(self):
         """
         Remove header information
@@ -907,20 +944,20 @@
                         retindex = indexes[0]
                     #print("Findtime index:",retindex)
                     return retindex, LineStruct()
                 else:
                     return 0, []
                 #return list(self.ndarray[0]).index(st), LineStruct()
             except:
-                loggerstream.warning("findtime: Didn't find selected time - returning 0")
+                logger.warning("findtime: Didn't find selected time - returning 0")
                 return 0, []
         for index, line in enumerate(self):
             if line.time == st:
                 return index, line
-        loggerstream.warning("findtime: Didn't find selected time - returning 0")
+        logger.warning("findtime: Didn't find selected time - returning 0")
         return 0, []
 
     def _find_t_limits(self):
         """
         DEFINITION:
             Find start and end times in stream.
         RETURNS:
@@ -1072,16 +1109,16 @@
             #self.ndarray = self.ndarray[:, np.argsort(self.ndarray[0])] # does not work if some rows have a different length)
             ind =  np.argsort(self.ndarray[0])
             for i,el in enumerate(self.ndarray):
                 if len(el) == len(ind):
                     self.ndarray[i] = el[ind]
                 else:
                     print("Sorting: key %s has the wrong length - replacing row with NaNs" % KEYLIST[i])
-                    loggerstream.warning("Sorting: key %s has the wrong length - replacing row with NaNs" % KEYLIST[i])
-                    loggerstream.warning("len(t-axis)=%d len(%s)=%d" % (len(self.ndarray[0]), KEYLIST[i], len(self.ndarray[i])))
+                    logger.warning("Sorting: key %s has the wrong length - replacing row with NaNs" % KEYLIST[i])
+                    logger.warning("len(t-axis)=%d len(%s)=%d" % (len(self.ndarray[0]), KEYLIST[i], len(self.ndarray[i])))
                     self.ndarray[i] = np.empty(len(self.ndarray[0])) * np.nan
 
             self.ndarray = self.fillempty(self.ndarray,keylst)
             for idx,el in enumerate(self.ndarray):
                 self.ndarray[idx] = np.asarray(self.ndarray[idx]).astype(object)
         else:
             self.ndarray = self.ndarray
@@ -1264,19 +1301,19 @@
         - stream:       (DataStream) DataStream object.
 
     EXAMPLE:
         >>> data_stream._move_column('f', 'var1')
         '''
 
         if not key in KEYLIST:
-            loggerstream.error("_move_column: Column key %s not valid!" % key)
+            logger.error("_move_column: Column key %s not valid!" % key)
         if key == 'time':
-            loggerstream.error("_move_column: Cannot move time column!")
+            logger.error("_move_column: Cannot move time column!")
         if not put2key in KEYLIST:
-            loggerstream.error("_move_column: Column key %s (to move %s to) is not valid!" % (put2key,key))
+            logger.error("_move_column: Column key %s (to move %s to) is not valid!" % (put2key,key))
         if len(self.ndarray[0]) > 0:
             col = self._get_column(key)
             self =self._put_column(col,put2key)
             return self
 
         try:
             for i, elem in enumerate(self):
@@ -1289,18 +1326,18 @@
                     #exec('elem.'+key+' = "-"')
             try:
                 exec('self.header["col-%s"] = self.header["col-%s"]' % (put2key, key))
                 exec('self.header["unit-col-%s"] = self.header["unit-col-%s"]' % (put2key, key))
                 exec('self.header["col-%s"] = None' % (key))
                 exec('self.header["unit-col-%s"] = None' % (key))
             except:
-                loggerstream.error("_move_column: Error updating headers.")
-            loggerstream.info("_move_column: Column %s moved to column %s." % (key, put2key))
+                logger.error("_move_column: Error updating headers.")
+            logger.info("_move_column: Column %s moved to column %s." % (key, put2key))
         except:
-            loggerstream.error("_move_column: It's an error.")
+            logger.error("_move_column: It's an error.")
 
         return self
 
 
     def _drop_column(self,key):
         """
         remove a column of a Stream
@@ -1372,18 +1409,18 @@
 
         if divisor > 1.:
             for elem in self:
                 if count%divisor == 0.:
                     lst.append(elem)
                 count += 1.
         else:
-            loggerstream.warning("_reduce_stream: Stream size (%s) is already below pointlimit (%s)." % (size,pointlimit))
+            logger.warning("_reduce_stream: Stream size (%s) is already below pointlimit (%s)." % (size,pointlimit))
             return self
 
-        loggerstream.info("_reduce_stream: Stream size reduced from %s to %s points." % (size,len(lst)))
+        logger.info("_reduce_stream: Stream size reduced from %s to %s points." % (size,len(lst)))
 
         return DataStream(lst, self.header)
 
 
     def _remove_nancolumns(self):
         """
     DEFINITION:
@@ -1419,15 +1456,15 @@
     # ------------------------------------------------------------------------
 
     def _aic(self, signal, k, debugmode=None):
         try:
             aicval = (k-1)* np.log(np.var(signal[:k]))+(len(signal)-k-1)*np.log(np.var(signal[k:]))
         except:
             if debugmode:
-                loggerstream.debug('_AIC: could not evaluate AIC at index position %i' % (k))
+                logger.debug('_AIC: could not evaluate AIC at index position %i' % (k))
             pass
         return aicval
 
 
     def harmfit(self,nt, val, fitdegree):
         # method for harminic fit according to Phil McFadden's fortran program
         """
@@ -2101,57 +2138,57 @@
         #self.header['DataAbsFunc'] = fitfunc
         #self.header['DataAbsDegree'] = fitdegree
         #self.header['DataAbsKnots'] = knotstep
         #self.header['DataAbsDate'] = datetime.strftime(datetime.utcnow(),'%Y-%m-%d %H:%M:%S')
 
         usestepinbetween = False # for better extrapolation
 
-        loggerstream.info(' --- Start baseline-correction at %s' % str(datetime.now()))
+        logger.info(' --- Start baseline-correction at %s' % str(datetime.now()))
 
         absolutestream  = absolutedata.copy()
 
         #print("Baseline", absolutestream.length())
         absolutestream = absolutestream.remove_flagged()
         #print("Baseline", absolutestream.length())
         #print("Baseline", absolutestream.ndarray[0])
 
         absndtype = False
         if len(absolutestream.ndarray[0]) > 0:
             absolutestream.ndarray[0] = absolutestream.ndarray[0].astype(float)
             absndtype = True
             if not np.min(absolutestream.ndarray[0]) < endtime:
-                loggerstream.warning("Baseline: Last measurement prior to beginning of absolute measurements ")
+                logger.warning("Baseline: Last measurement prior to beginning of absolute measurements ")
             abst = absolutestream.ndarray[0]
             if not startabs or startabs < np.min(absolutestream.ndarray[0]):
                 startabs = np.min(absolutestream.ndarray[0])
             if not endabs or endabs > np.max(absolutestream.ndarray[0]):
                 endabs = np.max(absolutestream.ndarray[0])
         else:
             # 1) test whether absolutes are in the selected absolute data stream
             if absolutestream[0].time == 0 or absolutestream[0].time == float('nan'):
                 raise ValueError ("Baseline: Input stream needs to contain absolute data ")
             # 2) check whether enddate is within abs time range or larger:
             if not absolutestream[0].time-1 < endtime:
-                loggerstream.warning("Baseline: Last measurement prior to beginning of absolute measurements ")
+                logger.warning("Baseline: Last measurement prior to beginning of absolute measurements ")
             abst = absolutestream._get_column('time')
             startabs = absolutestream[0].time
             endabs = absolutestream[-1].time
 
         # 3) check time ranges of stream and absolute values:
         if startabs > starttime:
-            #loggerstream.warning('Baseline: First absolute value measured after beginning of stream - duplicating first abs value at beginning of time series')
+            #logger.warning('Baseline: First absolute value measured after beginning of stream - duplicating first abs value at beginning of time series')
             #absolutestream.add(absolutestream[0])
             #absolutestream[-1].time = starttime
             #absolutestream.sorting()
-            loggerstream.info('Baseline: %d days without absolutes at the beginning of the stream' % int(np.floor(np.min(abst)-starttime)))
+            logger.info('Baseline: %d days without absolutes at the beginning of the stream' % int(np.floor(np.min(abst)-starttime)))
         if endabs < endtime:
-            loggerstream.info("Baseline: Last absolute measurement before end of stream - extrapolating baseline")
+            logger.info("Baseline: Last absolute measurement before end of stream - extrapolating baseline")
             if num2date(endabs).replace(tzinfo=None) + timedelta(days=extradays) < num2date(endtime).replace(tzinfo=None):
                 usestepinbetween = True
-                loggerstream.warning("Baseline: Well... thats an adventurous extrapolation, but as you wish...")
+                logger.warning("Baseline: Well... thats an adventurous extrapolation, but as you wish...")
 
         starttime = num2date(starttime).replace(tzinfo=None)
         endtime = num2date(endtime).replace(tzinfo=None)
 
         # 4) get standard time rang of one year and extradays at start and end
         #           test whether absstream covers this time range including extradays
         # ###########
@@ -2233,15 +2270,15 @@
         #self.header['DataAbsMinTime'] = func[1] #num2date(func[1]).replace(tzinfo=None)
         #self.header['DataAbsMaxTime'] = func[2] #num2date(func[2]).replace(tzinfo=None)
         #self.header['DataAbsFunctionObject'] = func
 
         #else:
         #    self = self.func_add(func)
 
-        loggerstream.info(' --- Finished baseline-correction at %s' % str(datetime.now()))
+        logger.info(' --- Finished baseline-correction at %s' % str(datetime.now()))
 
         for key in self.header:
             if key.startswith('DataAbs'):
                 print(key, self.header[key])
 
         return func
 
@@ -2646,31 +2683,31 @@
         offset = kwargs.get('offset')
         skipdelta = kwargs.get('skipdelta')
 
         if not offset:
             offset = [0,0,0]
         else:
             if not len(offset) == 3:
-                loggerstream.error('calc_f: offset with wrong dimension given - needs to contain a three dim array like [a,b,c] - returning stream without changes')
+                logger.error('calc_f: offset with wrong dimension given - needs to contain a three dim array like [a,b,c] - returning stream without changes')
                 return self
 
         ndtype = False
         try:
             if len(self.ndarray[0]) > 0:
                 ndtype = True
             elif len(self) > 1:
                 ndtype = False
             else:
-                loggerstream.error('calc_f: empty stream - aborting')
+                logger.error('calc_f: empty stream - aborting')
                 return self
         except:
-            loggerstream.error('calc_f: inapropriate data provided - aborting')
+            logger.error('calc_f: inapropriate data provided - aborting')
             return self
 
-        loggerstream.info('calc_f: --- Calculating f started at %s ' % str(datetime.now()))
+        logger.info('calc_f: --- Calculating f started at %s ' % str(datetime.now()))
 
         if ndtype:
             inddf = KEYLIST.index('df')
             indf = KEYLIST.index('f')
             indx = KEYLIST.index('x')
             indy = KEYLIST.index('y')
             indz = KEYLIST.index('z')
@@ -2685,15 +2722,15 @@
         else:
             for elem in self:
                 elem.f = np.sqrt((elem.x+offset[0])**2+(elem.y+offset[1])**2+(elem.z+offset[2])**2)
 
         self.header['col-f'] = 'f'
         self.header['unit-col-f'] = 'nT'
 
-        loggerstream.info('calc_f: --- Calculating f finished at %s ' % str(datetime.now()))
+        logger.info('calc_f: --- Calculating f finished at %s ' % str(datetime.now()))
 
         return self
 
 
     def dailymeans(self, keys=['x','y','z','f'], **kwargs):
         """
     DEFINITION:
@@ -2802,15 +2839,15 @@
 
         for elem in self:
             newtime = num2date(elem.time).replace(tzinfo=None) + offset
             elem.sectime = elem.time
             elem.time = date2num(newtime)
             newstream.add(elem)
 
-        loggerstream.info('date_offset: Corrected time column by %s sec' % str(offset.total_seconds))
+        logger.info('date_offset: Corrected time column by %s sec' % str(offset.total_seconds))
 
         return DataStream(newstream,header,array)
 
 
     def delta_f(self, **kwargs):
         """
         DESCRIPTION:
@@ -2829,15 +2866,15 @@
         offset = kwargs.get('offset')
         digits = kwargs.get('digits')
         if not offset:
             offset = 0
         if not digits:
             digits = 8
 
-        loggerstream.info('--- Calculating delta f started at %s ' % str(datetime.now()))
+        logger.info('--- Calculating delta f started at %s ' % str(datetime.now()))
 
         try:
             syst = self.header['DataComponents']
         except:
             syst = None
 
 
@@ -2860,15 +2897,15 @@
         else:
             for elem in self:
                 elem.df = round(np.sqrt(elem.x**2+elem.y**2+elem.z**2),digits) - (elem.f + offset)
 
         self.header['col-df'] = 'delta f'
         self.header['unit-col-df'] = 'nT'
 
-        loggerstream.info('--- Calculating delta f finished at %s ' % str(datetime.now()))
+        logger.info('--- Calculating delta f finished at %s ' % str(datetime.now()))
 
         return self
 
 
     def f_from_df(self, **kwargs):
         """
         DESCRIPTION:
@@ -2887,15 +2924,15 @@
         offset = kwargs.get('offset')
         digits = kwargs.get('digits')
         if not offset:
             offset = 0.
         if not digits:
             digits = 8
 
-        loggerstream.info('--- Calculating f started at %s ' % str(datetime.now()))
+        logger.info('--- Calculating f started at %s ' % str(datetime.now()))
 
         try:
             syst = self.header['DataComponents']
         except:
             syst = None
 
 
@@ -2918,15 +2955,15 @@
         else:
             for elem in self:
                 elem.f = round(np.sqrt(elem.x**2+elem.y**2+elem.z**2),digits) - (elem.df + offset)
 
         self.header['col-f'] = 'f'
         self.header['unit-col-f'] = 'nT'
 
-        loggerstream.info('--- Calculating f finished at %s ' % str(datetime.now()))
+        logger.info('--- Calculating f finished at %s ' % str(datetime.now()))
 
         return self
 
 
     def differentiate(self, **kwargs):
         """
     DEFINITION:
@@ -2947,25 +2984,25 @@
 
     EXAMPLE:
         >>> stream = stream.differentiate(keys=['f'],put2keys=['df'])
 
     APPLICATION:
         """
 
-        loggerstream.info('differentiate: Calculating derivative started.')
+        logger.info('differentiate: Calculating derivative started.')
 
         keys = kwargs.get('keys')
         put2keys = kwargs.get('put2keys')
         if not keys:
             keys = ['x','y','z','f']
         if not put2keys:
             put2keys = ['dx','dy','dz','df']
 
         if len(keys) != len(put2keys):
-            loggerstream.error('Amount of columns read must be equal to outputcolumns')
+            logger.error('Amount of columns read must be equal to outputcolumns')
             return self
 
         stream = self.copy()
 
         ndtype = False
         if len(stream.ndarray[0]) > 0:
             t = stream.ndarray[0].astype(float)
@@ -2979,15 +3016,15 @@
                 val = stream.ndarray[ind].astype(float)
             else:
                 val = stream._get_column(key)
             dval = np.gradient(np.asarray(val))
             stream._put_column(dval, put2keys[i])
             stream.header['col-'+put2keys[i]] = r"d%s vs dt" % (key)
 
-        loggerstream.info('--- derivative obtained at %s ' % str(datetime.now()))
+        logger.info('--- derivative obtained at %s ' % str(datetime.now()))
         return stream
 
 
     def DWT_calc(self,key='x',wavelet='db4',level=3,plot=False,outfile=None,
                 window=5):
         """
     DEFINITION:
@@ -3062,15 +3099,15 @@
         array = [[] for key in KEYLIST]
         x_ind = KEYLIST.index('x')
         dx_ind = KEYLIST.index('dx')
         var1_ind = KEYLIST.index('var1')
         var2_ind = KEYLIST.index('var2')
         var3_ind = KEYLIST.index('var3')
         i = 0
-        loggerstream.info("DWT_calc: Starting Discrete Wavelet Transform of key %s." % key)
+        logger.info("DWT_calc: Starting Discrete Wavelet Transform of key %s." % key)
 
         # 1b. Loop for sliding window
         while True:
             if i >= (len(data)-window):
                 break
 
             #row = LineStruct()
@@ -3115,29 +3152,29 @@
             array[var1_ind].append(fin_fns[3])
             array[var2_ind].append(fin_fns[2])
             array[var3_ind].append(fin_fns[1])
 
             #DWT_stream.add(row)
             i += window
 
-        loggerstream.info("DWT_calc: Finished DWT.")
+        logger.info("DWT_calc: Finished DWT.")
 
         DWT_stream.header['col-x'] = 'A3'
         DWT_stream.header['unit-col-x'] = 'nT^2'
         DWT_stream.header['col-var1'] = 'D1'
         DWT_stream.header['unit-col-var1'] = 'nT^2'
         DWT_stream.header['col-var2'] = 'D2'
         DWT_stream.header['unit-col-var2'] = 'nT^2'
         DWT_stream.header['col-var3'] = 'D3'
         DWT_stream.header['unit-col-var3'] = 'nT^2'
 
         # Plot stream:
         if plot == True:
-            date = datetime.strftime(num2date(self[0].time),'%Y-%m-%d')
-            loggerstream.info('DWT_calc: Plotting data...')
+            date = datetime.strftime(num2date(self.ndarray[0][0]),'%Y-%m-%d')
+            logger.info('DWT_calc: Plotting data...')
             if outfile:
                 DWT_stream.plot(['x','var1','var2','var3'],
                                 plottitle="DWT Decomposition of %s (%s)" % (key,date),
                                 outfile=outfile)
             else:
                 DWT_stream.plot(['x','var1','var2','var3'],
                                 plottitle="DWT Decomposition of %s (%s)" % (key,date))
@@ -3174,22 +3211,22 @@
         st.eventlogger(['var3'],[15,20,30],'>')
         """
         assert type(values) == list
 
         if not compare:
             compare = '=='
         if not compare in ['<','>','<=','>=','==','!=']:
-            loggerstream.warning('Eventlogger: wrong value for compare: needs to be among <,>,<=,>=,==,!=')
+            logger.warning('Eventlogger: wrong value for compare: needs to be among <,>,<=,>=,==,!=')
             return self
         if not stringvalues:
             stringvalues = ['Minor storm onset','Moderate storm onset','Major storm onset']
         else:
             assert type(stringvalues) == list
         if not len(stringvalues) == len(values):
-            loggerstream.warning('Eventlogger: Provided comments do not match amount of values')
+            logger.warning('Eventlogger: Provided comments do not match amount of values')
             return self
 
         for elem in self:
             #evaluationstring = 'elem.' + key + ' ' + compare + ' ' + str(values[0])
             if eval('elem.'+key+' '+compare+' '+str(values[2])):
                 stormlogger.warning('%s at %s' % (stringvalues[2],num2date(elem.time).replace(tzinfo=None)))
                 if addcomment:
@@ -3238,15 +3275,15 @@
             >>> extractedstream = stream.extract('x',20000,'>')
             >>> extractedstream = stream.extract('str1','Berger')
         """
 
         if not compare:
             compare = '=='
         if not compare in [">=", "<=",">", "<", "==", "!=", 'like']:
-            loggerstream.info('--- Extract: Please provide proper compare parameter ">=", "<=",">", "<", "==", "like" or "!=" ')
+            logger.info('--- Extract: Please provide proper compare parameter ">=", "<=",">", "<", "==", "like" or "!=" ')
             return self
 
         if value in ['',None]:
             return self
 
         ndtype = False
         if len(self.ndarray[0]) > 0:
@@ -3254,15 +3291,15 @@
 
         ind = KEYLIST.index(key)
 
         stream = self.copy()
 
         if not self._is_number(value):
             if value.startswith('(') and value.endswith(')') and compare == '==':
-                loggerstream.info("extract: Selected special functional type -equality defined by difference less then 10 exp-6")
+                logger.info("extract: Selected special functional type -equality defined by difference less then 10 exp-6")
                 if ndtype:
                     val = eval(value[1:-1])
                     indexar = np.where((np.abs(stream.ndarray[ind]-val)) < 0.000001)[0]
                 else:
                     val = value[1:-1]
                     liste = []
                     for elem in self:
@@ -3570,21 +3607,21 @@
 
         ndtype = False
 
         # ########################
         # Basic validity checks and window size definitions
         # ########################
         if not filter_type in filterlist:
-            loggerstream.error("smooth: Window is none of 'flat', 'hanning', 'hamming', 'bartlett', 'blackman', etc")
-            loggerstream.debug("smooth: You entered non-existing filter type -  %s  - " % filter_type)
+            logger.error("smooth: Window is none of 'flat', 'hanning', 'hamming', 'bartlett', 'blackman', etc")
+            logger.debug("smooth: You entered non-existing filter type -  %s  - " % filter_type)
             return self
 
         #print self.length()[0]
         if not self.length()[0] > 1:
-            loggerstream.error("Filter: stream needs to contain data - returning.")
+            logger.error("Filter: stream needs to contain data - returning.")
             return self
 
         if debugmode:
             print("Starting length:", self.length())
 
         #if not dontfillgaps:   ### changed--- now using dont fill gaps as default
         if fillgaps:
@@ -3619,15 +3656,15 @@
         else:
             window_len = np.round(window_period/sampling_period)
             if window_len % 2:
                 window_len = window_len+1
             trange = window_period/2
 
         if sampling_period >= window_period:
-            loggerstream.warning("Filter: Sampling period is equal or larger then projected filter window - returning.")
+            logger.warning("Filter: Sampling period is equal or larger then projected filter window - returning.")
             return self
 
         # ########################
         # Reading data of each selected column in stream
         # ########################
 
         if len(self.ndarray[0])>0:
@@ -3638,15 +3675,15 @@
 
         if debugmode:
             print("Length time column:", len(t))
 
         for key in keys:
             #print "Start filtering for", key
             if not key in KEYLIST:
-                loggerstream.error("Column key %s not valid." % key)
+                logger.error("Column key %s not valid." % key)
             keyindex = KEYLIST.index(key)
             if len(self.ndarray[keyindex])>0:
                 v = self.ndarray[keyindex]
             else:
                 v = self._get_column(key)
 
             # INTERMAGNET 90 percent rule: interpolate missing values if less than 10 percent are missing
@@ -3659,25 +3696,25 @@
                     else:
                         fill = 'mean'
                 except:
                     fill = 'mean'
                 v = self.missingvalue(v,np.round(window_period/sampling_period),fill=fill) # using ratio here and not _len
 
             if key in autofill:
-                loggerstream.warning("Filter: key %s has been selected for linear interpolation before filtering." % key)
-                loggerstream.warning("Filter: I guess you know what you are doing...")
+                logger.warning("Filter: key %s has been selected for linear interpolation before filtering." % key)
+                logger.warning("Filter: I guess you know what you are doing...")
                 nans, x= nan_helper(v)
                 v[nans]= interp(x(nans), x(~nans), v[~nans])
 
             # Make sure that we are dealing with numbers
             v = np.array(list(map(float, v)))
             if v.ndim != 1:
-                loggerstream.error("Filter: Only accepts 1 dimensional arrays.")
+                logger.error("Filter: Only accepts 1 dimensional arrays.")
             if window_len<3:
-                loggerstream.error("Filter: Window lenght defined by filter_width needs to cover at least three data points")
+                logger.error("Filter: Window lenght defined by filter_width needs to cover at least three data points")
 
             if debugmode:
                 print("Treating k:", key, v.size)
 
             if v.size >= window_len:
                 s=np.r_[v[window_len-1:0:-1],v,v[-1:-window_len:-1]]
 
@@ -3864,40 +3901,40 @@
                 try:
                     #print val, sp, knotstep
                     knots = np.array(arange(np.min(nt)+knotstep,np.max(nt)-knotstep,knotstep))
                     #print knots, len(knots), len(val)
                     if len(knots) > len(val):
                         knotstep = knotstep*4
                         knots = np.array(arange(np.min(nt)+knotstep,np.max(nt)-knotstep,knotstep))
-                        loggerstream.warning('Too many knots in spline for available data. Please check amount of fitted data in time range. Trying to reduce resolution ...')
+                        logger.warning('Too many knots in spline for available data. Please check amount of fitted data in time range. Trying to reduce resolution ...')
                     #print nt, len(knots), len(val)
                     ti = interpolate.splrep(nt, val, k=3, s=0, t=knots)
                 except:
-                    loggerstream.error('Value error in fit function - likely reason: no valid numbers or too few numbers for fit')
+                    logger.error('Value error in fit function - likely reason: no valid numbers or too few numbers for fit')
                     raise ValueError("Value error in fit function - not enough data or invalid numbers")
                     return
                 #print nt, val, len(knots), knots
                 #ti = interpolate.interp1d(nt, val, kind='cubic')
                 #print "X", x, np.min(nt),np.max(nt),sp
                 #print "TI", ti
                 f_fit = interpolate.splev(x,ti)
             elif len(val)>1 and fitfunc == 'poly':
-                loggerstream.debug('Selected polynomial fit - amount of data: %d, time steps: %d, degree of fit: %d' % (len(nt), len(val), fitdegree))
+                logger.debug('Selected polynomial fit - amount of data: %d, time steps: %d, degree of fit: %d' % (len(nt), len(val), fitdegree))
                 ti = polyfit(nt, val, fitdegree)
                 f_fit = polyval(ti,x)
             elif len(val)>1 and fitfunc == 'harmonic':
-                loggerstream.debug('Selected harmonic fit - using inverse fourier transform')
+                logger.debug('Selected harmonic fit - using inverse fourier transform')
                 f_fit = self.harmfit(nt, val, fitdegree)
                 # Don't use resampled list for harmonic time series
                 x = nt
             elif len(val)<=1:
-                loggerstream.warning('Fit: No valid data')
+                logger.warning('Fit: No valid data')
                 return
             else:
-                loggerstream.warning('Fit: function not valid')
+                logger.warning('Fit: function not valid')
                 return
             exec('f'+key+' = interpolate.interp1d(x, f_fit, bounds_error=False)')
             exec('functionkeylist["f'+key+'"] = f'+key)
 
         if tok:
             func = [functionkeylist, sv, ev]
         else:
@@ -4261,19 +4298,19 @@
 
         # Position of flag in flagstring
         # f (intensity): pos 0
         # x,y,z (vector): pos 1
         # other (vector): pos 2
 
         if not len(self.ndarray[0]) > 0:
-            loggerstream.info('flag_outlier: No ndarray - starting remove_outlier.')
+            logger.info('flag_outlier: No ndarray - starting remove_outlier.')
             self = self.remove_outlier(keys=keys,threshold=threshold,timerange=timerange,stdout=stdout,markall=markall)
             return self
 
-        loggerstream.info('flag_outlier: Starting outlier removal.')
+        logger.info('flag_outlier: Starting outlier removal.')
 
         flagidx = KEYLIST.index('flag')
         commentidx = KEYLIST.index('comment')
         if not len(self.ndarray[flagidx]) > 0:
             self.ndarray[flagidx] = [''] * len(self.ndarray[0])
         else:
             self.ndarray[flagidx] = self.ndarray[flagidx].astype(object)
@@ -4322,15 +4359,15 @@
                     whisker = threshold*iqd
                     #print key, md, iqd, whisker
                 except:
                     try:
                         md = np.median(selcol)
                         whisker = md*0.005
                     except:
-                        loggerstream.warning("remove_outlier: Eliminate outliers produced a problem: please check.")
+                        logger.warning("remove_outlier: Eliminate outliers produced a problem: please check.")
                         pass
 
                 #print md, whisker, np.asarray(selcol)
                 for elem in range(idxst,idxat):
                     #print flagpos, elem
                     if not md-whisker < self.ndarray[flagpos][elem] < md+whisker and not np.isnan(self.ndarray[flagpos][elem]):
                         #print "Found:", key, self.ndarray[flagpos][elem]
@@ -4366,15 +4403,15 @@
                             newflag = ''.join(newflagls)
 
                         self.ndarray[flagidx][elem] = newflag
                         #print self.ndarray[flagidx][elem]
                         commline = "aof - threshold: {a}, window: {b} sec".format(a=str(threshold), b=str(timerange.total_seconds()))
                         self.ndarray[commentidx][elem] = commline
                         infoline = "flag_outlier: at {a} - removed {b} (= {c})".format(a=str(self.ndarray[0][elem]), b=key, c=self.ndarray[flagpos][elem])
-                        loggerstream.info(infoline)
+                        logger.info(infoline)
                         #[starttime,endtime,key,flagid,flagcomment]
                         flagtime = self.ndarray[0][elem]
                         flaglist.append([flagtime,flagtime,key,1,commline])
                         if stdout:
                             print(infoline)
                     else:
                         try:
@@ -4385,15 +4422,15 @@
                         except:
                             self.ndarray[flagidx][elem] = ''
                             self.ndarray[commentidx][elem] = ''
 
         self.ndarray[flagidx] = np.asarray(self.ndarray[flagidx])
         self.ndarray[commentidx] = np.asarray(self.ndarray[commentidx])
 
-        loggerstream.info('flag_outlier: Outlier flagging finished.')
+        logger.info('flag_outlier: Outlier flagging finished.')
 
         ## METHOD WHICH SORTS/COMBINES THE FLAGLIST
         #print("flag_outlier",flaglist)
         newlist = []
         srday = sr/(3600.*24.)
         for line in flaglist:
             ft = line[0]
@@ -4726,18 +4763,18 @@
 
         sr = samplingrate
 
         #t1 = datetime.utcnow()
         #print("starting flag_stream method at",t1)
 
         if not key in KEYLIST:
-            loggerstream.error("flag_stream: %s is not a valid key." % key)
+            logger.error("flag_stream: %s is not a valid key." % key)
             return self
         if not flag in [0,1,2,3,4]:
-            loggerstream.error("flag_stream: %s is not a valid flag." % flag)
+            logger.error("flag_stream: %s is not a valid flag." % flag)
             return self
 
         ndtype = False
         if len(self.ndarray[0]) > 0:
             ndtype = True
         elif not len(self) > 0:
             return DataStream()
@@ -4748,15 +4785,15 @@
             # Set enddate to startdat
             # Hereby flag nearest might be used later
             enddate = startdate
             """
             start = date2num(startdate)
             check_startdate, val = self.findtime(start)
             if check_startdate == 0:
-                loggerstream.info("flag_stream: No data at given date for flag. Finding nearest data point.")
+                logger.info("flag_stream: No data at given date for flag. Finding nearest data point.")
                 if ndtype:
                     time = self.ndarray[0]
                 else:
                     time = self._get_column('time')
                 #print start, len(time)
                 new_endtime, index = find_nearest(time, start)
                 if new_endtime > start:
@@ -4913,20 +4950,20 @@
                     fllist[pos] = str(flag)
                     elem.flag=''.join(fllist)
                     elem.comment = comment
         if flag == 1 or flag == 3:
             if enddate:
                 #print ("flag_stream: Flagged data from %s to %s -> (%s)" % (startdate.isoformat(),enddate.isoformat(),comment))
                 try:
-                    loggerstream.info("flag_stream: Flagged data from %s to %s -> (%s)" % (startdate.isoformat().encode('ascii','ignore'),enddate.isoformat().encode('ascii','ignore'),comment.encode('ascii','ignore')))
+                    logger.info("flag_stream: Flagged data from %s to %s -> (%s)" % (startdate.isoformat().encode('ascii','ignore'),enddate.isoformat().encode('ascii','ignore'),comment.encode('ascii','ignore')))
                 except:
                     pass
             else:
                 try:
-                    loggerstream.info("flag_stream: Flagged data at %s -> (%s)" % (startdate.isoformat().encode('ascii','ignore'),comment.encode('ascii','ignore')))
+                    logger.info("flag_stream: Flagged data at %s -> (%s)" % (startdate.isoformat().encode('ascii','ignore'),comment.encode('ascii','ignore')))
                 except:
                     pass
 
         #print self.ndarray[flagind][np.where(self.ndarray[flagind] != '')]
         #print self.ndarray[flagind]
         #t1 = datetime.utcnow()
         #print("Finished flag",t1)
@@ -5226,15 +5263,15 @@
         if not accuracy:
             accuracy = 0.9/(3600.0*24.0) # one second relative to day
             accuracy = 0.05*newsp # 5 percent of samplingrate
 
         if newsps < 0.9 and not accuracy:
             accuracy = (newsps-(newsps*0.1))/(3600.0*24.0)
 
-        loggerstream.info('--- Starting filling gaps with NANs at %s ' % (str(datetime.now())))
+        logger.info('--- Starting filling gaps with NANs at %s ' % (str(datetime.now())))
 
         stream = self.copy()
         prevtime = 0
 
         ndtype = False
         if len(stream.ndarray[0]) > 0:
             maxtime = stream.ndarray[0][-1]
@@ -5255,28 +5292,28 @@
             # Get time diff and expected count
             timediff = maxtime - mintime
             expN = int(round(timediff/newsp))+1
             if debug:
                 print("Expected length vs actual length:", expN, length)
             if expN == len(sourcetime):
                 # Found the expected amount of time steps - no gaps
-                loggerstream.info("get_gaps: No gaps found - Returning")
+                logger.info("get_gaps: No gaps found - Returning")
                 return stream
             else:
                 # correct way (will be used by default) - does not use any accuracy value
                 #projtime = np.linspace(mintime, maxtime, num=expN, endpoint=True)
                 #print("proj:", projtime, len(projtime))
                 # find values or projtime, which are not in sourcetime
                 #dif = setdiff1d(projtime,sourcetime, assume_unique=True)
                 #print (dif, len(dif))
                 #print (len(dif),len(sourcetime),len(projtime))                
                 diff = sourcetime[1:] - sourcetime[:-1]
                 num_fills = np.round(diff / newsp) - 1
                 getdiffids = np.where(diff > newsp+accuracy)[0]
-                loggerstream.info("get_gaps: Found gaps - Filling nans to them")
+                logger.info("get_gaps: Found gaps - Filling nans to them")
                 if debug:
                     print ("Here", diff, num_fills, newsp, getdiffids)
                 missingt = []
                 # Get critical differences and number of missing steps 
                 for i in getdiffids:
                     #print (i,  sourcetime[i-1], sourcetime[i], sourcetime[i+1])
                     nf = num_fills[i]
@@ -5328,15 +5365,15 @@
                     exec('elem.'+gapvariable+' = 0.0')
                     if key in KEYLIST:
                         if isnan(eval('elem.'+key)):
                             exec('elem.'+gapvariable+' = 1.0')
                     stream.add(elem)
                 prevtime = elem.time
 
-        loggerstream.info('--- Filling gaps finished at %s ' % (str(datetime.now())))
+        logger.info('--- Filling gaps finished at %s ' % (str(datetime.now())))
         if debugmode:
             print("Ending:", stream[0].time, stream[-1].time)
 
         return stream.sorting()
 
 
     def get_rotationangle(self, xcompensation=0,keys=['x','y','z'],**kwargs):
@@ -5355,18 +5392,18 @@
 
         #1. get vector from data
         # x = y*tan(dec)
         if not keys:
             keys = ['x','y','z']
 
         if not len(keys) == 3:
-            loggerstream.error('get_rotation: provided keylist need to have three components.')
+            logger.error('get_rotation: provided keylist need to have three components.')
             return stream #self
 
-        loggerstream.info('get_rotation: Determining rotation angle towards a magnetic coordinate system assuming z to be vertical down.')
+        logger.info('get_rotation: Determining rotation angle towards a magnetic coordinate system assuming z to be vertical down.')
 
         ind1 = KEYLIST.index(keys[0])
         ind2 = KEYLIST.index(keys[1])
         ind3 = KEYLIST.index(keys[2])
 
         if len(self.ndarray[0]) > 0:
             if len(self.ndarray[ind1]) > 0 and len(self.ndarray[ind2]) > 0 and len(self.ndarray[ind3]) > 0:
@@ -5379,15 +5416,15 @@
                     meanx = np.mean(xl)+xcompensation
                 meany = np.mean(yl)
                 # get rotation angle so that meany == 0
                 #zeroy = meanx*np.sin(ra)+meany*np.cos(ra)
                 #-meany/meanx = np.tan(ra)
                 rotangle = np.arctan2(-meany,meanx) * (180.) / np.pi
 
-        loggerstream.info('getrotation: Rotation angle determined: {} deg'.format(rotangle))
+        logger.info('getrotation: Rotation angle determined: {} deg'.format(rotangle))
 
         return rotangle
 
 
     def get_sampling_period(self):
         """
         returns the dominant sampling frequency in unit ! days !
@@ -5440,24 +5477,24 @@
 
         #print self
         if not len(timedifflist) == 0:
             timedifflist.sort(key=lambda x: int(x[0]))
             # get the most often found timediff
             domtd = timedifflist[-1][1]
         else:
-            loggerstream.error("get_sampling_period: unkown problem - returning 0")
+            logger.error("get_sampling_period: unkown problem - returning 0")
             domtd = 0
 
         if not domtd == 0:
             return domtd
         else:
             try:
                 return timedifflist[-2][1]
             except:
-                loggerstream.error("get_sampling_period: could not identify dominant sampling rate")
+                logger.error("get_sampling_period: could not identify dominant sampling rate")
                 return 0
         """
 
     def samplingrate(self, **kwargs):
         """
         DEFINITION:
             returns a rounded value of the sampling rate
@@ -5523,15 +5560,15 @@
             -- Using scipy.integrate.cumtrapz
         VARIABLES:
             optional:
             keys: (list - default ['x','y','z','f'] provide limited key-list
         """
 
 
-        loggerstream.info('--- Integrating started at %s ' % str(datetime.now()))
+        logger.info('--- Integrating started at %s ' % str(datetime.now()))
 
         keys = kwargs.get('keys')
         if not keys:
             keys = ['x','y','z']
 
         array = [[] for key in KEYLIST]
         ndtype = False
@@ -5553,15 +5590,15 @@
             if ndtype:
                 ind = KEYLIST.index('d'+key)
                 array[ind] = np.asarray(dval)
             else:
                 self._put_column(dval, 'd'+key)
 
         self.ndarray = np.asarray(array)
-        loggerstream.info('--- integration finished at %s ' % str(datetime.now()))
+        logger.info('--- integration finished at %s ' % str(datetime.now()))
         return self
 
 
     def interpol(self, keys, **kwargs):
         """
     DEFINITION:
         Uses Numpy interpolate.interp1d to interpolate streams.
@@ -5597,32 +5634,32 @@
 
         kind = kwargs.get('kind')
 
         if not kind:
             kind = 'linear'
 
         if kind not in ['linear','slinear','quadratic','cubic','nearest','zero']:
-            loggerstream.warning("interpol: Interpolation kind %s not valid. Using linear interpolation instead." % kind)
+            logger.warning("interpol: Interpolation kind %s not valid. Using linear interpolation instead." % kind)
             kind = 'linear'
 
         ndtype = False
         if len(self.ndarray[0]) > 0:
             t = self.ndarray[0]
             ndtype = True
         else:
             t = self._get_column('time')
         nt,sv,ev = self._normalize(t)
         sp = self.get_sampling_period()
         functionkeylist = {}
 
-        loggerstream.info("interpol: Interpolating stream with %s interpolation." % kind)
+        logger.info("interpol: Interpolating stream with %s interpolation." % kind)
 
         for key in keys:
             if not key in NUMKEYLIST:
-                loggerstream.error("interpol: Column key not valid!")
+                logger.error("interpol: Column key not valid!")
             if ndtype:
                 ind = KEYLIST.index(key)
                 val = self.ndarray[ind].astype(float)
             else:
                 val = self._get_column(key)
             # interplolate NaN values
             nans, xxx= nan_helper(val)
@@ -5631,18 +5668,18 @@
             except:
                 #val[nans]=int(nan)
                 pass
             if len(val)>1:
                 exec('f'+key+' = interpolate.interp1d(nt, val, kind)')
                 exec('functionkeylist["f'+key+'"] = f'+key)
             else:
-                loggerstream.warning("interpol: interpolation of zero length data set - wont work.")
+                logger.warning("interpol: interpolation of zero length data set - wont work.")
                 pass
 
-        loggerstream.info("interpol: Interpolation complete.")
+        logger.info("interpol: Interpolation complete.")
 
         func = [functionkeylist, sv, ev]
 
         return func
 
     def k_extend(self, **kwargs):
         """
@@ -5762,15 +5799,15 @@
         # important: how to do that - what is the latitudinal relationship, how to transfer the scale,
         # it is frequently mentioned to be quasi-log but it is not a simple Log scale
         # func can be fitted reasonably well by
         # func[a_] := Exp[0.8308663199145958 + 0.7894060396483681 k -  0.021250627459823503 k^2]
 
         kstream = DataStream()
 
-        loggerstream.info('--- Starting k value calculation: %s ' % (str(datetime.now())))
+        logger.info('--- Starting k value calculation: %s ' % (str(datetime.now())))
 
         # Non destructive - using a coyp of the supplied stream
         stream = self.copy()
 
         # ############################################
         # ##           Step 1           ##############
         # ##   ------------------------ ##############
@@ -6373,24 +6410,24 @@
 
         ndtype = False
         if len(self.ndarray[0])>0:
             ndtype = True
         elif len(self) > 0:
             pass
         else:
-            loggerstream.error('mean: empty stream - aborting')
+            logger.error('mean: empty stream - aborting')
             if std:
                 return float("NaN"), float("NaN")
             else:
                 return float("NaN")
 
         if not isinstance( percentage, (int,long)):
-            loggerstream.error("mean: Percentage needs to be an integer!")
+            logger.error("mean: Percentage needs to be an integer!")
         if not key in KEYLIST[:16]:
-            loggerstream.error("mean: Column key not valid!")
+            logger.error("mean: Column key not valid!")
 
         if ndtype:
             ind = KEYLIST.index(key)
             length = len(self.ndarray[0])
             self.ndarray[ind] = np.asarray(self.ndarray[ind])
             ar = self.ndarray[ind].astype(float)
             ar = ar[~np.isnan(ar)]
@@ -6402,15 +6439,15 @@
         if div >= percentage:
             if std:
                 return eval('np.'+meanfunction+'(ar)'), np.std(ar)
             else:
                 return eval('np.'+meanfunction+'(ar)')
         else:
             print ('mean: Too many nans in column, exceeding %d percent' % percentage)
-            loggerstream.warning('mean: Too many nans in column, exceeding %d percent' % percentage)
+            logger.warning('mean: Too many nans in column, exceeding %d percent' % percentage)
             if std:
                 return float("NaN"), float("NaN")
             else:
                 return float("NaN")
 
     def missingvalue(self,v,window_len,threshold=0.9,fill='mean'):
         """
@@ -6528,15 +6565,15 @@
         var1_ind = KEYLIST.index('var1')
         var2_ind = KEYLIST.index('var2')
         var3_ind = KEYLIST.index('var3')
         var4_ind = KEYLIST.index('var4')
         var5_ind = KEYLIST.index('var5')
         dy_ind = KEYLIST.index('dy')
         i = 0
-        loggerstream.info("MODWT_calc: Starting Discrete Wavelet Transform of key %s." % key)
+        logger.info("MODWT_calc: Starting Discrete Wavelet Transform of key %s." % key)
 
         if len(data) % 2 == 1:
             data = data[0:-1]
 
         # Results have format:
         # (cAn, cDn), ..., (cA2, cD2), (cA1, cD1)
         coeffs = pywt.swt(data, wavelet, level)
@@ -6572,15 +6609,15 @@
                         key = 'dy'
                     elif j == 7:
                         key = 'dz'
                     array[KEYLIST.index(key)].append(sum(d_cut)/float(window))
                     
             i += window
 
-        loggerstream.info("MODWT_calc: Finished MODWT.")
+        logger.info("MODWT_calc: Finished MODWT.")
 
         MODWT_stream.header['col-x'] = 'A3'
         MODWT_stream.header['unit-col-x'] = 'nT^2'
         MODWT_stream.header['col-var1'] = 'D1'
         MODWT_stream.header['unit-col-var1'] = 'nT^2'
         MODWT_stream.header['col-var2'] = 'D2'
         MODWT_stream.header['unit-col-var2'] = 'nT^2'
@@ -6591,16 +6628,16 @@
         MODWT_stream.header['col-var5'] = 'D5'
         MODWT_stream.header['unit-col-var5'] = 'nT^2'
         MODWT_stream.header['col-dy'] = 'D6'
         MODWT_stream.header['unit-col-dy'] = 'nT^2'
 
         # Plot stream:
         if plot == True:
-            date = datetime.strftime(num2date(self[0].time),'%Y-%m-%d')
-            loggerstream.info('MODWT_calc: Plotting data...')
+            date = datetime.strftime(num2date(self.ndarray[0][0]),'%Y-%m-%d')
+            logger.info('MODWT_calc: Plotting data...')
             if outfile:
                 MODWT_stream.plot(['x','var1','var2','var3'],
                                 plottitle="MODWT Decomposition of %s (%s)" % (key,date),
                                 outfile=outfile)
             else:
                 MODWT_stream.plot(['x','var1','var2','var3'],
                                 plottitle="MODWT Decomposition of %s (%s)" % (key,date))
@@ -6641,28 +6678,28 @@
             if key in KEYLIST:
                 if ndtype:
                     ind = KEYLIST.index(key)
                     val = self.ndarray[ind]
                 else:
                     val = self._get_column(key)
                 if key == 'time':
-                    loggerstream.error("factor: Multiplying time? That's just plain silly.")
+                    logger.error("factor: Multiplying time? That's just plain silly.")
                 else:
                     if square == False:
                         newval = [elem * factors[key] for elem in val]
-                        loggerstream.info('factor: Multiplied column %s by %s.' % (key, factors[key]))
+                        logger.info('factor: Multiplied column %s by %s.' % (key, factors[key]))
                     else:
                         newval = [elem ** factors[key] for elem in val]
-                        loggerstream.info('factor: Multiplied column %s by %s.' % (key, factors[key]))
+                        logger.info('factor: Multiplied column %s by %s.' % (key, factors[key]))
                 if ndtype:
                     self.ndarray[ind] = np.asarray(newval)
                 else:
                     self = self._put_column(newval, key)
             else:
-                loggerstream.warning("factor: Key '%s' not in keylist." % key)
+                logger.warning("factor: Key '%s' not in keylist." % key)
 
         return self
 
 
     def obspyspectrogram(self, data, samp_rate, per_lap=0.9, wlen=None, log=False,
                     outfile=None, fmt=None, axes=None, dbscale=False,
                     mult=8.0, cmap=None, zorder=None, title=None, show=True,
@@ -6880,15 +6917,15 @@
         if len(self.ndarray[0]) > 0:
             ndtype =True
             tcol = self.ndarray[0]
         else:
             tcol = self._get_column('time')
 
         if not len(tcol) > 0:
-            loggerstream.error("offset: No data found - aborting")
+            logger.error("offset: No data found - aborting")
             return self
 
         stidx = 0
         edidx = len(tcol)
         if starttime:
             st = date2num(self._testtime(starttime))
             # get index number of first element >= starttime in timecol
@@ -6947,27 +6984,27 @@
                         except:
                             print("offset: error with time offset - check provided timedelta")
                             break
                     val = val + os
                     #print num2date(val[0]).replace(tzinfo=None)
                     #print num2date(val[0]).replace(tzinfo=None) + offsets[key]
                     #newval = [date2num(num2date(elem).replace(tzinfo=None) + offsets[key]) for elem in val]
-                    loggerstream.info('offset: Corrected time column by %s sec' % str(offsets[key]))
+                    logger.info('offset: Corrected time column by %s sec' % str(offsets[key]))
                 else:
                     val = val + offsets[key]
                     #newval = [elem + offsets[key] for elem in val]
-                    loggerstream.info('offset: Corrected column %s by %.3f' % (key, offsets[key]))
+                    logger.info('offset: Corrected column %s by %.3f' % (key, offsets[key]))
                 if ndtype:
                     self.ndarray[ind][stidx:edidx] = val
                 else:
                     nval = self._get_column(key) # repeated extraction of column - could be optimzed but usage of LineStruct will not be supported in future
                     nval[stidx:edidx] = val
                     self = self._put_column(nval, key)
             else:
-                loggerstream.error("offset: Key '%s' not in keylist." % key)
+                logger.error("offset: Key '%s' not in keylist." % key)
 
         return self
 
 
     def plot(self, keys=None, debugmode=None, **kwargs):
         """
     DEFINITION:
@@ -6978,15 +7015,15 @@
         >>> cs1_data.plot(['f'],
                 outfile = 'frequenz.png',
                 specialdict = {'f':[44184.8,44185.8]},
                 plottitle = 'Station Graz - Feldstaerke 05.08.2013',
                 bgcolor='white')
         """
 
-        import mpplot as mp
+        import magpy.mpplot as mp
         if keys == None:
             keys = []
         mp.plot(self, variables=keys, **kwargs)
 
 
     def powerspectrum(self, key, debugmode=None, outfile=None, fmt=None, axes=None, title=None,**kwargs):
         """
@@ -7037,15 +7074,15 @@
             show = False
         else:
             show = True
 
         dt = self.get_sampling_period()*24*3600
 
         if not len(self) > 0:
-            loggerstream.error("Powerspectrum: Stream of zero length -- aborting")
+            logger.error("Powerspectrum: Stream of zero length -- aborting")
             raise Exception("Can't analyse stream of zero length!")
 
         t = np.asarray(self._get_column('time'))
         val = np.asarray(self._get_column(key))
         mint = np.min(t)
         tnew, valnew = [],[]
 
@@ -7209,18 +7246,18 @@
         >>> data = data.trim(starttime, endtime)
 
     APPLICATION:
         """
 
         if starttime and endtime:
             if self._testtime(starttime) > self._testtime(endtime):
-                loggerstream.error('Trim: Starttime (%s) is larger than endtime (%s).' % (starttime,endtime))
+                logger.error('Trim: Starttime (%s) is larger than endtime (%s).' % (starttime,endtime))
                 raise ValueError("Starttime is larger than endtime.")
 
-        loggerstream.info('Remove: Started from %s to %s' % (starttime,endtime))
+        logger.info('Remove: Started from %s to %s' % (starttime,endtime))
 
         cutstream = DataStream()
         cutstream.header = self.header
         cutstream.ndarray = self.ndarray
         starttime = self._testtime(starttime)
         endtime = self._testtime(endtime)
         stval = 0
@@ -7390,29 +7427,29 @@
         if not stdout:
             stdout = False
         # Position of flag in flagstring
         # f (intensity): pos 0
         # x,y,z (vector): pos 1
         # other (vector): pos 2
 
-        loggerstream.info('remove_outlier: Starting outlier removal.')
+        logger.info('remove_outlier: Starting outlier removal.')
 
         ndtype = False
         if len(self.ndarray[0]) > 0:
             ndtype = True
             arraytime = self.ndarray[0]
             flagind = KEYLIST.index('flag')
             commentind = KEYLIST.index('comment')
             print ("Found ndarray - using flag_outlier instead")
             return self.flag_outlier(**kwargs)
 
         elif len(self) > 1:
             arraytime = self._get_column('time')
         else:
-            loggerstream.warning('remove_outlier: No data - Stopping outlier removal.')
+            logger.warning('remove_outlier: No data - Stopping outlier removal.')
             return self
 
         # Working non-destructive
         restream = self.copy()
 
         # Start here with for key in keys:
         for key in keys:
@@ -7453,15 +7490,15 @@
                     md = np.median(selcol)
                     whisker = threshold*iqd
                 except:
                     try:
                         md = np.median(selcol)
                         whisker = md*0.005
                     except:
-                        loggerstream.warning("remove_outlier: Eliminate outliers produced a problem: please check.")
+                        logger.warning("remove_outlier: Eliminate outliers produced a problem: please check.")
                         pass
 
                 if ndtype:
                     # XXX DOES NOT WORK, TODO
                     for i in range(idxst,idxat):
                         if row.flag == '' or row.flag == '0000000000000000-' or row.flag == '-' or row.flag == '-0000000000000000':
                             row.flag = '-' * len(FLAGKEYLIST)
@@ -7499,15 +7536,15 @@
                                         fllist = fl
                                     fllist[flagpos] = '1'
                                     row.flag=''.join(fllist)
                                     row.comment = "aof - threshold: %s, window: %s sec" % (str(threshold), str(timerange.total_seconds()))
                                     #print row.flag, key
                                     if not isnan(eval('elem.'+key)):
                                         infoline = "remove_outlier: at %s - removed %s (= %f)" % (str(num2date(elem.time)),key, eval('elem.'+key))
-                                        loggerstream.info(infoline)
+                                        logger.info(infoline)
                                         if stdout:
                                             print(infoline)
                         else:
                             fllist = list(row.flag)
                             if len(fllist) >= flagpos:
                                 if row.flag == '':
                                     pass
@@ -7515,15 +7552,15 @@
                                     testlst = [el for el in fllist if el in ['0','1','2','3','4']]
                                     if not len(testlst) > 0:
                                         row.flag = ''
                                 else:
                                     pass
                         newst.add(row)
 
-        loggerstream.info('remove_outlier: Outlier removal finished.')
+        logger.info('remove_outlier: Outlier removal finished.')
 
         if ndtype:
             return restream
         else:
             return DataStream(newst, self.header, self.ndarray)
 
 
@@ -7559,17 +7596,17 @@
 
         ndtype = False
         if len(self.ndarray[0]) > 0:
             ndtype = True
 
         sp = self.samplingrate()
 
-        loggerstream.info("resample: Resampling stream of sampling period %s to period %s." % (sp,period))
+        logger.info("resample: Resampling stream of sampling period %s to period %s." % (sp,period))
 
-        loggerstream.info("resample: Resampling keys %s " % (','.join(keys)))
+        logger.info("resample: Resampling keys %s " % (','.join(keys)))
 
         # Determine the minimum time
         t_min,t_max = self._find_t_limits()
         t_start = t_min
 
         if offset:
             t_min = ceil_dt(t_min,period)
@@ -7580,20 +7617,20 @@
             startperiod, line = self.findtime(t_min)
         else:
             t_min = ceil_dt(t_min,period)
             startperiod, line = self.findtime(t_min)
 
         if fast:   # To be done if timesteps are at period timesteps
             try:
-                loggerstream.info("resample: Using fast algorithm.")
+                logger.info("resample: Using fast algorithm.")
                 si = timedelta(seconds=sp)
                 sampling_period = si.seconds
 
                 if period <= sampling_period:
-                    loggerstream.warning("resample: Resampling period must be larger than original sampling period.")
+                    logger.warning("resample: Resampling period must be larger than original sampling period.")
                     return self
 
                 #print "Trying fast algorythm"
                 if not line == [] or ndtype: # or (ndtype and not line == []):
                     xx = int(np.round(period/sampling_period))
                     if ndtype:
                         newstream = DataStream([LineStruct()],{},np.asarray([]))
@@ -7609,17 +7646,17 @@
                     else:
                         newstream = DataStream([],{},np.asarray([[] for el in KEYLIST]))
                         newstream.header = self.header
                         for line in self[startperiod::xx]:
                             newstream.add(line)
                     newstream.header['DataSamplingRate'] = str(period) + ' sec'
                     return newstream
-                loggerstream.warning("resample: Fast resampling failed - switching to slow mode")
+                logger.warning("resample: Fast resampling failed - switching to slow mode")
             except:
-                loggerstream.warning("resample: Fast resampling failed - switching to slow mode")
+                logger.warning("resample: Fast resampling failed - switching to slow mode")
                 pass
 
         # This is done if timesteps are not at period intervals
         # -----------------------------------------------------
 
         #print ("RESAMPLE Here 3")
         # Create a list containing time steps
@@ -7631,16 +7668,22 @@
            time = time + timedelta(seconds=period)
 
         # Compare length of new time list with old timelist
         # multiplicator is used to check whether nan value is at the corresponding position of the orgdata file - used for not yet completely but sufficiently correct missing value treatment
         if not len(t_list) > 0:
             return DataStream()
         multiplicator = float(self.length()[0])/float(len(t_list))
+        logger.info("resample a: {},{},{}".format(float(self.length()[0]), float(len(t_list)),startperiod))
 
         stwithnan = self.copy()
+        #logger.info("stwithnan: {}".format(stwithnan.ndarray))
+
+        tmp = self.trim(starttime=736011.58337400458,endtime=736011.59721099539)
+        logger.info("resample test: {}".format(tmp.ndarray))
+
         res_stream = DataStream()
         res_stream.header = self.header
         array=[np.asarray([]) for elem in KEYLIST]
         if ndtype:
             array[0] = np.asarray(t_list)
             res_stream.add(LineStruct())
         else:
@@ -7648,15 +7691,15 @@
                 row = LineStruct()
                 row.time = item
                 res_stream.add(row)
 
         for key in keys:
             #print "Resampling:", key
             if key not in KEYLIST[1:16]:
-                loggerstream.warning("resample: Key %s not supported!" % key)
+                logger.warning("resample: Key %s not supported!" % key)
 
             index = KEYLIST.index(key)
             try:
                 int_data = self.interpol([key],kind='linear')#'cubic')
                 int_func = int_data[0]['f'+key]
                 int_min = int_data[1]
                 int_max = int_data[2]
@@ -7664,15 +7707,36 @@
                 key_list = []
                 for ind, item in enumerate(t_list):
                     functime = (item - int_min)/(int_max - int_min)
                     #orgval = eval('self[int(ind*multiplicator)].'+key)
                     if ndtype:
                         if int(ind*multiplicator) <= len(self.ndarray[index]):
                             #orgval = self.ndarray[index][int(ind*multiplicator)]
-                            orgval = stwithnan.ndarray[index][int(ind*multiplicator+startperiod)] # + offset
+                            estimate = False   
+                            # Please note: here a two techniques (exact and estimate)
+                            # Speeddiff (example data set (500000 data points)
+                            # Exact:    7.55 sec (including one minute filter)
+                            # Estimate: 7.15 sec
+                            if estimate:
+                                orgval = stwithnan.ndarray[index][int(ind*multiplicator+startperiod)] # + offset
+                            else:
+                                # Exact solution:
+                                mv = int(ind*multiplicator+startperiod)
+                                stv = mv-int(20*multiplicator)
+                                if stv < 0:
+                                    stv = 0
+                                etv = mv+int(20*multiplicator)
+                                if etv >= len(self.ndarray[index]):
+                                    etv = len(self.ndarray[index])
+                                subar = stwithnan.ndarray[0][stv:etv]
+                                idx = (np.abs(subar-item)).argmin()
+                                #subar = stwithnan.ndarray[index][stv:etv]
+                                orgval = stwithnan.ndarray[index][stv+idx] # + offset
+                                #if item > 736011.58337400458 and item < 736011.59721099539:
+                                #   print ("Found", item, stv+idx, idx, orgval)
                         else:
                             print("Check Resampling method")
                             orgval = 1.0
                     else:
                         orgval = getattr(stwithnan[int(ind*multiplicator+startperiod)],key)
                     tempval = np.nan
                     # Not a safe fix, but appears to cover decimal leftover problems
@@ -7686,19 +7750,19 @@
                     key_list.append(float(tempval))
 
                 if ndtype:
                     array[index] = np.asarray(key_list)
                 else:
                     res_stream._put_column(key_list,key)
             except:
-                loggerstream.error("resample: Error interpolating stream. Stream either too large or no data for selected key")
+                logger.error("resample: Error interpolating stream. Stream either too large or no data for selected key")
 
         res_stream.ndarray = np.asarray(array)
 
-        loggerstream.info("resample: Data resampling complete.")
+        logger.info("resample: Data resampling complete.")
         #return DataStream(res_stream,self.headers)
         res_stream.header['DataSamplingRate'] = str(period) + ' sec'
         return res_stream
 
 
     def rotation(self,**kwargs):
         """
@@ -7738,18 +7802,18 @@
             alpha = 0.
         if not beta:
             beta = 0.
         if not keys:
             keys = ['x','y','z']
 
         if not len(keys) == 3:
-            loggerstream.error('rotation: provided keylist need to have three components.')
+            logger.error('rotation: provided keylist need to have three components.')
             return self
 
-        loggerstream.info('rotation: Applying rotation matrix.')
+        logger.info('rotation: Applying rotation matrix.')
 
         """
         a[0][0] = cos(p)*cos(b);
         a[0][1] = -sin(b);
         a[0][2] = sin(p)*cos(b);
         a[1][0] = cos(p)*sin(b);
         a[1][1] = cos(b);
@@ -7786,15 +7850,15 @@
             #fafter = sqrt(xs**2+ys**2+zs**2)
             #print "f:", fbefore,fafter,fbefore-fafter
 
             elem.x = xs
             elem.y = ys
             elem.z = zs
 
-        loggerstream.info('rotation: Finished reorientation.')
+        logger.info('rotation: Finished reorientation.')
 
         return self
 
 
     def scale_correction(self, keys, scales, **kwargs):
         """
         DEFINITION:
@@ -7814,32 +7878,32 @@
         # Take care: if there is only 0.1 nT accurracy then there will be a similar noise in the deltaF signal
 
         offset = kwargs.get('offset')
         if not offset:
             offset = [0]*len(keys)
         else:
             if not len(offset) == len(keys):
-                loggerstream.error('scale_correction: offset with wrong dimension given - needs to have the same length as given keys - returning stream without changes')
+                logger.error('scale_correction: offset with wrong dimension given - needs to have the same length as given keys - returning stream without changes')
                 return self
 
         try:
             assert len(self) > 0
         except:
-            loggerstream.error('scale_correction: empty stream - aborting')
+            logger.error('scale_correction: empty stream - aborting')
             return self
 
         offsetlst = []
         for key in KEYLIST:
             if key in keys:
                 pos = keys.index(key)
                 offsetlst.append(offset[pos])
             else:
                 offsetlst.append(0.0)
 
-        loggerstream.info('scale_correction:  --- Scale correction started at %s ' % str(datetime.now()))
+        logger.info('scale_correction:  --- Scale correction started at %s ' % str(datetime.now()))
         for elem in self:
             for i,key in enumerate(keys):
                 exec('elem.'+key+' = (elem.'+key+'+offset[i]) * scales[i]')
 
         scalelst = []
         for key in KEYLIST:
             if key in keys:
@@ -7848,15 +7912,15 @@
             else:
                 scalelst.append(1.)
 
         #print '_'.join(map(str,offsetlst)), scalelst
         self.header['DataScaleValues'] = '_'.join(map(str,scalelst))
         self.header['DataOffsets'] = '_'.join(map(str,offsetlst))
 
-        loggerstream.info('scale_correction:  --- Scale correction finished at %s ' % str(datetime.now()))
+        logger.info('scale_correction:  --- Scale correction finished at %s ' % str(datetime.now()))
 
         return self
 
 
     def selectkeys(self, keys, **kwargs):
         """
     DEFINITION:
@@ -7942,36 +8006,36 @@
         if not keys:
             keys=self._get_key_headers(numerical=True)
 
         ndtype = False
         if len(self.ndarray[0])>0:
             ndtype = True
 
-        loggerstream.info('smooth: Start smoothing (%s window, width %d) at %s' % (window, window_len, str(datetime.now())))
+        logger.info('smooth: Start smoothing (%s window, width %d) at %s' % (window, window_len, str(datetime.now())))
 
         for key in keys:
             if key in NUMKEYLIST:
 
                 if ndtype:
                     ind = KEYLIST.index(key)
                     x = self.ndarray[ind]
                 else:
                     x = self._get_column(key)
                 x = maskNAN(x)
 
                 if x.ndim != 1:
-                    loggerstream.error("smooth: Only accepts 1 dimensional arrays.")
+                    logger.error("smooth: Only accepts 1 dimensional arrays.")
                 if x.size < window_len:
                     print(x.size, window_len)
-                    loggerstream.error("smooth: Input vector needs to be bigger than window size.")
+                    logger.error("smooth: Input vector needs to be bigger than window size.")
                 if window_len<3:
                     return x
                 if not window in ['flat', 'hanning', 'hamming', 'bartlett', 'blackman']:
-                    loggerstream.error("smooth: Window is none of 'flat', 'hanning', 'hamming', 'bartlett', 'blackman'")
-                    loggerstream.debug("smooth: You entered string %s as a window." % window)
+                    logger.error("smooth: Window is none of 'flat', 'hanning', 'hamming', 'bartlett', 'blackman'")
+                    logger.debug("smooth: You entered string %s as a window." % window)
 
                 s=np.r_[x[window_len-1:0:-1],x,x[-1:-window_len:-1]]
                 #print(len(s))
                 if window == 'flat': #moving average
                     w=np.ones(window_len,'d')
                 else:
                     w=eval('np.'+window+'(window_len)')
@@ -7979,18 +8043,18 @@
                 y=np.convolve(w/w.sum(),s,mode='valid')
 
                 if ndtype:
                     self.ndarray[ind] = np.asarray(y[(int(window_len/2)):(len(x)+int(window_len/2))])
                 else:
                     self._put_column(y[(int(window_len/2)):(len(x)+int(window_len/2))],key)
             else:
-                loggerstream.error("Column key %s not valid." % key)
+                logger.error("Column key %s not valid." % key)
 
 
-        loggerstream.info('smooth: Finished smoothing at %s' % (str(datetime.now())))
+        logger.info('smooth: Finished smoothing at %s' % (str(datetime.now())))
 
         return self
 
 
     def spectrogram(self, keys, per_lap=0.9, wlen=None, log=False,
                     outfile=None, fmt=None, axes=None, dbscale=False,
                     mult=8.0, cmap=None, zorder=None, title=None, show=True,
@@ -8007,15 +8071,15 @@
 
         if not samp_rate_multiplicator:
             samp_rate_multiplicator = 24*3600
 
         t = self._get_column('time')
 
         if not len(t) > 0:
-            loggerstream.error('Spectrogram: stream of zero length -- aborting')
+            logger.error('Spectrogram: stream of zero length -- aborting')
             return
 
         for key in keys:
             val = self._get_column(key)
             val = maskNAN(val)
             dt = self.get_sampling_period()*(samp_rate_multiplicator)
             Fs = float(1.0/dt)
@@ -8109,15 +8173,15 @@
             print("steadyrise: no data found in selected column %s" % key)
             return np.asarray([])
         # Finally fill the end
         for i in range(count):
             rescol.append(stacked)
 
         if not len(rescol) == len(self) and not len(rescol) == len(self.ndarray[0]) :
-            loggerstream.error('steadrise: An error leading to unequal lengths has been encountered')
+            logger.error('steadrise: An error leading to unequal lengths has been encountered')
             return []
 
         return np.asarray(rescol)
 
     def stereoplot(self, **kwargs):
         """
             DEFINITION:
@@ -8191,29 +8255,29 @@
             legend = 'True'
         if not labellimit:
             labellimit = 11
         if not legendposition:
             legendposition = "lower left"
 
         if not self[0].typ == 'idff':
-            loggerstream.error('Stereoplot: you need to provide idf data')
+            logger.error('Stereoplot: you need to provide idf data')
             return
 
         inc = self._get_column('x')
         dec = self._get_column('y')
 
         col = ['']
         if groups:
             sel = self._get_column(groups)
             col = list(set(list(sel)))
             if len(col) > 7:
                 col = col[:7]
 
         if not len(dec) == len(inc):
-            loggerstream.error('Stereoplot: check you data file - unequal inc and dec data?')
+            logger.error('Stereoplot: check you data file - unequal inc and dec data?')
             return
 
         if not figure:
             fig = plt.figure()
         else:
             fig = figure
         ax = plt.gca()
@@ -8384,18 +8448,18 @@
         >>> data = data.trim(starttime, endtime)
 
     APPLICATION:
         """
 
         if starttime and endtime:
             if self._testtime(starttime) > self._testtime(endtime):
-                loggerstream.error('Trim: Starttime (%s) is larger than endtime (%s).' % (starttime,endtime))
+                logger.error('Trim: Starttime (%s) is larger than endtime (%s).' % (starttime,endtime))
                 raise ValueError("Starttime is larger than endtime.")
 
-        loggerstream.info('Trim: Started from %s to %s' % (starttime,endtime))
+        logger.info('Trim: Started from %s to %s' % (starttime,endtime))
 
         ndtype = False
         if self.ndarray[0].size > 0:
             ndtype = True
             self.container = [LineStruct()]
 
         #-ndarrray---------------------------------------
@@ -8719,21 +8783,21 @@
                     fkey = 'f'+key
                     if fkey in function[0]:
                         try:
                             orgval = float(function[0][fkey](valatorgtime))
                             newval = float(function[0][fkey](valatnewtime))
                             diff = orgval - newval
                         except:
-                            loggerstream.error("variometercorrection: error in assigning new values")
+                            logger.error("variometercorrection: error in assigning new values")
                             return
                         exec('elem.'+key+' = elem.'+key+' - diff')
                     else:
                         pass
             else:
-                loggerstream.warning("variometercorrection: Variometer stream does not cover the projected time range")
+                logger.warning("variometercorrection: Variometer stream does not cover the projected time range")
                 pass
 
         # 5 Convert absresult - xyzf to idff
         absstream = absstream._convertstream('xyz2idf')
 
         return absstream
         """
@@ -8973,28 +9037,28 @@
 
         t1 = datetime.utcnow()
 
         if not format_type in PYMAG_SUPPORTED_FORMATS:
             if not format_type:
                 format_type = 'PYSTR'
             else:
-                loggerstream.warning('write: Output format not supported.')
+                logger.warning('write: Output format not supported.')
                 return False
         else:
             if not 'w' in PYMAG_SUPPORTED_FORMATS[format_type][0]:
-                loggerstream.warning('write: Selected format does not support write methods.')
+                logger.warning('write: Selected format does not support write methods.')
                 return False
 
         format_type, filenamebegins, filenameends, coverage, dateformat = self._write_format(format_type, filenamebegins, filenameends, coverage, dateformat, year)
 
         if not mode:
             mode= 'overwrite'
 
         if len(self) < 1 and len(self.ndarray[0]) < 1:
-            loggerstream.error('write: Stream is empty!')
+            logger.error('write: Stream is empty!')
             raise Exception("Can't write an empty stream to file!")
 
         ndtype = False
         if len(self.ndarray[0]) > 0:
             self.ndarray[0] = self.ndarray[0].astype(float)
             # remove all data from array where time is not numeric
             #1. get indicies of nonnumerics in ndarray[0]
@@ -9123,15 +9187,15 @@
                     filename = filename.upper()
 
                 if debug:
                     print ("Writing data:", os.path.join(filepath,filename))
 
                 if len(lst) > 0 or ndtype:
                     if len(newst.ndarray[0]) > 0 or len(newst) > 1:
-                        loggerstream.info('write: writing %s' % filename)
+                        logger.info('write: writing %s' % filename)
                         #print("Here", num2date(newst.ndarray[0][0]), newst.ndarray)
                         success = writeFormat(newst, os.path.join(filepath,filename),format_type,mode=mode,keys=keys,version=version,gin=gin,datatype=datatype, useg=useg,skipcompression=skipcompression,compression=compression, addflags=addflags)
                 starttime = endtime
                 endtime = endtime + cov
 
                 t5 = datetime.utcnow()
                 #print "write - written:", t5-t3
@@ -9787,39 +9851,39 @@
         proxy_handler = ProxyHandler( {} )
         opener = build_opener(proxy_handler)
         # install this opener
         install_opener(opener)
 
     # 1. No path
     if not path_or_url:
-        loggerstream.error("read: File not specified.")
+        logger.error("read: File not specified.")
         raise Exception("No path given for data in read function!")
 
     # 2. Create DataStream
     st = DataStream([],{},np.array([[] for ke in KEYLIST]))
 
     # 3. Read data
     if not isinstance(path_or_url, basestring):
         # not a string - we assume a file-like object
         pass
         """
         elif path_or_url.startswith("DB:"):
         # a database table
         if
-        loggerstream.error("read: File not specified.")
+        logger.error("read: File not specified.")
         raise Exception("No path given for data in read function!")
         pathname = path_or_url
         for file in iglob(pathname):
             stp = DataStream([],{},np.array([[] for ke in KEYLIST]))
             stp = _read(file, dataformat, headonly, **kwargs) glob
         """
     elif "://" in path_or_url:
         # some URL
         # extract extension if any
-        loggerstream.info("read: Found URL to read at %s" % path_or_url)
+        logger.info("read: Found URL to read at %s" % path_or_url)
         content = urlopen(path_or_url).read()
         if debugmode:
             print(urlopen(path_or_url).info())
         if path_or_url[-1] == '/':
             # directory
             string = content.decode('utf-8')
             for line in string.split("\n"):
@@ -9889,43 +9953,41 @@
                     if not theday[-1] >= datetime.date(st._testtime(starttime)):
                         getfile = False
                 if endtime:
                     if not theday[0] <= datetime.date(st._testtime(endtime)):
                         getfile = False
             except:
                 # Date format not recognised. Read all files
-                loggerstream.warning("read: Unable to detect date string in filename. Reading all files...")
+                logger.warning("read: Unable to detect date string in filename. Reading all files...")
                 getfile = True
             if getfile:
                 stp = DataStream([],{},np.array([[] for ke in KEYLIST]))
                 stp = _read(filename, dataformat, headonly, **kwargs)
                 if (len(stp) > 0 and not np.isnan(stp[0].time)) or len(stp.ndarray[0]) > 0:   # important - otherwise header is going to be deleted
                     st.extend(stp.container,stp.header,stp.ndarray)
             #del stp
         if st.length()[0] == 0:
             # try to give more specific information why the stream is empty
             if has_magic(pathname) and not glob(pathname):
-                loggerstream.error("read: Check file/pathname - No file matching pattern: %s" % pathname)
-                loggerstream.error("read: No file matching file pattern: %s" % pathname)
+                logger.error("read: No file matching file pattern: %s" % pathname)
                 raise Exception("Cannot read non-existent file!")
             elif not has_magic(pathname) and not os.path.isfile(pathname):
-                loggerstream.error("read: No such file or directory: %s" % pathname)
+                logger.error("read: No such file or directory: %s" % pathname)
                 raise Exception("Cannot read non-existent file!")
             # Only raise error if no starttime/endtime has been set. This
             # will return an empty stream if the user chose a time window with
             # no data in it.
             # XXX: Might cause problems if the data is faulty and the user
             # set starttime/endtime. Not sure what to do in this case.
             elif not 'starttime' in kwargs and not 'endtime' in kwargs:
-                loggerstream.error("read: Cannot open file/files: %s" % pathname)
-                print("read: Cannot open file/files: {}".format(pathname))
+                logger.error("read: Cannot open file/files: %s" % pathname)
 
     if headonly and (starttime or endtime):
         msg = "read: Keyword headonly cannot be combined with starttime or endtime."
-        loggerstream.error(msg)
+        logger.error(msg)
 
     # Sort the input data regarding time
     if not skipsorting:
         st = st.sorting()
     # eventually trim data
     if starttime:
         st = st.trim(starttime=starttime)
@@ -9949,33 +10011,35 @@
     stream = DataStream([],{})
     format_type = None
     foundapproptiate = False
     if not dataformat:
         # auto detect format - go through all known formats in given sort order
         for format_type in PYMAG_SUPPORTED_FORMATS:
             # check format
-            if debug:
-                print ("Checking format:", format_type)
+            logger.debug("_read: Checking format:", format_type)
             if isFormat(filename, format_type):
-                if debug:
-                    print ("  -- found:", format_type)
+                logger.debug("  -- found: {}".format(format_type))
                 foundapproptiate = True
                 break
         if not foundapproptiate:
-            print ("Could not identify a suitable data format")
+            temp = open(filename, 'rt').readline()
+            if temp.startswith('# MagPy Absolutes'):
+                logger.warning("_read: You apparently tried to open a DI object - please use the absoluteAnalysis method")
+            else:
+                logger.error("_read: Could not identify a suitable data format")
             return DataStream([LineStruct()],{},np.asarray([[] for el in KEYLIST]))
     else:
         # format given via argument
         dataformat = dataformat.upper()
         try:
             formats = [el for el in PYMAG_SUPPORTED_FORMATS if el == dataformat]
             format_type = formats[0]
         except IndexError:
             msg = "Format \"%s\" is not supported. Supported types: %s"
-            loggerstream.error(msg % (dataformat, ', '.join(PYMAG_SUPPORTED_FORMATS)))
+            logger.error(msg % (dataformat, ', '.join(PYMAG_SUPPORTED_FORMATS)))
             raise TypeError(msg % (dataformat, ', '.join(PYMAG_SUPPORTED_FORMATS)))
 
     """
     try:
         # search readFormat for given entry point
         readFormat = load_entry_point(format_ep.dist.key,
             'obspy.plugin.waveform.%s' % (format_ep.name), 'readFormat')
@@ -9984,15 +10048,15 @@
         raise TypeError(msg % (format_ep.name,
                                ', '.join(WAVEFORM_ENTRY_POINTS)))
     """
     stream = readFormat(filename, format_type, headonly=headonly, **kwargs)
 
     return stream
 
-def saveflags(mylist=None,path=None):
+def saveflags(mylist=None,path=None, overwrite=False):
     """
     DEFINITION:
         Save list e.g. flaglist to file using pickle.
 
     PARAMETERS:
     Variables:
         - path:  (str) Path to data files in form:
@@ -10005,20 +10069,24 @@
     """
     print("Saving flaglist")
     if not mylist:
         print("error 1")
         return False
     if not path:
         path = 'myfile.pkl'
+    if not overwrite:
+        existflag = loadflags(path)
+        existflag.extend(mylist)
+        mylist = existflag
     try:
         # TODO: check whether package is already loaded
         from pickle import dump
         dump(mylist,open(path,'wb'))
         print("saveflags: list saved to {}".format(path))
-        return true
+        return True
     except:
         return False
 
 def loadflags(path=None,sensorid=None,begin=None, end=None):
     """
     DEFINITION:
         Load list e.g. flaglist from file using pickle.
@@ -10053,15 +10121,15 @@
 
 
 def joinStreams(stream_a,stream_b, **kwargs):
     """
     DEFINITION:
         Copy two streams together eventually replacing already existing time steps.
     """
-    loggerstream.info('joinStreams: Start joining at %s.' % str(datetime.now()))
+    logger.info('joinStreams: Start joining at %s.' % str(datetime.now()))
 
     # Check stream type and eventually convert them to ndarrays
     # --------------------------------------
     ndtype = False
     if len(stream_a.ndarray[0]) > 0:
         # Using ndarray and eventually convert stream_b to ndarray as well
         ndtype = True
@@ -10075,15 +10143,15 @@
         if not len(stream_a.ndarray[0]) > 0:
             return stream_b
     else:
         ndtype = True
         stream_a = stream_a.linestruct2ndarray()
         stream_b = stream_b.linestruct2ndarray()
         if not len(stream_a.ndarray[0]) > 0 and not len(stream_b.ndarray[0]) > 0:
-            loggerstream.error('subtractStreams: stream(s) empty - aborting subtraction.')
+            logger.error('subtractStreams: stream(s) empty - aborting subtraction.')
             return stream_a
 
     # non-destructive
     # --------------------------------------
     sa = stream_a.copy()
     sb = stream_b.copy()
 
@@ -10231,15 +10299,15 @@
     if not comment:
         comment = 'keys %s added from %s' % (','.join(keys), sensidb)
     if not flagid:
         flagid = 4
 
     fllst = [] # flaglist
 
-    loggerstream.info('mergeStreams: Start mergings at %s.' % str(datetime.now()))
+    logger.info('mergeStreams: Start mergings at %s.' % str(datetime.now()))
 
 
     # Check stream type and eventually convert them to ndarrays
     # --------------------------------------
     ndtype = False
     if len(stream_a.ndarray[0]) > 0:
         # Using ndarray and eventually convert stream_b to ndarray as well
@@ -10250,15 +10318,15 @@
         ndtype = True
         stream_a = stream_a.linestruct2ndarray()
     else:
         ndtype = True
         stream_a = stream_a.linestruct2ndarray()
         stream_b = stream_b.linestruct2ndarray()
         if not len(stream_a.ndarray[0]) > 0 and len(stream_b.ndarray[0]) > 0:
-            loggerstream.error('subtractStreams: stream(s) empty - aborting subtraction.')
+            logger.error('subtractStreams: stream(s) empty - aborting subtraction.')
             return stream_a
 
     # non-destructive
     # --------------------------------------
     sa = stream_a.copy()
     sb = stream_b.copy()
     sa = sa.removeduplicates()
@@ -10560,15 +10628,15 @@
 
             return DataStream([LineStruct()],header,array)
 
 
     sta = list(stream_a)
     stb = list(stream_b)
     if addall:
-        loggerstream.info('mergeStreams: Adding streams together not regarding for timeconstraints of data.')
+        logger.info('mergeStreams: Adding streams together not regarding for timeconstraints of data.')
         if ndtype:
             for idx,elem in enumerate(stream_a.ndarray):
                 ndarray = stream_a.ndarray
                 if len(elem) == 0 and len(stream_b.ndarray[idx]) > 0:
                     # print add nan's of len_a to stream a
                     # then append stream b
                     pass
@@ -10591,33 +10659,33 @@
                 headera[elem]
                 ha = True
             except:
                 ha = False
             if headerb[elem] and not ha:
                 newsta.header[elem] = headerb[elem]
             elif headerb[elem] and ha:
-                loggerstream.warning("mergeStreams: headers both have keys for %s. Headers may be incorrect." % elem)
+                logger.warning("mergeStreams: headers both have keys for %s. Headers may be incorrect." % elem)
         newsta.sorting()
         return newsta
     elif extend:
-        loggerstream.info('mergeStreams: Extending stream a with data from b.')
+        logger.info('mergeStreams: Extending stream a with data from b.')
         for elem in stream_b:
             if not elem.time in timea:
                 sta.append(elem)
         newsta = DataStream(sta, headera)
         for elem in headerb:
             try:
                 headera[elem]
                 ha = True
             except:
                 ha = False
             if headerb[elem] and not ha:
                 newsta.header[elem] = headerb[elem]
             elif headerb[elem] and ha:
-                loggerstream.warning("mergeStreams: headers both have keys for %s. Headers may be incorrect." % elem)
+                logger.warning("mergeStreams: headers both have keys for %s. Headers may be incorrect." % elem)
         newsta.sorting()
         return newsta
     else:
         # interpolate stream_b
         # changed the following trim section to prevent removal of first input in trim method
         if stream_b[0].time == np.min(timea):
             sb = stream_b.trim(endtime=np.max(timea))
@@ -10634,15 +10702,15 @@
             pos = foundina[1]
             ta = foundina[0]
             if (ta > taprev) and (np.min(timeb) <= ta <= np.max(timeb)):
                 taprev = ta
                 functime = (ta-function[1])/(function[2]-function[1])
                 for key in keys:
                     if not key in KEYLIST[1:16]:
-                        loggerstream.error('mergeStreams: Column key (%s) not valid.' % key)
+                        logger.error('mergeStreams: Column key (%s) not valid.' % key)
                     #keyval = getattr(stream_a[pos], key)# should be much better
                     exec('keyval = stream_a[pos].'+key)
                     fkey = 'f'+key
                     if fkey in function[0] and (isnan(keyval) or not stream_a._is_number(keyval)):
                         newval = function[0][fkey](functime)
                         exec('stream_a['+str(pos)+'].'+key+' = float(newval) + offset')
                         exec('stream_a['+str(pos)+'].comment = comment')
@@ -10665,15 +10733,15 @@
                             flagpos = flagposlst[0]
                             fllist = list(stream_a[pos].flag)
                             fllist[flagpos] = '4'
                             stream_a[pos].flag=''.join(fllist)
                         except:
                             pass
 
-    loggerstream.info('mergeStreams: Mergings finished at %s ' % str(datetime.now()))
+    logger.info('mergeStreams: Mergings finished at %s ' % str(datetime.now()))
 
     return DataStream(stream_a, headera)
 
 def dms2d(dms):
         """
         DESCRIPTION:
             converts a string with degree:minutes:seconds to degree.decimals
@@ -10785,18 +10853,18 @@
 
     # Interpolate one stream:
     # Note: higher errors with lower degree of interpolation. Highest degree possible is desirable, linear terrible.
     try:
         int_data = stream_b.interpol(['f'],kind='cubic')
     except:
         try:
-            loggerstream.warning("find_offset: Not enough memory for cubic spline. Attempting quadratic...")
+            logger.warning("find_offset: Not enough memory for cubic spline. Attempting quadratic...")
             int_data = stream_b.interpol(['f'],kind='quadratic')
         except:
-            loggerstream.error("find_offset: Too much data! Cannot interpolate function with high enough accuracy.")
+            logger.error("find_offset: Too much data! Cannot interpolate function with high enough accuracy.")
             return "nan"
 
     int_func = int_data[0]['ff']
     int_min = date2num(num2date(int_data[1])+timedelta(milliseconds=guess_low*1000.))
     int_max = date2num(num2date(int_data[2])+timedelta(milliseconds=guess_low*1000.))
 
     timea = stream_a._get_column('f')
@@ -10824,15 +10892,15 @@
         newfile = open('chisq.txt','a')
         writestring = str(deltat)+' '+str(chisq_)+' '+str(chisq_)+' '+str(len(datarray_base))+'\n'
         newfile.write(writestring)
         newfile.close()
 
     # 4. Start iteration to find best chi-squared minimisation:
 
-    loggerstream.info("find_offset: Starting chi-squared iterations...")
+    logger.info("find_offset: Starting chi-squared iterations...")
 
     chi_lst = []
     time_lst = []
     min_lst = []
     max_lst = []
     results = []
 
@@ -10878,15 +10946,15 @@
     if plot:
         plt.plot(time_lst,chi_lst,'-')
         plt.show()
 
     if not main_a:
         t_offset = t_offset * (-1)
 
-    loggerstream.info("find_offset: Found an offset of stream_a of %s seconds." % t_offset)
+    logger.info("find_offset: Found an offset of stream_a of %s seconds." % t_offset)
 
     # RESULTS
     return t_offset
 
 
 def diffStreams(stream_a, stream_b, **kwargs):
     """
@@ -10895,15 +10963,15 @@
     """
 
     ndtype_a = False
     if len(stream_a.ndarray[0]) > 0:
         ndtype_a = True
 
     if not ndtype_a or not len(stream_a) > 0:
-        loggerstream.error('diffStreams: stream_a empty - aborting.')
+        logger.error('diffStreams: stream_a empty - aborting.')
         return stream_a
 
     ndtype_b = False
     if len(stream_b.ndarray[0]) > 0:
         ndtype_b = True
 
     # 1. Amount of columns
@@ -10961,24 +11029,26 @@
     elif len(stream_b.ndarray[0]) > 0:
         ndtype = True
         stream_a = stream_a.linestruct2ndarray()
     else:
         try:
             assert len(stream_a) > 0
         except:
-            loggerstream.error('subtractStreams: stream_a empty - aborting subtraction.')
+            logger.error('subtractStreams: stream_a empty - aborting subtraction.')
             return stream_a
 
-    loggerstream.info('subtractStreams: Start subtracting streams.')
+    logger.info('subtractStreams: Start subtracting streams.')
 
     headera = stream_a.header
     headerb = stream_b.header
 
 
     # non-destructive
+    print ("SA:", stream_a.length())
+    print ("SB:", stream_b.length())
     sa = stream_a.copy()
     sb = stream_b.copy()
 
     # Sampling rates
     sampratea = sa.samplingrate()
     samprateb = sb.samplingrate()
     minsamprate = min(sampratea,samprateb)
@@ -11030,35 +11100,35 @@
     # 1- No overlap of a and b
     # 2- a high resolution and b low resolution (tested)
     # 3- a low resolution and b high resolution (tested)
     # 4- a shorter and fully covered by b (tested)
     # 5- b shorter and fully covered by a
 
     if ndtype:
-            print("Running ndtype subtraction")
+            logger.info('subtractStreams: Running ndtype subtraction')
             # Assuming similar time steps
             #t1s = datetime.utcnow()
             # Get indicies of stream_b of which times are present in stream_a
             array = [[] for key in KEYLIST]
-            try: # TODO Find a better solution here!
+            try: # TODO Find a better solution here! Roman 2017
                 # The try clause is not correct as searchsorted just finds
                 # positions independet of agreement (works well if data is similar)
                 idxB = np.argsort(timeb)
                 sortedB = timeb[idxB]
                 idxA = np.searchsorted(sortedB, timea)
                 #print timea, timeb,len(idxA), len(idxB)
                 indtib = idxB[idxA]
             except:
                 indtib = np.nonzero(np.in1d(timeb, timea))[0]
             #print timeb[pos]
-            #print timea
-            #print indtib
+            #print ("Here", timea)
+            #print (indtib)
             # If equal elements occur in time columns
             if len(indtib) > int(0.5*len(timeb)):
-                print("Found identical timesteps - using simple subtraction")
+                logger.info('subtractStreams: Found identical timesteps - using simple subtraction')
                 # get tb times for all matching indicies
                 tb = np.asarray([timeb[ind] for ind in indtib])
                 # Get indicies of stream_a of which times are present in matching tbs
                 try:
                     idxA = np.argsort(timea)
                     sortedA = timea[idxA]
                     idxB = np.searchsorted(sortedA, tb)
@@ -11203,15 +11273,15 @@
             if ttt > stime:
                 stimeb = timeb[idx-1]
                 break
     else:
         stimeb = stime
 
     if (etime <= stime):
-        loggerstream.error('subtractStreams: Streams are not overlapping!')
+        logger.error('subtractStreams: Streams are not overlapping!')
         return stream_a
 
 
     # ----------------------------------------------
     # --------- if loop for new technique ----------
     # ----------------------------------------------
     # changes from 23 May 2014 by leon
@@ -11219,15 +11289,15 @@
     # need to check all subsequent functions !!!
     if newway == True:
         subtractedstream = DataStream([],{},np.asarray([[] for key in KEYLIST]))
         sa = stream_a.trim(starttime=num2date(stime).replace(tzinfo=None), endtime=num2date(etime).replace(tzinfo=None)+timedelta(seconds=sampratea),newway=True)
         sb = stream_b.trim(starttime=num2date(stimeb).replace(tzinfo=None), endtime=num2date(etimeb).replace(tzinfo=None)+timedelta(seconds=samprateb),newway=True)
         samplingrate_b = sb.get_sampling_period()
 
-        loggerstream.info('subtractStreams (newway): Time range from %s to %s' % (num2date(stime).replace(tzinfo=None),num2date(etime).replace(tzinfo=None)))
+        logger.info('subtractStreams (newway): Time range from %s to %s' % (num2date(stime).replace(tzinfo=None),num2date(etime).replace(tzinfo=None)))
 
         # Interpolate stream_b
         # --------------------
         function = sb.interpol(keys)
         taprev = 0
 
         # Check for the following cases:
@@ -11302,15 +11372,15 @@
     # Take only the time range of the shorter stream
     # Important for baselines: extend the absfile to start and endtime of the stream to be corrected
     stream_a = stream_a.trim(starttime=num2date(stime).replace(tzinfo=None), endtime=num2date(etime).replace(tzinfo=None))
     stream_b = stream_b.trim(starttime=num2date(stimeb).replace(tzinfo=None), endtime=num2date(etimeb).replace(tzinfo=None))
 
     samplingrate_b = stream_b.get_sampling_period()
 
-    loggerstream.info('subtractStreams: Time range from %s to %s' % (num2date(stime).replace(tzinfo=None),num2date(etime).replace(tzinfo=None)))
+    logger.info('subtractStreams: Time range from %s to %s' % (num2date(stime).replace(tzinfo=None),num2date(etime).replace(tzinfo=None)))
 
     # Interpolate stream_b
     function = stream_b.interpol(keys)
     taprev = 0
     for elem in stream_a:
         ta = elem.time
         if ta >= function[1]: # in records of different resolution the first element might be older then the function start
@@ -11318,49 +11388,49 @@
             # Do the subtraction if there is is an element within stream b within twice the sampling rate distance
             # If not wite NaN to the diffs
             tb, itmp = find_nearest(timeb,ta)
             #Test whether a time_b event exists in the vicinity of ta and whether tb is within the time_b range otherwise interpolation fails
             if ta-samplingrate_b < tb < ta+samplingrate_b and timeb[0]<ta<timeb[-1] :
                 for key in keys:
                     if not key in KEYLIST[1:16]:
-                        loggerstream.error("subtractStreams: Column key %s not valid!" % key)
+                        logger.error("subtractStreams: Column key %s not valid!" % key)
                     fkey = 'f'+key
                     try:
                         if fkey in function[0] and not isnan(eval('stream_b[itmp].' + key)):
                             newval = function[0][fkey](functime)
                             exec('elem.'+key+' -= float(newval)')
                         else:
                             setattr(elem, key, float(NaN))
                             #exec('elem.'+key+' = float(NaN)')
                     except:
-                        loggerstream.warning("subtractStreams: Check why exception was thrown.")
+                        logger.warning("subtractStreams: Check why exception was thrown.")
                         setattr(elem, key, float(NaN))
                         #exec('elem.'+key+' = float(NaN)')
             else:
                 for key in keys:
                     if not key in KEYLIST[1:16]:
-                        loggerstream.error("subtractStreams: Column key %s not valid!" % key)
+                        logger.error("subtractStreams: Column key %s not valid!" % key)
                     fkey = 'f'+key
                     if fkey in function[0]:
                         setattr(elem, key, float(NaN))
                         #exec('elem.'+key+' = float(NaN)')
         else: # put NaNs in cloumn if no interpolated values in b exist
             for key in keys:
                 if not key in KEYLIST[1:16]:
-                    loggerstream.error("subtractStreams: Column key %s not valid!" % key)
+                    logger.error("subtractStreams: Column key %s not valid!" % key)
                 fkey = 'f'+key
                 if fkey in function[0]:
                     setattr(elem, key, float(NaN))
                     #exec('elem.'+key+' = float(NaN)')
 
     try:
         headera['SensorID'] = headera['SensorID']+'-'+headerb['SensorID']
     except:
         pass
-    loggerstream.info('subtractStreams: Stream-subtraction finished.')
+    logger.info('subtractStreams: Stream-subtraction finished.')
 
     return DataStream(stream_a, headera)
 
 
 def stackStreams(streamlist, **kwargs): # TODO
     """
     DEFINITION:
@@ -11575,15 +11645,15 @@
     replace = True
 
     # Do the sampling periods match?
     samplingrate_a = stream_a.get_sampling_period()
     samplingrate_b = stream_b.get_sampling_period()
 
     if samplingrate_a != samplingrate_b:
-        loggerstream.error('CompareStreams: Cannot compare streams with different sampling rates!')
+        logger.error('CompareStreams: Cannot compare streams with different sampling rates!')
         return stream_a
 
     # Do the timelines overlap?
     timea = stream_a._get_column('time')
     timeb = stream_b._get_column('time')
 
     if np.min(timeb) < np.min(timea):
@@ -11592,75 +11662,75 @@
         stime = np.min(timeb)
     if np.max(timeb) > np.max(timea):
         etime = np.max(timea)
     else:
         etime = np.max(timeb)
 
     if (etime <= stime):
-        loggerstream.error('compareStreams: Streams do not overlap!')
+        logger.error('compareStreams: Streams do not overlap!')
         return stream_a
 
     # Trim to overlapping areas:
     stream_a = stream_a.trim(starttime=num2date(stime).replace(tzinfo=None),
                                 endtime=num2date(etime).replace(tzinfo=None))
     stream_b = stream_b.trim(starttime=num2date(stime).replace(tzinfo=None),
                                 endtime=num2date(etime).replace(tzinfo=None))
 
 
-    loggerstream.info('compareStreams: Starting comparison...')
+    logger.info('compareStreams: Starting comparison...')
 
     # Compare value for value between the streams:
 
     flag_len = False
 
     t_a = stream_a._get_column('time')
     t_b = stream_b._get_column('time')
 
     # Check length:
     if len(t_a) < len(t_b):
-        loggerstream.debug("compareStreams: Missing data in main stream.")
+        logger.debug("compareStreams: Missing data in main stream.")
         flag_len = True
 
     # If the lengths are the same, compare single values for differences:
     if not flag_len:
         for i in range(len(t_a)):
             for key in FLAGKEYLIST:
                 exec('val_a = stream_a[i].'+key)
                 exec('val_b = stream_b[i].'+key)
                 if not isnan(val_a):
                     if val_a != val_b:
-                        loggerstream.debug("compareStreams: Data points do not match: %s and %s at time %s." % (val_a, val_b, stream_a[i].time))
+                        logger.debug("compareStreams: Data points do not match: %s and %s at time %s." % (val_a, val_b, stream_a[i].time))
                         if replace == True:
                             exec('stream_a[i].'+key+' = stream_b[i].'+key)
 
     # If the lengths are different, find where values are missing:
     else:
         for i in range(len(t_b)):
             if stream_a[i].time == stream_b[i].time:
                 for key in FLAGKEYLIST:
                     exec('val_a = stream_a[i].'+key)
                     exec('val_b = stream_b[i].'+key)
                     if not isnan(val_a):
                         if val_a != val_b:
-                            loggerstream.debug("compareStreams: Data points do not match: %s and %s at time %s." % (val_a, val_b, stream_a[i].time))
+                            logger.debug("compareStreams: Data points do not match: %s and %s at time %s." % (val_a, val_b, stream_a[i].time))
                             if replace == True:
                                 exec('stream_a[i].'+key+' = stream_b[i].'+key)
             else:       # insert row into stream_a
-                loggerstream.debug("compareStreams: Line from secondary stream missing in main stream. Timestamp: %s." % stream_b[i].time)
+                logger.debug("compareStreams: Line from secondary stream missing in main stream. Timestamp: %s." % stream_b[i].time)
                 if insert == True:
                     row = LineStruct()
                     stream_a.add(row)
                     for key in KEYLIST:
                         temp = stream_a._get_column(key)
                         if len(temp) > 0:
                             for j in range(i+1,len(stream_a)):
                                 exec('stream_a[j].'+key+' = temp[j-1]')
                             exec('stream_a[i].'+key+' = stream_b[i].'+key)
 
-    loggerstream.info('compareStreams: Finished comparison!')
+    logger.info('compareStreams: Finished comparison!')
     return stream_a
 
 
 # Some helpful methods
 def array2stream(listofarrays, keystring,starttime=None,sr=None):
         """
         DESCRIPTION:
@@ -11970,19 +12040,19 @@
                     num_found = True
             if num_found:
                 mcolumn = np.ma.masked_invalid(column)
                 numdat = True
                 column = mcolumn
             else:
                 numdat = False
-                loggerstream.warning("NAN warning: only nan in column")
+                logger.warning("NAN warning: only nan in column")
                 return []
     except:
         numdat = False
-        #loggerstream.warning("Here: NAN warning: only nan in column")
+        #logger.warning("Here: NAN warning: only nan in column")
         return []
 
     return column
 
 
 def nan_helper(y):
     """Helper to handle indices and logical indices of NaNs. Taken from eat (http://stackoverflow.com/questions/6518811/interpolate-nan-values-in-a-numpy-array)
```

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/csprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/csprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/bm35protocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/bm35protocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/pos1protocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/pos1protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         splittedfull = timestring.split(' ')
         splittedday = splittedfull[0].split('-')
         splittedsec = splittedfull[1].split('.')
         splittedtime = splittedsec[0].split(':')
         datearray = splittedday + splittedtime
         datearray.append(splittedsec[1])
         datearray = map(int,datearray)
-        return datearray
+        return datetime(*datearray)
     except:
         log.msg('Error while extracting time array')
         return []
 
 
 def _dataToFile(outputdir, sensorid, filedate, bindata, header):
     # File Operations
@@ -249,14 +249,15 @@
         log.msg(' Pos1 connection lost.')
 
     def connectionMade(self):
         log.msg('%s connected.' % self.sensor)
 
     def processPos1Data(self, data):
         """Convert raw ADC counts into SI units as per datasheets"""
+        #print (data)
         if len(data) != 44:
             log.err('POS1 - Protocol: Unable to parse data of length %i' % len(data))
 
         currenttime = datetime.utcnow()
         date = datetime.strftime(currenttime, "%Y-%m-%d")
         actualtime = datetime.strftime(currenttime, "%Y-%m-%dT%H:%M:%S.%f")
         outtime = datetime.strftime(currenttime, "%H:%M:%S")
@@ -274,24 +275,27 @@
             newdate = datetime.strftime(dataelements,"%Y-%m-%d")
             gps_time = newdate + ' ' + str(data_array[5])[:11]
         except:
             log.err('POS1 - Protocol: Data formatting error.')
             intensity = 0.0
             sigma_int = 0.0
             err_code = 0.0
+        #try:
+        # extract time data
+        datedt = _timeToArray(timestamp)        
+        # new line for time shift
+        datedt = datedt - timedelta(seconds=6.770)
+        gpsdt = _timeToArray(gps_time)
         try:
-            # extract time data
-            datearray = _timeToArray(timestamp)
-            # new line for time shift
-            datearray = datearray - timedelta(seconds=6.770)
-            gpsarray = _timeToArray(gps_time)
             try:
+                datearray = [datedt.year, datedt.month, datedt.day, datedt.hour, datedt.minute, datedt.second, datedt.microsecond]
                 datearray.append(int(intensity*1000))
                 datearray.append(int(sigma_int*1000))
                 datearray.append(err_code)
+                gpsarray = [gpsdt.year, gpsdt.month, gpsdt.day, gpsdt.hour, gpsdt.minute, gpsdt.second, gpsdt.microsecond]
                 datearray.extend(gpsarray)
                 data_bin = struct.pack(packcode,datearray[0],datearray[1],datearray[2],datearray[3],datearray[4],datearray[5],datearray[6],datearray[7],datearray[8],datearray[9],datearray[10],datearray[11],datearray[12],datearray[13],datearray[14],datearray[15],datearray[16])
                 # File Operations
                 _dataToFile(self.outputdir,self.sensor, date, data_bin, header)
             except:
                 log.msg('POS1 - Protocol: Error while packing binary data')
                 pass
```

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/gsm90protocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/gsm90protocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/envprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/envprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/gsmp20protocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/gsmp20protocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/arduinoprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/arduinoprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/gsm19protocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/gsm19protocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/acquisition.py` & `GeomagPy-v0.3.93/magpy/acquisition/acquisition.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/kernprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/kernprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/cobs_ws_protocols.py` & `GeomagPy-v0.3.93/magpy/acquisition/cobs_ws_protocols.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/STANDARD_KEYS.py` & `GeomagPy-v0.3.93/magpy/acquisition/STANDARD_KEYS.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/callprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/callprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/lemiprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/lemiprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/palmacqprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/palmacqprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/acquisition/owprotocol.py` & `GeomagPy-v0.3.93/magpy/acquisition/owprotocol.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/__init__.py` & `GeomagPy-v0.3.93/magpy/__init__.py`

 * *Files identical despite different names*

### Comparing `GeomagPy-v0.3.92/magpy/database.py` & `GeomagPy-v0.3.93/magpy/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 from __future__ import absolute_import
 from __future__ import division
 
 from magpy.stream import *
 from magpy.absolutes import *
 from magpy.transfer import *
 
-print("Loading python's SQL support")
+import logging
+logger = logging.getLogger(__name__)
+
+logger.info("Loading python's SQL support")
 try:
     # Loading MySQL functionality
     import MySQLdb as mysql
-    print("... success")
+    logger.info("... success")
 except ImportError:
     try:
         # Loading alternative MySQL functionality
         import pymysql as mysql
         mysql.install_as_MySQLdb()
-        print("... success")
+        logger.info("... success")
     except:
-        print("Failed to import SQL packages 'MySQLdb' or 'pymysql'")
+        logger.warning("Failed to import SQL packages 'MySQLdb' or 'pymysql'")
 except:
-    print("SQL package import failed")
+    logger.warning("MySQLdb package import failed")
     pass
 
 
 """
 AVAILABLE METHODS:
 ---------------------------------
 dbgetfloat(db,tablename,sensorid,columnid,revision=None)
@@ -3053,40 +3056,137 @@
     PARAMETER:
        db:              name of the mysql data base
        stream:          data stream which is corrected
 
     RETURNS:
        a data stream with offsets applied
     """
+    def calloffset(datastream, key, value, st=None, et=None):
+        #print ("Getting offset", key, value, st, et)
+        tst = True
+        tet = True
+        if st in ['',None]:
+            tst = False 
+        if et in ['',None]:
+            tet = False 
+        try:
+            st = float(st)
+            et = float(et)
+        except:
+            pass
+        #print (tst, tet)
+        if tst and tet :
+            #print ("st and et")
+            datastream = datastream.offset({key:value},starttime=st,endtime=et)
+        elif tst:
+            #print ("st")
+            datastream = datastream.offset({key:value},starttime=st)
+        else:
+            #print ("old")
+            datastream = datastream.offset({key:value})
+        return datastream
+
     dataid = stream.header.get('DataID','')
     if dataid == '':
         print ("applyDeltas: No dataid found in streams header - aborting")
         return stream
 
     deltas = stream.header.get('DataDeltaValues','')
     if deltas == '':
         print ("applyDeltas: No delta values found - returning unmodified stream")
         return stream
+    try:
+        deltalines = deltas.split(';')
+    except:
+        #print("Could not extract delta values for ", dataid)
+        pass
 
+    logger.info("applyDeltas: Running delta app")
     try:
-        deltas = deltas.split(',')
-        for el in deltas:
-            dat = el.split('_')
-            print ("Correcting {a} offset: {b}".format(a=dat[0],b=dat[1]))
-            if dat[0] == 'time':
-                stream = stream.offset({'time': dat[1]})
-            if dat[0] in NUMKEYLIST:
-                stream = stream.offset({dat[0]: float(dat[1])})
+        for delt in deltalines:
+            deltdict = {}
+            starttime = ''
+            endtime = ''
+            delts = delt.split(',')
+            for el in delts:
+                dat = el.split('_')
+                deltdict[dat[0]] = dat[1]
+            if not deltdict.get('st','') == '':
+                starttime = deltdict.get('st','')
+            if not deltdict.get('et','') == '':
+                endtime = deltdict.get('et','')
+            #logger.info("applyDeltas: {}, {}, {}".format(delts, starttime, endtime))
+            for key in deltdict:
+                if not key in ['st','et']:
+                    if key == 'time':
+                        stream = calloffset(stream,'time',deltdict[key],starttime,endtime)
+                    elif key in NUMKEYLIST:
+                        stream = calloffset(stream,key,float(deltdict[key]),starttime,endtime)
         stream.header['DataDeltaValues'] = ''
     except:
-        print("Could not extract delta values for ", dataid)
+        pass
 
     return stream
 
 
+def dbaddBLV2DATAINFO(db,blvname, stationid):
+     keylist = []
+     valuelist = []
+
+     existingblv = dbselect(db, 'DataID', 'DATAINFO', 'DataID = "{}"'.format(blvname))
+
+     try:
+         data = readDB(db,blvname)
+         tlimits = data._find_t_limits()
+         keylist.append('DataMinTime')
+         valuelist.append(datetime.strftime(tlimits[0],"%Y-%m-%d %H:%M:%S.%f"))
+         keylist.append('DataMaxTime')
+         valuelist.append(datetime.strftime(tlimits[1],"%Y-%m-%d %H:%M:%S.%f"))
+     except:
+         pass
+
+     if not len(existingblv) > 0:
+         keylist.append('DataID')
+         valuelist.append(blvname)
+         keylist.append('SensorID')
+         valuelist.append(blvname)
+         keylist.append('StationID')
+         valuelist.append(stationid)
+         keylist.append('ColumnContents')
+         valuelist.append('i,d,f,f,T,ScaleValueDI,Dec_S0,Dec_deltaH,Dec_epsilonZ,Inc_S0,Inc_epsilonZ,H-base,D-base,Z-base,,Person,DI-Inst,Mire,F-type,,,,')
+         keylist.append('ColumnUnits')
+         valuelist.append('deg,deg,nT,nT,deg C,deg/unit,,,,,,nT,deg,nT,,,,,,,,,')
+         keylist.append('DataFormat')
+         valuelist.append('MagPyDI')
+         keylist.append('DataComponents')
+         valuelist.append('IDFF')
+         keylist.append('DataPier')
+         valuelist.append(blvname.split('_')[-1])
+
+         sql = 'INSERT INTO DATAINFO (%s) VALUE (%s)' %  (', '.join(keylist), '"'+'", "'.join(valuelist)+'"')
+     else:
+         updatelst=[]
+         for idx,key in enumerate(keylist):
+             updatelst.append(key+"='"+valuelist[idx]+"'")
+         sql = "UPDATE DATAINFO SET {} WHERE DataID = '{}'".format(','.join(updatelst),blvname)
+
+     # Execute the sql statement
+     cursor = db.cursor()
+     try:
+         print ("Updating DATAINFO table with {}".format(blvname))
+         cursor.execute(sql)
+     except mysql.Error as e:
+         print ("Failed: {}".format(e))
+     except:
+         print ("Failed for unknown reason")
+     db.commit()
+     cursor.close()
+
+
+
 def getBaseline(db,sensorid, date=None):
     """
     DESCRIPTION:
        Method to extract a list of baseline fitting data from db.
 
     PARAMETER:
        db:              name of the mysql data base
```

### Comparing `GeomagPy-v0.3.92/setup.py` & `GeomagPy-v0.3.93/setup.py`

 * *Files identical despite different names*

