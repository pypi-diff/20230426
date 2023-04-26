# Comparing `tmp/avutil-1.5.1.tar.gz` & `tmp/avutil-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avutil-1.5.1.tar", last modified: Tue Mar 21 11:37:46 2023, max compression
+gzip compressed data, was "avutil-1.6.0.tar", last modified: Wed Apr 26 11:41:51 2023, max compression
```

## Comparing `avutil-1.5.1.tar` & `avutil-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-03-21 11:37:46.329039 avutil-1.5.1/
--rw-r--r--   0 robinlu    (501) staff       (20)    35149 2021-02-03 05:30:31.000000 avutil-1.5.1/LICENSE
--rw-r--r--   0 robinlu    (501) staff       (20)     3183 2023-03-21 11:37:46.328378 avutil-1.5.1/PKG-INFO
--rw-r--r--   0 robinlu    (501) staff       (20)     2751 2022-08-06 06:50:08.000000 avutil-1.5.1/README.md
-drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-03-21 11:37:46.317349 avutil-1.5.1/avutil/
--rw-r--r--   0 robinlu    (501) staff       (20)      107 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/__init__.py
-drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-03-21 11:37:46.323923 avutil-1.5.1/avutil/encoder/
--rw-r--r--   0 robinlu    (501) staff       (20)       90 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/encoder/__init__.py
--rw-r--r--   0 robinlu    (501) staff       (20)     2423 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/encoder/nfo.py
--rw-r--r--   0 robinlu    (501) staff       (20)     3398 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/encoder/vsmeta.py
--rw-r--r--   0 robinlu    (501) staff       (20)     1573 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/info.py
-drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-03-21 11:37:46.327000 avutil-1.5.1/avutil/source/
--rw-r--r--   0 robinlu    (501) staff       (20)       76 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/source/__init__.py
--rw-r--r--   0 robinlu    (501) staff       (20)     5073 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/source/bus.py
--rw-r--r--   0 robinlu    (501) staff       (20)     6100 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/source/library.py
--rwxr-xr-x   0 robinlu    (501) staff       (20)     3506 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/tidy_up.py
--rw-r--r--   0 robinlu    (501) staff       (20)     1535 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/util.py
--rwxr-xr-x   0 robinlu    (501) staff       (20)     7828 2023-03-21 11:36:44.000000 avutil-1.5.1/avutil/video.py
-drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-03-21 11:37:46.321033 avutil-1.5.1/avutil.egg-info/
--rw-r--r--   0 robinlu    (501) staff       (20)     3183 2023-03-21 11:37:46.000000 avutil-1.5.1/avutil.egg-info/PKG-INFO
--rw-r--r--   0 robinlu    (501) staff       (20)      437 2023-03-21 11:37:46.000000 avutil-1.5.1/avutil.egg-info/SOURCES.txt
--rw-r--r--   0 robinlu    (501) staff       (20)        1 2023-03-21 11:37:46.000000 avutil-1.5.1/avutil.egg-info/dependency_links.txt
--rw-r--r--   0 robinlu    (501) staff       (20)       40 2023-03-21 11:37:46.000000 avutil-1.5.1/avutil.egg-info/entry_points.txt
--rw-r--r--   0 robinlu    (501) staff       (20)       75 2023-03-21 11:37:46.000000 avutil-1.5.1/avutil.egg-info/requires.txt
--rw-r--r--   0 robinlu    (501) staff       (20)        7 2023-03-21 11:37:46.000000 avutil-1.5.1/avutil.egg-info/top_level.txt
--rw-r--r--   0 robinlu    (501) staff       (20)       38 2023-03-21 11:37:46.329248 avutil-1.5.1/setup.cfg
--rw-r--r--   0 robinlu    (501) staff       (20)      927 2023-03-21 11:37:14.000000 avutil-1.5.1/setup.py
+drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-04-26 11:41:51.740393 avutil-1.6.0/
+-rw-r--r--   0 robinlu    (501) staff       (20)    35149 2021-02-03 05:30:31.000000 avutil-1.6.0/LICENSE
+-rw-r--r--   0 robinlu    (501) staff       (20)     3183 2023-04-26 11:41:51.739922 avutil-1.6.0/PKG-INFO
+-rw-r--r--   0 robinlu    (501) staff       (20)     2751 2022-08-06 06:50:08.000000 avutil-1.6.0/README.md
+drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-04-26 11:41:51.731176 avutil-1.6.0/avutil/
+-rw-r--r--   0 robinlu    (501) staff       (20)      107 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/__init__.py
+drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-04-26 11:41:51.737331 avutil-1.6.0/avutil/encoder/
+-rw-r--r--   0 robinlu    (501) staff       (20)       90 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/encoder/__init__.py
+-rw-r--r--   0 robinlu    (501) staff       (20)     2423 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/encoder/nfo.py
+-rw-r--r--   0 robinlu    (501) staff       (20)     5167 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/encoder/vsmeta.py
+-rw-r--r--   0 robinlu    (501) staff       (20)     1573 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/info.py
+drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-04-26 11:41:51.739215 avutil-1.6.0/avutil/source/
+-rw-r--r--   0 robinlu    (501) staff       (20)       76 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/source/__init__.py
+-rw-r--r--   0 robinlu    (501) staff       (20)     5073 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/source/bus.py
+-rw-r--r--   0 robinlu    (501) staff       (20)     6100 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/source/library.py
+-rwxr-xr-x   0 robinlu    (501) staff       (20)     3810 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/tidy_up.py
+-rw-r--r--   0 robinlu    (501) staff       (20)     1535 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/util.py
+-rwxr-xr-x   0 robinlu    (501) staff       (20)     7797 2023-04-26 11:40:34.000000 avutil-1.6.0/avutil/video.py
+drwxr-xr-x   0 robinlu    (501) staff       (20)        0 2023-04-26 11:41:51.734960 avutil-1.6.0/avutil.egg-info/
+-rw-r--r--   0 robinlu    (501) staff       (20)     3183 2023-04-26 11:41:51.000000 avutil-1.6.0/avutil.egg-info/PKG-INFO
+-rw-r--r--   0 robinlu    (501) staff       (20)      437 2023-04-26 11:41:51.000000 avutil-1.6.0/avutil.egg-info/SOURCES.txt
+-rw-r--r--   0 robinlu    (501) staff       (20)        1 2023-04-26 11:41:51.000000 avutil-1.6.0/avutil.egg-info/dependency_links.txt
+-rw-r--r--   0 robinlu    (501) staff       (20)       40 2023-04-26 11:41:51.000000 avutil-1.6.0/avutil.egg-info/entry_points.txt
+-rw-r--r--   0 robinlu    (501) staff       (20)       75 2023-04-26 11:41:51.000000 avutil-1.6.0/avutil.egg-info/requires.txt
+-rw-r--r--   0 robinlu    (501) staff       (20)        7 2023-04-26 11:41:51.000000 avutil-1.6.0/avutil.egg-info/top_level.txt
+-rw-r--r--   0 robinlu    (501) staff       (20)       38 2023-04-26 11:41:51.740559 avutil-1.6.0/setup.cfg
+-rw-r--r--   0 robinlu    (501) staff       (20)      927 2023-04-26 11:41:45.000000 avutil-1.6.0/setup.py
```

### Comparing `avutil-1.5.1/LICENSE` & `avutil-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avutil-1.5.1/PKG-INFO` & `avutil-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avutil
-Version: 1.5.1
+Version: 1.6.0
 Summary: Provide some useful util functions and a poweful tool (tidyup) for tidying up your video folder
 Author: Everyone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4.0
 Description-Content-Type: text/markdown
