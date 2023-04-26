# Comparing `tmp/liitos-2023.2.7.tar.gz` & `tmp/liitos-2023.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liitos-2023.2.7.tar", last modified: Mon Feb  6 19:33:53 2023, max compression
+gzip compressed data, was "liitos-2023.2.8.tar", last modified: Tue Feb  7 23:01:04 2023, max compression
```

## Comparing `liitos-2023.2.7.tar` & `liitos-2023.2.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-06 19:33:53.372360 liitos-2023.2.7/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.2.7/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.2.7/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2540 2023-02-06 19:33:53.372112 liitos-2023.2.7/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1623 2023-01-22 12:34:33.000000 liitos-2023.2.7/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-06 19:33:53.257743 liitos-2023.2.7/liitos/
--rw-r--r--   0 ruth       (501) staff       (20)     5044 2023-02-06 19:31:14.000000 liitos-2023.2.7/liitos/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.2.7/liitos/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3875 2023-02-04 14:18:21.000000 liitos-2023.2.7/liitos/approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1624 2022-12-09 18:23:12.000000 liitos-2023.2.7/liitos/captions.py
--rw-r--r--   0 ruth       (501) staff       (20)     4295 2023-02-04 14:18:21.000000 liitos-2023.2.7/liitos/changes.py
--rw-r--r--   0 ruth       (501) staff       (20)    10259 2023-02-06 19:27:14.000000 liitos-2023.2.7/liitos/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    31810 2023-02-04 14:18:21.000000 liitos-2023.2.7/liitos/concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.2.7/liitos/configure.py
--rw-r--r--   0 ruth       (501) staff       (20)     1780 2023-01-29 18:11:25.000000 liitos-2023.2.7/liitos/description_lists.py
--rw-r--r--   0 ruth       (501) staff       (20)     1958 2023-01-02 19:41:38.000000 liitos-2023.2.7/liitos/eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     1650 2022-12-06 19:43:32.000000 liitos-2023.2.7/liitos/figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    11799 2023-01-21 21:35:47.000000 liitos-2023.2.7/liitos/gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     3896 2022-12-09 18:24:04.000000 liitos-2023.2.7/liitos/labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.2.7/liitos/liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    41648 2023-02-04 14:18:21.000000 liitos-2023.2.7/liitos/meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.2.7/liitos/patch.py
--rw-r--r--   0 ruth       (501) staff       (20)    15890 2023-02-06 19:25:05.000000 liitos-2023.2.7/liitos/render.py
--rw-r--r--   0 ruth       (501) staff       (20)    12596 2023-02-01 20:20:42.000000 liitos-2023.2.7/liitos/tables.py
--rw-r--r--   0 ruth       (501) staff       (20)     1489 2023-01-02 19:38:06.000000 liitos-2023.2.7/liitos/template_loader.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-06 19:33:53.276722 liitos-2023.2.7/liitos/templates/
--rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.2.7/liitos/templates/approvals.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1198 2023-01-17 20:23:10.000000 liitos-2023.2.7/liitos/templates/bookmatter.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.2.7/liitos/templates/changes.yml
--rw-r--r--   0 ruth       (501) staff       (20)      853 2022-11-29 20:13:39.000000 liitos-2023.2.7/liitos/templates/driver.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)       97 2022-12-05 14:36:30.000000 liitos-2023.2.7/liitos/templates/meta-patch.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1448 2023-01-17 20:30:00.000000 liitos-2023.2.7/liitos/templates/meta.yml
--rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.2.7/liitos/templates/metadata.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.2.7/liitos/templates/mkdocs.yml.in
--rw-r--r--   0 ruth       (501) staff       (20)     1106 2022-12-04 13:44:55.000000 liitos-2023.2.7/liitos/templates/publisher.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     9614 2023-02-01 20:13:41.000000 liitos-2023.2.7/liitos/templates/setup.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.2.7/liitos/templates/vocabulary.yml
--rw-r--r--   0 ruth       (501) staff       (20)     7417 2023-02-06 18:39:24.000000 liitos-2023.2.7/liitos/tools.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-06 19:33:53.259324 liitos-2023.2.7/liitos.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2540 2023-02-06 19:33:53.000000 liitos-2023.2.7/liitos.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1264 2023-02-06 19:33:53.000000 liitos-2023.2.7/liitos.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-02-06 19:33:53.000000 liitos-2023.2.7/liitos.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       42 2023-02-06 19:33:53.000000 liitos-2023.2.7/liitos.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      179 2023-02-06 19:33:53.000000 liitos-2023.2.7/liitos.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       15 2023-02-06 19:33:53.000000 liitos-2023.2.7/liitos.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2645 2023-02-06 19:11:11.000000 liitos-2023.2.7/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-02-06 19:33:53.372423 liitos-2023.2.7/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-06 19:33:53.371663 liitos-2023.2.7/test/
--rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.2.7/test/test_approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1587 2022-12-05 16:52:23.000000 liitos-2023.2.7/test/test_captions.py
--rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.2.7/test/test_changes.py
--rw-r--r--   0 ruth       (501) staff       (20)     3720 2023-02-04 14:19:55.000000 liitos-2023.2.7/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.2.7/test/test_concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.2.7/test/test_eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.2.7/test/test_figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    10449 2022-11-02 19:26:27.000000 liitos-2023.2.7/test/test_gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.2.7/test/test_labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.2.7/test/test_liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.2.7/test/test_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.2.7/test/test_patch.py
--rw-r--r--   0 ruth       (501) staff       (20)      486 2023-01-31 21:27:46.000000 liitos-2023.2.7/test/test_render.py
--rw-r--r--   0 ruth       (501) staff       (20)      883 2022-12-09 17:00:56.000000 liitos-2023.2.7/test/test_tables.py
--rw-r--r--   0 ruth       (501) staff       (20)      431 2022-12-06 20:22:36.000000 liitos-2023.2.7/test/test_template_loader.py
--rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.2.7/test/test_tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.955176 liitos-2023.2.8/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.2.8/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.2.8/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     2540 2023-02-07 23:01:04.955014 liitos-2023.2.8/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1623 2023-01-22 12:34:33.000000 liitos-2023.2.8/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.930702 liitos-2023.2.8/liitos/
+-rw-r--r--   0 ruth       (501) staff       (20)     5044 2023-02-07 22:59:13.000000 liitos-2023.2.8/liitos/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.2.8/liitos/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3875 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1787 2023-02-07 22:52:39.000000 liitos-2023.2.8/liitos/captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4295 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10260 2023-02-07 22:48:13.000000 liitos-2023.2.8/liitos/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    31810 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.2.8/liitos/configure.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1780 2023-01-29 18:11:25.000000 liitos-2023.2.8/liitos/description_lists.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1958 2023-01-02 19:41:38.000000 liitos-2023.2.8/liitos/eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1650 2022-12-06 19:43:32.000000 liitos-2023.2.8/liitos/figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11799 2023-01-21 21:35:47.000000 liitos-2023.2.8/liitos/gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3896 2022-12-09 18:24:04.000000 liitos-2023.2.8/liitos/labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.2.8/liitos/liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    41648 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.2.8/liitos/patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)    15890 2023-02-06 19:25:05.000000 liitos-2023.2.8/liitos/render.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12596 2023-02-01 20:20:42.000000 liitos-2023.2.8/liitos/tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1489 2023-01-02 19:38:06.000000 liitos-2023.2.8/liitos/template_loader.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.938453 liitos-2023.2.8/liitos/templates/
+-rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.2.8/liitos/templates/approvals.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1198 2023-01-17 20:23:10.000000 liitos-2023.2.8/liitos/templates/bookmatter.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.2.8/liitos/templates/changes.yml
+-rw-r--r--   0 ruth       (501) staff       (20)      853 2022-11-29 20:13:39.000000 liitos-2023.2.8/liitos/templates/driver.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)       97 2022-12-05 14:36:30.000000 liitos-2023.2.8/liitos/templates/meta-patch.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1448 2023-01-17 20:30:00.000000 liitos-2023.2.8/liitos/templates/meta.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.2.8/liitos/templates/metadata.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.2.8/liitos/templates/mkdocs.yml.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1106 2022-12-04 13:44:55.000000 liitos-2023.2.8/liitos/templates/publisher.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     9614 2023-02-01 20:13:41.000000 liitos-2023.2.8/liitos/templates/setup.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.2.8/liitos/templates/vocabulary.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     7417 2023-02-06 18:39:24.000000 liitos-2023.2.8/liitos/tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.933173 liitos-2023.2.8/liitos.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     2540 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1264 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      179 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       15 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2645 2023-02-07 22:44:17.000000 liitos-2023.2.8/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-02-07 23:01:04.955215 liitos-2023.2.8/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.954700 liitos-2023.2.8/test/
+-rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.2.8/test/test_approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.2.8/test/test_captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.2.8/test/test_changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3720 2023-02-04 14:19:55.000000 liitos-2023.2.8/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.2.8/test/test_concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.2.8/test/test_eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.2.8/test/test_figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10449 2022-11-02 19:26:27.000000 liitos-2023.2.8/test/test_gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.2.8/test/test_labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.2.8/test/test_liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.2.8/test/test_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.2.8/test/test_patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)      486 2023-01-31 21:27:46.000000 liitos-2023.2.8/test/test_render.py
+-rw-r--r--   0 ruth       (501) staff       (20)      883 2022-12-09 17:00:56.000000 liitos-2023.2.8/test/test_tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)      431 2022-12-06 20:22:36.000000 liitos-2023.2.8/test/test_template_loader.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.2.8/test/test_tools.py
```

### Comparing `liitos-2023.2.7/LICENSE` & `liitos-2023.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/PKG-INFO` & `liitos-2023.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.2.7
+Version: 2023.2.8
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
```

### Comparing `liitos-2023.2.7/README.md` & `liitos-2023.2.8/README.md`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/__init__.py` & `liitos-2023.2.8/liitos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import os
 import pathlib
 import shellingham  # type: ignore
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.2.7+parent.4f01d7b3'
-# [[[end]]] (checksum: 532593e3f30a4a904e6ed4486e271f7e)
+__version__ = '2023.2.8+parent.b08058c7'
+# [[[end]]] (checksum: 66a50e360bdddcd6850848c3808a189f)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Splice (Finnish liitos) contributions.'
 APP_ALIAS = 'liitos'
 APP_ENV = 'LIITOS'
```

