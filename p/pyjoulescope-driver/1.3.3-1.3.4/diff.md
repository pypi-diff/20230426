# Comparing `tmp/pyjoulescope_driver-1.3.3.tar.gz` & `tmp/pyjoulescope_driver-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoulescope_driver-1.3.3.tar", last modified: Wed Apr 19 20:44:27 2023, max compression
+gzip compressed data, was "pyjoulescope_driver-1.3.4.tar", last modified: Wed Apr 26 20:15:17 2023, max compression
```

## Comparing `pyjoulescope_driver-1.3.3.tar` & `pyjoulescope_driver-1.3.4.tar`

### file list

```diff
@@ -1,405 +1,405 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.211270 pyjoulescope_driver-1.3.3/
--rw-rw-rw-   0        0        0     7274 2023-04-19 19:57:15.000000 pyjoulescope_driver-1.3.3/CHANGELOG.md
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjoulescope_driver-1.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      345 2022-11-19 20:38:00.000000 pyjoulescope_driver-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5170 2023-04-19 20:44:27.211270 pyjoulescope_driver-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3360 2023-01-03 21:53:29.000000 pyjoulescope_driver-1.3.3/README.md
--rw-rw-rw-   0        0        0     6268 2022-09-20 19:25:49.000000 pyjoulescope_driver-1.3.3/credits.html
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.056554 pyjoulescope_driver-1.3.3/include/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.060565 pyjoulescope_driver-1.3.3/include/jsdrv/
--rw-rw-rw-   0        0        0     2698 2022-11-08 21:41:45.000000 pyjoulescope_driver-1.3.3/include/jsdrv/cmacro_inc.h
--rw-rw-rw-   0        0        0     8332 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.3/include/jsdrv/cstr.h
--rw-rw-rw-   0        0        0     5878 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.3/include/jsdrv/error_code.h
--rw-rw-rw-   0        0        0     6817 2023-04-14 18:25:40.000000 pyjoulescope_driver-1.3.3/include/jsdrv/log.h
--rw-rw-rw-   0        0        0     2002 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include/jsdrv/meta.h
--rw-rw-rw-   0        0        0    13833 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include/jsdrv/time.h
--rw-rw-rw-   0        0        0     3827 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/include/jsdrv/topic.h
--rw-rw-rw-   0        0        0    12351 2022-08-01 20:41:48.000000 pyjoulescope_driver-1.3.3/include/jsdrv/union.h
--rw-rw-rw-   0        0        0     4042 2023-04-14 11:59:37.000000 pyjoulescope_driver-1.3.3/include/jsdrv/version.h
--rw-rw-rw-   0        0        0    29282 2023-04-14 12:30:28.000000 pyjoulescope_driver-1.3.3/include/jsdrv.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.060565 pyjoulescope_driver-1.3.3/include_private/
--rw-rw-rw-   0        0        0    13394 2022-10-27 14:05:41.000000 pyjoulescope_driver-1.3.3/include_private/js220_api.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.074586 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/
--rw-rw-rw-   0        0        0     1683 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/assert.h
--rw-rw-rw-   0        0        0     2116 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/backend.h
--rw-rw-rw-   0        0        0     2774 2023-04-12 17:01:55.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer.h
--rw-rw-rw-   0        0        0     3935 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer_signal.h
--rw-rw-rw-   0        0        0     7138 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/cdef.h
--rw-rw-rw-   0        0        0     5647 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/dbc.h
--rw-rw-rw-   0        0        0     1385 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/device.h
--rw-rw-rw-   0        0        0     1291 2022-07-28 13:15:21.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/devices.h
--rw-rw-rw-   0        0        0     1633 2022-10-23 16:50:55.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/downsample.h
--rw-rw-rw-   0        0        0     1960 2022-09-19 13:38:02.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/event.h
--rw-rw-rw-   0        0        0     6987 2023-03-19 15:49:32.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/frontend.h
--rw-rw-rw-   0        0        0     1408 2022-08-01 19:59:27.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_cal.h
--rw-rw-rw-   0        0        0     3046 2022-11-01 14:07:32.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_sample_processor.h
--rw-rw-rw-   0        0        0     2858 2022-11-01 15:41:07.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_stats.h
--rw-rw-rw-   0        0        0     1647 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_i128.h
--rw-rw-rw-   0        0        0     1558 2022-10-04 22:55:17.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_stats.h
--rw-rw-rw-   0        0        0     3780 2022-08-01 13:11:32.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/json.h
--rw-rw-rw-   0        0        0    14035 2022-09-18 11:31:10.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/list.h
--rw-rw-rw-   0        0        0     8973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/log.h
--rw-rw-rw-   0        0        0     1650 2022-09-19 12:36:34.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/msg_queue.h
--rw-rw-rw-   0        0        0     2561 2022-07-28 13:01:35.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/mutex.h
--rw-rw-rw-   0        0        0     5093 2023-04-14 19:17:27.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/platform.h
--rw-rw-rw-   0        0        0     4061 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/pubsub.h
--rw-rw-rw-   0        0        0     2799 2022-10-07 12:17:37.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/sample_buffer_f32.h
--rw-rw-rw-   0        0        0     4561 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/statistics.h
--rw-rw-rw-   0        0        0     1939 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/thread.h
--rw-rw-rw-   0        0        0     8210 2022-07-29 18:34:03.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/usb_spec.h
--rw-rw-rw-   0        0        0     1533 2022-10-09 18:53:30.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/windows.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.081605 pyjoulescope_driver-1.3.3/pyjoulescope_driver/
--rw-rw-rw-   0        0        0      964 2023-03-29 21:30:50.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-03-29 21:47:21.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/__main__.py
--rw-rw-rw-   0        0        0  1592888 2023-04-19 20:28:54.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/binding.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.091619 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/
--rw-rw-rw-   0        0        0      987 2023-04-14 12:52:01.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-04-14 19:51:53.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/api_timeout.py
--rw-rw-rw-   0        0        0     1830 2023-01-25 14:57:14.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/gpi.py
--rw-rw-rw-   0        0        0     3702 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/info.py
--rw-rw-rw-   0        0        0     4213 2022-10-30 15:18:19.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/program.py
--rw-rw-rw-   0        0        0     5031 2023-04-13 12:02:12.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/record.py
--rw-rw-rw-   0        0        0      932 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/scan.py
--rw-rw-rw-   0        0        0     2410 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/set_parameter.py
--rw-rw-rw-   0        0        0     2981 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/statistics.py
--rw-rw-rw-   0        0        0     3723 2023-04-14 13:21:57.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/threads.py
--rw-rw-rw-   0        0        0   609280 2023-04-19 20:44:25.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_alpha.img
--rw-rw-rw-   0        0        0   609280 2023-04-19 20:44:25.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_beta.img
--rw-rw-rw-   0        0        0   609280 2023-04-19 20:44:25.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_stable.img
--rw-rw-rw-   0        0        0    10359 2023-04-15 14:37:51.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/program.py
--rw-rw-rw-   0        0        0     8508 2023-04-14 15:05:28.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/record.py
--rw-rw-rw-   0        0        0     8980 2022-11-11 19:24:16.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/release.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.092619 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/
--rw-rw-rw-   0        0        0        0 2022-10-09 12:38:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/__init__.py
--rw-rw-rw-   0        0        0     1901 2022-10-09 17:17:09.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_release.py
--rw-rw-rw-   0        0        0     2304 2023-03-29 16:02:01.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_time64.py
--rw-rw-rw-   0        0        0     4660 2023-03-29 16:00:59.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/time64.py
--rw-rw-rw-   0        0        0     1063 2023-04-14 11:59:37.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/version.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.087612 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/
--rw-rw-rw-   0        0        0     5170 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13694 2023-04-19 20:44:27.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      868 2022-11-30 13:52:01.000000 pyjoulescope_driver-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      117 2023-04-19 20:44:27.216777 pyjoulescope_driver-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0    10610 2023-04-14 19:59:13.000000 pyjoulescope_driver-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.105631 pyjoulescope_driver-1.3.3/src/
--rw-rw-rw-   0        0        0     2655 2023-04-14 19:59:17.000000 pyjoulescope_driver-1.3.3/src/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.108138 pyjoulescope_driver-1.3.3/src/backend/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.109138 pyjoulescope_driver-1.3.3/src/backend/libusb/
--rw-rw-rw-   0        0        0    30330 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/backend/libusb/backend.c
--rw-rw-rw-   0        0        0     4580 2022-09-19 12:40:12.000000 pyjoulescope_driver-1.3.3/src/backend/libusb/msg_queue.c
--rw-rw-rw-   0        0        0     5503 2023-04-14 20:55:21.000000 pyjoulescope_driver-1.3.3/src/backend/posix.c
--rw-rw-rw-   0        0        0     6886 2023-04-14 20:54:20.000000 pyjoulescope_driver-1.3.3/src/backend/windows.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.109138 pyjoulescope_driver-1.3.3/src/backend/winusb/
--rw-rw-rw-   0        0        0    38641 2023-04-04 15:07:16.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/backend.c
--rw-rw-rw-   0        0        0     7713 2022-09-18 12:51:07.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.c
--rw-rw-rw-   0        0        0     2798 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.h
--rw-rw-rw-   0        0        0     4807 2023-03-19 16:29:53.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/msg_queue.c
--rw-rw-rw-   0        0        0    25596 2023-03-15 17:50:15.000000 pyjoulescope_driver-1.3.3/src/buffer.c
--rw-rw-rw-   0        0        0    32515 2023-03-30 18:49:53.000000 pyjoulescope_driver-1.3.3/src/buffer_signal.c
--rw-rw-rw-   0        0        0    11771 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/cstr.c
--rw-rw-rw-   0        0        0     1671 2022-09-19 11:52:36.000000 pyjoulescope_driver-1.3.3/src/devices.c
--rw-rw-rw-   0        0        0     8709 2022-10-24 15:34:41.000000 pyjoulescope_driver-1.3.3/src/downsample.c
--rw-rw-rw-   0        0        0     5925 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.3/src/emu.c
--rw-rw-rw-   0        0        0     4649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/emulated.c
--rw-rw-rw-   0        0        0     4817 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.3/src/error_code.c
--rw-rw-rw-   0        0        0     9335 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/js110_api.h
--rw-rw-rw-   0        0        0     3972 2022-09-18 11:26:57.000000 pyjoulescope_driver-1.3.3/src/js110_cal.c
--rw-rw-rw-   0        0        0     9038 2022-11-01 14:07:47.000000 pyjoulescope_driver-1.3.3/src/js110_sample_processor.c
--rw-rw-rw-   0        0        0     4551 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.3/src/js110_stats.c
--rw-rw-rw-   0        0        0    52566 2023-04-19 20:14:10.000000 pyjoulescope_driver-1.3.3/src/js110_usb.c
--rw-rw-rw-   0        0        0     5162 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/js220_i128.c
--rw-rw-rw-   0        0        0     1188 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/src/js220_params.c
--rw-rw-rw-   0        0        0     2893 2022-10-05 01:35:24.000000 pyjoulescope_driver-1.3.3/src/js220_stats.c
--rw-rw-rw-   0        0        0    62891 2023-04-14 13:07:09.000000 pyjoulescope_driver-1.3.3/src/js220_usb.c
--rw-rw-rw-   0        0        0    37782 2023-04-14 12:55:05.000000 pyjoulescope_driver-1.3.3/src/jsdrv.c
--rw-rw-rw-   0        0        0    10974 2022-08-01 18:37:59.000000 pyjoulescope_driver-1.3.3/src/json.c
--rw-rw-rw-   0        0        0    16499 2023-04-14 20:57:15.000000 pyjoulescope_driver-1.3.3/src/log.c
--rw-rw-rw-   0        0        0    10627 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/meta.c
--rw-rw-rw-   0        0        0    24211 2023-03-19 15:32:24.000000 pyjoulescope_driver-1.3.3/src/pubsub.c
--rw-rw-rw-   0        0        0     4944 2022-10-07 12:24:15.000000 pyjoulescope_driver-1.3.3/src/sample_buffer_f32.c
--rw-rw-rw-   0        0        0     5262 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/statistics.c
--rw-rw-rw-   0        0        0     2814 2023-03-09 19:53:59.000000 pyjoulescope_driver-1.3.3/src/time.c
--rw-rw-rw-   0        0        0     3763 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/src/topic.c
--rw-rw-rw-   0        0        0    12780 2022-09-18 11:32:07.000000 pyjoulescope_driver-1.3.3/src/union.c
--rw-rw-rw-   0        0        0     1001 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/version.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.110646 pyjoulescope_driver-1.3.3/third-party/
--rw-rw-rw-   0        0        0      810 2022-09-20 18:21:09.000000 pyjoulescope_driver-1.3.3/third-party/CMakeLists.txt
--rw-rw-rw-   0        0        0      364 2022-08-01 20:40:07.000000 pyjoulescope_driver-1.3.3/third-party/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.117149 pyjoulescope_driver-1.3.3/third-party/cmocka/
--rw-rw-rw-   0        0        0       18 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/.clang_complete
--rw-rw-rw-   0        0        0     9611 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     3508 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/.ycm_extra_conf.py
--rw-rw-rw-   0        0        0     1209 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/5.patch
--rw-rw-rw-   0        0        0     3601 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CMakeLists.txt
--rw-rw-rw-   0        0        0     1845 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CPackConfig.cmake
--rw-rw-rw-   0        0        0      284 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CTestConfig.cmake
--rw-rw-rw-   0        0        0     5331 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CompilerChecks.cmake
--rw-rw-rw-   0        0        0     4648 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/ConfigureChecks.cmake
--rw-rw-rw-   0        0        0      431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/DefineOptions.cmake
--rw-rw-rw-   0        0        0     3217 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/INSTALL.md
--rw-rw-rw-   0        0        0      658 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.118151 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.121677 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/
--rw-rw-rw-   0        0        0      866 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
--rw-rw-rw-   0        0        0     3360 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
--rw-rw-rw-   0        0        0     1952 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
--rw-rw-rw-   0        0        0      811 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
--rw-rw-rw-   0        0        0     3973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
--rw-rw-rw-   0        0        0      585 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
--rw-rw-rw-   0        0        0     1480 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/FindNSIS.cmake
--rw-rw-rw-   0        0        0      680 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
--rw-rw-rw-   0        0        0      656 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
--rw-rw-rw-   0        0        0     1145 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
--rw-rw-rw-   0        0        0       53 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmocka-build-tree-settings.cmake.in
--rw-rw-rw-   0        0        0      507 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmocka-config.cmake.in
--rw-rw-rw-   0        0        0      189 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmocka.pc.cmake
--rw-rw-rw-   0        0        0     5161 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/config.h.cmake
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.122677 pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/
--rw-rw-rw-   0        0        0     3918 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/coverity_assert_model.c
--rw-rw-rw-   0        0        0      142 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/coverity_internal_model.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.123677 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/
--rw-rw-rw-   0        0        0     2206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/CMakeLists.txt
--rw-rw-rw-   0        0        0    26974 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/index.html
--rw-rw-rw-   0        0        0     5291 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/mainpage.dox
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.125177 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/
--rw-rw-rw-   0        0        0     1301 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/README.md
--rw-rw-rw-   0        0        0     2121 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/header.html
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.129185 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/
--rw-rw-rw-   0        0        0     6714 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/doc.svg
--rw-rw-rw-   0        0        0     3604 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderclosed.svg
--rw-rw-rw-   0        0        0     4299 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderopen.svg
--rw-rw-rw-   0        0        0     3955 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/mag_glass.svg
--rw-rw-rw-   0        0        0     3988 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
--rw-rw-rw-   0        0        0     3249 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
--rw-rw-rw-   0        0        0     3262 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
--rw-rw-rw-   0        0        0     7409 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
--rw-rw-rw-   0        0        0      483 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/sync_off.png
--rw-rw-rw-   0        0        0      488 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/sync_on.png
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.129685 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/js/
--rw-rw-rw-   0        0        0      977 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/js/striped_bg.js
--rw-rw-rw-   0        0        0    32455 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/that_style.css
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.135692 pyjoulescope_driver-1.3.3/third-party/cmocka/example/
--rw-rw-rw-   0        0        0     2562 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/CMakeLists.txt
--rw-rw-rw-   0        0        0     1755 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module.c
--rw-rw-rw-   0        0        0     1640 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module_test.c
--rw-rw-rw-   0        0        0     1254 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro.c
--rw-rw-rw-   0        0        0      144 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro.h
--rw-rw-rw-   0        0        0     1649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro_test.c
--rw-rw-rw-   0        0        0     1216 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.c
--rw-rw-rw-   0        0        0      692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.h
--rw-rw-rw-   0        0        0     1692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module_test.c
--rw-rw-rw-   0        0        0     9746 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator.c
--rw-rw-rw-   0        0        0    16244 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator_test.c
--rw-rw-rw-   0        0        0     1439 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/database.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.136192 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/
--rw-rw-rw-   0        0        0      197 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.137691 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/
--rw-rw-rw-   0        0        0      620 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
--rw-rw-rw-   0        0        0     1431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.c
--rw-rw-rw-   0        0        0      789 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.h
--rw-rw-rw-   0        0        0     5222 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
--rw-rw-rw-   0        0        0       61 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.140197 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/
--rw-rw-rw-   0        0        0      685 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/CMakeLists.txt
--rw-rw-rw-   0        0        0     2033 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/README.md
--rw-rw-rw-   0        0        0     1882 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.c
--rw-rw-rw-   0        0        0      793 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.h
--rw-rw-rw-   0        0        0     5237 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/test_uptime.c
--rw-rw-rw-   0        0        0     3305 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/uptime.c
--rw-rw-rw-   0        0        0      415 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/simple_test.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.142206 pyjoulescope_driver-1.3.3/third-party/cmocka/include/
--rw-rw-rw-   0        0        0      465 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/CMakeLists.txt
--rw-rw-rw-   0        0        0    77952 2022-08-01 20:01:08.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka.h
--rw-rw-rw-   0        0        0     1893 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_pbc.h
--rw-rw-rw-   0        0        0     4137 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_private.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.142705 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmockery/
--rw-rw-rw-   0        0        0       21 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmockery/cmockery.h
--rw-rw-rw-   0        0        0       25 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmockery/pbc.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.144204 pyjoulescope_driver-1.3.3/third-party/cmocka/src/
--rw-rw-rw-   0        0        0     3668 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/src/CMakeLists.txt
--rw-rw-rw-   0        0        0   119941 2022-09-18 17:05:56.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.c
--rw-rw-rw-   0        0        0     1174 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.def
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.154711 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/
--rw-rw-rw-   0        0        0     7657 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0     6215 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/cmocka_test.cmake
--rw-rw-rw-   0        0        0     2758 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/ctest-default.cmake
--rw-rw-rw-   0        0        0     1922 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_alloc.c
--rw-rw-rw-   0        0        0      818 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros.c
--rw-rw-rw-   0        0        0      862 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros_fail.c
--rw-rw-rw-   0        0        0     1550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_basics.c
--rw-rw-rw-   0        0        0      970 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_cmockery.c
--rw-rw-rw-   0        0        0      869 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_exception_handler.c
--rw-rw-rw-   0        0        0     1774 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_fixtures.c
--rw-rw-rw-   0        0        0     1206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_float_macros.c
--rw-rw-rw-   0        0        0      992 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_fixtures.c
--rw-rw-rw-   0        0        0      699 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_assert.c
--rw-rw-rw-   0        0        0      696 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_fail.c
--rw-rw-rw-   0        0        0     1757 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_groups.c
--rw-rw-rw-   0        0        0     2767 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering.c
--rw-rw-rw-   0        0        0     2420 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering_fail.c
--rw-rw-rw-   0        0        0     1577 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns.c
--rw-rw-rw-   0        0        0     1704 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns_fail.c
--rw-rw-rw-   0        0        0     1092 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_setup_fail.c
--rw-rw-rw-   0        0        0     1043 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip.c
--rw-rw-rw-   0        0        0     1362 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip_filter.c
--rw-rw-rw-   0        0        0     2280 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_strmatch.c
--rw-rw-rw-   0        0        0     1260 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_wildcard.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.158712 pyjoulescope_driver-1.3.3/third-party/libusb/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.159716 pyjoulescope_driver-1.3.3/third-party/libusb/.github/
--rw-rw-rw-   0        0        0      719 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/cifuzz.yml
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.161220 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/
--rw-rw-rw-   0        0        0     1188 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/linux.yml
--rw-rw-rw-   0        0        0     1023 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0      527 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/msys2.yml
--rw-rw-rw-   0        0        0      827 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.164719 pyjoulescope_driver-1.3.3/third-party/libusb/.private/
--rw-rw-rw-   0        0        0      202 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/README.txt
--rw-rw-rw-   0        0        0      548 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/appveyor_build.sh
--rw-rw-rw-   0        0        0     1424 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/bm.sh
--rw-rw-rw-   0        0        0     1109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-build.sh
--rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-container-build.sh
--rw-rw-rw-   0        0        0      959 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/post-rewrite.sh
--rw-rw-rw-   0        0        0     1995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/pre-commit.sh
--rw-rw-rw-   0        0        0     2545 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/wbs.txt
--rw-rw-rw-   0        0        0     1465 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.travis.yml
--rw-rw-rw-   0        0        0     2523 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.3/third-party/libusb/CMakeLists.txt
--rw-rw-rw-   0        0        0     1972 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/INSTALL_WIN.txt
--rw-rw-rw-   0        0        0     1495 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Makefile.am
--rw-rw-rw-   0        0        0     1395 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/README-FORK.md
--rw-rw-rw-   0        0        0     1894 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/README.git
--rw-rw-rw-   0        0        0        6 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.167719 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/
--rw-rw-rw-   0        0        0     2409 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/common.xcconfig
--rw-rw-rw-   0        0        0      995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/config.h
--rw-rw-rw-   0        0        0     1135 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/debug.xcconfig
--rw-rw-rw-   0        0        0      988 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcconfig
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.168219 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcodeproj/
--rw-rw-rw-   0        0        0    62286 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
--rw-rw-rw-   0        0        0      963 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_debug.xcconfig
--rw-rw-rw-   0        0        0      965 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_release.xcconfig
--rw-rw-rw-   0        0        0     1208 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/release.xcconfig
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.168219 pyjoulescope_driver-1.3.3/third-party/libusb/android/
--rw-rw-rw-   0        0        0     2016 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/config.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.169219 pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/
--rw-rw-rw-   0        0        0    11355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.c
--rw-rw-rw-   0        0        0     1156 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.171225 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/
--rw-rw-rw-   0        0        0      997 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Android.mk
--rw-rw-rw-   0        0        0     1370 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Application.mk
--rw-rw-rw-   0        0        0     3425 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/examples.mk
--rw-rw-rw-   0        0        0     2056 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/libusb.mk
--rw-rw-rw-   0        0        0     1355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/tests.mk
--rw-rw-rw-   0        0        0     3820 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/appveyor.yml
--rw-rw-rw-   0        0        0      191 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/autogen.sh
--rw-rw-rw-   0        0        0      109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/bootstrap.sh
--rw-rw-rw-   0        0        0    16514 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/configure.ac
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.172225 pyjoulescope_driver-1.3.3/third-party/libusb/doc/
--rw-rw-rw-   0        0        0      685 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/doc/Makefile.in
--rw-rw-rw-   0        0        0   115647 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/doc/doxygen.cfg.in
--rw-rw-rw-   0        0        0     2923 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/doc/libusb.png
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.176726 pyjoulescope_driver-1.3.3/third-party/libusb/examples/
--rw-rw-rw-   0        0        0      416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/Makefile.am
--rw-rw-rw-   0        0        0    15812 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/dpfp.c
--rw-rw-rw-   0        0        0    24573 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.c
--rw-rw-rw-   0        0        0     4247 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.h
--rw-rw-rw-   0        0        0     9593 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/fxload.c
--rw-rw-rw-   0        0        0     3580 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/hotplugtest.c
--rw-rw-rw-   0        0        0     2081 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/listdevs.c
--rw-rw-rw-   0        0        0     6149 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/sam3u_benchmark.c
--rw-rw-rw-   0        0        0     9765 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/testlibusb.c
--rw-rw-rw-   0        0        0    40008 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/xusb.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.052046 pyjoulescope_driver-1.3.3/third-party/libusb/include/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.176726 pyjoulescope_driver-1.3.3/third-party/libusb/include/linux/
--rw-rw-rw-   0        0        0     5104 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.3/third-party/libusb/include/linux/config.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.177226 pyjoulescope_driver-1.3.3/third-party/libusb/include/macos/
--rw-rw-rw-   0        0        0     5130 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/include/macos/config.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.183734 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/
--rw-rw-rw-   0        0        0     2539 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am
--rw-rw-rw-   0        0        0      780 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am.extra
--rw-rw-rw-   0        0        0    99186 2022-09-20 23:33:57.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/core.c
--rw-rw-rw-   0        0        0    37583 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/descriptor.c
--rw-rw-rw-   0        0        0    15552 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/hotplug.c
--rw-rw-rw-   0        0        0   113897 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/io.c
--rw-rw-rw-   0        0        0     8221 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.def
--rw-rw-rw-   0        0        0     1642 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.rc
--rw-rw-rw-   0        0        0    78746 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb.h
--rw-rw-rw-   0        0        0    53532 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusbi.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.197249 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/
--rw-rw-rw-   0        0        0   103226 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.c
--rw-rw-rw-   0        0        0     7071 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.h
--rw-rw-rw-   0        0        0    24325 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/emscripten_webusb.cpp
--rw-rw-rw-   0        0        0     9581 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.c
--rw-rw-rw-   0        0        0     1776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.h
--rw-rw-rw-   0        0        0     6948 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.c
--rw-rw-rw-   0        0        0     1520 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.h
--rw-rw-rw-   0        0        0     7884 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_pollfs.cpp
--rw-rw-rw-   0        0        0     3386 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb.h
--rw-rw-rw-   0        0        0    16687 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_backend.cpp
--rw-rw-rw-   0        0        0     7477 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.cpp
--rw-rw-rw-   0        0        0     4080 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.h
--rw-rw-rw-   0        0        0    10778 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_netlink.c
--rw-rw-rw-   0        0        0     8864 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_udev.c
--rw-rw-rw-   0        0        0    83335 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.c
--rw-rw-rw-   0        0        0     6551 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.h
--rw-rw-rw-   0        0        0    16279 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/netbsd_usb.c
--rw-rw-rw-   0        0        0     2996 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/null_usb.c
--rw-rw-rw-   0        0        0    18179 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/openbsd_usb.c
--rw-rw-rw-   0        0        0    45204 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.c
--rw-rw-rw-   0        0        0     2254 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.h
--rw-rw-rw-   0        0        0     3488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.c
--rw-rw-rw-   0        0        0     3052 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.h
--rw-rw-rw-   0        0        0     1416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.c
--rw-rw-rw-   0        0        0     3280 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.h
--rw-rw-rw-   0        0        0    30524 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.c
--rw-rw-rw-   0        0        0    14347 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.h
--rw-rw-rw-   0        0        0    24491 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.c
--rw-rw-rw-   0        0        0     2926 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.h
--rw-rw-rw-   0        0        0   171316 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.c
--rw-rw-rw-   0        0        0    24670 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.h
--rw-rw-rw-   0        0        0     8776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/strerror.c
--rw-rw-rw-   0        0        0    13160 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/sync.c
--rw-rw-rw-   0        0        0      449 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/version.h
--rw-rw-rw-   0        0        0       27 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/version_nano.h
--rw-rw-rw-   0        0        0      323 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb-1.0.pc.in
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.206762 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/
--rw-rw-rw-   0        0        0      136 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/.gitattributes
--rw-rw-rw-   0        0        0     2982 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Base.props
--rw-rw-rw-   0        0        0      287 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.Application.props
--rw-rw-rw-   0        0        0     2817 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.Base.props
--rw-rw-rw-   0        0        0      612 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.DynamicLibrary.props
--rw-rw-rw-   0        0        0      289 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.StaticLibrary.props
--rw-rw-rw-   0        0        0     1438 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/ProjectConfigurations.Base.props
--rw-rw-rw-   0        0        0      713 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/build_all.ps1
--rw-rw-rw-   0        0        0     2007 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/config.h
--rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp.vcxproj
--rw-rw-rw-   0        0        0     1659 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp_threaded.vcxproj
--rw-rw-rw-   0        0        0     2125 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/fxload.vcxproj
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.207762 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/
--rw-rw-rw-   0        0        0    31341 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.c
--rw-rw-rw-   0        0        0     6627 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.h
--rw-rw-rw-   0        0        0     4708 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt1.c
--rw-rw-rw-   0        0        0     1522 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt.vcxproj
--rw-rw-rw-   0        0        0     1444 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/hotplugtest.vcxproj
--rw-rw-rw-   0        0        0    17271 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb.sln
--rw-rw-rw-   0        0        0     2762 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_dll.vcxproj
--rw-rw-rw-   0        0        0     2336 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_static.vcxproj
--rw-rw-rw-   0        0        0     1441 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/listdevs.vcxproj
--rw-rw-rw-   0        0        0     1488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/sam3u_benchmark.vcxproj
--rw-rw-rw-   0        0        0     1579 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/stress.vcxproj
--rw-rw-rw-   0        0        0     1443 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/testlibusb.vcxproj
--rw-rw-rw-   0        0        0     1709 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/xusb.vcxproj
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.209263 pyjoulescope_driver-1.3.3/third-party/libusb/tests/
--rw-rw-rw-   0        0        0      623 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/Makefile.am
--rw-rw-rw-   0        0        0     2490 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/libusb_testlib.h
--rw-rw-rw-   0        0        0     4935 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/stress.c
--rw-rw-rw-   0        0        0     4919 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/testlib.c
--rw-rw-rw-   0        0        0    37223 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/umockdev.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.211270 pyjoulescope_driver-1.3.3/third-party/tinyprintf/
--rw-rw-rw-   0        0        0      122 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/CMakeLists.txt
--rw-rw-rw-   0        0        0    13188 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.c
--rw-rw-rw-   0        0        0     6550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.h
--rw-rw-rw-   0        0        0     1554 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.965904 pyjoulescope_driver-1.3.4/
+-rw-rw-rw-   0        0        0     7476 2023-04-26 19:47:58.000000 pyjoulescope_driver-1.3.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjoulescope_driver-1.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      345 2022-11-19 20:38:00.000000 pyjoulescope_driver-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5170 2023-04-26 20:15:17.965904 pyjoulescope_driver-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3360 2023-01-03 21:53:29.000000 pyjoulescope_driver-1.3.4/README.md
+-rw-rw-rw-   0        0        0     6268 2022-09-20 19:25:49.000000 pyjoulescope_driver-1.3.4/credits.html
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.807086 pyjoulescope_driver-1.3.4/include/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.811093 pyjoulescope_driver-1.3.4/include/jsdrv/
+-rw-rw-rw-   0        0        0     2698 2022-11-08 21:41:45.000000 pyjoulescope_driver-1.3.4/include/jsdrv/cmacro_inc.h
+-rw-rw-rw-   0        0        0     8332 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.4/include/jsdrv/cstr.h
+-rw-rw-rw-   0        0        0     5878 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.4/include/jsdrv/error_code.h
+-rw-rw-rw-   0        0        0     6817 2023-04-14 18:25:40.000000 pyjoulescope_driver-1.3.4/include/jsdrv/log.h
+-rw-rw-rw-   0        0        0     2002 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include/jsdrv/meta.h
+-rw-rw-rw-   0        0        0    13833 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/include/jsdrv/time.h
+-rw-rw-rw-   0        0        0     3827 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.4/include/jsdrv/topic.h
+-rw-rw-rw-   0        0        0    12351 2022-08-01 20:41:48.000000 pyjoulescope_driver-1.3.4/include/jsdrv/union.h
+-rw-rw-rw-   0        0        0     4042 2023-04-26 19:51:47.000000 pyjoulescope_driver-1.3.4/include/jsdrv/version.h
+-rw-rw-rw-   0        0        0    29282 2023-04-14 12:30:28.000000 pyjoulescope_driver-1.3.4/include/jsdrv.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.811093 pyjoulescope_driver-1.3.4/include_private/
+-rw-rw-rw-   0        0        0    13394 2022-10-27 14:05:41.000000 pyjoulescope_driver-1.3.4/include_private/js220_api.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.823633 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/
+-rw-rw-rw-   0        0        0     1683 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/assert.h
+-rw-rw-rw-   0        0        0     2116 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/backend.h
+-rw-rw-rw-   0        0        0     2774 2023-04-12 17:01:55.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/buffer.h
+-rw-rw-rw-   0        0        0     3987 2023-04-21 20:34:04.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/buffer_signal.h
+-rw-rw-rw-   0        0        0     7138 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/cdef.h
+-rw-rw-rw-   0        0        0     5647 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/dbc.h
+-rw-rw-rw-   0        0        0     1385 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/device.h
+-rw-rw-rw-   0        0        0     1291 2022-07-28 13:15:21.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/devices.h
+-rw-rw-rw-   0        0        0     1633 2022-10-23 16:50:55.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/downsample.h
+-rw-rw-rw-   0        0        0     1960 2022-09-19 13:38:02.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/event.h
+-rw-rw-rw-   0        0        0     6987 2023-03-19 15:49:32.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/frontend.h
+-rw-rw-rw-   0        0        0     1408 2022-08-01 19:59:27.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js110_cal.h
+-rw-rw-rw-   0        0        0     3046 2022-11-01 14:07:32.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js110_sample_processor.h
+-rw-rw-rw-   0        0        0     2858 2022-11-01 15:41:07.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js110_stats.h
+-rw-rw-rw-   0        0        0     1647 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js220_i128.h
+-rw-rw-rw-   0        0        0     1558 2022-10-04 22:55:17.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js220_stats.h
+-rw-rw-rw-   0        0        0     3780 2022-08-01 13:11:32.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/json.h
+-rw-rw-rw-   0        0        0    14035 2022-09-18 11:31:10.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/list.h
+-rw-rw-rw-   0        0        0     8973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/log.h
+-rw-rw-rw-   0        0        0     1650 2022-09-19 12:36:34.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/msg_queue.h
+-rw-rw-rw-   0        0        0     2561 2022-07-28 13:01:35.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/mutex.h
+-rw-rw-rw-   0        0        0     5093 2023-04-14 19:17:27.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/platform.h
+-rw-rw-rw-   0        0        0     4061 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/pubsub.h
+-rw-rw-rw-   0        0        0     2799 2022-10-07 12:17:37.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/sample_buffer_f32.h
+-rw-rw-rw-   0        0        0     4561 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/statistics.h
+-rw-rw-rw-   0        0        0     1939 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/thread.h
+-rw-rw-rw-   0        0        0     8210 2022-07-29 18:34:03.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/usb_spec.h
+-rw-rw-rw-   0        0        0     1533 2022-10-09 18:53:30.000000 pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/windows.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.830145 pyjoulescope_driver-1.3.4/pyjoulescope_driver/
+-rw-rw-rw-   0        0        0      964 2023-03-29 21:30:50.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-03-29 21:47:21.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/__main__.py
+-rw-rw-rw-   0        0        0  1592784 2023-04-26 20:00:21.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/binding.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.842686 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/
+-rw-rw-rw-   0        0        0      987 2023-04-14 12:52:01.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-04-14 19:51:53.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/api_timeout.py
+-rw-rw-rw-   0        0        0     1830 2023-01-25 14:57:14.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/gpi.py
+-rw-rw-rw-   0        0        0     3702 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/info.py
+-rw-rw-rw-   0        0        0     4213 2022-10-30 15:18:19.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/program.py
+-rw-rw-rw-   0        0        0     5031 2023-04-13 12:02:12.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/record.py
+-rw-rw-rw-   0        0        0      932 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/scan.py
+-rw-rw-rw-   0        0        0     2410 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/set_parameter.py
+-rw-rw-rw-   0        0        0     2981 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/statistics.py
+-rw-rw-rw-   0        0        0     3723 2023-04-14 13:21:57.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/threads.py
+-rw-rw-rw-   0        0        0   609280 2023-04-26 20:15:16.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/img_alpha.img
+-rw-rw-rw-   0        0        0   609280 2023-04-26 20:15:16.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/img_beta.img
+-rw-rw-rw-   0        0        0   609280 2023-04-26 20:15:16.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/img_stable.img
+-rw-rw-rw-   0        0        0    10359 2023-04-15 14:37:51.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/program.py
+-rw-rw-rw-   0        0        0     8432 2023-04-26 14:37:52.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/record.py
+-rw-rw-rw-   0        0        0     8980 2022-11-11 19:24:16.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/release.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.843689 pyjoulescope_driver-1.3.4/pyjoulescope_driver/test/
+-rw-rw-rw-   0        0        0        0 2022-10-09 12:38:26.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/test/__init__.py
+-rw-rw-rw-   0        0        0     1901 2022-10-09 17:17:09.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/test/test_release.py
+-rw-rw-rw-   0        0        0     2304 2023-03-29 16:02:01.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/test/test_time64.py
+-rw-rw-rw-   0        0        0     4660 2023-03-29 16:00:59.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/time64.py
+-rw-rw-rw-   0        0        0     1063 2023-04-26 19:51:47.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver/version.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.838174 pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/
+-rw-rw-rw-   0        0        0     5170 2023-04-26 20:15:17.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13694 2023-04-26 20:15:17.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 20:15:17.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-26 20:15:17.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-04-26 20:15:17.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-26 20:15:17.000000 pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      868 2022-11-30 13:52:01.000000 pyjoulescope_driver-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0      117 2023-04-26 20:15:17.969909 pyjoulescope_driver-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0    10610 2023-04-14 19:59:13.000000 pyjoulescope_driver-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.857205 pyjoulescope_driver-1.3.4/src/
+-rw-rw-rw-   0        0        0     2655 2023-04-14 19:59:17.000000 pyjoulescope_driver-1.3.4/src/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.859208 pyjoulescope_driver-1.3.4/src/backend/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.859711 pyjoulescope_driver-1.3.4/src/backend/libusb/
+-rw-rw-rw-   0        0        0    30330 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/src/backend/libusb/backend.c
+-rw-rw-rw-   0        0        0     4580 2022-09-19 12:40:12.000000 pyjoulescope_driver-1.3.4/src/backend/libusb/msg_queue.c
+-rw-rw-rw-   0        0        0     5503 2023-04-14 20:55:21.000000 pyjoulescope_driver-1.3.4/src/backend/posix.c
+-rw-rw-rw-   0        0        0     6886 2023-04-14 20:54:20.000000 pyjoulescope_driver-1.3.4/src/backend/windows.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.860713 pyjoulescope_driver-1.3.4/src/backend/winusb/
+-rw-rw-rw-   0        0        0    38641 2023-04-04 15:07:16.000000 pyjoulescope_driver-1.3.4/src/backend/winusb/backend.c
+-rw-rw-rw-   0        0        0     7713 2022-09-18 12:51:07.000000 pyjoulescope_driver-1.3.4/src/backend/winusb/device_change_notifier.c
+-rw-rw-rw-   0        0        0     2798 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/src/backend/winusb/device_change_notifier.h
+-rw-rw-rw-   0        0        0     4807 2023-03-19 16:29:53.000000 pyjoulescope_driver-1.3.4/src/backend/winusb/msg_queue.c
+-rw-rw-rw-   0        0        0    25694 2023-04-21 20:34:16.000000 pyjoulescope_driver-1.3.4/src/buffer.c
+-rw-rw-rw-   0        0        0    32685 2023-04-21 20:33:57.000000 pyjoulescope_driver-1.3.4/src/buffer_signal.c
+-rw-rw-rw-   0        0        0    11771 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/src/cstr.c
+-rw-rw-rw-   0        0        0     1671 2022-09-19 11:52:36.000000 pyjoulescope_driver-1.3.4/src/devices.c
+-rw-rw-rw-   0        0        0     8709 2022-10-24 15:34:41.000000 pyjoulescope_driver-1.3.4/src/downsample.c
+-rw-rw-rw-   0        0        0     5925 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.4/src/emu.c
+-rw-rw-rw-   0        0        0     4649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/src/emulated.c
+-rw-rw-rw-   0        0        0     4817 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.4/src/error_code.c
+-rw-rw-rw-   0        0        0     9335 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/src/js110_api.h
+-rw-rw-rw-   0        0        0     3972 2022-09-18 11:26:57.000000 pyjoulescope_driver-1.3.4/src/js110_cal.c
+-rw-rw-rw-   0        0        0     9038 2022-11-01 14:07:47.000000 pyjoulescope_driver-1.3.4/src/js110_sample_processor.c
+-rw-rw-rw-   0        0        0     4551 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.4/src/js110_stats.c
+-rw-rw-rw-   0        0        0    52566 2023-04-19 20:14:10.000000 pyjoulescope_driver-1.3.4/src/js110_usb.c
+-rw-rw-rw-   0        0        0     5162 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/src/js220_i128.c
+-rw-rw-rw-   0        0        0     1188 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.4/src/js220_params.c
+-rw-rw-rw-   0        0        0     2893 2022-10-05 01:35:24.000000 pyjoulescope_driver-1.3.4/src/js220_stats.c
+-rw-rw-rw-   0        0        0    62976 2023-04-20 12:52:32.000000 pyjoulescope_driver-1.3.4/src/js220_usb.c
+-rw-rw-rw-   0        0        0    37782 2023-04-14 12:55:05.000000 pyjoulescope_driver-1.3.4/src/jsdrv.c
+-rw-rw-rw-   0        0        0    10974 2022-08-01 18:37:59.000000 pyjoulescope_driver-1.3.4/src/json.c
+-rw-rw-rw-   0        0        0    16499 2023-04-14 20:57:15.000000 pyjoulescope_driver-1.3.4/src/log.c
+-rw-rw-rw-   0        0        0    10627 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/src/meta.c
+-rw-rw-rw-   0        0        0    24211 2023-03-19 15:32:24.000000 pyjoulescope_driver-1.3.4/src/pubsub.c
+-rw-rw-rw-   0        0        0     4944 2022-10-07 12:24:15.000000 pyjoulescope_driver-1.3.4/src/sample_buffer_f32.c
+-rw-rw-rw-   0        0        0     5262 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.4/src/statistics.c
+-rw-rw-rw-   0        0        0     2814 2023-03-09 19:53:59.000000 pyjoulescope_driver-1.3.4/src/time.c
+-rw-rw-rw-   0        0        0     3763 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.4/src/topic.c
+-rw-rw-rw-   0        0        0    12780 2022-09-18 11:32:07.000000 pyjoulescope_driver-1.3.4/src/union.c
+-rw-rw-rw-   0        0        0     1001 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/src/version.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.861716 pyjoulescope_driver-1.3.4/third-party/
+-rw-rw-rw-   0        0        0      810 2022-09-20 18:21:09.000000 pyjoulescope_driver-1.3.4/third-party/CMakeLists.txt
+-rw-rw-rw-   0        0        0      364 2022-08-01 20:40:07.000000 pyjoulescope_driver-1.3.4/third-party/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.868721 pyjoulescope_driver-1.3.4/third-party/cmocka/
+-rw-rw-rw-   0        0        0       18 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/.clang_complete
+-rw-rw-rw-   0        0        0     9611 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     3508 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/.ycm_extra_conf.py
+-rw-rw-rw-   0        0        0     1209 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/5.patch
+-rw-rw-rw-   0        0        0     3601 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1845 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/CPackConfig.cmake
+-rw-rw-rw-   0        0        0      284 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/CTestConfig.cmake
+-rw-rw-rw-   0        0        0     5331 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/CompilerChecks.cmake
+-rw-rw-rw-   0        0        0     4648 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/ConfigureChecks.cmake
+-rw-rw-rw-   0        0        0      431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/DefineOptions.cmake
+-rw-rw-rw-   0        0        0     3217 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/INSTALL.md
+-rw-rw-rw-   0        0        0      658 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.869723 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.872736 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/
+-rw-rw-rw-   0        0        0      866 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
+-rw-rw-rw-   0        0        0     3360 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
+-rw-rw-rw-   0        0        0     1952 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
+-rw-rw-rw-   0        0        0      811 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
+-rw-rw-rw-   0        0        0     3973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
+-rw-rw-rw-   0        0        0      585 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
+-rw-rw-rw-   0        0        0     1480 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/FindNSIS.cmake
+-rw-rw-rw-   0        0        0      680 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
+-rw-rw-rw-   0        0        0      656 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
+-rw-rw-rw-   0        0        0     1145 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
+-rw-rw-rw-   0        0        0       53 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmocka-build-tree-settings.cmake.in
+-rw-rw-rw-   0        0        0      507 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmocka-config.cmake.in
+-rw-rw-rw-   0        0        0      189 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/cmocka.pc.cmake
+-rw-rw-rw-   0        0        0     5161 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/config.h.cmake
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.874240 pyjoulescope_driver-1.3.4/third-party/cmocka/coverity/
+-rw-rw-rw-   0        0        0     3918 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/coverity/coverity_assert_model.c
+-rw-rw-rw-   0        0        0      142 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/coverity/coverity_internal_model.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.875240 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/
+-rw-rw-rw-   0        0        0     2206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/CMakeLists.txt
+-rw-rw-rw-   0        0        0    26974 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/index.html
+-rw-rw-rw-   0        0        0     5291 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/mainpage.dox
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.876741 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/
+-rw-rw-rw-   0        0        0     1301 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/README.md
+-rw-rw-rw-   0        0        0     2121 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/header.html
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.880746 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/
+-rw-rw-rw-   0        0        0     6714 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/doc.svg
+-rw-rw-rw-   0        0        0     3604 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/folderclosed.svg
+-rw-rw-rw-   0        0        0     4299 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/folderopen.svg
+-rw-rw-rw-   0        0        0     3955 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/mag_glass.svg
+-rw-rw-rw-   0        0        0     3988 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
+-rw-rw-rw-   0        0        0     3249 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
+-rw-rw-rw-   0        0        0     3262 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
+-rw-rw-rw-   0        0        0     7409 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
+-rw-rw-rw-   0        0        0      483 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/sync_off.png
+-rw-rw-rw-   0        0        0      488 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/sync_on.png
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.881260 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/js/
+-rw-rw-rw-   0        0        0      977 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/js/striped_bg.js
+-rw-rw-rw-   0        0        0    32455 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/that_style.css
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.887269 pyjoulescope_driver-1.3.4/third-party/cmocka/example/
+-rw-rw-rw-   0        0        0     2562 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1755 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/allocate_module.c
+-rw-rw-rw-   0        0        0     1640 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/allocate_module_test.c
+-rw-rw-rw-   0        0        0     1254 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_macro.c
+-rw-rw-rw-   0        0        0      144 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_macro.h
+-rw-rw-rw-   0        0        0     1649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_macro_test.c
+-rw-rw-rw-   0        0        0     1216 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_module.c
+-rw-rw-rw-   0        0        0      692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_module.h
+-rw-rw-rw-   0        0        0     1692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_module_test.c
+-rw-rw-rw-   0        0        0     9746 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/calculator.c
+-rw-rw-rw-   0        0        0    16244 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/calculator_test.c
+-rw-rw-rw-   0        0        0     1439 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/database.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.887269 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/
+-rw-rw-rw-   0        0        0      197 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.889769 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/
+-rw-rw-rw-   0        0        0      620 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/chef.c
+-rw-rw-rw-   0        0        0      789 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/chef.h
+-rw-rw-rw-   0        0        0     5222 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
+-rw-rw-rw-   0        0        0       61 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.892790 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/
+-rw-rw-rw-   0        0        0      685 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/CMakeLists.txt
+-rw-rw-rw-   0        0        0     2033 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/README.md
+-rw-rw-rw-   0        0        0     1882 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/proc_uptime.c
+-rw-rw-rw-   0        0        0      793 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/proc_uptime.h
+-rw-rw-rw-   0        0        0     5237 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/test_uptime.c
+-rw-rw-rw-   0        0        0     3305 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/uptime.c
+-rw-rw-rw-   0        0        0      415 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/example/simple_test.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.894295 pyjoulescope_driver-1.3.4/third-party/cmocka/include/
+-rw-rw-rw-   0        0        0      465 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/include/CMakeLists.txt
+-rw-rw-rw-   0        0        0    77952 2022-08-01 20:01:08.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmocka.h
+-rw-rw-rw-   0        0        0     1893 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmocka_pbc.h
+-rw-rw-rw-   0        0        0     4137 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmocka_private.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.895295 pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmockery/
+-rw-rw-rw-   0        0        0       21 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmockery/cmockery.h
+-rw-rw-rw-   0        0        0       25 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmockery/pbc.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.896294 pyjoulescope_driver-1.3.4/third-party/cmocka/src/
+-rw-rw-rw-   0        0        0     3668 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/src/CMakeLists.txt
+-rw-rw-rw-   0        0        0   119941 2022-09-18 17:05:56.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/src/cmocka.c
+-rw-rw-rw-   0        0        0     1174 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/src/cmocka.def
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.907316 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/
+-rw-rw-rw-   0        0        0     7657 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0     6215 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/cmocka_test.cmake
+-rw-rw-rw-   0        0        0     2758 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/ctest-default.cmake
+-rw-rw-rw-   0        0        0     1922 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_alloc.c
+-rw-rw-rw-   0        0        0      818 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_assert_macros.c
+-rw-rw-rw-   0        0        0      862 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_assert_macros_fail.c
+-rw-rw-rw-   0        0        0     1550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_basics.c
+-rw-rw-rw-   0        0        0      970 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_cmockery.c
+-rw-rw-rw-   0        0        0      869 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_exception_handler.c
+-rw-rw-rw-   0        0        0     1774 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_fixtures.c
+-rw-rw-rw-   0        0        0     1206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_float_macros.c
+-rw-rw-rw-   0        0        0      992 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_group_fixtures.c
+-rw-rw-rw-   0        0        0      699 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_group_setup_assert.c
+-rw-rw-rw-   0        0        0      696 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_group_setup_fail.c
+-rw-rw-rw-   0        0        0     1757 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_groups.c
+-rw-rw-rw-   0        0        0     2767 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_ordering.c
+-rw-rw-rw-   0        0        0     2420 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_ordering_fail.c
+-rw-rw-rw-   0        0        0     1577 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_returns.c
+-rw-rw-rw-   0        0        0     1704 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_returns_fail.c
+-rw-rw-rw-   0        0        0     1092 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_setup_fail.c
+-rw-rw-rw-   0        0        0     1043 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_skip.c
+-rw-rw-rw-   0        0        0     1362 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_skip_filter.c
+-rw-rw-rw-   0        0        0     2280 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_strmatch.c
+-rw-rw-rw-   0        0        0     1260 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_wildcard.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.912830 pyjoulescope_driver-1.3.4/third-party/libusb/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.913330 pyjoulescope_driver-1.3.4/third-party/libusb/.github/
+-rw-rw-rw-   0        0        0      719 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.github/cifuzz.yml
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.914332 pyjoulescope_driver-1.3.4/third-party/libusb/.github/workflows/
+-rw-rw-rw-   0        0        0     1188 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.github/workflows/linux.yml
+-rw-rw-rw-   0        0        0     1023 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0      527 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.github/workflows/msys2.yml
+-rw-rw-rw-   0        0        0      827 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.917835 pyjoulescope_driver-1.3.4/third-party/libusb/.private/
+-rw-rw-rw-   0        0        0      202 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/README.txt
+-rw-rw-rw-   0        0        0      548 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/appveyor_build.sh
+-rw-rw-rw-   0        0        0     1424 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/bm.sh
+-rw-rw-rw-   0        0        0     1109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/ci-build.sh
+-rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/ci-container-build.sh
+-rw-rw-rw-   0        0        0      959 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/post-rewrite.sh
+-rw-rw-rw-   0        0        0     1995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/pre-commit.sh
+-rw-rw-rw-   0        0        0     2545 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.private/wbs.txt
+-rw-rw-rw-   0        0        0     1465 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/.travis.yml
+-rw-rw-rw-   0        0        0     2523 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.4/third-party/libusb/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1972 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/INSTALL_WIN.txt
+-rw-rw-rw-   0        0        0     1495 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Makefile.am
+-rw-rw-rw-   0        0        0     1395 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/README-FORK.md
+-rw-rw-rw-   0        0        0     1894 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/README.git
+-rw-rw-rw-   0        0        0        6 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.919835 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/
+-rw-rw-rw-   0        0        0     2409 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/common.xcconfig
+-rw-rw-rw-   0        0        0      995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/config.h
+-rw-rw-rw-   0        0        0     1135 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/debug.xcconfig
+-rw-rw-rw-   0        0        0      988 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb.xcconfig
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.920837 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb.xcodeproj/
+-rw-rw-rw-   0        0        0    62286 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
+-rw-rw-rw-   0        0        0      963 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb_debug.xcconfig
+-rw-rw-rw-   0        0        0      965 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb_release.xcconfig
+-rw-rw-rw-   0        0        0     1208 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/release.xcconfig
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.921340 pyjoulescope_driver-1.3.4/third-party/libusb/android/
+-rw-rw-rw-   0        0        0     2016 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/config.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.922342 pyjoulescope_driver-1.3.4/third-party/libusb/android/examples/
+-rw-rw-rw-   0        0        0    11355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/examples/unrooted_android.c
+-rw-rw-rw-   0        0        0     1156 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/examples/unrooted_android.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.923844 pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/
+-rw-rw-rw-   0        0        0      997 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/Android.mk
+-rw-rw-rw-   0        0        0     1370 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/Application.mk
+-rw-rw-rw-   0        0        0     3425 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/examples.mk
+-rw-rw-rw-   0        0        0     2056 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/libusb.mk
+-rw-rw-rw-   0        0        0     1355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/tests.mk
+-rw-rw-rw-   0        0        0     3820 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/appveyor.yml
+-rw-rw-rw-   0        0        0      191 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/autogen.sh
+-rw-rw-rw-   0        0        0      109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/bootstrap.sh
+-rw-rw-rw-   0        0        0    16514 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/configure.ac
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.925349 pyjoulescope_driver-1.3.4/third-party/libusb/doc/
+-rw-rw-rw-   0        0        0      685 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/doc/Makefile.in
+-rw-rw-rw-   0        0        0   115647 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/doc/doxygen.cfg.in
+-rw-rw-rw-   0        0        0     2923 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/doc/libusb.png
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.929349 pyjoulescope_driver-1.3.4/third-party/libusb/examples/
+-rw-rw-rw-   0        0        0      416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/Makefile.am
+-rw-rw-rw-   0        0        0    15812 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/dpfp.c
+-rw-rw-rw-   0        0        0    24573 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/ezusb.c
+-rw-rw-rw-   0        0        0     4247 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/ezusb.h
+-rw-rw-rw-   0        0        0     9593 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/fxload.c
+-rw-rw-rw-   0        0        0     3580 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/hotplugtest.c
+-rw-rw-rw-   0        0        0     2081 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/listdevs.c
+-rw-rw-rw-   0        0        0     6149 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/sam3u_benchmark.c
+-rw-rw-rw-   0        0        0     9765 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/testlibusb.c
+-rw-rw-rw-   0        0        0    40008 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/examples/xusb.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.802580 pyjoulescope_driver-1.3.4/third-party/libusb/include/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.929849 pyjoulescope_driver-1.3.4/third-party/libusb/include/linux/
+-rw-rw-rw-   0        0        0     5104 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.4/third-party/libusb/include/linux/config.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.929849 pyjoulescope_driver-1.3.4/third-party/libusb/include/macos/
+-rw-rw-rw-   0        0        0     5130 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/include/macos/config.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.937364 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/
+-rw-rw-rw-   0        0        0     2539 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/Makefile.am
+-rw-rw-rw-   0        0        0      780 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/Makefile.am.extra
+-rw-rw-rw-   0        0        0    99186 2022-09-20 23:33:57.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/core.c
+-rw-rw-rw-   0        0        0    37583 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/descriptor.c
+-rw-rw-rw-   0        0        0    15552 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/hotplug.c
+-rw-rw-rw-   0        0        0   113897 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/io.c
+-rw-rw-rw-   0        0        0     8221 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusb-1.0.def
+-rw-rw-rw-   0        0        0     1642 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusb-1.0.rc
+-rw-rw-rw-   0        0        0    78746 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusb.h
+-rw-rw-rw-   0        0        0    53532 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusbi.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.951884 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/
+-rw-rw-rw-   0        0        0   103226 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/darwin_usb.c
+-rw-rw-rw-   0        0        0     7071 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/darwin_usb.h
+-rw-rw-rw-   0        0        0    24325 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/emscripten_webusb.cpp
+-rw-rw-rw-   0        0        0     9581 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_posix.c
+-rw-rw-rw-   0        0        0     1776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_posix.h
+-rw-rw-rw-   0        0        0     6948 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_windows.c
+-rw-rw-rw-   0        0        0     1520 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_windows.h
+-rw-rw-rw-   0        0        0     7884 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_pollfs.cpp
+-rw-rw-rw-   0        0        0     3386 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb.h
+-rw-rw-rw-   0        0        0    16687 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb_backend.cpp
+-rw-rw-rw-   0        0        0     7477 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb_raw.cpp
+-rw-rw-rw-   0        0        0     4080 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb_raw.h
+-rw-rw-rw-   0        0        0    10778 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_netlink.c
+-rw-rw-rw-   0        0        0     8864 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_udev.c
+-rw-rw-rw-   0        0        0    83335 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_usbfs.c
+-rw-rw-rw-   0        0        0     6551 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_usbfs.h
+-rw-rw-rw-   0        0        0    16279 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/netbsd_usb.c
+-rw-rw-rw-   0        0        0     2996 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/null_usb.c
+-rw-rw-rw-   0        0        0    18179 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/openbsd_usb.c
+-rw-rw-rw-   0        0        0    45204 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/sunos_usb.c
+-rw-rw-rw-   0        0        0     2254 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/sunos_usb.h
+-rw-rw-rw-   0        0        0     3488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_posix.c
+-rw-rw-rw-   0        0        0     3052 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_posix.h
+-rw-rw-rw-   0        0        0     1416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_windows.c
+-rw-rw-rw-   0        0        0     3280 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_windows.h
+-rw-rw-rw-   0        0        0    30524 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_common.c
+-rw-rw-rw-   0        0        0    14347 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_common.h
+-rw-rw-rw-   0        0        0    24491 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_usbdk.c
+-rw-rw-rw-   0        0        0     2926 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_usbdk.h
+-rw-rw-rw-   0        0        0   171316 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_winusb.c
+-rw-rw-rw-   0        0        0    24670 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_winusb.h
+-rw-rw-rw-   0        0        0     8776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/strerror.c
+-rw-rw-rw-   0        0        0    13160 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/sync.c
+-rw-rw-rw-   0        0        0      449 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/version.h
+-rw-rw-rw-   0        0        0       27 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb/version_nano.h
+-rw-rw-rw-   0        0        0      323 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/libusb-1.0.pc.in
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.960895 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/
+-rw-rw-rw-   0        0        0      136 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/.gitattributes
+-rw-rw-rw-   0        0        0     2982 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Base.props
+-rw-rw-rw-   0        0        0      287 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Configuration.Application.props
+-rw-rw-rw-   0        0        0     2817 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Configuration.Base.props
+-rw-rw-rw-   0        0        0      612 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Configuration.DynamicLibrary.props
+-rw-rw-rw-   0        0        0      289 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Configuration.StaticLibrary.props
+-rw-rw-rw-   0        0        0     1438 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/ProjectConfigurations.Base.props
+-rw-rw-rw-   0        0        0      713 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/build_all.ps1
+-rw-rw-rw-   0        0        0     2007 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/config.h
+-rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/dpfp.vcxproj
+-rw-rw-rw-   0        0        0     1659 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/dpfp_threaded.vcxproj
+-rw-rw-rw-   0        0        0     2125 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/fxload.vcxproj
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.962398 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt/
+-rw-rw-rw-   0        0        0    31341 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt/getopt.c
+-rw-rw-rw-   0        0        0     6627 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt/getopt.h
+-rw-rw-rw-   0        0        0     4708 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt/getopt1.c
+-rw-rw-rw-   0        0        0     1522 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt.vcxproj
+-rw-rw-rw-   0        0        0     1444 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/hotplugtest.vcxproj
+-rw-rw-rw-   0        0        0    17271 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/libusb.sln
+-rw-rw-rw-   0        0        0     2762 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/libusb_dll.vcxproj
+-rw-rw-rw-   0        0        0     2336 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/libusb_static.vcxproj
+-rw-rw-rw-   0        0        0     1441 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/listdevs.vcxproj
+-rw-rw-rw-   0        0        0     1488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/sam3u_benchmark.vcxproj
+-rw-rw-rw-   0        0        0     1579 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/stress.vcxproj
+-rw-rw-rw-   0        0        0     1443 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/testlibusb.vcxproj
+-rw-rw-rw-   0        0        0     1709 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/msvc/xusb.vcxproj
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.963398 pyjoulescope_driver-1.3.4/third-party/libusb/tests/
+-rw-rw-rw-   0        0        0      623 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/tests/Makefile.am
+-rw-rw-rw-   0        0        0     2490 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/tests/libusb_testlib.h
+-rw-rw-rw-   0        0        0     4935 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/tests/stress.c
+-rw-rw-rw-   0        0        0     4919 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/tests/testlib.c
+-rw-rw-rw-   0        0        0    37223 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.4/third-party/libusb/tests/umockdev.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:15:17.965403 pyjoulescope_driver-1.3.4/third-party/tinyprintf/
+-rw-rw-rw-   0        0        0      122 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/tinyprintf/CMakeLists.txt
+-rw-rw-rw-   0        0        0    13188 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/tinyprintf/tinyprintf.c
+-rw-rw-rw-   0        0        0     6550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/tinyprintf/tinyprintf.h
+-rw-rw-rw-   0        0        0     1554 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.4/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
```

### Comparing `pyjoulescope_driver-1.3.3/CHANGELOG.md` & `pyjoulescope_driver-1.3.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the Joulescope driver.
 
 
+## 1.3.4
+
+2023 Apr 26
+
+* Fixed record jls version check.
+* Send buffer signal clear on free.
+* Updated to pyjls 0.6.0.
+  * Fixed pyjoulescope_driver.record to not remove sample_id offset.  
+
+
 ## 1.3.3
 
 2023 Apr 19
 
 * Cleared all message fields at allocation.
 * Added api_timeout entry point test.
 * Improved thread entry point test.
