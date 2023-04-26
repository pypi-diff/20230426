# Comparing `tmp/isbnlib-3.9.8.tar.gz` & `tmp/isbnlib-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isbnlib-3.9.8.tar", last modified: Mon May  6 14:19:29 2019, max compression
+gzip compressed data, was "dist/isbnlib-3.9.9.tar", last modified: Thu Oct 17 08:59:43 2019, max compression
```

## Comparing `isbnlib-3.9.8.tar` & `isbnlib-3.9.9.tar`

### file list

```diff
@@ -1,76 +1,57 @@
-drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-05-06 14:19:29.000000 isbnlib-3.9.8/
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     7651 2018-01-24 08:40:53.000000 isbnlib-3.9.8/LICENSE
-drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib.egg-info/
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1544 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)        1 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)       47 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    17935 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3081 2019-05-06 14:16:13.000000 isbnlib-3.9.8/CHANGES.txt
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      365 2019-05-06 14:19:29.000000 isbnlib-3.9.8/setup.cfg
--rw-------   0 alexandre  (1000) alexandre  (1000)        0 2019-05-06 10:32:41.000000 isbnlib-3.9.8/requirements.txt
--rw-------   0 alexandre  (1000) alexandre  (1000)       67 2019-05-06 10:32:39.000000 isbnlib-3.9.8/requirements-appveyor.txt
-drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib/
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     7352 2019-02-19 16:47:12.000000 isbnlib-3.9.8/isbnlib/_core.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1790 2019-01-18 08:35:49.000000 isbnlib-3.9.8/isbnlib/_msk.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1538 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/config.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      579 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/_doitotex.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1192 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/_openled.py
-drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib/_data/
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    10749 2019-05-06 11:14:18.000000 isbnlib-3.9.8/isbnlib/_data/data4info.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)    78089 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/_data/data4tex.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)        1 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/_data/__init__.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    48985 2019-05-06 11:14:18.000000 isbnlib-3.9.8/isbnlib/_data/data4mask.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1467 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/_exceptions.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2484 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/_goob.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1071 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/_imcache.py
-drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib/test/
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     1374 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_metadata.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      315 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_goom.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      460 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_unicode_to_utf8tex.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      366 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_webservice.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      950 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_fmt.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1752 2019-05-06 11:14:18.000000 isbnlib-3.9.8/isbnlib/test/test_data.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     6939 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_core.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      417 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_words.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      780 2019-05-06 11:14:18.000000 isbnlib-3.9.8/isbnlib/test/speed.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     2453 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_ext.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     1137 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_info.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      270 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_doi2tex.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2444 2019-05-06 11:14:18.000000 isbnlib-3.9.8/isbnlib/test/test_rename.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)        1 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/__init__.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1567 2019-05-06 11:14:18.000000 isbnlib-3.9.8/isbnlib/test/test_editions.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     2080 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_helpers.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     2218 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_files.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     1690 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/data4tests.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      401 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/test/test_openl.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1141 2019-05-06 14:16:13.000000 isbnlib-3.9.8/isbnlib/_thinged.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1352 2019-02-24 21:28:14.000000 isbnlib-3.9.8/isbnlib/_desc.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     1192 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/_gwords.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2688 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/registry.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2693 2019-02-17 14:13:16.000000 isbnlib-3.9.8/isbnlib/_ext.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1222 2019-05-06 11:14:18.000000 isbnlib-3.9.8/isbnlib/_cover.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2346 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/_goom.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1767 2019-05-06 14:16:13.000000 isbnlib-3.9.8/isbnlib/__init__.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1160 2019-05-06 14:16:13.000000 isbnlib-3.9.8/isbnlib/_metadata.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2101 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/_openl.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2391 2019-05-06 14:16:13.000000 isbnlib-3.9.8/isbnlib/_editions.py
-drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-05-06 14:19:29.000000 isbnlib-3.9.8/isbnlib/dev/
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2235 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/dev/webquery.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      795 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/dev/_bouth23.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3291 2019-03-12 14:40:45.000000 isbnlib-3.9.8/isbnlib/dev/_data.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1818 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/dev/vias.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2410 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/dev/_exceptions.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      638 2019-02-10 12:05:49.000000 isbnlib-3.9.8/isbnlib/dev/helpers.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     3272 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/dev/_files.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)     3064 2018-11-26 12:01:33.000000 isbnlib-3.9.8/isbnlib/dev/webservice.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3971 2019-01-18 08:35:49.000000 isbnlib-3.9.8/isbnlib/dev/_fmt.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1015 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/dev/__init__.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2781 2019-03-08 15:49:51.000000 isbnlib-3.9.8/isbnlib/dev/_helpers.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      972 2019-02-24 21:28:15.000000 isbnlib-3.9.8/isbnlib/_infogroup.py
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    17935 2019-05-06 14:19:29.000000 isbnlib-3.9.8/PKG-INFO
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3346 2019-02-24 21:28:15.000000 isbnlib-3.9.8/setup.py
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)      737 2019-02-10 12:05:49.000000 isbnlib-3.9.8/COPYRIGHT.txt
--rw-r--r--   0 alexandre  (1000) alexandre  (1000)       65 2019-02-23 15:02:20.000000 isbnlib-3.9.8/MANIFEST.in
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      797 2017-12-12 21:33:01.000000 isbnlib-3.9.8/.coveragerc
--rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    13374 2019-05-06 14:16:13.000000 isbnlib-3.9.8/README.rst
--rw-------   0 alexandre  (1000) alexandre  (1000)      209 2019-05-06 10:32:40.000000 isbnlib-3.9.8/requirements-dev.txt
+drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-10-17 08:59:43.000000 isbnlib-3.9.9/
+drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib.egg-info/
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1062 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)        1 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)       34 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    20406 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     7651 2019-10-17 08:48:48.000000 isbnlib-3.9.9/LICENSE-LGPL-3.0-only.txt
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3165 2019-10-17 08:48:48.000000 isbnlib-3.9.9/CHANGES.txt
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      234 2019-10-17 08:59:43.000000 isbnlib-3.9.9/setup.cfg
+-rw-------   0 alexandre  (1000) alexandre  (1000)        0 2019-07-23 12:21:44.000000 isbnlib-3.9.9/requirements.txt
+-rw-------   0 alexandre  (1000) alexandre  (1000)       67 2019-07-23 12:21:36.000000 isbnlib-3.9.9/requirements-appveyor.txt
+drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib/
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     7592 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_core.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1790 2019-01-18 08:35:49.000000 isbnlib-3.9.9/isbnlib/_msk.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1562 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/config.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      642 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_doitotex.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1233 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_openled.py
+drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib/_data/
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     8995 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_data/data4info.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    78089 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_data/data4tex.py
+-rw-r--r--   0 alexandre  (1000) alexandre  (1000)        1 2018-11-26 12:01:33.000000 isbnlib-3.9.9/isbnlib/_data/__init__.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    32160 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_data/data4mask.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1621 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_exceptions.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2484 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_goob.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1182 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_imcache.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1173 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_thinged.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      971 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_desc.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1400 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_gwords.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2912 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/registry.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2693 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_ext.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      703 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_cover.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2370 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_goom.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1767 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/__init__.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1146 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_metadata.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2101 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_openl.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2211 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/_editions.py
+drwxrwxr-x   0 alexandre  (1000) alexandre  (1000)        0 2019-10-17 08:59:43.000000 isbnlib-3.9.9/isbnlib/dev/
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2304 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/webquery.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      795 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/_bouth23.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3356 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/_data.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1911 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/vias.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2541 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/_exceptions.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      638 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/helpers.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3353 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/_files.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      628 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/_decorators.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3211 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/webservice.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3986 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/_fmt.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     1146 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/__init__.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     2770 2019-10-17 08:48:48.000000 isbnlib-3.9.9/isbnlib/dev/_helpers.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      972 2019-02-24 21:28:15.000000 isbnlib-3.9.9/isbnlib/_infogroup.py
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    20406 2019-10-17 08:59:43.000000 isbnlib-3.9.9/PKG-INFO
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)     3270 2019-10-17 08:48:48.000000 isbnlib-3.9.9/setup.py
+-rw-r--r--   0 alexandre  (1000) alexandre  (1000)      737 2019-02-10 12:05:49.000000 isbnlib-3.9.9/COPYRIGHT.txt
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)       83 2019-10-17 08:48:48.000000 isbnlib-3.9.9/MANIFEST.in
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      795 2019-10-17 08:48:48.000000 isbnlib-3.9.9/.coveragerc
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)    15211 2019-10-17 08:48:48.000000 isbnlib-3.9.9/README.rst
+-rw-rw-r--   0 alexandre  (1000) alexandre  (1000)      414 2019-10-17 08:48:48.000000 isbnlib-3.9.9/requirements-dev.txt
```

### Comparing `isbnlib-3.9.8/LICENSE` & `isbnlib-3.9.9/LICENSE-LGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `isbnlib-3.9.8/isbnlib.egg-info/PKG-INFO` & `isbnlib-3.9.9/isbnlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 1.1
 Name: isbnlib
-Version: 3.9.8
+Version: 3.9.9
 Summary: Extract, clean, transform, hyphenate and metadata for ISBNs (International Standard Book Number).
 Home-page: https://github.com/xlcnd/isbnlib
 Author: Alexandre Lima Conde
 Author-email: xlcnd@outlook.com
 License: LGPL v3
-Download-URL: https://github.com/xlcnd/isbnlib/archive/v3.9.8.zip
+Download-URL: https://github.com/xlcnd/isbnlib/archive/v3.9.9.zip
 Project-URL: Bug Reports, https://github.com/xlcnd/isbnlib/issues
 Project-URL: Dev Docs, https://isbnlib.readthedocs.io/en/latest/devs.html
 Project-URL: Forum, https://stackoverflow.com/search?tab=newest&q=isbnlib
-Project-URL: License, https://github.com/xlcnd/isbnlib/blob/dev/LICENSE
+Project-URL: License, https://github.com/xlcnd/isbnlib/blob/dev/LICENSE-LGPL-3.0-only.txt
 Description: 
         .. image:: https://img.shields.io/badge/Sourcegraph-Status-blue.svg
             :target: https://sourcegraph.com/github.com/xlcnd/isbnlib
             :alt: Graph
         
         .. image:: https://readthedocs.org/projects/isbnlib/badge/?version=latest
             :target: https://isbnlib.readthedocs.org/en/latest/
             :alt: Documentation Status
         
-        .. image:: https://coveralls.io/repos/github/xlcnd/isbnlib/badge.svg?branch=v3.9.8
-            :target: https://coveralls.io/github/xlcnd/isbnlib?branch=v3.9.8
+        .. image:: https://coveralls.io/repos/github/xlcnd/isbnlib/badge.svg?branch=v3.9.9
+            :target: https://coveralls.io/github/xlcnd/isbnlib?branch=v3.9.9
             :alt: Coverage Status
         
-        .. image:: https://travis-ci.org/xlcnd/isbnlib.svg?branch=v3.9.8
+        .. image:: https://travis-ci.org/xlcnd/isbnlib.svg?branch=v3.9.9
             :target: https://travis-ci.org/xlcnd/isbnlib
             :alt: Built Status
         
-        .. image:: https://ci.appveyor.com/api/projects/status/github/xlcnd/isbnlib?branch=v3.9.8&svg=true
+        .. image:: https://ci.appveyor.com/api/projects/status/github/xlcnd/isbnlib?branch=v3.9.9&svg=true
             :target: https://ci.appveyor.com/project/xlcnd/isbnlib
             :alt: Windows Built Status
         
         .. image:: https://img.shields.io/github/issues/xlcnd/isbnlib/bug.svg?label=bugs&style=flat
             :target: https://github.com/xlcnd/isbnlib/labels/bug
             :alt: Bugs
         
@@ -41,14 +41,15 @@
             :alt: PYPI Downloads
         
         
         
         Warning
         =======
         
+        
             **Breaking Change** The service xISBN was decommissioned (see issue 51_)!
         
         
         
         Info
         ====
         
@@ -181,14 +182,15 @@
         
         See files test_core_ and test_ext_ for **a lot of examples**.
         
         
         Install
         =======
         
+        
         From the command line, enter (in some cases you have to preced the
         command with ``sudo``):
         
         
         .. code-block:: bash
         
             $ pip install isbnlib
@@ -203,19 +205,22 @@
         For Devs
         ========
         
         
         API's Main Namespaces
         ---------------------
         
-        In the namespace ``isbnlib`` you have access to the core methods:
+        In the namespace ``isbnlib`` you have access to the **core functions**:
         ``is_isbn10``, ``is_isbn13``, ``to_isbn10``, ``to_isbn13``, ``canonical``,
         ``clean``, ``notisbn``, ``get_isbnlike``, ``get_canonical_isbn``, ``mask``,
-        ``meta``, ``info``, ``editions``, ``goom``, ``ren``, ``doi``, ``EAN13``,
-        ``isbn_from_words``, ``desc`` and ``cover``.
+        ``info``, ``check_digit10``, ``check_digit13``, ``doi`` and ``EAN13``.
+        
+        In addition, you have access to **metadata functions**, namely:
+        ``meta``, ``editions``, ``ren``, ``desc``, ``cover``,
+        ``goom``, ``doi2tex`` and ``isbn_from_words``.
         
         The exceptions raised by these methods can all be catched using ``ISBNLibException``.
         
         
         You can extend the lib by using the classes and functions exposed in
         namespace ``isbnlib.dev``, namely:
         
@@ -302,14 +307,78 @@
         at goob_.
         
         
         Remember that plugins **must** support python 2.7 and python 3.5+ (see python-future.org_).
         
         
         
+        Patterns of Usage
+        -----------------
+        
+        The library implements a very simple API with sensible defaults, but there are cases
+        that need your attention (see case 3 below).
+        
+        
+        
+        A. You only need **core functions**:
+        
+        
+        .. code-block:: python
+        
+            # import the core functions you need
+            from isbnlib import canonical, is_isbn10, is_isbn13
+        
+            isbn = canonical("978-0446310789")
+            if is_isbn13(isbn):
+                ...
+            ...
+        
+        
+        B. You need also **metadata functions**, with **default config**:
+        
+        
+        .. code-block:: python
+        
+            from isbnlib import canonical, meta, description
+        
+            isbn = canonical("978-0446310789")
+            data = meta(isbn)
+            ...
+        
+        C. You need also **metadata functions**, with **special config**:
+        
+           *Lets suppose you need to add an api key for a metadata plugin
+           and change the cache too*.
+        
+        
+        .. code-block:: python
+        
+            from myapp.utils import MyCache
+        
+            # import the functions you need, plus 'config' and 'registry'
+            from isbnlib import canonical, config, meta, registry
+        
+            # you should use 'config' first
+            config.add_apikey('isbndb', 'kjshdfkjahsdflkjh')
+        
+            # then 'registry'
+            registry.set_cache(MyCache())
+        
+            # Only now you should use metadata functions
+            # (there are no adaptions for core functions,
+            #  so they can be used at any moment)
+            isbn = canonical("978-0446310789")
+            data = meta(isbn, service="isbndb")
+            ...
+        
+        
+        D. You want to build a **plugin** or use **isbnlib.dev** in your code:
+        
+           You should study very carefully the **public** methods in ``dir(isbnlib.dev)``.
+        
         
         
         Caveats
         -------
         
         
         1. These classes are optimized for one-call to services and not for batch calls.
@@ -321,38 +390,46 @@
         
         
         Projects using *isbnlib*
         ------------------------
         
         **isbntools**      https://github.com/xlcnd/isbntools
         
+        **isbnsrv**        https://github.com/xlcnd/isbnsrv
+        
         **Open Library**   https://github.com/internetarchive/openlibrary
         
-        **Spreads**        https://github.com/DIYBookScanner/spreads
+        **NYPL Library Simplified**  https://github.com/NYPL-Simplified
+        
+        **Manubot**   https://github.com/manubot
+        
+        **Spreads**  https://github.com/DIYBookScanner/spreads
         
         **Papis**    https://github.com/papis/papis
         
         **libBMC**    https://github.com/Phyks/libbmc/
         
-        **Alessandria**     https://gitlab.com/openlabmatera/alessandria
+        **Alessandria**      https://gitlab.com/openlabmatera/alessandria
         
         **Comic Collector**  https://github.com/wengole/comiccollector
         
-        **Abelujo**    http://www.abelujo.cc/
+        **Abelujo**   https://github.com/vindarel/abelujo
+        
+        **BibLib**    https://pypi.org/project/biblib/
         
-        **BibLib**    https://pypi.python.org/pypi/biblib
+        **L-Space**   https://pypi.org/project/lspace/
         
         
         
         Help
         ----
         
         
         If you need help, please take a look at github_ or post a question on
-        stackoverflow_ (with tag **isbnlib**)
+        stackoverflow_ .
         
         
         
         ----------------------------------------------------------------------------------------------
         
         .. class:: center
         
@@ -367,15 +444,15 @@
         
         .. _isbntools: https://pypi.python.org/pypi/isbntools
         
         .. _sourcegraph: http://bit.ly/ISBNLib_srcgraph
         
         .. _readthedocs: http://bit.ly/ISBNLib_rtd
         
-        .. _stackoverflow: http://stackoverflow.com/questions/tagged/isbnlib
+        .. _stackoverflow: http://stackoverflow.com/search?tab=newest&q=isbnlib
         
         .. _test_core: https://github.com/xlcnd/isbnlib/blob/master/isbnlib/test/test_core.py
         
         .. _test_ext: https://github.com/xlcnd/isbnlib/blob/master/isbnlib/test/test_ext.py
         
         .. _isbn-international.org: https://www.isbn-international.org/content/what-isbn
```

