# Comparing `tmp/podcast_archiver-0.4.3.tar.gz` & `tmp/podcast_archiver-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_archiver-0.4.3.tar", max compression
+gzip compressed data, was "podcast_archiver-0.5.0.tar", max compression
```

## Comparing `podcast_archiver-0.4.3.tar` & `podcast_archiver-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1056 2023-04-22 15:52:07.926595 podcast_archiver-0.4.3/LICENSE
--rw-r--r--   0        0        0     4943 2023-04-22 15:52:07.926595 podcast_archiver-0.4.3/README.md
--rwxr-xr-x   0        0        0    15774 2023-04-22 15:52:24.462695 podcast_archiver-0.4.3/podcast_archiver.py
--rw-r--r--   0        0        0     1623 2023-04-22 15:52:24.462695 podcast_archiver-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 podcast_archiver-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4943 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-26 18:05:51.556391 podcast_archiver-0.5.0/podcast_archiver/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/podcast_archiver/__main__.py
+-rw-r--r--   0        0        0     2545 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/podcast_archiver/argparse.py
+-rwxr-xr-x   0        0        0    12472 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/podcast_archiver/base.py
+-rw-r--r--   0        0        0     1625 2023-04-26 18:05:51.556391 podcast_archiver-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 podcast_archiver-0.5.0/PKG-INFO
```

### Comparing `podcast_archiver-0.4.3/LICENSE` & `podcast_archiver-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_archiver-0.4.3/README.md` & `podcast_archiver-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `podcast_archiver-0.4.3/pyproject.toml` & `podcast_archiver-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "podcast-archiver"
-version = "0.4.3"
+version = "0.5.0"
 description = "Archive all episodes from your favorite podcasts"
 authors = ["Jan Willhaus <mail@janwillhaus.de>"]
 license = "MIT"
 readme = "README.md"
-packages = [{ include = "podcast_archiver.py" }]
+packages = [{ include = "podcast_archiver" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Information Technology",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
@@ -22,15 +22,15 @@
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 strict = true
 
 [tool.poetry.scripts]
-podcast-archiver = 'podcast_archiver:main'
+podcast-archiver = 'podcast_archiver.base:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dateutil = "^2.8.2"
 feedparser = "^6.0.10"
 tqdm = "^4.65.0"
```

### Comparing `podcast_archiver-0.4.3/PKG-INFO` & `podcast_archiver-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-archiver
-Version: 0.4.3
+Version: 0.5.0
 Summary: Archive all episodes from your favorite podcasts
 License: MIT
 Author: Jan Willhaus
 Author-email: mail@janwillhaus.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

