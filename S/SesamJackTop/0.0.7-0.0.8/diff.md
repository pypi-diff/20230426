# Comparing `tmp/SesamJackTop-0.0.7.tar.gz` & `tmp/SesamJackTop-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SesamJackTop-0.0.7.tar", last modified: Wed Apr 26 10:13:07 2023, max compression
+gzip compressed data, was "SesamJackTop-0.0.8.tar", last modified: Wed Apr 26 10:24:12 2023, max compression
```

## Comparing `SesamJackTop-0.0.7.tar` & `SesamJackTop-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:13:07.215656 SesamJackTop-0.0.7/
--rw-rw-rw-   0        0        0     1089 2020-07-24 11:14:00.000000 SesamJackTop-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2020-07-24 11:12:48.000000 SesamJackTop-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      493 2023-04-26 10:13:07.212661 SesamJackTop-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       98 2022-12-07 13:54:16.000000 SesamJackTop-0.0.7/README.txt
--rw-rw-rw-   0        0        0      477 2023-04-26 10:12:05.000000 SesamJackTop-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 10:13:07.216651 SesamJackTop-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 10:13:07.076028 SesamJackTop-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 10:13:07.136868 SesamJackTop-0.0.7/src/SesamJackTop/
--rw-rw-rw-   0        0        0        0 2022-12-07 13:34:46.000000 SesamJackTop-0.0.7/src/SesamJackTop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:13:07.204687 SesamJackTop-0.0.7/src/SesamJackTop/geniEImporter/
--rw-rw-rw-   0        0        0       79 2022-12-08 10:56:44.000000 SesamJackTop-0.0.7/src/SesamJackTop/geniEImporter/enviroment.py
--rw-rw-rw-   0        0        0       87 2022-12-08 10:23:23.000000 SesamJackTop-0.0.7/src/SesamJackTop/sesam.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:13:07.186732 SesamJackTop-0.0.7/src/SesamJackTop.egg-info/
--rw-rw-rw-   0        0        0      493 2023-04-26 10:13:07.000000 SesamJackTop-0.0.7/src/SesamJackTop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-04-26 10:13:07.000000 SesamJackTop-0.0.7/src/SesamJackTop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:13:07.000000 SesamJackTop-0.0.7/src/SesamJackTop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-26 10:13:07.000000 SesamJackTop-0.0.7/src/SesamJackTop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 10:24:12.018180 SesamJackTop-0.0.8/
+-rw-rw-rw-   0        0        0     1089 2020-07-24 11:14:00.000000 SesamJackTop-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2020-07-24 11:12:48.000000 SesamJackTop-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      493 2023-04-26 10:24:12.016185 SesamJackTop-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2022-12-07 13:54:16.000000 SesamJackTop-0.0.8/README.txt
+-rw-rw-rw-   0        0        0      477 2023-04-26 10:21:17.000000 SesamJackTop-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 10:24:12.019178 SesamJackTop-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 10:24:11.937401 SesamJackTop-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 10:24:11.980282 SesamJackTop-0.0.8/src/SesamJackTop/
+-rw-rw-rw-   0        0        0        0 2022-12-07 13:34:46.000000 SesamJackTop-0.0.8/src/SesamJackTop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:24:12.011197 SesamJackTop-0.0.8/src/SesamJackTop/geniEImporter/
+-rw-rw-rw-   0        0        0       79 2022-12-08 10:56:44.000000 SesamJackTop-0.0.8/src/SesamJackTop/geniEImporter/enviroment.py
+-rw-rw-rw-   0        0        0       87 2022-12-08 10:23:23.000000 SesamJackTop-0.0.8/src/SesamJackTop/sesam.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:24:12.005215 SesamJackTop-0.0.8/src/SesamJackTop.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-04-26 10:24:11.000000 SesamJackTop-0.0.8/src/SesamJackTop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-04-26 10:24:11.000000 SesamJackTop-0.0.8/src/SesamJackTop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 10:24:11.000000 SesamJackTop-0.0.8/src/SesamJackTop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-26 10:24:11.000000 SesamJackTop-0.0.8/src/SesamJackTop.egg-info/top_level.txt
```

### Comparing `SesamJackTop-0.0.7/LICENSE.txt` & `SesamJackTop-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

