# Comparing `tmp/digiDownload-0.0.4.tar.gz` & `tmp/digiDownload-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiDownload-0.0.4.tar", last modified: Mon Apr 17 13:56:28 2023, max compression
+gzip compressed data, was "digiDownload-0.2.0.tar", last modified: Wed Apr 26 16:18:43 2023, max compression
```

## Comparing `digiDownload-0.0.4.tar` & `digiDownload-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-17 13:56:28.554043 digiDownload-0.0.4/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-17 13:56:28.554043 digiDownload-0.0.4/PKG-INFO
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-17 13:56:28.554043 digiDownload-0.0.4/digiDownload/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      176 2023-04-15 14:38:11.000000 digiDownload-0.0.4/digiDownload/AdBlockCookiePolicy.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     2564 2023-04-17 13:53:54.000000 digiDownload-0.0.4/digiDownload/Book.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)      628 2023-04-15 16:01:32.000000 digiDownload-0.0.4/digiDownload/LTIParser.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1293 2023-04-15 18:46:06.000000 digiDownload-0.0.4/digiDownload/Session.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)       29 2023-04-15 17:22:08.000000 digiDownload-0.0.4/digiDownload/__init__.py
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-17 13:56:28.554043 digiDownload-0.0.4/digiDownload.egg-info/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/PKG-INFO
--rw-r--r--   0 notyou    (1000) notyou    (1000)      329 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/SOURCES.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/dependency_links.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       24 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/requires.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-17 13:56:28.000000 digiDownload-0.0.4/digiDownload.egg-info/top_level.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       79 2023-04-17 13:56:28.554043 digiDownload-0.0.4/setup.cfg
--rw-r--r--   0 notyou    (1000) notyou    (1000)      464 2023-04-17 13:56:26.000000 digiDownload-0.0.4/setup.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 16:18:43.188696 digiDownload-0.2.0/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1069 2023-04-20 11:45:13.000000 digiDownload-0.2.0/LICENSE
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 16:18:43.188696 digiDownload-0.2.0/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1142 2023-04-26 14:37:11.000000 digiDownload-0.2.0/README.md
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 16:18:43.188696 digiDownload-0.2.0/digiDownload/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      194 2023-04-20 13:03:54.000000 digiDownload-0.2.0/digiDownload/AdBlockCookiePolicy.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     5553 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/Book.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      789 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/LTIParser.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     2084 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/Session.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      214 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/__init__.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1695 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/cli_tool.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       85 2023-04-26 14:38:53.000000 digiDownload-0.2.0/digiDownload/exceptions.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 16:18:43.188696 digiDownload-0.2.0/digiDownload.egg-info/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      399 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/SOURCES.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/dependency_links.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       42 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/requires.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/top_level.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      102 2023-04-26 16:18:43.188696 digiDownload-0.2.0/setup.cfg
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      537 2023-04-26 16:14:25.000000 digiDownload-0.2.0/setup.py
```

