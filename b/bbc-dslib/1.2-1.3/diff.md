# Comparing `tmp/bbc-dslib-1.2.tar.gz` & `tmp/bbc-dslib-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbc-dslib-1.2.tar", last modified: Mon Nov 29 16:53:54 2021, max compression
+gzip compressed data, was "bbc-dslib-1.3.tar", last modified: Wed Apr 26 08:26:23 2023, max compression
```

## Comparing `bbc-dslib-1.2.tar` & `bbc-dslib-1.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.342812 bbc-dslib-1.2/
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.304901 bbc-dslib-1.2/.github/
--rw-r--r--   0 r.berly    (503) staff       (20)       26 2020-12-10 16:08:21.000000 bbc-dslib-1.2/.github/CODEOWNERS
--rw-r--r--   0 r.berly    (503) staff       (20)      279 2021-04-12 12:47:13.000000 bbc-dslib-1.2/.gitignore
--rw-r--r--   0 r.berly    (503) staff       (20)       13 2020-12-10 16:08:21.000000 bbc-dslib-1.2/MANIFEST.in
--rw-r--r--   0 r.berly    (503) staff       (20)      411 2021-11-29 16:53:54.342255 bbc-dslib-1.2/PKG-INFO
--rw-r--r--   0 r.berly    (503) staff       (20)     3013 2021-11-26 11:05:03.000000 bbc-dslib-1.2/README.md
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.310442 bbc-dslib-1.2/bbc_dslib.egg-info/
--rw-r--r--   0 r.berly    (503) staff       (20)      411 2021-11-29 16:53:53.000000 bbc-dslib-1.2/bbc_dslib.egg-info/PKG-INFO
--rw-r--r--   0 r.berly    (503) staff       (20)      953 2021-11-29 16:53:54.000000 bbc-dslib-1.2/bbc_dslib.egg-info/SOURCES.txt
--rw-r--r--   0 r.berly    (503) staff       (20)        1 2021-11-29 16:53:53.000000 bbc-dslib-1.2/bbc_dslib.egg-info/dependency_links.txt
--rw-r--r--   0 r.berly    (503) staff       (20)      495 2021-11-29 16:53:53.000000 bbc-dslib-1.2/bbc_dslib.egg-info/requires.txt
--rw-r--r--   0 r.berly    (503) staff       (20)        6 2021-11-29 16:53:53.000000 bbc-dslib-1.2/bbc_dslib.egg-info/top_level.txt
--rw-r--r--   0 r.berly    (503) staff       (20)      472 2021-04-12 12:53:19.000000 bbc-dslib-1.2/create_git_tag.py
--rwxr-xr-x   0 r.berly    (503) staff       (20)      106 2021-11-26 11:04:55.000000 bbc-dslib-1.2/deploy.sh
--rw-r--r--   0 r.berly    (503) staff       (20)       30 2020-12-10 16:08:21.000000 bbc-dslib-1.2/deployment-requirements.txt
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.311585 bbc-dslib-1.2/dslib/
--rw-r--r--   0 r.berly    (503) staff       (20)        0 2020-06-26 15:56:55.000000 bbc-dslib-1.2/dslib/__init__.py
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.313638 bbc-dslib-1.2/dslib/database/
--rw-r--r--   0 r.berly    (503) staff       (20)       68 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/database/__init__.py
--rw-r--r--   0 r.berly    (503) staff       (20)     8233 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/database/_database.py
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.316515 bbc-dslib-1.2/dslib/facebook/
--rw-r--r--   0 r.berly    (503) staff       (20)       34 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/facebook/__init__.py
--rw-r--r--   0 r.berly    (503) staff       (20)     1560 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/facebook/_prophet.py
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.321686 bbc-dslib-1.2/dslib/google/
--rw-r--r--   0 r.berly    (503) staff       (20)      193 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/google/__init__.py
--rw-r--r--   0 r.berly    (503) staff       (20)    14538 2021-11-25 16:26:22.000000 bbc-dslib-1.2/dslib/google/_bigquery.py
--rw-r--r--   0 r.berly    (503) staff       (20)     7366 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/google/_drive.py
--rw-r--r--   0 r.berly    (503) staff       (20)     8884 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/google/_spreadsheet.py
--rw-r--r--   0 r.berly    (503) staff       (20)     6371 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/google/_storage.py
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.324988 bbc-dslib-1.2/dslib/science/
--rw-r--r--   0 r.berly    (503) staff       (20)      168 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/science/__init__.py
--rw-r--r--   0 r.berly    (503) staff       (20)      474 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/science/_pandas.py
--rw-r--r--   0 r.berly    (503) staff       (20)     4941 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/science/_sklearn.py
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.332458 bbc-dslib-1.2/dslib/utils/
--rw-r--r--   0 r.berly    (503) staff       (20)      468 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/utils/__init__.py
--rw-r--r--   0 r.berly    (503) staff       (20)     1405 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/utils/_caching.py
--rw-r--r--   0 r.berly    (503) staff       (20)     5007 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/utils/_io.py
--rw-r--r--   0 r.berly    (503) staff       (20)     4255 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/utils/_logging.py
--rw-r--r--   0 r.berly    (503) staff       (20)     1145 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/utils/_meta.py
--rw-r--r--   0 r.berly    (503) staff       (20)     1395 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/utils/_templating.py
--rw-r--r--   0 r.berly    (503) staff       (20)     2311 2021-04-12 12:47:13.000000 bbc-dslib-1.2/dslib/utils/_temporality.py
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.333652 bbc-dslib-1.2/img/
--rw-r--r--   0 r.berly    (503) staff       (20)    64001 2019-08-01 13:28:00.000000 bbc-dslib-1.2/img/git_flow.png
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.336054 bbc-dslib-1.2/scripts/
--rw-r--r--   0 r.berly    (503) staff       (20)     1846 2021-04-12 12:47:13.000000 bbc-dslib-1.2/scripts/export_to_gcs.py
--rw-r--r--   0 r.berly    (503) staff       (20)     1636 2021-04-12 12:47:13.000000 bbc-dslib-1.2/scripts/import_from_gcs.py
--rw-r--r--   0 r.berly    (503) staff       (20)       38 2021-11-29 16:53:54.342981 bbc-dslib-1.2/setup.cfg
--rw-r--r--   0 r.berly    (503) staff       (20)     1391 2021-11-29 10:35:45.000000 bbc-dslib-1.2/setup.py
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.338111 bbc-dslib-1.2/tests/
--rw-r--r--   0 r.berly    (503) staff       (20)      854 2021-04-12 12:47:13.000000 bbc-dslib-1.2/tests/README.md
-drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2021-11-29 16:53:54.340844 bbc-dslib-1.2/tests/google/
--rw-r--r--   0 r.berly    (503) staff       (20)      791 2021-04-12 12:47:13.000000 bbc-dslib-1.2/tests/google/conftest.py
--rw-r--r--   0 r.berly    (503) staff       (20)    18671 2021-04-12 12:47:13.000000 bbc-dslib-1.2/tests/google/test_bigquery.py
--rw-r--r--   0 r.berly    (503) staff       (20)    15681 2021-04-12 09:49:31.000000 bbc-dslib-1.2/tests/test_bigquery.py
--rw-r--r--   0 r.berly    (503) staff       (20)       20 2021-11-29 10:35:45.000000 bbc-dslib-1.2/version.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.479763 bbc-dslib-1.3/
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.472934 bbc-dslib-1.3/.github/
+-rw-r--r--   0 r.berly    (503) staff       (20)       26 2020-12-10 16:08:21.000000 bbc-dslib-1.3/.github/CODEOWNERS
+-rw-r--r--   0 r.berly    (503) staff       (20)      279 2021-04-12 12:47:13.000000 bbc-dslib-1.3/.gitignore
+-rw-r--r--   0 r.berly    (503) staff       (20)       13 2020-12-10 16:08:21.000000 bbc-dslib-1.3/MANIFEST.in
+-rw-r--r--   0 r.berly    (503) staff       (20)      383 2023-04-26 08:26:23.479603 bbc-dslib-1.3/PKG-INFO
+-rw-r--r--   0 r.berly    (503) staff       (20)     3013 2021-11-26 11:05:03.000000 bbc-dslib-1.3/README.md
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.473755 bbc-dslib-1.3/bbc_dslib.egg-info/
+-rw-r--r--   0 r.berly    (503) staff       (20)      383 2023-04-26 08:26:23.000000 bbc-dslib-1.3/bbc_dslib.egg-info/PKG-INFO
+-rw-r--r--   0 r.berly    (503) staff       (20)      953 2023-04-26 08:26:23.000000 bbc-dslib-1.3/bbc_dslib.egg-info/SOURCES.txt
+-rw-r--r--   0 r.berly    (503) staff       (20)        1 2023-04-26 08:26:23.000000 bbc-dslib-1.3/bbc_dslib.egg-info/dependency_links.txt
+-rw-r--r--   0 r.berly    (503) staff       (20)      494 2023-04-26 08:26:23.000000 bbc-dslib-1.3/bbc_dslib.egg-info/requires.txt
+-rw-r--r--   0 r.berly    (503) staff       (20)        6 2023-04-26 08:26:23.000000 bbc-dslib-1.3/bbc_dslib.egg-info/top_level.txt
+-rw-r--r--   0 r.berly    (503) staff       (20)      472 2021-04-12 12:53:19.000000 bbc-dslib-1.3/create_git_tag.py
+-rwxr-xr-x   0 r.berly    (503) staff       (20)      106 2021-11-26 11:04:55.000000 bbc-dslib-1.3/deploy.sh
+-rw-r--r--   0 r.berly    (503) staff       (20)       30 2020-12-10 16:08:21.000000 bbc-dslib-1.3/deployment-requirements.txt
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.473907 bbc-dslib-1.3/dslib/
+-rw-r--r--   0 r.berly    (503) staff       (20)        0 2020-06-26 15:56:55.000000 bbc-dslib-1.3/dslib/__init__.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.474199 bbc-dslib-1.3/dslib/database/
+-rw-r--r--   0 r.berly    (503) staff       (20)       68 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/database/__init__.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     8233 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/database/_database.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.474581 bbc-dslib-1.3/dslib/facebook/
+-rw-r--r--   0 r.berly    (503) staff       (20)       34 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/facebook/__init__.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     1560 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/facebook/_prophet.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.475575 bbc-dslib-1.3/dslib/google/
+-rw-r--r--   0 r.berly    (503) staff       (20)      193 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/google/__init__.py
+-rw-r--r--   0 r.berly    (503) staff       (20)    14538 2021-11-25 16:26:22.000000 bbc-dslib-1.3/dslib/google/_bigquery.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     7366 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/google/_drive.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     8884 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/google/_spreadsheet.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     6371 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/google/_storage.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.476078 bbc-dslib-1.3/dslib/science/
+-rw-r--r--   0 r.berly    (503) staff       (20)      168 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/science/__init__.py
+-rw-r--r--   0 r.berly    (503) staff       (20)      474 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/science/_pandas.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     4941 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/science/_sklearn.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.477570 bbc-dslib-1.3/dslib/utils/
+-rw-r--r--   0 r.berly    (503) staff       (20)      468 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/utils/__init__.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     1405 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/utils/_caching.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     5007 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/utils/_io.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     4255 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/utils/_logging.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     1145 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/utils/_meta.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     1395 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/utils/_templating.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     2311 2021-04-12 12:47:13.000000 bbc-dslib-1.3/dslib/utils/_temporality.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.477808 bbc-dslib-1.3/img/
+-rw-r--r--   0 r.berly    (503) staff       (20)    64001 2019-08-01 13:28:00.000000 bbc-dslib-1.3/img/git_flow.png
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.478380 bbc-dslib-1.3/scripts/
+-rw-r--r--   0 r.berly    (503) staff       (20)     1846 2021-04-12 12:47:13.000000 bbc-dslib-1.3/scripts/export_to_gcs.py
+-rw-r--r--   0 r.berly    (503) staff       (20)     1636 2021-04-12 12:47:13.000000 bbc-dslib-1.3/scripts/import_from_gcs.py
+-rw-r--r--   0 r.berly    (503) staff       (20)       38 2023-04-26 08:26:23.479811 bbc-dslib-1.3/setup.cfg
+-rw-r--r--   0 r.berly    (503) staff       (20)     1390 2023-04-25 15:46:40.000000 bbc-dslib-1.3/setup.py
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.478776 bbc-dslib-1.3/tests/
+-rw-r--r--   0 r.berly    (503) staff       (20)      854 2021-04-12 12:47:13.000000 bbc-dslib-1.3/tests/README.md
+drwxr-xr-x   0 r.berly    (503) staff       (20)        0 2023-04-26 08:26:23.479290 bbc-dslib-1.3/tests/google/
+-rw-r--r--   0 r.berly    (503) staff       (20)      787 2023-04-25 15:46:40.000000 bbc-dslib-1.3/tests/google/conftest.py
+-rw-r--r--   0 r.berly    (503) staff       (20)    18671 2021-04-12 12:47:13.000000 bbc-dslib-1.3/tests/google/test_bigquery.py
+-rw-r--r--   0 r.berly    (503) staff       (20)    15601 2023-04-25 15:46:40.000000 bbc-dslib-1.3/tests/test_bigquery.py
+-rw-r--r--   0 r.berly    (503) staff       (20)       20 2023-04-25 15:46:40.000000 bbc-dslib-1.3/version.py
```

### Comparing `bbc-dslib-1.2/README.md` & `bbc-dslib-1.3/README.md`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/bbc_dslib.egg-info/SOURCES.txt` & `bbc-dslib-1.3/bbc_dslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/database/_database.py` & `bbc-dslib-1.3/dslib/database/_database.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/facebook/_prophet.py` & `bbc-dslib-1.3/dslib/facebook/_prophet.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/google/_bigquery.py` & `bbc-dslib-1.3/dslib/google/_bigquery.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/google/_drive.py` & `bbc-dslib-1.3/dslib/google/_drive.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/google/_spreadsheet.py` & `bbc-dslib-1.3/dslib/google/_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/google/_storage.py` & `bbc-dslib-1.3/dslib/google/_storage.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/science/_sklearn.py` & `bbc-dslib-1.3/dslib/science/_sklearn.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/utils/_caching.py` & `bbc-dslib-1.3/dslib/utils/_caching.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/utils/_io.py` & `bbc-dslib-1.3/dslib/utils/_io.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/utils/_logging.py` & `bbc-dslib-1.3/dslib/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/utils/_meta.py` & `bbc-dslib-1.3/dslib/utils/_meta.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/utils/_templating.py` & `bbc-dslib-1.3/dslib/utils/_templating.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/dslib/utils/_temporality.py` & `bbc-dslib-1.3/dslib/utils/_temporality.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/img/git_flow.png` & `bbc-dslib-1.3/img/git_flow.png`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/scripts/export_to_gcs.py` & `bbc-dslib-1.3/scripts/export_to_gcs.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/scripts/import_from_gcs.py` & `bbc-dslib-1.3/scripts/import_from_gcs.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/setup.py` & `bbc-dslib-1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,28 +19,28 @@
     packages=setuptools.find_packages(),
     python_requires='>=3.7.9',
     install_requires=['humanfriendly', 'pyyaml', 'jinja2'],
     extras_require={
         'database': ['sqlalchemy', 'psycopg2-binary', 'PyMySQL', 'pandas'],
         'facebook': ['fbprophet'],
         'google': [
-            'google-cloud-bigquery==2.30.1',
-            'google-cloud-bigquery-storage==2.10.1',
-            'google-cloud-storage==1.43.0',
-            'google-api-python-client==2.31.0',
+            'google-cloud-bigquery==3.10.0',
+            'google-cloud-bigquery-storage==2.19.1',
+            'google-cloud-storage==2.8.0',
+            'google-api-python-client==2.86.0',
             'oauth2client==4.1.3',
-            'pandas==1.3.4',
-            'pandas-gbq==0.16.0',
-            'tqdm==4.62.3',
-            'gspread==4.0.1',
-            'gspread-dataframe==3.2.1'
+            'pandas==2.0.1',
+            'pandas-gbq==0.19.1',
+            'tqdm==4.65.0',
+            'gspread==5.8.0',
+            'gspread-dataframe==3.3.0'
         ],
         'science': [
-            'scikit-learn==1.0.1',
-            'numpy==1.21.4',
-            'matplotlib==3.5.0',
-            'dill==0.3.4',
-            'pandas==1.3.4'
+            'scikit-learn==1.2.2',
+            'numpy==1.24.3',
+            'matplotlib==3.7.1',
+            'dill==0.3.6',
+            'pandas==2.0.1'
         ],
         'testing': ['pytest', 'pytest-cov', 'coverage', 'mock', 'testfixtures'],
     }
 )
