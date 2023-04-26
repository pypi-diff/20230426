# Comparing `tmp/chapsnap-1.0.0.tar.gz` & `tmp/chapsnap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chapsnap-1.0.0.tar", max compression
+gzip compressed data, was "chapsnap-1.1.0.tar", max compression
```

## Comparing `chapsnap-1.0.0.tar` & `chapsnap-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 00:41:54.909853 chapsnap-1.0.0/LICENSE
--rw-r--r--   0        0        0      469 2023-04-26 00:41:54.909853 chapsnap-1.0.0/README.md
--rw-r--r--   0        0        0       23 2023-04-26 00:41:54.909853 chapsnap-1.0.0/chapsnap/__init__.py
--rw-r--r--   0        0        0     5109 2023-04-26 00:41:54.909853 chapsnap-1.0.0/chapsnap/main.py
--rw-r--r--   0        0        0     1064 2023-04-26 00:41:54.909853 chapsnap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 chapsnap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 16:15:52.298321 chapsnap-1.1.0/LICENSE
+-rw-r--r--   0        0        0      468 2023-04-26 16:15:52.298321 chapsnap-1.1.0/README.md
+-rw-r--r--   0        0        0       23 2023-04-26 16:15:52.298321 chapsnap-1.1.0/chapsnap/__init__.py
+-rw-r--r--   0        0        0     7565 2023-04-26 16:15:52.298321 chapsnap-1.1.0/chapsnap/main.py
+-rw-r--r--   0        0        0     1064 2023-04-26 16:15:52.298321 chapsnap-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 chapsnap-1.1.0/PKG-INFO
```

### Comparing `chapsnap-1.0.0/LICENSE` & `chapsnap-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chapsnap-1.0.0/pyproject.toml` & `chapsnap-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ChapSnap"
-version = "1.0.0"
+version = "1.1.0"
 description = "Resync Chapters by snapping them to Scene Changes."
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 readme = "README.md"
 repository = "https://github.com/rlaphoenix/ChapSnap"
 keywords = ["python", "chapters", "video", "analysis", "scene-detection"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `chapsnap-1.0.0/PKG-INFO` & `chapsnap-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chapsnap
-Version: 1.0.0
+Version: 1.1.0
 Summary: Resync Chapters by snapping them to Scene Changes.
 Home-page: https://github.com/rlaphoenix/ChapSnap
 Keywords: python,chapters,video,analysis,scene-detection
 Author: rlaphoenix
 Author-email: rlaphoenix@pm.me
 Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -30,15 +30,15 @@
 
 # ChapSnap
 
 Resync Chapters by snapping them to Scene Changes.
 
 ## To-do
 
-- [ ] Automatically replace the subtitles in the input video container.
+- [x] Automatically replace the chapters in the input video container.
 
 Likely lot's more.
 
 ## Contributors
 
 <a href="https://github.com/rlaphoenix"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/17136956?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt=""/></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chapsnap Version: 1.0.0 Summary: Resync Chapters by
+Metadata-Version: 2.1 Name: chapsnap Version: 1.1.0 Summary: Resync Chapters by
 snapping them to Scene Changes. Home-page: https://github.com/rlaphoenix/
 ChapSnap Keywords: python,chapters,video,analysis,scene-detection Author:
 rlaphoenix Author-email: rlaphoenix@pm.me Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience :: End
 Users/Desktop Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
@@ -12,10 +12,10 @@
 Multimedia :: Video Classifier: Topic :: Utilities Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: rich (>=13.3.4,<14.0.0) Project-URL: Bug
 Tracker, https://github.com/rlaphoenix/ChapSnap/issues Project-URL: Changelog,
 https://github.com/rlaphoenix/ChapSnap/blob/master/CHANGELOG.md Project-URL:
 Forums, https://github.com/rlaphoenix/ChapSnap/discussions Project-URL:
 Repository, https://github.com/rlaphoenix/ChapSnap Description-Content-Type:
 text/markdown # ChapSnap Resync Chapters by snapping them to Scene Changes. ##
-To-do - [ ] Automatically replace the subtitles in the input video container.
+To-do - [x] Automatically replace the chapters in the input video container.
 Likely lot's more. ## Contributors  ## License Â© 2023 rlaphoenix â [GNU
 General Public License, Version 3.0](LICENSE)
```

