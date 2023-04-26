# Comparing `tmp/PlexPreferNonForcedSubs-2.0.2.tar.gz` & `tmp/PlexPreferNonForcedSubs-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexPreferNonForcedSubs-2.0.2.tar", last modified: Wed Apr 26 19:08:42 2023, max compression
+gzip compressed data, was "PlexPreferNonForcedSubs-2.0.3.tar", last modified: Wed Apr 26 19:11:03 2023, max compression
```

## Comparing `PlexPreferNonForcedSubs-2.0.2.tar` & `PlexPreferNonForcedSubs-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 19:08:42.285473 PlexPreferNonForcedSubs-2.0.2/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     4331 2023-04-26 19:08:42.284973 PlexPreferNonForcedSubs-2.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 19:08:42.264136 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs/
--rw-rw-rw-   0        0        0     5856 2023-04-26 16:45:01.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 19:08:42.282976 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/
--rw-rw-rw-   0        0        0     4331 2023-04-26 19:08:42.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-26 19:08:42.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 19:08:42.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-04-26 19:08:42.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 19:08:42.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-26 19:08:42.000000 PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3707 2023-04-26 05:41:36.000000 PlexPreferNonForcedSubs-2.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 19:08:42.285973 PlexPreferNonForcedSubs-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1516 2023-04-26 19:08:33.000000 PlexPreferNonForcedSubs-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:11:03.811014 PlexPreferNonForcedSubs-2.0.3/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4331 2023-04-26 19:11:03.810524 PlexPreferNonForcedSubs-2.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 19:11:03.789052 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs/
+-rw-rw-rw-   0        0        0     5856 2023-04-26 16:45:01.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:11:03.808526 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/
+-rw-rw-rw-   0        0        0     4331 2023-04-26 19:11:03.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-26 19:11:03.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 19:11:03.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-26 19:11:03.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 19:11:03.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-26 19:11:03.000000 PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3707 2023-04-26 05:41:36.000000 PlexPreferNonForcedSubs-2.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 19:11:03.811513 PlexPreferNonForcedSubs-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2023-04-26 19:10:45.000000 PlexPreferNonForcedSubs-2.0.3/setup.py
```

### Comparing `PlexPreferNonForcedSubs-2.0.2/LICENSE` & `PlexPreferNonForcedSubs-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.0.2/PKG-INFO` & `PlexPreferNonForcedSubs-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.0.2
+Version: 2.0.3
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py` & `PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.0.2/PlexPreferNonForcedSubs.egg-info/PKG-INFO` & `PlexPreferNonForcedSubs-2.0.3/PlexPreferNonForcedSubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.0.2
+Version: 2.0.3
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexPreferNonForcedSubs-2.0.2/README.md` & `PlexPreferNonForcedSubs-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.0.2/setup.py` & `PlexPreferNonForcedSubs-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.0.2'
+VERSION = '2.0.3'
 DESCRIPTION = 'This script will set all movies and shows in your local Plex library to English non forced subtitles by default.'
 LONG_DESCRIPTION = 'This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.'
 
 # Setting up
 setup(
     name="PlexPreferNonForcedSubs",
     version=VERSION,
@@ -29,11 +29,11 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'PlexPreferNonForcedSubs = PlexPreferNonForcedSubs.PlexPreferNonForcedSubs.py'
+            'PlexPreferNonForcedSubs = PlexPreferNonForcedSubs.PlexPreferNonForcedSubs.main'
         ]
     }
 )
```

