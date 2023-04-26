# Comparing `tmp/digiDownload-1.0.3.tar.gz` & `tmp/digiDownload-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiDownload-1.0.3.tar", last modified: Wed Apr 26 17:17:57 2023, max compression
+gzip compressed data, was "digiDownload-1.0.5.tar", last modified: Wed Apr 26 17:22:14 2023, max compression
```

## Comparing `digiDownload-1.0.3.tar` & `digiDownload-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:17:57.815537 digiDownload-1.0.3/
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1069 2023-04-20 11:45:13.000000 digiDownload-1.0.3/LICENSE
--rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 17:17:57.815537 digiDownload-1.0.3/PKG-INFO
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1142 2023-04-26 14:37:11.000000 digiDownload-1.0.3/README.md
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:17:57.815537 digiDownload-1.0.3/digiDownload/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      194 2023-04-20 13:03:54.000000 digiDownload-1.0.3/digiDownload/AdBlockCookiePolicy.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     5563 2023-04-26 17:08:41.000000 digiDownload-1.0.3/digiDownload/Book.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)      800 2023-04-26 17:08:41.000000 digiDownload-1.0.3/digiDownload/LTIParser.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     2120 2023-04-26 17:08:41.000000 digiDownload-1.0.3/digiDownload/Session.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)       60 2023-04-26 17:16:57.000000 digiDownload-1.0.3/digiDownload/__init__.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)      101 2023-04-26 17:16:57.000000 digiDownload-1.0.3/digiDownload/__main__.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1703 2023-04-26 17:08:41.000000 digiDownload-1.0.3/digiDownload/cli_tool.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)       85 2023-04-26 14:38:53.000000 digiDownload-1.0.3/digiDownload/exceptions.py
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:17:57.815537 digiDownload-1.0.3/digiDownload.egg-info/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 17:17:57.000000 digiDownload-1.0.3/digiDownload.egg-info/PKG-INFO
--rw-r--r--   0 notyou    (1000) notyou    (1000)      424 2023-04-26 17:17:57.000000 digiDownload-1.0.3/digiDownload.egg-info/SOURCES.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-26 17:17:57.000000 digiDownload-1.0.3/digiDownload.egg-info/dependency_links.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       49 2023-04-26 17:17:57.000000 digiDownload-1.0.3/digiDownload.egg-info/requires.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-26 17:17:57.000000 digiDownload-1.0.3/digiDownload.egg-info/top_level.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)      102 2023-04-26 17:17:57.815537 digiDownload-1.0.3/setup.cfg
--rw-r--r--   0 notyou    (1000) notyou    (1000)      555 2023-04-26 17:17:30.000000 digiDownload-1.0.3/setup.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:22:14.205806 digiDownload-1.0.5/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1069 2023-04-20 11:45:13.000000 digiDownload-1.0.5/LICENSE
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      328 2023-04-26 17:22:14.205806 digiDownload-1.0.5/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1142 2023-04-26 14:37:11.000000 digiDownload-1.0.5/README.md
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:22:14.205806 digiDownload-1.0.5/digiDownload/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      194 2023-04-20 13:03:54.000000 digiDownload-1.0.5/digiDownload/AdBlockCookiePolicy.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     5563 2023-04-26 17:08:41.000000 digiDownload-1.0.5/digiDownload/Book.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      800 2023-04-26 17:08:41.000000 digiDownload-1.0.5/digiDownload/LTIParser.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     2120 2023-04-26 17:08:41.000000 digiDownload-1.0.5/digiDownload/Session.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       60 2023-04-26 17:16:57.000000 digiDownload-1.0.5/digiDownload/__init__.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      101 2023-04-26 17:16:57.000000 digiDownload-1.0.5/digiDownload/__main__.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1703 2023-04-26 17:08:41.000000 digiDownload-1.0.5/digiDownload/cli_tool.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       85 2023-04-26 14:38:53.000000 digiDownload-1.0.5/digiDownload/exceptions.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:22:14.205806 digiDownload-1.0.5/digiDownload.egg-info/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      328 2023-04-26 17:22:14.000000 digiDownload-1.0.5/digiDownload.egg-info/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      424 2023-04-26 17:22:14.000000 digiDownload-1.0.5/digiDownload.egg-info/SOURCES.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-26 17:22:14.000000 digiDownload-1.0.5/digiDownload.egg-info/dependency_links.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       50 2023-04-26 17:22:14.000000 digiDownload-1.0.5/digiDownload.egg-info/requires.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-26 17:22:14.000000 digiDownload-1.0.5/digiDownload.egg-info/top_level.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      102 2023-04-26 17:22:14.205806 digiDownload-1.0.5/setup.cfg
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      557 2023-04-26 17:21:22.000000 digiDownload-1.0.5/setup.py
```

### Comparing `digiDownload-1.0.3/LICENSE` & `digiDownload-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `digiDownload-1.0.3/README.md` & `digiDownload-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `digiDownload-1.0.3/digiDownload/Book.py` & `digiDownload-1.0.5/digiDownload/Book.py`

 * *Files identical despite different names*

### Comparing `digiDownload-1.0.3/digiDownload/LTIParser.py` & `digiDownload-1.0.5/digiDownload/LTIParser.py`

 * *Files identical despite different names*

### Comparing `digiDownload-1.0.3/digiDownload/Session.py` & `digiDownload-1.0.5/digiDownload/Session.py`

 * *Files identical despite different names*

### Comparing `digiDownload-1.0.3/digiDownload/cli_tool.py` & `digiDownload-1.0.5/digiDownload/cli_tool.py`

 * *Files identical despite different names*

