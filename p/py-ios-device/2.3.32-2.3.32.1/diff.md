# Comparing `tmp/py_ios_device-2.3.32.tar.gz` & `tmp/py_ios_device-2.3.32.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ios_device-2.3.32.tar", last modified: Thu Apr 20 03:24:56 2023, max compression
+gzip compressed data, was "py_ios_device-2.3.32.1.tar", last modified: Wed Apr 26 06:22:31 2023, max compression
```

## Comparing `py_ios_device-2.3.32.tar` & `py_ios_device-2.3.32.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.285835 py_ios_device-2.3.32/
--rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/LICENSE
--rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/MANIFEST.in
--rw-r--r--   0 rongcloud   (501) staff       (20)    11009 2023-04-20 03:24:56.285654 py_ios_device-2.3.32/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)    10544 2023-04-20 03:06:40.000000 py_ios_device-2.3.32/README.md
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.270862 py_ios_device-2.3.32/demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/demo/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/demo/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/demo/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32/demo/installation_proxy.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.274316 py_ios_device-2.3.32/demo/instrument_demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/demo/instrument_demo/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/demo/instrument_demo/activity.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 py_ios_device-2.3.32/demo/instrument_demo/app_lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/demo/instrument_demo/applictionListing.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32/demo/instrument_demo/channel.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-04-07 02:39:15.000000 py_ios_device-2.3.32/demo/instrument_demo/coreprofilesessiontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-02-21 09:11:42.000000 py_ios_device-2.3.32/demo/instrument_demo/coreprofilesessiontap_parse.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 py_ios_device-2.3.32/demo/instrument_demo/deviceinfo.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-04-07 02:35:34.000000 py_ios_device-2.3.32/demo/instrument_demo/energy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-03-17 08:58:28.000000 py_ios_device-2.3.32/demo/instrument_demo/gpu.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/demo/instrument_demo/graphics.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-03-17 08:58:33.000000 py_ios_device-2.3.32/demo/instrument_demo/launchAPP.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32/demo/instrument_demo/mobileNotifications.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32/demo/instrument_demo/netstatPID.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 py_ios_device-2.3.32/demo/instrument_demo/networking.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 py_ios_device-2.3.32/demo/instrument_demo/sysmontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/demo/instrument_demo/xcuitest.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/demo/mobile_config.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/demo/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/demo/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/demo/syslog.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.274878 py_ios_device-2.3.32/ios_device/
--rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)       23 2023-04-20 03:24:54.000000 py_ios_device-2.3.32/ios_device/__version__.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.276450 py_ios_device-2.3.32/ios_device/cli/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/cli/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    29436 2023-04-20 02:52:36.000000 py_ios_device-2.3.32/ios_device/cli/base.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 py_ios_device-2.3.32/ios_device/cli/cli.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    19123 2023-04-20 03:02:09.000000 py_ios_device-2.3.32/ios_device/cli/instruments.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    10985 2023-01-04 04:18:58.000000 py_ios_device-2.3.32/ios_device/cli/mobile.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/main.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32/ios_device/py_ios_device.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.280579 py_ios_device-2.3.32/ios_device/servers/
--rw-r--r--   0 rongcloud   (501) staff       (20)     6867 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/Installation.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32/ios_device/servers/Instrument.py
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/servers/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/amfi.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      993 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/diagnostics_relay.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 py_ios_device-2.3.32/ios_device/servers/dvt.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 py_ios_device-2.3.32/ios_device/servers/house_arrest.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/image_mounter.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 py_ios_device-2.3.32/ios_device/servers/mc_install.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/notification_proxy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 py_ios_device-2.3.32/ios_device/servers/os_trace.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/servers/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32/ios_device/servers/simulate_location.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32/ios_device/servers/spring_board.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32/ios_device/servers/syslog.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 py_ios_device-2.3.32/ios_device/servers/testmanagerd.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      718 2023-04-07 04:00:58.000000 py_ios_device-2.3.32/ios_device/servers/wireless.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.284744 py_ios_device-2.3.32/ios_device/util/
--rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/util/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/util/api_util.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32/ios_device/util/bpylist2.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/util/ca.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/util/constants.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/util/dtx_msg.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/util/exceptions.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/util/forward.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 py_ios_device-2.3.32/ios_device/util/gpu_decode.py
--rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32/ios_device/util/kc_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32/ios_device/util/kperf_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32/ios_device/util/lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32/ios_device/util/lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32/ios_device/util/plist_service.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2022-09-26 09:47:22.000000 py_ios_device-2.3.32/ios_device/util/plistlib.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32/ios_device/util/usbmux.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 py_ios_device-2.3.32/ios_device/util/utils.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32/ios_device/util/variables.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-20 03:24:56.285475 py_ios_device-2.3.32/py_ios_device.egg-info/
--rw-r--r--   0 rongcloud   (501) staff       (20)    11009 2023-04-20 03:24:56.000000 py_ios_device-2.3.32/py_ios_device.egg-info/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)     2427 2023-04-20 03:24:56.000000 py_ios_device-2.3.32/py_ios_device.egg-info/SOURCES.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-04-20 03:24:56.000000 py_ios_device-2.3.32/py_ios_device.egg-info/dependency_links.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-04-20 03:24:56.000000 py_ios_device-2.3.32/py_ios_device.egg-info/entry_points.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-04-20 03:24:56.000000 py_ios_device-2.3.32/py_ios_device.egg-info/requires.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-04-20 03:24:56.000000 py_ios_device-2.3.32/py_ios_device.egg-info/top_level.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32/requirements.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-04-20 03:24:56.285879 py_ios_device-2.3.32/setup.cfg
--rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32/setup.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.779176 py_ios_device-2.3.32.1/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/LICENSE
+-rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/MANIFEST.in
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11011 2023-04-26 06:22:31.778979 py_ios_device-2.3.32.1/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10544 2023-04-20 03:06:40.000000 py_ios_device-2.3.32.1/README.md
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.760948 py_ios_device-2.3.32.1/demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32.1/demo/installation_proxy.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.764445 py_ios_device-2.3.32.1/demo/instrument_demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/activity.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/demo/instrument_demo/app_lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/applictionListing.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.1/demo/instrument_demo/channel.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-02-21 09:11:42.000000 py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap_parse.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.1/demo/instrument_demo/deviceinfo.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.1/demo/instrument_demo/energy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-03-17 08:58:28.000000 py_ios_device-2.3.32.1/demo/instrument_demo/gpu.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/graphics.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-03-17 08:58:33.000000 py_ios_device-2.3.32.1/demo/instrument_demo/launchAPP.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32.1/demo/instrument_demo/mobileNotifications.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.1/demo/instrument_demo/netstatPID.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.1/demo/instrument_demo/networking.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 py_ios_device-2.3.32.1/demo/instrument_demo/sysmontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/xcuitest.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/mobile_config.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/syslog.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.765039 py_ios_device-2.3.32.1/ios_device/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-04-26 06:17:20.000000 py_ios_device-2.3.32.1/ios_device/__version__.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.767284 py_ios_device-2.3.32.1/ios_device/cli/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/cli/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    29436 2023-04-20 02:52:36.000000 py_ios_device-2.3.32.1/ios_device/cli/base.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 py_ios_device-2.3.32.1/ios_device/cli/cli.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    19123 2023-04-20 03:02:09.000000 py_ios_device-2.3.32.1/ios_device/cli/instruments.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 py_ios_device-2.3.32.1/ios_device/cli/mobile.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/main.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/py_ios_device.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.773422 py_ios_device-2.3.32.1/ios_device/servers/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 py_ios_device-2.3.32.1/ios_device/servers/Installation.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.1/ios_device/servers/Instrument.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/servers/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/amfi.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      993 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/diagnostics_relay.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.1/ios_device/servers/dvt.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 py_ios_device-2.3.32.1/ios_device/servers/house_arrest.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/image_mounter.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 py_ios_device-2.3.32.1/ios_device/servers/mc_install.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/notification_proxy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 py_ios_device-2.3.32.1/ios_device/servers/os_trace.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32.1/ios_device/servers/simulate_location.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32.1/ios_device/servers/spring_board.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32.1/ios_device/servers/syslog.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 py_ios_device-2.3.32.1/ios_device/servers/testmanagerd.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.778045 py_ios_device-2.3.32.1/ios_device/util/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/util/api_util.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32.1/ios_device/util/bpylist2.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/ca.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/constants.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/util/dtx_msg.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/exceptions.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/forward.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 py_ios_device-2.3.32.1/ios_device/util/gpu_decode.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/util/kc_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/util/kperf_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/util/lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32.1/ios_device/util/lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/util/plist_service.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 py_ios_device-2.3.32.1/ios_device/util/plistlib.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32.1/ios_device/util/usbmux.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 py_ios_device-2.3.32.1/ios_device/util/utils.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32.1/ios_device/util/variables.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.778792 py_ios_device-2.3.32.1/py_ios_device.egg-info/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11011 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2406 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/SOURCES.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/dependency_links.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/entry_points.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/requires.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/top_level.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/requirements.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-04-26 06:22:31.779216 py_ios_device-2.3.32.1/setup.cfg
+-rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.1/setup.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      959 2023-04-20 03:34:06.000000 py_ios_device-2.3.32.1/setup2.py
```

### Comparing `py_ios_device-2.3.32/LICENSE` & `py_ios_device-2.3.32.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/PKG-INFO` & `py_ios_device-2.3.32.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ios_device
-Version: 2.3.32
+Version: 2.3.32.1
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.3.32/README.md` & `py_ios_device-2.3.32.1/README.md`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/afc.py` & `py_ios_device-2.3.32.1/demo/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/crash_log.py` & `py_ios_device-2.3.32.1/demo/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/installation_proxy.py` & `py_ios_device-2.3.32.1/demo/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/activity.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/activity.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/app_lifecycle.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/app_lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/applictionListing.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/applictionListing.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/coreprofilesessiontap.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/coreprofilesessiontap_parse.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap_parse.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/deviceinfo.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/gpu.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/gpu.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/graphics.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/graphics.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/launchAPP.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/launchAPP.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/mobileNotifications.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/mobileNotifications.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/netstatPID.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/netstatPID.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/networking.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/networking.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/sysmontap.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/sysmontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/instrument_demo/xcuitest.py` & `py_ios_device-2.3.32.1/demo/instrument_demo/xcuitest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/mobile_config.py` & `py_ios_device-2.3.32.1/demo/mobile_config.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/pcapd.py` & `py_ios_device-2.3.32.1/demo/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/screenshotr.py` & `py_ios_device-2.3.32.1/demo/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/demo/syslog.py` & `py_ios_device-2.3.32.1/demo/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/cli/base.py` & `py_ios_device-2.3.32.1/ios_device/cli/base.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/cli/cli.py` & `py_ios_device-2.3.32.1/ios_device/cli/cli.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/cli/instruments.py` & `py_ios_device-2.3.32.1/ios_device/cli/instruments.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/cli/mobile.py` & `py_ios_device-2.3.32.1/ios_device/cli/mobile.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,24 +143,26 @@
     """ application options """
     pass
 
 
 @apps.command('list', cls=Command)
 @click.option('-u', '--user', is_flag=True, help='include user apps')
 @click.option('-s', '--system', is_flag=True, help='include system apps')
-def apps_list(udid, network, format, user, system):
-    """ list installed apps """
-    app_types = []
+@click.option('--size', is_flag=True, help='get app size')
+def apps_list(udid, network, format, user, system, size):
+    """ list installed apps `-size` get app size """
+    options = {}
     if user:
-        app_types.append('User')
+        options['ApplicationType'] = 'User'
     if system:
-        app_types.append('System')
-    if not app_types:
-        app_types = ['User', 'System']
-    print_json(InstallationProxyService(udid=udid, network=network, logger=log).get_apps(app_types), format=format)
+        options['ApplicationType'] = 'System'
+    if size:
+        options['ReturnAttributes'] = ['CFBundleIdentifier', 'CFBundleVersion', 'CFBundleDisplayName',
+                                       'StaticDiskUsage', 'DynamicDiskUsage']
+    print_json(InstallationProxyService(udid=udid, network=network, logger=log).apps_info(options), format=format)
 
 
 @apps.command('uninstall', cls=Command)
 @click.option('-b', '--bundle_id', default=None, help='Process app bundleId to filter')
 def uninstall(udid, network, format, bundle_id):
     """ uninstall app by given bundle_id """
     print_json(InstallationProxyService(udid=udid, network=network, logger=log).uninstall(bundle_id))
```