```

### Comparing `pyjoulescope_driver-1.3.3/LICENSE.txt` & `pyjoulescope_driver-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/PKG-INFO` & `pyjoulescope_driver-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope_driver
-Version: 1.3.3
+Version: 1.3.4
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.3.3/README.md` & `pyjoulescope_driver-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/credits.html` & `pyjoulescope_driver-1.3.4/credits.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/cmacro_inc.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/cmacro_inc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/cstr.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/cstr.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/error_code.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/error_code.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/log.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/log.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/meta.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/meta.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/time.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/time.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/topic.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/topic.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/union.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/union.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv/version.h` & `pyjoulescope_driver-1.3.4/include/jsdrv/version.h`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 #define JSDRV_VERSION_MINOR 3
 
 /**
  * @brief The Joulescope driver patch version.
  *
  * Changes in the patch version indicate bug fixes and improvements.
  */
-#define JSDRV_VERSION_PATCH 3
+#define JSDRV_VERSION_PATCH 4
 
 /**
  * \brief The maximum version string length.
  *
  * The actual length is 14 bytes (MMM.mmm.ppppp\\x00), but round up
  * to simplify packing.
  */
```

### Comparing `pyjoulescope_driver-1.3.3/include/jsdrv.h` & `pyjoulescope_driver-1.3.4/include/jsdrv.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/js220_api.h` & `pyjoulescope_driver-1.3.4/include_private/js220_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/assert.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/assert.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/backend.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/backend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/buffer.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer_signal.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/buffer_signal.h`

 * *Files 4% similar despite different names*

