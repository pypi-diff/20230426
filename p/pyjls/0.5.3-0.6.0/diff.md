# Comparing `tmp/pyjls-0.5.3.tar.gz` & `tmp/pyjls-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.5.3.tar", last modified: Wed Apr 19 20:43:22 2023, max compression
+gzip compressed data, was "pyjls-0.6.0.tar", last modified: Wed Apr 26 20:14:11 2023, max compression
```

## Comparing `pyjls-0.5.3.tar` & `pyjls-0.6.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.495623 pyjls-0.5.3/
--rw-rw-rw-   0        0        0     3885 2023-04-19 20:33:20.000000 pyjls-0.5.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.5.3/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.5.3/LICENSE
--rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14665 2023-04-19 20:43:22.495623 pyjls-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.455550 pyjls-0.5.3/include/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.461069 pyjls-0.5.3/include/jls/
--rw-rw-rw-   0        0        0     2729 2023-04-19 20:33:33.000000 pyjls-0.5.3/include/jls/backend.h
--rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/cmacro.h
--rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/crc32c.h
--rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/ec.h
--rw-rw-rw-   0        0        0    24367 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/format.h
--rw-rw-rw-   0        0        0    11561 2023-04-19 17:02:21.000000 pyjls-0.5.3/include/jls/log.h
--rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/raw.h
--rw-rw-rw-   0        0        0     9052 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/reader.h
--rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/statistics.h
--rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/threaded_writer.h
--rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.5.3/include/jls/time.h
--rw-rw-rw-   0        0        0     2760 2023-04-19 20:32:45.000000 pyjls-0.5.3/include/jls/version.h
--rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls/writer.h
--rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.5.3/include/jls.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.452041 pyjls-0.5.3/include_prv/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.464573 pyjls-0.5.3/include_prv/jls/
--rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.5.3/include_prv/jls/bit_shift.h
--rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/cdef.h
--rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.5.3/include_prv/jls/datatype.h
--rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/msg_ring_buffer.h
--rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/util.h
--rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/wr_fsr.h
--rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/wr_prv.h
--rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.5.3/include_prv/jls/wr_ts.h
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.467578 pyjls-0.5.3/pyjls/
--rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.5.3/pyjls/__init__.py
--rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/__main__.py
--rw-rw-rw-   0        0        0  1571611 2023-04-19 20:27:59.000000 pyjls-0.5.3/pyjls/binding.c
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.487104 pyjls-0.5.3/pyjls/entry_points/
--rw-rw-rw-   0        0        0      853 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/entry_points/__init__.py
--rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/entry_points/annotate.py
--rw-rw-rw-   0        0        0     1621 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/entry_points/info.py
--rw-rw-rw-   0        0        0     2128 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.488104 pyjls-0.5.3/pyjls/test/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/test/__init__.py
--rw-rw-rw-   0        0        0     9517 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/test/test_binding.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.488104 pyjls-0.5.3/pyjls/v1/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.5.3/pyjls/v1/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-04-19 17:03:22.000000 pyjls-0.5.3/pyjls/version.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.485599 pyjls-0.5.3/pyjls.egg-info/
--rw-rw-rw-   0        0        0    14665 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1272 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 20:43:22.000000 pyjls-0.5.3/pyjls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 20:43:22.496625 pyjls-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     6931 2023-03-09 18:55:17.000000 pyjls-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:43:22.495623 pyjls-0.5.3/src/
--rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.5.3/src/backend_posix.c
--rw-rw-rw-   0        0        0     9046 2023-04-19 20:31:50.000000 pyjls-0.5.3/src/backend_win.c
--rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.5.3/src/bit_shift.c
--rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/crc32c_arm_neon.c
--rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/crc32c_intel_sse4.c
--rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/crc32c_sw.c
--rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.5.3/src/datatype.c
--rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/ec.c
--rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.5.3/src/log.c
--rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.5.3/src/msg_ring_buffer.c
--rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.5.3/src/raw.c
--rw-rw-rw-   0        0        0    50573 2023-03-04 19:36:06.000000 pyjls-0.5.3/src/reader.c
--rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/statistics.c
--rw-rw-rw-   0        0        0    11268 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/threaded_writer.c
--rw-rw-rw-   0        0        0    22020 2023-03-16 12:30:55.000000 pyjls-0.5.3/src/wr_fsr.c
--rw-rw-rw-   0        0        0     9691 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/wr_ts.c
--rw-rw-rw-   0        0        0    30342 2022-03-05 19:14:45.000000 pyjls-0.5.3/src/writer.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.177720 pyjls-0.6.0/
+-rw-rw-rw-   0        0        0     4058 2023-04-26 19:37:06.000000 pyjls-0.6.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.6.0/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14665 2023-04-26 20:14:11.177720 pyjls-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.146674 pyjls-0.6.0/include/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.152190 pyjls-0.6.0/include/jls/
+-rw-rw-rw-   0        0        0     2729 2023-04-19 20:33:33.000000 pyjls-0.6.0/include/jls/backend.h
+-rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/cmacro.h
+-rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/crc32c.h
+-rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/ec.h
+-rw-rw-rw-   0        0        0    24468 2023-04-26 11:42:25.000000 pyjls-0.6.0/include/jls/format.h
+-rw-rw-rw-   0        0        0    11561 2023-04-26 14:23:01.000000 pyjls-0.6.0/include/jls/log.h
+-rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/raw.h
+-rw-rw-rw-   0        0        0    10319 2023-04-26 17:43:17.000000 pyjls-0.6.0/include/jls/reader.h
+-rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/statistics.h
+-rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/threaded_writer.h
+-rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.6.0/include/jls/time.h
+-rw-rw-rw-   0        0        0     2760 2023-04-26 19:51:39.000000 pyjls-0.6.0/include/jls/version.h
+-rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls/writer.h
+-rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.6.0/include/jls.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.141663 pyjls-0.6.0/include_prv/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.155690 pyjls-0.6.0/include_prv/jls/
+-rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.6.0/include_prv/jls/bit_shift.h
+-rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/cdef.h
+-rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.6.0/include_prv/jls/datatype.h
+-rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/msg_ring_buffer.h
+-rw-rw-rw-   0        0        0     1784 2023-04-26 18:12:34.000000 pyjls-0.6.0/include_prv/jls/rd_fsr.h
+-rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/util.h
+-rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/wr_fsr.h
+-rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/wr_prv.h
+-rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.6.0/include_prv/jls/wr_ts.h
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.158690 pyjls-0.6.0/pyjls/
+-rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.6.0/pyjls/__init__.py
+-rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/__main__.py
+-rw-rw-rw-   0        0        0  1587118 2023-04-26 19:59:45.000000 pyjls-0.6.0/pyjls/binding.c
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.168206 pyjls-0.6.0/pyjls/entry_points/
+-rw-rw-rw-   0        0        0      853 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/entry_points/annotate.py
+-rw-rw-rw-   0        0        0     1621 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/entry_points/info.py
+-rw-rw-rw-   0        0        0     2206 2023-04-26 14:31:44.000000 pyjls-0.6.0/pyjls/structs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.169206 pyjls-0.6.0/pyjls/test/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/test/__init__.py
+-rw-rw-rw-   0        0        0    10313 2023-04-26 19:18:13.000000 pyjls-0.6.0/pyjls/test/test_binding.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.169206 pyjls-0.6.0/pyjls/v1/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.0/pyjls/v1/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-04-26 19:51:39.000000 pyjls-0.6.0/pyjls/version.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.167208 pyjls-0.6.0/pyjls.egg-info/
+-rw-rw-rw-   0        0        0    14665 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1310 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-26 20:14:11.000000 pyjls-0.6.0/pyjls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 20:14:11.177720 pyjls-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     6960 2023-04-26 19:16:46.000000 pyjls-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:14:11.176720 pyjls-0.6.0/src/
+-rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.6.0/src/backend_posix.c
+-rw-rw-rw-   0        0        0     9046 2023-04-19 20:31:50.000000 pyjls-0.6.0/src/backend_win.c
+-rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.6.0/src/bit_shift.c
+-rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/crc32c_arm_neon.c
+-rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/crc32c_intel_sse4.c
+-rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/crc32c_sw.c
+-rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.6.0/src/datatype.c
+-rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/ec.c
+-rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.6.0/src/log.c
+-rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.6.0/src/msg_ring_buffer.c
+-rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.6.0/src/raw.c
+-rw-rw-rw-   0        0        0     5903 2023-04-26 19:35:45.000000 pyjls-0.6.0/src/rd_fsr.c
+-rw-rw-rw-   0        0        0    54236 2023-04-26 19:37:31.000000 pyjls-0.6.0/src/reader.c
+-rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/statistics.c
+-rw-rw-rw-   0        0        0    11268 2022-03-05 19:14:45.000000 pyjls-0.6.0/src/threaded_writer.c
+-rw-rw-rw-   0        0        0    22039 2023-04-26 14:52:04.000000 pyjls-0.6.0/src/wr_fsr.c
+-rw-rw-rw-   0        0        0     9691 2023-04-26 14:57:54.000000 pyjls-0.6.0/src/wr_ts.c
+-rw-rw-rw-   0        0        0    30342 2023-04-26 12:23:06.000000 pyjls-0.6.0/src/writer.c
```

### Comparing `pyjls-0.5.3/CHANGELOG.md` & `pyjls-0.6.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the JLS project.
 
 
+## 0.6.0
+
+2023 Apr 26
+
+* Fixed JLS to handle non-zero sample_id for first FSR data sample.
+* Added pyjls.Reader.timestamp_to_sample_id and sample_id_to_timestamp.
+
+
 ## 0.5.3
 
 2023 Apr 19
 
 * Fixed build warnings for fn() declarations.
```

### Comparing `pyjls-0.5.3/CREDITS.html` & `pyjls-0.6.0/CREDITS.html`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/LICENSE` & `pyjls-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/PKG-INFO` & `pyjls-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.5.3
+Version: 0.6.0
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.5.3/README.md` & `pyjls-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/backend.h` & `pyjls-0.6.0/include/jls/backend.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/cmacro.h` & `pyjls-0.6.0/include/jls/cmacro.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/crc32c.h` & `pyjls-0.6.0/include/jls/crc32c.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/ec.h` & `pyjls-0.6.0/include/jls/ec.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/format.h` & `pyjls-0.6.0/include/jls/format.h`

 * *Files 1% similar despite different names*

```diff
@@ -400,14 +400,15 @@
     uint32_t sample_rate;               // 0 for VSR
     uint32_t samples_per_data;          // suggestion, will be rounded
     uint32_t sample_decimate_factor;    // definite
     uint32_t entries_per_summary;       // suggestion, will be rounded
     uint32_t summary_decimate_factor;   // definite
     uint32_t annotation_decimate_factor;
     uint32_t utc_decimate_factor;
+    int64_t sample_id_offset;           // FSR read-only, dynamically loaded from first data chunk.
     // on disk: reserve 64 bytes as 0 for future use
     const char * name;                  // The signal name
     const char * units;                 // The units string, normally as SI with no scale prefix.
 };
 
 //  struct jls_track_def_s  // empty, only need chunk_meta for now
```

### Comparing `pyjls-0.5.3/include/jls/log.h` & `pyjls-0.6.0/include/jls/log.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/raw.h` & `pyjls-0.6.0/include/jls/raw.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/reader.h` & `pyjls-0.6.0/include/jls/reader.h`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,17 @@
  */
 JLS_API int32_t jls_rd_fsr_length(struct jls_rd_s * self, uint16_t signal_id, int64_t * samples);
 
 /**
  * @brief Read fixed sample rate (FSR) data.
  *
  * @param self The reader instance.
- * @param signal_id The signal id.
+ * @param signal_id The signal id.  The first
+ *      recorded sample is always 0.  To get the first recorded sample_id,
+ *      see jls_signal_def_s.sample_id_offset.
  * @param start_sample_id The starting sample id to read.
  * @param[out] data The samples read.
  * @param data_length The number of samples to read.
  *      data is at least this many samples.
  *      For data types less than 8 bits long, you need to provide an
  *      extra byte to allow for data shifting.  Therefore
  *      data is at least 1 + (data_length * entry_size_bits) / 8 bytes.
@@ -116,30 +118,34 @@
 JLS_API int32_t jls_rd_fsr(struct jls_rd_s * self, uint16_t signal_id, int64_t start_sample_id,
                            void * data, int64_t data_length);
 
 /**
  * @brief Read fixed sample rate (FSR) float32 data.
  *
  * @param self The reader instance.
- * @param signal_id The signal id.
+ * @param signal_id The signal id.  The first
+ *      recorded sample is always 0.  To get the first recorded sample_id,
+ *      see jls_signal_def_s.sample_id_offset.
  * @param start_sample_id The starting sample id to read.
  * @param[out] data The samples read.
  * @param data_length The number of samples to read.  data is
  *      also at least this many entries (4 * data_length bytes).
  * @return 0 or error code
  */
 JLS_API int32_t jls_rd_fsr_f32(struct jls_rd_s * self, uint16_t signal_id, int64_t start_sample_id,
                                float * data, int64_t data_length);
 
 /**
  * @brief Read the statistics data for a fixed sampling rate signal.
  *
  * @param self The reader instance.
  * @param signal_id The FSR signal.
- * @param start_sample_id The starting sample id to read.
+ * @param start_sample_id The starting sample id to read.  The first
+ *      recorded sample is always 0.  To get the first recorded sample_id,
+ *      see jls_signal_def_s.sample_id_offset.
  * @param increment The number of samples that form a single output summary.
  * @param[out] data The statistics information, in the shape of
  *      data[data_length][JLS_SUMMARY_FSR_COUNT].  The elements are
  *      mean, standard_deviation, min, max.
  *      Use JLS_SUMMARY_FSR_MEAN, JLS_SUMMARY_FSR_STD,
  *      JLS_SUMMARY_FSR_MIN, and JLS_SUMMARY_FSR_MAX to index the values.
  * @param data_length The number of statistics points to populate.  data
@@ -236,12 +242,36 @@
  *      to the next UTC entries or a non-zero value to stop iteration.
  * @param cbk_user_data The arbitrary data provided to cbk_fn.
  * @return 0 or error code.
  */
 JLS_API int32_t jls_rd_utc(struct jls_rd_s * self, uint16_t signal_id, int64_t sample_id,
                            jls_rd_utc_cbk_fn cbk_fn, void * cbk_user_data);
 
+/**
+ * @brief Convert from sample_id to timestamp for FSR signals.
+ *
+ * @param self The reader instance.
+ * @param signal_id The signal id.
+ * @param sample_id The sample id to convert.
+ * @param timestamp[out] The JLS timestamp for the sample_id.
+ * @return 0 or error code.
+ */
+JLS_API int32_t jls_rd_sample_id_to_timestamp(struct jls_rd_s * self, uint16_t signal_id,
+        int64_t sample_id, int64_t * timestamp);
+
+/**
+ * @brief Convert from timestamp to sample_id for FSR signals.
+ *
+ * @param self The reader instance.
+ * @param signal_id The signal id.
+ * @param timestamp The JLS timestamp to convert.
+ * @param sample_id[out] The sample_id for timestamp.
+ * @return 0 or error code.
+ */
+JLS_API int32_t jls_rd_timestamp_to_sample_id(struct jls_rd_s * self, uint16_t signal_id,
+        int64_t timestamp, int64_t * sample_id);
+
 JLS_CPP_GUARD_END
 
 /** @} */
 
 #endif  /* JLS_READER_H__ */
```

### Comparing `pyjls-0.5.3/include/jls/statistics.h` & `pyjls-0.6.0/include/jls/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/threaded_writer.h` & `pyjls-0.6.0/include/jls/threaded_writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/time.h` & `pyjls-0.6.0/include/jls/time.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls/version.h` & `pyjls-0.6.0/include/jls/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
  * @{
  */
 
 JLS_CPP_GUARD_START
 
 // Use version_update.py to update.
 #define JLS_VERSION_MAJOR 0
-#define JLS_VERSION_MINOR 5
-#define JLS_VERSION_PATCH 3
+#define JLS_VERSION_MINOR 6
+#define JLS_VERSION_PATCH 0
 
 /**
  * \brief Macro to encode version to uint32_t.
  *
  * \param major The major release number (0 to 255)
  * \param minor The minor release number (0 to 255)
  * \param patch The patch release number (0 to 65535)
```

### Comparing `pyjls-0.5.3/include/jls/writer.h` & `pyjls-0.6.0/include/jls/writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include/jls.h` & `pyjls-0.6.0/include/jls.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/bit_shift.h` & `pyjls-0.6.0/include_prv/jls/bit_shift.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/cdef.h` & `pyjls-0.6.0/include_prv/jls/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/datatype.h` & `pyjls-0.6.0/include_prv/jls/datatype.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/msg_ring_buffer.h` & `pyjls-0.6.0/include_prv/jls/msg_ring_buffer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/util.h` & `pyjls-0.6.0/include_prv/jls/util.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/wr_fsr.h` & `pyjls-0.6.0/include_prv/jls/wr_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/wr_prv.h` & `pyjls-0.6.0/include_prv/jls/wr_prv.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/include_prv/jls/wr_ts.h` & `pyjls-0.6.0/include_prv/jls/wr_ts.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/__init__.py` & `pyjls-0.6.0/pyjls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/__main__.py` & `pyjls-0.6.0/pyjls/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/binding.c` & `pyjls-0.6.0/pyjls/binding.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
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
+            "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
         ],
         "include_dirs": [
             "include",
             "include_prv",
-            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include"
+            "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "pyjls.binding",
         "sources": [
             "pyjls/binding.pyx",
             "src/bit_shift.c",
             "src/datatype.c",
             "src/ec.c",
             "src/log.c",
             "src/msg_ring_buffer.c",
             "src/raw.c",
+            "src/rd_fsr.c",
             "src/reader.c",
             "src/statistics.c",
             "src/threaded_writer.c",
             "src/wr_fsr.c",
             "src/wr_ts.c",
             "src/writer.c",
             "src/backend_win.c",
@@ -1138,195 +1139,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":717
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":724
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1360,79 +1361,79 @@
 struct __pyx_obj_5pyjls_7binding_AnnotationCallback;
 struct __pyx_obj_5pyjls_7binding_Reader;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":728
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":732
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "pyjls/binding.pyx":251
+/* "pyjls/binding.pyx":252
  * 
  * 
  * cdef class Writer:             # <<<<<<<<<<<<<<
  *     cdef c_jls.jls_twr_s * _wr
  *     cdef c_jls.jls_signal_def_s _signals[_JLS_SIGNAL_COUNT]
  */
 struct __pyx_obj_5pyjls_7binding_Writer {
   PyObject_HEAD
   struct jls_twr_s *_wr;
   struct jls_signal_def_s _signals[0x100];
 };
 
 
-/* "pyjls/binding.pyx":390
+/* "pyjls/binding.pyx":391
  * 
  * 
  * cdef class AnnotationCallback:             # <<<<<<<<<<<<<<
  *     cdef uint8_t is_fsr
  *     cdef object cbk_fn
  */
 struct __pyx_obj_5pyjls_7binding_AnnotationCallback {
   PyObject_HEAD
   uint8_t is_fsr;
   PyObject *cbk_fn;
 };
 
 
-/* "pyjls/binding.pyx":399
+/* "pyjls/binding.pyx":400
  * 
  * 
  * cdef class Reader:             # <<<<<<<<<<<<<<
  *     cdef c_jls.jls_rd_s * _rd
  *     cdef object _sources
  */
 struct __pyx_obj_5pyjls_7binding_Reader {
@@ -1881,22 +1882,14 @@
 #endif
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_TrueDivideObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_TrueDivideObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceTrueDivide(op1, op2) : PyNumber_TrueDivide(op1, op2))
-#endif
-
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
 /* PyObjectFormatSimple.proto */
 #if CYTHON_COMPILING_IN_PYPY
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
@@ -2734,14 +2727,15 @@
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_strip[] = "strip";
 static const char __pyx_k_uint8[] = "uint8";
 static const char __pyx_k_units[] = "units";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_Reader[] = "Reader";
+static const char __pyx_k_SECOND[] = "SECOND";
 static const char __pyx_k_Writer[] = "Writer";
 static const char __pyx_k_cbk_fn[] = "cbk_fn";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_handle[] = "handle";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_is_fsr[] = "is_fsr";
@@ -2844,28 +2838,30 @@
 static const char __pyx_k_data_type_map[] = "_data_type_map";
 static const char __pyx_k_log_level_map[] = "_log_level_map";
 static const char __pyx_k_pyjls_binding[] = "pyjls.binding";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_rd_fsr_length[] = "rd_fsr_length";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_serial_number[] = "serial_number";
+static const char __pyx_k_utc_timestamp[] = "utc_timestamp";
 static const char __pyx_k_AnnotationType[] = "AnnotationType";
 static const char __pyx_k_annotation_map[] = "_annotation_map";
 static const char __pyx_k_jls_inject_log[] = "jls_inject_log";
 static const char __pyx_k_rd_annotations[] = "rd_annotations";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_annotation_type[] = "annotation_type";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_start_sample_id[] = "start_sample_id";
 static const char __pyx_k_vertical_marker[] = "vertical_marker";
 static const char __pyx_k_data_type_as_str[] = "_data_type_as_str";
+static const char __pyx_k_sample_id_offset[] = "sample_id_offset";
 static const char __pyx_k_samples_per_data[] = "samples_per_data";
 static const char __pyx_k_data_type_as_enum[] = "_data_type_as_enum";
 static const char __pyx_k_horizontal_marker[] = "horizontal_marker";
 static const char __pyx_k_pyjls_binding_pyx[] = "pyjls\\binding.pyx";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_rd_fsr_statistics[] = "rd_fsr_statistics";
 static const char __pyx_k_AnnotationCallback[] = "AnnotationCallback";
@@ -2878,14 +2874,16 @@
 static const char __pyx_k_entries_per_summary[] = "entries_per_summary";
 static const char __pyx_k_utc_decimate_factor[] = "utc_decimate_factor";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_in_annotation_callback[] = "in annotation callback";
 static const char __pyx_k_sample_decimate_factor[] = "sample_decimate_factor";
+static const char __pyx_k_sample_id_to_timestamp[] = "sample_id_to_timestamp";
+static const char __pyx_k_timestamp_to_sample_id[] = "timestamp_to_sample_id";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_summary_decimate_factor[] = "summary_decimate_factor";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_annotation_decimate_factor[] = "annotation_decimate_factor";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
@@ -2966,14 +2964,15 @@
 static PyObject *__pyx_n_u_N;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_Reader;
 static PyObject *__pyx_n_u_Reader;
 static PyObject *__pyx_n_s_RuntimeError;
+static PyObject *__pyx_n_s_SECOND;
 static PyObject *__pyx_n_s_STD;
 static PyObject *__pyx_n_s_SignalDef;
 static PyObject *__pyx_n_u_SignalDef;
 static PyObject *__pyx_n_s_SignalType;
 static PyObject *__pyx_n_u_SignalType;
 static PyObject *__pyx_n_s_SourceDef;
 static PyObject *__pyx_n_u_SourceDef;
@@ -3153,14 +3152,16 @@
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_kp_b_s;
 static PyObject *__pyx_n_s_s_2;
 static PyObject *__pyx_n_s_sample_decimate_factor;
 static PyObject *__pyx_n_s_sample_id;
+static PyObject *__pyx_n_s_sample_id_offset;
+static PyObject *__pyx_n_u_sample_id_to_timestamp;
 static PyObject *__pyx_n_s_sample_rate;
 static PyObject *__pyx_n_s_samples_per_data;
 static PyObject *__pyx_kp_s_self__rd_cannot_be_converted_to;
 static PyObject *__pyx_kp_s_self__wr_cannot_be_converted_to;
 static PyObject *__pyx_n_s_serial_number;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
@@ -3189,14 +3190,15 @@
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_structs;
 static PyObject *__pyx_n_s_summary_decimate_factor;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_u_text;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_timestamp;
+static PyObject *__pyx_n_u_timestamp_to_sample_id;
 static PyObject *__pyx_n_s_traceback;
 static PyObject *__pyx_n_u_txt;
 static PyObject *__pyx_n_s_type;
 static PyObject *__pyx_n_u_u1;
 static PyObject *__pyx_n_u_u16;
 static PyObject *__pyx_n_u_u32;
 static PyObject *__pyx_n_u_u4;
@@ -3214,14 +3216,15 @@
 static PyObject *__pyx_n_u_user;
 static PyObject *__pyx_n_u_user_data;
 static PyObject *__pyx_n_u_usr;
 static PyObject *__pyx_n_s_utc;
 static PyObject *__pyx_n_u_utc;
 static PyObject *__pyx_n_s_utc_decimate_factor;
 static PyObject *__pyx_n_s_utc_i64;
+static PyObject *__pyx_n_s_utc_timestamp;
 static PyObject *__pyx_n_s_utc_to_jls;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_vendor;
 static PyObject *__pyx_n_s_version;
 static PyObject *__pyx_n_u_vertical_marker;
 static PyObject *__pyx_n_s_view;
@@ -3263,16 +3266,18 @@
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_7sources___get__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_7signals___get__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_8fsr(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_start_sample_id, PyObject *__pyx_v_length); /* proto */
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_10fsr_statistics(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_start_sample_id, PyObject *__pyx_v_increment, PyObject *__pyx_v_length); /* proto */
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_12annotations(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_timestamp, PyObject *__pyx_v_cbk_fn); /* proto */
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_14user_data(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_cbk_fn); /* proto */
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_16utc(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_sample_id, PyObject *__pyx_v_cbk_fn); /* proto */
-static PyObject *__pyx_pf_5pyjls_7binding_6Reader_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5pyjls_7binding_6Reader_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_18sample_id_to_timestamp(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_sample_id); /* proto */
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_20timestamp_to_sample_id(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_utc_timestamp); /* proto */
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_22__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_24__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_5pyjls_7binding_20__pyx_unpickle_AnnotationCallback(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
@@ -3394,15 +3399,15 @@
 static PyObject *__pyx_codeobj__50;
 static PyObject *__pyx_codeobj__52;
 static PyObject *__pyx_codeobj__54;
 static PyObject *__pyx_codeobj__56;
 static PyObject *__pyx_codeobj__63;
 /* Late includes */
 
-/* "pyjls/binding.pyx":49
+/* "pyjls/binding.pyx":50
  * 
  * 
  * def _data_type_def(basetype, size, q):             # <<<<<<<<<<<<<<
  *     return (basetype & 0x0f) | ((size & 0xff) << 8) | ((q & 0xff) << 16)
  * 
  */
 
@@ -3440,40 +3445,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_basetype)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_data_type_def", 1, 3, 3, 1); __PYX_ERR(0, 49, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_data_type_def", 1, 3, 3, 1); __PYX_ERR(0, 50, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_data_type_def", 1, 3, 3, 2); __PYX_ERR(0, 49, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_data_type_def", 1, 3, 3, 2); __PYX_ERR(0, 50, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_data_type_def") < 0)) __PYX_ERR(0, 49, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_data_type_def") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_basetype = values[0];
     __pyx_v_size = values[1];
     __pyx_v_q = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_data_type_def", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 49, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_data_type_def", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 50, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding._data_type_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding__data_type_def(__pyx_self, __pyx_v_basetype, __pyx_v_size, __pyx_v_q);
 
@@ -3489,47 +3494,47 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_data_type_def", 0);
 
-  /* "pyjls/binding.pyx":50
+  /* "pyjls/binding.pyx":51
  * 
  * def _data_type_def(basetype, size, q):
  *     return (basetype & 0x0f) | ((size & 0xff) << 8) | ((q & 0xff) << 16)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_AndObjC(__pyx_v_basetype, __pyx_int_15, 0x0f, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_AndObjC(__pyx_v_basetype, __pyx_int_15, 0x0f, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_AndObjC(__pyx_v_size, __pyx_int_255, 0xff, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_AndObjC(__pyx_v_size, __pyx_int_255, 0xff, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_LshiftObjC(__pyx_t_2, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_LshiftObjC(__pyx_t_2, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Or(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Or(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_AndObjC(__pyx_v_q, __pyx_int_255, 0xff, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_AndObjC(__pyx_v_q, __pyx_int_255, 0xff, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyInt_LshiftObjC(__pyx_t_3, __pyx_int_16, 16, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_LshiftObjC(__pyx_t_3, __pyx_int_16, 16, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Or(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Or(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":49
+  /* "pyjls/binding.pyx":50
  * 
  * 
  * def _data_type_def(basetype, size, q):             # <<<<<<<<<<<<<<
  *     return (basetype & 0x0f) | ((size & 0xff) << 8) | ((q & 0xff) << 16)
  * 
  */
 
@@ -3542,15 +3547,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":119
+/* "pyjls/binding.pyx":120
  * 
  * 
  * def _populate_data_type():             # <<<<<<<<<<<<<<
  *     for key, value in list(_data_type_as_enum.items()):
  *         _data_type_as_enum[value] = value
  */
 
@@ -3581,152 +3586,152 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_populate_data_type", 0);
 
-  /* "pyjls/binding.pyx":120
+  /* "pyjls/binding.pyx":121
  * 
  * def _populate_data_type():
  *     for key, value in list(_data_type_as_enum.items()):             # <<<<<<<<<<<<<<
  *         _data_type_as_enum[value] = value
  *         _data_type_as_str[value] = key
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_3 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_t_3; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 121, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 120, __pyx_L1_error)
+        __PYX_ERR(0, 121, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       #else
-      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 120, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 120, __pyx_L1_error)
+      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext;
       index = 0; __pyx_t_2 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_2)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
       index = 1; __pyx_t_5 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_5)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
       __pyx_t_7 = NULL;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 120, __pyx_L1_error)
+      __PYX_ERR(0, 121, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":121
+    /* "pyjls/binding.pyx":122
  * def _populate_data_type():
  *     for key, value in list(_data_type_as_enum.items()):
  *         _data_type_as_enum[value] = value             # <<<<<<<<<<<<<<
  *         _data_type_as_str[value] = key
  *         _data_type_as_str[key] = key
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_v_value, __pyx_v_value) < 0)) __PYX_ERR(0, 121, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_v_value, __pyx_v_value) < 0)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pyjls/binding.pyx":122
+    /* "pyjls/binding.pyx":123
  *     for key, value in list(_data_type_as_enum.items()):
  *         _data_type_as_enum[value] = value
  *         _data_type_as_str[value] = key             # <<<<<<<<<<<<<<
  *         _data_type_as_str[key] = key
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_as_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_as_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_v_value, __pyx_v_key) < 0)) __PYX_ERR(0, 122, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_v_value, __pyx_v_key) < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pyjls/binding.pyx":123
+    /* "pyjls/binding.pyx":124
  *         _data_type_as_enum[value] = value
  *         _data_type_as_str[value] = key
  *         _data_type_as_str[key] = key             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_as_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_as_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_v_key, __pyx_v_key) < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_v_key, __pyx_v_key) < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pyjls/binding.pyx":120
+    /* "pyjls/binding.pyx":121
  * 
  * def _populate_data_type():
  *     for key, value in list(_data_type_as_enum.items()):             # <<<<<<<<<<<<<<
  *         _data_type_as_enum[value] = value
  *         _data_type_as_str[value] = key
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":119
+  /* "pyjls/binding.pyx":120
  * 
  * 
  * def _populate_data_type():             # <<<<<<<<<<<<<<
  *     for key, value in list(_data_type_as_enum.items()):
  *         _data_type_as_enum[value] = value
  */
 
@@ -3745,15 +3750,15 @@
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":129
+/* "pyjls/binding.pyx":130
  * 
  * 
  * def data_type_as_enum(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_enum[data_type]
  * 
  */
 
@@ -3777,32 +3782,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("data_type_as_enum", 0);
 
-  /* "pyjls/binding.pyx":130
+  /* "pyjls/binding.pyx":131
  * 
  * def data_type_as_enum(data_type):
  *     return _data_type_as_enum[data_type]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":129
+  /* "pyjls/binding.pyx":130
  * 
  * 
  * def data_type_as_enum(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_enum[data_type]
  * 
  */
 
@@ -3814,15 +3819,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":133
+/* "pyjls/binding.pyx":134
  * 
  * 
  * def data_type_as_str(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_str[data_type]
  * 
  */
 
@@ -3846,32 +3851,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("data_type_as_str", 0);
 
-  /* "pyjls/binding.pyx":134
+  /* "pyjls/binding.pyx":135
  * 
  * def data_type_as_str(data_type):
  *     return _data_type_as_str[data_type]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_data_type_as_str); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_data_type_as_str); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":133
+  /* "pyjls/binding.pyx":134
  * 
  * 
  * def data_type_as_str(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_str[data_type]
  * 
  */
 
@@ -3883,15 +3888,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":185
+/* "pyjls/binding.pyx":186
  * 
  * 
  * cdef void _log_cbk(const char * msg) nogil:             # <<<<<<<<<<<<<<
  *     with gil:
  *         m = msg.decode('utf-8').strip()
  */
 
@@ -3918,77 +3923,77 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_RefNannySetupContext("_log_cbk", 1);
 
