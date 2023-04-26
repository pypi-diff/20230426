# Comparing `tmp/camerahub_tagger-0.2.0.tar.gz` & `tmp/camerahub_tagger-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.2.0.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.2.1.tar", max compression
```

## Comparing `camerahub_tagger-0.2.0.tar` & `camerahub_tagger-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2839 2023-04-26 13:20:21.793012 camerahub_tagger-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-26 13:20:21.793012 camerahub_tagger-0.2.0/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-26 13:20:21.793012 camerahub_tagger-0.2.0/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2011 2023-04-26 13:20:21.793012 camerahub_tagger-0.2.0/camerahub_tagger/config.py
--rw-r--r--   0        0        0     5572 2023-04-26 13:20:21.793012 camerahub_tagger-0.2.0/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     5468 2023-04-26 13:20:21.793012 camerahub_tagger-0.2.0/camerahub_tagger/main.py
--rw-r--r--   0        0        0      649 2023-04-26 13:20:39.224898 camerahub_tagger-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 camerahub_tagger-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2839 2023-04-26 13:56:22.765117 camerahub_tagger-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 13:56:22.765117 camerahub_tagger-0.2.1/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-26 13:56:22.765117 camerahub_tagger-0.2.1/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2011 2023-04-26 13:56:22.765117 camerahub_tagger-0.2.1/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     5513 2023-04-26 13:56:22.765117 camerahub_tagger-0.2.1/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     5468 2023-04-26 13:56:22.765117 camerahub_tagger-0.2.1/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      649 2023-04-26 13:56:46.348722 camerahub_tagger-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 camerahub_tagger-0.2.1/PKG-INFO
```

### Comparing `camerahub_tagger-0.2.0/README.md` & `camerahub_tagger-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.0/camerahub_tagger/api.py` & `camerahub_tagger-0.2.1/camerahub_tagger/api.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.0/camerahub_tagger/config.py` & `camerahub_tagger-0.2.1/camerahub_tagger/config.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.0/camerahub_tagger/funcs.py` & `camerahub_tagger-0.2.1/camerahub_tagger/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,14 @@
         'FNumber': 'Exif.Photo.FNumber',
         'UserComment': 'Exif.Photo.UserComment',
         'FocalLength': 'Exif.Photo.FocalLength',
         'Flash': 'Exif.Photo.Flash',
         'Artist': 'Exif.Image.Artist',
         'LensSerialNumber': 'Exif.Photo.LensSerialNumber',
         'ExposureTime': 'Exif.Photo.ExposureTime',
-        'MaxApertureValue': 'Exif.Image.MaxApertureValue',
         'Copyright': 'Exif.Image.Copyright',
         'FocalLengthIn35mmFilm': 'Exif.Photo.FocalLengthIn35mmFilm',
         'GPSLatitude': 'Exif.GPSInfo.GPSLatitude',
         'GPSLatitudeRef': 'Exif.GPSInfo.GPSLatitudeRef',
         'GPSLongitude': 'Exif.GPSInfo.GPSLongitude',
         'GPSLongitudeRef': 'Exif.GPSInfo.GPSLongitudeRef',
     }
```

### Comparing `camerahub_tagger-0.2.0/camerahub_tagger/main.py` & `camerahub_tagger-0.2.1/camerahub_tagger/main.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.2.0/pyproject.toml` & `camerahub_tagger-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub-tagger"
-version = "0.2.0"
+version = "0.2.1"
 description = "EXIF tagger for CameraHub"
 authors = ["Jonathan Gazeley <me@jonathangazeley.com>"]
 repository = "https://github.com/camerahub/tagger"
 homepage = "https://camerahub.info/"
 readme = ["README.md"]
 keywords = ["EXIF", "photography", "CameraHub", "metadata"]
```

### Comparing `camerahub_tagger-0.2.0/PKG-INFO` & `camerahub_tagger-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.2.0
+Version: 0.2.1
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