### Comparing `isbnlib-3.9.8/CHANGES.txt` & `isbnlib-3.9.9/CHANGES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -44,7 +44,8 @@
 v3.9.2, 2018-09-28 -- Updated data.
 v3.9.3, 2018-10-05 -- Make it easier to override 'WEBService.data'.
 v3.9.4, 2019-01-18 -- Fix bibjson and updated data.
 v3.9.5, 2019-02-10 -- PR #53 and updated data.
 v3.9.6, 2019-02-24 -- Performance improvements (close #55).
 v3.9.7, 2019-05-06 -- Editions is now cached and consistent return types.
 v3.9.8, 2019-05-06 -- Fix bug #58 on 'editions'.
+v3.9.9, 2019-10-17 -- Better caching, improved security, fix 'catch all exception'.
```

### Comparing `isbnlib-3.9.8/isbnlib/_core.py` & `isbnlib-3.9.9/isbnlib/_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     r'97[89]{1}(?:-?\d){10}|\d{9}[0-9X]{1}|'
     r'[-0-9X]{10,16}', re.I | re.M | re.S)
 RE_LOOSE = re.compile(r'[- 0-9X]{10,19}', re.I | re.M | re.S)
 ISBN13_PREFIX = '978'
 LEGAL = '0123456789xXisbnISBN- '
 
 
+# pylint: disable=broad-except
 def check_digit10(firstninedigits):
     """Check sum ISBN-10."""
     # minimum checks
     if len(firstninedigits) != 9:
         return None
     try:
         int(firstninedigits)
@@ -61,14 +62,15 @@
     else:
         tenthdigit = 11 - remainder
     if tenthdigit == 10:
         tenthdigit = 'X'
     return str(tenthdigit)
 
 
+# pylint: disable=broad-except
 def check_digit13(firsttwelvedigits):
     """Check sum ISBN-13."""
     # minimum checks
     if len(firsttwelvedigits) != 12:
         return None
     try:
         int(firsttwelvedigits)
@@ -79,24 +81,27 @@
         (i % 2 * 2 + 1) * int(x) for i, x in enumerate(firsttwelvedigits))
     thirteenthdigit = 10 - int(val % 10)
     if thirteenthdigit == 10:
         thirteenthdigit = '0'
     return str(thirteenthdigit)
 
 
+# pylint: disable=simplifiable-if-expression
 def _check_structure10(isbn10like):
     """Check structure of an ISBN-10."""
     return True if re.match(RE_ISBN10, isbn10like) else False
 
 
+# pylint: disable=simplifiable-if-expression
 def _check_structure13(isbn13like):
     """Check structure of an ISBN-13."""
     return True if re.match(RE_ISBN13, isbn13like) else False
 
 
+# pylint: disable=simplifiable-if-expression
 def is_isbn10(isbn10):
     """Validate as ISBN-10."""
     isbn10 = canonical(isbn10)
     if len(isbn10) != 10:
         return False  # pragma: no cover
     else:
         return False if check_digit10(isbn10[:-1]) != isbn10[-1] else True
