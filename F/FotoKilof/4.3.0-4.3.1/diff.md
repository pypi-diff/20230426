# Comparing `tmp/FotoKilof-4.3.0.tar.gz` & `tmp/FotoKilof-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FotoKilof-4.3.0.tar", last modified: Tue Apr 25 00:01:00 2023, max compression
+gzip compressed data, was "FotoKilof-4.3.1.tar", last modified: Tue Apr 25 19:49:10 2023, max compression
```

## Comparing `FotoKilof-4.3.0.tar` & `FotoKilof-4.3.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5622 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/CHANGES.md
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1003 2020-02-11 22:24:58.000000 FotoKilof-4.3.0/CONTRIBUTING.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/FotoKilof.egg-info/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5369 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/PKG-INFO
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1188 2023-04-25 00:01:00.000000 FotoKilof-4.3.0/FotoKilof.egg-info/SOURCES.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)        1 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/dependency_links.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       45 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/entry_points.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       25 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/requires.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       10 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/FotoKilof.egg-info/top_level.txt
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1083 2023-01-25 17:40:54.000000 FotoKilof-4.3.0/LICENSE
--rw-rw-r--   0 tlu       (1000) tlu       (1000)      208 2022-12-11 22:24:11.000000 FotoKilof-4.3.0/MANIFEST.in
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     5369 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/PKG-INFO
--rw-rw-r--   0 tlu       (1000) tlu       (1000)      696 2022-12-27 19:31:14.000000 FotoKilof-4.3.0/PROGRAM_GUIDE.md
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4845 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/README.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/doc/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/doc/en/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7934 2021-08-24 09:13:03.000000 FotoKilof-4.3.0/doc/en/fotokilof.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/doc/pl/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    10704 2021-08-24 09:23:40.000000 FotoKilof-4.3.0/doc/pl/fotokilof.md
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/fotokilof/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1232 2023-04-25 00:00:59.000000 FotoKilof-4.3.0/fotokilof/__init__.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)   109944 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/fotokilof/__main__.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7911 2023-02-25 15:39:02.000000 FotoKilof-4.3.0/fotokilof/common.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3704 2023-01-14 16:46:10.000000 FotoKilof-4.3.0/fotokilof/convert.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    10946 2023-02-25 23:07:28.000000 FotoKilof-4.3.0/fotokilof/convert_wand.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2324 2021-08-22 10:05:08.000000 FotoKilof-4.3.0/fotokilof/entries.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2329 2023-01-14 12:59:21.000000 FotoKilof-4.3.0/fotokilof/gui.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    17389 2023-02-25 15:43:09.000000 FotoKilof-4.3.0/fotokilof/ini_read.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7620 2023-02-02 19:03:24.000000 FotoKilof-4.3.0/fotokilof/ini_save.py
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.110741 FotoKilof-4.3.0/fotokilof/locale/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/bg/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4538 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     8627 2021-08-22 21:54:10.000000 FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/de/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3927 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7738 2021-08-22 21:54:36.000000 FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/en/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4420 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7567 2021-08-22 21:55:08.000000 FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.po
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    16461 2023-01-25 20:12:16.000000 FotoKilof-4.3.0/fotokilof/locale/fotokilof.pot
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/id/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     3312 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7602 2021-08-22 21:55:36.000000 FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/pl/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    18673 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)    24151 2023-01-25 20:13:53.000000 FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.106741 FotoKilof-4.3.0/fotokilof/locale/tr/
-drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4277 2023-04-24 23:35:16.000000 FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     7216 2022-12-03 17:15:26.000000 FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2630 2023-01-14 16:53:17.000000 FotoKilof-4.3.0/fotokilof/log.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     2361 2022-12-29 00:42:19.000000 FotoKilof-4.3.0/fotokilof/magick.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1480 2021-08-17 16:35:46.000000 FotoKilof-4.3.0/fotokilof/mswindows.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     4284 2023-03-09 22:49:13.000000 FotoKilof-4.3.0/fotokilof/preview.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1378 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/fotokilof/version.py
--rw-rw-r--   0 tlu       (1000) tlu       (1000)       38 2023-04-25 00:01:00.114741 FotoKilof-4.3.0/setup.cfg
--rw-rw-r--   0 tlu       (1000) tlu       (1000)     1050 2023-04-24 23:46:25.000000 FotoKilof-4.3.0/setup.py
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5622 2023-04-24 23:46:25.000000 FotoKilof-4.3.1/CHANGES.md
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1003 2020-02-11 22:24:58.000000 FotoKilof-4.3.1/CONTRIBUTING.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.166597 FotoKilof-4.3.1/FotoKilof.egg-info/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5369 2023-04-25 19:49:09.000000 FotoKilof-4.3.1/FotoKilof.egg-info/PKG-INFO
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1188 2023-04-25 19:49:10.000000 FotoKilof-4.3.1/FotoKilof.egg-info/SOURCES.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)        1 2023-04-25 19:49:09.000000 FotoKilof-4.3.1/FotoKilof.egg-info/dependency_links.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       45 2023-04-25 19:49:09.000000 FotoKilof-4.3.1/FotoKilof.egg-info/entry_points.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       25 2023-04-25 19:49:09.000000 FotoKilof-4.3.1/FotoKilof.egg-info/requires.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       10 2023-04-25 19:49:09.000000 FotoKilof-4.3.1/FotoKilof.egg-info/top_level.txt
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1083 2023-01-25 17:40:54.000000 FotoKilof-4.3.1/LICENSE
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)      208 2022-12-11 22:24:11.000000 FotoKilof-4.3.1/MANIFEST.in
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     5369 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/PKG-INFO
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)      696 2022-12-27 19:31:14.000000 FotoKilof-4.3.1/PROGRAM_GUIDE.md
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4845 2023-04-24 23:46:25.000000 FotoKilof-4.3.1/README.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.162597 FotoKilof-4.3.1/doc/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.166597 FotoKilof-4.3.1/doc/en/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7934 2021-08-24 09:13:03.000000 FotoKilof-4.3.1/doc/en/fotokilof.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.166597 FotoKilof-4.3.1/doc/pl/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    10704 2021-08-24 09:23:40.000000 FotoKilof-4.3.1/doc/pl/fotokilof.md
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1232 2023-04-25 19:49:09.000000 FotoKilof-4.3.1/fotokilof/__init__.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)   110157 2023-04-25 19:45:41.000000 FotoKilof-4.3.1/fotokilof/__main__.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7911 2023-02-25 15:39:02.000000 FotoKilof-4.3.1/fotokilof/common.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3704 2023-01-14 16:46:10.000000 FotoKilof-4.3.1/fotokilof/convert.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    10946 2023-02-25 23:07:28.000000 FotoKilof-4.3.1/fotokilof/convert_wand.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2324 2021-08-22 10:05:08.000000 FotoKilof-4.3.1/fotokilof/entries.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2329 2023-01-14 12:59:21.000000 FotoKilof-4.3.1/fotokilof/gui.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    17389 2023-02-25 15:43:09.000000 FotoKilof-4.3.1/fotokilof/ini_read.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7620 2023-02-02 19:03:24.000000 FotoKilof-4.3.1/fotokilof/ini_save.py
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/locale/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.162597 FotoKilof-4.3.1/fotokilof/locale/bg/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4538 2023-04-25 19:46:52.000000 FotoKilof-4.3.1/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     8627 2021-08-22 21:54:10.000000 FotoKilof-4.3.1/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.162597 FotoKilof-4.3.1/fotokilof/locale/de/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3927 2023-04-25 19:46:52.000000 FotoKilof-4.3.1/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7738 2021-08-22 21:54:36.000000 FotoKilof-4.3.1/fotokilof/locale/de/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.162597 FotoKilof-4.3.1/fotokilof/locale/en/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4420 2023-04-25 19:46:52.000000 FotoKilof-4.3.1/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7567 2021-08-22 21:55:08.000000 FotoKilof-4.3.1/fotokilof/locale/en/LC_MESSAGES/fotokilof.po
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    16461 2023-01-25 20:12:16.000000 FotoKilof-4.3.1/fotokilof/locale/fotokilof.pot
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.162597 FotoKilof-4.3.1/fotokilof/locale/id/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     3312 2023-04-25 19:46:52.000000 FotoKilof-4.3.1/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7602 2021-08-22 21:55:36.000000 FotoKilof-4.3.1/fotokilof/locale/id/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.162597 FotoKilof-4.3.1/fotokilof/locale/pl/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    18673 2023-04-25 19:46:52.000000 FotoKilof-4.3.1/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)    24151 2023-01-25 20:13:53.000000 FotoKilof-4.3.1/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.162597 FotoKilof-4.3.1/fotokilof/locale/tr/
+drwxrwxr-x   0 tlu       (1000) tlu       (1000)        0 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/fotokilof/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4277 2023-04-25 19:46:52.000000 FotoKilof-4.3.1/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     7216 2022-12-03 17:15:26.000000 FotoKilof-4.3.1/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2630 2023-01-14 16:53:17.000000 FotoKilof-4.3.1/fotokilof/log.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     2361 2022-12-29 00:42:19.000000 FotoKilof-4.3.1/fotokilof/magick.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1480 2021-08-17 16:35:46.000000 FotoKilof-4.3.1/fotokilof/mswindows.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     4284 2023-03-09 22:49:13.000000 FotoKilof-4.3.1/fotokilof/preview.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1378 2023-04-25 19:24:29.000000 FotoKilof-4.3.1/fotokilof/version.py
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)       38 2023-04-25 19:49:10.170597 FotoKilof-4.3.1/setup.cfg
+-rw-rw-r--   0 tlu       (1000) tlu       (1000)     1050 2023-04-24 23:46:25.000000 FotoKilof-4.3.1/setup.py
```

### Comparing `FotoKilof-4.3.0/CHANGES.md` & `FotoKilof-4.3.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/CONTRIBUTING.md` & `FotoKilof-4.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/FotoKilof.egg-info/PKG-INFO` & `FotoKilof-4.3.1/FotoKilof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FotoKilof
-Version: 4.3.0
+Version: 4.3.1
 Summary: Nice gui for ImageMagick
 Home-page: https://github.com/TeaM-TL/FotoKilof
 Author: Tomasz Łuczak
 Author-email: tlu@team-tl.pl
 License: MIT
 Keywords: GUI ImageMagick FotoKilof
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FotoKilof-4.3.0/FotoKilof.egg-info/SOURCES.txt` & `FotoKilof-4.3.1/FotoKilof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/LICENSE` & `FotoKilof-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/PKG-INFO` & `FotoKilof-4.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FotoKilof
-Version: 4.3.0
+Version: 4.3.1
 Summary: Nice gui for ImageMagick
 Home-page: https://github.com/TeaM-TL/FotoKilof
 Author: Tomasz Łuczak
 Author-email: tlu@team-tl.pl
 License: MIT
 Keywords: GUI ImageMagick FotoKilof
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FotoKilof-4.3.0/PROGRAM_GUIDE.md` & `FotoKilof-4.3.1/PROGRAM_GUIDE.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/README.md` & `FotoKilof-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/doc/en/fotokilof.md` & `FotoKilof-4.3.1/doc/en/fotokilof.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/doc/pl/fotokilof.md` & `FotoKilof-4.3.1/doc/pl/fotokilof.md`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/__init__.py` & `FotoKilof-4.3.1/fotokilof/__init__.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/__main__.py` & `FotoKilof-4.3.1/fotokilof/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 import sys
 import tempfile
 
 import ttkbootstrap as ttk
 from ttkbootstrap.scrolled import ScrolledText, ScrolledFrame
 from ttkbootstrap.tooltip import ToolTip
 from ttkbootstrap.dialogs.colorchooser import ColorChooserDialog
-from ttkbootstrap.constants import N, S, W, E, X, BOTH, LEFT, RIGHT, TOP, BOTTOM, END, DISABLED, NORMAL, HORIZONTAL
+from ttkbootstrap.constants import N, S, W, E, X, BOTH, LEFT, RIGHT, TOP, BOTTOM, END, \
+                                    DISABLED, NORMAL, HORIZONTAL
 
 # my modules
 import convert
 import convert_wand
 import common
 import gui
 import ini_read
@@ -98,15 +99,15 @@
 else:
     PREVIEW_ORIG = 450
     PREVIEW_NEW = 450
     PREVIEW_LOGO = 100
 
 preview_size_list = (300, 350, 400, 450, 500, 550, 600, 650, 700, 800,
         900, 1000, 1200, 1400, 1600, 1800, 1920, 'none')
-##########################
+###################
 
 
 def print_command(cmd):
     """ print command in custom window """
     t_custom.insert(END, cmd + " ")
 
 
@@ -705,58 +706,61 @@
         except:
             log.write_log('open_screenshot(), error in make screeshot ', 'E')
             do_it = 1
     if do_it:
         open_file_common(today_dir, filename)
 
 
-def askcolor(initial):
+def ask_color(initial):
     """ Use color widget ColorChooserDialog from ttkbootstrap"""
-    cd = ColorChooserDialog()
-    cd.show()
-    colors = cd.result
-    result = colors.hex
+    color_dialog = ColorChooserDialog(initialcolor=initial)
+    color_dialog.show()
+    colors = color_dialog.result
+    if colors:
+        result = colors.hex
+    else:
+        result = None
     return result
 
 
 def color_choose_rotate():
     """ color selection for rotate"""
-    color = askcolor(img_rotate_color.get())
+    color = ask_color(img_rotate_color.get())
     if color is not None:
         img_rotate_color.set(color)
         l_rotate_color.configure(bg=color)
 
 
 def color_choose_border():
     """ Border color selection """
-    color = askcolor(img_border_color.get())
+    color = ask_color(img_border_color.get())
     if color is not None:
         img_border_color.set(color)
         l_border_color.configure(bg=color)
 
 
 def color_choose_vignette():
     """ color selection for rotate"""
-    color = askcolor(img_vignette_color.get())
+    color = ask_color(img_vignette_color.get())
     if color is not None:
         img_vignette_color.set(color)
         l_vignette_color.configure(bg=color)
 
 
 def color_choose_box():
     """ Background color selection """
-    color = askcolor(img_text_color.get())
+    color = ask_color(img_text_color.get())
     if color is not None:
         img_text_box_color.set(color)
         l_text_color.configure(bg=img_text_box_color.get())
 
 
 def color_choose():
     """ Color selection """
-    color = askcolor(img_text_color.get())
+    color = ask_color(img_text_color.get())
     if color is not None:
         img_text_color.set(color)
         l_text_color.configure(fg=img_text_color.get())
 
 
 def ini_read_wraper():
     """ Read config INI file """
@@ -1091,15 +1095,15 @@
                 x0 = int(x0 * ratio_x)
                 y0 = int(y0 * ratio_y)
                 x1 = int(x1 * ratio_x)
                 y1 = int(y1 * ratio_y)
 
                 crop_rectangle = (x0, y0, x1, y1)
             else:
-                crop_rectangle = (" ")
+                crop_rectangle = ""
 
             preview_picture = preview.preview_wand(file_in_path.get(),
                                                   int(co_preview_selector_orig.get()),
                                                   crop_rectangle)
 
             try:
                 pi_preview_orig.configure(file=preview_picture['filename'])
@@ -1366,16 +1370,16 @@
         frame_text_rotate.grid()
 
 
 ###############################################################################
 # GUI main window
 ###############################################################################
 
-#root = Tk()
-root = ttk.Window(resizable=(1,1), title=version.__author__ + " : " + version.__appname__ + " " + version.__version__)
+title_begin = version.__author__ + " : " + version.__appname__ + " " + version.__version__
+root = ttk.Window(resizable=(1,1), title=title_begin)
 ttk.Sizegrip()
 # hidden file
 # https://code.activestate.com/lists/python-tkinter-discuss/3723/
 try:
     # call a dummy dialog with an impossible option to initialize the file
     # dialog without really getting a dialog window; this will throw a
     # TclError, so we need a try...except :
@@ -1463,16 +1467,16 @@
 main_progress.pack(side=BOTTOM, expand=0, fill=X, anchor=S)
 main_paned.pack(side=BOTTOM, expand=1, fill=BOTH)
 
 
 validation = main_paned.register(gui.only_numbers)  # Entry validation
 validationint = main_paned.register(gui.only_integer)  # Entry validation integer value
 ####################################################################
-progressbar = ttk.Progressbar(main_progress, orient=HORIZONTAL, bootstyle="info", mode='determinate',
-                                variable=progressbar_var, maximum=100)
+progressbar = ttk.Progressbar(main_progress, orient=HORIZONTAL, bootstyle="info",
+                            mode='determinate', variable=progressbar_var, maximum=100)
 progressbar.pack(side=BOTTOM, padx=0, pady=0, fill=X, expand=0, anchor=S)
 ####################################################################
 # main_menu row
 ####################################################################
 ###########################
 # Picture selection
 ###########################
@@ -1533,16 +1537,18 @@
 
 ###########################
 # Buttons
 ###########################
 frame_save = ttk.LabelFrame(main_menu, text=_("Settings"))
 frame_save.grid(row=1, column=3, sticky=(N, W, E, S), padx=5, pady=5)
 
-b_last_save = ttk.Button(frame_save, text=_("Save"), command=ini_save_wraper, bootstyle="info-outline")
-b_last_read = ttk.Button(frame_save, text=_("Load"), command=ini_read_wraper, bootstyle="info-outline")
+b_last_save = ttk.Button(frame_save, text=_("Save"), bootstyle="info-outline",
+                         command=ini_save_wraper)
+b_last_read = ttk.Button(frame_save, text=_("Load"), bootstyle="info-outline",
+                         command=ini_read_wraper)
 
 b_last_save.pack(padx=5, pady=1, anchor=W, side=LEFT)
 b_last_read.pack(padx=5, pady=1, anchor=W, side=LEFT)
 
 ####################################################################
 # main_tools row
 ####################################################################
@@ -1795,23 +1801,23 @@
 e4_crop_2.grid(row=3, column=5, sticky=W, padx=5, pady=5)
 rb3_crop.grid(row=4, column=1, sticky=W, padx=5, pady=1)
 e1_crop_3.grid(row=4, column=2, sticky=W, padx=10, pady=1)
 e2_crop_3.grid(row=4, column=3, sticky=W, padx=5, pady=1)
 e3_crop_3.grid(row=4, column=4, sticky=W, padx=5, pady=1)
 e4_crop_3.grid(row=4, column=5, sticky=W, padx=5, pady=1)
 frame_crop_gravity.grid(row=2, column=2, rowspan=2, padx=5, columnspan=4, sticky=E)
-rb_crop_NW.grid(row=1, column=1, sticky=W, pady=1)
-rb_crop_N.grid(row=1, column=2, pady=1)
-rb_crop_NE.grid(row=1, column=3, sticky=W, pady=1)
-rb_crop_W.grid(row=2, column=1, sticky=W, pady=1)
-rb_crop_C.grid(row=2, column=2, sticky=W, pady=1)
-rb_crop_E.grid(row=2, column=3, sticky=W, pady=1)
-rb_crop_SW.grid(row=3, column=1, sticky=W, pady=1)
-rb_crop_S.grid(row=3, column=2, pady=1)
-rb_crop_SE.grid(row=3, column=3, sticky=W, pady=1)
+rb_crop_NW.grid(row=1, column=1, sticky=W, padx=3, pady=1)
+rb_crop_N.grid(row=1, column=2, padx=3, pady=1)
+rb_crop_NE.grid(row=1, column=3, sticky=W, padx=3, pady=1)
+rb_crop_W.grid(row=2, column=1, sticky=W, padx=3, pady=1)
+rb_crop_C.grid(row=2, column=2, sticky=W, padx=3, pady=1)
+rb_crop_E.grid(row=2, column=3, sticky=W, padx=3, pady=1)
+rb_crop_SW.grid(row=3, column=1, sticky=W, padx=3, pady=1)
+rb_crop_S.grid(row=3, column=2, padx=3, pady=1)
+rb_crop_SE.grid(row=3, column=3, sticky=W, padx=3, pady=1)
 frame_crop_buttons.grid(row=5, column=1, sticky=(W, E))
 b_crop_read.grid(row=1, column=1, sticky=W, padx=15, pady=5)
 b_crop_show.grid(row=1, column=2, sticky=W, padx=5, pady=5)
 b_crop_run.grid(row=5, column=4, columnspan=2, sticky=W, padx=5, pady=5)
 
 ###########################
 # Tekst
@@ -1871,23 +1877,23 @@
 rb_text_SW = ttk.Radiobutton(frame_text_gravity, text="SW",
                              variable=img_text_gravity, value="SW")
 rb_text_S = ttk.Radiobutton(frame_text_gravity, text="S",
                             variable=img_text_gravity, value="S")
 rb_text_SE = ttk.Radiobutton(frame_text_gravity, text="SE",
                              variable=img_text_gravity, value="SE")
 frame_text_gravity.grid(row=2, column=2, rowspan=3,  padx=25, pady=2, sticky=(W, N))
-rb_text_NW.grid(row=1, column=1, sticky=W, pady=1)
-rb_text_N.grid(row=1, column=2, pady=1)
-rb_text_NE.grid(row=1, column=3, sticky=W, pady=1)
-rb_text_W.grid(row=2, column=1, sticky=W, pady=1)
-rb_text_C.grid(row=2, column=2, pady=1)
-rb_text_E.grid(row=2, column=3, sticky=W, pady=1)
-rb_text_SW.grid(row=3, column=1, sticky=W, pady=1)
-rb_text_S.grid(row=3, column=2, pady=1)
-rb_text_SE.grid(row=3, column=3, sticky=W, pady=1)
+rb_text_NW.grid(row=1, column=1, sticky=W, padx=3, pady=1)
+rb_text_N.grid(row=1, column=2, padx=3, pady=1)
+rb_text_NE.grid(row=1, column=3, sticky=W, padx=3, pady=1)
+rb_text_W.grid(row=2, column=1, sticky=W, padx=3, pady=1)
+rb_text_C.grid(row=2, column=2, padx=3, pady=1)
+rb_text_E.grid(row=2, column=3, sticky=W, padx=3, pady=1)
+rb_text_SW.grid(row=3, column=1, padx=3, sticky=W, pady=1)
+rb_text_S.grid(row=3, column=2, padx=3, pady=1)
+rb_text_SE.grid(row=3, column=3, sticky=W, padx=3, pady=1)
 
 ###
 co_text_font = ttk.Combobox(frame_text, width=30,
                             textvariable=img_text_font)
 co_text_font.configure(state='readonly')
 e_text_size = ttk.Entry(frame_text, width=3,
                         validate="key", validatecommand=(validation, '%S'))
@@ -2455,18 +2461,15 @@
 ToolTip(b_logo_run, text=_("Execute only add logo on current picture"))
 
 ##########################################
 # Run functions
 #
 
 Python_version = "Py " + platform.python_version() + " Tk " + str(TkVersion)
-window_title = ( version.__author__ + " : "
-                + version.__appname__ + " "
-                + version.__version__ + " : "
-                + IMAGEMAGICK_WAND_VERSION + " : " + Python_version + " | " )
+window_title = title_begin + IMAGEMAGICK_WAND_VERSION + " : " + Python_version + " | "
 root.title(window_title)
 if IMAGEMAGICK_WAND is not None:
     img_text_font_dict = fonts()    # Reading available fonts
     ini_read_wraper()  # Loading settings from config file
     tools_set(0)
     text_tool_hide_show()
     progress_files.set(_("Ready"))
```