-  /* "pyjls/binding.pyx":186
+  /* "pyjls/binding.pyx":187
  * 
  * cdef void _log_cbk(const char * msg) nogil:
  *     with gil:             # <<<<<<<<<<<<<<
  *         m = msg.decode('utf-8').strip()
  *         level, location, s = m.split(' ', 2)
  */
   /*try:*/ {
     {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         /*try:*/ {
 
-          /* "pyjls/binding.pyx":187
+          /* "pyjls/binding.pyx":188
  * cdef void _log_cbk(const char * msg) nogil:
  *     with gil:
  *         m = msg.decode('utf-8').strip()             # <<<<<<<<<<<<<<
  *         level, location, s = m.split(' ', 2)
  *         lvl = _log_level_map.get(level, logging.DEBUG)
  */
-          __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_t_2 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
             __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
             if (likely(__pyx_t_2)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
               __Pyx_INCREF(__pyx_t_2);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_3, function);
             }
           }
           __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L7_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __pyx_v_m = __pyx_t_1;
           __pyx_t_1 = 0;
 
-          /* "pyjls/binding.pyx":188
+          /* "pyjls/binding.pyx":189
  *     with gil:
  *         m = msg.decode('utf-8').strip()
  *         level, location, s = m.split(' ', 2)             # <<<<<<<<<<<<<<
  *         lvl = _log_level_map.get(level, logging.DEBUG)
  *         filename, line, _ = location.split(':')
  */
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_m, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L7_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_m, __pyx_n_s_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
             PyObject* sequence = __pyx_t_3;
             Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
             if (unlikely(size != 3)) {
               if (size > 3) __Pyx_RaiseTooManyValuesError(3);
               else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-              __PYX_ERR(0, 188, __pyx_L7_error)
+              __PYX_ERR(0, 189, __pyx_L7_error)
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             if (likely(PyTuple_CheckExact(sequence))) {
               __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
               __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
               __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
             } else {
@@ -3996,67 +4001,67 @@
               __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
               __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
             }
             __Pyx_INCREF(__pyx_t_1);
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_4);
             #else
-            __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L7_error)
+            __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L7_error)
+            __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L7_error)
+            __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_4);
             #endif
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           } else {
             Py_ssize_t index = -1;
-            __pyx_t_5 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L7_error)
+            __pyx_t_5 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext;
             index = 0; __pyx_t_1 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_1)) goto __pyx_L9_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_1);
             index = 1; __pyx_t_2 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L9_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_2);
             index = 2; __pyx_t_4 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L9_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_4);
-            if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 188, __pyx_L7_error)
+            if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 189, __pyx_L7_error)
             __pyx_t_6 = NULL;
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             goto __pyx_L10_unpacking_done;
             __pyx_L9_unpacking_failed:;
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             __pyx_t_6 = NULL;
             if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-            __PYX_ERR(0, 188, __pyx_L7_error)
+            __PYX_ERR(0, 189, __pyx_L7_error)
             __pyx_L10_unpacking_done:;
           }
           __pyx_v_level = __pyx_t_1;
           __pyx_t_1 = 0;
           __pyx_v_location = __pyx_t_2;
           __pyx_t_2 = 0;
           __pyx_v_s = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "pyjls/binding.pyx":189
+          /* "pyjls/binding.pyx":190
  *         m = msg.decode('utf-8').strip()
  *         level, location, s = m.split(' ', 2)
  *         lvl = _log_level_map.get(level, logging.DEBUG)             # <<<<<<<<<<<<<<
  *         filename, line, _ = location.split(':')
  *         record = logging.LogRecord(_log_c_name, lvl, filename, int(line), s, None, None)
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_log_level_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_log_level_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logging); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logging); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L7_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __pyx_t_4 = NULL;
           __pyx_t_7 = 0;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
             __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
             if (likely(__pyx_t_4)) {
@@ -4066,80 +4071,80 @@
               __Pyx_DECREF_SET(__pyx_t_2, function);
               __pyx_t_7 = 1;
             }
           }
           #if CYTHON_FAST_PYCALL
           if (PyFunction_Check(__pyx_t_2)) {
             PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_level, __pyx_t_1};
-            __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L7_error)
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           } else
           #endif
           #if CYTHON_FAST_PYCCALL
           if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
             PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_level, __pyx_t_1};
-            __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L7_error)
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           } else
           #endif
           {
-            __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L7_error)
+            __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_5);
             if (__pyx_t_4) {
               __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
             }
             __Pyx_INCREF(__pyx_v_level);
             __Pyx_GIVEREF(__pyx_v_level);
             PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_v_level);
             __Pyx_GIVEREF(__pyx_t_1);
             PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_1);
             __pyx_t_1 = 0;
-            __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_v_lvl = __pyx_t_3;
           __pyx_t_3 = 0;
 
-          /* "pyjls/binding.pyx":190
+          /* "pyjls/binding.pyx":191
  *         level, location, s = m.split(' ', 2)
  *         lvl = _log_level_map.get(level, logging.DEBUG)
  *         filename, line, _ = location.split(':')             # <<<<<<<<<<<<<<
  *         record = logging.LogRecord(_log_c_name, lvl, filename, int(line), s, None, None)
  *         _log_c.handle(record)
  */
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_location, __pyx_n_s_split); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_location, __pyx_n_s_split); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_5 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
             __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
             if (likely(__pyx_t_5)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
               __Pyx_INCREF(__pyx_t_5);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_2, function);
             }
           }
           __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_kp_u__3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u__3);
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L7_error)
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
             PyObject* sequence = __pyx_t_3;
             Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
             if (unlikely(size != 3)) {
               if (size > 3) __Pyx_RaiseTooManyValuesError(3);
               else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-              __PYX_ERR(0, 190, __pyx_L7_error)
+              __PYX_ERR(0, 191, __pyx_L7_error)
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             if (likely(PyTuple_CheckExact(sequence))) {
               __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
               __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
               __pyx_t_1 = PyTuple_GET_ITEM(sequence, 2); 
             } else {
@@ -4147,67 +4152,67 @@
               __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
               __pyx_t_1 = PyList_GET_ITEM(sequence, 2); 
             }
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_5);
             __Pyx_INCREF(__pyx_t_1);
             #else
-            __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L7_error)
+            __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L7_error)
+            __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_5);
-            __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L7_error)
+            __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_1);
             #endif
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           } else {
             Py_ssize_t index = -1;
-            __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L7_error)
+            __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext;
             index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L11_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_2);
             index = 1; __pyx_t_5 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_5)) goto __pyx_L11_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_5);
             index = 2; __pyx_t_1 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_1)) goto __pyx_L11_unpacking_failed;
             __Pyx_GOTREF(__pyx_t_1);
-            if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 3) < 0) __PYX_ERR(0, 190, __pyx_L7_error)
+            if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 3) < 0) __PYX_ERR(0, 191, __pyx_L7_error)
             __pyx_t_6 = NULL;
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             goto __pyx_L12_unpacking_done;
             __pyx_L11_unpacking_failed:;
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             __pyx_t_6 = NULL;
             if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-            __PYX_ERR(0, 190, __pyx_L7_error)
+            __PYX_ERR(0, 191, __pyx_L7_error)
             __pyx_L12_unpacking_done:;
           }
           __pyx_v_filename = __pyx_t_2;
           __pyx_t_2 = 0;
           __pyx_v_line = __pyx_t_5;
           __pyx_t_5 = 0;
           __pyx_v__ = __pyx_t_1;
           __pyx_t_1 = 0;
 
-          /* "pyjls/binding.pyx":191
+          /* "pyjls/binding.pyx":192
  *         lvl = _log_level_map.get(level, logging.DEBUG)
  *         filename, line, _ = location.split(':')
  *         record = logging.LogRecord(_log_c_name, lvl, filename, int(line), s, None, None)             # <<<<<<<<<<<<<<
  *         _log_c.handle(record)
  * 
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_LogRecord); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L7_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_LogRecord); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_c_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_c_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_v_line); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_v_line); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_4 = NULL;
           __pyx_t_7 = 0;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
             __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
             if (likely(__pyx_t_4)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -4216,33 +4221,33 @@
               __Pyx_DECREF_SET(__pyx_t_5, function);
               __pyx_t_7 = 1;
             }
           }
           #if CYTHON_FAST_PYCALL
           if (PyFunction_Check(__pyx_t_5)) {
             PyObject *__pyx_temp[8] = {__pyx_t_4, __pyx_t_1, __pyx_v_lvl, __pyx_v_filename, __pyx_t_2, __pyx_v_s, Py_None, Py_None};
-            __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 7+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 7+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L7_error)
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           } else
           #endif
           #if CYTHON_FAST_PYCCALL
           if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
             PyObject *__pyx_temp[8] = {__pyx_t_4, __pyx_t_1, __pyx_v_lvl, __pyx_v_filename, __pyx_t_2, __pyx_v_s, Py_None, Py_None};
-            __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 7+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 7+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L7_error)
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           } else
           #endif
           {
-            __pyx_t_8 = PyTuple_New(7+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 191, __pyx_L7_error)
+            __pyx_t_8 = PyTuple_New(7+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 192, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_8);
             if (__pyx_t_4) {
               __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4); __pyx_t_4 = NULL;
             }
             __Pyx_GIVEREF(__pyx_t_1);
             PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
             __Pyx_INCREF(__pyx_v_lvl);
@@ -4260,53 +4265,53 @@
             __Pyx_GIVEREF(Py_None);
             PyTuple_SET_ITEM(__pyx_t_8, 5+__pyx_t_7, Py_None);
             __Pyx_INCREF(Py_None);
             __Pyx_GIVEREF(Py_None);
             PyTuple_SET_ITEM(__pyx_t_8, 6+__pyx_t_7, Py_None);
             __pyx_t_1 = 0;
             __pyx_t_2 = 0;
-            __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
           }
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __pyx_v_record = __pyx_t_3;
           __pyx_t_3 = 0;
 
-          /* "pyjls/binding.pyx":192
+          /* "pyjls/binding.pyx":193
  *         filename, line, _ = location.split(':')
  *         record = logging.LogRecord(_log_c_name, lvl, filename, int(line), s, None, None)
  *         _log_c.handle(record)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_log_c); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_log_c); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_handle); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 192, __pyx_L7_error)
+          __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_handle); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 193, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __pyx_t_5 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
             __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
             if (likely(__pyx_t_5)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
               __Pyx_INCREF(__pyx_t_5);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_8, function);
             }
           }
           __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_5, __pyx_v_record) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_record);
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L7_error)
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
 
-        /* "pyjls/binding.pyx":186
+        /* "pyjls/binding.pyx":187
  * 
  * cdef void _log_cbk(const char * msg) nogil:
  *     with gil:             # <<<<<<<<<<<<<<
  *         m = msg.decode('utf-8').strip()
  *         level, location, s = m.split(' ', 2)
  */
         /*finally:*/ {
@@ -4338,15 +4343,15 @@
       __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       goto __pyx_L1_error;
     }
     __pyx_L5:;
   }
 
-  /* "pyjls/binding.pyx":185
+  /* "pyjls/binding.pyx":186
  * 
  * 
  * cdef void _log_cbk(const char * msg) nogil:             # <<<<<<<<<<<<<<
  *     with gil:
  *         m = msg.decode('utf-8').strip()
  */
 
@@ -4371,15 +4376,15 @@
   __Pyx_XDECREF(__pyx_v__);
   __Pyx_XDECREF(__pyx_v_record);
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "pyjls/binding.pyx":198
+/* "pyjls/binding.pyx":199
  * 
  * 
  * def jls_inject_log(level, filename, line, msg):             # <<<<<<<<<<<<<<
  *     cdef char * c_msg
  *     location = ':'.join([filename, str(line), ''])
  */
 
@@ -4420,31 +4425,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_level)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, 1); __PYX_ERR(0, 198, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, 1); __PYX_ERR(0, 199, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_line)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, 2); __PYX_ERR(0, 198, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, 2); __PYX_ERR(0, 199, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_msg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, 3); __PYX_ERR(0, 198, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, 3); __PYX_ERR(0, 199, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "jls_inject_log") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "jls_inject_log") < 0)) __PYX_ERR(0, 199, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -4453,15 +4458,15 @@
     __pyx_v_level = values[0];
     __pyx_v_filename = values[1];
     __pyx_v_line = values[2];
     __pyx_v_msg = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 198, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("jls_inject_log", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 199, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.jls_inject_log", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_8jls_inject_log(__pyx_self, __pyx_v_level, __pyx_v_filename, __pyx_v_line, __pyx_v_msg);
 
@@ -4481,88 +4486,88 @@
   char const *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("jls_inject_log", 0);
   __Pyx_INCREF(__pyx_v_msg);
 
-  /* "pyjls/binding.pyx":200
+  /* "pyjls/binding.pyx":201
  * def jls_inject_log(level, filename, line, msg):
  *     cdef char * c_msg
  *     location = ':'.join([filename, str(line), ''])             # <<<<<<<<<<<<<<
  *     msg = ' '.join([level, location, msg]).encode('utf-8')
  *     c_msg = msg
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_line); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_line); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_filename);
   __Pyx_GIVEREF(__pyx_v_filename);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_v_filename);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __Pyx_INCREF(__pyx_kp_u__4);
   __Pyx_GIVEREF(__pyx_kp_u__4);
   PyList_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u__4);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_location = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":201
+  /* "pyjls/binding.pyx":202
  *     cdef char * c_msg
  *     location = ':'.join([filename, str(line), ''])
  *     msg = ' '.join([level, location, msg]).encode('utf-8')             # <<<<<<<<<<<<<<
  *     c_msg = msg
  *     c_jls.jls_log_printf('%s\n'.encode('utf-8'), c_msg)
  */
-  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_level);
   __Pyx_GIVEREF(__pyx_v_level);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_level);
   __Pyx_INCREF(__pyx_v_location);
   __Pyx_GIVEREF(__pyx_v_location);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_v_location);
   __Pyx_INCREF(__pyx_v_msg);
   __Pyx_GIVEREF(__pyx_v_msg);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_v_msg);
-  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u_, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u_, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_AsUTF8String(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_msg, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":202
+  /* "pyjls/binding.pyx":203
  *     location = ':'.join([filename, str(line), ''])
  *     msg = ' '.join([level, location, msg]).encode('utf-8')
  *     c_msg = msg             # <<<<<<<<<<<<<<
  *     c_jls.jls_log_printf('%s\n'.encode('utf-8'), c_msg)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_msg); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_msg); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
   __pyx_v_c_msg = __pyx_t_3;
 
-  /* "pyjls/binding.pyx":203
+  /* "pyjls/binding.pyx":204
  *     msg = ' '.join([level, location, msg]).encode('utf-8')
  *     c_msg = msg
  *     c_jls.jls_log_printf('%s\n'.encode('utf-8'), c_msg)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_kp_b_s); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_kp_b_s); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 204, __pyx_L1_error)
   jls_log_printf(__pyx_t_4, __pyx_v_c_msg);
 
-  /* "pyjls/binding.pyx":198
+  /* "pyjls/binding.pyx":199
  * 
  * 
  * def jls_inject_log(level, filename, line, msg):             # <<<<<<<<<<<<<<
  *     cdef char * c_msg
  *     location = ':'.join([filename, str(line), ''])
  */
 
@@ -4578,15 +4583,15 @@
   __Pyx_XDECREF(__pyx_v_location);
   __Pyx_XDECREF(__pyx_v_msg);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":206
+/* "pyjls/binding.pyx":207
  * 
  * 
  * def _encode_str(s):             # <<<<<<<<<<<<<<
  *     if s is None:
  *         s = ''
  */
 
@@ -4614,74 +4619,74 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_encode_str", 0);
   __Pyx_INCREF(__pyx_v_s);
 
-  /* "pyjls/binding.pyx":207
+  /* "pyjls/binding.pyx":208
  * 
  * def _encode_str(s):
  *     if s is None:             # <<<<<<<<<<<<<<
  *         s = ''
  *     return s.encode('utf-8')
  */
   __pyx_t_1 = (__pyx_v_s == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":208
+    /* "pyjls/binding.pyx":209
  * def _encode_str(s):
  *     if s is None:
  *         s = ''             # <<<<<<<<<<<<<<
  *     return s.encode('utf-8')
  * 
  */
     __Pyx_INCREF(__pyx_kp_u__4);
     __Pyx_DECREF_SET(__pyx_v_s, __pyx_kp_u__4);
 
-    /* "pyjls/binding.pyx":207
+    /* "pyjls/binding.pyx":208
  * 
  * def _encode_str(s):
  *     if s is None:             # <<<<<<<<<<<<<<
  *         s = ''
  *     return s.encode('utf-8')
  */
   }
 
-  /* "pyjls/binding.pyx":209
+  /* "pyjls/binding.pyx":210
  *     if s is None:
  *         s = ''
  *     return s.encode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 209, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":206
+  /* "pyjls/binding.pyx":207
  * 
  * 
  * def _encode_str(s):             # <<<<<<<<<<<<<<
  *     if s is None:
  *         s = ''
  */
 
@@ -4695,15 +4700,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":212
+/* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, str):
  *         s = _encode_str(data)
  */
 
@@ -4734,165 +4739,165 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_storage_pack", 0);
 
-  /* "pyjls/binding.pyx":213
+  /* "pyjls/binding.pyx":214
  * 
  * def _storage_pack(data):
  *     if isinstance(data, str):             # <<<<<<<<<<<<<<
  *         s = _encode_str(data)
  *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":214
+    /* "pyjls/binding.pyx":215
  * def _storage_pack(data):
  *     if isinstance(data, str):
  *         s = _encode_str(data)             # <<<<<<<<<<<<<<
  *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
  *     elif isinstance(data, bytes):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_s = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "pyjls/binding.pyx":215
+    /* "pyjls/binding.pyx":216
  *     if isinstance(data, str):
  *         s = _encode_str(data)
  *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1             # <<<<<<<<<<<<<<
  *     elif isinstance(data, bytes):
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 215, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_s);
     __Pyx_GIVEREF(__pyx_v_s);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_s);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":213
+    /* "pyjls/binding.pyx":214
  * 
  * def _storage_pack(data):
  *     if isinstance(data, str):             # <<<<<<<<<<<<<<
  *         s = _encode_str(data)
  *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
  */
   }
 
-  /* "pyjls/binding.pyx":216
+  /* "pyjls/binding.pyx":217
  *         s = _encode_str(data)
  *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
  *     elif isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  *     else:
  */
   __pyx_t_2 = PyBytes_Check(__pyx_v_data); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "pyjls/binding.pyx":217
+    /* "pyjls/binding.pyx":218
  *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
  *     elif isinstance(data, bytes):
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)             # <<<<<<<<<<<<<<
  *     else:
  *         s = _encode_str(json.dumps(data))
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_BINARY); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_BINARY); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 217, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_6 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_data);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":216
+    /* "pyjls/binding.pyx":217
  *         s = _encode_str(data)
  *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
  *     elif isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  *     else:
  */
   }
 
-  /* "pyjls/binding.pyx":219
+  /* "pyjls/binding.pyx":220
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  *     else:
  *         s = _encode_str(json.dumps(data))             # <<<<<<<<<<<<<<
  *         return c_jls.JLS_STORAGE_TYPE_JSON, s, len(s) + 1
  * 
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_json); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_json); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_dumps); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_dumps); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
     __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_data);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -4900,34 +4905,34 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_s = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "pyjls/binding.pyx":220
+    /* "pyjls/binding.pyx":221
  *     else:
  *         s = _encode_str(json.dumps(data))
  *         return c_jls.JLS_STORAGE_TYPE_JSON, s, len(s) + 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_JSON); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_JSON); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_s);
     __Pyx_GIVEREF(__pyx_v_s);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_s);
     __Pyx_GIVEREF(__pyx_t_4);
@@ -4935,15 +4940,15 @@
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
   }
 
-  /* "pyjls/binding.pyx":212
+  /* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, str):
  *         s = _encode_str(data)
  */
 
@@ -4959,15 +4964,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":223
+/* "pyjls/binding.pyx":224
  * 
  * 
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):             # <<<<<<<<<<<<<<
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  */
 
@@ -4980,119 +4985,119 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_storage_unpack", 0);
 
-  /* "pyjls/binding.pyx":224
+  /* "pyjls/binding.pyx":225
  * 
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):
  *     cdef const char * str = <const char *> data             # <<<<<<<<<<<<<<
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  *         return str[:data_size - 1].decode('utf-8')
  */
   __pyx_v_str = ((char const *)__pyx_v_data);
 
-  /* "pyjls/binding.pyx":225
+  /* "pyjls/binding.pyx":226
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:             # <<<<<<<<<<<<<<
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  */
   switch (__pyx_v_storage_type) {
     case JLS_STORAGE_TYPE_STRING:
 
-    /* "pyjls/binding.pyx":226
+    /* "pyjls/binding.pyx":227
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  *         return str[:data_size - 1].decode('utf-8')             # <<<<<<<<<<<<<<
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  *         return data[:data_size]
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":225
+    /* "pyjls/binding.pyx":226
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:             # <<<<<<<<<<<<<<
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  */
     break;
     case JLS_STORAGE_TYPE_BINARY:
 
-    /* "pyjls/binding.pyx":228
+    /* "pyjls/binding.pyx":229
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  *         return data[:data_size]             # <<<<<<<<<<<<<<
  *     else:
  *         return json.loads(str[:data_size - 1].decode('utf-8'))
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_data) + 0, __pyx_v_data_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_data) + 0, __pyx_v_data_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":227
+    /* "pyjls/binding.pyx":228
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:             # <<<<<<<<<<<<<<
  *         return data[:data_size]
  *     else:
  */
     break;
     default:
 
-    /* "pyjls/binding.pyx":230
+    /* "pyjls/binding.pyx":231
  *         return data[:data_size]
  *     else:
  *         return json.loads(str[:data_size - 1].decode('utf-8'))             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
     break;
   }
 
-  /* "pyjls/binding.pyx":223
+  /* "pyjls/binding.pyx":224
  * 
  * 
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):             # <<<<<<<<<<<<<<
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  */
 
@@ -5106,20 +5111,20 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":233
+/* "pyjls/binding.pyx":234
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
- *     return int((utc - _UTC_OFFSET) * (2**30))
+ *     return int((utc - _UTC_OFFSET) * SECOND)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_15utc_to_jls(PyObject *__pyx_self, PyObject *__pyx_v_utc); /*proto*/
 static char __pyx_doc_5pyjls_7binding_14utc_to_jls[] = "Convert from python UTC timestamp to jls timestamp.";
 static PyMethodDef __pyx_mdef_5pyjls_7binding_15utc_to_jls = {"utc_to_jls", (PyCFunction)__pyx_pw_5pyjls_7binding_15utc_to_jls, METH_O, __pyx_doc_5pyjls_7binding_14utc_to_jls};
 static PyObject *__pyx_pw_5pyjls_7binding_15utc_to_jls(PyObject *__pyx_self, PyObject *__pyx_v_utc) {
@@ -5134,68 +5139,73 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_14utc_to_jls(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_utc) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("utc_to_jls", 0);
 
-  /* "pyjls/binding.pyx":235
+  /* "pyjls/binding.pyx":236
  * def utc_to_jls(utc):
  *     """Convert from python UTC timestamp to jls timestamp."""
- *     return int((utc - _UTC_OFFSET) * (2**30))             # <<<<<<<<<<<<<<
+ *     return int((utc - _UTC_OFFSET) * SECOND)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_v_utc, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_v_utc, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_int_1073741824); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SECOND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":233
+  /* "pyjls/binding.pyx":234
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
- *     return int((utc - _UTC_OFFSET) * (2**30))
+ *     return int((utc - _UTC_OFFSET) * SECOND)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("pyjls.binding.utc_to_jls", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":238
+/* "pyjls/binding.pyx":239
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
- *     return (timestamp / (2**30)) + _UTC_OFFSET
+ *     return (timestamp / SECOND) + _UTC_OFFSET
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_17jls_to_utc(PyObject *__pyx_self, PyObject *__pyx_v_timestamp); /*proto*/
 static char __pyx_doc_5pyjls_7binding_16jls_to_utc[] = "Convert from jls timestamp to python UTC timestamp.";
 static PyMethodDef __pyx_mdef_5pyjls_7binding_17jls_to_utc = {"jls_to_utc", (PyCFunction)__pyx_pw_5pyjls_7binding_17jls_to_utc, METH_O, __pyx_doc_5pyjls_7binding_16jls_to_utc};
 static PyObject *__pyx_pw_5pyjls_7binding_17jls_to_utc(PyObject *__pyx_self, PyObject *__pyx_v_timestamp) {
@@ -5216,40 +5226,43 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("jls_to_utc", 0);
 
-  /* "pyjls/binding.pyx":240
+  /* "pyjls/binding.pyx":241
  * def jls_to_utc(timestamp):
  *     """Convert from jls timestamp to python UTC timestamp."""
- *     return (timestamp / (2**30)) + _UTC_OFFSET             # <<<<<<<<<<<<<<
+ *     return (timestamp / SECOND) + _UTC_OFFSET             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_TrueDivideObjC(__pyx_v_timestamp, __pyx_int_1073741824, 0x40000000, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SECOND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_v_timestamp, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":238
+  /* "pyjls/binding.pyx":239
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
- *     return (timestamp / (2**30)) + _UTC_OFFSET
+ *     return (timestamp / SECOND) + _UTC_OFFSET
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -5257,15 +5270,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":243
+/* "pyjls/binding.pyx":244
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
 
@@ -5300,32 +5313,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, 1); __PYX_ERR(0, 243, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, 1); __PYX_ERR(0, 244, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_handle_rc") < 0)) __PYX_ERR(0, 243, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_handle_rc") < 0)) __PYX_ERR(0, 244, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_rc = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 243, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 244, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding._handle_rc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_18_handle_rc(__pyx_self, __pyx_v_name, __pyx_v_rc);
 
@@ -5348,139 +5361,139 @@
   Py_UCS4 __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_rc", 0);
 
-  /* "pyjls/binding.pyx":244
+  /* "pyjls/binding.pyx":245
  * 
  * def _handle_rc(name, rc):
  *     if rc == 0:             # <<<<<<<<<<<<<<
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_rc, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_rc, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":245
+    /* "pyjls/binding.pyx":246
  * def _handle_rc(name, rc):
  *     if rc == 0:
  *         return             # <<<<<<<<<<<<<<
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":244
+    /* "pyjls/binding.pyx":245
  * 
  * def _handle_rc(name, rc):
  *     if rc == 0:             # <<<<<<<<<<<<<<
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  */
   }
 
-  /* "pyjls/binding.pyx":246
+  /* "pyjls/binding.pyx":247
  *     if rc == 0:
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')             # <<<<<<<<<<<<<<
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')
  *     raise RuntimeError(f'{name} {rc_name}[{rc}]: {rc_descr}')
  */
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
   __pyx_t_4 = jls_error_code_name(__pyx_t_3);
-  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_rc_name = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":247
+  /* "pyjls/binding.pyx":248
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')             # <<<<<<<<<<<<<<
  *     raise RuntimeError(f'{name} {rc_name}[{rc}]: {rc_descr}')
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
   __pyx_t_5 = jls_error_code_description(__pyx_t_3);
-  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_rc_descr = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":248
+  /* "pyjls/binding.pyx":249
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')
  *     raise RuntimeError(f'{name} {rc_name}[{rc}]: {rc_descr}')             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyTuple_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = 0;
   __pyx_t_7 = 127;
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_8);
   __pyx_t_8 = 0;
   __Pyx_INCREF(__pyx_kp_u_);
   __pyx_t_6 += 1;
   __Pyx_GIVEREF(__pyx_kp_u_);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_);
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_8);
   __pyx_t_8 = 0;
   __Pyx_INCREF(__pyx_kp_u__5);
   __pyx_t_6 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__5);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__5);
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_8);
   __pyx_t_8 = 0;
   __Pyx_INCREF(__pyx_kp_u__6);
   __pyx_t_6 += 3;
   __Pyx_GIVEREF(__pyx_kp_u__6);
   PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_kp_u__6);
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_descr, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_descr, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_1, 7, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_1, 7, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 248, __pyx_L1_error)
+  __PYX_ERR(0, 249, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":243
+  /* "pyjls/binding.pyx":244
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
 
@@ -5494,15 +5507,15 @@
   __Pyx_XDECREF(__pyx_v_rc_name);
   __Pyx_XDECREF(__pyx_v_rc_descr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":255
+/* "pyjls/binding.pyx":256
  *     cdef c_jls.jls_signal_def_s _signals[_JLS_SIGNAL_COUNT]
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
  */
 
@@ -5531,32 +5544,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 255, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 256, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_path = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 255, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 256, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 255, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 256, __pyx_L1_error)
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer___init__(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -5576,50 +5589,50 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyjls/binding.pyx":257
+  /* "pyjls/binding.pyx":258
  *     def __init__(self, path: str):
  *         cdef int32_t rc
  *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_open(&self._wr, path.encode('utf-8'))
  *         _handle_rc('open', rc)
  */
   (__pyx_v_self->_signals[0]).signal_type = JLS_SIGNAL_TYPE_VSR;
 
-  /* "pyjls/binding.pyx":258
+  /* "pyjls/binding.pyx":259
  *         cdef int32_t rc
  *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
  *         rc = c_jls.jls_twr_open(&self._wr, path.encode('utf-8'))             # <<<<<<<<<<<<<<
  *         _handle_rc('open', rc)
  * 
  */
   if (unlikely(__pyx_v_path == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 258, __pyx_L1_error)
+    __PYX_ERR(0, 259, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L1_error)
   __pyx_v_rc = jls_twr_open((&__pyx_v_self->_wr), __pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":259
+  /* "pyjls/binding.pyx":260
  *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
  *         rc = c_jls.jls_twr_open(&self._wr, path.encode('utf-8'))
  *         _handle_rc('open', rc)             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -5628,49 +5641,49 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_open);
     __Pyx_GIVEREF(__pyx_n_u_open);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_u_open);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":255
+  /* "pyjls/binding.pyx":256
  *     cdef c_jls.jls_signal_def_s _signals[_JLS_SIGNAL_COUNT]
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
  */
 
@@ -5686,15 +5699,15 @@
   __Pyx_AddTraceback("pyjls.binding.Writer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":261
+/* "pyjls/binding.pyx":262
  *         _handle_rc('open', rc)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -5712,42 +5725,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_2__enter__(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "pyjls/binding.pyx":262
+  /* "pyjls/binding.pyx":263
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, type, value, traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":261
+  /* "pyjls/binding.pyx":262
  *         _handle_rc('open', rc)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":264
+/* "pyjls/binding.pyx":265
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -5784,40 +5797,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 264, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 265, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_traceback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 264, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 265, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 264, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 265, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_type = values[0];
     __pyx_v_value = values[1];
     __pyx_v_traceback = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 264, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 265, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_4__exit__(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_type, __pyx_v_value, __pyx_v_traceback);
 
@@ -5833,41 +5846,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "pyjls/binding.pyx":265
+  /* "pyjls/binding.pyx":266
  * 
  *     def __exit__(self, type, value, traceback):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":264
+  /* "pyjls/binding.pyx":265
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -5882,15 +5895,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":267
+/* "pyjls/binding.pyx":268
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_twr_close(self._wr)
  * 
  */
 
@@ -5908,39 +5921,39 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_6close(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "pyjls/binding.pyx":268
+  /* "pyjls/binding.pyx":269
  * 
  *     def close(self):
  *         c_jls.jls_twr_close(self._wr)             # <<<<<<<<<<<<<<
  * 
  *     def flush(self):
  */
   (void)(jls_twr_close(__pyx_v_self->_wr));
 
-  /* "pyjls/binding.pyx":267
+  /* "pyjls/binding.pyx":268
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_twr_close(self._wr)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":270
+/* "pyjls/binding.pyx":271
  *         c_jls.jls_twr_close(self._wr)
  * 
  *     def flush(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_twr_flush(self._wr)
  * 
  */
 
@@ -5958,39 +5971,39 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_8flush(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("flush", 0);
 
-  /* "pyjls/binding.pyx":271
+  /* "pyjls/binding.pyx":272
  * 
  *     def flush(self):
  *         c_jls.jls_twr_flush(self._wr)             # <<<<<<<<<<<<<<
  * 
  *     def source_def(self, source_id, name=None, vendor=None, model=None, version=None, serial_number=None):
  */
   (void)(jls_twr_flush(__pyx_v_self->_wr));
 
-  /* "pyjls/binding.pyx":270
+  /* "pyjls/binding.pyx":271
  *         c_jls.jls_twr_close(self._wr)
  * 
  *     def flush(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_twr_flush(self._wr)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":273
+/* "pyjls/binding.pyx":274
  *         c_jls.jls_twr_flush(self._wr)
  * 
  *     def source_def(self, source_id, name=None, vendor=None, model=None, version=None, serial_number=None):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s s
  */
 
@@ -6069,15 +6082,15 @@
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_number);
           if (value) { values[5] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "source_def") < 0)) __PYX_ERR(0, 273, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "source_def") < 0)) __PYX_ERR(0, 274, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
@@ -6097,15 +6110,15 @@
     __pyx_v_vendor = values[2];
     __pyx_v_model = values[3];
     __pyx_v_version = values[4];
     __pyx_v_serial_number = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("source_def", 0, 1, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 273, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("source_def", 0, 1, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 274, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.source_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_10source_def(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_source_id, __pyx_v_name, __pyx_v_vendor, __pyx_v_model, __pyx_v_version, __pyx_v_serial_number);
 
@@ -6137,228 +6150,228 @@
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("source_def", 0);
 
-  /* "pyjls/binding.pyx":276
+  /* "pyjls/binding.pyx":277
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s s
  *         name_b = _encode_str(name)             # <<<<<<<<<<<<<<
  *         vendor_b = _encode_str(vendor)
  *         model_b = _encode_str(model)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_name_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":277
+  /* "pyjls/binding.pyx":278
  *         cdef c_jls.jls_source_def_s s
  *         name_b = _encode_str(name)
  *         vendor_b = _encode_str(vendor)             # <<<<<<<<<<<<<<
  *         model_b = _encode_str(model)
  *         version_b = _encode_str(version)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_vendor) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_vendor);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_vendor_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":278
+  /* "pyjls/binding.pyx":279
  *         name_b = _encode_str(name)
  *         vendor_b = _encode_str(vendor)
  *         model_b = _encode_str(model)             # <<<<<<<<<<<<<<
  *         version_b = _encode_str(version)
  *         serial_number_b = _encode_str(serial_number)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_model) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_model);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_model_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":279
+  /* "pyjls/binding.pyx":280
  *         vendor_b = _encode_str(vendor)
  *         model_b = _encode_str(model)
  *         version_b = _encode_str(version)             # <<<<<<<<<<<<<<
  *         serial_number_b = _encode_str(serial_number)
  *         s.source_id = source_id
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_version) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_version);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_version_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":280
+  /* "pyjls/binding.pyx":281
  *         model_b = _encode_str(model)
  *         version_b = _encode_str(version)
  *         serial_number_b = _encode_str(serial_number)             # <<<<<<<<<<<<<<
  *         s.source_id = source_id
  *         s.name = name_b
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_serial_number) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_serial_number);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_serial_number_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":281
+  /* "pyjls/binding.pyx":282
  *         version_b = _encode_str(version)
  *         serial_number_b = _encode_str(serial_number)
  *         s.source_id = source_id             # <<<<<<<<<<<<<<
  *         s.name = name_b
  *         s.vendor = vendor_b
  */
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L1_error)
   __pyx_v_s.source_id = __pyx_t_4;
 
-  /* "pyjls/binding.pyx":282
+  /* "pyjls/binding.pyx":283
  *         serial_number_b = _encode_str(serial_number)
  *         s.source_id = source_id
  *         s.name = name_b             # <<<<<<<<<<<<<<
  *         s.vendor = vendor_b
  *         s.model = model_b
  */
-  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L1_error)
   __pyx_v_s.name = __pyx_t_5;
 
-  /* "pyjls/binding.pyx":283
+  /* "pyjls/binding.pyx":284
  *         s.source_id = source_id
  *         s.name = name_b
  *         s.vendor = vendor_b             # <<<<<<<<<<<<<<
  *         s.model = model_b
  *         s.version = version_b
  */
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_v_vendor_b); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_v_vendor_b); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
   __pyx_v_s.vendor = __pyx_t_6;
 
-  /* "pyjls/binding.pyx":284
+  /* "pyjls/binding.pyx":285
  *         s.name = name_b
  *         s.vendor = vendor_b
  *         s.model = model_b             # <<<<<<<<<<<<<<
  *         s.version = version_b
  *         s.serial_number = serial_number_b
  */
-  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_v_model_b); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_v_model_b); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
   __pyx_v_s.model = __pyx_t_7;
 