@@ -182,14 +187,15 @@
     level:
     strict almost as certain they are ISBNs
     normal (default)
     loose  catch many as possible
 
     """
     if level == 'normal':  # pragma: no cover
+        text = text.replace('-97', '- 97')
         isbnlike = RE_NORMAL
     elif level == 'strict':
         isbnlike = RE_STRICT
     elif level == 'loose':
         isbnlike = RE_LOOSE
     else:
         LOGGER.error('level as no option %s', level)
```

### Comparing `isbnlib-3.9.8/isbnlib/_msk.py` & `isbnlib-3.9.9/isbnlib/_msk.py`

 * *Files identical despite different names*

### Comparing `isbnlib-3.9.8/isbnlib/config.py` & `isbnlib-3.9.9/isbnlib/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 def set_option(option, value):  # pragma: no cover
     """Set the value for option."""
     global options
     options[option.upper()] = value
 
 
-# TODO don't expose this directly! BREAKING CHANGE!
+# TODO(NV) don't expose this directly! BREAKING CHANGE!
 # Timeouts
 URLOPEN_TIMEOUT = options.get('URLOPEN_TIMEOUT', 10)
 THREADS_TIMEOUT = options.get('THREADS_TIMEOUT', 12)
 
 
 # URLOPEN_TIMEOUT is used by webservice
 def seturlopentimeout(seconds):  # pragma: no cover
@@ -47,12 +47,12 @@
 def setthreadstimeout(seconds):  # pragma: no cover
     """Set the value of THREADS_TIMEOUT (in seconds)."""
     global options, THREADS_TIMEOUT
     set_option('THREADS_TIMEOUT', seconds)
     THREADS_TIMEOUT = seconds
 
 
-def setloadplugins(boolean=True):
+def setloadplugins(boolean=True):  # pragma: no cover
     """Set the value for all LOAD_XXX_PLUGINS."""
     global options
     set_option('LOAD_METADATA_PLUGINS', boolean)
     set_option('LOAD_FORMATTER_PLUGINS', boolean)
```

### Comparing `isbnlib-3.9.8/isbnlib/_doitotex.py` & `isbnlib-3.9.9/isbnlib/_doitotex.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 """Return metadata, of a given DOI, formated as BibTeX."""
 
 import logging
 
+from .dev import cache
 from .dev.webservice import query
 
 LOGGER = logging.getLogger(__name__)
 
 URL = 'http://dx.doi.org/{DOI}'
 UA = 'isbnlib (gzip)'
 
 
+@cache
 def doi2tex(doi):
     """Get the bibtex ref for doi."""
-    data = query(
-        URL.format(DOI=doi),
-        user_agent=UA,
-        appheaders={
-            'Accept': 'application/x-bibtex; charset=utf-8',
-        })
+    data = query(URL.format(DOI=doi),
+                 user_agent=UA,
+                 appheaders={
+                     'Accept': 'application/x-bibtex; charset=utf-8',
+                 })  # noqa
     if not data:  # pragma: no cover
         LOGGER.warning('no data return for doi: %s', doi)
-        return None
-    return data
+    return data if data else None
```

### Comparing `isbnlib-3.9.8/isbnlib/_openled.py` & `isbnlib-3.9.9/isbnlib/_openled.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from .dev._bouth23 import u
 from .dev.webquery import query as wquery
 
 LOGGER = logging.getLogger(__name__)
 UA = 'isbnlib (gzip)'
 SERVICE_URL = 'http://openlibrary.org/query.json?type=/type/edition&'\
               '{selectors}'
-CODES = 'isbn_13={isbn}&books='
+CODES = 'isbn_13={isbn}'
 ISBNS = '{code}&isbn_13='
 
 
+# pylint: disable=broad-except
 def query(isbn):
     """Query the Open Library for related ISBNs."""
     try:
-        data = wquery(
-            SERVICE_URL.format(selectors=CODES.format(isbn=isbn)),
-            user_agent=UA)
-        codes = [rec['key'] for rec in data]
+        data = wquery(SERVICE_URL.format(selectors=CODES.format(isbn=isbn)),
+                      user_agent=UA)
+        codes = {rec['key'] for rec in data}
         isbnlikes = [isbn]
         for code in codes:
-            txt = wquery(
-                SERVICE_URL.format(selectors=ISBNS.format(code=code)),
-                user_agent=UA,
-                parser=None)
+            txt = wquery(SERVICE_URL.format(selectors=ISBNS.format(code=code)),
+                         user_agent=UA,
+                         parser=None)
             isbnlikes.extend(get_isbnlike(txt))
-        isbns = [get_canonical_isbn(isbnlike) for isbnlike in isbnlikes]
-        isbns = sorted(list((u(n) for n in isbns if n)))
-    except Exception:  # pragma: no cover, qa: FIXME
-        LOGGER.debug('No data from Open Library for isbn %s', isbn)
+        isbns = {u(get_canonical_isbn(isbnlike)) for isbnlike in isbnlikes}
+    except Exception as ex:  # pragma: no cover
+        LOGGER.debug('No data from Open Library for isbn %s -- %s', isbn,
+                     str(ex))
+        return {get_canonical_isbn(isbn)}
     return isbns
```

### Comparing `isbnlib-3.9.8/isbnlib/_exceptions.py` & `isbnlib-3.9.9/isbnlib/_exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """Exceptions for isbnlib."""
 
 import sys
 
 
+# pylint: disable=unused-argument
 def quiet_errors(exc_type, exc_value, traceback):
     """Define error format suitable for end user scripts.
 
     Usage: enter the following lines in your script
     from isbnlib import quiet_errors
     sys.excepthook = quiet_errors
     """
@@ -22,30 +23,33 @@
     """
 
     def __str__(self):
         """Print message."""
         return getattr(self, 'message', '')  # pragma: no cover
 
 
+# pylint: disable=super-init-not-called
 class NotRecognizedServiceError(ISBNLibException):
     """Exception raised when the service is not in config.py."""
 
     def __init__(self, service):
         """Define message."""
-        self.message = "(%s) is not a recognized service" % service
+        self.message = '(%s) is not a recognized service' % service
 
 
+# pylint: disable=super-init-not-called
 class NotValidISBNError(ISBNLibException):
     """Exception raised when the ISBN is not valid."""
 
     def __init__(self, isbnlike):
         """Define message."""
-        self.message = "(%s) is not a valid ISBN" % isbnlike
+        self.message = '(%s) is not a valid ISBN' % isbnlike
 
 
+# pylint: disable=super-init-not-called
 class PluginNotLoadedError(ISBNLibException):  # pragma: no cover
     """Exception raised when the plugin's loader doesn't load the plugin.
 
     TODO: Delete this in version 4?
     """
 
     def __init__(self, path):
```

### Comparing `isbnlib-3.9.8/isbnlib/_goob.py` & `isbnlib-3.9.9/isbnlib/_goob.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         if 'publishedDate' in records \
            and len(records['publishedDate']) >= 4:
             canonical['Year'] = records['publishedDate'][0:4]
         else:  # pragma: no cover
             canonical['Year'] = u('')
         canonical['Language'] = records.get('language', u(''))
     except Exception:  # pragma: no cover
-        LOGGER.debug("RecordMappingError for %s with data %s", isbn, records)
+        LOGGER.debug('RecordMappingError for %s with data %s', isbn, records)
         raise RecordMappingError(isbn)
     # call stdmeta for extra cleanning and validation
     return stdmeta(canonical)
 
 
 def _records(isbn, data):
     """Classify (canonically) the parsed data."""
@@ -48,15 +48,15 @@
         raise NoDataForSelectorError(isbn)
     # consistency check (isbn request = isbn response)
     if recs:
         ids = recs.get('industryIdentifiers', '')
         if u('ISBN_13') in repr(ids) and \
            isbn not in repr(ids):  # pragma: no cover
             LOGGER.debug('ISBNNotConsistentError for %s (%s)', isbn, repr(ids))