### Comparing `FotoKilof-4.3.0/fotokilof/common.py` & `FotoKilof-4.3.1/fotokilof/common.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/convert.py` & `FotoKilof-4.3.1/fotokilof/convert.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/convert_wand.py` & `FotoKilof-4.3.1/fotokilof/convert_wand.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/entries.py` & `FotoKilof-4.3.1/fotokilof/entries.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/gui.py` & `FotoKilof-4.3.1/fotokilof/gui.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/ini_read.py` & `FotoKilof-4.3.1/fotokilof/ini_read.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/ini_save.py` & `FotoKilof-4.3.1/fotokilof/ini_save.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.1/fotokilof/locale/bg/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.1/fotokilof/locale/bg/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.1/fotokilof/locale/de/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/de/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.1/fotokilof/locale/de/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.1/fotokilof/locale/en/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/en/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.1/fotokilof/locale/en/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/fotokilof.pot` & `FotoKilof-4.3.1/fotokilof/locale/fotokilof.pot`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.1/fotokilof/locale/id/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/id/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.1/fotokilof/locale/id/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.1/fotokilof/locale/pl/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.1/fotokilof/locale/pl/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo` & `FotoKilof-4.3.1/fotokilof/locale/tr/LC_MESSAGES/fotokilof.mo`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po` & `FotoKilof-4.3.1/fotokilof/locale/tr/LC_MESSAGES/fotokilof.po`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/log.py` & `FotoKilof-4.3.1/fotokilof/log.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/magick.py` & `FotoKilof-4.3.1/fotokilof/magick.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/mswindows.py` & `FotoKilof-4.3.1/fotokilof/mswindows.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/preview.py` & `FotoKilof-4.3.1/fotokilof/preview.py`

 * *Files identical despite different names*

### Comparing `FotoKilof-4.3.0/fotokilof/version.py` & `FotoKilof-4.3.1/fotokilof/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-__version__ = "4.3.0"
+__version__ = "4.3.1"
 __author__ = "Tomasz Łuczak"
 __email__ = "tlu@team-tl.pl"
 __appname__ = "FotoKilof"
 __description__ = "Nice gui for ImageMagick"
 __keywords__ = "GUI ImageMagick FotoKilof"
 __url__ = "https://github.com/TeaM-TL/FotoKilof"
 __copyright__ = "2019-2023"
```

### Comparing `FotoKilof-4.3.0/setup.py` & `FotoKilof-4.3.1/setup.py`

 * *Files identical despite different names*

