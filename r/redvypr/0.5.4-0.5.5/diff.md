# Comparing `tmp/redvypr-0.5.4.tar.gz` & `tmp/redvypr-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvypr-0.5.4.tar", last modified: Tue Apr 25 17:46:13 2023, max compression
+gzip compressed data, was "redvypr-0.5.5.tar", last modified: Wed Apr 26 10:09:42 2023, max compression
```

## Comparing `redvypr-0.5.4.tar` & `redvypr-0.5.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.518166 redvypr-0.5.4/
--rw-r--r--   0 holterma  (1000) holterma  (1000)    35149 2022-03-17 04:29:20.000000 redvypr-0.5.4/LICENSE
--rw-r--r--   0 holterma  (1000) holterma  (1000)      813 2023-04-25 17:46:13.518166 redvypr-0.5.4/PKG-INFO
--rw-r--r--   0 holterma  (1000) holterma  (1000)     3030 2022-06-17 04:23:43.000000 redvypr-0.5.4/README.md
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.506166 redvypr-0.5.4/redvypr/
--rw-r--r--   0 holterma  (1000) holterma  (1000)        5 2023-04-25 17:45:16.000000 redvypr-0.5.4/redvypr/VERSION
--rw-r--r--   0 holterma  (1000) holterma  (1000)      286 2023-04-25 09:31:02.000000 redvypr-0.5.4/redvypr/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    26761 2023-04-25 09:24:41.000000 redvypr-0.5.4/redvypr/config.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    10726 2023-04-25 09:24:41.000000 redvypr-0.5.4/redvypr/configdata.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    40721 2023-04-25 10:43:41.000000 redvypr-0.5.4/redvypr/data_packets.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    27230 2023-04-25 04:44:39.000000 redvypr-0.5.4/redvypr/device.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.506166 redvypr-0.5.4/redvypr/devices/
--rw-r--r--   0 holterma  (1000) holterma  (1000)      135 2023-04-10 17:52:06.000000 redvypr-0.5.4/redvypr/devices/__init__.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.506166 redvypr-0.5.4/redvypr/devices/db/
--rw-r--r--   0 holterma  (1000) holterma  (1000)        0 2023-03-29 11:49:05.000000 redvypr-0.5.4/redvypr/devices/db/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     1872 2022-12-11 06:19:03.000000 redvypr-0.5.4/redvypr/devices/db/influxdb_device.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.506166 redvypr-0.5.4/redvypr/devices/develop/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       24 2023-04-19 10:29:29.000000 redvypr-0.5.4/redvypr/devices/develop/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    37708 2023-03-26 05:06:47.000000 redvypr-0.5.4/redvypr/devices/develop/csvlogger.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.510166 redvypr-0.5.4/redvypr/devices/fileio/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       56 2023-04-19 10:29:41.000000 redvypr-0.5.4/redvypr/devices/fileio/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    28729 2023-04-06 05:28:30.000000 redvypr-0.5.4/redvypr/devices/fileio/rawdatalogger.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    16771 2023-04-05 18:41:57.000000 redvypr-0.5.4/redvypr/devices/fileio/rawdatareplay.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.510166 redvypr-0.5.4/redvypr/devices/interface/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       28 2023-04-10 17:40:41.000000 redvypr-0.5.4/redvypr/devices/interface/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    15186 2023-04-17 11:51:35.000000 redvypr-0.5.4/redvypr/devices/interface/serial_device.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.510166 redvypr-0.5.4/redvypr/devices/network/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       77 2023-03-29 11:42:45.000000 redvypr-0.5.4/redvypr/devices/network/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)   101562 2023-04-25 04:50:06.000000 redvypr-0.5.4/redvypr/devices/network/iored.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    33337 2023-01-09 05:25:09.000000 redvypr-0.5.4/redvypr/devices/network/network_device.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     8771 2023-04-17 17:53:48.000000 redvypr-0.5.4/redvypr/devices/network/zeromq_device.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.510166 redvypr-0.5.4/redvypr/devices/plot/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       72 2023-04-10 17:41:27.000000 redvypr-0.5.4/redvypr/devices/plot/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    31897 2023-04-25 09:24:41.000000 redvypr-0.5.4/redvypr/devices/plot/plot.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    23149 2023-04-25 09:24:41.000000 redvypr-0.5.4/redvypr/devices/plot/plot_widgets.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     2907 2023-04-17 17:53:38.000000 redvypr-0.5.4/redvypr/devices/plot/rawdatadisp.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.510166 redvypr-0.5.4/redvypr/devices/processing/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       79 2023-04-10 17:58:08.000000 redvypr-0.5.4/redvypr/devices/processing/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     2147 2023-04-25 13:56:48.000000 redvypr-0.5.4/redvypr/devices/processing/csvparser.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6525 2023-04-25 13:56:08.000000 redvypr-0.5.4/redvypr/devices/processing/nmeaparser.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5761 2023-04-17 17:54:15.000000 redvypr-0.5.4/redvypr/devices/processing/sensor_raw2unit.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.510166 redvypr-0.5.4/redvypr/devices/test/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       26 2023-03-29 11:50:28.000000 redvypr-0.5.4/redvypr/devices/test/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     2156 2023-04-05 10:52:52.000000 redvypr-0.5.4/redvypr/devices/test/test_device.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      990 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/files.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    28218 2023-04-25 09:24:41.000000 redvypr-0.5.4/redvypr/gui.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.514166 redvypr-0.5.4/redvypr/icon/
--rw-r--r--   0 holterma  (1000) holterma  (1000)    11374 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/icon_v02.ico
--rw-r--r--   0 holterma  (1000) holterma  (1000)    10980 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/icon_v02.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    39662 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/icon_v03.1.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5924 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/icon_v03.1.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    34925 2022-06-05 18:16:36.000000 redvypr-0.5.4/redvypr/icon/icon_v03.1_small.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    38644 2022-06-06 07:01:58.000000 redvypr-0.5.4/redvypr/icon/icon_v03.2.ico
--rw-r--r--   0 holterma  (1000) holterma  (1000)    38680 2022-06-06 07:01:15.000000 redvypr-0.5.4/redvypr/icon/icon_v03.2.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6006 2022-06-06 07:00:49.000000 redvypr-0.5.4/redvypr/icon/icon_v03.2.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     1150 2022-06-06 13:10:10.000000 redvypr-0.5.4/redvypr/icon/icon_v03.2_favicon.ico
--rw-r--r--   0 holterma  (1000) holterma  (1000)    24079 2022-06-06 09:05:14.000000 redvypr-0.5.4/redvypr/icon/icon_v03.2_small.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    16110 2022-06-06 09:07:27.000000 redvypr-0.5.4/redvypr/icon/icon_v03.2_verysmall.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    25790 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/icon_v03.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5560 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/icon_v03.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    28999 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/logo_merged.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     4997 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/logo_v01.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5197 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/logo_v02.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    45795 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/logo_v03.1.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6585 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/logo_v03.1.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     6498 2022-06-06 06:59:44.000000 redvypr-0.5.4/redvypr/icon/logo_v03.2.svg
--rw-r--r--   0 holterma  (1000) holterma  (1000)    27174 2022-06-05 18:22:35.000000 redvypr-0.5.4/redvypr/icon/logo_v03.2_small.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    27301 2022-03-17 04:29:20.000000 redvypr-0.5.4/redvypr/icon/redvypr_logo_v02.png
--rw-r--r--   0 holterma  (1000) holterma  (1000)    84616 2023-04-25 09:07:34.000000 redvypr-0.5.4/redvypr/redvypr.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.514166 redvypr-0.5.4/redvypr/utils/
--rw-r--r--   0 holterma  (1000) holterma  (1000)       23 2023-04-25 09:30:22.000000 redvypr-0.5.4/redvypr/utils/__init__.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.518166 redvypr-0.5.4/redvypr/utils/csv2dict/
--rw-r--r--   0 holterma  (1000) holterma  (1000)     1805 2023-04-25 09:29:49.000000 redvypr-0.5.4/redvypr/utils/csv2dict/NMEA.yaml
--rw-r--r--   0 holterma  (1000) holterma  (1000)     1077 2023-04-25 09:29:49.000000 redvypr-0.5.4/redvypr/utils/csv2dict/NMEA_functions.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)       24 2023-04-25 10:51:36.000000 redvypr-0.5.4/redvypr/utils/csv2dict/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     9886 2023-04-25 14:33:14.000000 redvypr-0.5.4/redvypr/utils/csv2dict/csv2dict.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      516 2022-04-19 05:07:55.000000 redvypr-0.5.4/redvypr/version.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.518166 redvypr-0.5.4/redvypr/widgets/
--rw-r--r--   0 holterma  (1000) holterma  (1000)        0 2022-12-02 05:59:19.000000 redvypr-0.5.4/redvypr/widgets/__init__.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     7664 2023-03-24 16:08:24.000000 redvypr-0.5.4/redvypr/widgets/datastream_widget.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    32322 2023-04-25 09:24:41.000000 redvypr-0.5.4/redvypr/widgets/gui_config_widgets.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     5964 2023-02-20 13:31:35.000000 redvypr-0.5.4/redvypr/widgets/standard_device_widgets.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)    53424 2023-04-25 09:24:41.000000 redvypr-0.5.4/redvypr/widgets/tmp.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.506166 redvypr-0.5.4/redvypr.egg-info/
--rw-r--r--   0 holterma  (1000) holterma  (1000)      813 2023-04-25 17:46:13.000000 redvypr-0.5.4/redvypr.egg-info/PKG-INFO
--rw-r--r--   0 holterma  (1000) holterma  (1000)     2401 2023-04-25 17:46:13.000000 redvypr-0.5.4/redvypr.egg-info/SOURCES.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2023-04-25 17:46:13.000000 redvypr-0.5.4/redvypr.egg-info/dependency_links.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)       49 2023-04-25 17:46:13.000000 redvypr-0.5.4/redvypr.egg-info/entry_points.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2022-03-17 04:32:33.000000 redvypr-0.5.4/redvypr.egg-info/not-zip-safe
--rw-r--r--   0 holterma  (1000) holterma  (1000)       55 2023-04-25 17:46:13.000000 redvypr-0.5.4/redvypr.egg-info/requires.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)        8 2023-04-25 17:46:13.000000 redvypr-0.5.4/redvypr.egg-info/top_level.txt
--rw-r--r--   0 holterma  (1000) holterma  (1000)       38 2023-04-25 17:46:13.518166 redvypr-0.5.4/setup.cfg
--rw-r--r--   0 holterma  (1000) holterma  (1000)     1647 2023-04-25 12:40:47.000000 redvypr-0.5.4/setup.py
-drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-25 17:46:13.518166 redvypr-0.5.4/test/
--rw-r--r--   0 holterma  (1000) holterma  (1000)     8082 2023-01-05 11:46:21.000000 redvypr-0.5.4/test/test_config.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)     4749 2023-02-18 13:42:06.000000 redvypr-0.5.4/test/test_configwidget.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      705 2023-03-29 03:33:18.000000 redvypr-0.5.4/test/test_devicescanwidget.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      383 2023-03-28 10:24:09.000000 redvypr-0.5.4/test/test_find_devices.py
--rw-r--r--   0 holterma  (1000) holterma  (1000)      221 2023-01-14 15:22:49.000000 redvypr-0.5.4/test/test_iored_1.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.194350 redvypr-0.5.5/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    35149 2022-03-17 04:29:20.000000 redvypr-0.5.5/LICENSE
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      813 2023-04-26 10:09:42.194350 redvypr-0.5.5/PKG-INFO
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     3030 2022-06-17 04:23:43.000000 redvypr-0.5.5/README.md
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.186350 redvypr-0.5.5/redvypr/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        5 2023-04-26 10:08:57.000000 redvypr-0.5.5/redvypr/VERSION
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      286 2023-04-25 09:31:02.000000 redvypr-0.5.5/redvypr/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    26761 2023-04-25 09:24:41.000000 redvypr-0.5.5/redvypr/config.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    10726 2023-04-25 09:24:41.000000 redvypr-0.5.5/redvypr/configdata.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    40721 2023-04-25 10:43:41.000000 redvypr-0.5.5/redvypr/data_packets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    27230 2023-04-25 04:44:39.000000 redvypr-0.5.5/redvypr/device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.186350 redvypr-0.5.5/redvypr/devices/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      135 2023-04-10 17:52:06.000000 redvypr-0.5.5/redvypr/devices/__init__.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.186350 redvypr-0.5.5/redvypr/devices/db/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        0 2023-03-29 11:49:05.000000 redvypr-0.5.5/redvypr/devices/db/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1872 2022-12-11 06:19:03.000000 redvypr-0.5.5/redvypr/devices/db/influxdb_device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.186350 redvypr-0.5.5/redvypr/devices/develop/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       24 2023-04-19 10:29:29.000000 redvypr-0.5.5/redvypr/devices/develop/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    37708 2023-03-26 05:06:47.000000 redvypr-0.5.5/redvypr/devices/develop/csvlogger.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.186350 redvypr-0.5.5/redvypr/devices/fileio/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       56 2023-04-19 10:29:41.000000 redvypr-0.5.5/redvypr/devices/fileio/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    28729 2023-04-06 05:28:30.000000 redvypr-0.5.5/redvypr/devices/fileio/rawdatalogger.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    16771 2023-04-05 18:41:57.000000 redvypr-0.5.5/redvypr/devices/fileio/rawdatareplay.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.190350 redvypr-0.5.5/redvypr/devices/interface/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       28 2023-04-10 17:40:41.000000 redvypr-0.5.5/redvypr/devices/interface/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    15186 2023-04-17 11:51:35.000000 redvypr-0.5.5/redvypr/devices/interface/serial_device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.190350 redvypr-0.5.5/redvypr/devices/network/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       77 2023-03-29 11:42:45.000000 redvypr-0.5.5/redvypr/devices/network/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)   101562 2023-04-25 04:50:06.000000 redvypr-0.5.5/redvypr/devices/network/iored.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    33337 2023-01-09 05:25:09.000000 redvypr-0.5.5/redvypr/devices/network/network_device.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     8771 2023-04-17 17:53:48.000000 redvypr-0.5.5/redvypr/devices/network/zeromq_device.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.190350 redvypr-0.5.5/redvypr/devices/plot/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       72 2023-04-10 17:41:27.000000 redvypr-0.5.5/redvypr/devices/plot/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    31897 2023-04-25 09:24:41.000000 redvypr-0.5.5/redvypr/devices/plot/plot.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    23149 2023-04-25 09:24:41.000000 redvypr-0.5.5/redvypr/devices/plot/plot_widgets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2907 2023-04-17 17:53:38.000000 redvypr-0.5.5/redvypr/devices/plot/rawdatadisp.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.190350 redvypr-0.5.5/redvypr/devices/processing/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       79 2023-04-10 17:58:08.000000 redvypr-0.5.5/redvypr/devices/processing/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2147 2023-04-25 13:56:48.000000 redvypr-0.5.5/redvypr/devices/processing/csvparser.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6525 2023-04-25 13:56:08.000000 redvypr-0.5.5/redvypr/devices/processing/nmeaparser.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5761 2023-04-17 17:54:15.000000 redvypr-0.5.5/redvypr/devices/processing/sensor_raw2unit.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.190350 redvypr-0.5.5/redvypr/devices/test/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       26 2023-03-29 11:50:28.000000 redvypr-0.5.5/redvypr/devices/test/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2428 2023-04-26 09:38:24.000000 redvypr-0.5.5/redvypr/devices/test/test_device.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      990 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/files.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    28258 2023-04-26 09:35:19.000000 redvypr-0.5.5/redvypr/gui.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.194350 redvypr-0.5.5/redvypr/icon/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    11374 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/icon_v02.ico
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    10980 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/icon_v02.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    39662 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/icon_v03.1.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5924 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/icon_v03.1.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    34925 2022-06-05 18:16:36.000000 redvypr-0.5.5/redvypr/icon/icon_v03.1_small.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    38644 2022-06-06 07:01:58.000000 redvypr-0.5.5/redvypr/icon/icon_v03.2.ico
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    38680 2022-06-06 07:01:15.000000 redvypr-0.5.5/redvypr/icon/icon_v03.2.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6006 2022-06-06 07:00:49.000000 redvypr-0.5.5/redvypr/icon/icon_v03.2.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1150 2022-06-06 13:10:10.000000 redvypr-0.5.5/redvypr/icon/icon_v03.2_favicon.ico
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    24079 2022-06-06 09:05:14.000000 redvypr-0.5.5/redvypr/icon/icon_v03.2_small.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    16110 2022-06-06 09:07:27.000000 redvypr-0.5.5/redvypr/icon/icon_v03.2_verysmall.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    25790 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/icon_v03.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5560 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/icon_v03.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    28999 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/logo_merged.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     4997 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/logo_v01.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5197 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/logo_v02.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    45795 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/logo_v03.1.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6585 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/logo_v03.1.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     6498 2022-06-06 06:59:44.000000 redvypr-0.5.5/redvypr/icon/logo_v03.2.svg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    27174 2022-06-05 18:22:35.000000 redvypr-0.5.5/redvypr/icon/logo_v03.2_small.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    27301 2022-03-17 04:29:20.000000 redvypr-0.5.5/redvypr/icon/redvypr_logo_v02.png
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    84769 2023-04-26 09:30:24.000000 redvypr-0.5.5/redvypr/redvypr.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.194350 redvypr-0.5.5/redvypr/utils/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       23 2023-04-25 09:30:22.000000 redvypr-0.5.5/redvypr/utils/__init__.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.194350 redvypr-0.5.5/redvypr/utils/csv2dict/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1805 2023-04-25 09:29:49.000000 redvypr-0.5.5/redvypr/utils/csv2dict/NMEA.yaml
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1077 2023-04-25 09:29:49.000000 redvypr-0.5.5/redvypr/utils/csv2dict/NMEA_functions.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       24 2023-04-25 10:51:36.000000 redvypr-0.5.5/redvypr/utils/csv2dict/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     9886 2023-04-25 14:33:14.000000 redvypr-0.5.5/redvypr/utils/csv2dict/csv2dict.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      516 2022-04-19 05:07:55.000000 redvypr-0.5.5/redvypr/version.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.194350 redvypr-0.5.5/redvypr/widgets/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        0 2022-12-02 05:59:19.000000 redvypr-0.5.5/redvypr/widgets/__init__.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     7664 2023-03-24 16:08:24.000000 redvypr-0.5.5/redvypr/widgets/datastream_widget.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    32322 2023-04-25 09:24:41.000000 redvypr-0.5.5/redvypr/widgets/gui_config_widgets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     5964 2023-02-20 13:31:35.000000 redvypr-0.5.5/redvypr/widgets/standard_device_widgets.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)    53424 2023-04-25 09:24:41.000000 redvypr-0.5.5/redvypr/widgets/tmp.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.186350 redvypr-0.5.5/redvypr.egg-info/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      813 2023-04-26 10:09:42.000000 redvypr-0.5.5/redvypr.egg-info/PKG-INFO
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     2401 2023-04-26 10:09:42.000000 redvypr-0.5.5/redvypr.egg-info/SOURCES.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2023-04-26 10:09:42.000000 redvypr-0.5.5/redvypr.egg-info/dependency_links.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       49 2023-04-26 10:09:42.000000 redvypr-0.5.5/redvypr.egg-info/entry_points.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        1 2022-03-17 04:32:33.000000 redvypr-0.5.5/redvypr.egg-info/not-zip-safe
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       55 2023-04-26 10:09:42.000000 redvypr-0.5.5/redvypr.egg-info/requires.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)        8 2023-04-26 10:09:42.000000 redvypr-0.5.5/redvypr.egg-info/top_level.txt
+-rw-r--r--   0 holterma  (1000) holterma  (1000)       38 2023-04-26 10:09:42.194350 redvypr-0.5.5/setup.cfg
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     1647 2023-04-25 12:40:47.000000 redvypr-0.5.5/setup.py
+drwxr-xr-x   0 holterma  (1000) holterma  (1000)        0 2023-04-26 10:09:42.194350 redvypr-0.5.5/test/
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     8082 2023-01-05 11:46:21.000000 redvypr-0.5.5/test/test_config.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)     4749 2023-02-18 13:42:06.000000 redvypr-0.5.5/test/test_configwidget.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      705 2023-03-29 03:33:18.000000 redvypr-0.5.5/test/test_devicescanwidget.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      383 2023-03-28 10:24:09.000000 redvypr-0.5.5/test/test_find_devices.py
+-rw-r--r--   0 holterma  (1000) holterma  (1000)      221 2023-01-14 15:22:49.000000 redvypr-0.5.5/test/test_iored_1.py
```

### Comparing `redvypr-0.5.4/LICENSE` & `redvypr-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/PKG-INFO` & `redvypr-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvypr
-Version: 0.5.4
+Version: 0.5.5
 Summary: redvypr: REaltime Data Viewer and PRocessor (in PYthon)
 Home-page: https://github.com/redvypr/redvypr
 Author: Peter Holtermann
 Author-email: peter.holtermann@io-warnemuende.de
 License: GPLv03
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `redvypr-0.5.4/README.md` & `redvypr-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/config.py` & `redvypr-0.5.5/redvypr/config.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/configdata.py` & `redvypr-0.5.5/redvypr/configdata.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/data_packets.py` & `redvypr-0.5.5/redvypr/data_packets.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/device.py` & `redvypr-0.5.5/redvypr/device.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/db/influxdb_device.py` & `redvypr-0.5.5/redvypr/devices/db/influxdb_device.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/develop/csvlogger.py` & `redvypr-0.5.5/redvypr/devices/develop/csvlogger.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/fileio/rawdatalogger.py` & `redvypr-0.5.5/redvypr/devices/fileio/rawdatalogger.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/fileio/rawdatareplay.py` & `redvypr-0.5.5/redvypr/devices/fileio/rawdatareplay.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/interface/serial_device.py` & `redvypr-0.5.5/redvypr/devices/interface/serial_device.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/network/iored.py` & `redvypr-0.5.5/redvypr/devices/network/iored.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/network/network_device.py` & `redvypr-0.5.5/redvypr/devices/network/network_device.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/network/zeromq_device.py` & `redvypr-0.5.5/redvypr/devices/network/zeromq_device.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/plot/plot.py` & `redvypr-0.5.5/redvypr/devices/plot/plot.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/plot/plot_widgets.py` & `redvypr-0.5.5/redvypr/devices/plot/plot_widgets.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/plot/rawdatadisp.py` & `redvypr-0.5.5/redvypr/devices/plot/rawdatadisp.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/processing/csvparser.py` & `redvypr-0.5.5/redvypr/devices/processing/csvparser.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/processing/nmeaparser.py` & `redvypr-0.5.5/redvypr/devices/processing/nmeaparser.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/processing/sensor_raw2unit.py` & `redvypr-0.5.5/redvypr/devices/processing/sensor_raw2unit.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/devices/test/test_device.py` & `redvypr-0.5.5/redvypr/devices/test/test_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,13 +64,19 @@
                 break
 
         dstr = str(config['string_send'])
         #print(dstr)
         dataqueue.put(dstr)
         dataqueue.put({'count': i})
         dataqueue.put({'count': i+10,'_redvypr':{'device':'t2'}})
+        # Calculate some sine
+        data_rand = float(np.random.rand(1)-0.5)
+        f_sin = 1/30 # Frequency in Hz
+        A_sin = 10 # Amplitude
+        data_sine = float(A_sin * np.sin(f_sin * time.time()))
+        dataqueue.put({'sine_rand': data_rand + data_sine})
         i+=1
         time.sleep(config['delay_s'])
```