```diff
@@ -86,17 +86,19 @@
  * @param r0 The number of samples in the first reduction.
  * @param rN The number of samples in subsequent reductions.
  */
 void jsdrv_bufsig_alloc(struct bufsig_s * self, uint64_t N, uint64_t r0, uint64_t rN);
 
 void jsdrv_bufsig_free(struct bufsig_s * self);
 
+void jsdrv_bufsig_clear(struct bufsig_s * self);
+
 void jsdrv_bufsig_recv_data(struct bufsig_s * self, struct jsdrv_stream_signal_s * s);
 
-void jsdrv_bufsig_info(struct bufsig_s * self, struct jsdrv_buffer_info_s * info);
+bool jsdrv_bufsig_info(struct bufsig_s * self, struct jsdrv_buffer_info_s * info);
 
 /**
  * @brief Process a request.
  *
  * @param self The buffer instance.
  * @param req The request to process.
  * @param rsp The response to populate which is mostly populated by the caller.
```

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/cdef.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/dbc.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/dbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/device.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/device.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/devices.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/devices.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/downsample.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/downsample.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/event.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/event.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/frontend.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/frontend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_cal.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js110_cal.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_sample_processor.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js110_sample_processor.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_stats.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js110_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_i128.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js220_i128.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_stats.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/js220_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/json.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/json.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/list.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/list.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/log.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/log.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/msg_queue.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/msg_queue.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/mutex.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/mutex.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/platform.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/platform.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/pubsub.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/pubsub.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/sample_buffer_f32.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/sample_buffer_f32.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/statistics.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/thread.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/thread.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/usb_spec.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/usb_spec.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/windows.h` & `pyjoulescope_driver-1.3.4/include_private/jsdrv_prv/windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/__init__.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/__main__.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/binding.c` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/binding.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
         ],
         "include_dirs": [
             "C:\\repos\\Jetperch\\joulescope_driver\\include",
             "C:\\repos\\Jetperch\\joulescope_driver\\include_private",
             "C:\\repos\\Jetperch\\joulescope_driver\\third-party\\tinyprintf",
-            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include"
+            "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include"
         ],
         "libraries": [
             "Setupapi",
             "Winusb",
             "user32"
         ],
         "name": "pyjoulescope_driver.binding",
@@ -1161,195 +1161,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1381,42 +1381,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_19pyjoulescope_driver_7binding_Driver;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -13086,15 +13086,15 @@
   __Pyx_XDECREF(__pyx_v_record);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13103,29 +13103,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13136,15 +13136,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13153,29 +13153,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13186,15 +13186,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13203,29 +13203,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13236,15 +13236,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13253,29 +13253,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13286,15 +13286,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13303,29 +13303,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13336,212 +13336,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":928
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":932
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":940
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13557,15 +13557,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -13573,53 +13573,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -13627,30 +13627,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13665,15 +13665,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":946
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13689,15 +13689,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13705,53 +13705,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -13759,30 +13759,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13797,15 +13797,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":952
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13821,15 +13821,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13837,53 +13837,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -13891,30 +13891,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13929,176 +13929,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":981
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":996
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -28585,26 +28585,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._context cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_self__context_cannot_be_converte); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../bin/Python3_11_3/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 950, __pyx_L1_error)
```

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/__init__.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/api_timeout.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/api_timeout.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/gpi.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/gpi.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/info.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/program.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/record.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/record.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/scan.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/set_parameter.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/set_parameter.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/statistics.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/threads.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/entry_points/threads.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_alpha.img` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/img_alpha.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_beta.img` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/img_beta.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_stable.img` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/img_stable.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/program.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/record.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import copy
 import numpy as np
 from pyjoulescope_driver import time64
 import logging
 
 
-_PYJLS_VERSION_MIN = (0, 5, 0)  # inclusive
+_PYJLS_VERSION_MIN = (0, 6, 0)  # inclusive
 _PYJLS_VERSION_MAX = (1, 0, 0)  # exclusive
 
 
 try:
     from pyjls import Writer, SignalType, DataType, __version__
     _DTYPE_MAP = {
         'f32': DataType.F32,
@@ -131,15 +131,15 @@
     Call :meth:`open` to start recording and :meth:`close` to stop.
     """
 
     def __init__(self, driver, device_path, signals=None):
         if Writer is None:
             raise RuntimeError('pyjls package not found.  Install using:\n' +
                                '  pip3 install -U pyjls')
-        pyjls_version = [int(x) for x in __version__.split('.')]
+        pyjls_version = tuple([int(x) for x in __version__.split('.')])
         if pyjls_version < _PYJLS_VERSION_MIN or pyjls_version >= _PYJLS_VERSION_MAX:
             raise ImportError(f'Unsupported pyjls version {__version__}\n' +
                               f'  Require {_PYJLS_VERSION_MIN} <= pyjls version < {_PYJLS_VERSION_MAX}\n' +
                               '  pip3 install -U pyjls')
         self._utc_interval = time64.MINUTE
         self._log = logging.getLogger(__name__)
         self._wr = None
@@ -224,29 +224,28 @@
 
     def _on_data(self, topic, value):
         signal = self._data_map[topic]
         decimate_factor = value['decimate_factor']
         signal_id = signal['signal_id']
         sample_id = value['sample_id']
         if signal['utc_next'] is None:
-            signal['sample_id_offset'] = sample_id
             signal['sample_id_next'] = 0
             self._wr.signal_def(
                 signal_id=signal['signal_id'],
                 source_id=1,
                 signal_type=SignalType.FSR,
                 data_type=signal['signal_type'],
                 sample_rate=value['sample_rate'] // decimate_factor,
                 name=signal['name'],
                 units=signal['units'],
             )
             self._wr.utc(signal_id, 0, value['utc'])
             signal['utc_next'] = value['utc'] + self._utc_interval
 
-        sample_id = (sample_id - signal['sample_id_offset']) // decimate_factor
+        sample_id = sample_id // decimate_factor
         if value['utc'] >= signal['utc_next']:
             self._wr.utc(signal_id, sample_id, value['utc'])
             signal['utc_next'] += self._utc_interval
             signal['utc'] = None
         elif sample_id:
             signal['utc'] = (sample_id, value['utc'])
```

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/release.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_release.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/test/test_release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_time64.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/test/test_time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/time64.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver/version.py` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 
 __title__ = "pyjoulescope_driver"
 __description__ = 'Joulescope™ driver'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/PKG-INFO` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope-driver