```

### Comparing `avutil-1.5.1/README.md` & `avutil-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `avutil-1.5.1/avutil/encoder/nfo.py` & `avutil-1.6.0/avutil/encoder/nfo.py`

 * *Files identical despite different names*

### Comparing `avutil-1.5.1/avutil/info.py` & `avutil-1.6.0/avutil/info.py`

 * *Files identical despite different names*

### Comparing `avutil-1.5.1/avutil/source/bus.py` & `avutil-1.6.0/avutil/source/bus.py`

 * *Files identical despite different names*

### Comparing `avutil-1.5.1/avutil/source/library.py` & `avutil-1.6.0/avutil/source/library.py`

 * *Files identical despite different names*

### Comparing `avutil-1.5.1/avutil/tidy_up.py` & `avutil-1.6.0/avutil/tidy_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 sys.setrecursionlimit(10000)
 
 src_folder = "./"
 dst_folder = "./"
 http_proxy = ""
 source = avutil.source.Library
-encoder = avutil.encoder.NFOEncoder
+encoders = []
 thread = 8
 with_poster = False
 
 
 def VideoProcess(video):
     global src_folder
     global dst_folder
     global http_proxy
     global source
-    global encoder
+    global encoders
     global thread
     global with_poster
 
     try:
         designatio, file_paths = video
         video = avutil.Video(designatio, file_paths)
 