### Comparing `liitos-2023.2.7/liitos/approvals.py` & `liitos-2023.2.8/liitos/approvals.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/captions.py` & `liitos-2023.2.8/liitos/captions.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,17 +24,21 @@
                 log.info(f'- found the caption start at line #{slot + 1}')
                 caption.append(line)
                 if not line.strip().endswith(r'}\tabularnewline'):
                     log.info(f'- multi line caption at line #{slot + 1}')
                     modus = 'caption'
             elif line.startswith(r'\end{longtable}'):
                 log.info(f'end of table env detected at line #{slot + 1}')
-                outgoing.extend(table)
-                outgoing.append(r'\rowcolor{white}')
-                outgoing.extend(caption)
+                for stmt in table:
+                    if not stmt.startswith(r'\endlastfoot'):
+                        outgoing.append(stmt)
+                        continue
+                    else:
+                        outgoing.extend(caption)
+                        outgoing.append(stmt)
                 outgoing.append(line)
                 modus = 'copy'
             else:
                 log.debug('- table continues')
                 table.append(line)
 
         elif modus == 'caption':
```

### Comparing `liitos-2023.2.7/liitos/changes.py` & `liitos-2023.2.8/liitos/changes.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/cli.py` & `liitos-2023.2.8/liitos/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
         acted = 'Did not render'
         code = 0  # HACK A DID ACK
     log.info(f'{acted} {target} document for {facet} at {doc} in {duration_secs} secs')
     return sys.exit(code)
 
 
 @app.command('report')