### Comparing `py_ios_device-2.3.32/ios_device/py_ios_device.py` & `py_ios_device-2.3.32.1/ios_device/py_ios_device.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/Installation.py` & `py_ios_device-2.3.32.1/ios_device/servers/Installation.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,34 +95,37 @@
             afc.set_file_contents("/" + os.path.basename(ipaPath), open(ipaPath, "rb").read())
         cmd = {"Command": cmd,
                "ClientOptions": options,
                "PackagePath": os.path.basename(ipaPath)}
         self.service.send_plist(cmd)
         return self.watch_completion(handler, args)
 
-    def install(self, ipaPath, options={}, handler=None, *args):
-        return self.install_or_upgrade(ipaPath, "Install", options, handler, args)
+    def install(self, ipaPath, options: dict = None, handler=None, *args):
+        return self.install_or_upgrade(ipaPath, "Install", options or {}, handler, args)
 
-    def upgrade(self, ipaPath, options={}, handler=None, *args):
-        return self.install_or_upgrade(ipaPath, "Upgrade", options, handler, args)
+    def upgrade(self, ipaPath, options: dict = None, handler=None, *args):
+        return self.install_or_upgrade(ipaPath, "Upgrade", options or {}, handler, args)
 
-    def check_capabilities_match(self, capabilities, options={}):
+    def check_capabilities_match(self, capabilities, options: dict = None):
         cmd = {"Command": "CheckCapabilitiesMatch",
-               "ClientOptions": options}
+               "ClientOptions": options or {}}
 
         if capabilities:
             cmd["Capabilities"] = capabilities
 
         self.service.send_plist(cmd)
         result = self.service.recv_plist().get("LookupResult")
         return result
 