@@ -39,16 +39,17 @@
         # Download cover
         video.download_cover(dst_dir=dst_folder,
                              http_proxy=http_proxy, with_poster=with_poster)
 
         # Tidy up
         video.rename(dst_dir=dst_folder)
 
-        # Save video info as .nfo
-        video.save_info(dst_dir=dst_folder, encoder=encoder)
+        # Save video info with encoders
+        for encoder in encoders:
+            video.save_info(dst_dir=dst_folder, encoder=encoder)
     except Exception as e:
         print("WARN:", e)
         pass
 
 
 def get_arguments(args=sys.argv[1:]):
     parser = argparse.ArgumentParser(
@@ -62,27 +63,27 @@
     parser.add_argument("-p", "--proxy", dest='proxy',
                         help="http proxy address")
     parser.add_argument("-s", "--source", dest='source',
                         help="data source of video info, 'library' or 'bus'")
     parser.add_argument("-t", "--thread", dest='thread', type=int,
                         help="threads num, use multi-threads to download info & images")
     parser.add_argument("-e", "--encoder", dest='encoder',
-                        help="encoder of meta-data, 'nfo'(default) or 'vsmeta'")
+                        help="encoders of meta-data, 'nfo'(default) or 'vsmeta'", )
     parser.add_argument("--with-poster", dest='with_poster', action='store_true',
                         help="save poster")
     return parser.parse_args(args)
 
 
 def main():
 
     global src_folder
     global dst_folder
     global http_proxy
     global source
-    global encoder
+    global encoders
     global thread
     global with_poster
 
     args = get_arguments()
     # args.dir
     if args.IN is not None:
         src_folder = args.IN
@@ -96,16 +97,23 @@
         http_proxy = args.proxy
 
     # Data source
     if args.source == "bus":
         source = avutil.source.Bus
 
     # Encoder
-    if args.encoder == "vsmeta":
-        encoder = avutil.encoder.VSMETAEncoder
+    if args.encoder is not None:
+        selected_encoders = args.encoder.split(",")
+        for e in selected_encoders:
+            if e == "nfo":
+                encoders.append(avutil.encoder.NFOEncoder)
+            elif e == "vsmeta":
+                encoders.append(avutil.encoder.VSMETAEncoder)
+    else:
+        encoders = [avutil.encoder.NFOEncoder]
 
     # Gen poster
     if args.with_poster == True:
         with_poster = True
 
     # Threads num
     if args.thread is not None:
```

### Comparing `avutil-1.5.1/avutil/util.py` & `avutil-1.6.0/avutil/util.py`

 * *Files identical despite different names*

### Comparing `avutil-1.5.1/avutil/video.py` & `avutil-1.6.0/avutil/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import io
 import re
 import requests
 import xml.etree.ElementTree as ET
 import PIL.Image
 
 from avutil.info import VideoInfo
-# from avutil import VideoInfo
 from avutil.encoder import NFOEncoder
 from avutil.encoder import VSMETAEncoder
 from avutil.source import Library
 from avutil.source import Bus
 
 
 def strip(string):
```

### Comparing `avutil-1.5.1/avutil.egg-info/PKG-INFO` & `avutil-1.6.0/avutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avutil
-Version: 1.5.1
+Version: 1.6.0
 Summary: Provide some useful util functions and a poweful tool (tidyup) for tidying up your video folder
 Author: Everyone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4.0
 Description-Content-Type: text/markdown
```

### Comparing `avutil-1.5.1/setup.py` & `avutil-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="avutil",
-    version="1.5.1",
+    version="1.6.0",
     author="Everyone",
     description="Provide some useful util functions and a poweful tool (tidyup) for tidying up your video folder",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