-Version: 1.3.3
+Version: 1.3.4
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/SOURCES.txt` & `pyjoulescope_driver-1.3.4/pyjoulescope_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/pyproject.toml` & `pyjoulescope_driver-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/setup.py` & `pyjoulescope_driver-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/libusb/backend.c` & `pyjoulescope_driver-1.3.4/src/backend/libusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/libusb/msg_queue.c` & `pyjoulescope_driver-1.3.4/src/backend/libusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/posix.c` & `pyjoulescope_driver-1.3.4/src/backend/posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/windows.c` & `pyjoulescope_driver-1.3.4/src/backend/windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/winusb/backend.c` & `pyjoulescope_driver-1.3.4/src/backend/winusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.c` & `pyjoulescope_driver-1.3.4/src/backend/winusb/device_change_notifier.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.h` & `pyjoulescope_driver-1.3.4/src/backend/winusb/device_change_notifier.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/backend/winusb/msg_queue.c` & `pyjoulescope_driver-1.3.4/src/backend/winusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/buffer.c` & `pyjoulescope_driver-1.3.4/src/buffer.c`

 * *Files 0% similar despite different names*

```diff
@@ -175,20 +175,21 @@
     }
     return true;
 }
 
 static void bufsig_publish_info(struct bufsig_s * self) {
     struct jsdrv_context_s * context = self->parent->context;
     struct jsdrv_buffer_info_s info;
-    jsdrv_bufsig_info(self, &info);
-    struct jsdrvp_msg_s * m = jsdrvp_msg_alloc_value(context, "",
-            &jsdrv_union_cbin_r((uint8_t *) &info, sizeof(info)));
-    tfp_snprintf(m->topic, sizeof(m->topic), "m/%03d/s/%03d/info", self->parent->idx, self->idx);
-    m->value.app = JSDRV_PAYLOAD_TYPE_BUFFER_INFO;
-    jsdrvp_backend_send(context, m);
+    if (jsdrv_bufsig_info(self, &info)) {
+        struct jsdrvp_msg_s * m = jsdrvp_msg_alloc_value(context, "",
+                &jsdrv_union_cbin_r((uint8_t *) &info, sizeof(info)));
+        tfp_snprintf(m->topic, sizeof(m->topic), "m/%03d/s/%03d/info", self->parent->idx, self->idx);
+        m->value.app = JSDRV_PAYLOAD_TYPE_BUFFER_INFO;
+        jsdrvp_backend_send(context, m);
+    }
 }
 
 static void buffer_alloc(struct buffer_s * self) {
     double coef_f32 = sizeof(float);
     double coef_u = 0.0;
     JSDRV_LOGI("buffer_alloc %" PRIu64, self->size);
     size_t summary_entry_sz = sizeof(struct jsdrv_summary_entry_s);
@@ -249,14 +250,16 @@
 
 static void buffer_free(struct buffer_s * self) {
     if (self->state == ST_ACTIVE) {
         self->state = ST_AWAIT;
     }
     for (uint32_t idx = 0; idx < JSDRV_BUFSIG_COUNT_MAX; ++idx) {
         struct bufsig_s *b = &self->signals[idx];
+        jsdrv_bufsig_clear(b);
+        bufsig_publish_info(b);
         jsdrv_bufsig_free(b);
     }
 }
 
 static void req_post(struct buffer_s * self, uint32_t bufsig_idx, struct jsdrv_buffer_request_s * req) {
     struct jsdrv_list_s * item;
     struct req_s * r;
```

### Comparing `pyjoulescope_driver-1.3.3/src/buffer_signal.c` & `pyjoulescope_driver-1.3.4/src/buffer_signal.c`

 * *Files 0% similar despite different names*

```diff
@@ -149,16 +149,19 @@
         samples->end = 0;
     } else {
         samples->end = jsdrv_time_to_counter(&self->time_map, utc->end);
     }
     samples->length = length;
 }
 