-  /* "pyjls/binding.pyx":285
+  /* "pyjls/binding.pyx":286
  *         s.vendor = vendor_b
  *         s.model = model_b
  *         s.version = version_b             # <<<<<<<<<<<<<<
  *         s.serial_number = serial_number_b
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_version_b); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_version_b); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 286, __pyx_L1_error)
   __pyx_v_s.version = __pyx_t_8;
 
-  /* "pyjls/binding.pyx":286
+  /* "pyjls/binding.pyx":287
  *         s.model = model_b
  *         s.version = version_b
  *         s.serial_number = serial_number_b             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)
  *         _handle_rc('source_def', rc)
  */
-  __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_serial_number_b); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_serial_number_b); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L1_error)
   __pyx_v_s.serial_number = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":287
+  /* "pyjls/binding.pyx":288
  *         s.version = version_b
  *         s.serial_number = serial_number_b
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)             # <<<<<<<<<<<<<<
  *         _handle_rc('source_def', rc)
  * 
  */
   __pyx_v_rc = jls_twr_source_def(__pyx_v_self->_wr, (&__pyx_v_s));
 
-  /* "pyjls/binding.pyx":288
+  /* "pyjls/binding.pyx":289
  *         s.serial_number = serial_number_b
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)
  *         _handle_rc('source_def', rc)             # <<<<<<<<<<<<<<
  * 
  *     def source_def_from_struct(self, s: SourceDef):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_10 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -6367,49 +6380,49 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_source_def, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_source_def, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     if (__pyx_t_10) {
       __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_source_def);
     __Pyx_GIVEREF(__pyx_n_u_source_def);
     PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_n_u_source_def);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":273
+  /* "pyjls/binding.pyx":274
  *         c_jls.jls_twr_flush(self._wr)
  * 
  *     def source_def(self, source_id, name=None, vendor=None, model=None, version=None, serial_number=None):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s s
  */
 
@@ -6431,15 +6444,15 @@
   __Pyx_XDECREF(__pyx_v_version_b);
   __Pyx_XDECREF(__pyx_v_serial_number_b);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":290
+/* "pyjls/binding.pyx":291
  *         _handle_rc('source_def', rc)
  * 
  *     def source_def_from_struct(self, s: SourceDef):             # <<<<<<<<<<<<<<
  *         return self.source_def(s.source_id,
  *                                name=s.name,
  */
 
@@ -6464,111 +6477,111 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("source_def_from_struct", 0);
 
-  /* "pyjls/binding.pyx":291
+  /* "pyjls/binding.pyx":292
  * 
  *     def source_def_from_struct(self, s: SourceDef):
  *         return self.source_def(s.source_id,             # <<<<<<<<<<<<<<
  *                                name=s.name,
  *                                vendor=s.vendor,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":292
+  /* "pyjls/binding.pyx":293
  *     def source_def_from_struct(self, s: SourceDef):
  *         return self.source_def(s.source_id,
  *                                name=s.name,             # <<<<<<<<<<<<<<
  *                                vendor=s.vendor,
  *                                model=s.model,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":293
+  /* "pyjls/binding.pyx":294
  *         return self.source_def(s.source_id,
  *                                name=s.name,
  *                                vendor=s.vendor,             # <<<<<<<<<<<<<<
  *                                model=s.model,
  *                                version=s.version,
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_vendor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_vendor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vendor, __pyx_t_4) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vendor, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":294
+  /* "pyjls/binding.pyx":295
  *                                name=s.name,
  *                                vendor=s.vendor,
  *                                model=s.model,             # <<<<<<<<<<<<<<
  *                                version=s.version,
  *                                serial_number=s.serial_number)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_model); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_model); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_model, __pyx_t_4) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_model, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":295
+  /* "pyjls/binding.pyx":296
  *                                vendor=s.vendor,
  *                                model=s.model,
  *                                version=s.version,             # <<<<<<<<<<<<<<
  *                                serial_number=s.serial_number)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_version); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_version); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_version, __pyx_t_4) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_version, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":296
+  /* "pyjls/binding.pyx":297
  *                                model=s.model,
  *                                version=s.version,
  *                                serial_number=s.serial_number)             # <<<<<<<<<<<<<<
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_serial_number); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_serial_number); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_serial_number, __pyx_t_4) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_serial_number, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":291
+  /* "pyjls/binding.pyx":292
  * 
  *     def source_def_from_struct(self, s: SourceDef):
  *         return self.source_def(s.source_id,             # <<<<<<<<<<<<<<
  *                                name=s.name,
  *                                vendor=s.vendor,
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":290
+  /* "pyjls/binding.pyx":291
  *         _handle_rc('source_def', rc)
  * 
  *     def source_def_from_struct(self, s: SourceDef):             # <<<<<<<<<<<<<<
  *         return self.source_def(s.source_id,
  *                                name=s.name,
  */
 
@@ -6582,15 +6595,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":298
+/* "pyjls/binding.pyx":299
  *                                serial_number=s.serial_number)
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,             # <<<<<<<<<<<<<<
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  */
 
@@ -6619,37 +6632,37 @@
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_signal_id,&__pyx_n_s_source_id,&__pyx_n_s_signal_type,&__pyx_n_s_data_type,&__pyx_n_s_sample_rate,&__pyx_n_s_samples_per_data,&__pyx_n_s_sample_decimate_factor,&__pyx_n_s_entries_per_summary,&__pyx_n_s_summary_decimate_factor,&__pyx_n_s_annotation_decimate_factor,&__pyx_n_s_utc_decimate_factor,&__pyx_n_s_name,&__pyx_n_s_units,0};
     PyObject* values[13] = {0,0,0,0,0,0,0,0,0,0,0,0,0};
     values[2] = ((PyObject *)Py_None);
     values[3] = ((PyObject *)Py_None);
     values[4] = ((PyObject *)Py_None);
 
-    /* "pyjls/binding.pyx":299
+    /* "pyjls/binding.pyx":300
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,             # <<<<<<<<<<<<<<
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  *                    name=None, units=None):
  */
     values[5] = ((PyObject *)Py_None);
     values[6] = ((PyObject *)Py_None);
     values[7] = ((PyObject *)Py_None);
 
-    /* "pyjls/binding.pyx":300
+    /* "pyjls/binding.pyx":301
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,             # <<<<<<<<<<<<<<
  *                    name=None, units=None):
  *         cdef int32_t rc
  */
     values[8] = ((PyObject *)Py_None);
     values[9] = ((PyObject *)Py_None);
     values[10] = ((PyObject *)Py_None);
 
-    /* "pyjls/binding.pyx":301
+    /* "pyjls/binding.pyx":302
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  *                    name=None, units=None):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_signal_def_s * s
  */
     values[11] = ((PyObject *)Py_None);
@@ -6692,15 +6705,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_source_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, 1); __PYX_ERR(0, 298, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, 1); __PYX_ERR(0, 299, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_type);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -6762,15 +6775,15 @@
         case 12:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_units);
           if (value) { values[12] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "signal_def") < 0)) __PYX_ERR(0, 298, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "signal_def") < 0)) __PYX_ERR(0, 299, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case 13: values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
         CYTHON_FALLTHROUGH;
         case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
         CYTHON_FALLTHROUGH;
@@ -6810,23 +6823,23 @@
     __pyx_v_annotation_decimate_factor = values[9];
     __pyx_v_utc_decimate_factor = values[10];
     __pyx_v_name = values[11];
     __pyx_v_units = values[12];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 298, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 299, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.signal_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_14signal_def(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_source_id, __pyx_v_signal_type, __pyx_v_data_type, __pyx_v_sample_rate, __pyx_v_samples_per_data, __pyx_v_sample_decimate_factor, __pyx_v_entries_per_summary, __pyx_v_summary_decimate_factor, __pyx_v_annotation_decimate_factor, __pyx_v_utc_decimate_factor, __pyx_v_name, __pyx_v_units);
 
-  /* "pyjls/binding.pyx":298
+  /* "pyjls/binding.pyx":299
  *                                serial_number=s.serial_number)
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,             # <<<<<<<<<<<<<<
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  */
 
@@ -6860,371 +6873,371 @@
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signal_def", 0);
   __Pyx_INCREF(__pyx_v_data_type);
 
-  /* "pyjls/binding.pyx":304
+  /* "pyjls/binding.pyx":305
  *         cdef int32_t rc
  *         cdef c_jls.jls_signal_def_s * s
  *         s = &self._signals[signal_id]             # <<<<<<<<<<<<<<
  *         if data_type is None:
  *             data_type = DataType.F32
  */
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 305, __pyx_L1_error)
   __pyx_v_s = (&(__pyx_v_self->_signals[__pyx_t_1]));
 
-  /* "pyjls/binding.pyx":305
+  /* "pyjls/binding.pyx":306
  *         cdef c_jls.jls_signal_def_s * s
  *         s = &self._signals[signal_id]
  *         if data_type is None:             # <<<<<<<<<<<<<<
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):
  */
   __pyx_t_2 = (__pyx_v_data_type == Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "pyjls/binding.pyx":306
+    /* "pyjls/binding.pyx":307
  *         s = &self._signals[signal_id]
  *         if data_type is None:
  *             data_type = DataType.F32             # <<<<<<<<<<<<<<
  *         elif isinstance(data_type, str):
  *             data_type = _data_type_as_enum[data_type]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 306, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_F32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 306, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_F32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_data_type, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":305
+    /* "pyjls/binding.pyx":306
  *         cdef c_jls.jls_signal_def_s * s
  *         s = &self._signals[signal_id]
  *         if data_type is None:             # <<<<<<<<<<<<<<
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):
  */
     goto __pyx_L3;
   }
 
-  /* "pyjls/binding.pyx":307
+  /* "pyjls/binding.pyx":308
  *         if data_type is None:
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):             # <<<<<<<<<<<<<<
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id
  */
   __pyx_t_3 = PyUnicode_Check(__pyx_v_data_type); 
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":308
+    /* "pyjls/binding.pyx":309
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):
  *             data_type = _data_type_as_enum[data_type]             # <<<<<<<<<<<<<<
  *         s.signal_id = signal_id
  *         s.source_id = source_id
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 309, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 309, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_data_type, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":307
+    /* "pyjls/binding.pyx":308
  *         if data_type is None:
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):             # <<<<<<<<<<<<<<
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id
  */
   }
   __pyx_L3:;
 
-  /* "pyjls/binding.pyx":309
+  /* "pyjls/binding.pyx":310
  *         elif isinstance(data_type, str):
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id             # <<<<<<<<<<<<<<
  *         s.source_id = source_id
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  */
-  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L1_error)
   __pyx_v_s->signal_id = __pyx_t_6;
 
-  /* "pyjls/binding.pyx":310
+  /* "pyjls/binding.pyx":311
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id
  *         s.source_id = source_id             # <<<<<<<<<<<<<<
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  *         s.data_type = data_type
  */
-  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L1_error)
   __pyx_v_s->source_id = __pyx_t_6;
 
-  /* "pyjls/binding.pyx":311
+  /* "pyjls/binding.pyx":312
  *         s.signal_id = signal_id
  *         s.source_id = source_id
  *         s.signal_type = 0 if signal_type is None else int(signal_type)             # <<<<<<<<<<<<<<
  *         s.data_type = data_type
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  */
   __pyx_t_2 = (__pyx_v_signal_type == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_7 = 0;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_t_4); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_t_4); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_7 = __pyx_t_8;
   }
   __pyx_v_s->signal_type = __pyx_t_7;
 
-  /* "pyjls/binding.pyx":312
+  /* "pyjls/binding.pyx":313
  *         s.source_id = source_id
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  *         s.data_type = data_type             # <<<<<<<<<<<<<<
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  */
-  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_data_type); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_data_type); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 313, __pyx_L1_error)
   __pyx_v_s->data_type = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":313
+  /* "pyjls/binding.pyx":314
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  *         s.data_type = data_type
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)             # <<<<<<<<<<<<<<
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_sample_rate == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 313, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 313, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->sample_rate = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":314
+  /* "pyjls/binding.pyx":315
  *         s.data_type = data_type
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)             # <<<<<<<<<<<<<<
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  */
   __pyx_t_2 = (__pyx_v_samples_per_data == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x186A0;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->samples_per_data = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":315
+  /* "pyjls/binding.pyx":316
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)             # <<<<<<<<<<<<<<
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_sample_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 315, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 316, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->sample_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":316
+  /* "pyjls/binding.pyx":317
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)             # <<<<<<<<<<<<<<
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_entries_per_summary == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x4E20;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->entries_per_summary = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":317
+  /* "pyjls/binding.pyx":318
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)             # <<<<<<<<<<<<<<
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_summary_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->summary_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":318
+  /* "pyjls/binding.pyx":319
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)             # <<<<<<<<<<<<<<
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  *         name_b = _encode_str(name)
  */
   __pyx_t_2 = (__pyx_v_annotation_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 318, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 318, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->annotation_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":319
+  /* "pyjls/binding.pyx":320
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)             # <<<<<<<<<<<<<<
  *         name_b = _encode_str(name)
  *         units_b = _encode_str(units)
  */
   __pyx_t_2 = (__pyx_v_utc_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->utc_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":320
+  /* "pyjls/binding.pyx":321
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  *         name_b = _encode_str(name)             # <<<<<<<<<<<<<<
  *         units_b = _encode_str(units)
  *         s.name = name_b
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_11, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 320, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_name_b = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":321
+  /* "pyjls/binding.pyx":322
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  *         name_b = _encode_str(name)
  *         units_b = _encode_str(units)             # <<<<<<<<<<<<<<
  *         s.name = name_b
  *         s.units = units_b
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_11, __pyx_v_units) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_units);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_units_b = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":322
+  /* "pyjls/binding.pyx":323
  *         name_b = _encode_str(name)
  *         units_b = _encode_str(units)
  *         s.name = name_b             # <<<<<<<<<<<<<<
  *         s.units = units_b
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)
  */
-  __pyx_t_12 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L1_error)
   __pyx_v_s->name = __pyx_t_12;
 
-  /* "pyjls/binding.pyx":323
+  /* "pyjls/binding.pyx":324
  *         units_b = _encode_str(units)
  *         s.name = name_b
  *         s.units = units_b             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)
  *         _handle_rc('signal_def', rc)
  */
-  __pyx_t_13 = __Pyx_PyObject_AsString(__pyx_v_units_b); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_AsString(__pyx_v_units_b); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 324, __pyx_L1_error)
   __pyx_v_s->units = __pyx_t_13;
 
-  /* "pyjls/binding.pyx":324
+  /* "pyjls/binding.pyx":325
  *         s.name = name_b
  *         s.units = units_b
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)             # <<<<<<<<<<<<<<
  *         _handle_rc('signal_def', rc)
  * 
  */
   __pyx_v_rc = jls_twr_signal_def(__pyx_v_self->_wr, __pyx_v_s);
 
-  /* "pyjls/binding.pyx":325
+  /* "pyjls/binding.pyx":326
  *         s.units = units_b
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)
  *         _handle_rc('signal_def', rc)             # <<<<<<<<<<<<<<
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_11 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __pyx_t_14 = NULL;
   __pyx_t_15 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -7233,49 +7246,49 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_15 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_n_u_signal_def, __pyx_t_11};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_n_u_signal_def, __pyx_t_11};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   {
-    __pyx_t_16 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __pyx_t_16 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 326, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     if (__pyx_t_14) {
       __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_14); __pyx_t_14 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_signal_def);
     __Pyx_GIVEREF(__pyx_n_u_signal_def);
     PyTuple_SET_ITEM(__pyx_t_16, 0+__pyx_t_15, __pyx_n_u_signal_def);
     __Pyx_GIVEREF(__pyx_t_11);
     PyTuple_SET_ITEM(__pyx_t_16, 1+__pyx_t_15, __pyx_t_11);
     __pyx_t_11 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":298
+  /* "pyjls/binding.pyx":299
  *                                serial_number=s.serial_number)
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,             # <<<<<<<<<<<<<<
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  */
 
@@ -7295,15 +7308,15 @@
   __Pyx_XDECREF(__pyx_v_units_b);
   __Pyx_XDECREF(__pyx_v_data_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":327
+/* "pyjls/binding.pyx":328
  *         _handle_rc('signal_def', rc)
  * 
  *     def signal_def_from_struct(self, s: SignalDef):             # <<<<<<<<<<<<<<
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,
  */
 
@@ -7328,204 +7341,204 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signal_def_from_struct", 0);
 
-  /* "pyjls/binding.pyx":328
+  /* "pyjls/binding.pyx":329
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,             # <<<<<<<<<<<<<<
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_signal_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_signal_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "pyjls/binding.pyx":329
+  /* "pyjls/binding.pyx":330
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,             # <<<<<<<<<<<<<<
  *                                signal_type=s.signal_type,
  *                                data_type=s.data_type,
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "pyjls/binding.pyx":328
+  /* "pyjls/binding.pyx":329
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,             # <<<<<<<<<<<<<<
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  */
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":330
+  /* "pyjls/binding.pyx":331
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,
  *                                signal_type=s.signal_type,             # <<<<<<<<<<<<<<
  *                                data_type=s.data_type,
  *                                sample_rate=s.sample_rate,
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":331
+  /* "pyjls/binding.pyx":332
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  *                                data_type=s.data_type,             # <<<<<<<<<<<<<<
  *                                sample_rate=s.sample_rate,
  *                                samples_per_data=s.samples_per_data,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":332
+  /* "pyjls/binding.pyx":333
  *                                signal_type=s.signal_type,
  *                                data_type=s.data_type,
  *                                sample_rate=s.sample_rate,             # <<<<<<<<<<<<<<
  *                                samples_per_data=s.samples_per_data,
  *                                sample_decimate_factor=s.sample_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":333
+  /* "pyjls/binding.pyx":334
  *                                data_type=s.data_type,
  *                                sample_rate=s.sample_rate,
  *                                samples_per_data=s.samples_per_data,             # <<<<<<<<<<<<<<
  *                                sample_decimate_factor=s.sample_decimate_factor,
  *                                entries_per_summary=s.entries_per_summary,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_samples_per_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_samples_per_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":334
+  /* "pyjls/binding.pyx":335
  *                                sample_rate=s.sample_rate,
  *                                samples_per_data=s.samples_per_data,
  *                                sample_decimate_factor=s.sample_decimate_factor,             # <<<<<<<<<<<<<<
  *                                entries_per_summary=s.entries_per_summary,
  *                                summary_decimate_factor=s.summary_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":335
+  /* "pyjls/binding.pyx":336
  *                                samples_per_data=s.samples_per_data,
  *                                sample_decimate_factor=s.sample_decimate_factor,
  *                                entries_per_summary=s.entries_per_summary,             # <<<<<<<<<<<<<<
  *                                summary_decimate_factor=s.summary_decimate_factor,
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_entries_per_summary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_entries_per_summary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":336
+  /* "pyjls/binding.pyx":337
  *                                sample_decimate_factor=s.sample_decimate_factor,
  *                                entries_per_summary=s.entries_per_summary,
  *                                summary_decimate_factor=s.summary_decimate_factor,             # <<<<<<<<<<<<<<
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  *                                utc_decimate_factor=s.utc_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_summary_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_summary_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":337
+  /* "pyjls/binding.pyx":338
  *                                entries_per_summary=s.entries_per_summary,
  *                                summary_decimate_factor=s.summary_decimate_factor,
  *                                annotation_decimate_factor=s.annotation_decimate_factor,             # <<<<<<<<<<<<<<
  *                                utc_decimate_factor=s.utc_decimate_factor,
  *                                name=s.name,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_annotation_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_annotation_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":338
+  /* "pyjls/binding.pyx":339
  *                                summary_decimate_factor=s.summary_decimate_factor,
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  *                                utc_decimate_factor=s.utc_decimate_factor,             # <<<<<<<<<<<<<<
  *                                name=s.name,
  *                                units=s.units)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_utc_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_utc_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":339
+  /* "pyjls/binding.pyx":340
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  *                                utc_decimate_factor=s.utc_decimate_factor,
  *                                name=s.name,             # <<<<<<<<<<<<<<
  *                                units=s.units)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":340
+  /* "pyjls/binding.pyx":341
  *                                utc_decimate_factor=s.utc_decimate_factor,
  *                                name=s.name,
  *                                units=s.units)             # <<<<<<<<<<<<<<
  * 
  *     def user_data(self, chunk_meta, data):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_units); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_units); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_2) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":328
+  /* "pyjls/binding.pyx":329
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,             # <<<<<<<<<<<<<<
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":327
+  /* "pyjls/binding.pyx":328
  *         _handle_rc('signal_def', rc)
  * 
  *     def signal_def_from_struct(self, s: SignalDef):             # <<<<<<<<<<<<<<
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,
  */
 
@@ -7539,15 +7552,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":342
+/* "pyjls/binding.pyx":343
  *                                units=s.units)
  * 
  *     def user_data(self, chunk_meta, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         storage_type, payload, payload_length = _storage_pack(data)
  */
 
@@ -7581,32 +7594,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_chunk_meta)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, 1); __PYX_ERR(0, 342, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, 1); __PYX_ERR(0, 343, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "user_data") < 0)) __PYX_ERR(0, 342, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "user_data") < 0)) __PYX_ERR(0, 343, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_chunk_meta = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 342, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 343, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.user_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_18user_data(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_chunk_meta, __pyx_v_data);
 
@@ -7634,45 +7647,45 @@
   uint32_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("user_data", 0);
 
-  /* "pyjls/binding.pyx":344
+  /* "pyjls/binding.pyx":345
  *     def user_data(self, chunk_meta, data):
  *         cdef int32_t rc
  *         storage_type, payload, payload_length = _storage_pack(data)             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_user_data(self._wr, chunk_meta, storage_type, payload, payload_length)
  *         _handle_rc('user_data', rc)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 344, __pyx_L1_error)
+      __PYX_ERR(0, 345, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -7680,75 +7693,75 @@
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 2; __pyx_t_4 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 345, __pyx_L1_error)
     __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 344, __pyx_L1_error)
+    __PYX_ERR(0, 345, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_storage_type = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_payload = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_payload_length = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":345
+  /* "pyjls/binding.pyx":346
  *         cdef int32_t rc
  *         storage_type, payload, payload_length = _storage_pack(data)
  *         rc = c_jls.jls_twr_user_data(self._wr, chunk_meta, storage_type, payload, payload_length)             # <<<<<<<<<<<<<<
  *         _handle_rc('user_data', rc)
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_chunk_meta); if (unlikely((__pyx_t_7 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
-  __pyx_t_8 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_v_storage_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_payload); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_v_payload_length); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_chunk_meta); if (unlikely((__pyx_t_7 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_8 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_v_storage_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_payload); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_v_payload_length); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
   __pyx_v_rc = jls_twr_user_data(__pyx_v_self->_wr, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10);
 
-  /* "pyjls/binding.pyx":346
+  /* "pyjls/binding.pyx":347
  *         storage_type, payload, payload_length = _storage_pack(data)
  *         rc = c_jls.jls_twr_user_data(self._wr, chunk_meta, storage_type, payload, payload_length)
  *         _handle_rc('user_data', rc)             # <<<<<<<<<<<<<<
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7757,49 +7770,49 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_n_u_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_n_u_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_user_data);
     __Pyx_GIVEREF(__pyx_n_u_user_data);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_11, __pyx_n_u_user_data);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_11, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":342
+  /* "pyjls/binding.pyx":343
  *                                units=s.units)
  * 
  *     def user_data(self, chunk_meta, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         storage_type, payload, payload_length = _storage_pack(data)
  */
 
@@ -7819,15 +7832,15 @@
   __Pyx_XDECREF(__pyx_v_payload);
   __Pyx_XDECREF(__pyx_v_payload_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":348
+/* "pyjls/binding.pyx":349
  *         _handle_rc('user_data', rc)
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
  *         return self.fsr(signal_id, sample_id, data)
  * 
  */
 
@@ -7864,40 +7877,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 1); __PYX_ERR(0, 348, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 1); __PYX_ERR(0, 349, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 2); __PYX_ERR(0, 348, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 2); __PYX_ERR(0, 349, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_f32") < 0)) __PYX_ERR(0, 348, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_f32") < 0)) __PYX_ERR(0, 349, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 348, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 349, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.fsr_f32", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_20fsr_f32(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data);
 
@@ -7915,23 +7928,23 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr_f32", 0);
 
-  /* "pyjls/binding.pyx":349
+  /* "pyjls/binding.pyx":350
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):
  *         return self.fsr(signal_id, sample_id, data)             # <<<<<<<<<<<<<<
  * 
  *     def fsr(self, signal_id, sample_id, data):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fsr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fsr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7940,52 +7953,52 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_signal_id);
     __Pyx_GIVEREF(__pyx_v_signal_id);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_signal_id);
     __Pyx_INCREF(__pyx_v_sample_id);
     __Pyx_GIVEREF(__pyx_v_sample_id);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_sample_id);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_data);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":348
+  /* "pyjls/binding.pyx":349
  *         _handle_rc('user_data', rc)
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
  *         return self.fsr(signal_id, sample_id, data)
  * 
  */
 
@@ -7999,15 +8012,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":351
+/* "pyjls/binding.pyx":352
  *         return self.fsr(signal_id, sample_id, data)
  * 
  *     def fsr(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef np.uint8_t [::1] u8
  */
 
@@ -8044,40 +8057,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 351, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 352, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 351, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 352, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 351, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 352, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 351, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 352, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.fsr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_22fsr(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data);
 
@@ -8112,247 +8125,247 @@
   int __pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr", 0);
 
-  /* "pyjls/binding.pyx":358
+  /* "pyjls/binding.pyx":359
  *         cdef uint32_t length
  * 
  *         data_type = self._signals[signal_id].data_type             # <<<<<<<<<<<<<<
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  */
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 359, __pyx_L1_error)
   __pyx_t_2 = (__pyx_v_self->_signals[__pyx_t_1]).data_type;
   __pyx_v_data_type = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":359
+  /* "pyjls/binding.pyx":360
  * 
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff             # <<<<<<<<<<<<<<
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:
  */
   __pyx_v_entry_size_bits = ((__pyx_v_data_type >> 8) & 0xff);
 
-  /* "pyjls/binding.pyx":360
+  /* "pyjls/binding.pyx":361
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]             # <<<<<<<<<<<<<<
  *         if np_type != data.dtype:
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = (__pyx_v_data_type & 0xffff);
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_3, __pyx_t_4, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_3, __pyx_t_4, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_np_type = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":361
+  /* "pyjls/binding.pyx":362
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_np_type, __pyx_t_5, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_v_np_type, __pyx_t_5, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_t_6)) {
 
-    /* "pyjls/binding.pyx":362
+    /* "pyjls/binding.pyx":363
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')             # <<<<<<<<<<<<<<
  *         data_u8 = data.view(dtype=np.uint8)
  *         u8 = data_u8
  */
-    __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Data_type_mismatch);
     __pyx_t_1 += 19;
     __Pyx_GIVEREF(__pyx_kp_u_Data_type_mismatch);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Data_type_mismatch);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 363, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
     __pyx_t_1 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u__7);
     __pyx_t_1 += 4;
     __Pyx_GIVEREF(__pyx_kp_u__7);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__7);
-    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_np_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_np_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
     __pyx_t_1 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_t_8);
     __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 362, __pyx_L1_error)
+    __PYX_ERR(0, 363, __pyx_L1_error)
 
-    /* "pyjls/binding.pyx":361
+    /* "pyjls/binding.pyx":362
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)
  */
   }
 
-  /* "pyjls/binding.pyx":363
+  /* "pyjls/binding.pyx":364
  *         if np_type != data.dtype:
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)             # <<<<<<<<<<<<<<
  *         u8 = data_u8
  *         length = len(data)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_view); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_view); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_data_u8 = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "pyjls/binding.pyx":364
+  /* "pyjls/binding.pyx":365
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)
  *         u8 = data_u8             # <<<<<<<<<<<<<<
  *         length = len(data)
  *         if entry_size_bits == 4:
  */
-  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 365, __pyx_L1_error)
   __pyx_v_u8 = __pyx_t_10;
   __pyx_t_10.memview = NULL;
   __pyx_t_10.data = NULL;
 
-  /* "pyjls/binding.pyx":365
+  /* "pyjls/binding.pyx":366
  *         data_u8 = data.view(dtype=np.uint8)
  *         u8 = data_u8
  *         length = len(data)             # <<<<<<<<<<<<<<
  *         if entry_size_bits == 4:
  *             length *= 2
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 366, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "pyjls/binding.pyx":366
+  /* "pyjls/binding.pyx":367
  *         u8 = data_u8
  *         length = len(data)
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             length *= 2
  *         elif entry_size_bits == 1:
  */
   switch (__pyx_v_entry_size_bits) {
     case 4:
 
-    /* "pyjls/binding.pyx":367
+    /* "pyjls/binding.pyx":368
  *         length = len(data)
  *         if entry_size_bits == 4:
  *             length *= 2             # <<<<<<<<<<<<<<
  *         elif entry_size_bits == 1:
  *             length *= 8
  */
     __pyx_v_length = (__pyx_v_length * 2);
 
-    /* "pyjls/binding.pyx":366
+    /* "pyjls/binding.pyx":367
  *         u8 = data_u8
  *         length = len(data)
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             length *= 2
  *         elif entry_size_bits == 1:
  */
     break;
     case 1:
 
-    /* "pyjls/binding.pyx":369
+    /* "pyjls/binding.pyx":370
  *             length *= 2
  *         elif entry_size_bits == 1:
  *             length *= 8             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)
  *         _handle_rc('fsr', rc)
  */
     __pyx_v_length = (__pyx_v_length * 8);
 
-    /* "pyjls/binding.pyx":368
+    /* "pyjls/binding.pyx":369
  *         if entry_size_bits == 4:
  *             length *= 2
  *         elif entry_size_bits == 1:             # <<<<<<<<<<<<<<
  *             length *= 8
  *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)
  */
     break;
     default: break;
   }
 