-    def browse(self, options={}, attributes=None, handler=None, *args):
+    def browse(self, options=None, attributes=None, app_types=None, handler=None, *args):
+        options = options or {}
         if attributes:
             options["ReturnAttributes"] = attributes
+        if app_types:
+            options["ApplicationType"] = app_types
 
         cmd = {"Command": "Browse",
                "ClientOptions": options}
 
         self.service.send_plist(cmd)
 
         result = []
@@ -136,58 +139,64 @@
                 result += data
 
             if z.get("Status") == "Complete":
                 break
 
         return result
 
-    def apps_info(self, options={}):
+    def apps_info(self, options: dict = None):
         cmd = {"Command": "Lookup",
-               "ClientOptions": options}
+               "ClientOptions": options or {}}
 
         self.service.send_plist(cmd)
         return self.service.recv_plist().get('LookupResult')
 
-    def archive(self, bid, options={}, handler=None, *args):
-        self.send_cmd_for_bid(bid, "Archive", options, handler, args)
+    def archive(self, bid, options: dict = None, handler=None, *args):
+        self.send_cmd_for_bid(bid, "Archive", options or {}, handler, args)
 
-    def restore_archive(self, bid, options={}, handler=None, *args):
-        self.send_cmd_for_bid(bid, "Restore", options, handler, args)
+    def restore_archive(self, bid, options: dict = None, handler=None, *args):
+        self.send_cmd_for_bid(bid, "Restore", options or {}, handler, args)
 