-def eject() -> int:
+def report() -> int:
     """
     Report on the environment.
     """
     log.info(LOG_SEPARATOR)
     log.info('inspecting environment (tool version information):')
     for tool_key in TOOL_VERSION_COMMAND_MAP:
         too.report(tool_key)
```

### Comparing `liitos-2023.2.7/liitos/concat.py` & `liitos-2023.2.8/liitos/concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/configure.py` & `liitos-2023.2.8/liitos/configure.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/description_lists.py` & `liitos-2023.2.8/liitos/description_lists.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/eject.py` & `liitos-2023.2.8/liitos/eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/figures.py` & `liitos-2023.2.8/liitos/figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/gather.py` & `liitos-2023.2.8/liitos/gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/labels.py` & `liitos-2023.2.8/liitos/labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/meta.py` & `liitos-2023.2.8/liitos/meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/patch.py` & `liitos-2023.2.8/liitos/patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/render.py` & `liitos-2023.2.8/liitos/render.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/tables.py` & `liitos-2023.2.8/liitos/tables.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/template_loader.py` & `liitos-2023.2.8/liitos/template_loader.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/bookmatter.tex.in` & `liitos-2023.2.8/liitos/templates/bookmatter.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/driver.tex.in` & `liitos-2023.2.8/liitos/templates/driver.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/meta.yml` & `liitos-2023.2.8/liitos/templates/meta.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/metadata.tex.in` & `liitos-2023.2.8/liitos/templates/metadata.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/mkdocs.yml.in` & `liitos-2023.2.8/liitos/templates/mkdocs.yml.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/publisher.tex.in` & `liitos-2023.2.8/liitos/templates/publisher.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/setup.tex.in` & `liitos-2023.2.8/liitos/templates/setup.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/templates/vocabulary.yml` & `liitos-2023.2.8/liitos/templates/vocabulary.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos/tools.py` & `liitos-2023.2.8/liitos/tools.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/liitos.egg-info/PKG-INFO` & `liitos-2023.2.8/liitos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.2.7
+Version: 2023.2.8
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
```

### Comparing `liitos-2023.2.7/liitos.egg-info/SOURCES.txt` & `liitos-2023.2.8/liitos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/pyproject.toml` & `liitos-2023.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "liitos"
-version = "2023.2.7"
+version = "2023.2.8"
 description = "Splice (Finnish liitos) contributions."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `liitos-2023.2.7/test/test_cli.py` & `liitos-2023.2.8/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_concat.py` & `liitos-2023.2.8/test/test_concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_eject.py` & `liitos-2023.2.8/test/test_eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_figures.py` & `liitos-2023.2.8/test/test_figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_gather.py` & `liitos-2023.2.8/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_labels.py` & `liitos-2023.2.8/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_meta.py` & `liitos-2023.2.8/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_patch.py` & `liitos-2023.2.8/test/test_patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_tables.py` & `liitos-2023.2.8/test/test_tables.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.7/test/test_tools.py` & `liitos-2023.2.8/test/test_tools.py`

 * *Files identical despite different names*