-  /* "pyjls/binding.pyx":370
+  /* "pyjls/binding.pyx":371
  *         elif entry_size_bits == 1:
  *             length *= 8
  *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)             # <<<<<<<<<<<<<<
  *         _handle_rc('fsr', rc)
  * 
  */
-  __pyx_t_11 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_11 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 370, __pyx_L1_error)
-  __pyx_t_12 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_12 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_11 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_12 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
   __pyx_t_13 = 0;
   __pyx_t_14 = -1;
   if (__pyx_t_13 < 0) {
     __pyx_t_13 += __pyx_v_u8.shape[0];
     if (unlikely(__pyx_t_13 < 0)) __pyx_t_14 = 0;
   } else if (unlikely(__pyx_t_13 >= __pyx_v_u8.shape[0])) __pyx_t_14 = 0;
   if (unlikely(__pyx_t_14 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_14);
-    __PYX_ERR(0, 370, __pyx_L1_error)
+    __PYX_ERR(0, 371, __pyx_L1_error)
   }
   __pyx_v_rc = jls_twr_fsr(__pyx_v_self->_wr, __pyx_t_11, __pyx_t_12, (&(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_u8.data) + __pyx_t_13)) )))), __pyx_v_length);
 
-  /* "pyjls/binding.pyx":371
+  /* "pyjls/binding.pyx":372
  *             length *= 8
  *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)
  *         _handle_rc('fsr', rc)             # <<<<<<<<<<<<<<
  * 
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_14 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -8361,49 +8374,49 @@
       __Pyx_DECREF_SET(__pyx_t_8, function);
       __pyx_t_14 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_8)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_fsr, __pyx_t_3};
-    __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_fsr, __pyx_t_3};
-    __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_15 = PyTuple_New(2+__pyx_t_14); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_15 = PyTuple_New(2+__pyx_t_14); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_fsr);
     __Pyx_GIVEREF(__pyx_n_u_fsr);
     PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_14, __pyx_n_u_fsr);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_15, 1+__pyx_t_14, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_15, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_15, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   }
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "pyjls/binding.pyx":351
+  /* "pyjls/binding.pyx":352
  *         return self.fsr(signal_id, sample_id, data)
  * 
  *     def fsr(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef np.uint8_t [::1] u8
  */
 
@@ -8424,15 +8437,15 @@
   __Pyx_XDECREF(__pyx_v_np_type);
   __Pyx_XDECREF(__pyx_v_data_u8);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":373
+/* "pyjls/binding.pyx":374
  *         _handle_rc('fsr', rc)
  * 
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         if isinstance(annotation_type, str):
  */
 
@@ -8478,43 +8491,43 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timestamp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 1); __PYX_ERR(0, 373, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 1); __PYX_ERR(0, 374, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_y)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 2); __PYX_ERR(0, 373, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 2); __PYX_ERR(0, 374, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_annotation_type)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 3); __PYX_ERR(0, 373, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 3); __PYX_ERR(0, 374, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_group_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 4); __PYX_ERR(0, 373, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 4); __PYX_ERR(0, 374, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 5); __PYX_ERR(0, 373, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 5); __PYX_ERR(0, 374, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotation") < 0)) __PYX_ERR(0, 373, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotation") < 0)) __PYX_ERR(0, 374, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -8527,15 +8540,15 @@
     __pyx_v_y = values[2];
     __pyx_v_annotation_type = values[3];
     __pyx_v_group_id = values[4];
     __pyx_v_data = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 373, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 374, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.annotation", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_24annotation(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_timestamp, __pyx_v_y, __pyx_v_annotation_type, __pyx_v_group_id, __pyx_v_data);
 
@@ -8572,98 +8585,98 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("annotation", 0);
   __Pyx_INCREF(__pyx_v_y);
   __Pyx_INCREF(__pyx_v_annotation_type);
 
-  /* "pyjls/binding.pyx":375
+  /* "pyjls/binding.pyx":376
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):
  *         cdef int32_t rc
  *         if isinstance(annotation_type, str):             # <<<<<<<<<<<<<<
  *             annotation_type = _annotation_map[annotation_type.lower()]
  *         storage_type, payload, payload_length = _storage_pack(data)
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_annotation_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":376
+    /* "pyjls/binding.pyx":377
  *         cdef int32_t rc
  *         if isinstance(annotation_type, str):
  *             annotation_type = _annotation_map[annotation_type.lower()]             # <<<<<<<<<<<<<<
  *         storage_type, payload, payload_length = _storage_pack(data)
  *         if y is None or not np.isfinite(y):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_annotation_map); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 376, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_annotation_map); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_annotation_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_annotation_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_annotation_type, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":375
+    /* "pyjls/binding.pyx":376
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):
  *         cdef int32_t rc
  *         if isinstance(annotation_type, str):             # <<<<<<<<<<<<<<
  *             annotation_type = _annotation_map[annotation_type.lower()]
  *         storage_type, payload, payload_length = _storage_pack(data)
  */
   }
 
