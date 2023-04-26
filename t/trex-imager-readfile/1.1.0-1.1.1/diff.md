# Comparing `tmp/trex_imager_readfile-1.1.0.tar.gz` & `tmp/trex_imager_readfile-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex_imager_readfile-1.1.0.tar", max compression
+gzip compressed data, was "trex_imager_readfile-1.1.1.tar", max compression
```

## Comparing `trex_imager_readfile-1.1.0.tar` & `trex_imager_readfile-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1078 2020-11-26 23:54:30.000000 trex_imager_readfile-1.1.0/LICENSE
--rw-r--r--   0        0        0     2989 2022-12-12 02:45:08.000000 trex_imager_readfile-1.1.0/README.md
--rw-r--r--   0        0        0      675 2023-03-07 15:58:14.209921 trex_imager_readfile-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      431 2023-03-07 15:07:21.699225 trex_imager_readfile-1.1.0/trex_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8171 2023-03-07 15:42:19.050937 trex_imager_readfile-1.1.0/trex_imager_readfile/blueline.py
--rw-r--r--   0        0        0     8121 2023-03-07 15:42:32.213166 trex_imager_readfile-1.1.0/trex_imager_readfile/nir.py
--rw-r--r--   0        0        0    16020 2023-03-07 16:42:26.556341 trex_imager_readfile-1.1.0/trex_imager_readfile/rgb.py
--rw-r--r--   0        0        0     8215 2023-03-07 15:41:52.731479 trex_imager_readfile-1.1.0/trex_imager_readfile/spectrograph.py
--rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 trex_imager_readfile-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.1.1/README.md
+-rw-r--r--   0        0        0      677 2023-04-26 18:45:57.197926 trex_imager_readfile-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      431 2023-04-26 18:45:57.231927 trex_imager_readfile-1.1.1/trex_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8171 2023-03-07 15:42:19.050937 trex_imager_readfile-1.1.1/trex_imager_readfile/blueline.py
+-rw-r--r--   0        0        0     8121 2023-03-07 15:42:32.213166 trex_imager_readfile-1.1.1/trex_imager_readfile/nir.py
+-rw-r--r--   0        0        0    15985 2023-04-26 18:43:07.594848 trex_imager_readfile-1.1.1/trex_imager_readfile/rgb.py
+-rw-r--r--   0        0        0     8215 2023-03-07 15:41:52.731479 trex_imager_readfile-1.1.1/trex_imager_readfile/spectrograph.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 trex_imager_readfile-1.1.1/PKG-INFO
```

### Comparing `trex_imager_readfile-1.1.0/pyproject.toml` & `trex_imager_readfile-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "trex-imager-readfile"
-version = "1.1.0"
-description = "Read functions for TREx ASI PGM raw files"
+version = "1.1.1"
+description = "Read functions for TREx ASI raw image files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "trex_imager_readfile" },
```

### Comparing `trex_imager_readfile-1.1.0/trex_imager_readfile/blueline.py` & `trex_imager_readfile-1.1.1/trex_imager_readfile/blueline.py`

 * *Files identical despite different names*

### Comparing `trex_imager_readfile-1.1.0/trex_imager_readfile/nir.py` & `trex_imager_readfile-1.1.1/trex_imager_readfile/nir.py`

 * *Files identical despite different names*

### Comparing `trex_imager_readfile-1.1.0/trex_imager_readfile/rgb.py` & `trex_imager_readfile-1.1.1/trex_imager_readfile/rgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,19 @@
     problematic = False
     error_message = ""
     image_width = 480
     image_height = 553
     image_channels = 1
     image_dtype = __RGB_PGM_DT
 
+    # Set metadata values
+    file_split = _os.path.basename(file_obj["filename"]).split('_')
+    site_uid = file_split[3]
+    device_uid = file_split[4]
+
     # check file extension to see if it's gzipped or not
     try:
         if file_obj["filename"].endswith("pgm.gz"):
             unzipped = _gzip.open(file_obj["filename"], mode='rb')
         elif file_obj["filename"].endswith("pgm"):
             unzipped = open(file_obj["filename"], mode='rb')
         else:
@@ -131,29 +136,19 @@
             # add entry to dictionary
             if (key in metadata_dict):
                 # key already exists, turn existing value into list and append new value
                 if (isinstance(metadata_dict[key], list)):
                     # is a list already
                     metadata_dict[key].append(value)
                 else:
-                    metadata_dict[key] = [metadata_dict[key]]
+                    metadata_dict[key] = [metadata_dict[key], value]
             else:
                 # normal metadata value
                 metadata_dict[key] = value
 
-            # set the site/device uids, or inject the site and device UIDs if they are missing
-            if ("Site unique ID" not in metadata_dict):
-                metadata_dict["Site unique ID"] = site_uid
-            else:
-                site_uid = metadata_dict["Site unique ID"]
-            if ("Imager unique ID" not in metadata_dict):
-                metadata_dict["Imager unique ID"] = device_uid
-            else:
-                device_uid = metadata_dict["Imager unique ID"]
-
             # split dictionaries up per frame, exposure plus initial readout is
             # always the end of metadata for frame
             if (key.startswith("Effective image exposure")):
                 metadata_dict_list.append(metadata_dict)
                 metadata_dict = {}
         elif line == b'65535\n':
             # there are 2 lines between "exposure plus read out" and the image
@@ -184,14 +179,21 @@
                 first_frame = False
             else:
                 images = _np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
 
     # close gzip file
     unzipped.close()
 
+    # set the site/device uids, or inject the site and device UIDs if they are missing
+    if ("Site unique ID" not in metadata_dict):
+        metadata_dict["Site unique ID"] = site_uid
+
+    if ("Imager unique ID" not in metadata_dict):
+        metadata_dict["Imager unique ID"] = device_uid
+
     # return
     return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
         image_width, image_height, image_channels, image_dtype
 
 
 def __rgb_readfile_worker_png(file_obj):
     # init
```

### Comparing `trex_imager_readfile-1.1.0/trex_imager_readfile/spectrograph.py` & `trex_imager_readfile-1.1.1/trex_imager_readfile/spectrograph.py`

 * *Files identical despite different names*