-    def remove_archive(self, bid, options={}, handler=None, *args):
-        self.send_cmd_for_bid(bid, "RemoveArchive", options, handler, args)
+    def remove_archive(self, bid, options: dict = None, handler=None, *args):
+        self.send_cmd_for_bid(bid, "RemoveArchive", options or {}, handler, args)
 
-    def archives_info(self, options={}):
+    def archives_info(self, options: dict = None):
         cmd = {"Command": "LookupArchive",
-               "ClientOptions": options}
+               "ClientOptions": options or {}}
         return self.service.send_plist(cmd).get("LookupResult")
 
     def search_path_for_bid(self, bid):
         path = None
         for a in self.get_apps(appTypes=["User", "System"]):
             if a.get("CFBundleIdentifier") == bid:
                 path = a.get("Path") + "/" + a.get("CFBundleExecutable")
         return path
 
-    def get_apps(self, appTypes=["User"]):
+    def get_apps(self, appTypes=None):
+        if appTypes is None:
+            appTypes = ["User"]
         return [app for app in self.apps_info().values()
                 if app.get("ApplicationType") in appTypes]
 
-    def print_apps(self, appType=["User"]):
+    def print_apps(self, appType=None):
+        if appType is None:
+            appType = ["User"]
         for app in self.get_apps(appType):
             print(("%s : %s => %s" % (app.get("CFBundleDisplayName"),
                                       app.get("CFBundleIdentifier"),
                                       app.get("Path") if app.get("Path")
                                       else app.get("Container"))).encode('utf-8'))
 
     def find_bundle_id(self, bundle_id):
         for app in self.get_apps():
             if app.get('CFBundleIdentifier') == bundle_id:
                 return app
 
-    def get_apps_bid(self, appTypes=["User"]):
+    def get_apps_bid(self, appTypes=None):
+        if appTypes is None:
+            appTypes = ["User"]
         return [app["CFBundleIdentifier"]
                 for app in self.get_apps()
                 if app.get("ApplicationType") in appTypes]
 
     def close(self):
         self.service.close()