-  /* "pyjls/binding.pyx":377
+  /* "pyjls/binding.pyx":378
  *         if isinstance(annotation_type, str):
  *             annotation_type = _annotation_map[annotation_type.lower()]
  *         storage_type, payload, payload_length = _storage_pack(data)             # <<<<<<<<<<<<<<
  *         if y is None or not np.isfinite(y):
  *             y = NAN
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
     PyObject* sequence = __pyx_t_5;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 377, __pyx_L1_error)
+      __PYX_ERR(0, 378, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_6 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -8671,157 +8684,157 @@
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_6 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_6);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L1_error)
+    __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     #endif
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_7 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 377, __pyx_L1_error)
+    __pyx_t_7 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
     index = 0; __pyx_t_4 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_4)) goto __pyx_L4_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
     index = 1; __pyx_t_3 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_3)) goto __pyx_L4_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 2; __pyx_t_6 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_6)) goto __pyx_L4_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_6);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 3) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 3) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
     __pyx_t_8 = NULL;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     goto __pyx_L5_unpacking_done;
     __pyx_L4_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 377, __pyx_L1_error)
+    __PYX_ERR(0, 378, __pyx_L1_error)
     __pyx_L5_unpacking_done:;
   }
   __pyx_v_storage_type = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_payload = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_payload_length = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "pyjls/binding.pyx":378
+  /* "pyjls/binding.pyx":379
  *             annotation_type = _annotation_map[annotation_type.lower()]
  *         storage_type, payload, payload_length = _storage_pack(data)
  *         if y is None or not np.isfinite(y):             # <<<<<<<<<<<<<<
  *             y = NAN
  *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
  */
   __pyx_t_1 = (__pyx_v_y == Py_None);
   __pyx_t_9 = (__pyx_t_1 != 0);
   if (!__pyx_t_9) {
   } else {
     __pyx_t_2 = __pyx_t_9;
     goto __pyx_L7_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_v_y) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_y);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_1 = ((!__pyx_t_9) != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":379
+    /* "pyjls/binding.pyx":380
  *         storage_type, payload, payload_length = _storage_pack(data)
  *         if y is None or not np.isfinite(y):
  *             y = NAN             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
  *             group_id, storage_type, payload, payload_length)
  */
-    __pyx_t_5 = PyFloat_FromDouble(NAN); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __pyx_t_5 = PyFloat_FromDouble(NAN); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 380, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF_SET(__pyx_v_y, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":378
+    /* "pyjls/binding.pyx":379
  *             annotation_type = _annotation_map[annotation_type.lower()]
  *         storage_type, payload, payload_length = _storage_pack(data)
  *         if y is None or not np.isfinite(y):             # <<<<<<<<<<<<<<
  *             y = NAN
  *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
  */
   }
 
-  /* "pyjls/binding.pyx":380
+  /* "pyjls/binding.pyx":381
  *         if y is None or not np.isfinite(y):
  *             y = NAN
  *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,             # <<<<<<<<<<<<<<
  *             group_id, storage_type, payload, payload_length)
  *         _handle_rc('annotation', rc)
  */
-  __pyx_t_10 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_10 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_11 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
-  __pyx_t_12 = __pyx_PyFloat_AsFloat(__pyx_v_y); if (unlikely((__pyx_t_12 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
-  __pyx_t_13 = ((enum jls_annotation_type_e)__Pyx_PyInt_As_enum__jls_annotation_type_e(__pyx_v_annotation_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_10 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_11 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_12 = __pyx_PyFloat_AsFloat(__pyx_v_y); if (unlikely((__pyx_t_12 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_13 = ((enum jls_annotation_type_e)__Pyx_PyInt_As_enum__jls_annotation_type_e(__pyx_v_annotation_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":381
+  /* "pyjls/binding.pyx":382
  *             y = NAN
  *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
  *             group_id, storage_type, payload, payload_length)             # <<<<<<<<<<<<<<
  *         _handle_rc('annotation', rc)
  * 
  */
-  __pyx_t_14 = __Pyx_PyInt_As_uint8_t(__pyx_v_group_id); if (unlikely((__pyx_t_14 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
-  __pyx_t_15 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_v_storage_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
-  __pyx_t_16 = __Pyx_PyObject_AsUString(__pyx_v_payload); if (unlikely((!__pyx_t_16) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
-  __pyx_t_17 = __Pyx_PyInt_As_uint32_t(__pyx_v_payload_length); if (unlikely((__pyx_t_17 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_As_uint8_t(__pyx_v_group_id); if (unlikely((__pyx_t_14 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_15 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_v_storage_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_AsUString(__pyx_v_payload); if (unlikely((!__pyx_t_16) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyInt_As_uint32_t(__pyx_v_payload_length); if (unlikely((__pyx_t_17 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":380
+  /* "pyjls/binding.pyx":381
  *         if y is None or not np.isfinite(y):
  *             y = NAN
  *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,             # <<<<<<<<<<<<<<
  *             group_id, storage_type, payload, payload_length)
  *         _handle_rc('annotation', rc)
  */
   __pyx_v_rc = jls_twr_annotation(__pyx_v_self->_wr, __pyx_t_10, __pyx_t_11, __pyx_t_12, __pyx_t_13, __pyx_t_14, __pyx_t_15, __pyx_t_16, __pyx_t_17);
 
-  /* "pyjls/binding.pyx":382
+  /* "pyjls/binding.pyx":383
  *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
  *             group_id, storage_type, payload, payload_length)
  *         _handle_rc('annotation', rc)             # <<<<<<<<<<<<<<
  * 
  *     def utc(self, signal_id, sample_id, utc_i64):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = NULL;
   __pyx_t_18 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -8830,49 +8843,49 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_18 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_annotation, __pyx_t_6};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 2+__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 2+__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_annotation, __pyx_t_6};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 2+__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 2+__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_annotation);
     __Pyx_GIVEREF(__pyx_n_u_annotation);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_18, __pyx_n_u_annotation);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_18, __pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":373
+  /* "pyjls/binding.pyx":374
  *         _handle_rc('fsr', rc)
  * 
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         if isinstance(annotation_type, str):
  */
 
@@ -8894,15 +8907,15 @@
   __Pyx_XDECREF(__pyx_v_y);
   __Pyx_XDECREF(__pyx_v_annotation_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":384
+/* "pyjls/binding.pyx":385
  *         _handle_rc('annotation', rc)
  * 
  *     def utc(self, signal_id, sample_id, utc_i64):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)
  */
 
@@ -8939,40 +8952,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 384, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 385, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_utc_i64)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 384, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 385, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 384, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 385, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_utc_i64 = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 384, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 385, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.utc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_26utc(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_utc_i64);
 
@@ -8995,36 +9008,36 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("utc", 0);
 
-  /* "pyjls/binding.pyx":386
+  /* "pyjls/binding.pyx":387
  *     def utc(self, signal_id, sample_id, utc_i64):
  *         cdef int32_t rc
  *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)             # <<<<<<<<<<<<<<
  *         _handle_rc('utc', rc)
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_As_int64_t(__pyx_v_utc_i64); if (unlikely((__pyx_t_3 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int64_t(__pyx_v_utc_i64); if (unlikely((__pyx_t_3 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
   __pyx_v_rc = jls_twr_utc(__pyx_v_self->_wr, __pyx_t_1, __pyx_t_2, __pyx_t_3);
 
-  /* "pyjls/binding.pyx":387
+  /* "pyjls/binding.pyx":388
  *         cdef int32_t rc
  *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)
  *         _handle_rc('utc', rc)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -9033,49 +9046,49 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_utc, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_utc, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_utc);
     __Pyx_GIVEREF(__pyx_n_u_utc);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_n_u_utc);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":384
+  /* "pyjls/binding.pyx":385
  *         _handle_rc('annotation', rc)
  * 
  *     def utc(self, signal_id, sample_id, utc_i64):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)
  */
 
@@ -9205,15 +9218,15 @@
   __Pyx_AddTraceback("pyjls.binding.Writer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":394
+/* "pyjls/binding.pyx":395
  *     cdef object cbk_fn
  * 
  *     def __init__(self, is_fsr, cbk_fn):             # <<<<<<<<<<<<<<
  *         self.is_fsr = is_fsr
  *         self.cbk_fn = cbk_fn
  */
 
@@ -9247,32 +9260,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_is_fsr)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cbk_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 394, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 395, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 394, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 395, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_is_fsr = values[0];
     __pyx_v_cbk_fn = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 394, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 395, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.AnnotationCallback.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_18AnnotationCallback___init__(((struct __pyx_obj_5pyjls_7binding_AnnotationCallback *)__pyx_v_self), __pyx_v_is_fsr, __pyx_v_cbk_fn);
 
@@ -9286,38 +9299,38 @@
   __Pyx_RefNannyDeclarations
   uint8_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyjls/binding.pyx":395
+  /* "pyjls/binding.pyx":396
  * 
  *     def __init__(self, is_fsr, cbk_fn):
  *         self.is_fsr = is_fsr             # <<<<<<<<<<<<<<
  *         self.cbk_fn = cbk_fn
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_is_fsr); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 395, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_is_fsr); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L1_error)
   __pyx_v_self->is_fsr = __pyx_t_1;
 
-  /* "pyjls/binding.pyx":396
+  /* "pyjls/binding.pyx":397
  *     def __init__(self, is_fsr, cbk_fn):
  *         self.is_fsr = is_fsr
  *         self.cbk_fn = cbk_fn             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __Pyx_GIVEREF(__pyx_v_cbk_fn);
   __Pyx_GOTREF(__pyx_v_self->cbk_fn);
   __Pyx_DECREF(__pyx_v_self->cbk_fn);
   __pyx_v_self->cbk_fn = __pyx_v_cbk_fn;
 
-  /* "pyjls/binding.pyx":394
+  /* "pyjls/binding.pyx":395
  *     cdef object cbk_fn
  * 
  *     def __init__(self, is_fsr, cbk_fn):             # <<<<<<<<<<<<<<
  *         self.is_fsr = is_fsr
  *         self.cbk_fn = cbk_fn
  */
 
@@ -9626,15 +9639,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":404
+/* "pyjls/binding.pyx":405
  *     cdef object _signals
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s * sources
  */
 
@@ -9663,32 +9676,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 404, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 405, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_path = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 404, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 405, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 404, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 405, __pyx_L1_error)
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader___init__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -9728,71 +9741,71 @@
   char const *__pyx_t_18;
   int __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyjls/binding.pyx":410
+  /* "pyjls/binding.pyx":411
  *         cdef uint16_t count
  *         cdef int64_t samples
  *         self._sources: Mapping[int, SourceDef] = {}             # <<<<<<<<<<<<<<
  *         self._signals: Mapping[int, SignalDef] = {}
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_sources);
   __Pyx_DECREF(__pyx_v_self->_sources);
   __pyx_v_self->_sources = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":411
+  /* "pyjls/binding.pyx":412
  *         cdef int64_t samples
  *         self._sources: Mapping[int, SourceDef] = {}
  *         self._signals: Mapping[int, SignalDef] = {}             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))
  *         _handle_rc('open', rc)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_signals);
   __Pyx_DECREF(__pyx_v_self->_signals);
   __pyx_v_self->_signals = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":412
+  /* "pyjls/binding.pyx":413
  *         self._sources: Mapping[int, SourceDef] = {}
  *         self._signals: Mapping[int, SignalDef] = {}
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))             # <<<<<<<<<<<<<<
  *         _handle_rc('open', rc)
  * 
  */
   if (unlikely(__pyx_v_path == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 412, __pyx_L1_error)
+    __PYX_ERR(0, 413, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L1_error)
   __pyx_v_rc = jls_rd_open((&__pyx_v_self->_rd), __pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":413
+  /* "pyjls/binding.pyx":414
  *         self._signals: Mapping[int, SignalDef] = {}
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))
  *         _handle_rc('open', rc)             # <<<<<<<<<<<<<<
  * 
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9801,67 +9814,67 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_open);
     __Pyx_GIVEREF(__pyx_n_u_open);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_u_open);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":415
+  /* "pyjls/binding.pyx":416
  *         _handle_rc('open', rc)
  * 
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):
  */
   __pyx_v_rc = jls_rd_sources(__pyx_v_self->_rd, (&__pyx_v_sources), (&__pyx_v_count));
 
-  /* "pyjls/binding.pyx":416
+  /* "pyjls/binding.pyx":417
  * 
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)
  *         _handle_rc('rd_sources', rc)             # <<<<<<<<<<<<<<
  *         for i in range(count):
  *             source_def = SourceDef(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9870,192 +9883,192 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_sources, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_sources, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_sources);
     __Pyx_GIVEREF(__pyx_n_u_rd_sources);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_n_u_rd_sources);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_t_7);
     __pyx_t_7 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":417
+  /* "pyjls/binding.pyx":418
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):             # <<<<<<<<<<<<<<
  *             source_def = SourceDef(
  *                 source_id=sources[i].source_id,
  */
   __pyx_t_8 = __pyx_v_count;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pyjls/binding.pyx":418
+    /* "pyjls/binding.pyx":419
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):
  *             source_def = SourceDef(             # <<<<<<<<<<<<<<
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SourceDef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SourceDef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "pyjls/binding.pyx":419
+    /* "pyjls/binding.pyx":420
  *         for i in range(count):
  *             source_def = SourceDef(
  *                 source_id=sources[i].source_id,             # <<<<<<<<<<<<<<
  *                 name=sources[i].name.decode('utf-8'),
  *                 vendor=sources[i].vendor.decode('utf-8'),
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyInt_From_uint16_t((__pyx_v_sources[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint16_t((__pyx_v_sources[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":420
+    /* "pyjls/binding.pyx":421
  *             source_def = SourceDef(
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 vendor=sources[i].vendor.decode('utf-8'),
  *                 model=sources[i].model.decode('utf-8'),
  */
     __pyx_t_11 = (__pyx_v_sources[__pyx_v_i]).name;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_11, 0, strlen(__pyx_t_11), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_11, 0, strlen(__pyx_t_11), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":421
+    /* "pyjls/binding.pyx":422
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),
  *                 vendor=sources[i].vendor.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 model=sources[i].model.decode('utf-8'),
  *                 version=sources[i].version.decode('utf-8'),
  */
     __pyx_t_12 = (__pyx_v_sources[__pyx_v_i]).vendor;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_12, 0, strlen(__pyx_t_12), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_12, 0, strlen(__pyx_t_12), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vendor, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vendor, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":422
+    /* "pyjls/binding.pyx":423
  *                 name=sources[i].name.decode('utf-8'),
  *                 vendor=sources[i].vendor.decode('utf-8'),
  *                 model=sources[i].model.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 version=sources[i].version.decode('utf-8'),
  *                 serial_number=sources[i].serial_number.decode('utf-8'))
  */
     __pyx_t_13 = (__pyx_v_sources[__pyx_v_i]).model;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_13, 0, strlen(__pyx_t_13), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_13, 0, strlen(__pyx_t_13), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":423
+    /* "pyjls/binding.pyx":424
  *                 vendor=sources[i].vendor.decode('utf-8'),
  *                 model=sources[i].model.decode('utf-8'),
  *                 version=sources[i].version.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 serial_number=sources[i].serial_number.decode('utf-8'))
  *             self._sources[sources[i].source_id] = source_def
  */
     __pyx_t_14 = (__pyx_v_sources[__pyx_v_i]).version;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_14, 0, strlen(__pyx_t_14), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 423, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_14, 0, strlen(__pyx_t_14), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_version, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_version, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":424
+    /* "pyjls/binding.pyx":425
  *                 model=sources[i].model.decode('utf-8'),
  *                 version=sources[i].version.decode('utf-8'),
  *                 serial_number=sources[i].serial_number.decode('utf-8'))             # <<<<<<<<<<<<<<
  *             self._sources[sources[i].source_id] = source_def
  * 
  */
     __pyx_t_15 = (__pyx_v_sources[__pyx_v_i]).serial_number;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_15, 0, strlen(__pyx_t_15), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 424, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_15, 0, strlen(__pyx_t_15), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_serial_number, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_serial_number, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":418
+    /* "pyjls/binding.pyx":419
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):
  *             source_def = SourceDef(             # <<<<<<<<<<<<<<
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_source_def, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":425
+    /* "pyjls/binding.pyx":426
  *                 version=sources[i].version.decode('utf-8'),
  *                 serial_number=sources[i].serial_number.decode('utf-8'))
  *             self._sources[sources[i].source_id] = source_def             # <<<<<<<<<<<<<<
  * 
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)
  */
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_sources, (__pyx_v_sources[__pyx_v_i]).source_id, __pyx_v_source_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 425, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_sources, (__pyx_v_sources[__pyx_v_i]).source_id, __pyx_v_source_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 426, __pyx_L1_error)
   }
 
-  /* "pyjls/binding.pyx":427
+  /* "pyjls/binding.pyx":428
  *             self._sources[sources[i].source_id] = source_def
  * 
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_signals', rc)
  *         for i in range(count):
  */
   __pyx_v_rc = jls_rd_signals(__pyx_v_self->_rd, (&__pyx_v_signals), (&__pyx_v_count));
 
-  /* "pyjls/binding.pyx":428
+  /* "pyjls/binding.pyx":429
  * 
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)
  *         _handle_rc('rd_signals', rc)             # <<<<<<<<<<<<<<
  *         for i in range(count):
  *             signal_id = signals[i].signal_id
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -10064,291 +10077,303 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_rd_signals, __pyx_t_1};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 429, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_rd_signals, __pyx_t_1};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 429, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 429, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_signals);
     __Pyx_GIVEREF(__pyx_n_u_rd_signals);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_n_u_rd_signals);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 429, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":429
+  /* "pyjls/binding.pyx":430
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)
  *         _handle_rc('rd_signals', rc)
  *         for i in range(count):             # <<<<<<<<<<<<<<
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(
  */
   __pyx_t_8 = __pyx_v_count;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pyjls/binding.pyx":430
+    /* "pyjls/binding.pyx":431
  *         _handle_rc('rd_signals', rc)
  *         for i in range(count):
  *             signal_id = signals[i].signal_id             # <<<<<<<<<<<<<<
  *             signal_def = SignalDef(
  *                 signal_id=signal_id,
  */
     __pyx_t_16 = (__pyx_v_signals[__pyx_v_i]).signal_id;
     __pyx_v_signal_id = __pyx_t_16;
 
-    /* "pyjls/binding.pyx":431
+    /* "pyjls/binding.pyx":432
  *         for i in range(count):
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(             # <<<<<<<<<<<<<<
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SignalDef); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 431, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SignalDef); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "pyjls/binding.pyx":432
+    /* "pyjls/binding.pyx":433
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(
  *                 signal_id=signal_id,             # <<<<<<<<<<<<<<
  *                 source_id=signals[i].source_id,
  *                 signal_type=signals[i].signal_type,
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(14); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_signal_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_signal_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_id, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_id, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":433
+    /* "pyjls/binding.pyx":434
  *             signal_def = SignalDef(
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,             # <<<<<<<<<<<<<<
  *                 signal_type=signals[i].signal_type,
  *                 data_type=signals[i].data_type,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t((__pyx_v_signals[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t((__pyx_v_signals[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 434, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":434
+    /* "pyjls/binding.pyx":435
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,
  *                 signal_type=signals[i].signal_type,             # <<<<<<<<<<<<<<
  *                 data_type=signals[i].data_type,
  *                 sample_rate=signals[i].sample_rate,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_signals[__pyx_v_i]).signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 434, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_signals[__pyx_v_i]).signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":435
+    /* "pyjls/binding.pyx":436
  *                 source_id=signals[i].source_id,
  *                 signal_type=signals[i].signal_type,
  *                 data_type=signals[i].data_type,             # <<<<<<<<<<<<<<
  *                 sample_rate=signals[i].sample_rate,
  *                 samples_per_data=signals[i].samples_per_data,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":436
+    /* "pyjls/binding.pyx":437
  *                 signal_type=signals[i].signal_type,
  *                 data_type=signals[i].data_type,
  *                 sample_rate=signals[i].sample_rate,             # <<<<<<<<<<<<<<
  *                 samples_per_data=signals[i].samples_per_data,
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":437
+    /* "pyjls/binding.pyx":438
  *                 data_type=signals[i].data_type,
  *                 sample_rate=signals[i].sample_rate,
  *                 samples_per_data=signals[i].samples_per_data,             # <<<<<<<<<<<<<<
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  *                 entries_per_summary=signals[i].entries_per_summary,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":438
+    /* "pyjls/binding.pyx":439
  *                 sample_rate=signals[i].sample_rate,
  *                 samples_per_data=signals[i].samples_per_data,
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,             # <<<<<<<<<<<<<<
  *                 entries_per_summary=signals[i].entries_per_summary,
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":439
+    /* "pyjls/binding.pyx":440
  *                 samples_per_data=signals[i].samples_per_data,
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  *                 entries_per_summary=signals[i].entries_per_summary,             # <<<<<<<<<<<<<<
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":440
+    /* "pyjls/binding.pyx":441
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  *                 entries_per_summary=signals[i].entries_per_summary,
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,             # <<<<<<<<<<<<<<
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 441, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":441
+    /* "pyjls/binding.pyx":442
  *                 entries_per_summary=signals[i].entries_per_summary,
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,             # <<<<<<<<<<<<<<
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,
- *                 name=signals[i].name.decode('utf-8'),
+ *                 sample_id_offset=signals[i].sample_id_offset,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":442
+    /* "pyjls/binding.pyx":443
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,             # <<<<<<<<<<<<<<
+ *                 sample_id_offset=signals[i].sample_id_offset,
  *                 name=signals[i].name.decode('utf-8'),
- *                 units=signals[i].units.decode('utf-8'))
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 443, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":443
+    /* "pyjls/binding.pyx":444
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,
+ *                 sample_id_offset=signals[i].sample_id_offset,             # <<<<<<<<<<<<<<
+ *                 name=signals[i].name.decode('utf-8'),
+ *                 units=signals[i].units.decode('utf-8'))
+ */
+    __pyx_t_4 = __Pyx_PyInt_From_int64_t((__pyx_v_signals[__pyx_v_i]).sample_id_offset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_id_offset, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "pyjls/binding.pyx":445
+ *                 utc_decimate_factor=signals[i].utc_decimate_factor,
+ *                 sample_id_offset=signals[i].sample_id_offset,
  *                 name=signals[i].name.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  */
     __pyx_t_17 = (__pyx_v_signals[__pyx_v_i]).name;
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_17, 0, strlen(__pyx_t_17), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_17, 0, strlen(__pyx_t_17), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 445, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":444
- *                 utc_decimate_factor=signals[i].utc_decimate_factor,
+    /* "pyjls/binding.pyx":446
+ *                 sample_id_offset=signals[i].sample_id_offset,
  *                 name=signals[i].name.decode('utf-8'),
  *                 units=signals[i].units.decode('utf-8'))             # <<<<<<<<<<<<<<
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  */
     __pyx_t_18 = (__pyx_v_signals[__pyx_v_i]).units;
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_18, 0, strlen(__pyx_t_18), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_18, 0, strlen(__pyx_t_18), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":431
+    /* "pyjls/binding.pyx":432
  *         for i in range(count):
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(             # <<<<<<<<<<<<<<
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 431, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_signal_def, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":445
+    /* "pyjls/binding.pyx":447
  *                 name=signals[i].name.decode('utf-8'),
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:             # <<<<<<<<<<<<<<
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_signal_def, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_signal_def, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_19 < 0)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_19 < 0)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (__pyx_t_19) {
 
-      /* "pyjls/binding.pyx":446
+      /* "pyjls/binding.pyx":448
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)             # <<<<<<<<<<<<<<
  *                 _handle_rc('rd_fsr_length', rc)
  *                 signal_def.length = samples
  */
       __pyx_v_rc = jls_rd_fsr_length(__pyx_v_self->_rd, __pyx_v_signal_id, (&__pyx_v_samples));
 
-      /* "pyjls/binding.pyx":447
+      /* "pyjls/binding.pyx":449
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)             # <<<<<<<<<<<<<<
  *                 signal_def.length = samples
  *             self._signals[signal_id] = signal_def
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_1 = NULL;
       __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -10357,80 +10382,80 @@
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_6 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_n_u_rd_fsr_length, __pyx_t_4};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_n_u_rd_fsr_length, __pyx_t_4};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else
       #endif
       {
-        __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 447, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 449, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         if (__pyx_t_1) {
           __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1); __pyx_t_1 = NULL;
         }
         __Pyx_INCREF(__pyx_n_u_rd_fsr_length);
         __Pyx_GIVEREF(__pyx_n_u_rd_fsr_length);
         PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_u_rd_fsr_length);
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
         __pyx_t_4 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "pyjls/binding.pyx":448
+      /* "pyjls/binding.pyx":450
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)
  *                 signal_def.length = samples             # <<<<<<<<<<<<<<
  *             self._signals[signal_id] = signal_def
  * 
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_samples); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 448, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_samples); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 450, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_PyObject_SetAttrStr(__pyx_v_signal_def, __pyx_n_s_length, __pyx_t_5) < 0) __PYX_ERR(0, 448, __pyx_L1_error)
+      if (__Pyx_PyObject_SetAttrStr(__pyx_v_signal_def, __pyx_n_s_length, __pyx_t_5) < 0) __PYX_ERR(0, 450, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "pyjls/binding.pyx":445
+      /* "pyjls/binding.pyx":447
  *                 name=signals[i].name.decode('utf-8'),
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:             # <<<<<<<<<<<<<<
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)
  */
     }
 
-    /* "pyjls/binding.pyx":449
+    /* "pyjls/binding.pyx":451
  *                 _handle_rc('rd_fsr_length', rc)
  *                 signal_def.length = samples
  *             self._signals[signal_id] = signal_def             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_signals, __pyx_v_signal_id, __pyx_v_signal_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 449, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_signals, __pyx_v_signal_id, __pyx_v_signal_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 451, __pyx_L1_error)
   }
 
-  /* "pyjls/binding.pyx":404
+  /* "pyjls/binding.pyx":405
  *     cdef object _signals
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s * sources
  */
 
@@ -10448,15 +10473,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_source_def);
   __Pyx_XDECREF(__pyx_v_signal_def);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":451
+/* "pyjls/binding.pyx":453
  *             self._signals[signal_id] = signal_def
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -10474,42 +10499,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_2__enter__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "pyjls/binding.pyx":452
+  /* "pyjls/binding.pyx":454
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, type, value, traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":451
+  /* "pyjls/binding.pyx":453
  *             self._signals[signal_id] = signal_def
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":454
+/* "pyjls/binding.pyx":456
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -10546,40 +10571,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 454, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 456, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_traceback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 454, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 456, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 454, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 456, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_type = values[0];
     __pyx_v_value = values[1];
     __pyx_v_traceback = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 454, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 456, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_4__exit__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_type, __pyx_v_value, __pyx_v_traceback);
 
@@ -10595,41 +10620,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "pyjls/binding.pyx":455
+  /* "pyjls/binding.pyx":457
  * 
  *     def __exit__(self, type, value, traceback):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":454
+  /* "pyjls/binding.pyx":456
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -10644,15 +10669,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":457
+/* "pyjls/binding.pyx":459
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_rd_close(self._rd)
  * 
  */
 
@@ -10670,39 +10695,39 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_6close(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "pyjls/binding.pyx":458
+  /* "pyjls/binding.pyx":460
  * 
  *     def close(self):
  *         c_jls.jls_rd_close(self._rd)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   jls_rd_close(__pyx_v_self->_rd);
 
-  /* "pyjls/binding.pyx":457
+  /* "pyjls/binding.pyx":459
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_rd_close(self._rd)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":461
+/* "pyjls/binding.pyx":463
  * 
  *     @property
  *     def sources(self) -> Mapping[int, SourceDef]:             # <<<<<<<<<<<<<<
  *         return self._sources
  * 
  */
 
@@ -10720,42 +10745,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_7sources___get__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyjls/binding.pyx":462
+  /* "pyjls/binding.pyx":464
  *     @property
  *     def sources(self) -> Mapping[int, SourceDef]:
  *         return self._sources             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_sources);
   __pyx_r = __pyx_v_self->_sources;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":461
+  /* "pyjls/binding.pyx":463
  * 
  *     @property
  *     def sources(self) -> Mapping[int, SourceDef]:             # <<<<<<<<<<<<<<
  *         return self._sources
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":465
+/* "pyjls/binding.pyx":467
  * 
  *     @property
  *     def signals(self) -> Mapping[int, SignalDef]:             # <<<<<<<<<<<<<<
  *         return self._signals
  * 
  */
 
@@ -10773,42 +10798,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_7signals___get__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyjls/binding.pyx":466
+  /* "pyjls/binding.pyx":468
  *     @property
  *     def signals(self) -> Mapping[int, SignalDef]:
  *         return self._signals             # <<<<<<<<<<<<<<
  * 
  *     def fsr(self, signal_id, start_sample_id, length):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_signals);
   __pyx_r = __pyx_v_self->_signals;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":465
+  /* "pyjls/binding.pyx":467
  * 
  *     @property
  *     def signals(self) -> Mapping[int, SignalDef]:             # <<<<<<<<<<<<<<
  *         return self._signals
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":468
+/* "pyjls/binding.pyx":470
  *         return self._signals
  * 
  *     def fsr(self, signal_id, start_sample_id, length):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef np.uint8_t [::1] u8
  */
 
@@ -10845,40 +10870,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 468, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 470, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_length)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 468, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 470, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 468, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 470, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_start_sample_id = values[1];
     __pyx_v_length = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 468, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 470, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.fsr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_8fsr(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_start_sample_id, __pyx_v_length);
 
@@ -10914,271 +10939,271 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr", 0);
 
-  /* "pyjls/binding.pyx":474
+  /* "pyjls/binding.pyx":476
  *         cdef uint32_t entry_size_bits
  *         cdef uint32_t u8_length
  *         cdef uint16_t signal_id_u16 = signal_id             # <<<<<<<<<<<<<<
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t length_i64 = length
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 476, __pyx_L1_error)
   __pyx_v_signal_id_u16 = __pyx_t_1;
 
-  /* "pyjls/binding.pyx":475
+  /* "pyjls/binding.pyx":477
  *         cdef uint32_t u8_length
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id             # <<<<<<<<<<<<<<
  *         cdef int64_t length_i64 = length
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 477, __pyx_L1_error)
   __pyx_v_start_sample_id_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":476
+  /* "pyjls/binding.pyx":478
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t length_i64 = length             # <<<<<<<<<<<<<<
  * 
  *         data_type = self._signals[signal_id].data_type
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 478, __pyx_L1_error)
   __pyx_v_length_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":478
+  /* "pyjls/binding.pyx":480
  *         cdef int64_t length_i64 = length
  * 
  *         data_type = self._signals[signal_id].data_type             # <<<<<<<<<<<<<<
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_data_type = __pyx_t_5;
 
-  /* "pyjls/binding.pyx":479
+  /* "pyjls/binding.pyx":481
  * 
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff             # <<<<<<<<<<<<<<
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length
  */
   __pyx_v_entry_size_bits = ((__pyx_v_data_type >> 8) & 0xff);
 
-  /* "pyjls/binding.pyx":480
+  /* "pyjls/binding.pyx":482
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]             # <<<<<<<<<<<<<<
  *         u8_length = length
  *         if entry_size_bits == 4:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 482, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = (__pyx_v_data_type & 0xffff);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_np_type = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":481
+  /* "pyjls/binding.pyx":483
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length             # <<<<<<<<<<<<<<
  *         if entry_size_bits == 4:
  *             u8_length = (length + 1) // 2
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_length); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_length); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L1_error)
   __pyx_v_u8_length = __pyx_t_5;
 
-  /* "pyjls/binding.pyx":482
+  /* "pyjls/binding.pyx":484
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:
  */
   switch (__pyx_v_entry_size_bits) {
     case 4:
 
-    /* "pyjls/binding.pyx":483
+    /* "pyjls/binding.pyx":485
  *         u8_length = length
  *         if entry_size_bits == 4:
  *             u8_length = (length + 1) // 2             # <<<<<<<<<<<<<<
  *         elif entry_size_bits == 1:
  *             u8_length = (length + 7) // 8
  */
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_3, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_3, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 485, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 485, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_u8_length = __pyx_t_5;
 
-    /* "pyjls/binding.pyx":482
+    /* "pyjls/binding.pyx":484
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:
  */
     break;
     case 1:
 
-    /* "pyjls/binding.pyx":485
+    /* "pyjls/binding.pyx":487
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:
  *             u8_length = (length + 7) // 8             # <<<<<<<<<<<<<<
  *         else:
  *             u8_length *= entry_size_bits // 8
  */
-    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_7, 7, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 485, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_7, 7, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_4, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_4, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 485, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_u8_length = __pyx_t_5;
 
-    /* "pyjls/binding.pyx":484
+    /* "pyjls/binding.pyx":486
  *         if entry_size_bits == 4:
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:             # <<<<<<<<<<<<<<
  *             u8_length = (length + 7) // 8
  *         else:
  */
     break;
     default:
 
-    /* "pyjls/binding.pyx":487
+    /* "pyjls/binding.pyx":489
  *             u8_length = (length + 7) // 8
  *         else:
  *             u8_length *= entry_size_bits // 8             # <<<<<<<<<<<<<<
  * 
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)
  */
     __pyx_v_u8_length = (__pyx_v_u8_length * __Pyx_div_long(__pyx_v_entry_size_bits, 8));
     break;
   }
 
-  /* "pyjls/binding.pyx":489
+  /* "pyjls/binding.pyx":491
  *             u8_length *= entry_size_bits // 8
  * 
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)             # <<<<<<<<<<<<<<
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_u8_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_u8_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 489, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data_u8 = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "pyjls/binding.pyx":490
+  /* "pyjls/binding.pyx":492
  * 
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)
  *         data = data_u8.view(dtype=np_type)             # <<<<<<<<<<<<<<
  *         u8 = data_u8
  *         with nogil:
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_u8, __pyx_n_s_view); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_u8, __pyx_n_s_view); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_v_np_type) < 0) __PYX_ERR(0, 490, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 490, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_v_np_type) < 0) __PYX_ERR(0, 492, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":491
+  /* "pyjls/binding.pyx":493
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  */
-  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 493, __pyx_L1_error)
   __pyx_v_u8 = __pyx_t_10;
   __pyx_t_10.memview = NULL;
   __pyx_t_10.data = NULL;
 
-  /* "pyjls/binding.pyx":492
+  /* "pyjls/binding.pyx":494
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjls/binding.pyx":493
+        /* "pyjls/binding.pyx":495
  *         u8 = data_u8
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_fsr', rc)
  *         return data
  */
         __pyx_t_11 = 0;
         __pyx_t_12 = -1;
         if (__pyx_t_11 < 0) {
           __pyx_t_11 += __pyx_v_u8.shape[0];
           if (unlikely(__pyx_t_11 < 0)) __pyx_t_12 = 0;
         } else if (unlikely(__pyx_t_11 >= __pyx_v_u8.shape[0])) __pyx_t_12 = 0;
         if (unlikely(__pyx_t_12 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_12);
-          __PYX_ERR(0, 493, __pyx_L4_error)
+          __PYX_ERR(0, 495, __pyx_L4_error)
         }
         __pyx_v_rc = jls_rd_fsr(__pyx_v_self->_rd, __pyx_v_signal_id_u16, __pyx_v_start_sample_id_i64, (&(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_u8.data) + __pyx_t_11)) )))), __pyx_v_length_i64);
       }
 
-      /* "pyjls/binding.pyx":492
+      /* "pyjls/binding.pyx":494
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)
  */
       /*finally:*/ {
@@ -11196,24 +11221,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjls/binding.pyx":494
+  /* "pyjls/binding.pyx":496
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_9 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_4 = NULL;
   __pyx_t_12 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11222,61 +11247,61 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_12 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr, __pyx_t_9};
-    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr, __pyx_t_9};
-    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_fsr);
     __Pyx_GIVEREF(__pyx_n_u_rd_fsr);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_12, __pyx_n_u_rd_fsr);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_12, __pyx_t_9);
     __pyx_t_9 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":495
+  /* "pyjls/binding.pyx":497
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def fsr_statistics(self, signal_id, start_sample_id, increment, length):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":468
+  /* "pyjls/binding.pyx":470
  *         return self._signals
  * 
  *     def fsr(self, signal_id, start_sample_id, length):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef np.uint8_t [::1] u8
  */
 
@@ -11296,15 +11321,15 @@
   __Pyx_XDECREF(__pyx_v_data_u8);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":497
+/* "pyjls/binding.pyx":499
  *         return data
  * 
  *     def fsr_statistics(self, signal_id, start_sample_id, increment, length):             # <<<<<<<<<<<<<<
  *         """Read FSR statistics.
  * 
  */
 
@@ -11345,31 +11370,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 1); __PYX_ERR(0, 497, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 1); __PYX_ERR(0, 499, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_increment)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 2); __PYX_ERR(0, 497, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 2); __PYX_ERR(0, 499, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_length)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 3); __PYX_ERR(0, 497, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 3); __PYX_ERR(0, 499, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_statistics") < 0)) __PYX_ERR(0, 497, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_statistics") < 0)) __PYX_ERR(0, 499, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -11378,15 +11403,15 @@
     __pyx_v_signal_id = values[0];
     __pyx_v_start_sample_id = values[1];
     __pyx_v_increment = values[2];
     __pyx_v_length = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 497, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 499, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.fsr_statistics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_10fsr_statistics(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_start_sample_id, __pyx_v_increment, __pyx_v_length);
 
@@ -11417,126 +11442,126 @@
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr_statistics", 0);
 
-  /* "pyjls/binding.pyx":509
+  /* "pyjls/binding.pyx":511
  *         cdef int32_t rc
  *         cdef np.float64_t [:, :] c_data
  *         cdef uint16_t signal_id_u16 = signal_id             # <<<<<<<<<<<<<<
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t increment_i64 = increment
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 511, __pyx_L1_error)
   __pyx_v_signal_id_u16 = __pyx_t_1;
 
-  /* "pyjls/binding.pyx":510
+  /* "pyjls/binding.pyx":512
  *         cdef np.float64_t [:, :] c_data
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id             # <<<<<<<<<<<<<<
  *         cdef int64_t increment_i64 = increment
  *         cdef int64_t length_i64 = length
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L1_error)
   __pyx_v_start_sample_id_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":511
+  /* "pyjls/binding.pyx":513
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t increment_i64 = increment             # <<<<<<<<<<<<<<
  *         cdef int64_t length_i64 = length
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_increment); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_increment); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L1_error)
   __pyx_v_increment_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":512
+  /* "pyjls/binding.pyx":514
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t increment_i64 = increment
  *         cdef int64_t length_i64 = length             # <<<<<<<<<<<<<<
  * 
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 514, __pyx_L1_error)
   __pyx_v_length_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":514
+  /* "pyjls/binding.pyx":516
  *         cdef int64_t length_i64 = length
  * 
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)             # <<<<<<<<<<<<<<
  *         c_data = data
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_COUNT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_COUNT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_length);
   __Pyx_GIVEREF(__pyx_v_length);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_length);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 514, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_data = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":515
+  /* "pyjls/binding.pyx":517
  * 
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  *         c_data = data             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  */
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5numpy_float64_t(__pyx_v_data, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5numpy_float64_t(__pyx_v_data, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 517, __pyx_L1_error)
   __pyx_v_c_data = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
-  /* "pyjls/binding.pyx":516
+  /* "pyjls/binding.pyx":518
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  *         c_data = data
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjls/binding.pyx":518
+        /* "pyjls/binding.pyx":520
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_fsr_statistics', rc)
  *         return data
  */
         __pyx_t_9 = 0;
@@ -11548,28 +11573,28 @@
         } else if (unlikely(__pyx_t_9 >= __pyx_v_c_data.shape[0])) __pyx_t_11 = 0;
         if (__pyx_t_10 < 0) {
           __pyx_t_10 += __pyx_v_c_data.shape[1];
           if (unlikely(__pyx_t_10 < 0)) __pyx_t_11 = 1;
         } else if (unlikely(__pyx_t_10 >= __pyx_v_c_data.shape[1])) __pyx_t_11 = 1;
         if (unlikely(__pyx_t_11 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_11);
-          __PYX_ERR(0, 518, __pyx_L4_error)
+          __PYX_ERR(0, 520, __pyx_L4_error)
         }
 
-        /* "pyjls/binding.pyx":517
+        /* "pyjls/binding.pyx":519
  *         c_data = data
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,             # <<<<<<<<<<<<<<
  *                                              increment_i64, &c_data[0, 0], length_i64)
  *         _handle_rc('rd_fsr_statistics', rc)
  */
         __pyx_v_rc = jls_rd_fsr_statistics(__pyx_v_self->_rd, __pyx_v_signal_id_u16, __pyx_v_start_sample_id_i64, __pyx_v_increment_i64, (&(*((__pyx_t_5numpy_float64_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_c_data.data + __pyx_t_9 * __pyx_v_c_data.strides[0]) ) + __pyx_t_10 * __pyx_v_c_data.strides[1]) )))), __pyx_v_length_i64);
       }
 
-      /* "pyjls/binding.pyx":516
+      /* "pyjls/binding.pyx":518
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  *         c_data = data
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)
  */
       /*finally:*/ {
@@ -11587,24 +11612,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjls/binding.pyx":519
+  /* "pyjls/binding.pyx":521
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)
  *         _handle_rc('rd_fsr_statistics', rc)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -11613,61 +11638,61 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr_statistics, __pyx_t_3};
-    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr_statistics, __pyx_t_3};
-    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_fsr_statistics);
     __Pyx_GIVEREF(__pyx_n_u_rd_fsr_statistics);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_11, __pyx_n_u_rd_fsr_statistics);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_11, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":520
+  /* "pyjls/binding.pyx":522
  *                                              increment_i64, &c_data[0, 0], length_i64)
  *         _handle_rc('rd_fsr_statistics', rc)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def annotations(self, signal_id, timestamp, cbk_fn):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":497
+  /* "pyjls/binding.pyx":499
  *         return data
  * 
  *     def fsr_statistics(self, signal_id, start_sample_id, increment, length):             # <<<<<<<<<<<<<<
  *         """Read FSR statistics.
  * 
  */
 
@@ -11685,15 +11710,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_c_data, 1);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":522
+/* "pyjls/binding.pyx":524
  *         return data
  * 
  *     def annotations(self, signal_id, timestamp, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read annotations from a signal.
  * 
  */
 
@@ -11731,40 +11756,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timestamp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 1); __PYX_ERR(0, 522, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 1); __PYX_ERR(0, 524, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cbk_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 2); __PYX_ERR(0, 522, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 2); __PYX_ERR(0, 524, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotations") < 0)) __PYX_ERR(0, 522, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotations") < 0)) __PYX_ERR(0, 524, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_timestamp = values[1];
     __pyx_v_cbk_fn = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 522, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 524, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.annotations", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_12annotations(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_timestamp, __pyx_v_cbk_fn);
 
@@ -11788,76 +11813,76 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("annotations", 0);
 
-  /* "pyjls/binding.pyx":532
+  /* "pyjls/binding.pyx":534
  *         """
  *         cdef int32_t rc
  *         is_fsr = self._signals[signal_id].signal_type == c_jls.JLS_SIGNAL_TYPE_FSR             # <<<<<<<<<<<<<<
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 534, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 534, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 534, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 534, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_is_fsr = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":533
+  /* "pyjls/binding.pyx":535
  *         cdef int32_t rc
  *         is_fsr = self._signals[signal_id].signal_type == c_jls.JLS_SIGNAL_TYPE_FSR
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)
  *         _handle_rc('rd_annotations', rc)
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 533, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_is_fsr);
   __Pyx_GIVEREF(__pyx_v_is_fsr);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_is_fsr);
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __Pyx_GIVEREF(__pyx_v_cbk_fn);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_cbk_fn);
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5pyjls_7binding_AnnotationCallback), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 533, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5pyjls_7binding_AnnotationCallback), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_user_data = ((struct __pyx_obj_5pyjls_7binding_AnnotationCallback *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":534
+  /* "pyjls/binding.pyx":536
  *         is_fsr = self._signals[signal_id].signal_type == c_jls.JLS_SIGNAL_TYPE_FSR
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_annotations', rc)
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 534, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 536, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 536, __pyx_L1_error)
   __pyx_v_rc = jls_rd_annotations(__pyx_v_self->_rd, __pyx_t_4, __pyx_t_5, __pyx_f_5pyjls_7binding__annotation_cbk_fn, ((void *)__pyx_v_user_data));
 
-  /* "pyjls/binding.pyx":535
+  /* "pyjls/binding.pyx":537
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)
  *         _handle_rc('rd_annotations', rc)             # <<<<<<<<<<<<<<
  * 
  *     def user_data(self, cbk_fn):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 537, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 537, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11866,49 +11891,49 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_annotations, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 535, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_annotations, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 535, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 535, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_annotations);
     __Pyx_GIVEREF(__pyx_n_u_rd_annotations);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_rd_annotations);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 535, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 537, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":522
+  /* "pyjls/binding.pyx":524
  *         return data
  * 
  *     def annotations(self, signal_id, timestamp, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read annotations from a signal.
  * 
  */
 
@@ -11927,15 +11952,15 @@
   __Pyx_XDECREF(__pyx_v_is_fsr);
   __Pyx_XDECREF((PyObject *)__pyx_v_user_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":537
+/* "pyjls/binding.pyx":539
  *         _handle_rc('rd_annotations', rc)
  * 
  *     def user_data(self, cbk_fn):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)
  */
 
@@ -11963,33 +11988,33 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("user_data", 0);
 
-  /* "pyjls/binding.pyx":539
+  /* "pyjls/binding.pyx":541
  *     def user_data(self, cbk_fn):
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_user_data', rc)
  * 
  */
   __pyx_v_rc = jls_rd_user_data(__pyx_v_self->_rd, __pyx_f_5pyjls_7binding__user_data_cbk_fn, ((void *)__pyx_v_cbk_fn));
 
-  /* "pyjls/binding.pyx":540
+  /* "pyjls/binding.pyx":542
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)
  *         _handle_rc('rd_user_data', rc)             # <<<<<<<<<<<<<<
  * 
  *     def utc(self, signal_id, sample_id, cbk_fn):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -11998,49 +12023,49 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 540, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 540, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 540, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_user_data);
     __Pyx_GIVEREF(__pyx_n_u_rd_user_data);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_n_u_rd_user_data);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 540, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":537
+  /* "pyjls/binding.pyx":539
  *         _handle_rc('rd_annotations', rc)
  * 
  *     def user_data(self, cbk_fn):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)
  */
 
@@ -12057,15 +12082,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":542
+/* "pyjls/binding.pyx":544
  *         _handle_rc('rd_user_data', rc)
  * 
  *     def utc(self, signal_id, sample_id, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read the sample_id / utc pairs from a FSR signal.
  * 
  */
 
@@ -12103,40 +12128,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 542, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 544, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cbk_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 542, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 544, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 542, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 544, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_cbk_fn = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 542, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 544, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.utc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_16utc(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_cbk_fn);
 
@@ -12158,35 +12183,35 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("utc", 0);
 
-  /* "pyjls/binding.pyx":554
+  /* "pyjls/binding.pyx":556
  *         """
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_utc(self._rd, signal_id, sample_id, _utc_cbk_fn, <void *> cbk_fn)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_utc', rc)
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 554, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 554, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 556, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 556, __pyx_L1_error)
   __pyx_v_rc = jls_rd_utc(__pyx_v_self->_rd, __pyx_t_1, __pyx_t_2, __pyx_f_5pyjls_7binding__utc_cbk_fn, ((void *)__pyx_v_cbk_fn));
 
-  /* "pyjls/binding.pyx":555
+  /* "pyjls/binding.pyx":557
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_utc(self._rd, signal_id, sample_id, _utc_cbk_fn, <void *> cbk_fn)
  *         _handle_rc('rd_utc', rc)             # <<<<<<<<<<<<<<
  * 
- * 
+ *     def sample_id_to_timestamp(self, signal_id, sample_id):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -12195,49 +12220,49 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_utc, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 555, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_utc, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 555, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 555, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_utc);
     __Pyx_GIVEREF(__pyx_n_u_rd_utc);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_rd_utc);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 555, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":542
+  /* "pyjls/binding.pyx":544
  *         _handle_rc('rd_user_data', rc)
  * 
  *     def utc(self, signal_id, sample_id, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read the sample_id / utc pairs from a FSR signal.
  * 
  */
 
@@ -12254,34 +12279,432 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "pyjls/binding.pyx":559
+ *         _handle_rc('rd_utc', rc)
+ * 
+ *     def sample_id_to_timestamp(self, signal_id, sample_id):             # <<<<<<<<<<<<<<
+ *         """Convert sample_id to UTC timestamp for FSR signals.
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_19sample_id_to_timestamp(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_5pyjls_7binding_6Reader_18sample_id_to_timestamp[] = "Convert sample_id to UTC timestamp for FSR signals.\n\n        :param signal_id: The signal id.\n        :param sample_id: The sample_id to convert.\n        :return: The JLS timestamp corresponding to sample_id.\n        :raise RuntimeError: on error.\n        ";
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_19sample_id_to_timestamp(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_signal_id = 0;
+  PyObject *__pyx_v_sample_id = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("sample_id_to_timestamp (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_signal_id,&__pyx_n_s_sample_id,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("sample_id_to_timestamp", 1, 2, 2, 1); __PYX_ERR(0, 559, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample_id_to_timestamp") < 0)) __PYX_ERR(0, 559, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_signal_id = values[0];
+    __pyx_v_sample_id = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("sample_id_to_timestamp", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 559, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyjls.binding.Reader.sample_id_to_timestamp", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_18sample_id_to_timestamp(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_18sample_id_to_timestamp(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_sample_id) {
+  int64_t __pyx_v_utc_timestamp;
+  int32_t __pyx_v_rc;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  uint16_t __pyx_t_1;
+  int64_t __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("sample_id_to_timestamp", 0);
+
+  /* "pyjls/binding.pyx":568
+ *         """
+ *         cdef int64_t utc_timestamp
+ *         rc = c_jls.jls_rd_sample_id_to_timestamp(self._rd, signal_id, sample_id, &utc_timestamp)             # <<<<<<<<<<<<<<
+ *         _handle_rc('sample_id_to_timestamp', rc)
+ *         return utc_timestamp
+ */
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_v_rc = jls_rd_sample_id_to_timestamp(__pyx_v_self->_rd, __pyx_t_1, __pyx_t_2, (&__pyx_v_utc_timestamp));
+
+  /* "pyjls/binding.pyx":569
+ *         cdef int64_t utc_timestamp
+ *         rc = c_jls.jls_rd_sample_id_to_timestamp(self._rd, signal_id, sample_id, &utc_timestamp)
+ *         _handle_rc('sample_id_to_timestamp', rc)             # <<<<<<<<<<<<<<
+ *         return utc_timestamp
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_4)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_sample_id_to_timestamp, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_sample_id_to_timestamp, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  } else
+  #endif
+  {
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    if (__pyx_t_6) {
+      __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
+    }
+    __Pyx_INCREF(__pyx_n_u_sample_id_to_timestamp);
+    __Pyx_GIVEREF(__pyx_n_u_sample_id_to_timestamp);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_sample_id_to_timestamp);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "pyjls/binding.pyx":570
+ *         rc = c_jls.jls_rd_sample_id_to_timestamp(self._rd, signal_id, sample_id, &utc_timestamp)
+ *         _handle_rc('sample_id_to_timestamp', rc)
+ *         return utc_timestamp             # <<<<<<<<<<<<<<
+ * 
+ *     def timestamp_to_sample_id(self, signal_id, utc_timestamp):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_utc_timestamp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 570, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "pyjls/binding.pyx":559
+ *         _handle_rc('rd_utc', rc)
+ * 
+ *     def sample_id_to_timestamp(self, signal_id, sample_id):             # <<<<<<<<<<<<<<
+ *         """Convert sample_id to UTC timestamp for FSR signals.
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("pyjls.binding.Reader.sample_id_to_timestamp", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pyjls/binding.pyx":572
+ *         return utc_timestamp
+ * 
+ *     def timestamp_to_sample_id(self, signal_id, utc_timestamp):             # <<<<<<<<<<<<<<
+ *         """Convert UTC timestamp to sample_id for FSR signals.
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_21timestamp_to_sample_id(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_5pyjls_7binding_6Reader_20timestamp_to_sample_id[] = "Convert UTC timestamp to sample_id for FSR signals.\n\n        :param signal_id: The signal id.\n        :param utc_timestamp: The UTC timestamp to convert.\n        :return: The sample_id corresponding to utc_timestamp.\n        :raise RuntimeError: on error.\n        ";
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_21timestamp_to_sample_id(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_signal_id = 0;
+  PyObject *__pyx_v_utc_timestamp = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("timestamp_to_sample_id (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_signal_id,&__pyx_n_s_utc_timestamp,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_utc_timestamp)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("timestamp_to_sample_id", 1, 2, 2, 1); __PYX_ERR(0, 572, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "timestamp_to_sample_id") < 0)) __PYX_ERR(0, 572, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_signal_id = values[0];
+    __pyx_v_utc_timestamp = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("timestamp_to_sample_id", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 572, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyjls.binding.Reader.timestamp_to_sample_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_20timestamp_to_sample_id(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_utc_timestamp);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_20timestamp_to_sample_id(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_utc_timestamp) {
+  int64_t __pyx_v_sample_id;
+  int32_t __pyx_v_rc;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  uint16_t __pyx_t_1;
+  int64_t __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("timestamp_to_sample_id", 0);
+
+  /* "pyjls/binding.pyx":581
+ *         """
+ *         cdef int64_t sample_id
+ *         rc = c_jls.jls_rd_timestamp_to_sample_id(self._rd, signal_id, utc_timestamp, &sample_id)             # <<<<<<<<<<<<<<
+ *         _handle_rc('timestamp_to_sample_id', rc)
+ *         return sample_id
+ */
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_utc_timestamp); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_v_rc = jls_rd_timestamp_to_sample_id(__pyx_v_self->_rd, __pyx_t_1, __pyx_t_2, (&__pyx_v_sample_id));
+
+  /* "pyjls/binding.pyx":582
+ *         cdef int64_t sample_id
+ *         rc = c_jls.jls_rd_timestamp_to_sample_id(self._rd, signal_id, utc_timestamp, &sample_id)
+ *         _handle_rc('timestamp_to_sample_id', rc)             # <<<<<<<<<<<<<<
+ *         return sample_id
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_4)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_timestamp_to_sample_id, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_timestamp_to_sample_id, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  } else
+  #endif
+  {
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    if (__pyx_t_6) {
+      __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
+    }
+    __Pyx_INCREF(__pyx_n_u_timestamp_to_sample_id);
+    __Pyx_GIVEREF(__pyx_n_u_timestamp_to_sample_id);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_timestamp_to_sample_id);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "pyjls/binding.pyx":583
+ *         rc = c_jls.jls_rd_timestamp_to_sample_id(self._rd, signal_id, utc_timestamp, &sample_id)
+ *         _handle_rc('timestamp_to_sample_id', rc)
+ *         return sample_id             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_sample_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "pyjls/binding.pyx":572
+ *         return utc_timestamp
+ * 
+ *     def timestamp_to_sample_id(self, signal_id, utc_timestamp):             # <<<<<<<<<<<<<<
+ *         """Convert UTC timestamp to sample_id for FSR signals.
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("pyjls.binding.Reader.timestamp_to_sample_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5pyjls_7binding_6Reader_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_5pyjls_7binding_6Reader_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_23__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_23__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_18__reduce_cython__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_22__reduce_cython__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5pyjls_7binding_6Reader_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_22__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -12318,27 +12741,27 @@
  * def __reduce_cython__(self):
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5pyjls_7binding_6Reader_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_5pyjls_7binding_6Reader_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_25__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_5pyjls_7binding_6Reader_25__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_20__setstate_cython__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_24__setstate_cython__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5pyjls_7binding_6Reader_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_5pyjls_7binding_6Reader_24__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -12367,15 +12790,15 @@
   __Pyx_AddTraceback("pyjls.binding.Reader.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":558
+/* "pyjls/binding.pyx":586
  * 
  * 
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):             # <<<<<<<<<<<<<<
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  */
 
@@ -12404,121 +12827,121 @@
   PyObject *__pyx_t_15 = NULL;
   int32_t __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_annotation_cbk_fn", 0);
 
-  /* "pyjls/binding.pyx":559
+  /* "pyjls/binding.pyx":587
  * 
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):
  *     obj: AnnotationCallback = <object> user_data             # <<<<<<<<<<<<<<
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  *     y = annotation[0].y
  */
-  if (!(likely(((((PyObject *)__pyx_v_user_data)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user_data), __pyx_ptype_5pyjls_7binding_AnnotationCallback))))) __PYX_ERR(0, 559, __pyx_L1_error)
+  if (!(likely(((((PyObject *)__pyx_v_user_data)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user_data), __pyx_ptype_5pyjls_7binding_AnnotationCallback))))) __PYX_ERR(0, 587, __pyx_L1_error)
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_obj = ((struct __pyx_obj_5pyjls_7binding_AnnotationCallback *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":560
+  /* "pyjls/binding.pyx":588
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)             # <<<<<<<<<<<<<<
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp
  */
-  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack((__pyx_v_annotation[0]).storage_type, (__pyx_v_annotation[0]).data, (__pyx_v_annotation[0]).data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack((__pyx_v_annotation[0]).storage_type, (__pyx_v_annotation[0]).data, (__pyx_v_annotation[0]).data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":561
+  /* "pyjls/binding.pyx":589
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  *     y = annotation[0].y             # <<<<<<<<<<<<<<
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:
  */
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_annotation[0]).y); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_annotation[0]).y); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_y = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":562
+  /* "pyjls/binding.pyx":590
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp             # <<<<<<<<<<<<<<
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp
  */
   __pyx_t_2 = (__pyx_v_annotation[0]).timestamp;
   __pyx_v_timestamp = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":563
+  /* "pyjls/binding.pyx":591
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:             # <<<<<<<<<<<<<<
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):
  */
   __pyx_t_3 = ((!(__pyx_v_obj->is_fsr != 0)) != 0);
   if (__pyx_t_3) {
 
-    /* "pyjls/binding.pyx":564
+    /* "pyjls/binding.pyx":592
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp             # <<<<<<<<<<<<<<
  *     if not isfinite(y):
  *         y = None
  */
     __pyx_t_2 = (__pyx_v_annotation[0]).timestamp;
     __pyx_v_timestamp = __pyx_t_2;
 
-    /* "pyjls/binding.pyx":563
+    /* "pyjls/binding.pyx":591
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:             # <<<<<<<<<<<<<<
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):
  */
   }
 
-  /* "pyjls/binding.pyx":565
+  /* "pyjls/binding.pyx":593
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):             # <<<<<<<<<<<<<<
  *         y = None
  *     try:
  */
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_y); if (unlikely((__pyx_t_4 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_y); if (unlikely((__pyx_t_4 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(0, 593, __pyx_L1_error)
   __pyx_t_3 = ((!(isfinite(__pyx_t_4) != 0)) != 0);
   if (__pyx_t_3) {
 
-    /* "pyjls/binding.pyx":566
+    /* "pyjls/binding.pyx":594
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):
  *         y = None             # <<<<<<<<<<<<<<
  *     try:
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  */
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_y, Py_None);
 
-    /* "pyjls/binding.pyx":565
+    /* "pyjls/binding.pyx":593
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):             # <<<<<<<<<<<<<<
  *         y = None
  *     try:
  */
   }
 
-  /* "pyjls/binding.pyx":567
+  /* "pyjls/binding.pyx":595
  *     if not isfinite(y):
  *         y = None
  *     try:             # <<<<<<<<<<<<<<
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  */
   {
@@ -12526,26 +12949,26 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_7);
     /*try:*/ {
 
-      /* "pyjls/binding.pyx":568
+      /* "pyjls/binding.pyx":596
  *         y = None
  *     try:
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)             # <<<<<<<<<<<<<<
  *     except Exception:
  *         logging.getLogger(__name__).exception('in annotation callback')
  */
-      __pyx_t_8 = __Pyx_PyInt_From_int64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 568, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyInt_From_int64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 596, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).annotation_type); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 568, __pyx_L5_error)
+      __pyx_t_9 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).annotation_type); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 596, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).group_id); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 568, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).group_id); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 596, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_INCREF(__pyx_v_obj->cbk_fn);
       __pyx_t_11 = __pyx_v_obj->cbk_fn; __pyx_t_12 = NULL;
       __pyx_t_13 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_12)) {
@@ -12555,35 +12978,35 @@
           __Pyx_DECREF_SET(__pyx_t_11, function);
           __pyx_t_13 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_11)) {
         PyObject *__pyx_temp[6] = {__pyx_t_12, __pyx_t_8, __pyx_v_y, __pyx_t_9, __pyx_t_10, __pyx_v_data};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L5_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L5_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
         PyObject *__pyx_temp[6] = {__pyx_t_12, __pyx_t_8, __pyx_v_y, __pyx_t_9, __pyx_t_10, __pyx_v_data};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L5_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L5_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       {
-        __pyx_t_14 = PyTuple_New(5+__pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 568, __pyx_L5_error)
+        __pyx_t_14 = PyTuple_New(5+__pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 596, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_14);
         if (__pyx_t_12) {
           __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_12); __pyx_t_12 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_8);
         PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_13, __pyx_t_8);
         __Pyx_INCREF(__pyx_v_y);