### Comparing `redvypr-0.5.4/redvypr/files.py` & `redvypr-0.5.5/redvypr/files.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/gui.py` & `redvypr-0.5.5/redvypr/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         self.mp_label = QtWidgets.QLabel('Multiprocessing options')
         self.mp_thread = QtWidgets.QRadioButton('Thread')
         self.mp_multi = QtWidgets.QRadioButton('Multiprocessing')
         self.mp_multi.setChecked(True)
         self.mp_group = QtWidgets.QButtonGroup()
         self.mp_group.addButton(self.mp_thread)
         self.mp_group.addButton(self.mp_multi)
+        self.mp_thread.setChecked(True)
 
         self.layout = QtWidgets.QFormLayout(self)
         self.layout.addRow(self.devicetree)
         self.layout.addRow(self.deviceinfo)
         self.layout.addRow(self.mp_label)
         self.layout.addRow(self.mp_thread, self.mp_multi)
         self.layout.addRow(self.devnamelabel, self.devname)
```

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v02.ico` & `redvypr-0.5.5/redvypr/icon/icon_v02.ico`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v02.png` & `redvypr-0.5.5/redvypr/icon/icon_v02.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.1.png` & `redvypr-0.5.5/redvypr/icon/icon_v03.1.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.1.svg` & `redvypr-0.5.5/redvypr/icon/icon_v03.1.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.1_small.png` & `redvypr-0.5.5/redvypr/icon/icon_v03.1_small.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.2.ico` & `redvypr-0.5.5/redvypr/icon/icon_v03.2.ico`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.2.png` & `redvypr-0.5.5/redvypr/icon/icon_v03.2.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.2.svg` & `redvypr-0.5.5/redvypr/icon/icon_v03.2.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.2_favicon.ico` & `redvypr-0.5.5/redvypr/icon/icon_v03.2_favicon.ico`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.2_small.png` & `redvypr-0.5.5/redvypr/icon/icon_v03.2_small.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.2_verysmall.png` & `redvypr-0.5.5/redvypr/icon/icon_v03.2_verysmall.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.png` & `redvypr-0.5.5/redvypr/icon/icon_v03.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/icon_v03.svg` & `redvypr-0.5.5/redvypr/icon/icon_v03.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/logo_merged.svg` & `redvypr-0.5.5/redvypr/icon/logo_merged.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/logo_v01.svg` & `redvypr-0.5.5/redvypr/icon/logo_v01.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/logo_v02.svg` & `redvypr-0.5.5/redvypr/icon/logo_v02.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/logo_v03.1.png` & `redvypr-0.5.5/redvypr/icon/logo_v03.1.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/logo_v03.1.svg` & `redvypr-0.5.5/redvypr/icon/logo_v03.1.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/logo_v03.2.svg` & `redvypr-0.5.5/redvypr/icon/logo_v03.2.svg`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/logo_v03.2_small.png` & `redvypr-0.5.5/redvypr/icon/logo_v03.2_small.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/icon/redvypr_logo_v02.png` & `redvypr-0.5.5/redvypr/icon/redvypr_logo_v02.png`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/redvypr.py` & `redvypr-0.5.5/redvypr/redvypr.py`

 * *Files 0% similar despite different names*

```diff
@@ -2074,14 +2074,16 @@
             'Available screen size: {:d} x {:d} using {:d} x {:d}'.format(rect.width(), rect.height(), width, height))
         ex = redvyprMainWidget(width=width, height=height, config=config_all,hostname=hostname,hostinfo_opt=hostinfo_opt)
 
         sys.exit(app.exec_())
 
 
 if __name__ == '__main__':
