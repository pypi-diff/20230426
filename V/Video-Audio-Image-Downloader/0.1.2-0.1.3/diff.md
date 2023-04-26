# Comparing `tmp/Video_Audio_Image_Downloader-0.1.2.tar.gz` & `tmp/Video_Audio_Image_Downloader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Video_Audio_Image_Downloader-0.1.2.tar", last modified: Tue Apr 25 16:54:36 2023, max compression
+gzip compressed data, was "Video_Audio_Image_Downloader-0.1.3.tar", last modified: Tue Apr 25 16:59:51 2023, max compression
```

## Comparing `Video_Audio_Image_Downloader-0.1.2.tar` & `Video_Audio_Image_Downloader-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:54:36.874502 Video_Audio_Image_Downloader-0.1.2/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4348 2023-04-25 16:54:36.874502 Video_Audio_Image_Downloader-0.1.2/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4088 2023-04-25 16:54:26.000000 Video_Audio_Image_Downloader-0.1.2/README.md
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:54:36.874502 Video_Audio_Image_Downloader-0.1.2/Video_Audio_Image_Downloader.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4348 2023-04-25 16:54:36.000000 Video_Audio_Image_Downloader-0.1.2/Video_Audio_Image_Downloader.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      413 2023-04-25 16:54:36.000000 Video_Audio_Image_Downloader-0.1.2/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-25 16:54:36.000000 Video_Audio_Image_Downloader-0.1.2/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-25 16:54:36.000000 Video_Audio_Image_Downloader-0.1.2/Video_Audio_Image_Downloader.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-25 16:54:36.000000 Video_Audio_Image_Downloader-0.1.2/Video_Audio_Image_Downloader.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-25 16:54:36.874502 Video_Audio_Image_Downloader-0.1.2/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      914 2023-04-25 16:54:32.000000 Video_Audio_Image_Downloader-0.1.2/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:54:36.874502 Video_Audio_Image_Downloader-0.1.2/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:22:38.000000 Video_Audio_Image_Downloader-0.1.2/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:54:36.874502 Video_Audio_Image_Downloader-0.1.2/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-25 16:22:38.000000 Video_Audio_Image_Downloader-0.1.2/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3519 2023-04-25 16:38:31.000000 Video_Audio_Image_Downloader-0.1.2/source/lib/Command_function.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-25 16:22:38.000000 Video_Audio_Image_Downloader-0.1.2/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3522 2023-04-25 16:41:22.000000 Video_Audio_Image_Downloader-0.1.2/source/lib/help.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4259 2023-04-25 16:38:39.000000 Video_Audio_Image_Downloader-0.1.2/source/source.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:59:51.727624 Video_Audio_Image_Downloader-0.1.3/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4299 2023-04-25 16:59:51.727624 Video_Audio_Image_Downloader-0.1.3/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4038 2023-04-25 16:57:56.000000 Video_Audio_Image_Downloader-0.1.3/README.md
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:59:51.723624 Video_Audio_Image_Downloader-0.1.3/Video_Audio_Image_Downloader.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4299 2023-04-25 16:59:51.000000 Video_Audio_Image_Downloader-0.1.3/Video_Audio_Image_Downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      413 2023-04-25 16:59:51.000000 Video_Audio_Image_Downloader-0.1.3/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-25 16:59:51.000000 Video_Audio_Image_Downloader-0.1.3/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-25 16:59:51.000000 Video_Audio_Image_Downloader-0.1.3/Video_Audio_Image_Downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-25 16:59:51.000000 Video_Audio_Image_Downloader-0.1.3/Video_Audio_Image_Downloader.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-25 16:59:51.727624 Video_Audio_Image_Downloader-0.1.3/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      914 2023-04-25 16:59:36.000000 Video_Audio_Image_Downloader-0.1.3/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:59:51.727624 Video_Audio_Image_Downloader-0.1.3/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:22:38.000000 Video_Audio_Image_Downloader-0.1.3/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 16:59:51.727624 Video_Audio_Image_Downloader-0.1.3/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-25 16:22:38.000000 Video_Audio_Image_Downloader-0.1.3/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3519 2023-04-25 16:38:31.000000 Video_Audio_Image_Downloader-0.1.3/source/lib/Command_function.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-25 16:22:38.000000 Video_Audio_Image_Downloader-0.1.3/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3522 2023-04-25 16:41:22.000000 Video_Audio_Image_Downloader-0.1.3/source/lib/help.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4259 2023-04-25 16:38:39.000000 Video_Audio_Image_Downloader-0.1.3/source/source.py
```

### Comparing `Video_Audio_Image_Downloader-0.1.2/PKG-INFO` & `Video_Audio_Image_Downloader-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Video_Audio_Image_Downloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: In this tool is help to Download the Youtube Video,Audio and Any type of Google and other site's Images
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/audio_video_image_downloder-1
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -139,10 +139,9 @@
 
     optional arguments:
 
             -path           
                             The Path of the Image to  be download.
                             For now,The default path is your Current Working Directory
 
-### Contact 
-    1. Email - dcsvsridhar@gmail.com
+
```

### Comparing `Video_Audio_Image_Downloader-0.1.2/README.md` & `Video_Audio_Image_Downloader-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -128,9 +128,7 @@
 
     optional arguments:
 
             -path           
                             The Path of the Image to  be download.
                             For now,The default path is your Current Working Directory
 
-### Contact 
-    1. Email - dcsvsridhar@gmail.com
```

### Comparing `Video_Audio_Image_Downloader-0.1.2/Video_Audio_Image_Downloader.egg-info/PKG-INFO` & `Video_Audio_Image_Downloader-0.1.3/Video_Audio_Image_Downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Video-Audio-Image-Downloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: In this tool is help to Download the Youtube Video,Audio and Any type of Google and other site's Images
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/audio_video_image_downloder-1
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -139,10 +139,9 @@
 
     optional arguments:
 
             -path           
                             The Path of the Image to  be download.
                             For now,The default path is your Current Working Directory
 
-### Contact 
-    1. Email - dcsvsridhar@gmail.com
+
```

### Comparing `Video_Audio_Image_Downloader-0.1.2/setup.py` & `Video_Audio_Image_Downloader-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Video_Audio_Image_Downloader',
-    version='0.1.2',
+    version='0.1.3',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     #  to help download videos and audio files from Youtube
     description="In this tool is help to Download the Youtube Video,Audio and Any type of Google and other site's Images",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/audio_video_image_downloder-1',
     install_requires=requirements,
```

### Comparing `Video_Audio_Image_Downloader-0.1.2/source/lib/Argument.py` & `Video_Audio_Image_Downloader-0.1.3/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.1.2/source/lib/Command_function.py` & `Video_Audio_Image_Downloader-0.1.3/source/lib/Command_function.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.1.2/source/lib/help.py` & `Video_Audio_Image_Downloader-0.1.3/source/lib/help.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.1.2/source/source.py` & `Video_Audio_Image_Downloader-0.1.3/source/source.py`

 * *Files identical despite different names*