```

### Comparing `bbc-dslib-1.2/tests/README.md` & `bbc-dslib-1.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/tests/google/conftest.py` & `bbc-dslib-1.3/tests/google/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from contextlib import contextmanager
 from os import path
 
 import pytest
 from google.cloud import storage
 
-PROJECT_ID = 'bbc-data-marketplace'
+PROJECT_ID = 'data-science-360fc06f'
 TEMP_DATASET = 'temp_1day'
-TEMP_BUCKET = 'bbc-data-marketplace-temp1day'
+TEMP_BUCKET = 'data_science_temp_30days'
 
 
 @pytest.fixture(scope='module')
 def storage_client():
     return storage.Client(PROJECT_ID)
```

### Comparing `bbc-dslib-1.2/tests/google/test_bigquery.py` & `bbc-dslib-1.3/tests/google/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `bbc-dslib-1.2/tests/test_bigquery.py` & `bbc-dslib-1.3/tests/test_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from google.api_core.exceptions import NotFound
 from google.cloud import bigquery, storage
 from google.cloud.bigquery_storage import BigQueryReadClient
 from pandas_gbq.gbq import TableCreationError
 from testfixtures import LogCapture
 
 from dslib.utils import get_tmp_dirpath
-from dslib.wrappers.google.bigquery import BigQueryWrapper, BigQueryError
+from dslib.google import BigQueryWrapper, BigQueryError
 
 
 # HELPERS ##############################################################################################################
 
-PROJECT_ID = 'bbc-data-marketplace'
+PROJECT_ID = 'data-science-360fc06f'
 TEMP_DATASET = 'temp_1day'
-TEMP_BUCKET = 'bbc-data-marketplace-temp1day'
+TEMP_BUCKET = 'data_science_temp_30days'
 
 
 def generate_temp_table_ref():
     return f'{TEMP_DATASET}.test_dslib_{str(uuid4())[-10:]}'
 
 
 def generate_temp_file_ref():
@@ -140,15 +140,15 @@
 
     def test_invalid(self, bq):
         assert bq.assess_query('SELECT count(*) FROM') is False
 
     def test_valid(self, bq, temp_table_ref):
         with LogCapture(level=logging.INFO) as logs:
             assert bq.assess_query(f'SELECT count(*) FROM {temp_table_ref}') is True
-        logs.check_present(('dslib.wrappers.google.bigquery', 'INFO', 'Query is valid. It would process 0 bytes'))
+        logs.check_present(('dslib.google._bigquery', 'INFO', 'Query is valid. It would process 0 bytes'))
 
 
 class TestRunQuery:
 
     def test_invalid(self, bq):
         with pytest.raises(BigQueryError):
             bq.run_query('SELECT count(*) FROM')
@@ -170,20 +170,20 @@
 
     def test_no_cache(self, bq, temp_table_ref):
         # Run it a first time to have it in the cache
         bq.run_query(f'SELECT * FROM {temp_table_ref}', output_type=None)
         # Check with that cache is used with use_query_cache = True
         with LogCapture(level=logging.INFO) as logs:
             bq.run_query(f'SELECT * FROM {temp_table_ref}', output_type=None, use_query_cache=True)
-        logs.check_present(('dslib.wrappers.google.bigquery', 'INFO', 'Query processed: 0 bytes'))
+        logs.check_present(('dslib.google._bigquery', 'INFO', 'Query processed: 0 bytes'))
         # Check with that cache is not used with use_query_cache = False
         with LogCapture(level=logging.INFO) as logs:
             bq.run_query(f'SELECT * FROM {temp_table_ref}', output_type=None, use_query_cache=False)
-        with pytest.raises(AssertionError, match='sequence not as expected'):
-            logs.check_present(('dslib.wrappers.google.bigquery', 'INFO', 'Query processed: 0 bytes'))
+        with pytest.raises(AssertionError):
+            logs.check_present(('dslib.google._bigquery', 'INFO', 'Query processed: 0 bytes'))
 
     def test_add_tags(self, bq, temp_table_ref):
         query = f'SELECT * FROM {temp_table_ref};'
         queue = Queue()
 
         def mock_start_query(query, *args, **kwargs):
             queue.put(query)
```