@@ -12595,23 +13018,23 @@
         PyTuple_SET_ITEM(__pyx_t_14, 3+__pyx_t_13, __pyx_t_10);
         __Pyx_INCREF(__pyx_v_data);
         __Pyx_GIVEREF(__pyx_v_data);
         PyTuple_SET_ITEM(__pyx_t_14, 4+__pyx_t_13, __pyx_v_data);
         __pyx_t_8 = 0;
         __pyx_t_9 = 0;
         __pyx_t_10 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L5_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       }
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_v_rc = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "pyjls/binding.pyx":567
+      /* "pyjls/binding.pyx":595
  *     if not isfinite(y):
  *         y = None
  *     try:             # <<<<<<<<<<<<<<
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  */
     }
@@ -12624,80 +13047,80 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "pyjls/binding.pyx":569
+    /* "pyjls/binding.pyx":597
  *     try:
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:             # <<<<<<<<<<<<<<
  *         logging.getLogger(__name__).exception('in annotation callback')
  *         return 1
  */
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("pyjls.binding._annotation_cbk_fn", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_11, &__pyx_t_14) < 0) __PYX_ERR(0, 569, __pyx_L7_except_error)
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_11, &__pyx_t_14) < 0) __PYX_ERR(0, 597, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_GOTREF(__pyx_t_14);
 
-      /* "pyjls/binding.pyx":570
+      /* "pyjls/binding.pyx":598
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  *         logging.getLogger(__name__).exception('in annotation callback')             # <<<<<<<<<<<<<<
  *         return 1
  *     return 1 if bool(rc) else 0
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logging); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 570, __pyx_L7_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logging); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 598, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 570, __pyx_L7_except_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 598, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_name_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 570, __pyx_L7_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_name_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 598, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_15 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_15)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_9 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_15, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_8);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 570, __pyx_L7_except_error)
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 598, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_exception); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 570, __pyx_L7_except_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_exception); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 598, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_10 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_9, __pyx_kp_u_in_annotation_callback) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_kp_u_in_annotation_callback);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 570, __pyx_L7_except_error)
+      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 598, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-      /* "pyjls/binding.pyx":571
+      /* "pyjls/binding.pyx":599
  *     except Exception:
  *         logging.getLogger(__name__).exception('in annotation callback')
  *         return 1             # <<<<<<<<<<<<<<
  *     return 1 if bool(rc) else 0
  * 
  */
       __pyx_r = 1;
@@ -12705,15 +13128,15 @@
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       goto __pyx_L8_except_return;
     }
     goto __pyx_L7_except_error;
     __pyx_L7_except_error:;
 
-    /* "pyjls/binding.pyx":567
+    /* "pyjls/binding.pyx":595
  *     if not isfinite(y):
  *         y = None
  *     try:             # <<<<<<<<<<<<<<
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_5);
@@ -12726,31 +13149,31 @@
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
     goto __pyx_L0;
     __pyx_L10_try_end:;
   }
 
-  /* "pyjls/binding.pyx":572
+  /* "pyjls/binding.pyx":600
  *         logging.getLogger(__name__).exception('in annotation callback')
  *         return 1
  *     return 1 if bool(rc) else 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 572, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 600, __pyx_L1_error)
   if (((!(!__pyx_t_3)) != 0)) {
     __pyx_t_16 = 1;
   } else {
     __pyx_t_16 = 0;
   }
   __pyx_r = __pyx_t_16;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":558
+  /* "pyjls/binding.pyx":586
  * 
  * 
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):             # <<<<<<<<<<<<<<
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  */
 
@@ -12771,15 +13194,15 @@
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_y);
   __Pyx_XDECREF(__pyx_v_rc);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":575
+/* "pyjls/binding.pyx":603
  * 
  * 
  * cdef int32_t _user_data_cbk_fn(void * user_data, uint16_t chunk_meta, c_jls.jls_storage_type_e storage_type,             # <<<<<<<<<<<<<<
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data
  */
 
@@ -12798,46 +13221,46 @@
   int32_t __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_user_data_cbk_fn", 0);
 
-  /* "pyjls/binding.pyx":577
+  /* "pyjls/binding.pyx":605
  * cdef int32_t _user_data_cbk_fn(void * user_data, uint16_t chunk_meta, c_jls.jls_storage_type_e storage_type,
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data             # <<<<<<<<<<<<<<
  *     d = _storage_unpack(storage_type, data, data_size)
  *     rc = cbk_fn(chunk_meta, d)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_cbk_fn = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":578
+  /* "pyjls/binding.pyx":606
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data
  *     d = _storage_unpack(storage_type, data, data_size)             # <<<<<<<<<<<<<<
  *     rc = cbk_fn(chunk_meta, d)
  *     return 1 if bool(rc) else 0
  */
-  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack(__pyx_v_storage_type, __pyx_v_data, __pyx_v_data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 578, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack(__pyx_v_storage_type, __pyx_v_data, __pyx_v_data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_d = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":579
+  /* "pyjls/binding.pyx":607
  *     cbk_fn = <object> user_data
  *     d = _storage_unpack(storage_type, data, data_size)
  *     rc = cbk_fn(chunk_meta, d)             # <<<<<<<<<<<<<<
  *     return 1 if bool(rc) else 0
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_chunk_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 579, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_chunk_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __pyx_t_3 = __pyx_v_cbk_fn; __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -12847,66 +13270,66 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_d};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_d};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 607, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_d);
     __Pyx_GIVEREF(__pyx_v_d);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_d);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_rc = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":580
+  /* "pyjls/binding.pyx":608
  *     d = _storage_unpack(storage_type, data, data_size)
  *     rc = cbk_fn(chunk_meta, d)
  *     return 1 if bool(rc) else 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 608, __pyx_L1_error)
   if (((!(!__pyx_t_8)) != 0)) {
     __pyx_t_7 = 1;
   } else {
     __pyx_t_7 = 0;
   }
   __pyx_r = __pyx_t_7;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":575
+  /* "pyjls/binding.pyx":603
  * 
  * 
  * cdef int32_t _user_data_cbk_fn(void * user_data, uint16_t chunk_meta, c_jls.jls_storage_type_e storage_type,             # <<<<<<<<<<<<<<
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data
  */
 
@@ -12923,15 +13346,15 @@
   __Pyx_XDECREF(__pyx_v_cbk_fn);
   __Pyx_XDECREF(__pyx_v_d);
   __Pyx_XDECREF(__pyx_v_rc);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":583
+/* "pyjls/binding.pyx":611
  * 
  * 
  * cdef int32_t _utc_cbk_fn(void * user_data, const c_jls.jls_utc_summary_entry_s * utc, uint32_t size):             # <<<<<<<<<<<<<<
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data
  */
 
@@ -12953,130 +13376,130 @@
   int32_t __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_utc_cbk_fn", 0);
 
-  /* "pyjls/binding.pyx":585
+  /* "pyjls/binding.pyx":613
  * cdef int32_t _utc_cbk_fn(void * user_data, const c_jls.jls_utc_summary_entry_s * utc, uint32_t size):
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data             # <<<<<<<<<<<<<<
  *     entries = np.empty((size, 2), dtype=np.int64)
  *     for idx in range(size):
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_cbk_fn = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":586
+  /* "pyjls/binding.pyx":614
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data
  *     entries = np.empty((size, 2), dtype=np.int64)             # <<<<<<<<<<<<<<
  *     for idx in range(size):
  *         entries[idx, 0] = utc[idx].sample_id
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_2);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 586, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 614, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_entries = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":587
+  /* "pyjls/binding.pyx":615
  *     cbk_fn = <object> user_data
  *     entries = np.empty((size, 2), dtype=np.int64)
  *     for idx in range(size):             # <<<<<<<<<<<<<<
  *         entries[idx, 0] = utc[idx].sample_id
  *         entries[idx, 1] = utc[idx].timestamp
  */
   __pyx_t_6 = __pyx_v_size;
   __pyx_t_7 = __pyx_t_6;
   for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
     __pyx_v_idx = __pyx_t_8;
 
-    /* "pyjls/binding.pyx":588
+    /* "pyjls/binding.pyx":616
  *     entries = np.empty((size, 2), dtype=np.int64)
  *     for idx in range(size):
  *         entries[idx, 0] = utc[idx].sample_id             # <<<<<<<<<<<<<<
  *         entries[idx, 1] = utc[idx].timestamp
  *     rc = cbk_fn(entries)
  */
-    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).sample_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 588, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).sample_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 616, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 588, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_0);
     __pyx_t_3 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_1, __pyx_t_5) < 0)) __PYX_ERR(0, 588, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_1, __pyx_t_5) < 0)) __PYX_ERR(0, 616, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":589
+    /* "pyjls/binding.pyx":617
  *     for idx in range(size):
  *         entries[idx, 0] = utc[idx].sample_id
  *         entries[idx, 1] = utc[idx].timestamp             # <<<<<<<<<<<<<<
  *     rc = cbk_fn(entries)
  *     return 1 if bool(rc) else 0
  */
-    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).timestamp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 589, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).timestamp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 617, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 589, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 617, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_1);
     __pyx_t_1 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_3, __pyx_t_5) < 0)) __PYX_ERR(0, 589, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_3, __pyx_t_5) < 0)) __PYX_ERR(0, 617, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
 
-  /* "pyjls/binding.pyx":590
+  /* "pyjls/binding.pyx":618
  *         entries[idx, 0] = utc[idx].sample_id
  *         entries[idx, 1] = utc[idx].timestamp
  *     rc = cbk_fn(entries)             # <<<<<<<<<<<<<<
  *     return 1 if bool(rc) else 0
  */
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __pyx_t_3 = __pyx_v_cbk_fn; __pyx_t_1 = NULL;
@@ -13087,35 +13510,35 @@
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_entries) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_entries);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 590, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_rc = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":591
+  /* "pyjls/binding.pyx":619
  *         entries[idx, 1] = utc[idx].timestamp
  *     rc = cbk_fn(entries)
  *     return 1 if bool(rc) else 0             # <<<<<<<<<<<<<<
  */
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 619, __pyx_L1_error)
   if (((!(!__pyx_t_10)) != 0)) {
     __pyx_t_9 = 1;
   } else {
     __pyx_t_9 = 0;
   }
   __pyx_r = __pyx_t_9;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":583
+  /* "pyjls/binding.pyx":611
  * 
  * 
  * cdef int32_t _utc_cbk_fn(void * user_data, const c_jls.jls_utc_summary_entry_s * utc, uint32_t size):             # <<<<<<<<<<<<<<
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data
  */
 
@@ -13543,15 +13966,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13560,29 +13983,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":735
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13593,15 +14016,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13610,29 +14033,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":738
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13643,15 +14066,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13660,29 +14083,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":741
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13693,15 +14116,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13710,29 +14133,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":744
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13743,15 +14166,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13760,29 +14183,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":747
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13793,212 +14216,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":749
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":749
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":751
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
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":753
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":749
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
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":928
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":928
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
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":932
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":935
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
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":936
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":932
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
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14014,15 +14437,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -14030,53 +14453,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":941
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
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":943
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
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -14084,30 +14507,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":941
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14122,15 +14545,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":946
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14146,15 +14569,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14162,53 +14585,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":947
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
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":949
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
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -14216,30 +14639,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":947
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14254,15 +14677,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":952
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14278,15 +14701,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14294,53 +14717,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":953
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
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":955
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
+      /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -14348,30 +14771,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":953
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14386,176 +14809,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":966
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":966
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
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":981
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
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":981
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
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":996
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
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":1006
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
+/* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -27903,16 +28326,18 @@
   {"__exit__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyjls_7binding_6Reader_5__exit__, METH_VARARGS|METH_KEYWORDS, 0},
   {"close", (PyCFunction)__pyx_pw_5pyjls_7binding_6Reader_7close, METH_NOARGS, 0},
   {"fsr", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyjls_7binding_6Reader_9fsr, METH_VARARGS|METH_KEYWORDS, 0},
   {"fsr_statistics", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyjls_7binding_6Reader_11fsr_statistics, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5pyjls_7binding_6Reader_10fsr_statistics},
   {"annotations", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyjls_7binding_6Reader_13annotations, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5pyjls_7binding_6Reader_12annotations},
   {"user_data", (PyCFunction)__pyx_pw_5pyjls_7binding_6Reader_15user_data, METH_O, 0},
   {"utc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyjls_7binding_6Reader_17utc, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5pyjls_7binding_6Reader_16utc},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_5pyjls_7binding_6Reader_19__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_5pyjls_7binding_6Reader_21__setstate_cython__, METH_O, 0},
+  {"sample_id_to_timestamp", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyjls_7binding_6Reader_19sample_id_to_timestamp, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5pyjls_7binding_6Reader_18sample_id_to_timestamp},
+  {"timestamp_to_sample_id", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyjls_7binding_6Reader_21timestamp_to_sample_id, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5pyjls_7binding_6Reader_20timestamp_to_sample_id},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_5pyjls_7binding_6Reader_23__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_5pyjls_7binding_6Reader_25__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_5pyjls_7binding_Reader[] = {
   {(char *)"sources", __pyx_getprop_5pyjls_7binding_6Reader_sources, 0, (char *)0, 0},
   {(char *)"signals", __pyx_getprop_5pyjls_7binding_6Reader_signals, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
@@ -28818,14 +29243,15 @@
   {&__pyx_n_u_N, __pyx_k_N, sizeof(__pyx_k_N), 0, 1, 0, 1},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_Reader, __pyx_k_Reader, sizeof(__pyx_k_Reader), 0, 0, 1, 1},
   {&__pyx_n_u_Reader, __pyx_k_Reader, sizeof(__pyx_k_Reader), 0, 1, 0, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
+  {&__pyx_n_s_SECOND, __pyx_k_SECOND, sizeof(__pyx_k_SECOND), 0, 0, 1, 1},
   {&__pyx_n_s_STD, __pyx_k_STD, sizeof(__pyx_k_STD), 0, 0, 1, 1},
   {&__pyx_n_s_SignalDef, __pyx_k_SignalDef, sizeof(__pyx_k_SignalDef), 0, 0, 1, 1},
   {&__pyx_n_u_SignalDef, __pyx_k_SignalDef, sizeof(__pyx_k_SignalDef), 0, 1, 0, 1},
   {&__pyx_n_s_SignalType, __pyx_k_SignalType, sizeof(__pyx_k_SignalType), 0, 0, 1, 1},
   {&__pyx_n_u_SignalType, __pyx_k_SignalType, sizeof(__pyx_k_SignalType), 0, 1, 0, 1},
   {&__pyx_n_s_SourceDef, __pyx_k_SourceDef, sizeof(__pyx_k_SourceDef), 0, 0, 1, 1},
   {&__pyx_n_u_SourceDef, __pyx_k_SourceDef, sizeof(__pyx_k_SourceDef), 0, 1, 0, 1},
@@ -29005,14 +29431,16 @@
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_kp_b_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 0, 0},
   {&__pyx_n_s_s_2, __pyx_k_s_2, sizeof(__pyx_k_s_2), 0, 0, 1, 1},
   {&__pyx_n_s_sample_decimate_factor, __pyx_k_sample_decimate_factor, sizeof(__pyx_k_sample_decimate_factor), 0, 0, 1, 1},
   {&__pyx_n_s_sample_id, __pyx_k_sample_id, sizeof(__pyx_k_sample_id), 0, 0, 1, 1},
+  {&__pyx_n_s_sample_id_offset, __pyx_k_sample_id_offset, sizeof(__pyx_k_sample_id_offset), 0, 0, 1, 1},
+  {&__pyx_n_u_sample_id_to_timestamp, __pyx_k_sample_id_to_timestamp, sizeof(__pyx_k_sample_id_to_timestamp), 0, 1, 0, 1},
   {&__pyx_n_s_sample_rate, __pyx_k_sample_rate, sizeof(__pyx_k_sample_rate), 0, 0, 1, 1},
   {&__pyx_n_s_samples_per_data, __pyx_k_samples_per_data, sizeof(__pyx_k_samples_per_data), 0, 0, 1, 1},
   {&__pyx_kp_s_self__rd_cannot_be_converted_to, __pyx_k_self__rd_cannot_be_converted_to, sizeof(__pyx_k_self__rd_cannot_be_converted_to), 0, 0, 1, 0},
   {&__pyx_kp_s_self__wr_cannot_be_converted_to, __pyx_k_self__wr_cannot_be_converted_to, sizeof(__pyx_k_self__wr_cannot_be_converted_to), 0, 0, 1, 0},
   {&__pyx_n_s_serial_number, __pyx_k_serial_number, sizeof(__pyx_k_serial_number), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
@@ -29041,14 +29469,15 @@
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_structs, __pyx_k_structs, sizeof(__pyx_k_structs), 0, 0, 1, 1},
   {&__pyx_n_s_summary_decimate_factor, __pyx_k_summary_decimate_factor, sizeof(__pyx_k_summary_decimate_factor), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_u_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 1, 0, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_timestamp, __pyx_k_timestamp, sizeof(__pyx_k_timestamp), 0, 0, 1, 1},
+  {&__pyx_n_u_timestamp_to_sample_id, __pyx_k_timestamp_to_sample_id, sizeof(__pyx_k_timestamp_to_sample_id), 0, 1, 0, 1},
   {&__pyx_n_s_traceback, __pyx_k_traceback, sizeof(__pyx_k_traceback), 0, 0, 1, 1},
   {&__pyx_n_u_txt, __pyx_k_txt, sizeof(__pyx_k_txt), 0, 1, 0, 1},
   {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
   {&__pyx_n_u_u1, __pyx_k_u1, sizeof(__pyx_k_u1), 0, 1, 0, 1},
   {&__pyx_n_u_u16, __pyx_k_u16, sizeof(__pyx_k_u16), 0, 1, 0, 1},
   {&__pyx_n_u_u32, __pyx_k_u32, sizeof(__pyx_k_u32), 0, 1, 0, 1},
   {&__pyx_n_u_u4, __pyx_k_u4, sizeof(__pyx_k_u4), 0, 1, 0, 1},
@@ -29066,30 +29495,31 @@
   {&__pyx_n_u_user, __pyx_k_user, sizeof(__pyx_k_user), 0, 1, 0, 1},
   {&__pyx_n_u_user_data, __pyx_k_user_data, sizeof(__pyx_k_user_data), 0, 1, 0, 1},
   {&__pyx_n_u_usr, __pyx_k_usr, sizeof(__pyx_k_usr), 0, 1, 0, 1},
   {&__pyx_n_s_utc, __pyx_k_utc, sizeof(__pyx_k_utc), 0, 0, 1, 1},
   {&__pyx_n_u_utc, __pyx_k_utc, sizeof(__pyx_k_utc), 0, 1, 0, 1},
   {&__pyx_n_s_utc_decimate_factor, __pyx_k_utc_decimate_factor, sizeof(__pyx_k_utc_decimate_factor), 0, 0, 1, 1},
   {&__pyx_n_s_utc_i64, __pyx_k_utc_i64, sizeof(__pyx_k_utc_i64), 0, 0, 1, 1},
+  {&__pyx_n_s_utc_timestamp, __pyx_k_utc_timestamp, sizeof(__pyx_k_utc_timestamp), 0, 0, 1, 1},
   {&__pyx_n_s_utc_to_jls, __pyx_k_utc_to_jls, sizeof(__pyx_k_utc_to_jls), 0, 0, 1, 1},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_vendor, __pyx_k_vendor, sizeof(__pyx_k_vendor), 0, 0, 1, 1},
   {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
   {&__pyx_n_u_vertical_marker, __pyx_k_vertical_marker, sizeof(__pyx_k_vertical_marker), 0, 1, 0, 1},
   {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
   {&__pyx_n_u_vmarker, __pyx_k_vmarker, sizeof(__pyx_k_vmarker), 0, 1, 0, 1},
   {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 248, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 363, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 418, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
   return 0;
@@ -29097,22 +29527,22 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pyjls/binding.pyx":188
+  /* "pyjls/binding.pyx":189
  *     with gil:
  *         m = msg.decode('utf-8').strip()
  *         level, location, s = m.split(' ', 2)             # <<<<<<<<<<<<<<
  *         lvl = _log_level_map.get(level, logging.DEBUG)
  *         filename, line, _ = location.split(':')
  */
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_kp_u_, __pyx_int_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_kp_u_, __pyx_int_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -29149,26 +29579,26 @@
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_self__rd_cannot_be_converted_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
   __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_3248624, __pyx_int_200305830, __pyx_int_134405936); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -29366,133 +29796,133 @@
   __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
   __pyx_tuple__33 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
 
-  /* "pyjls/binding.pyx":49
+  /* "pyjls/binding.pyx":50
  * 
  * 
  * def _data_type_def(basetype, size, q):             # <<<<<<<<<<<<<<
  *     return (basetype & 0x0f) | ((size & 0xff) << 8) | ((q & 0xff) << 16)
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_n_s_basetype, __pyx_n_s_size, __pyx_n_s_q); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_n_s_basetype, __pyx_n_s_size, __pyx_n_s_q); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_def, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_def, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 50, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":119
+  /* "pyjls/binding.pyx":120
  * 
  * 
  * def _populate_data_type():             # <<<<<<<<<<<<<<
  *     for key, value in list(_data_type_as_enum.items()):
  *         _data_type_as_enum[value] = value
  */
-  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_key, __pyx_n_s_value); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_key, __pyx_n_s_value); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_populate_data_type, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_populate_data_type, 120, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 120, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":129
+  /* "pyjls/binding.pyx":130
  * 
  * 
  * def data_type_as_enum(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_enum[data_type]
  * 
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_enum_2, 129, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_enum_2, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 130, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":133
+  /* "pyjls/binding.pyx":134
  * 
  * 
  * def data_type_as_str(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_str[data_type]
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_str_2, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_str_2, 134, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 134, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":198
+  /* "pyjls/binding.pyx":199
  * 
  * 
  * def jls_inject_log(level, filename, line, msg):             # <<<<<<<<<<<<<<
  *     cdef char * c_msg
  *     location = ':'.join([filename, str(line), ''])
  */
-  __pyx_tuple__43 = PyTuple_Pack(6, __pyx_n_s_level, __pyx_n_s_filename, __pyx_n_s_line, __pyx_n_s_msg, __pyx_n_s_c_msg, __pyx_n_s_location); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(6, __pyx_n_s_level, __pyx_n_s_filename, __pyx_n_s_line, __pyx_n_s_msg, __pyx_n_s_c_msg, __pyx_n_s_location); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(4, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_inject_log, 198, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(4, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_inject_log, 199, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 199, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":206
+  /* "pyjls/binding.pyx":207
  * 
  * 
  * def _encode_str(s):             # <<<<<<<<<<<<<<
  *     if s is None:
  *         s = ''
  */
-  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_encode_str, 206, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_encode_str, 207, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 207, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":212
+  /* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, str):
  *         s = _encode_str(data)
  */
-  __pyx_tuple__47 = PyTuple_Pack(2, __pyx_n_s_data, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(2, __pyx_n_s_data, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_storage_pack, 212, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_storage_pack, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 213, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":233
+  /* "pyjls/binding.pyx":234
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
- *     return int((utc - _UTC_OFFSET) * (2**30))
+ *     return int((utc - _UTC_OFFSET) * SECOND)
  */
-  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_n_s_utc); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_n_s_utc); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_utc_to_jls, 233, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_utc_to_jls, 234, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 234, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":238
+  /* "pyjls/binding.pyx":239
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
- *     return (timestamp / (2**30)) + _UTC_OFFSET
+ *     return (timestamp / SECOND) + _UTC_OFFSET
  */
-  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_n_s_timestamp); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_n_s_timestamp); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_to_utc, 238, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_to_utc, 239, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 239, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":243
+  /* "pyjls/binding.pyx":244
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
-  __pyx_tuple__53 = PyTuple_Pack(4, __pyx_n_s_name, __pyx_n_s_rc, __pyx_n_s_rc_name, __pyx_n_s_rc_descr); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_tuple__53 = PyTuple_Pack(4, __pyx_n_s_name, __pyx_n_s_rc, __pyx_n_s_rc_name, __pyx_n_s_rc_descr); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__53);
   __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_handle_rc, 243, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_handle_rc, 244, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 244, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_AnnotationCallback(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_tuple__55 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -29639,43 +30069,43 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5pyjls_7binding_Writer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5pyjls_7binding_Writer.tp_dictoffset && __pyx_type_5pyjls_7binding_Writer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5pyjls_7binding_Writer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Writer, (PyObject *)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Writer, (PyObject *)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
   __pyx_ptype_5pyjls_7binding_Writer = &__pyx_type_5pyjls_7binding_Writer;
-  if (PyType_Ready(&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5pyjls_7binding_AnnotationCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5pyjls_7binding_AnnotationCallback.tp_dictoffset && __pyx_type_5pyjls_7binding_AnnotationCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5pyjls_7binding_AnnotationCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnnotationCallback, (PyObject *)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnnotationCallback, (PyObject *)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
   __pyx_ptype_5pyjls_7binding_AnnotationCallback = &__pyx_type_5pyjls_7binding_AnnotationCallback;
-  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5pyjls_7binding_Reader.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5pyjls_7binding_Reader.tp_dictoffset && __pyx_type_5pyjls_7binding_Reader.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5pyjls_7binding_Reader.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Reader, (PyObject *)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Reader, (PyObject *)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
   __pyx_ptype_5pyjls_7binding_Reader = &__pyx_type_5pyjls_7binding_Reader;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
@@ -30201,112 +30631,121 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_c, __pyx_t_3) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyjls/binding.pyx":45
  * _log_c = logging.getLogger(_log_c_name)
  * # _UTC_OFFSET = dateutil.parser.parse('2018-01-01T00:00:00Z').timestamp()
  * _UTC_OFFSET = 1514764800  # seconds             # <<<<<<<<<<<<<<
+ * SECOND = 1 << 30
  * DEF _JLS_SIGNAL_COUNT = 256  # From jls/format.h
- * 
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_UTC_OFFSET, __pyx_int_1514764800) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":49
+  /* "pyjls/binding.pyx":46
+ * # _UTC_OFFSET = dateutil.parser.parse('2018-01-01T00:00:00Z').timestamp()
+ * _UTC_OFFSET = 1514764800  # seconds
+ * SECOND = 1 << 30             # <<<<<<<<<<<<<<
+ * DEF _JLS_SIGNAL_COUNT = 256  # From jls/format.h
+ * 
+ */
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SECOND, __pyx_int_1073741824) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+
+  /* "pyjls/binding.pyx":50
  * 
  * 
  * def _data_type_def(basetype, size, q):             # <<<<<<<<<<<<<<
  *     return (basetype & 0x0f) | ((size & 0xff) << 8) | ((q & 0xff) << 16)
  * 
  */
-  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_1_data_type_def, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_1_data_type_def, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_def, __pyx_t_3) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_def, __pyx_t_3) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":53
+  /* "pyjls/binding.pyx":54
  * 
  * 
  * class _DataTypeBase:             # <<<<<<<<<<<<<<
  *     INT       = 0x01
  *     UNSIGNED  = 0x02
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_DataTypeBase, __pyx_n_s_DataTypeBase, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_DataTypeBase, __pyx_n_s_DataTypeBase, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "pyjls/binding.pyx":54
+  /* "pyjls/binding.pyx":55
  * 
  * class _DataTypeBase:
  *     INT       = 0x01             # <<<<<<<<<<<<<<
  *     UNSIGNED  = 0x02
  *     UINT      = 0x03
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_INT, __pyx_int_1) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_INT, __pyx_int_1) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":55
+  /* "pyjls/binding.pyx":56
  * class _DataTypeBase:
  *     INT       = 0x01
  *     UNSIGNED  = 0x02             # <<<<<<<<<<<<<<
  *     UINT      = 0x03
  *     FLOAT     = 0x04
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_UNSIGNED, __pyx_int_2) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_UNSIGNED, __pyx_int_2) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":56
+  /* "pyjls/binding.pyx":57
  *     INT       = 0x01
  *     UNSIGNED  = 0x02
  *     UINT      = 0x03             # <<<<<<<<<<<<<<
  *     FLOAT     = 0x04
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_UINT, __pyx_int_3) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_UINT, __pyx_int_3) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":57
+  /* "pyjls/binding.pyx":58
  *     UNSIGNED  = 0x02
  *     UINT      = 0x03
  *     FLOAT     = 0x04             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_FLOAT, __pyx_int_4) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_FLOAT, __pyx_int_4) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":53
+  /* "pyjls/binding.pyx":54
  * 
  * 
  * class _DataTypeBase:             # <<<<<<<<<<<<<<
  *     INT       = 0x01
  *     UNSIGNED  = 0x02
  */