```

### Comparing `py_ios_device-2.3.32/ios_device/servers/Instrument.py` & `py_ios_device-2.3.32.1/ios_device/servers/Instrument.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/afc.py` & `py_ios_device-2.3.32.1/ios_device/servers/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/amfi.py` & `py_ios_device-2.3.32.1/ios_device/servers/amfi.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/crash_log.py` & `py_ios_device-2.3.32.1/ios_device/servers/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/diagnostics_relay.py` & `py_ios_device-2.3.32.1/ios_device/servers/diagnostics_relay.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/dvt.py` & `py_ios_device-2.3.32.1/ios_device/servers/dvt.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/house_arrest.py` & `py_ios_device-2.3.32.1/ios_device/servers/house_arrest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/image_mounter.py` & `py_ios_device-2.3.32.1/ios_device/servers/image_mounter.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/mc_install.py` & `py_ios_device-2.3.32.1/ios_device/servers/mc_install.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/notification_proxy.py` & `py_ios_device-2.3.32.1/ios_device/servers/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/os_trace.py` & `py_ios_device-2.3.32.1/ios_device/servers/os_trace.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/pcapd.py` & `py_ios_device-2.3.32.1/ios_device/servers/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/screenshotr.py` & `py_ios_device-2.3.32.1/ios_device/servers/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/simulate_location.py` & `py_ios_device-2.3.32.1/ios_device/servers/simulate_location.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/spring_board.py` & `py_ios_device-2.3.32.1/ios_device/servers/spring_board.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/syslog.py` & `py_ios_device-2.3.32.1/ios_device/servers/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/servers/testmanagerd.py` & `py_ios_device-2.3.32.1/ios_device/servers/testmanagerd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/__init__.py` & `py_ios_device-2.3.32.1/ios_device/util/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/api_util.py` & `py_ios_device-2.3.32.1/ios_device/util/api_util.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/bpylist2.py` & `py_ios_device-2.3.32.1/ios_device/util/bpylist2.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/ca.py` & `py_ios_device-2.3.32.1/ios_device/util/ca.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/constants.py` & `py_ios_device-2.3.32.1/ios_device/util/constants.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/dtx_msg.py` & `py_ios_device-2.3.32.1/ios_device/util/dtx_msg.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/exceptions.py` & `py_ios_device-2.3.32.1/ios_device/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/forward.py` & `py_ios_device-2.3.32.1/ios_device/util/forward.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/gpu_decode.py` & `py_ios_device-2.3.32.1/ios_device/util/gpu_decode.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/kc_data.py` & `py_ios_device-2.3.32.1/ios_device/util/kc_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/kperf_data.py` & `py_ios_device-2.3.32.1/ios_device/util/kperf_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/lifecycle.py` & `py_ios_device-2.3.32.1/ios_device/util/lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/lockdown.py` & `py_ios_device-2.3.32.1/ios_device/util/lockdown.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/plist_service.py` & `py_ios_device-2.3.32.1/ios_device/util/plist_service.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/plistlib.py` & `py_ios_device-2.3.32.1/ios_device/util/plistlib.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/usbmux.py` & `py_ios_device-2.3.32.1/ios_device/util/usbmux.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/utils.py` & `py_ios_device-2.3.32.1/ios_device/util/utils.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/ios_device/util/variables.py` & `py_ios_device-2.3.32.1/ios_device/util/variables.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32/py_ios_device.egg-info/PKG-INFO` & `py_ios_device-2.3.32.1/py_ios_device.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ios-device
-Version: 2.3.32
+Version: 2.3.32.1
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.3.32/py_ios_device.egg-info/SOURCES.txt` & `py_ios_device-2.3.32.1/py_ios_device.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+setup2.py
 demo/__init__.py
 demo/afc.py
 demo/crash_log.py
 demo/installation_proxy.py
 demo/mobile_config.py
 demo/pcapd.py
 demo/screenshotr.py
@@ -52,15 +53,14 @@
 ios_device/servers/os_trace.py
 ios_device/servers/pcapd.py
 ios_device/servers/screenshotr.py
 ios_device/servers/simulate_location.py
 ios_device/servers/spring_board.py
 ios_device/servers/syslog.py
 ios_device/servers/testmanagerd.py
-ios_device/servers/wireless.py
 ios_device/util/__init__.py
 ios_device/util/api_util.py
 ios_device/util/bpylist2.py
 ios_device/util/ca.py
 ios_device/util/constants.py
 ios_device/util/dtx_msg.py
 ios_device/util/exceptions.py
```

### Comparing `py_ios_device-2.3.32/setup.py` & `py_ios_device-2.3.32.1/setup.py`

 * *Files identical despite different names*

