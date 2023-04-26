# Comparing `tmp/podcast_archiver-0.5.0.tar.gz` & `tmp/podcast_archiver-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_archiver-0.5.0.tar", max compression
+gzip compressed data, was "podcast_archiver-0.5.1.tar", max compression
```

## Comparing `podcast_archiver-0.5.0.tar` & `podcast_archiver-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1056 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/LICENSE
--rw-r--r--   0        0        0     4943 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/README.md
--rw-r--r--   0        0        0       22 2023-04-26 18:05:51.556391 podcast_archiver-0.5.0/podcast_archiver/__init__.py
--rw-r--r--   0        0        0      632 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/podcast_archiver/__main__.py
--rw-r--r--   0        0        0     2545 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/podcast_archiver/argparse.py
--rwxr-xr-x   0        0        0    12472 2023-04-26 18:05:34.764216 podcast_archiver-0.5.0/podcast_archiver/base.py
--rw-r--r--   0        0        0     1625 2023-04-26 18:05:51.556391 podcast_archiver-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 podcast_archiver-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-26 18:26:34.820101 podcast_archiver-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4943 2023-04-26 18:26:34.820101 podcast_archiver-0.5.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-26 18:26:51.304555 podcast_archiver-0.5.1/podcast_archiver/__init__.py
+-rw-r--r--   0        0        0      753 2023-04-26 18:26:34.820101 podcast_archiver-0.5.1/podcast_archiver/__main__.py
+-rw-r--r--   0        0        0     2637 2023-04-26 18:26:34.820101 podcast_archiver-0.5.1/podcast_archiver/argparse.py
+-rwxr-xr-x   0        0        0    12472 2023-04-26 18:26:34.820101 podcast_archiver-0.5.1/podcast_archiver/base.py
+-rw-r--r--   0        0        0     1629 2023-04-26 18:26:51.300554 podcast_archiver-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 podcast_archiver-0.5.1/PKG-INFO
```

### Comparing `podcast_archiver-0.5.0/LICENSE` & `podcast_archiver-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_archiver-0.5.0/README.md` & `podcast_archiver-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `podcast_archiver-0.5.0/podcast_archiver/__main__.py` & `podcast_archiver-0.5.1/podcast_archiver/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import argparse
 import sys
 
+from podcast_archiver import __version__
 from podcast_archiver.argparse import parser
 from podcast_archiver.base import PodcastArchiver
 
 
 def main():
     try:
         args = parser.parse_args()
+        if args.version:
+            print(__version__)
+            sys.exit(0)
         if not (args.opml or args.feed):
             parser.error("Must provide at least one of --feed or --opml")
 
         pa = PodcastArchiver()
         pa.addArguments(args)
         pa.processFeeds()
     except KeyboardInterrupt:
```

### Comparing `podcast_archiver-0.5.0/podcast_archiver/argparse.py` & `podcast_archiver-0.5.1/podcast_archiver/argparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,7 +70,8 @@
     "--date-prefix",
     action="store_true",
     help=(
         "Prefix all episodes with an ISO8602 formatted date of when they were published. Useful to ensure"
         " chronological ordering."
     ),
 )
+parser.add_argument("-V", "--version", action="store_true", help="Print version and exit.")
```

### Comparing `podcast_archiver-0.5.0/podcast_archiver/base.py` & `podcast_archiver-0.5.1/podcast_archiver/base.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-0.5.0/pyproject.toml` & `podcast_archiver-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "podcast-archiver"
-version = "0.5.0"
+version = "0.5.1"
 description = "Archive all episodes from your favorite podcasts"
 authors = ["Jan Willhaus <mail@janwillhaus.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "podcast_archiver" }]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -22,15 +22,15 @@
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 strict = true
 
 [tool.poetry.scripts]
-podcast-archiver = 'podcast_archiver.base:main'
+podcast-archiver = 'podcast_archiver.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dateutil = "^2.8.2"
 feedparser = "^6.0.10"
 tqdm = "^4.65.0"
```

### Comparing `podcast_archiver-0.5.0/PKG-INFO` & `podcast_archiver-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-archiver
-Version: 0.5.0
+Version: 0.5.1
 Summary: Archive all episodes from your favorite podcasts
 License: MIT
 Author: Jan Willhaus
 Author-email: mail@janwillhaus.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