-  __pyx_t_1 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_DataTypeBase, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_DataTypeBase, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DataTypeBase, __pyx_t_1) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DataTypeBase, __pyx_t_1) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":60
+  /* "pyjls/binding.pyx":61
  * 
  * 
  * class DataType:             # <<<<<<<<<<<<<<
  *     U1 = _data_type_def(_DataTypeBase.UINT, 1, 0)
  *     U4 = _data_type_def(_DataTypeBase.UINT, 4, 0)
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_DataType, __pyx_n_s_DataType, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_DataType, __pyx_n_s_DataType, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "pyjls/binding.pyx":61
+  /* "pyjls/binding.pyx":62
  * 
  * class DataType:
  *     U1 = _data_type_def(_DataTypeBase.UINT, 1, 0)             # <<<<<<<<<<<<<<
  *     U4 = _data_type_def(_DataTypeBase.UINT, 4, 0)
  *     U8 = _data_type_def(_DataTypeBase.UINT, 8, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -30316,64 +30755,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_1, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_1, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_int_1);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U1, __pyx_t_1) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U1, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":62
+  /* "pyjls/binding.pyx":63
  * class DataType:
  *     U1 = _data_type_def(_DataTypeBase.UINT, 1, 0)
  *     U4 = _data_type_def(_DataTypeBase.UINT, 4, 0)             # <<<<<<<<<<<<<<
  *     U8 = _data_type_def(_DataTypeBase.UINT, 8, 0)
  *     U16 = _data_type_def(_DataTypeBase.UINT, 16, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -30383,64 +30822,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_4, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_4, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_4);
     __Pyx_GIVEREF(__pyx_int_4);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_int_4);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U4, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U4, __pyx_t_1) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":63
+  /* "pyjls/binding.pyx":64
  *     U1 = _data_type_def(_DataTypeBase.UINT, 1, 0)
  *     U4 = _data_type_def(_DataTypeBase.UINT, 4, 0)
  *     U8 = _data_type_def(_DataTypeBase.UINT, 8, 0)             # <<<<<<<<<<<<<<
  *     U16 = _data_type_def(_DataTypeBase.UINT, 16, 0)
  *     U32 = _data_type_def(_DataTypeBase.UINT, 32, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -30450,64 +30889,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_8, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_8, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_8);
     __Pyx_GIVEREF(__pyx_int_8);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_int_8);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U8, __pyx_t_1) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U8, __pyx_t_1) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":64
+  /* "pyjls/binding.pyx":65
  *     U4 = _data_type_def(_DataTypeBase.UINT, 4, 0)
  *     U8 = _data_type_def(_DataTypeBase.UINT, 8, 0)
  *     U16 = _data_type_def(_DataTypeBase.UINT, 16, 0)             # <<<<<<<<<<<<<<
  *     U32 = _data_type_def(_DataTypeBase.UINT, 32, 0)
  *     U64 = _data_type_def(_DataTypeBase.UINT, 64, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -30517,64 +30956,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_16, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_16, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_16);
     __Pyx_GIVEREF(__pyx_int_16);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_int_16);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U16, __pyx_t_1) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U16, __pyx_t_1) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":65
+  /* "pyjls/binding.pyx":66
  *     U8 = _data_type_def(_DataTypeBase.UINT, 8, 0)
  *     U16 = _data_type_def(_DataTypeBase.UINT, 16, 0)
  *     U32 = _data_type_def(_DataTypeBase.UINT, 32, 0)             # <<<<<<<<<<<<<<
  *     U64 = _data_type_def(_DataTypeBase.UINT, 64, 0)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -30584,64 +31023,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_32, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_32, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_32);
     __Pyx_GIVEREF(__pyx_int_32);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_int_32);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U32, __pyx_t_1) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U32, __pyx_t_1) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":66
+  /* "pyjls/binding.pyx":67
  *     U16 = _data_type_def(_DataTypeBase.UINT, 16, 0)
  *     U32 = _data_type_def(_DataTypeBase.UINT, 32, 0)
  *     U64 = _data_type_def(_DataTypeBase.UINT, 64, 0)             # <<<<<<<<<<<<<<
  * 
  *     I4 = _data_type_def(_DataTypeBase.INT, 4, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_UINT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -30651,64 +31090,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_64, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_64, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_64);
     __Pyx_GIVEREF(__pyx_int_64);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_int_64);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U64, __pyx_t_1) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_U64, __pyx_t_1) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":68
+  /* "pyjls/binding.pyx":69
  *     U64 = _data_type_def(_DataTypeBase.UINT, 64, 0)
  * 
  *     I4 = _data_type_def(_DataTypeBase.INT, 4, 0)             # <<<<<<<<<<<<<<
  *     I8 = _data_type_def(_DataTypeBase.INT, 8, 0)
  *     I16 = _data_type_def(_DataTypeBase.INT, 16, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -30718,64 +31157,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_4, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_4, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_4);
     __Pyx_GIVEREF(__pyx_int_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_int_4);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I4, __pyx_t_1) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I4, __pyx_t_1) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":69
+  /* "pyjls/binding.pyx":70
  * 
  *     I4 = _data_type_def(_DataTypeBase.INT, 4, 0)
  *     I8 = _data_type_def(_DataTypeBase.INT, 8, 0)             # <<<<<<<<<<<<<<
  *     I16 = _data_type_def(_DataTypeBase.INT, 16, 0)
  *     I32 = _data_type_def(_DataTypeBase.INT, 32, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -30785,64 +31224,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_8, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_8, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_8);
     __Pyx_GIVEREF(__pyx_int_8);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_int_8);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I8, __pyx_t_1) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I8, __pyx_t_1) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":70
+  /* "pyjls/binding.pyx":71
  *     I4 = _data_type_def(_DataTypeBase.INT, 4, 0)
  *     I8 = _data_type_def(_DataTypeBase.INT, 8, 0)
  *     I16 = _data_type_def(_DataTypeBase.INT, 16, 0)             # <<<<<<<<<<<<<<
  *     I32 = _data_type_def(_DataTypeBase.INT, 32, 0)
  *     I64 = _data_type_def(_DataTypeBase.INT, 64, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -30852,64 +31291,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_16, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_16, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_16);
     __Pyx_GIVEREF(__pyx_int_16);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_int_16);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I16, __pyx_t_1) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I16, __pyx_t_1) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":71
+  /* "pyjls/binding.pyx":72
  *     I8 = _data_type_def(_DataTypeBase.INT, 8, 0)
  *     I16 = _data_type_def(_DataTypeBase.INT, 16, 0)
  *     I32 = _data_type_def(_DataTypeBase.INT, 32, 0)             # <<<<<<<<<<<<<<
  *     I64 = _data_type_def(_DataTypeBase.INT, 64, 0)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -30919,64 +31358,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_32, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_32, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_32);
     __Pyx_GIVEREF(__pyx_int_32);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_int_32);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I32, __pyx_t_1) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I32, __pyx_t_1) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":72
+  /* "pyjls/binding.pyx":73
  *     I16 = _data_type_def(_DataTypeBase.INT, 16, 0)
  *     I32 = _data_type_def(_DataTypeBase.INT, 32, 0)
  *     I64 = _data_type_def(_DataTypeBase.INT, 64, 0)             # <<<<<<<<<<<<<<
  * 
  *     F32 = _data_type_def(_DataTypeBase.FLOAT, 32, 0)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_INT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -30986,64 +31425,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_64, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_64, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_64);
     __Pyx_GIVEREF(__pyx_int_64);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_int_64);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I64, __pyx_t_1) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_I64, __pyx_t_1) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":74
+  /* "pyjls/binding.pyx":75
  *     I64 = _data_type_def(_DataTypeBase.INT, 64, 0)
  * 
  *     F32 = _data_type_def(_DataTypeBase.FLOAT, 32, 0)             # <<<<<<<<<<<<<<
  *     F64 = _data_type_def(_DataTypeBase.FLOAT, 64, 0)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_FLOAT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_FLOAT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
@@ -31053,64 +31492,64 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_32, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_5, __pyx_int_32, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_32);
     __Pyx_GIVEREF(__pyx_int_32);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_int_32);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_F32, __pyx_t_1) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_F32, __pyx_t_1) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":75
+  /* "pyjls/binding.pyx":76
  * 
  *     F32 = _data_type_def(_DataTypeBase.FLOAT, 32, 0)
  *     F64 = _data_type_def(_DataTypeBase.FLOAT, 64, 0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_data_type_def); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataTypeBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_FLOAT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_FLOAT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -31120,1206 +31559,1206 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_64, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_5, __pyx_int_64, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_5);
     __Pyx_INCREF(__pyx_int_64);
     __Pyx_GIVEREF(__pyx_int_64);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_int_64);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_int_0);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_F64, __pyx_t_1) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_F64, __pyx_t_1) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":60
+  /* "pyjls/binding.pyx":61
  * 
  * 
  * class DataType:             # <<<<<<<<<<<<<<
  *     U1 = _data_type_def(_DataTypeBase.UINT, 1, 0)
  *     U4 = _data_type_def(_DataTypeBase.UINT, 4, 0)
  */
-  __pyx_t_1 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_DataType, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_DataType, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DataType, __pyx_t_1) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DataType, __pyx_t_1) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":79
+  /* "pyjls/binding.pyx":80
  * 
  * _data_type_map = {
  *     DataType.U1: np.uint8,      # packed             # <<<<<<<<<<<<<<
  *     DataType.U4: np.uint8,      # packed
  *     DataType.U8: np.uint8,
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_U1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_U1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":80
+  /* "pyjls/binding.pyx":81
  * _data_type_map = {
  *     DataType.U1: np.uint8,      # packed
  *     DataType.U4: np.uint8,      # packed             # <<<<<<<<<<<<<<
  *     DataType.U8: np.uint8,
  *     DataType.U16: np.uint16,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":81
+  /* "pyjls/binding.pyx":82
  *     DataType.U1: np.uint8,      # packed
  *     DataType.U4: np.uint8,      # packed
  *     DataType.U8: np.uint8,             # <<<<<<<<<<<<<<
  *     DataType.U16: np.uint16,
  *     DataType.U32: np.uint32,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_U8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_U8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":82
+  /* "pyjls/binding.pyx":83
  *     DataType.U4: np.uint8,      # packed
  *     DataType.U8: np.uint8,
  *     DataType.U16: np.uint16,             # <<<<<<<<<<<<<<
  *     DataType.U32: np.uint32,
  *     DataType.U64: np.uint64,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":83
+  /* "pyjls/binding.pyx":84
  *     DataType.U8: np.uint8,
  *     DataType.U16: np.uint16,
  *     DataType.U32: np.uint32,             # <<<<<<<<<<<<<<
  *     DataType.U64: np.uint64,
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_U32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_U32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":84
+  /* "pyjls/binding.pyx":85
  *     DataType.U16: np.uint16,
  *     DataType.U32: np.uint32,
  *     DataType.U64: np.uint64,             # <<<<<<<<<<<<<<
  * 
  *     DataType.I4: np.uint8,      # packed
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":86
+  /* "pyjls/binding.pyx":87
  *     DataType.U64: np.uint64,
  * 
  *     DataType.I4: np.uint8,      # packed             # <<<<<<<<<<<<<<
  *     DataType.I8: np.int8,
  *     DataType.I16: np.int16,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_I4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_I4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":87
+  /* "pyjls/binding.pyx":88
  * 
  *     DataType.I4: np.uint8,      # packed
  *     DataType.I8: np.int8,             # <<<<<<<<<<<<<<
  *     DataType.I16: np.int16,
  *     DataType.I32: np.int32,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":88
+  /* "pyjls/binding.pyx":89
  *     DataType.I4: np.uint8,      # packed
  *     DataType.I8: np.int8,
  *     DataType.I16: np.int16,             # <<<<<<<<<<<<<<
  *     DataType.I32: np.int32,
  *     DataType.I64: np.int64,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_I16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_I16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":89
+  /* "pyjls/binding.pyx":90
  *     DataType.I8: np.int8,
  *     DataType.I16: np.int16,
  *     DataType.I32: np.int32,             # <<<<<<<<<<<<<<
  *     DataType.I64: np.int64,
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":90
+  /* "pyjls/binding.pyx":91
  *     DataType.I16: np.int16,
  *     DataType.I32: np.int32,
  *     DataType.I64: np.int64,             # <<<<<<<<<<<<<<
  * 
  *     DataType.F32: np.float32,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_I64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_I64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":92
+  /* "pyjls/binding.pyx":93
  *     DataType.I64: np.int64,
  * 
  *     DataType.F32: np.float32,             # <<<<<<<<<<<<<<
  *     DataType.F64: np.float64,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_F32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_F32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":93
+  /* "pyjls/binding.pyx":94
  * 
  *     DataType.F32: np.float32,
  *     DataType.F64: np.float64,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_F64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_F64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_2, __pyx_t_7) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_map, __pyx_t_3) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_map, __pyx_t_3) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":98
+  /* "pyjls/binding.pyx":99
  * 
  * _data_type_as_enum = {
  *     'u1': DataType.U1,             # <<<<<<<<<<<<<<
  *     'u4': DataType.U4,
  *     'u8': DataType.U8,
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u1, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u1, __pyx_t_2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":99
+  /* "pyjls/binding.pyx":100
  * _data_type_as_enum = {
  *     'u1': DataType.U1,
  *     'u4': DataType.U4,             # <<<<<<<<<<<<<<
  *     'u8': DataType.U8,
  *     'u16': DataType.U16,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_U4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_U4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u4, __pyx_t_7) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u4, __pyx_t_7) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":100
+  /* "pyjls/binding.pyx":101
  *     'u1': DataType.U1,
  *     'u4': DataType.U4,
  *     'u8': DataType.U8,             # <<<<<<<<<<<<<<
  *     'u16': DataType.U16,
  *     'u32': DataType.U32,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u8, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u8, __pyx_t_2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":101
+  /* "pyjls/binding.pyx":102
  *     'u4': DataType.U4,
  *     'u8': DataType.U8,
  *     'u16': DataType.U16,             # <<<<<<<<<<<<<<
  *     'u32': DataType.U32,
  *     'u64': DataType.U64,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_U16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_U16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u16, __pyx_t_7) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u16, __pyx_t_7) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":102
+  /* "pyjls/binding.pyx":103
  *     'u8': DataType.U8,
  *     'u16': DataType.U16,
  *     'u32': DataType.U32,             # <<<<<<<<<<<<<<
  *     'u64': DataType.U64,
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_U32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u32, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u32, __pyx_t_2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":103
+  /* "pyjls/binding.pyx":104
  *     'u16': DataType.U16,
  *     'u32': DataType.U32,
  *     'u64': DataType.U64,             # <<<<<<<<<<<<<<
  * 
  *     'i4': DataType.I4,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_U64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_U64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u64, __pyx_t_7) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_u64, __pyx_t_7) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":105
+  /* "pyjls/binding.pyx":106
  *     'u64': DataType.U64,
  * 
  *     'i4': DataType.I4,             # <<<<<<<<<<<<<<
  *     'i8': DataType.I8,
  *     'i16': DataType.I16,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i4, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i4, __pyx_t_2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":106
+  /* "pyjls/binding.pyx":107
  * 
  *     'i4': DataType.I4,
  *     'i8': DataType.I8,             # <<<<<<<<<<<<<<
  *     'i16': DataType.I16,
  *     'i32': DataType.I32,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_I8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_I8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i8, __pyx_t_7) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i8, __pyx_t_7) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":107
+  /* "pyjls/binding.pyx":108
  *     'i4': DataType.I4,
  *     'i8': DataType.I8,
  *     'i16': DataType.I16,             # <<<<<<<<<<<<<<
  *     'i32': DataType.I32,
  *     'i64': DataType.I64,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i16, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i16, __pyx_t_2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":108
+  /* "pyjls/binding.pyx":109
  *     'i8': DataType.I8,
  *     'i16': DataType.I16,
  *     'i32': DataType.I32,             # <<<<<<<<<<<<<<
  *     'i64': DataType.I64,
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_I32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_I32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i32, __pyx_t_7) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i32, __pyx_t_7) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":109
+  /* "pyjls/binding.pyx":110
  *     'i16': DataType.I16,
  *     'i32': DataType.I32,
  *     'i64': DataType.I64,             # <<<<<<<<<<<<<<
  * 
  *     'f32': DataType.F32,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_I64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i64, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_i64, __pyx_t_2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":111
+  /* "pyjls/binding.pyx":112
  *     'i64': DataType.I64,
  * 
  *     'f32': DataType.F32,             # <<<<<<<<<<<<<<
  *     'f64': DataType.F64,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_F32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_F32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_f32, __pyx_t_7) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_f32, __pyx_t_7) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":112
+  /* "pyjls/binding.pyx":113
  * 
  *     'f32': DataType.F32,
  *     'f64': DataType.F64,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DataType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_F64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_F64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_f64, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_f64, __pyx_t_2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_enum, __pyx_t_3) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_enum, __pyx_t_3) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":116
+  /* "pyjls/binding.pyx":117
  * 
  * 
  * _data_type_as_str = {}             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_str, __pyx_t_3) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_str, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":119
+  /* "pyjls/binding.pyx":120
  * 
  * 
  * def _populate_data_type():             # <<<<<<<<<<<<<<
  *     for key, value in list(_data_type_as_enum.items()):
  *         _data_type_as_enum[value] = value
  */
-  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_3_populate_data_type, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_3_populate_data_type, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_populate_data_type, __pyx_t_3) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_populate_data_type, __pyx_t_3) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":126
+  /* "pyjls/binding.pyx":127
  * 
  * 
  * _populate_data_type()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_populate_data_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_populate_data_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":129
+  /* "pyjls/binding.pyx":130
  * 
  * 
  * def data_type_as_enum(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_enum[data_type]
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_5data_type_as_enum, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_5data_type_as_enum, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_enum_2, __pyx_t_2) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_enum_2, __pyx_t_2) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":133
+  /* "pyjls/binding.pyx":134
  * 
  * 
  * def data_type_as_str(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_str[data_type]
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_7data_type_as_str, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_7data_type_as_str, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_str_2, __pyx_t_2) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_data_type_as_str_2, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":137
+  /* "pyjls/binding.pyx":138
  * 
  * 
  * class AnnotationType:             # <<<<<<<<<<<<<<
  *     USER = c_jls.JLS_ANNOTATION_TYPE_USER
  *     TEXT = c_jls.JLS_ANNOTATION_TYPE_TEXT
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_AnnotationType, __pyx_n_s_AnnotationType, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_AnnotationType, __pyx_n_s_AnnotationType, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "pyjls/binding.pyx":138
+  /* "pyjls/binding.pyx":139
  * 
  * class AnnotationType:
  *     USER = c_jls.JLS_ANNOTATION_TYPE_USER             # <<<<<<<<<<<<<<
  *     TEXT = c_jls.JLS_ANNOTATION_TYPE_TEXT
  *     VMARKER = c_jls.JLS_ANNOTATION_TYPE_VERTICAL_MARKER
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_USER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_USER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_USER, __pyx_t_3) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_USER, __pyx_t_3) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":139
+  /* "pyjls/binding.pyx":140
  * class AnnotationType:
  *     USER = c_jls.JLS_ANNOTATION_TYPE_USER
  *     TEXT = c_jls.JLS_ANNOTATION_TYPE_TEXT             # <<<<<<<<<<<<<<
  *     VMARKER = c_jls.JLS_ANNOTATION_TYPE_VERTICAL_MARKER
  *     HMARKER = c_jls.JLS_ANNOTATION_TYPE_HORIZONTAL_MARKER
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_TEXT, __pyx_t_3) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_TEXT, __pyx_t_3) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":140
+  /* "pyjls/binding.pyx":141
  *     USER = c_jls.JLS_ANNOTATION_TYPE_USER
  *     TEXT = c_jls.JLS_ANNOTATION_TYPE_TEXT
  *     VMARKER = c_jls.JLS_ANNOTATION_TYPE_VERTICAL_MARKER             # <<<<<<<<<<<<<<
  *     HMARKER = c_jls.JLS_ANNOTATION_TYPE_HORIZONTAL_MARKER
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_VERTICAL_MARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_VERTICAL_MARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_VMARKER, __pyx_t_3) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_VMARKER, __pyx_t_3) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":141
+  /* "pyjls/binding.pyx":142
  *     TEXT = c_jls.JLS_ANNOTATION_TYPE_TEXT
  *     VMARKER = c_jls.JLS_ANNOTATION_TYPE_VERTICAL_MARKER
  *     HMARKER = c_jls.JLS_ANNOTATION_TYPE_HORIZONTAL_MARKER             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_HORIZONTAL_MARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_annotation_type_e(JLS_ANNOTATION_TYPE_HORIZONTAL_MARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_HMARKER, __pyx_t_3) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_HMARKER, __pyx_t_3) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":137
+  /* "pyjls/binding.pyx":138
  * 
  * 
  * class AnnotationType:             # <<<<<<<<<<<<<<
  *     USER = c_jls.JLS_ANNOTATION_TYPE_USER
  *     TEXT = c_jls.JLS_ANNOTATION_TYPE_TEXT
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_AnnotationType, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_AnnotationType, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AnnotationType, __pyx_t_3) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AnnotationType, __pyx_t_3) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":145
+  /* "pyjls/binding.pyx":146
  * 
  * _annotation_map = {
  *     'user': AnnotationType.USER,             # <<<<<<<<<<<<<<
  *     'usr': AnnotationType.USER,
  *     'text': AnnotationType.TEXT,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_USER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_USER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_user, __pyx_t_7) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_user, __pyx_t_7) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":146
+  /* "pyjls/binding.pyx":147
  * _annotation_map = {
  *     'user': AnnotationType.USER,
  *     'usr': AnnotationType.USER,             # <<<<<<<<<<<<<<
  *     'text': AnnotationType.TEXT,
  *     'txt': AnnotationType.TEXT,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_USER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_USER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_usr, __pyx_t_3) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_usr, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":147
+  /* "pyjls/binding.pyx":148
  *     'user': AnnotationType.USER,
  *     'usr': AnnotationType.USER,
  *     'text': AnnotationType.TEXT,             # <<<<<<<<<<<<<<
  *     'txt': AnnotationType.TEXT,
  *     'str': AnnotationType.TEXT,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_7) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_7) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":148
+  /* "pyjls/binding.pyx":149
  *     'usr': AnnotationType.USER,
  *     'text': AnnotationType.TEXT,
  *     'txt': AnnotationType.TEXT,             # <<<<<<<<<<<<<<
  *     'str': AnnotationType.TEXT,
  *     'string': AnnotationType.TEXT,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_txt, __pyx_t_3) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_txt, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":149
+  /* "pyjls/binding.pyx":150
  *     'text': AnnotationType.TEXT,
  *     'txt': AnnotationType.TEXT,
  *     'str': AnnotationType.TEXT,             # <<<<<<<<<<<<<<
  *     'string': AnnotationType.TEXT,
  *     'marker': AnnotationType.VMARKER,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_str, __pyx_t_7) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_str, __pyx_t_7) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":150
+  /* "pyjls/binding.pyx":151
  *     'txt': AnnotationType.TEXT,
  *     'str': AnnotationType.TEXT,
  *     'string': AnnotationType.TEXT,             # <<<<<<<<<<<<<<
  *     'marker': AnnotationType.VMARKER,
  *     'vertical_marker': AnnotationType.VMARKER,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_string, __pyx_t_3) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_string, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":151
+  /* "pyjls/binding.pyx":152
  *     'str': AnnotationType.TEXT,
  *     'string': AnnotationType.TEXT,
  *     'marker': AnnotationType.VMARKER,             # <<<<<<<<<<<<<<
  *     'vertical_marker': AnnotationType.VMARKER,
  *     'vmarker': AnnotationType.VMARKER,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_VMARKER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_VMARKER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_marker, __pyx_t_7) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_marker, __pyx_t_7) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":152
+  /* "pyjls/binding.pyx":153
  *     'string': AnnotationType.TEXT,
  *     'marker': AnnotationType.VMARKER,
  *     'vertical_marker': AnnotationType.VMARKER,             # <<<<<<<<<<<<<<
  *     'vmarker': AnnotationType.VMARKER,
  *     'horizontal_marker': AnnotationType.HMARKER,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_VMARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_VMARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_vertical_marker, __pyx_t_3) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_vertical_marker, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":153
+  /* "pyjls/binding.pyx":154
  *     'marker': AnnotationType.VMARKER,
  *     'vertical_marker': AnnotationType.VMARKER,
  *     'vmarker': AnnotationType.VMARKER,             # <<<<<<<<<<<<<<
  *     'horizontal_marker': AnnotationType.HMARKER,
  *     'hmarker': AnnotationType.HMARKER,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_VMARKER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_VMARKER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_vmarker, __pyx_t_7) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_vmarker, __pyx_t_7) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":154
+  /* "pyjls/binding.pyx":155
  *     'vertical_marker': AnnotationType.VMARKER,
  *     'vmarker': AnnotationType.VMARKER,
  *     'horizontal_marker': AnnotationType.HMARKER,             # <<<<<<<<<<<<<<
  *     'hmarker': AnnotationType.HMARKER,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_HMARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_HMARKER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_horizontal_marker, __pyx_t_3) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_horizontal_marker, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":155
+  /* "pyjls/binding.pyx":156
  *     'vmarker': AnnotationType.VMARKER,
  *     'horizontal_marker': AnnotationType.HMARKER,
  *     'hmarker': AnnotationType.HMARKER,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AnnotationType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_HMARKER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_HMARKER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_hmarker, __pyx_t_7) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_hmarker, __pyx_t_7) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_annotation_map, __pyx_t_2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_annotation_map, __pyx_t_2) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":159
+  /* "pyjls/binding.pyx":160
  * 
  * _log_level_map = {
  *     '!': logging.CRITICAL,             # <<<<<<<<<<<<<<
  *     'A': logging.CRITICAL,
  *     'C': logging.CRITICAL,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u__42, __pyx_t_3) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u__42, __pyx_t_3) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":160
+  /* "pyjls/binding.pyx":161
  * _log_level_map = {
  *     '!': logging.CRITICAL,
  *     'A': logging.CRITICAL,             # <<<<<<<<<<<<<<
  *     'C': logging.CRITICAL,
  *     'E': logging.ERROR,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_A, __pyx_t_7) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_A, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":161
+  /* "pyjls/binding.pyx":162
  *     '!': logging.CRITICAL,
  *     'A': logging.CRITICAL,
  *     'C': logging.CRITICAL,             # <<<<<<<<<<<<<<
  *     'E': logging.ERROR,
  *     'W': logging.WARNING,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_C, __pyx_t_3) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_C, __pyx_t_3) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":162
+  /* "pyjls/binding.pyx":163
  *     'A': logging.CRITICAL,
  *     'C': logging.CRITICAL,
  *     'E': logging.ERROR,             # <<<<<<<<<<<<<<
  *     'W': logging.WARNING,
  *     'N': logging.INFO,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_E, __pyx_t_7) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_E, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":163
+  /* "pyjls/binding.pyx":164
  *     'C': logging.CRITICAL,
  *     'E': logging.ERROR,
  *     'W': logging.WARNING,             # <<<<<<<<<<<<<<
  *     'N': logging.INFO,
  *     'I': logging.INFO,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_W, __pyx_t_3) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_W, __pyx_t_3) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":164
+  /* "pyjls/binding.pyx":165
  *     'E': logging.ERROR,
  *     'W': logging.WARNING,
  *     'N': logging.INFO,             # <<<<<<<<<<<<<<
  *     'I': logging.INFO,
  *     'D': logging.DEBUG,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_INFO); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_INFO); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_N, __pyx_t_7) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_N, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":165
+  /* "pyjls/binding.pyx":166
  *     'W': logging.WARNING,
  *     'N': logging.INFO,
  *     'I': logging.INFO,             # <<<<<<<<<<<<<<
  *     'D': logging.DEBUG,
  *     'D': logging.DEBUG,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_I, __pyx_t_3) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_I, __pyx_t_3) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":166
+  /* "pyjls/binding.pyx":167
  *     'N': logging.INFO,
  *     'I': logging.INFO,
  *     'D': logging.DEBUG,             # <<<<<<<<<<<<<<
  *     'D': logging.DEBUG,
  *     'D': logging.DEBUG,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_D, __pyx_t_7) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_D, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":167
+  /* "pyjls/binding.pyx":168
  *     'I': logging.INFO,
  *     'D': logging.DEBUG,
  *     'D': logging.DEBUG,             # <<<<<<<<<<<<<<
  *     'D': logging.DEBUG,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_D, __pyx_t_3) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_D, __pyx_t_3) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":168
+  /* "pyjls/binding.pyx":169
  *     'D': logging.DEBUG,
  *     'D': logging.DEBUG,
  *     'D': logging.DEBUG,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_D, __pyx_t_7) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_D, __pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_map, __pyx_t_2) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_map, __pyx_t_2) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":172
+  /* "pyjls/binding.pyx":173
  * 
  * 
  * class SignalType:             # <<<<<<<<<<<<<<
  *     FSR = c_jls.JLS_SIGNAL_TYPE_FSR
  *     VSR = c_jls.JLS_SIGNAL_TYPE_VSR
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SignalType, __pyx_n_s_SignalType, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SignalType, __pyx_n_s_SignalType, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "pyjls/binding.pyx":173
+  /* "pyjls/binding.pyx":174
  * 
  * class SignalType:
  *     FSR = c_jls.JLS_SIGNAL_TYPE_FSR             # <<<<<<<<<<<<<<
  *     VSR = c_jls.JLS_SIGNAL_TYPE_VSR
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_FSR, __pyx_t_7) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_FSR, __pyx_t_7) < 0) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":174
+  /* "pyjls/binding.pyx":175
  * class SignalType:
  *     FSR = c_jls.JLS_SIGNAL_TYPE_FSR
  *     VSR = c_jls.JLS_SIGNAL_TYPE_VSR             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_VSR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_VSR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_VSR, __pyx_t_7) < 0) __PYX_ERR(0, 174, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_VSR, __pyx_t_7) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":172
+  /* "pyjls/binding.pyx":173
  * 
  * 
  * class SignalType:             # <<<<<<<<<<<<<<
  *     FSR = c_jls.JLS_SIGNAL_TYPE_FSR
  *     VSR = c_jls.JLS_SIGNAL_TYPE_VSR
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SignalType, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SignalType, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SignalType, __pyx_t_7) < 0) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SignalType, __pyx_t_7) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":177
+  /* "pyjls/binding.pyx":178
  * 
  * 
  * class SummaryFSR:             # <<<<<<<<<<<<<<
  *     MEAN = c_jls.JLS_SUMMARY_FSR_MEAN
  *     STD = c_jls.JLS_SUMMARY_FSR_STD
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SummaryFSR, __pyx_n_s_SummaryFSR, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SummaryFSR, __pyx_n_s_SummaryFSR, (PyObject *) NULL, __pyx_n_s_pyjls_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "pyjls/binding.pyx":178
+  /* "pyjls/binding.pyx":179
  * 
  * class SummaryFSR:
  *     MEAN = c_jls.JLS_SUMMARY_FSR_MEAN             # <<<<<<<<<<<<<<
  *     STD = c_jls.JLS_SUMMARY_FSR_STD
  *     MIN = c_jls.JLS_SUMMARY_FSR_MIN
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_MEAN); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_MEAN); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_MEAN, __pyx_t_7) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_MEAN, __pyx_t_7) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":179
+  /* "pyjls/binding.pyx":180
  * class SummaryFSR:
  *     MEAN = c_jls.JLS_SUMMARY_FSR_MEAN
  *     STD = c_jls.JLS_SUMMARY_FSR_STD             # <<<<<<<<<<<<<<
  *     MIN = c_jls.JLS_SUMMARY_FSR_MIN
  *     MAX = c_jls.JLS_SUMMARY_FSR_MAX
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_STD); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_STD); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_STD, __pyx_t_7) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_STD, __pyx_t_7) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":180
+  /* "pyjls/binding.pyx":181
  *     MEAN = c_jls.JLS_SUMMARY_FSR_MEAN
  *     STD = c_jls.JLS_SUMMARY_FSR_STD
  *     MIN = c_jls.JLS_SUMMARY_FSR_MIN             # <<<<<<<<<<<<<<
  *     MAX = c_jls.JLS_SUMMARY_FSR_MAX
  *     COUNT = c_jls.JLS_SUMMARY_FSR_COUNT
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_MIN); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_MIN); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_MIN, __pyx_t_7) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_MIN, __pyx_t_7) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":181
+  /* "pyjls/binding.pyx":182
  *     STD = c_jls.JLS_SUMMARY_FSR_STD
  *     MIN = c_jls.JLS_SUMMARY_FSR_MIN
  *     MAX = c_jls.JLS_SUMMARY_FSR_MAX             # <<<<<<<<<<<<<<
  *     COUNT = c_jls.JLS_SUMMARY_FSR_COUNT
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_MAX); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_MAX); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_MAX, __pyx_t_7) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_MAX, __pyx_t_7) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":182
+  /* "pyjls/binding.pyx":183
  *     MIN = c_jls.JLS_SUMMARY_FSR_MIN
  *     MAX = c_jls.JLS_SUMMARY_FSR_MAX
  *     COUNT = c_jls.JLS_SUMMARY_FSR_COUNT             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_COUNT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_COUNT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_COUNT, __pyx_t_7) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_COUNT, __pyx_t_7) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":177
+  /* "pyjls/binding.pyx":178
  * 
  * 
  * class SummaryFSR:             # <<<<<<<<<<<<<<
  *     MEAN = c_jls.JLS_SUMMARY_FSR_MEAN
  *     STD = c_jls.JLS_SUMMARY_FSR_STD
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SummaryFSR, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SummaryFSR, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SummaryFSR, __pyx_t_7) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SummaryFSR, __pyx_t_7) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":195
+  /* "pyjls/binding.pyx":196
  * 
  * 
  * c_jls.jls_log_register(_log_cbk)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   jls_log_register(__pyx_f_5pyjls_7binding__log_cbk);
 
-  /* "pyjls/binding.pyx":198
+  /* "pyjls/binding.pyx":199
  * 
  * 
  * def jls_inject_log(level, filename, line, msg):             # <<<<<<<<<<<<<<
  *     cdef char * c_msg
  *     location = ':'.join([filename, str(line), ''])
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_9jls_inject_log, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_9jls_inject_log, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jls_inject_log, __pyx_t_2) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jls_inject_log, __pyx_t_2) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":206
+  /* "pyjls/binding.pyx":207
  * 
  * 
  * def _encode_str(s):             # <<<<<<<<<<<<<<
  *     if s is None:
  *         s = ''
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_11_encode_str, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_11_encode_str, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_str, __pyx_t_2) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_str, __pyx_t_2) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":212
+  /* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
  *     if isinstance(data, str):
  *         s = _encode_str(data)
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_13_storage_pack, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_13_storage_pack, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_storage_pack, __pyx_t_2) < 0) __PYX_ERR(0, 212, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_storage_pack, __pyx_t_2) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":233
+  /* "pyjls/binding.pyx":234
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
- *     return int((utc - _UTC_OFFSET) * (2**30))
+ *     return int((utc - _UTC_OFFSET) * SECOND)
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_15utc_to_jls, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_15utc_to_jls, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_utc_to_jls, __pyx_t_2) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_utc_to_jls, __pyx_t_2) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":238
+  /* "pyjls/binding.pyx":239
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
- *     return (timestamp / (2**30)) + _UTC_OFFSET
+ *     return (timestamp / SECOND) + _UTC_OFFSET
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_17jls_to_utc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_17jls_to_utc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jls_to_utc, __pyx_t_2) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jls_to_utc, __pyx_t_2) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":243
+  /* "pyjls/binding.pyx":244
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_19_handle_rc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_19_handle_rc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_handle_rc, __pyx_t_2) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_handle_rc, __pyx_t_2) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_AnnotationCallback(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
@@ -33542,114 +33981,14 @@
     }
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
-/* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-#if PY_MAJOR_VERSION < 3 || CYTHON_USE_PYLONG_INTERNALS
-#define __Pyx_PyInt_TrueDivideObjC_ZeroDivisionError(operand)\
-    if (unlikely(zerodivision_check && ((operand) == 0))) {\
-        PyErr_SetString(PyExc_ZeroDivisionError, "integer division by zero");\
-        return NULL;\
-    }
-#endif
-static PyObject* __Pyx_PyInt_TrueDivideObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
-    (void)inplace;
-    (void)zerodivision_check;
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long a = PyInt_AS_LONG(op1);
-            __Pyx_PyInt_TrueDivideObjC_ZeroDivisionError(b)
-            if (8 * sizeof(long) <= 53 || likely(labs(a) <= ((PY_LONG_LONG)1 << 53))) {
-                return PyFloat_FromDouble((double)a / (double)b);
-            }
-            return PyInt_Type.tp_as_number->nb_true_divide(op1, op2);
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
-        } else {
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT && 1 * PyLong_SHIFT < 53) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT && 1 * PyLong_SHIFT < 53) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT && 2 * PyLong_SHIFT < 53) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT && 2 * PyLong_SHIFT < 53) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT && 3 * PyLong_SHIFT < 53) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT && 3 * PyLong_SHIFT < 53) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_true_divide(op1, op2);
-            }
-        }
-                __Pyx_PyInt_TrueDivideObjC_ZeroDivisionError(b)
-                if ((8 * sizeof(long) <= 53 || likely(labs(a) <= ((PY_LONG_LONG)1 << 53)))
-                        || __Pyx_sst_abs(size) <= 52 / PyLong_SHIFT) {
-                    return PyFloat_FromDouble((double)a / (double)b);
-                }
-                return PyLong_Type.tp_as_number->nb_true_divide(op1, op2);
-            return PyLong_FromLong(x);
-        
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-        double a = PyFloat_AS_DOUBLE(op1);
-            double result;
-            if (unlikely(zerodivision_check && b == 0)) {
-                PyErr_SetString(PyExc_ZeroDivisionError, "float division by zero");
-                return NULL;
-            }
-            PyFPE_START_PROTECT("divide", return NULL)
-            result = ((double)a) / (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
-    }
-    return (inplace ? PyNumber_InPlaceTrueDivide : PyNumber_TrueDivide)(op1, op2);
-}
-#endif
-
 /* PyIntCompare */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
     if (op1 == op2) {
         Py_RETURN_TRUE;
     }
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
```

### Comparing `pyjls-0.5.3/pyjls/entry_points/__init__.py` & `pyjls-0.6.0/pyjls/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/entry_points/annotate.py` & `pyjls-0.6.0/pyjls/entry_points/annotate.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/entry_points/info.py` & `pyjls-0.6.0/pyjls/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/structs.py` & `pyjls-0.6.0/pyjls/structs.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,21 +41,23 @@
     sample_rate: int = 0
     samples_per_data: int = 100000
     sample_decimate_factor: int = 1000
     entries_per_summary: int = 20000
     summary_decimate_factor: int = 100
     annotation_decimate_factor: int = 100
     utc_decimate_factor: int = 100