+    #https://stackoverflow.com/questions/46335842/python-multiprocessing-throws-error-with-argparse-and-pyinstaller
+    multiprocessing.freeze_support()
     redvypr_main()
```

### Comparing `redvypr-0.5.4/redvypr/utils/csv2dict/NMEA.yaml` & `redvypr-0.5.5/redvypr/utils/csv2dict/NMEA.yaml`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/utils/csv2dict/NMEA_functions.py` & `redvypr-0.5.5/redvypr/utils/csv2dict/NMEA_functions.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/utils/csv2dict/csv2dict.py` & `redvypr-0.5.5/redvypr/utils/csv2dict/csv2dict.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/version.py` & `redvypr-0.5.5/redvypr/version.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/widgets/datastream_widget.py` & `redvypr-0.5.5/redvypr/widgets/datastream_widget.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/widgets/gui_config_widgets.py` & `redvypr-0.5.5/redvypr/widgets/gui_config_widgets.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/widgets/standard_device_widgets.py` & `redvypr-0.5.5/redvypr/widgets/standard_device_widgets.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr/widgets/tmp.py` & `redvypr-0.5.5/redvypr/widgets/tmp.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/redvypr.egg-info/PKG-INFO` & `redvypr-0.5.5/redvypr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvypr
-Version: 0.5.4
+Version: 0.5.5
 Summary: redvypr: REaltime Data Viewer and PRocessor (in PYthon)
 Home-page: https://github.com/redvypr/redvypr
 Author: Peter Holtermann
 Author-email: peter.holtermann@io-warnemuende.de
 License: GPLv03
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `redvypr-0.5.4/redvypr.egg-info/SOURCES.txt` & `redvypr-0.5.5/redvypr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/setup.py` & `redvypr-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/test/test_config.py` & `redvypr-0.5.5/test/test_config.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/test/test_configwidget.py` & `redvypr-0.5.5/test/test_configwidget.py`

 * *Files identical despite different names*

### Comparing `redvypr-0.5.4/test/test_devicescanwidget.py` & `redvypr-0.5.5/test/test_devicescanwidget.py`

 * *Files identical despite different names*