-            raise ISBNNotConsistentError("{0} not in {1}".format(
+            raise ISBNNotConsistentError('{0} not in {1}'.format(
                 isbn, repr(ids)))
     # map canonical <- records
     return _mapper(isbn, recs)
 
 
 def query(isbn):
     """Query the Google Books (JSON API v1) service for metadata."""
```

### Comparing `isbnlib-3.9.8/isbnlib/_imcache.py` & `isbnlib-3.9.9/isbnlib/_imcache.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 class IMCache(MutableMapping):
     """Read and write to a dict-like cache."""
 
     MAXLEN = 1000
 
+    # pylint: disable=keyword-arg-before-vararg
     def __init__(self, maxlen=MAXLEN, *a, **k):
         self.filepath = 'IN MEMORY'
         self.maxlen = maxlen
         self.d = dict(*a, **k)
         while len(self) > maxlen:  # pragma: no cache
             self.popitem()
 
@@ -26,14 +27,17 @@
         return self.d[k]
 
     def __setitem__(self, k, v):
         if k not in self and len(self) == self.maxlen:
             self.popitem()
         self.d[k] = v
 
+    def __contains__(self, key):
+        return key in self.d
+
     def __delitem__(self, k):
         del self.d[k]
 
     def __bool__(self):
         return len(self) != 0
 
     # For PY2 compatibility
```

### Comparing `isbnlib-3.9.8/isbnlib/_thinged.py` & `isbnlib-3.9.9/isbnlib/_thinged.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 LOGGER = logging.getLogger(__name__)
 UA = 'isbnlib (gzip)'
 SERVICE_URL = 'http://www.librarything.com/api/thingISBN/{isbn}'
 
 
 def _get_text(topnode):
     """Get the text values in the child nodes."""
-    text = ""
+    text = ''
     for node in topnode.childNodes:
         if node.nodeType == node.TEXT_NODE:
             text = text + node.data
     return text
 
 
 def parser_thinged(xml):
     """Parse the response from the ThingISBN service."""
     dom = parseString(xml)
-    nodes = dom.getElementsByTagName("idlist")[0].getElementsByTagName("isbn")
+    nodes = dom.getElementsByTagName('idlist')[0].getElementsByTagName('isbn')
     return [EAN13(_get_text(isbn)) for isbn in nodes]
 
 
 def query(isbn):
     """Query the ThingISBN service for related ISBNs."""
-    data = wquery(
-        SERVICE_URL.format(isbn=isbn), user_agent=UA, parser=parser_thinged)
+    data = wquery(SERVICE_URL.format(isbn=isbn),
+                  user_agent=UA,
+                  parser=parser_thinged)
     if not data:  # pragma: no cover
         LOGGER.debug('No data from ThingISBN for isbn %s', isbn)
         data = []
     data.append(EAN13(isbn))
-    return data
+    return set(data)
```

### Comparing `isbnlib-3.9.8/isbnlib/_gwords.py` & `isbnlib-3.9.9/isbnlib/_gwords.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 # -*- coding: utf-8 -*-
 """Use Google to get an ISBN from words from title and author's name."""
 
 import logging
 
 from ._core import get_canonical_isbn, get_isbnlike
-from .dev import webservice
+from .dev import cache, webservice
 
 try:  # pragma: no cover
     from urllib.parse import quote
 except ImportError:  # pragma: no cover
 
     def quote(x):  # pragma: no cover
         """Do nothing if PY2."""
         return x
 
 
 LOGGER = logging.getLogger(__name__)
 
 
+@cache
 def goos(words):
     """Use Google to get an ISBN from words from title and author's name."""
-    service_url = "http://www.google.com/search?q=ISBN+"
+    service_url = 'http://www.google.com/search?q=ISBN+'
     search_url = service_url + quote(words.replace(' ', '+'))
 
     user_agent = 'w3m/0.5.3'
 
-    content = webservice.query(
-        search_url,
-        user_agent=user_agent,
-        appheaders={
-            'Content-Type': 'text/plain; charset="UTF-8"',
-            'Content-Transfer-Encoding': 'Quoted-Printable',
-        })
+    content = webservice.query(search_url,
+                               user_agent=user_agent,
+                               appheaders={
+                                   'Content-Type':
+                                   'text/plain; charset="UTF-8"',
+                                   'Content-Transfer-Encoding':
+                                   'Quoted-Printable',
+                               })
     isbns = get_isbnlike(content)
 
     for item in isbns:
         isbn = get_canonical_isbn(item, output='isbn13')
-        if isbn:
+        if isbn:  # pragma: no cover
             break
     if not isbns or not isbn:  # pragma: no cover
         LOGGER.debug('No ISBN found for %s', words)
-        return None
-    return isbn
+    return isbn if isbn else None
```

### Comparing `isbnlib-3.9.8/isbnlib/registry.py` & `isbnlib-3.9.9/isbnlib/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 """Registry for metadata services, formatters and cache."""
 
+import logging
+
 from pkg_resources import iter_entry_points
 
 from . import _goob as goob
 from . import _openl as openl
 from ._imcache import IMCache
 from .config import options
 from .dev._fmt import _fmtbib
 
+LOGGER = logging.getLogger(__name__)
+
 # SERVICES
 
 services = {
     'default': goob.query,
     'goob': goob.query,
     'openl': openl.query,
 }
 
-PROVIDERS = []
+PROVIDERS = ()
 
 
 def setdefaultservice(name):  # pragma: no cover
     """Set the default service."""
     global services
     services['default'] = services[name.lower()]
 
@@ -42,58 +46,60 @@
     'json': lambda x: _fmtbib('json', x),
     'opf': lambda x: _fmtbib('opf', x),
     'endnote': lambda x: _fmtbib('endnote', x),
     'refworks': lambda x: _fmtbib('refworks', x),
     'msword': lambda x: _fmtbib('msword', x),
 }  # pragma: no cover
 
-BIBFORMATS = []
+BIBFORMATS = ()
 
 
 def setdefaultbibformatter(name):  # pragma: no cover
     """Set the default formatter."""
     global bibformatters
     bibformatters['default'] = bibformatters[name.lower()]
 
 
 def add_bibformatter(name, formatter):  # pragma: no cover
     """Add a new formatter to formatters."""
     global bibformatters
     bibformatters[name] = formatter.lower()
 
 
+# pylint: disable=broad-except
 def load_plugins():  # pragma: no cover
     """Load plugins with groups: isbnlib.metadata & isbnlib.formatters."""
     # get metadata plugins from entry_points
     if options.get('LOAD_METADATA_PLUGINS', True):
         try:
             for entry in iter_entry_points(group='isbnlib.metadata'):
                 add_service(entry.name, entry.load())
         except Exception:
-            pass
+            LOGGER.critical('Some metadata plugins were not loaded!')
     global PROVIDERS
     _buf = list(services.keys())
     _buf.remove('default')
-    PROVIDERS = sorted(_buf)
+    PROVIDERS = tuple(sorted(_buf))
     # get formatters from entry_points
     if options.get('LOAD_FORMATTER_PLUGINS', True):
         try:
             for entry in iter_entry_points(group='isbnlib.formatters'):
                 add_bibformatter(entry.name, entry.load())
         except Exception:
-            pass
+            LOGGER.critical('Some formatters plugins were not loaded!')
     global BIBFORMATS
     _buf = list(bibformatters.keys())
     _buf.remove('labels')
     _buf.remove('default')
-    BIBFORMATS = sorted(_buf)
+    BIBFORMATS = tuple(sorted(_buf))
 
 
 # load plugins on import
 load_plugins()
+del load_plugins
 
 # CACHE
 metadata_cache = IMCache()  # should be an instance
 
 
 def set_cache(cache):  # pragma: no cover
     """Set cache for metadata."""
```

### Comparing `isbnlib-3.9.8/isbnlib/_ext.py` & `isbnlib-3.9.9/isbnlib/_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def isbn_from_words(words):
     """Return the most probable ISBN from a list of words."""
     return goos(words)
 
 
 def doi(isbn):
     """Return a DOI's ISBN-A from a ISBN-13."""
-    return "10.%s.%s%s/%s%s" % \
+    return '10.%s.%s%s/%s%s' % \
            tuple(msk(EAN13(isbn), '-').split('-'))
 
 
 def ren(fp):
     """Rename a file using metadata from an ISBN in his filename."""
     cfp = File(fp)
     isbn = EAN13(cfp.name)
@@ -73,15 +73,15 @@
     if title == u('UNKNOWN') or not title:  # pragma: no cover
         return None
     if ' ' in title:  # pragma: no cover
         tokens = title.split(' ')
         stitle = cutoff_tokens(tokens, maxlen)
         title = ' '.join(stitle)
     isbn13 = data.get('ISBN-13', u('UNKNOWN'))
-    new_name = "%s%s_%s_%s" % (author, year, title, isbn13)
+    new_name = '%s%s_%s_%s' % (author, year, title, isbn13)
     return cfp.baserename(b2u3(new_name + cfp.ext))
 
 
 def cover(isbn):
     """Get the img urls of the cover of the ISBN."""
     isbn = EAN13(isbn)
     return gcover(isbn) if isbn else None
```

### Comparing `isbnlib-3.9.8/isbnlib/_goom.py` & `isbnlib-3.9.9/isbnlib/_goom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """Query the Google Books (JSON API v1) for metadata."""
 
 import logging
 
-from .dev import stdmeta
+from .dev import cache, stdmeta
 from .dev._bouth23 import u
-from .dev._exceptions import (NoDataForSelectorError, RecordMappingError)
+from .dev._exceptions import NoDataForSelectorError, RecordMappingError
 from .dev.webquery import query as wquery
 
 UA = 'isbnlib (gzip)'
 SERVICE_URL = 'https://www.googleapis.com/books/v1/volumes?q={words}'\
     '&fields=items/volumeInfo(title,authors,publisher,publishedDate,'\
     'language,industryIdentifiers)&maxResults=10'
 LOGGER = logging.getLogger(__name__)
@@ -18,23 +18,23 @@
 def _mapper(record):
     """Map canonical <- record."""
     # canonical:
     # -> ISBN-13, Title, Authors, Publisher, Year, Language
     try:
         # mapping: canonical <- records
         if 'industryIdentifiers' not in record:  # pragma: no cover
-            return None
+            return {}
         canonical = {}
         isbn = None
         for ident in record['industryIdentifiers']:
             if ident['type'] == 'ISBN_13':
                 isbn = ident['identifier']
                 break
         if not isbn:  # pragma: no cover
-            return None
+            return {}
         canonical['ISBN-13'] = isbn
         canonical['Title'] = record.get('title', u('')).replace(' :', ':')
         canonical['Authors'] = record.get('authors', [])
         canonical['Publisher'] = record.get('publisher', u(''))
         if 'publishedDate' in record \
            and len(record['publishedDate']) >= 4:
             canonical['Year'] = record['publishedDate'][0:4]
@@ -55,11 +55,12 @@
     except Exception:  # pragma: no cover
         LOGGER.debug('NoDataForSelectorError for (%s)', words)
         raise NoDataForSelectorError(words)
     # map canonical <- records
     return [_mapper(r) for r in recs if _mapper(r)]
 
 
+@cache
 def query(words):
     """Query the Google Books (JSON API v1) for metadata."""
     data = wquery(SERVICE_URL.format(words=words.replace(' ', '+')), UA)
-    return _records(words, data)
+    return _records(words, data) if data else {}
```

### Comparing `isbnlib-3.9.8/isbnlib/__init__.py` & `isbnlib-3.9.9/isbnlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,9 +41,9 @@
            'notisbn', 'ean13', 'EAN13', 'cover', 'desc', 'canonical',
            'get_canonical_isbn', 'editions', 'isbn_from_words', 'quiet_errors',
            'config', '__version__', '__support__', 'doi', 'ren', 'ISBN13',
            'GTIN13', 'ISBNLibException', 'NotRecognizedServiceError',
            'NotValidISBNError', 'PluginNotLoadedError', 'goom', 'doi2tex',
            'RDDATE')
 
-__version__ = '3.9.8'
+__version__ = '3.9.9'
 __support__ = 'py27, py34, py35, py36, py37, pypy, pypy3'
```

### Comparing `isbnlib-3.9.8/isbnlib/_metadata.py` & `isbnlib-3.9.9/isbnlib/_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # -*- coding: utf-8 -*-
 """Query providers for metadata."""
 
 from ._core import EAN13
 from ._exceptions import NotRecognizedServiceError, NotValidISBNError
 
+# TODO(v3.10) use @cache and delete parameter cache= on query
+
 
 def query(isbn, service='default', cache='default'):
     """Query services like Google Books (JSON API), ... for metadata."""
     # validate inputs
     ean = EAN13(isbn)
     if not ean:
         raise NotValidISBNError(isbn)
     isbn = ean
-    # only import when needed (code splitting)
+    # only import when needed
     from .registry import services
     if service != 'default' and service not in services:  # pragma: no cover
         raise NotRecognizedServiceError(service)
     # set cache and get metadata
     if cache is None:  # pragma: no cover
         return services[service](isbn)
-    if cache == 'default':
+    if cache == 'default':  # pragma: no cover
         from .registry import metadata_cache
         cache = metadata_cache
-    key = isbn + service
-    try:
-        if cache[key]:
+    if cache is not None:
+        key = isbn + service
+        if key in cache:
             return cache[key]
-        else:  # pragma: no cover
-            raise KeyError  # <-- IMPORTANT: "caches don't return error"!
-    except KeyError:
-        meta = services[service](isbn)
-        if meta:
-            cache[key] = meta
-        return meta if meta else {}
+    meta = services[service](isbn)
+    if meta and cache is not None:  # pragma: no cover
+        cache[key] = meta
+    return meta if meta else {}
```

### Comparing `isbnlib-3.9.8/isbnlib/_openl.py` & `isbnlib-3.9.9/isbnlib/_openl.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         canonical['Year'] = u('')
         strdate = records.get('publish_date', u(''))
         if strdate:  # pragma: no cover
             match = re.search(r'\d{4}', strdate)
             if match:
                 canonical['Year'] = match.group(0)
     except Exception:  # pragma: no cover
-        LOGGER.debug("RecordMappingError for %s with data %s", isbn, records)
+        LOGGER.debug('RecordMappingError for %s with data %s', isbn, records)
         raise RecordMappingError(isbn)
     # call stdmeta for extra cleanning and validation
     return stdmeta(canonical)
 
 
 def _records(isbn, data):
     """Classify (canonically) the parsed data."""