+    sample_id_offset: int = 0
     name: str = None
     units: str = None
     length: int = 0
 
     def info(self, verbose=None) -> str:
         strs = [f'{self.signal_id}: {self.name}']
         if verbose:
             for field in ['source_id', 'signal_type', 'data_type', 'sample_rate',
                           'samples_per_data', 'sample_decimate_factor',
                           'entries_per_summary', 'summary_decimate_factor',
                           'annotation_decimate_factor', 'utc_decimate_factor',
+                          'sample_id_offset',
                           'units', 'length']:
                 strs.append(f'    {field}: {getattr(self, field)}')
         return '\n'.join(strs)
```

### Comparing `pyjls-0.5.3/pyjls/test/__init__.py` & `pyjls-0.6.0/pyjls/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/test/test_binding.py` & `pyjls-0.6.0/pyjls/test/test_binding.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an 'AS IS' BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pyjls.binding import Writer, Reader, SummaryFSR, DataType, jls_inject_log
+from pyjls.binding import SECOND, Writer, Reader, SummaryFSR, DataType, jls_inject_log
 import io
 import logging
 from logging import StreamHandler
 import os
 import tempfile
 import unittest
 import numpy as np
@@ -36,14 +36,15 @@
         self.user_data.append(args)
 
     def _on_annotations(self, *args):
         self.annotations.append(args)
 
     def _on_utc(self, entries):
         self._utc.append(entries)
+        return False
 
     @property
     def utc(self):
         return np.concatenate(self._utc)
 
     def tearDown(self) -> None:
         if os.path.isfile(self._path):
@@ -175,36 +176,46 @@
     def test_annotation_seek(self):
         signal_id = 3
         expected = self._annotation_gen(signal_id)
         with Reader(self._path) as r:
             r.annotations(signal_id, expected[2][0], self._on_annotations)
         self.assertEqual(expected[2:], self.annotations)
 
-    def _utc_gen(self, signal_id):
-        signal_id = 3
+    def _utc_gen(self, signal_id, sample_id_offset=None):
+        sample_id_offset = 0 if sample_id_offset is None else int(sample_id_offset)
         data = []
         with Writer(self._path) as w:
             fs = 1000000
             w.source_def(source_id=1, name='name', vendor='vendor', model='model',
                          version='version', serial_number='serial_number')
             w.signal_def(signal_id=signal_id, source_id=1, sample_rate=fs, name='current', units='A')
-            w.fsr_f32(3, 0, np.array([1, 2, 3, 4], dtype=np.float32))
+            w.fsr_f32(3, sample_id_offset, np.array([1, 2, 3, 4], dtype=np.float32))
             for entry in range(100):
                 sample_id = entry * fs
-                timestamp = entry  # in seconds
+                timestamp = entry + 60 * 60 * 24 * 365  # in seconds
                 data.append([sample_id, timestamp])
-                w.utc(signal_id, entry * fs, entry)
+                w.utc(signal_id, sample_id + sample_id_offset, timestamp)
         return np.array(data, dtype=np.int64)
 
     def test_utc(self):
         signal_id = 3
-        expected = self._utc_gen(signal_id)
-        with Reader(self._path) as r:
-            r.utc(signal_id, 0, self._on_utc)
-        np.testing.assert_equal(expected, self.utc)
+        path_base, path_ext = os.path.splitext(self._path)
+        for idx in range(2):
+            self.subTest(idx)
+            self._path = f'{path_base}_{idx:04d}{path_ext}'
+            sample_id_offset = idx * 1_000_000
+            expected = self._utc_gen(signal_id, sample_id_offset=sample_id_offset)
+            with Reader(self._path) as r:
+                self.assertEqual(sample_id_offset, r.signals[signal_id].sample_id_offset)
+                r.utc(signal_id, 0, self._on_utc)
+                self.assertEqual(60 * 60 * 24 * 365, r.sample_id_to_timestamp(signal_id, 0))
+                self.assertEqual(0, r.timestamp_to_sample_id(signal_id, 60 * 60 * 24 * 365))
+            np.testing.assert_equal(expected, self.utc)
+            os.remove(self._path)
+            self._utc = []
 
     def test_utc_seek(self):
         signal_id = 3
         expected = self._utc_gen(signal_id)
         expected = expected[len(expected) // 2:, :]
         with Reader(self._path) as r:
             r.utc(signal_id, expected[0, 0], self._on_utc)
```

### Comparing `pyjls-0.5.3/pyjls/v1/__init__.py` & `pyjls-0.6.0/pyjls/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/pyjls/version.py` & `pyjls-0.6.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# Copyright 2021-2022 Jetperch LLC
+# Copyright 2022 Jetperch LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# See https://peps.python.org/pep-0518/
+# See https://toml.io/
 
-__version__ = "0.5.3"
-
-__title__ = "pyjls"
-__description__ = 'Joulescope™ file format'
-__url__ = 'https://joulescope.readthedocs.io'
-__author__ = 'Jetperch LLC'
-__author_email__ = 'joulescope-dev@jetperch.com'
-__license__ = 'Apache 2.0'
-__copyright__ = 'Copyright 2021-2022 Jetperch LLC'
-
-__all__ = ['__version__', '__title__', '__description__', '__url__',
-           '__author__', '__author_email__', '__license__',
-           '__copyright__']
+[build-system]
+# Minimum requirements for the build system to execute.
+requires = [
+    "Cython",
+    "numpy",
+    "pywin32; sys_platform == 'win32'",
+    "setuptools",
+    "wheel",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyjls-0.5.3/pyjls.egg-info/PKG-INFO` & `pyjls-0.6.0/pyjls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.5.3
+Version: 0.6.0
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.5.3/pyjls.egg-info/SOURCES.txt` & `pyjls-0.6.0/pyjls.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 include/jls/time.h
 include/jls/version.h
 include/jls/writer.h
 include_prv/jls/bit_shift.h
 include_prv/jls/cdef.h
 include_prv/jls/datatype.h
 include_prv/jls/msg_ring_buffer.h
+include_prv/jls/rd_fsr.h
 include_prv/jls/util.h
 include_prv/jls/wr_fsr.h
 include_prv/jls/wr_prv.h
 include_prv/jls/wr_ts.h
 pyjls/__init__.py
 pyjls/__main__.py
 pyjls/binding.c
@@ -51,13 +52,14 @@
 src/crc32c_intel_sse4.c
 src/crc32c_sw.c
 src/datatype.c
 src/ec.c
 src/log.c
 src/msg_ring_buffer.c
 src/raw.c
+src/rd_fsr.c
 src/reader.c
 src/statistics.c
 src/threaded_writer.c
 src/wr_fsr.c
 src/wr_ts.c
 src/writer.c
```

### Comparing `pyjls-0.5.3/setup.py` & `pyjls-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             'pyjls/binding' + ext,
             'src/bit_shift.c',
             'src/datatype.c',
             'src/ec.c',
             'src/log.c',
             'src/msg_ring_buffer.c',
             'src/raw.c',
+            'src/rd_fsr.c',
             'src/reader.c',
             'src/statistics.c',
             'src/threaded_writer.c',
             'src/wr_fsr.c',
             'src/wr_ts.c',
             'src/writer.c',
         ] + sources,
```

### Comparing `pyjls-0.5.3/src/backend_posix.c` & `pyjls-0.6.0/src/backend_posix.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/backend_win.c` & `pyjls-0.6.0/src/backend_win.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/bit_shift.c` & `pyjls-0.6.0/src/bit_shift.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/crc32c_arm_neon.c` & `pyjls-0.6.0/src/crc32c_arm_neon.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/crc32c_intel_sse4.c` & `pyjls-0.6.0/src/crc32c_intel_sse4.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/crc32c_sw.c` & `pyjls-0.6.0/src/crc32c_sw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/datatype.c` & `pyjls-0.6.0/src/datatype.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/ec.c` & `pyjls-0.6.0/src/ec.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/log.c` & `pyjls-0.6.0/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/msg_ring_buffer.c` & `pyjls-0.6.0/src/msg_ring_buffer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/raw.c` & `pyjls-0.6.0/src/raw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/reader.c` & `pyjls-0.6.0/src/reader.c`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #include "jls/reader.h"
 #include "jls/raw.h"
 #include "jls/format.h"
 #include "jls/datatype.h"
 #include "jls/ec.h"
 #include "jls/log.h"
 #include "jls/crc32c.h"
+#include "jls/rd_fsr.h"
 #include "jls/statistics.h"
 #include "jls/bit_shift.h"
 #include "jls/util.h"
 #include <inttypes.h>
 #include <math.h>
 #include <stdio.h>
 #include <stdlib.h>
@@ -104,14 +105,15 @@
 
 struct signal_s {
     int64_t timestamp_start;
     int64_t timestamp_end;
     int64_t track_defs[JLS_TRACK_TYPE_COUNT];
     int64_t track_head_offsets[JLS_TRACK_TYPE_COUNT];
     int64_t track_head_data[JLS_TRACK_TYPE_COUNT][JLS_SUMMARY_LEVEL_COUNT];
+    struct jls_rd_fsr_s * rd_fsr;
 };
 
 struct jls_rd_s {
     struct jls_raw_s * raw;
     struct jls_source_def_s source_def[JLS_SOURCE_COUNT];
     struct jls_source_def_s source_def_api[JLS_SOURCE_COUNT];
     struct jls_signal_def_s signal_def[JLS_SIGNAL_COUNT];
@@ -480,14 +482,39 @@
             break;
         }
         ROE(jls_raw_chunk_seek(self->raw, self->chunk_cur.hdr.item_next));
     }
     return 0;
 }
 
+static int32_t scan_fsr_sample_id(struct jls_rd_s * self) {
+    JLS_LOGD1("scan_fsr_sample_id");
+    for (uint32_t signal_id = 1; signal_id < JLS_SIGNAL_COUNT; ++signal_id) {
+        if ((self->signal_def[signal_id].signal_id != signal_id)
+                || (self->signal_def[signal_id].signal_type != JLS_SIGNAL_TYPE_FSR)) {
+            continue;
+        }
+        struct signal_s * s = &self->signals[signal_id];
+        int64_t offset = s->track_head_data[JLS_TRACK_TYPE_FSR][0];
+        if (offset == 0) {
+            continue;  // no data
+        }
+        ROE(jls_raw_chunk_seek(self->raw, offset));
+        ROE(rd(self));
+        if (self->chunk_cur.hdr.tag != JLS_TAG_TRACK_FSR_DATA) {
+            JLS_LOGW("scan_fsr_sample_id tag mismatch: %d", (int) self->chunk_cur.hdr.tag);
+            continue;
+        }
+
+        struct jls_fsr_data_s * r = (struct jls_fsr_data_s *) self->payload.start;
+        self->signal_def[signal_id].sample_id_offset = r->header.timestamp;
+    }
+    return 0;
+}
+
 static int32_t scan(struct jls_rd_s * self) {
     int32_t rc = 0;
     uint8_t found = 0;
 
     for (int i = 0; found != 7; ++i) {
         if (i == 3) {
             JLS_LOGW("malformed JLS, continue searching");
@@ -526,14 +553,15 @@
             default:
                 break;  // skip
         }
     }
     JLS_LOGD1("found initial tags");
     ROE(scan_sources(self));
     ROE(scan_signals(self));
+    ROE(scan_fsr_sample_id(self));
     return 0;
 }
 
 int32_t jls_rd_open(struct jls_rd_s ** instance, const char * path) {
     if (!instance) {
         return JLS_ERROR_PARAMETER_INVALID;
     }
@@ -642,14 +670,15 @@
         *signal = self->signal_def[signal_id];
     }
     return 0;
 }
 
 static int32_t ts_seek(struct jls_rd_s * self, uint16_t signal_id, uint8_t level,
                        enum jls_track_type_e track_type, int64_t timestamp) {
+    // timestamp in JLS units with possible non-zero offset
     if (!is_signal_defined(self, signal_id)) {
         return JLS_ERROR_NOT_FOUND;
     }
     switch (track_type) {
         case JLS_TRACK_TYPE_VSR: break;
         case JLS_TRACK_TYPE_ANNOTATION: break;
         case JLS_TRACK_TYPE_UTC: break;
@@ -693,15 +722,15 @@
         }
 
         int32_t idx = 0;
         for (; ; ++idx) {
             if (idx >= (int32_t) r->header.entry_count) {
                 idx = ((int32_t) r->header.entry_count) - 1;
                 break;
-            } else if (r->entries[idx].timestamp > timestamp) {
+            } else if (r->entries[idx].timestamp> timestamp) {
                 --idx;
                 break;
             } else if (r->entries[idx].timestamp == timestamp) {
                 break;
             }
         }
         if (idx < 0) {
@@ -711,14 +740,15 @@
     }
 
     ROE(jls_raw_chunk_seek(self->raw, offset));
     return 0;
 }
 
 static int32_t fsr_seek(struct jls_rd_s * self, uint16_t signal_id, uint8_t level, int64_t sample_id) {
+    // timestamp in JLS units with possible non-zero offset
     if (!is_signal_defined(self, signal_id)) {
         return JLS_ERROR_NOT_FOUND;
     }
     struct jls_signal_def_s * signal_def = &self->signal_def[signal_id];
     if (signal_def->signal_type != JLS_SIGNAL_TYPE_FSR) {
         JLS_LOGW("fsr_seek not support for signal type %d", (int) signal_def->signal_type);
         return JLS_ERROR_NOT_SUPPORTED;
@@ -734,15 +764,15 @@
         }
     }
     if (!offset) {
         return JLS_ERROR_NOT_FOUND;
     }
 
     for (int lvl = initial_level; lvl > level; --lvl) {
-        JLS_LOGD3("signal %d, level %d, index=%" PRIi64, (int) signal_id, (int) lvl, offset);
+        JLS_LOGD3("signal %d, level %d, offset=%" PRIi64, (int) signal_id, lvl, offset);
 
         // compute the step size in samples between each index entry.
         int64_t step_size = signal_def->samples_per_data;  // each data chunk
         if (lvl > 1) {
             step_size *= signal_def->entries_per_summary /
                     (signal_def->samples_per_data / signal_def->sample_decimate_factor);
         }
@@ -762,16 +792,17 @@
 
         if ((size_t) (p_end - self->payload.start) > self->payload.length) {
             JLS_LOGE("invalid payload length");
             return JLS_ERROR_PARAMETER_INVALID;
         }
 
         int64_t idx = (sample_id - chunk_timestamp) / step_size;
-        if (idx >= chunk_entries) {
+        if ((idx < 0) || (idx >= chunk_entries)) {
             JLS_LOGE("invalid index: %" PRIi64 " >= %" PRIi64, idx, chunk_entries);
+            return JLS_ERROR_IO;
         }
         offset = r->offsets[idx];
     }
 
     ROE(jls_raw_chunk_seek(self->raw, offset));
     return 0;
 }
@@ -821,21 +852,23 @@
             offset = r->offsets[r->header.entry_count - 1];
         }
     }
 
     ROE(jls_raw_chunk_seek(self->raw, offset));
     ROE(rd(self));
     r = (struct jls_fsr_index_s *) self->payload.start;
-    self->signal_length[signal_id] = r->header.timestamp + r->header.entry_count;
+    self->signal_length[signal_id] = r->header.timestamp + r->header.entry_count
+            - self->signal_def[signal_id].sample_id_offset;
     *samples = self->signal_length[signal_id];
     return 0;
 }
 
 int32_t jls_rd_fsr(struct jls_rd_s * self, uint16_t signal_id, int64_t start_sample_id,
                    void * data, int64_t data_length) {
+    // start_sample_id is API zero-based
     const int64_t data_length_orig = data_length;
     int32_t rv = 0;
     uint8_t * data_u8 = (uint8_t *) data;
     if (!is_signal_defined_type(self, signal_id, JLS_SIGNAL_TYPE_FSR)) {
         JLS_LOGW("signal_id %d invalid", (int) signal_id);
         return JLS_ERROR_PARAMETER_INVALID;
     }
@@ -843,14 +876,15 @@
         return 0;
     } else if (start_sample_id < 0) {
         JLS_LOGW("start_sample_id invalid: %" PRIi64, start_sample_id);
         return JLS_ERROR_PARAMETER_INVALID;
     }
 
     struct jls_signal_def_s * signal_def = &self->signal_def[signal_id];
+    const int64_t sample_id_offset = self->signal_def[signal_id].sample_id_offset;
     int64_t samples = 0;
     uint8_t entry_size_bits = jls_datatype_parse_size(signal_def->data_type);
 
     ROE(jls_rd_fsr_length(self, signal_id, &samples));
     if ((start_sample_id + data_length) > samples) {
         JLS_LOGW("length invalid: %" PRIi64 " > %" PRIi64,
                  start_sample_id + data_length, samples);
@@ -878,14 +912,15 @@
                 return JLS_ERROR_PARAMETER_INVALID;
         }
         data_length += start_sample_id - sample_id;
         start_sample_id = sample_id;
     }
 
     //JLS_LOGD3("jls_rd_fsr_f32(%d, %" PRIi64 ")", (int) signal_id, start_sample_id);
+    start_sample_id += sample_id_offset;  // file sample_id
     ROE(fsr_seek(self, signal_id, 0, start_sample_id));
     self->chunk_cur.hdr.item_next = jls_raw_chunk_tell(self->raw);
     while (data_length > 0) {
         if (jls_raw_chunk_seek(self->raw, self->chunk_cur.hdr.item_next)) {
             return JLS_ERROR_NOT_FOUND;
         }
         rv = rd(self);
@@ -993,23 +1028,26 @@
     */
     return 0;
 }
 
 static int32_t fsr_statistics(struct jls_rd_s * self, uint16_t signal_id,
                               int64_t start_sample_id, int64_t increment, uint8_t level,
                               double * data, int64_t data_length) {
+    // start_sample_id in JLS units with possible non-zero offset
     JLS_LOGD2("fsr_f32_statistics(signal_id=%d, start_id=%" PRIi64 ", incr=%" PRIi64 ", level=%d, len=%" PRIi64 ")",
               (int) signal_id, start_sample_id, increment, (int) level, data_length);
     bool is_f32;
     struct jls_signal_def_s * signal_def = &self->signal_def[signal_id];
     int64_t step_size = signal_def->sample_decimate_factor;
     for (uint8_t lvl = 2; lvl <= level; ++lvl) {
         step_size *= signal_def->summary_decimate_factor;
     }
     double f64_tmp4[JLS_SUMMARY_FSR_COUNT];
+    const int64_t sample_id_offset = self->signal_def[signal_id].sample_id_offset;
+
     ROE(fsr_seek(self, signal_id, level, start_sample_id)); // returns the index
     ROE(jls_raw_chunk_next(self->raw));  // statistics
     int64_t pos = jls_raw_chunk_tell(self->raw);
     ROE(rd_stats_chunk(self, signal_id, level));
 
     struct jls_fsr_f32_summary_s * f32_summary = (struct jls_fsr_f32_summary_s *) self->payload.start;
     struct jls_fsr_f64_summary_s * f64_summary = (struct jls_fsr_f64_summary_s *) self->payload.start;
@@ -1031,16 +1069,17 @@
     jls_statistics_reset(&stats_accum);
     struct jls_statistics_s stats_next;
 
     int64_t incr_remaining = increment;
 
     if (entry_sample_id != start_sample_id) {
         int64_t incr = entry_sample_id - start_sample_id;
-        // invalidates stats, need to reload
-        ROE(jls_rd_fsr_statistics(self, signal_id, start_sample_id, incr, f64_tmp4, 1));
+        // invalidates stats, need to reload, providing API sample_id
+        ROE(jls_rd_fsr_statistics(self, signal_id, start_sample_id - sample_id_offset,
+                                  incr, f64_tmp4, 1));
         ROE(jls_raw_chunk_seek(self->raw, pos));
         ROE(rd_stats_chunk(self, signal_id, level));
         f64_to_stats(&stats_accum, f64_tmp4, incr);
         incr_remaining -= incr;
         start_sample_id += incr;
     }
     src_offset += entry_offset;
@@ -1073,15 +1112,16 @@
                     return JLS_ERROR_PARAMETER_INVALID;
                 }
             }
         }
 
         if (incr_remaining <= step_size) {
             if (data_length == 1) {
-                ROE(jls_rd_fsr_statistics(self, signal_id, start_sample_id, incr_remaining, f64_tmp4, 1));
+                ROE(jls_rd_fsr_statistics(self, signal_id, start_sample_id - sample_id_offset,
+                                          incr_remaining, f64_tmp4, 1));
                 f64_to_stats(&stats_next, f64_tmp4, incr_remaining);
             } else if (is_f32) {
                 f32_to_stats(&stats_next, f32_summary->data[src_offset], incr_remaining);
             } else {
                 f64_to_stats(&stats_next, f64_summary->data[src_offset], incr_remaining);
             }
             jls_statistics_combine(&stats_accum, &stats_accum, &stats_next);
@@ -1114,14 +1154,15 @@
     }
     return 0;
 }
 
 int32_t jls_rd_fsr_statistics(struct jls_rd_s * self, uint16_t signal_id,
                               int64_t start_sample_id, int64_t increment,
                               double * data, int64_t data_length) {
+    // API zero-based start_sample_id
     if (!is_signal_defined_type(self, signal_id, JLS_SIGNAL_TYPE_FSR)) {
         JLS_LOGW("signal_id %d invalid", (int) signal_id);
         return JLS_ERROR_PARAMETER_INVALID;
     } else if (increment <= 0) {
         JLS_LOGW("invalid increment: %" PRIi64, increment);
         return JLS_ERROR_PARAMETER_INVALID;
     } else if (data_length <= 0) {
@@ -1130,29 +1171,31 @@
     } else if (start_sample_id < 0) {
         JLS_LOGW("invalid start_sample_id: %" PRIi64, start_sample_id);
         return JLS_ERROR_PARAMETER_INVALID;
     }
 
     int64_t samples = 0;
     ROE(jls_rd_fsr_length(self, signal_id, &samples));
-    if ((start_sample_id + increment * data_length) > samples) {
-        JLS_LOGW("invalid length: %" PRIi64 " > %" PRIi64,
-                 start_sample_id + increment * data_length, samples);
+    int64_t end_sample_id = start_sample_id + increment * data_length;
+    if (end_sample_id > samples) {
+        JLS_LOGW("invalid length: %" PRIi64 " > %" PRIi64, end_sample_id, samples);
         return JLS_ERROR_PARAMETER_INVALID;
     }
+    const int64_t sample_id_offset = self->signal_def[signal_id].sample_id_offset;
 
     struct jls_signal_def_s * signal_def = &self->signal_def[signal_id];
     uint8_t level = 0;
     int64_t sample_multiple_next = signal_def->sample_decimate_factor;
     int64_t duration = increment * data_length;
     while ((increment >= sample_multiple_next)
             && (duration >= (DECIMATE_PER_DURATION * sample_multiple_next))) {
         ++level;
         sample_multiple_next *= signal_def->summary_decimate_factor;
     }
+    start_sample_id += sample_id_offset; // JLS file sample_id
 
     if (level) {  // use summaries
         return fsr_statistics(self, signal_id, start_sample_id, increment, level, data, data_length);
     }  // else, use sample data
     JLS_LOGD2("f32(signal_id=%d, start_id=%" PRIi64 ", incr=%" PRIi64 ", level=0, len=%" PRIi64 ")",
               (int) signal_id, start_sample_id, increment, data_length);
 
@@ -1251,14 +1294,17 @@
     if (!cbk_fn) {
         return JLS_ERROR_PARAMETER_INVALID;
     }
     if (!is_signal_defined(self, signal_id)) {
         return JLS_ERROR_NOT_FOUND;
     }
 
+    const int64_t sample_id_offset = self->signal_def[signal_id].sample_id_offset;
+    timestamp += sample_id_offset;
+
     int32_t rv = ts_seek(self, signal_id, 0, JLS_TRACK_TYPE_ANNOTATION, timestamp);
     if (rv == JLS_ERROR_NOT_FOUND) {
         return 0;  // no annotations, and that's just fine
     } else if (rv) {
         return rv;
     }
 
@@ -1267,14 +1313,15 @@
     while (pos) {
         ROE(jls_raw_chunk_seek(self->raw, pos));
         ROE(rd(self));
         if (self->chunk_cur.hdr.tag != JLS_TAG_TRACK_ANNOTATION_DATA) {
             return JLS_ERROR_NOT_FOUND;
         }
         annotation = (struct jls_annotation_s *) self->payload.start;
+        annotation->timestamp -= sample_id_offset;
         if (cbk_fn(cbk_user_data, annotation)) {
             return 0;
         }
         pos = self->chunk_cur.hdr.item_next;
     }
     return 0;
 }
@@ -1318,14 +1365,16 @@
     if (!cbk_fn) {
         return JLS_ERROR_PARAMETER_INVALID;
     }
     if (!is_signal_defined(self, signal_id)) {
         return JLS_ERROR_NOT_FOUND;
     }
 
+    const int64_t sample_id_offset = self->signal_def[signal_id].sample_id_offset;
+    sample_id += sample_id_offset;
     int32_t rv = ts_seek(self, signal_id, 1, JLS_TRACK_TYPE_UTC, sample_id);
     if (rv == JLS_ERROR_NOT_FOUND) {
         return 0;  // no utc entries, and that's just fine
     } else if (rv) {
         return rv;
     }
 
@@ -1346,15 +1395,45 @@
         }
         utc = (struct jls_utc_summary_s *) self->payload.start;
         uint32_t idx = 0;
         for (; (idx < utc->header.entry_count) && (sample_id > utc->entries[idx].sample_id); ++idx) {
             // iterate
         }
         uint32_t size = utc->header.entry_count - idx;
+        for (uint32_t entry_idx = idx; entry_idx < utc->header.entry_count; ++entry_idx) {
+            utc->entries[entry_idx].sample_id -= sample_id_offset;
+        }
         if (size) {
             if (cbk_fn(cbk_user_data, utc->entries + idx, size)) {
                 return 0;
             }
         }
     }
     return 0;
 }
+
+static int32_t utc_load(struct jls_rd_s * self, uint16_t signal_id) {
+    if (!is_signal_defined_type(self, signal_id, JLS_SIGNAL_TYPE_FSR)) {
+        return JLS_ERROR_NOT_FOUND;
+    }
+    struct signal_s * signal = &self->signals[signal_id];
+    if (NULL != signal->rd_fsr) {
+        return 0;
+    }
+    signal->rd_fsr = jls_rd_fsr_alloc(self->signal_def[signal_id].sample_rate);
+    if (NULL == signal->rd_fsr) {
+        return JLS_ERROR_NOT_ENOUGH_MEMORY;
+    }
+    return jls_rd_utc(self, signal_id, 0, jls_rd_fsr_add_cbk, signal->rd_fsr);
+}
+
+int32_t jls_rd_sample_id_to_timestamp(struct jls_rd_s * self, uint16_t signal_id,
+                                      int64_t sample_id, int64_t * timestamp) {
+    ROE(utc_load(self, signal_id));
+    return jls_rd_fsr_sample_id_to_timestamp(self->signals[signal_id].rd_fsr, sample_id, timestamp);
+}
+
+int32_t jls_rd_timestamp_to_sample_id(struct jls_rd_s * self, uint16_t signal_id,
+                                              int64_t timestamp, int64_t * sample_id) {
+    ROE(utc_load(self, signal_id));
+    return jls_rd_fsr_timestamp_to_sample_id(self->signals[signal_id].rd_fsr, timestamp, sample_id);
+}
```

### Comparing `pyjls-0.5.3/src/statistics.c` & `pyjls-0.6.0/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/threaded_writer.c` & `pyjls-0.6.0/src/threaded_writer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/wr_fsr.c` & `pyjls-0.6.0/src/wr_fsr.c`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
 struct jls_wr_fsr_s {
     struct jls_wr_s * wr;
     struct jls_signal_def_s def;
     uint32_t data_length;  // for data, in samples
     struct jls_fsr_data_s * data;  // for level 0
     double * data_f64;
-    struct level_s * level[JLS_SUMMARY_LEVEL_COUNT];  // level 0 unused
     int64_t sample_id_offset;
+    struct level_s * level[JLS_SUMMARY_LEVEL_COUNT];  // level 0 unused
 };
 
 static int32_t summaryN(struct jls_wr_fsr_s * self, uint8_t level, int64_t pos);
 static int32_t summary1(struct jls_wr_fsr_s * self, int64_t pos);
 
 static inline uint8_t sample_size_bits(struct jls_wr_fsr_s * self) {
     return jls_datatype_parse_size(self->def.data_type);
@@ -134,22 +134,22 @@
     memset(b, 0, sizeof(struct level_s));
     b->level = level;
     b->index_entries = index_entries;
     b->summary_entries = self->def.entries_per_summary;
     buffer += sizeof(struct level_s);
 
     b->index = (struct jls_fsr_index_s *) buffer;
-    b->index->header.timestamp = 0;
+    b->index->header.timestamp = self->sample_id_offset;
     b->index->header.entry_count = 0;
     b->index->header.entry_size_bits = sizeof(b->index->offsets[0]) * 8;
     b->index->header.rsv16 = 0;
     buffer += index_sz;
 
     b->summary = (struct jls_fsr_f32_summary_s *) buffer;  // actually jls_fsr_f32_summary_s or jls_fsr_f64_summary_s
-    b->summary->header.timestamp = 0;
+    b->summary->header.timestamp = self->sample_id_offset;
     b->summary->header.entry_count = 0;
     b->summary->header.entry_size_bits = (uint16_t) (JLS_SUMMARY_FSR_COUNT * dt_sz_bits);
     b->summary->header.rsv16 = 0;
 
     self->level[level] = b;
     return 0;
 }
@@ -519,17 +519,16 @@
         default:
             break;
     }
 
     if (!b) {
         ROE(sample_buffer_alloc(self));
         b = self->data;
-        self->sample_id_offset = sample_id;
+        self->sample_id_offset = sample_id;  // can be nonzero
     }
-    sample_id -= self->sample_id_offset;
 
     // todo check for & handle sample_id skips
     if (!b->header.entry_count) {
         b->header.timestamp = sample_id;
     }
 
     while (data_length) {
```

### Comparing `pyjls-0.5.3/src/wr_ts.c` & `pyjls-0.6.0/src/wr_ts.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.5.3/src/writer.c` & `pyjls-0.6.0/src/writer.c`

 * *Files identical despite different names*

