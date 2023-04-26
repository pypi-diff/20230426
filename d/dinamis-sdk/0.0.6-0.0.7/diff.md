# Comparing `tmp/dinamis-sdk-0.0.6.tar.gz` & `tmp/dinamis-sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinamis-sdk-0.0.6.tar", last modified: Tue Apr 25 08:14:17 2023, max compression
+gzip compressed data, was "dinamis-sdk-0.0.7.tar", last modified: Tue Apr 25 17:30:45 2023, max compression
```

## Comparing `dinamis-sdk-0.0.6.tar` & `dinamis-sdk-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:14:17.614159 dinamis-sdk-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2023-02-22 11:50:47.000000 dinamis-sdk-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-25 08:14:17.614159 dinamis-sdk-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-28 12:19:28.000000 dinamis-sdk-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:14:17.610159 dinamis-sdk-0.0.6/dinamis_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.6/dinamis_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8267 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.6/dinamis_sdk/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:14:17.614159 dinamis-sdk-0.0.6/dinamis_sdk/examples/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 13:55:36.000000 dinamis-sdk-0.0.6/dinamis_sdk/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-03-30 18:09:54.000000 dinamis-sdk-0.0.6/dinamis_sdk/examples/pyotb_ndvi_loss.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-03-30 18:09:54.000000 dinamis-sdk-0.0.6/dinamis_sdk/examples/pyotb_toa_mosaic.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-30 14:16:11.000000 dinamis-sdk-0.0.6/dinamis_sdk/examples/rio_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    15621 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.6/dinamis_sdk/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-25 07:42:12.000000 dinamis-sdk-0.0.6/dinamis_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:14:17.614159 dinamis-sdk-0.0.6/dinamis_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-25 08:14:17.000000 dinamis-sdk-0.0.6/dinamis_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-04-25 08:14:17.000000 dinamis-sdk-0.0.6/dinamis_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 08:14:17.000000 dinamis-sdk-0.0.6/dinamis_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 08:14:17.000000 dinamis-sdk-0.0.6/dinamis_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-25 08:14:17.000000 dinamis-sdk-0.0.6/dinamis_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-25 08:14:17.000000 dinamis-sdk-0.0.6/dinamis_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 08:14:17.614159 dinamis-sdk-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-25 08:12:23.000000 dinamis-sdk-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2023-02-22 11:50:47.000000 dinamis-sdk-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-28 12:19:28.000000 dinamis-sdk-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.880950 dinamis-sdk-0.0.7/dinamis_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.7/dinamis_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8267 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.7/dinamis_sdk/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/dinamis_sdk/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 13:55:36.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-03-30 18:09:54.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/pyotb_ndvi_loss.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-03-30 18:09:54.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/pyotb_toa_mosaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-30 14:16:11.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/rio_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    15621 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.7/dinamis_sdk/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-04-25 17:28:43.000000 dinamis-sdk-0.0.7/dinamis_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-25 17:28:43.000000 dinamis-sdk-0.0.7/setup.py
```

### Comparing `dinamis-sdk-0.0.6/LICENSE` & `dinamis-sdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.6/README.md` & `dinamis-sdk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.6/dinamis_sdk/auth.py` & `dinamis-sdk-0.0.7/dinamis_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.6/dinamis_sdk/examples/pyotb_ndvi_loss.py` & `dinamis-sdk-0.0.7/dinamis_sdk/examples/pyotb_ndvi_loss.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.6/dinamis_sdk/examples/pyotb_toa_mosaic.py` & `dinamis-sdk-0.0.7/dinamis_sdk/examples/pyotb_toa_mosaic.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.6/dinamis_sdk/examples/rio_metadata.py` & `dinamis-sdk-0.0.7/dinamis_sdk/examples/rio_metadata.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.6/dinamis_sdk/s3.py` & `dinamis-sdk-0.0.7/dinamis_sdk/s3.py`

 * *Files identical despite different names*