-void jsdrv_bufsig_info(struct bufsig_s * self, struct jsdrv_buffer_info_s * info) {
+bool jsdrv_bufsig_info(struct bufsig_s * self, struct jsdrv_buffer_info_s * info) {
     memset(info, 0, sizeof(*info));
+    if (0 == self->hdr.element_size_bits) {
+        return false;
+    }
     info->version = 1;
     info->field_id = self->hdr.field_id;
     info->index = self->hdr.index;
     info->element_type = self->hdr.element_type;
     info->element_size_bits = self->hdr.element_size_bits;
     info->size_in_utc = self->size_in_utc;
     info->size_in_samples = self->N;
@@ -175,14 +178,15 @@
     } else {
         info->time_range_samples.start = self->sample_id_head - self->level0_size;
         info->time_range_samples.end = self->sample_id_head - 1;
         info->time_range_samples.length = self->level0_size;
         samples_to_utc(self, &info->time_range_samples, &info->time_range_utc);
     }
     info->time_map = self->time_map;
+    return true;
 }
 
 static void summarizeN(struct bufsig_s * self, uint8_t level, uint64_t start_idx, uint64_t length) {
     struct bufsig_level_s * lvl_dn = &self->levels[level - 1];
     struct bufsig_level_s * lvl_up = &self->levels[level];
     if (NULL == lvl_up->data) {
         return;
@@ -238,14 +242,18 @@
     self->level0_head = 0;
     self->level0_size = 0;
     self->sample_id_head = sample_id;
     self->time_map.offset_counter = sample_id;
     self->time_map.offset_time = jsdrv_time_utc();
 }
 
+void jsdrv_bufsig_clear(struct bufsig_s * self) {
+    clear(self, 0);
+}
+
 void jsdrv_bufsig_recv_data(struct bufsig_s * self, struct jsdrv_stream_signal_s * s) {
     self->hdr.sample_id = s->sample_id;
     self->hdr.field_id = s->field_id;
     self->hdr.index = s->index;
     self->hdr.element_type = s->element_type;
     self->hdr.element_size_bits = s->element_size_bits;
     self->hdr.element_count = s->element_count;
@@ -265,26 +273,26 @@
     if (self->sample_id_head == 0) {
         JSDRV_LOGI("received initial sample, ignore skips, "
                    "sample_id=%" PRIu64 " | %" PRIu64
                    ", sample_rate=%d, decimate=%d",
                    s->sample_id, sample_id, s->sample_rate, s->decimate_factor);
         clear(self, sample_id);
     } else if (sample_id_end < sample_id_expect) {
-        JSDRV_LOGW("bufsig_recv_data %s: duplicate rcv=[%" PRIu64 ", %" PRIu64 "] expect=%" PRIu64,
+        JSDRV_LOGI("bufsig_recv_data %s: duplicate rcv=[%" PRIu64 ", %" PRIu64 "] expect=%" PRIu64,
                    self->topic, sample_id, sample_id_end, sample_id_expect);
         if ((sample_id_expect - sample_id_end) < self->N) {
             clear(self, sample_id);
         }
         return;
     } else if (sample_id < sample_id_expect) {
-        JSDRV_LOGW("bufsig_recv_data %s: overlap rcv=[%" PRIu64 ", %" PRIu64 "] expect=%" PRIu64,
+        JSDRV_LOGI("bufsig_recv_data %s: overlap rcv=[%" PRIu64 ", %" PRIu64 "] expect=%" PRIu64,
                    self->topic, sample_id, sample_id_end, sample_id_expect);
         return;
     } else if (sample_id > sample_id_expect) {
-        JSDRV_LOGW("bufsig_recv_data %s: skip rcv=[%" PRIu64 ", %" PRIu64 "] expect=%" PRIu64,
+        JSDRV_LOGI("bufsig_recv_data %s: skip rcv=[%" PRIu64 ", %" PRIu64 "] expect=%" PRIu64,
                    self->topic, sample_id, sample_id_end, sample_id_expect);
         uint64_t k = sample_id - sample_id_expect;
         if (k > self->N) {
             clear(self, sample_id);
         } else {
             if (s->element_type == JSDRV_DATA_TYPE_FLOAT) {
                 if (s->element_size_bits == 32) {
```

### Comparing `pyjoulescope_driver-1.3.3/src/cstr.c` & `pyjoulescope_driver-1.3.4/src/cstr.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/devices.c` & `pyjoulescope_driver-1.3.4/src/devices.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/downsample.c` & `pyjoulescope_driver-1.3.4/src/downsample.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/emu.c` & `pyjoulescope_driver-1.3.4/src/emu.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/emulated.c` & `pyjoulescope_driver-1.3.4/src/emulated.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/error_code.c` & `pyjoulescope_driver-1.3.4/src/error_code.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js110_api.h` & `pyjoulescope_driver-1.3.4/src/js110_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js110_cal.c` & `pyjoulescope_driver-1.3.4/src/js110_cal.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js110_sample_processor.c` & `pyjoulescope_driver-1.3.4/src/js110_sample_processor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js110_stats.c` & `pyjoulescope_driver-1.3.4/src/js110_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js110_usb.c` & `pyjoulescope_driver-1.3.4/src/js110_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js220_i128.c` & `pyjoulescope_driver-1.3.4/src/js220_i128.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js220_params.c` & `pyjoulescope_driver-1.3.4/src/js220_params.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js220_stats.c` & `pyjoulescope_driver-1.3.4/src/js220_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/js220_usb.c` & `pyjoulescope_driver-1.3.4/src/js220_usb.c`

 * *Files 1% similar despite different names*

```diff
@@ -956,15 +956,15 @@
         d->time_map.offset_counter = sample_id;
     }
 }
 
 static void handle_stream_in_port(struct dev_s * d, uint8_t port_id, uint32_t * p_u32, uint16_t size) {
     struct field_def_s * field_def = &PORT_MAP[port_id & 0x0f];
     struct port_s * port = &d->ports[port_id & 0x0f];
-    struct jsdrv_stream_signal_s * s;
+    struct jsdrv_stream_signal_s * s = NULL;
     struct jsdrvp_msg_s * m = port->msg_in;
     if (!field_def->data_topic || !field_def->data_topic[0]) {
         return;
     }
 
     // header is u32 sample_id, consume and skip to payload
     // sample_id is always for 2 Msps, regardless of this port's sample rate
@@ -994,25 +994,28 @@
                    port_id, sample_id_u64, port->sample_id_next);
         uint32_t skip = (uint32_t) (port->sample_id_next - sample_id_u64);
         uint16_t skip_size = (uint16_t) ((skip * field_def->element_size_bits) / 8);
         size -= skip_size;
         sample_count -= skip;
         p_u32 += skip_size / sizeof(uint32_t);
     } else {
-        JSDRV_LOGI("stream_in_port %d sample_id skip: received=%" PRIu64 " expected=%" PRIu64,
-                   port_id, sample_id_u64, port->sample_id_next);
+        uint32_t element_count = 0;
         if (m) {
             s = (struct jsdrv_stream_signal_s *) m->value.value.bin;
-            JSDRV_LOGI("stream_in_port %d early send %" PRIu32 " bytes, %" PRIu32 " elements",
-                       port_id, m->value.size, s->element_count);
+            element_count = s->element_count;
             port->msg_in = NULL;
             jsdrvp_backend_send(d->context, m);
             m = NULL;
             s = NULL;
         }
+        JSDRV_LOGI("stream_in_port %d sample_id skip: received=%" PRIu64 " expected=%" PRIu64
+                   " d=%" PRIu64 ", %" PRIu32 " elements sent",
+                   port_id, sample_id_u64, port->sample_id_next,
+                   sample_id_u64 - port->sample_id_next,
+                   element_count);
         port->sample_id_next = sample_id_u64;
     }
 
     switch (port_id) {
         case PORT_ID_CURRENT:
             sbuf_f32_add(&d->i_buf, port->sample_id_next, (float *) p_u32, sample_count);
             break;
```

### Comparing `pyjoulescope_driver-1.3.3/src/jsdrv.c` & `pyjoulescope_driver-1.3.4/src/jsdrv.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/json.c` & `pyjoulescope_driver-1.3.4/src/json.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/log.c` & `pyjoulescope_driver-1.3.4/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/meta.c` & `pyjoulescope_driver-1.3.4/src/meta.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/pubsub.c` & `pyjoulescope_driver-1.3.4/src/pubsub.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/sample_buffer_f32.c` & `pyjoulescope_driver-1.3.4/src/sample_buffer_f32.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/statistics.c` & `pyjoulescope_driver-1.3.4/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/time.c` & `pyjoulescope_driver-1.3.4/src/time.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/topic.c` & `pyjoulescope_driver-1.3.4/src/topic.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/union.c` & `pyjoulescope_driver-1.3.4/src/union.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/src/version.c` & `pyjoulescope_driver-1.3.4/src/version.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/.gitlab-ci.yml` & `pyjoulescope_driver-1.3.4/third-party/cmocka/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/.ycm_extra_conf.py` & `pyjoulescope_driver-1.3.4/third-party/cmocka/.ycm_extra_conf.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/5.patch` & `pyjoulescope_driver-1.3.4/third-party/cmocka/5.patch`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/cmocka/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/CPackConfig.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/CPackConfig.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/CompilerChecks.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/CompilerChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/ConfigureChecks.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/ConfigureChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/INSTALL.md` & `pyjoulescope_driver-1.3.4/third-party/cmocka/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/README.md` & `pyjoulescope_driver-1.3.4/third-party/cmocka/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/FindNSIS.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/FindNSIS.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-cross-m32.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/cmake/Toolchain-cross-m32.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/config.h.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/coverity_assert_model.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/coverity/coverity_assert_model.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/index.html` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/mainpage.dox` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/mainpage.dox`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/README.md` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/header.html` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/header.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/doc.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/doc.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderclosed.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/folderclosed.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderopen.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/folderopen.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/mag_glass.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/mag_glass.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_left.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/nav_edge_left.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_right.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/nav_edge_right.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/splitbar_handle.svg` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/img/splitbar_handle.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/js/striped_bg.js` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/js/striped_bg.js`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/that_style.css` & `pyjoulescope_driver-1.3.4/third-party/cmocka/doc/that_style/that_style.css`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/allocate_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module_test.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/allocate_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_macro.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro_test.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_macro_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.h` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_module.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module_test.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/assert_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/calculator.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator_test.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/calculator_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/database.h` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/database.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/chef.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.h` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/chef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/README.md` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/proc_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.h` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/proc_uptime.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/test_uptime.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/test_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/uptime.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/example/mock/uptime/uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka.h` & `pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmocka.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_pbc.h` & `pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmocka_pbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_private.h` & `pyjoulescope_driver-1.3.4/third-party/cmocka/include/cmocka_private.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/src/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/cmocka/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/src/cmocka.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.def` & `pyjoulescope_driver-1.3.4/third-party/cmocka/src/cmocka.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/cmocka_test.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/cmocka_test.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/ctest-default.cmake` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/ctest-default.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_alloc.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_alloc.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_assert_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros_fail.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_assert_macros_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_basics.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_basics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_cmockery.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_cmockery.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_exception_handler.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_exception_handler.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_fixtures.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_float_macros.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_float_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_fixtures.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_group_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_assert.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_group_setup_assert.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_fail.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_group_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_groups.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_groups.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_ordering.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering_fail.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_ordering_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_returns.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns_fail.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_returns_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_setup_fail.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_skip.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip_filter.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_skip_filter.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_strmatch.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_strmatch.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_wildcard.c` & `pyjoulescope_driver-1.3.4/third-party/cmocka/tests/test_wildcard.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.github/cifuzz.yml` & `pyjoulescope_driver-1.3.4/third-party/libusb/.github/cifuzz.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/linux.yml` & `pyjoulescope_driver-1.3.4/third-party/libusb/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/macos.yml` & `pyjoulescope_driver-1.3.4/third-party/libusb/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/msys2.yml` & `pyjoulescope_driver-1.3.4/third-party/libusb/.github/workflows/msys2.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.gitignore` & `pyjoulescope_driver-1.3.4/third-party/libusb/.gitignore`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.private/appveyor_build.sh` & `pyjoulescope_driver-1.3.4/third-party/libusb/.private/appveyor_build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.private/bm.sh` & `pyjoulescope_driver-1.3.4/third-party/libusb/.private/bm.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-build.sh` & `pyjoulescope_driver-1.3.4/third-party/libusb/.private/ci-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-container-build.sh` & `pyjoulescope_driver-1.3.4/third-party/libusb/.private/ci-container-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.private/post-rewrite.sh` & `pyjoulescope_driver-1.3.4/third-party/libusb/.private/post-rewrite.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.private/pre-commit.sh` & `pyjoulescope_driver-1.3.4/third-party/libusb/.private/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.private/wbs.txt` & `pyjoulescope_driver-1.3.4/third-party/libusb/.private/wbs.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/.travis.yml` & `pyjoulescope_driver-1.3.4/third-party/libusb/.travis.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/CMakeLists.txt` & `pyjoulescope_driver-1.3.4/third-party/libusb/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/INSTALL_WIN.txt` & `pyjoulescope_driver-1.3.4/third-party/libusb/INSTALL_WIN.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Makefile.am` & `pyjoulescope_driver-1.3.4/third-party/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/README-FORK.md` & `pyjoulescope_driver-1.3.4/third-party/libusb/README-FORK.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/README.git` & `pyjoulescope_driver-1.3.4/third-party/libusb/README.git`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/common.xcconfig` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/common.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/config.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/debug.xcconfig` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcconfig` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_debug.xcconfig` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb_debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_release.xcconfig` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/libusb_release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/release.xcconfig` & `pyjoulescope_driver-1.3.4/third-party/libusb/Xcode/release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/config.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/examples/unrooted_android.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/examples/unrooted_android.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Android.mk` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/Android.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Application.mk` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/Application.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/examples.mk` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/examples.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/libusb.mk` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/libusb.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/tests.mk` & `pyjoulescope_driver-1.3.4/third-party/libusb/android/jni/tests.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/appveyor.yml` & `pyjoulescope_driver-1.3.4/third-party/libusb/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/configure.ac` & `pyjoulescope_driver-1.3.4/third-party/libusb/configure.ac`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/doc/Makefile.in` & `pyjoulescope_driver-1.3.4/third-party/libusb/doc/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/doc/doxygen.cfg.in` & `pyjoulescope_driver-1.3.4/third-party/libusb/doc/doxygen.cfg.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/doc/libusb.png` & `pyjoulescope_driver-1.3.4/third-party/libusb/doc/libusb.png`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/dpfp.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/dpfp.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/ezusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/ezusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/fxload.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/fxload.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/hotplugtest.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/hotplugtest.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/listdevs.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/listdevs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/sam3u_benchmark.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/sam3u_benchmark.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/testlibusb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/testlibusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/examples/xusb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/examples/xusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/include/linux/config.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/include/linux/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/include/macos/config.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/include/macos/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am.extra` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/Makefile.am.extra`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/core.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/core.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/descriptor.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/descriptor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/hotplug.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/hotplug.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/io.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/io.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.def` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusb-1.0.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.rc` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusb-1.0.rc`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusbi.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/libusbi.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/darwin_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/darwin_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/emscripten_webusb.cpp` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/emscripten_webusb.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/events_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_pollfs.cpp` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_pollfs.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_backend.cpp` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb_backend.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.cpp` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb_raw.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/haiku_usb_raw.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_netlink.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_netlink.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_udev.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_udev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_usbfs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/linux_usbfs.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/netbsd_usb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/netbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/null_usb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/null_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/openbsd_usb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/openbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/sunos_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/sunos_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/threads_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_common.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_common.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_usbdk.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_usbdk.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_winusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/os/windows_winusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/strerror.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/strerror.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/sync.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/libusb/sync.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Base.props` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.Base.props` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Configuration.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.DynamicLibrary.props` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/Configuration.DynamicLibrary.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/ProjectConfigurations.Base.props` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/ProjectConfigurations.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/build_all.ps1` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/build_all.ps1`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/config.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/dpfp.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp_threaded.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/dpfp_threaded.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/fxload.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/fxload.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt/getopt.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt/getopt.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt1.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt/getopt1.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/getopt.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/hotplugtest.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/hotplugtest.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb.sln` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/libusb.sln`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_dll.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/libusb_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_static.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/libusb_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/listdevs.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/listdevs.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/sam3u_benchmark.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/sam3u_benchmark.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/stress.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/stress.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/testlibusb.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/testlibusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/xusb.vcxproj` & `pyjoulescope_driver-1.3.4/third-party/libusb/msvc/xusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/tests/Makefile.am` & `pyjoulescope_driver-1.3.4/third-party/libusb/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/tests/libusb_testlib.h` & `pyjoulescope_driver-1.3.4/third-party/libusb/tests/libusb_testlib.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/tests/stress.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/tests/stress.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/tests/testlib.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/tests/testlib.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/libusb/tests/umockdev.c` & `pyjoulescope_driver-1.3.4/third-party/libusb/tests/umockdev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.c` & `pyjoulescope_driver-1.3.4/third-party/tinyprintf/tinyprintf.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.h` & `pyjoulescope_driver-1.3.4/third-party/tinyprintf/tinyprintf.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new` & `pyjoulescope_driver-1.3.4/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new`

 * *Files identical despite different names*