```

### Comparing `isbnlib-3.9.8/isbnlib/_editions.py` & `isbnlib-3.9.9/isbnlib/_editions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,71 @@
 # -*- coding: utf-8 -*-
 """Return editions for a given ISBN."""
 
 import logging
 
 from ._core import EAN13
-from .dev import vias
 from ._exceptions import NotRecognizedServiceError, NotValidISBNError
-from ._openled import query as oed
-from ._thinged import query as ted
+from ._openled import query as _oed
+from ._thinged import query as _ted
+from .dev import cache, vias
 
 PROVIDERS = ('any', 'merge', 'openl', 'thingl')
-TRUEPROVIDERS = ('openl', 'thingl')  # <-- by priority
 LOGGER = logging.getLogger(__name__)
 
 
-def fake_provider_any(isbn):
+# pylint: disable=broad-except
+def _fake_provider_any(isbn):
     """Fake provider 'any' service."""
-    providers = {'openl': oed, 'thingl': ted}
-    for provider in TRUEPROVIDERS:
-        data = []
+    providers = {'openl': _oed, 'thingl': _ted}
+    for provider in providers:
         try:
             data = providers[provider](isbn)
             if len(data) > 1:
-                return data
-            continue  # pragma: no cover
+                return list(data)
         except Exception:  # pragma: no cover
-            continue
-    return data  # pragma: no cover
+            LOGGER.error("Some error on editions 'any' service for %s (%s)!",
+                         isbn, provider)
+        continue  # pragma: no cover
+    return [isbn]  # pragma: no cover
 
 
-def fake_provider_merge(isbn):
+# pylint: disable=broad-except
+def _fake_provider_merge(isbn):
     """Fake provider 'merge' service."""
     try:  # pragma: no cover
-        named_tasks = (('openl', oed), ('thingl', ted))
+        named_tasks = (('openl', _oed), ('thingl', _ted))
         results = vias.parallel(named_tasks, isbn)
-        odata = results.get('openl', [])
-        tdata = results.get('thingl', [])
-        data = list(set(odata + tdata))
-        return data
+        odata = results.get('openl', set())
+        tdata = results.get('thingl', set())
+        return list(odata | tdata)
     except Exception:  # pragma: no cover
-        return []
+        LOGGER.error("Some error on editions 'merge' service for %s!", isbn)
+        return [isbn]
+
+
+@cache
+def get_editions(isbn, service):
+    """Select the provider."""
+    if service == 'merge':
+        eds = _fake_provider_merge(isbn)
+    if service == 'any':
+        eds = _fake_provider_any(isbn)
+    if service == 'openl':
+        eds = list(_oed(isbn))
+    if service == 'thingl':
+        eds = list(_ted(isbn))
+    return eds if eds else []
 
 
 def editions(isbn, service='merge'):
     """Return the list of ISBNs of editions related with this ISBN."""
     isbn = EAN13(isbn)
     if not isbn:
         LOGGER.critical('%s is not a valid ISBN', isbn)
         raise NotValidISBNError(isbn)
 
     if service not in PROVIDERS:
         LOGGER.critical('%s is not a recognized editions provider', service)
         raise NotRecognizedServiceError(service)
 
-    from .registry import metadata_cache
-    cache = metadata_cache
-    key = 'ed' + isbn + service
-    # some kinds of cache don't implement get!
-    # so don't use cache.get(key)
-    # BUG #58
-    try:
-        if cache[key]:
-            return cache[key]
-        else:  # pragma: no cover
-            raise KeyError  # <-- IMPORTANT: "caches don't return error"!
-    except KeyError:
-        if service == 'merge':
-            eds = fake_provider_merge(isbn)
-        if service == 'any':
-            eds = fake_provider_any(isbn)
-
-        if service == 'openl':
-            eds = oed(isbn)
-        if service == 'thingl':
-            eds = ted(isbn)
-
-        if eds:
-            cache[key] = eds
-            return eds
-    return []
+    return get_editions(isbn, service)
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/webquery.py` & `isbnlib-3.9.9/isbnlib/dev/webquery.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 """Base class to query a webservice and parse the result to py objects."""
 
 import json
 import logging
-from time import sleep, time as timestamp
+from time import sleep
+from time import time as timestamp
 
 from . import webservice
 from ._exceptions import DataNotFoundAtServiceError, ServiceIsDownError
 
 UA = 'isbnlib (gzip)'
 OUT_OF_SERVICE = 'Temporarily out of service'
 BOOK_NOT_FOUND = 'No results match your search'
 LOGGER = logging.getLogger(__name__)
 THROTTLING = 1
 
 
+# pylint: disable=useless-object-inheritance
 class WEBQuery(object):
     """Base class to query a webservice and parse the result to py objects."""
 
     T = {'id': timestamp()}  # noqa
 
     def __init__(self, service_url, ua=UA, throttling=THROTTLING):
         """Initialize & call webservice."""
@@ -30,15 +32,15 @@
         self.data = webservice.query(service_url, ua)
         WEBQuery.T[srv] = timestamp()
 
     def check_data(self, data_checker=None):  # pragma: no cover
         """Check the data & handle errors."""
         if data_checker:
             return data_checker(self.data)
-        if self.data == '{}':
+        if self.data == '{}':  # noqa
             LOGGER.warning('DataNotFoundAtServiceError for %s', self.url)
             raise DataNotFoundAtServiceError(self.url)
         if BOOK_NOT_FOUND in self.data:
             LOGGER.warning('DataNotFoundAtServiceError for %s', self.url)
             raise DataNotFoundAtServiceError(self.url)
         if OUT_OF_SERVICE in self.data:
             LOGGER.critical('ServiceIsDownError for %s', self.url)
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/_bouth23.py` & `isbnlib-3.9.9/isbnlib/dev/_bouth23.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,34 +11,34 @@
         return x
 
     def b(x):
         return x
 
     def u(x):
         try:
-            return unicode(x, "utf-8")
+            return unicode(x, 'utf-8')
         except TypeError:
             return x
 
     def b2u3(x):
-        return x.encode("utf-8")
+        return x.encode('utf-8')
 
     def type3str():
         return type(u'')
 
     def bstream(x):
         from StringIO import StringIO
         return StringIO(x)
 else:
 
     def s(x):
-        return x.decode("utf-8", 'ignore')
+        return x.decode('utf-8', 'ignore')
 
     def b(x):
-        return x.encode("utf-8")
+        return x.encode('utf-8')
 
     def u(x):
         return x
 
     def b2u3(x):
         return x
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/_data.py` & `isbnlib-3.9.9/isbnlib/dev/_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from ._helpers import normalize_space, titlecase
 
 # For now you cannot add custom fields!
 FIELDS = ('ISBN-13', 'Title', 'Authors', 'Publisher', 'Year', 'Language')
 LOGGER = logging.getLogger(__name__)
 
 
+# pylint: disable=useless-object-inheritance
 class Metadata(object):
     """Class for metadata objects."""
 
     def __init__(self, record=None):
         """Initialize attributes."""
         self._content = None
         self._set_empty()
-        if record:
+        if record:  # pragma: no cover
             self._content.update((k, v) for k, v in list(record.items()))
             if not self._validate():
                 self._set_empty()
                 LOGGER.debug(record)
                 raise NotValidMetadataError()
             self.clean()
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/vias.py` & `isbnlib-3.9.9/isbnlib/dev/vias.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 import logging
 
 from .. import config
 
 LOGGER = logging.getLogger(__name__)
 
 
+# pylint: disable=broad-except
 def serial(named_tasks, arg):
     """Use serial calls."""
     results = {}
     for name, task in named_tasks:
         try:
             results[name] = task(arg)
         except Exception:  # pragma: no cover
             LOGGER.debug("No result in 'serial' for %s[%s](%s)", task, name,
                          arg)
             results[name] = None
     return results
 
 
+# pylint: disable=broad-except
 def parallel(named_tasks, arg):
     """Use threaded calls."""
     from threading import Thread
     results = {}
 
     def _worker(name, task, arg):
         try:
@@ -37,14 +39,15 @@
     for name, task in named_tasks:
         t = Thread(target=_worker, args=(name, task, arg))
         t.start()
         t.join(config.THREADS_TIMEOUT)
     return results
 
 
+# pylint: disable=broad-except
 def multi(named_tasks, arg):
     """Use several cores (if available)."""
     from multiprocessing import Process, Queue
     results = {}
     q = Queue()
 
     def _worker(name, task, arg, q):
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/_exceptions.py` & `isbnlib-3.9.9/isbnlib/dev/_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # -*- coding: utf-8 -*-
 """Exceptions for 'isbnlib.dev'.
 
 The classes in isbnlib.dev should use the exceptions below.
 """
 
-# TODO merge these exceptions with the top exceptions on version 4.
+# TODO(MV) merge these exceptions with the top exceptions on version 4.
 
+from .._exceptions import ISBNLibException
 
-class ISBNLibDevException(Exception):
+
+# pylint: disable=super-init-not-called
+class ISBNLibDevException(ISBNLibException):
     """Base class for isbnlib.dev exceptions.
 
     This exception should not be raised directly,
     only subclasses of this exception should be used!
     """
 
     def __init__(self, msg=None):
@@ -21,68 +24,69 @@
     def __str__(self):
         return getattr(self, 'message', '')  # pragma: no cover
 
 
 class ISBNLibHTTPError(ISBNLibDevException):
     """Exception raised for HTTP related errors."""
 
-    message = "an HTTP error has ocurred"
+    message = 'an HTTP error has ocurred'
 
 
 class ISBNLibURLError(ISBNLibDevException):
     """Exception raised for URL related errors."""
 
-    message = "an URL error has ocurred"
+    message = 'an URL error has ocurred'
 
 
 class DataNotFoundAtServiceError(ISBNLibDevException):
     """Exception raised when there is no target data from the service."""
 
-    message = "the target data was not found at this service"
+    message = 'the target data was not found at this service'
 
 
 class ServiceIsDownError(ISBNLibDevException):
     """Exception raised when the service is not available."""
 
-    message = "the service is down (try later)"
+    message = 'the service is down (try later)'
 
 
 class DataWrongShapeError(ISBNLibDevException):
     """Exception raised when the data hasn't the expected format."""
 
     message = "the data hasn't the expected format"
 
 
 class NoDataForSelectorError(ISBNLibDevException):
     """Exception raised when there is no data for the selector."""
 
-    message = "no data for this selector"
+    message = 'no data for this selector'
 
 
 class NotValidMetadataError(ISBNLibDevException):
     """Exception raised when the metadata hasn't the expected format."""
 
     message = "the metadata hasn't the expected format"
 
 
 class ISBNNotConsistentError(ISBNLibDevException):
     """Exception raised when the isbn request != isbn response."""
 
-    message = "isbn request != isbn response"
+    message = 'isbn request != isbn response'
 
 
 class RecordMappingError(ISBNLibDevException):
     """Exception raised when the mapping records -> canonical doesn't work."""
 
     message = "the mapping `canonical <- records` doesn't work"
 
 
 class NoAPIKeyError(ISBNLibDevException):
     """Exception raised when the API Key for a service is not found."""
 
