# Comparing `tmp/PlexPreferNonForcedSubs-2.0.0.tar.gz` & `tmp/PlexPreferNonForcedSubs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexPreferNonForcedSubs-2.0.0.tar", last modified: Wed Apr 26 18:25:34 2023, max compression
+gzip compressed data, was "PlexPreferNonForcedSubs-2.0.1.tar", last modified: Wed Apr 26 18:57:18 2023, max compression
```

## Comparing `PlexPreferNonForcedSubs-2.0.0.tar` & `PlexPreferNonForcedSubs-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 18:25:34.256950 PlexPreferNonForcedSubs-2.0.0/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     4331 2023-04-26 18:25:34.256450 PlexPreferNonForcedSubs-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 18:25:34.226989 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs/
--rw-rw-rw-   0        0        0     5503 2023-04-25 19:48:56.000000 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 18:25:34.254453 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs.egg-info/
--rw-rw-rw-   0        0        0     4331 2023-04-26 18:25:34.000000 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-04-26 18:25:34.000000 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 18:25:34.000000 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 18:25:34.000000 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-26 18:25:34.000000 PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3707 2023-04-26 05:41:36.000000 PlexPreferNonForcedSubs-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 18:25:34.256950 PlexPreferNonForcedSubs-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1255 2023-04-26 18:16:19.000000 PlexPreferNonForcedSubs-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:57:18.668423 PlexPreferNonForcedSubs-2.0.1/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4331 2023-04-26 18:57:18.667923 PlexPreferNonForcedSubs-2.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 18:57:18.635465 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs/
+-rw-rw-rw-   0        0        0     5503 2023-04-25 19:48:56.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:57:18.665935 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/
+-rw-rw-rw-   0        0        0     4331 2023-04-26 18:57:18.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-26 18:57:18.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 18:57:18.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-26 18:57:18.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 18:57:18.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-26 18:57:18.000000 PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3707 2023-04-26 05:41:36.000000 PlexPreferNonForcedSubs-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 18:57:18.668922 PlexPreferNonForcedSubs-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2023-04-26 18:55:40.000000 PlexPreferNonForcedSubs-2.0.1/setup.py
```

### Comparing `PlexPreferNonForcedSubs-2.0.0/LICENSE` & `PlexPreferNonForcedSubs-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.0.0/PKG-INFO` & `PlexPreferNonForcedSubs-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.0.0
+Version: 2.0.1
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py` & `PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.0.0/PlexPreferNonForcedSubs.egg-info/PKG-INFO` & `PlexPreferNonForcedSubs-2.0.1/PlexPreferNonForcedSubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.0.0
+Version: 2.0.1
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexPreferNonForcedSubs-2.0.0/README.md` & `PlexPreferNonForcedSubs-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.0.0/setup.py` & `PlexPreferNonForcedSubs-2.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
+#To create package: python setup.py sdist bdist_wheel
+#To upload package: twine upload dist/*
+
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.0.0'
+VERSION = '2.0.1'
 DESCRIPTION = 'This script will set all movies and shows in your local Plex library to English non forced subtitles by default.'
 LONG_DESCRIPTION = 'This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.'
 
 # Setting up
 setup(
     name="PlexPreferNonForcedSubs",
     version=VERSION,
@@ -23,9 +26,14 @@
     install_requires=['plexapi'],
     keywords=['python', 'video', 'plex', 'subtitles', 'subs'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
-    ]
-)
+    ],
+    entry_points={
+        'console_scripts': [
+            'PlexPreferNonForcedSubs = PlexPreferNonForcedSubs.PlexPreferNonForcedSubs:main'
+        ]
+    }
+)
```