-    message = "this service needs an API key"
+    message = 'this service needs an API key'
 
 
+# pylint: disable=redefined-builtin
 class FileNotFoundError(ISBNLibDevException):
     """Exception raised when a given file doesn't exist."""
 
     message = "the file wasn't found"
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/helpers.py` & `isbnlib-3.9.9/isbnlib/dev/helpers.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # flake8:noqa
 # pylint: skip-file
 """Expose usefull features."""
 
 from .._imcache import IMCache
 from ._files import File, cwdfiles
 from ._fmt import _fmtbib, _fmts
-from ._helpers import unicode_to_utf8tex as to_utf8tex
 from ._helpers import (cutoff_tokens, fake_isbn, in_virtual, last_first,
                        normalize_space, parse_placeholders)
+from ._helpers import unicode_to_utf8tex as to_utf8tex
 
 # alias (to keep backwards compatibility)
 fmtbib = _fmtbib
 fmts = _fmts
 
 __all__ = [
     'File', 'IMCache', 'cutoff_tokens', 'cwdfiles', 'fmtbib', 'fmts',
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/_files.py` & `isbnlib-3.9.9/isbnlib/dev/_files.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 
 import fnmatch
 import logging
 import os
 import re
 from stat import S_IRGRP, S_IROTH, S_IRUSR, S_IWGRP, S_IWOTH, S_IWUSR
 
+# pylint: disable=redefined-builtin
 from ._exceptions import FileNotFoundError
 
 MAXLEN = 120
 ILEGAL = r'<>:"/\|?*'
 LOGGER = logging.getLogger(__name__)
 MODE666 = S_IRUSR | S_IWUSR | S_IRGRP | S_IWGRP | S_IROTH | S_IWOTH
 
 
+# pylint: disable=useless-object-inheritance
 class File(object):
     """Easy manipulation of files in the SAME directory."""
 
     def __init__(self, fp):
         """Set and validate the basic properties."""
         if not self.isfile(fp):
             raise FileNotFoundError(fp)
@@ -50,22 +52,22 @@
         name = re.sub(r'\s\s+', ' ', name) if space == ' ' else name
         return name[:MAXLEN]
 
     @staticmethod
     def validate(basename):
         """Check for a proper basename."""
         if basename != os.path.basename(basename):
-            LOGGER.critical("This (%s) is not a basename!", basename)
+            LOGGER.critical('This (%s) is not a basename!', basename)
             return False
         name, ext = os.path.splitext(basename)
         if not name:
-            LOGGER.critical("Not a valid name (lenght 0)!")
+            LOGGER.critical('Not a valid name (lenght 0)!')
             return False
         if not ext:
-            LOGGER.critical("Not a valid extension (lenght 0)!")
+            LOGGER.critical('Not a valid extension (lenght 0)!')
             return False
         return True
 
     def baserename(self, new_basename):
         """Rename the file to a 'safe' basename."""
         if not self.validate(new_basename):
             return False
@@ -74,21 +76,21 @@
         new_basename = name + ext
         if new_basename == self.basename:
             return True
         if new_basename not in self.siblings():
             try:
                 os.rename(self.basename, new_basename)
             except OSError as err:
-                LOGGER.critical("%s", err)
+                LOGGER.critical('%s', err)
                 return False
             self.basename = new_basename
             self.name = name
             self.ext = ext
         else:
-            LOGGER.info("The file (%s) already exist in the directory!",
+            LOGGER.info('The file (%s) already exist in the directory!',
                         new_basename)
         return True
 
     @staticmethod
     def uxchmod(fp, mode=MODE666):
         """Change the mode of the file (default is 0666)."""
         return os.chmod(fp, mode)
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/webservice.py` & `isbnlib-3.9.9/isbnlib/dev/webservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     from urllib2 import Request, urlopen, HTTPError, URLError
 
 UA = 'isbnlib (gzip)'
 LOGGER = logging.getLogger(__name__)
 
 
 # pylint: disable=too-few-public-methods
+# pylint: disable=useless-object-inheritance
 class WEBService(object):
     """Class to query web services."""
 
     def __init__(self, url, user_agent=UA, values=None, appheaders=None):
         """Initialize main properties."""
         self._url = url
         # headers to accept gzipped content
@@ -44,19 +45,19 @@
         try:
             response = urlopen(self._request, timeout=config.URLOPEN_TIMEOUT)
             LOGGER.debug('Request headers:\n%s', self._request.header_items())
         except HTTPError as e:  # pragma: no cover
             LOGGER.critical('ISBNLibHTTPError for %s with code %s [%s]',
                             self._url, e.code, e.msg)
             if e.code in (401, 403, 429):
-                raise ISBNLibHTTPError(
-                    '%s Are you making many requests?' % e.code)
+                raise ISBNLibHTTPError('%s Are you making many requests?' %
+                                       e.code)
             if e.code in (502, 504):
-                raise ISBNLibHTTPError(
-                    '%s Service temporarily unavailable!' % e.code)
+                raise ISBNLibHTTPError('%s Service temporarily unavailable!' %
+                                       e.code)
             raise ISBNLibHTTPError('(%s) %s' % (e.code, e.msg))
         except URLError as e:  # pragma: no cover
             LOGGER.critical('ISBNLibURLError for %s with reason %s', self._url,
                             e.reason)
             raise ISBNLibURLError(e.reason)
         return response if response else None
 
@@ -71,12 +72,14 @@
         else:  # pragma: no cover
             data = res.read()
         return s(data)
 
 
 def query(url, user_agent=UA, values=None, appheaders=None):
     """Query to a web service."""
-    service = WEBService(
-        url, user_agent=user_agent, values=values, appheaders=appheaders)
+    service = WEBService(url,
+                         user_agent=user_agent,
+                         values=values,
+                         appheaders=appheaders)
     data = service.data()
     LOGGER.debug('Raw data from service:\n%s', data)
     return data
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/_fmt.py` & `isbnlib-3.9.9/isbnlib/dev/_fmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,23 +113,23 @@
         AUTHORS = ' and '.join(authors)
     elif name == 'refworks':
         AUTHORS = '\nA1  - '.join(authors)
     elif name == 'endnote':
         AUTHORS = '\n%A '.join(authors)
     elif name == 'msword':
         fmtrec = fmtrec.replace('$uid', str(uuid.uuid4()))
-        person = r"<b:Person><b:Last>$last</b:Last>"\
-                 r"<b:First>$first</b:First></b:Person>"
+        person = r'<b:Person><b:Last>$last</b:Last>'\
+                 r'<b:First>$first</b:First></b:Person>'
         AUTHORS = '\n'.join(
             Template(person).safe_substitute(last_first(a)) for a in authors)
     elif name == 'json':
-        AUTHORS = ', '.join('{"name": "$"}'.replace("$", a) for a in authors)
+        AUTHORS = ', '.join('{"name": "$"}'.replace('$', a) for a in authors)
     elif name == 'csl':
-        AUTHORS = ', '.join(
-            '{"literal": "$"}'.replace("$", a) for a in authors)
+        AUTHORS = ', '.join('{"literal": "$"}'.replace('$', a)
+                            for a in authors)
     elif name == 'opf':
         fmtrec = fmtrec.replace('$uid', str(uuid.uuid4()))
         creator = r'<dc:creator opf:file-as="$last, $first"'\
                   r' opf:role="aut">$first $last</dc:creator>'
         AUTHORS = '\n    '.join(
             Template(creator).safe_substitute(last_first(author))
             for author in authors)
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/__init__.py` & `isbnlib-3.9.9/isbnlib/dev/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 """Interface for namespace 'isbnlib.dev'."""
 
 from . import helpers, vias
 from ._data import Metadata, stdmeta
-from ._exceptions import (
-    DataNotFoundAtServiceError, DataWrongShapeError, ISBNLibDevException,
-    ISBNLibHTTPError, ISBNLibURLError, NoAPIKeyError, NoDataForSelectorError,
-    NotValidMetadataError, RecordMappingError, ServiceIsDownError)
+from ._decorators import cache
+from ._exceptions import (DataNotFoundAtServiceError, DataWrongShapeError,
+                          ISBNLibDevException, ISBNLibHTTPError,
+                          ISBNLibURLError, NoAPIKeyError,
+                          NoDataForSelectorError, NotValidMetadataError,
+                          RecordMappingError, ServiceIsDownError)
 from .webquery import WEBQuery
 from .webservice import WEBService
 
 # alias
 ISBNToolsDevException = ISBNLibDevException
 ISBNToolsHTTPError = ISBNLibHTTPError
 ISBNToolsURLError = ISBNLibURLError
 
 __all__ = ('ISBNToolsDevException', 'ISBNLibDevException',
            'ISBNToolsHTTPError', 'ISBNToolsURLError', 'ISBNLibHTTPError',
            'ISBNLibURLError', 'DataNotFoundAtServiceError',
            'ServiceIsDownError', 'DataWrongShapeError',
            'NotValidMetadataError', 'NoDataForSelectorError',
            'RecordMappingError', 'NoAPIKeyError', 'Metadata', 'stdmeta',
-           'WEBService', 'WEBQuery', 'vias', 'helpers')
+           'WEBService', 'WEBQuery', 'vias', 'helpers', 'cache')
```

### Comparing `isbnlib-3.9.8/isbnlib/dev/_helpers.py` & `isbnlib-3.9.9/isbnlib/dev/_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from hashlib import md5
 
 from ._bouth23 import b, s
 
 
 def fake_isbn(title, author='unkown', publisher='unkown', sid=1):
     """Produce a fake ISBN from the (title, author, publisher) of the book."""
-    key = "%s %s %s" % (title, author, publisher)
+    key = '%s %s %s' % (title, author, publisher)
     # normalize
     regex1 = re.compile(r'\?|,|\.|!|\:|;', re.I | re.M | re.S)
     regex2 = re.compile(r'\s\s+', re.I | re.M | re.S)
     key = regex1.sub(' ', key)
     key = regex2.sub(' ', key).strip().lower()
     # hash
     return (str(sid) + str(int(md5(b(key)).hexdigest()[:10], 16)))[:13]
@@ -36,16 +36,16 @@
     return item.strip()
 
 
 def titlecase(st):
     """Format string in 'title case' (for ascii)."""
     try:
         st.encode('ascii')
-        return re.sub(r"[A-Za-z]+('[A-Za-z]+)?",
-                      lambda m: m.group(0)[0].upper() + m.group(0)[1:], st)
+        return re.sub(r"[A-Za-z]+('[A-Za-z]+)?", lambda m: m.group(0)[0].upper(
+        ) + m.group(0)[1:], st)
     except (UnicodeEncodeError, UnicodeDecodeError):  # pragma: no cover
         return st
 
 
 def last_first(author):
     """Parse an author name into last (name) and first."""
     if ',' in author:
@@ -59,28 +59,30 @@
     return {'last': last, 'first': first}
 
 
 def unicode_to_utf8tex(utex, filtre=()):
     """Replace unicode entities with tex entitites and returns utf8 bytes."""
     from .._data.data4tex import unicode_to_tex
     btex = utex.encode('utf-8')
-    table = dict((k.encode('utf-8'), v) for k, v in unicode_to_tex.items()
-                 if v not in filtre)
+    table = {
+        k.encode('utf-8'): v
+        for k, v in unicode_to_tex.items() if v not in filtre
+    }
     regex = re.compile(b('|'.join(re.escape(s(k)) for k in table)))
     return regex.sub(lambda m: table[m.group(0)], btex)
 
 
 def cutoff_tokens(tokens, cutoff):
     """Keep only the tokens with total length <= cutoff."""
     ltokens = [len(t) for t in tokens]
     length = 0
     stokens = []
-    for token, l in zip(tokens, ltokens):
-        if length + l <= cutoff:
-            length = length + l
+    for token, ln in zip(tokens, ltokens):
+        if length + ln <= cutoff:
+            length = length + ln
             stokens.append(token)
         else:
             break
     return stokens
 
 
 def parse_placeholders(pattern):
```

### Comparing `isbnlib-3.9.8/isbnlib/_infogroup.py` & `isbnlib-3.9.9/isbnlib/_infogroup.py`

 * *Files identical despite different names*

### Comparing `isbnlib-3.9.8/PKG-INFO` & `isbnlib-3.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 1.1
 Name: isbnlib
-Version: 3.9.8
+Version: 3.9.9
 Summary: Extract, clean, transform, hyphenate and metadata for ISBNs (International Standard Book Number).
 Home-page: https://github.com/xlcnd/isbnlib
 Author: Alexandre Lima Conde
 Author-email: xlcnd@outlook.com
 License: LGPL v3
-Download-URL: https://github.com/xlcnd/isbnlib/archive/v3.9.8.zip
+Download-URL: https://github.com/xlcnd/isbnlib/archive/v3.9.9.zip
 Project-URL: Bug Reports, https://github.com/xlcnd/isbnlib/issues
 Project-URL: Dev Docs, https://isbnlib.readthedocs.io/en/latest/devs.html
 Project-URL: Forum, https://stackoverflow.com/search?tab=newest&q=isbnlib
-Project-URL: License, https://github.com/xlcnd/isbnlib/blob/dev/LICENSE
+Project-URL: License, https://github.com/xlcnd/isbnlib/blob/dev/LICENSE-LGPL-3.0-only.txt
 Description: 
         .. image:: https://img.shields.io/badge/Sourcegraph-Status-blue.svg
             :target: https://sourcegraph.com/github.com/xlcnd/isbnlib
             :alt: Graph
         
         .. image:: https://readthedocs.org/projects/isbnlib/badge/?version=latest
             :target: https://isbnlib.readthedocs.org/en/latest/
             :alt: Documentation Status
         
-        .. image:: https://coveralls.io/repos/github/xlcnd/isbnlib/badge.svg?branch=v3.9.8
-            :target: https://coveralls.io/github/xlcnd/isbnlib?branch=v3.9.8
+        .. image:: https://coveralls.io/repos/github/xlcnd/isbnlib/badge.svg?branch=v3.9.9
+            :target: https://coveralls.io/github/xlcnd/isbnlib?branch=v3.9.9
             :alt: Coverage Status
         
-        .. image:: https://travis-ci.org/xlcnd/isbnlib.svg?branch=v3.9.8
+        .. image:: https://travis-ci.org/xlcnd/isbnlib.svg?branch=v3.9.9
             :target: https://travis-ci.org/xlcnd/isbnlib
             :alt: Built Status
         
-        .. image:: https://ci.appveyor.com/api/projects/status/github/xlcnd/isbnlib?branch=v3.9.8&svg=true
+        .. image:: https://ci.appveyor.com/api/projects/status/github/xlcnd/isbnlib?branch=v3.9.9&svg=true
             :target: https://ci.appveyor.com/project/xlcnd/isbnlib
             :alt: Windows Built Status
         
         .. image:: https://img.shields.io/github/issues/xlcnd/isbnlib/bug.svg?label=bugs&style=flat
             :target: https://github.com/xlcnd/isbnlib/labels/bug
             :alt: Bugs
         
@@ -41,14 +41,15 @@
             :alt: PYPI Downloads
         
         
         
         Warning
         =======
         
+        
             **Breaking Change** The service xISBN was decommissioned (see issue 51_)!
         
         
         
         Info
         ====
         
@@ -181,14 +182,15 @@
         
         See files test_core_ and test_ext_ for **a lot of examples**.
         
         
         Install
         =======
         
+        
         From the command line, enter (in some cases you have to preced the
         command with ``sudo``):
         
         
         .. code-block:: bash
         
             $ pip install isbnlib
@@ -203,19 +205,22 @@
         For Devs
         ========
         
         
         API's Main Namespaces
         ---------------------
         
-        In the namespace ``isbnlib`` you have access to the core methods:
+        In the namespace ``isbnlib`` you have access to the **core functions**:
         ``is_isbn10``, ``is_isbn13``, ``to_isbn10``, ``to_isbn13``, ``canonical``,
         ``clean``, ``notisbn``, ``get_isbnlike``, ``get_canonical_isbn``, ``mask``,
-        ``meta``, ``info``, ``editions``, ``goom``, ``ren``, ``doi``, ``EAN13``,
-        ``isbn_from_words``, ``desc`` and ``cover``.
+        ``info``, ``check_digit10``, ``check_digit13``, ``doi`` and ``EAN13``.
+        
+        In addition, you have access to **metadata functions**, namely:
+        ``meta``, ``editions``, ``ren``, ``desc``, ``cover``,
+        ``goom``, ``doi2tex`` and ``isbn_from_words``.
         
         The exceptions raised by these methods can all be catched using ``ISBNLibException``.
         
         
         You can extend the lib by using the classes and functions exposed in
         namespace ``isbnlib.dev``, namely:
         
@@ -302,14 +307,78 @@
         at goob_.
         
         
         Remember that plugins **must** support python 2.7 and python 3.5+ (see python-future.org_).
         
         
         
+        Patterns of Usage
+        -----------------
+        
+        The library implements a very simple API with sensible defaults, but there are cases
+        that need your attention (see case 3 below).
+        
+        
+        
+        A. You only need **core functions**:
+        
+        
+        .. code-block:: python
+        
+            # import the core functions you need
+            from isbnlib import canonical, is_isbn10, is_isbn13
+        
+            isbn = canonical("978-0446310789")
+            if is_isbn13(isbn):
+                ...
+            ...
+        
+        
+        B. You need also **metadata functions**, with **default config**:
+        
+        
+        .. code-block:: python
+        
+            from isbnlib import canonical, meta, description
+        
+            isbn = canonical("978-0446310789")
+            data = meta(isbn)
+            ...
+        
+        C. You need also **metadata functions**, with **special config**:
+        
+           *Lets suppose you need to add an api key for a metadata plugin
+           and change the cache too*.
+        
+        
+        .. code-block:: python
+        
+            from myapp.utils import MyCache
+        
+            # import the functions you need, plus 'config' and 'registry'
+            from isbnlib import canonical, config, meta, registry
+        
+            # you should use 'config' first
+            config.add_apikey('isbndb', 'kjshdfkjahsdflkjh')
+        
+            # then 'registry'
+            registry.set_cache(MyCache())
+        
+            # Only now you should use metadata functions
+            # (there are no adaptions for core functions,
+            #  so they can be used at any moment)
+            isbn = canonical("978-0446310789")
+            data = meta(isbn, service="isbndb")
+            ...
+        
+        
+        D. You want to build a **plugin** or use **isbnlib.dev** in your code:
+        
+           You should study very carefully the **public** methods in ``dir(isbnlib.dev)``.
+        
         
         
         Caveats
         -------
         
         
         1. These classes are optimized for one-call to services and not for batch calls.
@@ -321,38 +390,46 @@
         
         
         Projects using *isbnlib*
         ------------------------
         
         **isbntools**      https://github.com/xlcnd/isbntools
         
+        **isbnsrv**        https://github.com/xlcnd/isbnsrv
+        
         **Open Library**   https://github.com/internetarchive/openlibrary
         
-        **Spreads**        https://github.com/DIYBookScanner/spreads
+        **NYPL Library Simplified**  https://github.com/NYPL-Simplified
+        
+        **Manubot**   https://github.com/manubot
+        
+        **Spreads**  https://github.com/DIYBookScanner/spreads
         
         **Papis**    https://github.com/papis/papis
         
         **libBMC**    https://github.com/Phyks/libbmc/
         
-        **Alessandria**     https://gitlab.com/openlabmatera/alessandria
+        **Alessandria**      https://gitlab.com/openlabmatera/alessandria
         
         **Comic Collector**  https://github.com/wengole/comiccollector
         
-        **Abelujo**    http://www.abelujo.cc/
+        **Abelujo**   https://github.com/vindarel/abelujo
+        
+        **BibLib**    https://pypi.org/project/biblib/
         
-        **BibLib**    https://pypi.python.org/pypi/biblib
+        **L-Space**   https://pypi.org/project/lspace/
         
         
         
         Help
         ----
         
         
         If you need help, please take a look at github_ or post a question on
-        stackoverflow_ (with tag **isbnlib**)
+        stackoverflow_ .
         
         
         
         ----------------------------------------------------------------------------------------------
         
         .. class:: center
         
@@ -367,15 +444,15 @@
         
         .. _isbntools: https://pypi.python.org/pypi/isbntools
         
         .. _sourcegraph: http://bit.ly/ISBNLib_srcgraph
         
         .. _readthedocs: http://bit.ly/ISBNLib_rtd
         
-        .. _stackoverflow: http://stackoverflow.com/questions/tagged/isbnlib
+        .. _stackoverflow: http://stackoverflow.com/search?tab=newest&q=isbnlib
         
         .. _test_core: https://github.com/xlcnd/isbnlib/blob/master/isbnlib/test/test_core.py
         
         .. _test_ext: https://github.com/xlcnd/isbnlib/blob/master/isbnlib/test/test_ext.py
         
         .. _isbn-international.org: https://www.isbn-international.org/content/what-isbn
```

### Comparing `isbnlib-3.9.8/setup.py` & `isbnlib-3.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 from datetime import datetime as dt
 from setuptools import setup
 from isbnlib import __version__
 
 PROJECT_NAME = 'isbnlib'
 PROJECT_PACKAGE_NAME = 'isbnlib'
 PROJECT_LICENSE = 'LGPL v3'
-PROJECT_LICENSE_URL = 'https://github.com/xlcnd/isbnlib/blob/dev/LICENSE'
+PROJECT_LICENSE_URL = 'https://github.com/xlcnd/isbnlib/blob/dev/LICENSE-LGPL-3.0-only.txt'
 PROJECT_AUTHOR = 'Alexandre Lima Conde'
 PROJECT_COPYRIGHT = ' 2014-{}, {}'.format(dt.now().year, PROJECT_AUTHOR)
 PROJECT_URL = 'https://github.com/xlcnd/isbnlib'
 PROJECT_EMAIL = 'xlcnd@outlook.com'
 PROJECT_VERSION = __version__
 
 PROJECT_GITHUB_USERNAME = 'xlcnd'
 PROJECT_GITHUB_REPOSITORY = 'isbnlib'
 
 GITHUB_PATH = '{}/{}'.format(PROJECT_GITHUB_USERNAME,
                              PROJECT_GITHUB_REPOSITORY)
 GITHUB_URL = 'https://github.com/{}'.format(GITHUB_PATH)
 
-DOWNLOAD_URL = '{}/archive/{}.zip'.format(GITHUB_URL, "v" + PROJECT_VERSION)
+DOWNLOAD_URL = '{}/archive/{}.zip'.format(GITHUB_URL, 'v' + PROJECT_VERSION)
 PROJECT_URLS = {
     'Bug Reports': '{}/issues'.format(GITHUB_URL),
     'Dev Docs': 'https://isbnlib.readthedocs.io/en/latest/devs.html',
     'Forum': 'https://stackoverflow.com/search?tab=newest&q=isbnlib',
     'License': PROJECT_LICENSE_URL,
 }
 
@@ -64,18 +64,16 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
 ]
 
 PACKAGES = [
     'isbnlib',
     'isbnlib/dev',
     'isbnlib/_data',
-    'isbnlib/test',
 ]
 
-
 setup(
     name=PROJECT_PACKAGE_NAME,
     version=PROJECT_VERSION,
     url=PROJECT_URL,
     download_url=DOWNLOAD_URL,
     project_urls=PROJECT_URLS,
     author=PROJECT_AUTHOR,
@@ -84,10 +82,8 @@
     license=PROJECT_LICENSE,
     description=
     'Extract, clean, transform, hyphenate and metadata for ISBNs (International Standard Book Number).',
     long_description=open('README.rst').read(),
     keywords=
     'ISBN metadata World_Catalogue Google_Books Open_Library BibTeX EndNote RefWorks MSWord opf BibJSON',
     classifiers=PYPI_CLASSIFIERS,
-    tests_require=['nose', 'coverage'],
-    test_suite='nose.collector',
 )
```

### Comparing `isbnlib-3.9.8/COPYRIGHT.txt` & `isbnlib-3.9.9/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `isbnlib-3.9.8/.coveragerc` & `isbnlib-3.9.9/.coveragerc`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [run]
 source = isbnlib
 branch = True
 
 [report]
 # Regexes for directories to exclude from consideration
-omit = 
+omit =
     */test/*
     */python?.?/*
     */site-packages/nose/*
     *version*
     *isbndb*
     *fmt*
     *bouth*
@@ -36,8 +36,8 @@
 
     # Don't complain if non-runnable code isn't run:
     if 0:
     if __name__ == .__main__.:
 
 ignore_errors = True
 
-fail_under = 90 
+fail_under = 90
```

### Comparing `isbnlib-3.9.8/README.rst` & `isbnlib-3.9.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
     :target: https://sourcegraph.com/github.com/xlcnd/isbnlib
     :alt: Graph
 
 .. image:: https://readthedocs.org/projects/isbnlib/badge/?version=latest
     :target: https://isbnlib.readthedocs.org/en/latest/
     :alt: Documentation Status
 
-.. image:: https://coveralls.io/repos/github/xlcnd/isbnlib/badge.svg?branch=v3.9.8
-    :target: https://coveralls.io/github/xlcnd/isbnlib?branch=v3.9.8
+.. image:: https://coveralls.io/repos/github/xlcnd/isbnlib/badge.svg?branch=v3.9.9
+    :target: https://coveralls.io/github/xlcnd/isbnlib?branch=v3.9.9
     :alt: Coverage Status
 
-.. image:: https://travis-ci.org/xlcnd/isbnlib.svg?branch=v3.9.8
+.. image:: https://travis-ci.org/xlcnd/isbnlib.svg?branch=v3.9.9
     :target: https://travis-ci.org/xlcnd/isbnlib
     :alt: Built Status
 
-.. image:: https://ci.appveyor.com/api/projects/status/github/xlcnd/isbnlib?branch=v3.9.8&svg=true
+.. image:: https://ci.appveyor.com/api/projects/status/github/xlcnd/isbnlib?branch=v3.9.9&svg=true
     :target: https://ci.appveyor.com/project/xlcnd/isbnlib
     :alt: Windows Built Status
 
 .. image:: https://img.shields.io/github/issues/xlcnd/isbnlib/bug.svg?label=bugs&style=flat
     :target: https://github.com/xlcnd/isbnlib/labels/bug
     :alt: Bugs
 
@@ -28,14 +28,15 @@
     :alt: PYPI Downloads
 
 
 
 Warning
 =======
 
+
     **Breaking Change** The service xISBN was decommissioned (see issue 51_)!
 
 
 
 Info
 ====
 
@@ -168,14 +169,15 @@
 
 See files test_core_ and test_ext_ for **a lot of examples**.
 
 
 Install
 =======
 
+
 From the command line, enter (in some cases you have to preced the
 command with ``sudo``):
 
 
 .. code-block:: bash
 
     $ pip install isbnlib
@@ -190,19 +192,22 @@
 For Devs
 ========
 
 
 API's Main Namespaces
 ---------------------
 
-In the namespace ``isbnlib`` you have access to the core methods:
+In the namespace ``isbnlib`` you have access to the **core functions**:
 ``is_isbn10``, ``is_isbn13``, ``to_isbn10``, ``to_isbn13``, ``canonical``,
 ``clean``, ``notisbn``, ``get_isbnlike``, ``get_canonical_isbn``, ``mask``,
-``meta``, ``info``, ``editions``, ``goom``, ``ren``, ``doi``, ``EAN13``,
-``isbn_from_words``, ``desc`` and ``cover``.
+``info``, ``check_digit10``, ``check_digit13``, ``doi`` and ``EAN13``.
+
+In addition, you have access to **metadata functions**, namely:
+``meta``, ``editions``, ``ren``, ``desc``, ``cover``,
+``goom``, ``doi2tex`` and ``isbn_from_words``.
 
 The exceptions raised by these methods can all be catched using ``ISBNLibException``.
 
 
 You can extend the lib by using the classes and functions exposed in
 namespace ``isbnlib.dev``, namely:
 
@@ -289,14 +294,78 @@
 at goob_.
 
 
 Remember that plugins **must** support python 2.7 and python 3.5+ (see python-future.org_).
 
 
 
+Patterns of Usage
+-----------------
+
+The library implements a very simple API with sensible defaults, but there are cases
+that need your attention (see case 3 below).
+
+
+
+A. You only need **core functions**:
+
+
+.. code-block:: python
+
+    # import the core functions you need
+    from isbnlib import canonical, is_isbn10, is_isbn13
+
+    isbn = canonical("978-0446310789")
+    if is_isbn13(isbn):
+        ...
+    ...
+
+
+B. You need also **metadata functions**, with **default config**:
+
+
+.. code-block:: python
+
+    from isbnlib import canonical, meta, description
+
+    isbn = canonical("978-0446310789")
+    data = meta(isbn)
+    ...
+
+C. You need also **metadata functions**, with **special config**:
+
+   *Lets suppose you need to add an api key for a metadata plugin
+   and change the cache too*.
+
+
+.. code-block:: python
+
+    from myapp.utils import MyCache
+
+    # import the functions you need, plus 'config' and 'registry'
+    from isbnlib import canonical, config, meta, registry
+
+    # you should use 'config' first
+    config.add_apikey('isbndb', 'kjshdfkjahsdflkjh')
+
+    # then 'registry'
+    registry.set_cache(MyCache())
+
+    # Only now you should use metadata functions
+    # (there are no adaptions for core functions,
+    #  so they can be used at any moment)
+    isbn = canonical("978-0446310789")
+    data = meta(isbn, service="isbndb")
+    ...
+
+
+D. You want to build a **plugin** or use **isbnlib.dev** in your code:
+
+   You should study very carefully the **public** methods in ``dir(isbnlib.dev)``.
+
 
 
 Caveats
 -------
 
 
 1. These classes are optimized for one-call to services and not for batch calls.
@@ -308,38 +377,46 @@
 
 
 Projects using *isbnlib*
 ------------------------
 
 **isbntools**      https://github.com/xlcnd/isbntools
 
+**isbnsrv**        https://github.com/xlcnd/isbnsrv
+
 **Open Library**   https://github.com/internetarchive/openlibrary
 
-**Spreads**        https://github.com/DIYBookScanner/spreads
+**NYPL Library Simplified**  https://github.com/NYPL-Simplified
+
+**Manubot**   https://github.com/manubot
+
+**Spreads**  https://github.com/DIYBookScanner/spreads
 
 **Papis**    https://github.com/papis/papis
 
 **libBMC**    https://github.com/Phyks/libbmc/
 
-**Alessandria**     https://gitlab.com/openlabmatera/alessandria
+**Alessandria**      https://gitlab.com/openlabmatera/alessandria
 
 **Comic Collector**  https://github.com/wengole/comiccollector
 
-**Abelujo**    http://www.abelujo.cc/
+**Abelujo**   https://github.com/vindarel/abelujo
+
+**BibLib**    https://pypi.org/project/biblib/
 
-**BibLib**    https://pypi.python.org/pypi/biblib
+**L-Space**   https://pypi.org/project/lspace/
 
 
 
 Help
 ----
 
 
 If you need help, please take a look at github_ or post a question on
-stackoverflow_ (with tag **isbnlib**)
+stackoverflow_ .
 
 
 
 ----------------------------------------------------------------------------------------------
 
 .. class:: center
 
@@ -354,15 +431,15 @@
 
 .. _isbntools: https://pypi.python.org/pypi/isbntools
 
 .. _sourcegraph: http://bit.ly/ISBNLib_srcgraph
 
 .. _readthedocs: http://bit.ly/ISBNLib_rtd
 
-.. _stackoverflow: http://stackoverflow.com/questions/tagged/isbnlib
+.. _stackoverflow: http://stackoverflow.com/search?tab=newest&q=isbnlib
 
 .. _test_core: https://github.com/xlcnd/isbnlib/blob/master/isbnlib/test/test_core.py
 
 .. _test_ext: https://github.com/xlcnd/isbnlib/blob/master/isbnlib/test/test_ext.py
 
 .. _isbn-international.org: https://www.isbn-international.org/content/what-isbn
```

