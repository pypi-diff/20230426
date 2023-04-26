# Comparing `tmp/rssfixer-0.1.0.tar.gz` & `tmp/rssfixer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.1.0.tar", last modified: Sun Apr 23 11:36:05 2023, max compression
+gzip compressed data, was "rssfixer-0.1.1.tar", last modified: Wed Apr 26 11:15:08 2023, max compression
```

## Comparing `rssfixer-0.1.0.tar` & `rssfixer-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.510625 rssfixer-0.1.0/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.0/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     7797 2023-04-23 11:36:05.510489 rssfixer-0.1.0/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     6994 2023-04-23 08:48:37.000000 rssfixer-0.1.0/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)     1110 2023-04-23 11:34:36.000000 rssfixer-0.1.0/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-23 11:36:05.510675 rssfixer-0.1.0/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.508005 rssfixer-0.1.0/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.509257 rssfixer-0.1.0/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.0/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)     9423 2023-04-23 06:15:20.000000 rssfixer-0.1.0/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.510030 rssfixer-0.1.0/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     7797 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)      203 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.510149 rssfixer-0.1.0/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)     4362 2023-04-23 08:49:18.000000 rssfixer-0.1.0/src/tests/test_rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.524610 rssfixer-0.1.1/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.1/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     8201 2023-04-26 11:15:08.524389 rssfixer-0.1.1/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     7375 2023-04-25 13:13:18.000000 rssfixer-0.1.1/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-26 11:14:21.000000 rssfixer-0.1.1/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-26 11:15:08.524672 rssfixer-0.1.1/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.520047 rssfixer-0.1.1/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.521592 rssfixer-0.1.1/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.1/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)    10391 2023-04-26 10:13:53.000000 rssfixer-0.1.1/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.522807 rssfixer-0.1.1/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     8201 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      371 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.523883 rssfixer-0.1.1/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-26 04:26:11.000000 rssfixer-0.1.1/src/tests/test_rss.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     2535 2023-04-26 10:13:53.000000 rssfixer-0.1.1/src/tests/test_rss_args.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     2098 2023-04-26 10:13:53.000000 rssfixer-0.1.1/src/tests/test_rss_main.py
```

### Comparing `rssfixer-0.1.0/LICENSE` & `rssfixer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.0/PKG-INFO` & `rssfixer-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,28 +14,33 @@
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: audit
 Provides-Extra: build
 Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: github
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
-[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
-![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
-[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
-[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 <!-- CODE:BASH:START -->
+<!-- echo '[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)' -->
+<!-- echo '![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)' -->
+<!-- echo '[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)' -->
+<!-- echo '[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)' -->
 <!-- if jq '.metrics._totals | ."SEVERITY.HIGH"' resources/bandit.json | grep -vE '^0' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-red.svg)](https://github.com/PyCQA/bandit)' ; elif jq '.metrics._totals' resources/bandit.json | grep "SEVERITY" | grep -E ' 0,' | wc -l | grep -vE '4$' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)'; else echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)' ;fi -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
+![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
+[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 [![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 <!-- OUTPUT:END -->
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
@@ -99,62 +104,62 @@
 <!-- rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html]
-                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
-                [--html-title HTML_TITLE]
+usage: rssfixer [-h] (--html | --json | --list) [--version] [--atom]
+                [--base-url BASE_URL] [--html-entries HTML_ENTRIES]
+                [--html-url HTML_URL] [--html-title HTML_TITLE]
                 [--html-title-class HTML_TITLE_CLASS]
                 [--html-description HTML_DESCRIPTION]
-                [--html-description-class HTML_DESCRIPTION_CLASS] [--json]
+                [--html-description-class HTML_DESCRIPTION_CLASS]
                 [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
                 [--json-title JSON_TITLE]
                 [--json-description JSON_DESCRIPTION] [--output OUTPUT]
-                [--title TITLE] [-q] [--list] [--stdout]
+                [--title TITLE] [-q] [--stdout]
                 url
 
 Generate RSS feed for blog that don't publish a feed. Default is to find links
 in a simple <ul>-list. Options are available to find links in other HTML
 elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
+  --html                Find entries in HTML
+  --json                Find entries in JSON
+  --list                Find entries in HTML <ul>-list (default)
   --version             show program's version number and exit
   --atom                Generate Atom feed
   --base-url BASE_URL   Base URL for the blog
-  --html                Find entries in HTML
   --html-entries HTML_ENTRIES
                         HTML selector for entries
   --html-url HTML_URL   HTML selector for URL
   --html-title HTML_TITLE
                         HTML selector for title
   --html-title-class HTML_TITLE_CLASS
                         Flag to specify title class (regex)
   --html-description HTML_DESCRIPTION
                         HTML selector for description
   --html-description-class HTML_DESCRIPTION_CLASS
                         Flag to specify description class (regex)
-  --json                Find entries in JSON
   --json-entries JSON_ENTRIES
                         JSON key for entries (default: 'entries')
   --json-url JSON_URL   JSON key for URL (default: 'url')
   --json-title JSON_TITLE
                         JSON key for title
   --json-description JSON_DESCRIPTION
                         JSON key for description
   --output OUTPUT       Name of the output file
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
-  --list                Find entries in HTML <ul>-list (default)
   --stdout              Print to stdout
 ```
 
 <!-- OUTPUT:END -->
 
 ## Command-line examples for some blogs
 
@@ -167,20 +172,14 @@
 ```
 
 ### nccgroup
 
 Url: [https://research.nccgroup.com/][ncc]
 
 ```bash
-rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com
-```
-
-or you can specify _--list__ to find the links in a list which is the default:
-
-```bash
 rssfixer --title nccgroup --output nccgroup.xml --quiet --list https://research.nccgroup.com
 ```
 
 ### Tripwire
 
 Url: [https://www.tripwire.com/state-of-security][tri]
```

### Comparing `rssfixer-0.1.0/README.md` & `rssfixer-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # rssfixer
 
-[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
-![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
-[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
-[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 <!-- CODE:BASH:START -->
+<!-- echo '[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)' -->
+<!-- echo '![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)' -->
+<!-- echo '[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)' -->
+<!-- echo '[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)' -->
 <!-- if jq '.metrics._totals | ."SEVERITY.HIGH"' resources/bandit.json | grep -vE '^0' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-red.svg)](https://github.com/PyCQA/bandit)' ; elif jq '.metrics._totals' resources/bandit.json | grep "SEVERITY" | grep -E ' 0,' | wc -l | grep -vE '4$' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)'; else echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)' ;fi -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
+![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
+[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 [![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 <!-- OUTPUT:END -->
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
@@ -76,62 +80,62 @@
 <!-- rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html]
-                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
-                [--html-title HTML_TITLE]
+usage: rssfixer [-h] (--html | --json | --list) [--version] [--atom]
+                [--base-url BASE_URL] [--html-entries HTML_ENTRIES]
+                [--html-url HTML_URL] [--html-title HTML_TITLE]
                 [--html-title-class HTML_TITLE_CLASS]
                 [--html-description HTML_DESCRIPTION]
-                [--html-description-class HTML_DESCRIPTION_CLASS] [--json]
+                [--html-description-class HTML_DESCRIPTION_CLASS]
                 [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
                 [--json-title JSON_TITLE]
                 [--json-description JSON_DESCRIPTION] [--output OUTPUT]
-                [--title TITLE] [-q] [--list] [--stdout]
+                [--title TITLE] [-q] [--stdout]
                 url
 
 Generate RSS feed for blog that don't publish a feed. Default is to find links
 in a simple <ul>-list. Options are available to find links in other HTML
 elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
+  --html                Find entries in HTML
+  --json                Find entries in JSON
+  --list                Find entries in HTML <ul>-list (default)
   --version             show program's version number and exit
   --atom                Generate Atom feed
   --base-url BASE_URL   Base URL for the blog
-  --html                Find entries in HTML
   --html-entries HTML_ENTRIES
                         HTML selector for entries
   --html-url HTML_URL   HTML selector for URL
   --html-title HTML_TITLE
                         HTML selector for title
   --html-title-class HTML_TITLE_CLASS
                         Flag to specify title class (regex)
   --html-description HTML_DESCRIPTION
                         HTML selector for description
   --html-description-class HTML_DESCRIPTION_CLASS
                         Flag to specify description class (regex)
-  --json                Find entries in JSON
   --json-entries JSON_ENTRIES
                         JSON key for entries (default: 'entries')
   --json-url JSON_URL   JSON key for URL (default: 'url')
   --json-title JSON_TITLE
                         JSON key for title
   --json-description JSON_DESCRIPTION
                         JSON key for description
   --output OUTPUT       Name of the output file
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
-  --list                Find entries in HTML <ul>-list (default)
   --stdout              Print to stdout
 ```
 
 <!-- OUTPUT:END -->
 
 ## Command-line examples for some blogs
 
@@ -144,20 +148,14 @@
 ```
 
 ### nccgroup
 
 Url: [https://research.nccgroup.com/][ncc]
 
 ```bash
-rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com
-```
-
-or you can specify _--list__ to find the links in a list which is the default:
-
-```bash
 rssfixer --title nccgroup --output nccgroup.xml --quiet --list https://research.nccgroup.com
 ```
 
 ### Tripwire
 
 Url: [https://www.tripwire.com/state-of-security][tri]
```

### Comparing `rssfixer-0.1.0/pyproject.toml` & `rssfixer-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rssfixer"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
 description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -28,14 +28,15 @@
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
 audit = ["bandit"]
 build = ["build", "twine"]
 lint = ["pylint", "black", "flake8", "isort"]
 test = ["pytest", "requests-mock", "coverage"]
+github = ["coverage-badge", "markdown-code-runner"]
 dev = ["rssfixer[audit, lint, test, build]"]
 
 [project.urls]
 "Homepage" = "https://github.com/reuteras/rssfixer"
 "Bug Tracker" = "https://github.com/reuteras/rssfixer/issues"
 
 [project.scripts]
```

### Comparing `rssfixer-0.1.0/src/rssfixer/rss.py` & `rssfixer-0.1.1/src/rssfixer/rss.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,39 +11,55 @@
 
 try:
     __version__ = importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     __version__ = "0.0.0"
 
 
+class CheckHtmlAction(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        if not namespace.html:
+            parser.error(f"{option_string} requires --html to be specified.")
+        setattr(namespace, self.dest, values)
+
+
+class CheckJsonAction(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        if not namespace.json:
+            parser.error(f"{option_string} requires --json to be specified.")
+        setattr(namespace, self.dest, values)
+
+
 def fetch_html(url):
     """Fetch HTML content from a URL."""
     try:
         response = requests.get(url, timeout=10)
     except requests.exceptions.Timeout:  # pragma: no cover
         print("ERROR: Request timed out")
         sys.exit(1)
+    except requests.exceptions.ConnectionError:  # pragma: no cover
+        print("ERROR: Unable to connect to server")
+        sys.exit(1)
     return response.text
 
 
 def find_entries(json_object, entries_key):
     """Find the entries in a JSON object with key "entries_key"."""
     if isinstance(json_object, dict):
         for key, value in json_object.items():
             if key == entries_key:
                 return value
-            else:
-                result = find_entries(value, entries_key)
-                if result is not None:
-                    return result
+            result = find_entries(value, entries_key)
+            if result is not None:
+                return result
     elif isinstance(json_object, list):
         for item in json_object:
             result = find_entries(item, entries_key)
             if result is not None:
-                return result  # pragma: no cover
+                return result
     return None
 
 
 def extract_links_ul(soup):
     """Extract links from an HTML page with links in <ul>-lists."""
     links = []
     unique_links = set()
@@ -60,15 +76,15 @@
                 # Exclude URLs containing "/category/" or "/author/"
                 if "/category/" not in url and "/author/" not in url:
                     # Check if the URL is unique
                     if url not in unique_links:
                         unique_links.add(url)
                         links.append((url, title, description))
 
-    if not links:  # pragma: no cover
+    if not links:
         print("ERROR: No links found")
         sys.exit(1)
     return links
 
 
 def extract_links_html(soup, arguments):
     """Extract links from an HTML page with links in selectable elements."""
@@ -78,70 +94,68 @@
     # Iterate through all the elements of type html_entries in the page
     for entry in soup.find_all(arguments.html_entries):
         try:
             url = entry.findNext(arguments.html_url)["href"]
             title = entry.find(
                 arguments.html_title, re.compile(arguments.html_title_class)
             ).text.strip()
-        except (KeyError, AttributeError):  # pragma: no cover
+        except (KeyError, AttributeError):
             print("ERROR: Unable to find URL or title in HTML element")
             sys.exit(1)
         try:
             description = entry.find(
                 arguments.html_description, re.compile(arguments.html_description_class)
             ).text.strip()
-        except (KeyError, AttributeError):  # pragma: no cover
+        except (KeyError, AttributeError):
             # Ignore description if it's not found
             description = ""
         if url not in unique_links:
             unique_links.add(url)
             links.append((url, title, description))
 
-    if not links:  # pragma: no cover
+    if not links:
         print("ERROR: No links found")
         sys.exit(1)
     return links
 
 
 def extract_links_json(soup, arguments):
     """Extract links from JSON strings in an HTML page."""
+    entries = None
     links = []
     unique_links = set()
 
     # Find the JSON string in the page
     for json_text in soup.find_all("script", type="application/json"):
         json_object = json.loads(json_text.text)
         entries = find_entries(json_object, arguments.json_entries)
         if entries is not None:
             break
 
-    if entries is None:  # pragma: no cover
+    if entries is None:
         print("ERROR: Unable to find JSON object")
         sys.exit(1)
 
     # Extract the links from the JSON object
     for entry in entries:
         try:
             url = entry[arguments.json_url]
             title = entry[arguments.json_title]
-        except KeyError:  # pragma: no cover
+        except KeyError:
             print("ERROR: Unable to find URL or title in JSON object")
             sys.exit(1)
         try:
             description = entry[arguments.json_description]
         except KeyError:
             # Ignore description if it's not found
             description = ""
         if url not in unique_links:
             unique_links.add(url)
             links.append((url, title, description))
 
-    if links == []:  # pragma: no cover
-        print("ERROR: No links found")
-        sys.exit(1)
     return links
 
 
 def create_rss_feed(links, arguments):
     """Create an RSS feed from a list of links."""
     feed_description = f"RSS feed generated from the links at {arguments.url}"
 
@@ -160,87 +174,108 @@
         fe.id(url)
         fe.title(title)
         fe.link(href=url)
         fe.description(description)
 
     if vars(arguments).get("atom", False):
         return fg.atom_str(pretty=True).decode("utf-8")
-    else:
-        return fg.rss_str(pretty=True).decode("utf-8")
+    return fg.rss_str(pretty=True).decode("utf-8")
 
 
 def parse_arguments(arguments):
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         description="""Generate RSS feed for blog that don't publish a feed.
         Default is to find links in a simple <ul>-list.
         Options are available to find links in other HTML elements or JSON strings."""
     )
+
+    group = parser.add_mutually_exclusive_group(required=True)
+    group.add_argument("--html", action="store_true", help="Find entries in HTML")
+    group.add_argument("--json", action="store_true", help="Find entries in JSON")
+    group.add_argument(
+        "--list", action="store_true", help="Find entries in HTML <ul>-list (default)"
+    )
+
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s " + __version__,
     )
     parser.add_argument("url", help="URL for the blog")
     parser.add_argument("--atom", action="store_true", help="Generate Atom feed")
     parser.add_argument("--base-url", help="Base URL for the blog")
-    parser.add_argument("--html", action="store_true", help="Find entries in HTML")
     parser.add_argument(
-        "--html-entries", default="article", help="HTML selector for entries"
+        "--html-entries",
+        action=CheckHtmlAction,
+        default="article",
+        help="HTML selector for entries",
+    )
+    parser.add_argument(
+        "--html-url", action=CheckHtmlAction, default="a", help="HTML selector for URL"
+    )
+    parser.add_argument(
+        "--html-title",
+        action=CheckHtmlAction,
+        default="h3",
+        help="HTML selector for title",
     )
-    parser.add_argument("--html-url", default="a", help="HTML selector for URL")
-    parser.add_argument("--html-title", default="h3", help="HTML selector for title")
     parser.add_argument(
         "--html-title-class",
+        action=CheckHtmlAction,
         default="title",
         help="Flag to specify title class (regex)",
     )
     parser.add_argument(
         "--html-description",
+        action=CheckHtmlAction,
         default="div",
         help="HTML selector for description",
     )
     parser.add_argument(
         "--html-description-class",
+        action=CheckHtmlAction,
         default="summary",
         help="Flag to specify description class (regex)",
     )
-    parser.add_argument("--json", action="store_true", help="Find entries in JSON")
     parser.add_argument(
         "--json-entries",
+        action=CheckJsonAction,
         default="entries",
         help="JSON key for entries (default: 'entries')",
     )
     parser.add_argument(
-        "--json-url", default="url", help="JSON key for URL (default: 'url')"
+        "--json-url",
+        action=CheckJsonAction,
+        default="url",
+        help="JSON key for URL (default: 'url')",
     )
     parser.add_argument(
         "--json-title",
+        action=CheckJsonAction,
         default="title",
         help="JSON key for title",
     )
     parser.add_argument(
         "--json-description",
+        action=CheckJsonAction,
         default="description",
         help="JSON key for description",
     )
     parser.add_argument(
         "--output",
         default="rss_feed.xml",
         help="Name of the output file",
     )
     parser.add_argument(
         "--title",
         default="My RSS Feed",
         help='Title of the RSS feed (default: "My RSS Feed")',
     )
     parser.add_argument("-q", "--quiet", action="store_true", help="Suppress output")
-    parser.add_argument(
-        "--list", action="store_true", help="Find entries in HTML <ul>-list (default)"
-    )
     parser.add_argument("--stdout", action="store_true", help="Print to stdout")
 
     return parser.parse_args(arguments)
 
 
 def save_rss_feed(rss_feed, arguments):
     """Save the RSS feed to a file."""
@@ -254,17 +289,20 @@
     if not arguments.quiet:
         if arguments.atom:
             print(f"Atom feed created: {arguments.output}")
         else:
             print(f"RSS feed created: {arguments.output}")
 
 
-def main():
+def main(args=None):
     """Main function."""
-    args = parse_arguments(sys.argv[1:])
+    if args is None:
+        args = sys.argv[1:]
+
+    args = parse_arguments(args)
 
     if vars(args).get("version"):
         print(__version__)
         sys.exit(0)
 
     # Get HTML content from URL
     html_content = fetch_html(args.url)
@@ -284,9 +322,14 @@
     rss_feed = create_rss_feed(links, args)
     if args.stdout:
         print(rss_feed)
     else:
         save_rss_feed(rss_feed, args)
 
 
-if __name__ == "__main__":
-    main()  # pragma: no cover
+def init():
+    """Initialize the script."""
+    if __name__ == "__main__":
+        sys.exit(main())
+
+
+init()
```

### Comparing `rssfixer-0.1.0/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.1.1/src/rssfixer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,28 +14,33 @@
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: audit
 Provides-Extra: build
 Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: github
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
-[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
-![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
-[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
-[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 <!-- CODE:BASH:START -->
+<!-- echo '[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)' -->
+<!-- echo '![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)' -->
+<!-- echo '[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)' -->
+<!-- echo '[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)' -->
 <!-- if jq '.metrics._totals | ."SEVERITY.HIGH"' resources/bandit.json | grep -vE '^0' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-red.svg)](https://github.com/PyCQA/bandit)' ; elif jq '.metrics._totals' resources/bandit.json | grep "SEVERITY" | grep -E ' 0,' | wc -l | grep -vE '4$' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)'; else echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)' ;fi -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
+![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
+[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 [![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 <!-- OUTPUT:END -->
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
@@ -99,62 +104,62 @@
 <!-- rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html]
-                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
-                [--html-title HTML_TITLE]
+usage: rssfixer [-h] (--html | --json | --list) [--version] [--atom]
+                [--base-url BASE_URL] [--html-entries HTML_ENTRIES]
+                [--html-url HTML_URL] [--html-title HTML_TITLE]
                 [--html-title-class HTML_TITLE_CLASS]
                 [--html-description HTML_DESCRIPTION]
-                [--html-description-class HTML_DESCRIPTION_CLASS] [--json]
+                [--html-description-class HTML_DESCRIPTION_CLASS]
                 [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
                 [--json-title JSON_TITLE]
                 [--json-description JSON_DESCRIPTION] [--output OUTPUT]
-                [--title TITLE] [-q] [--list] [--stdout]
+                [--title TITLE] [-q] [--stdout]
                 url
 
 Generate RSS feed for blog that don't publish a feed. Default is to find links
 in a simple <ul>-list. Options are available to find links in other HTML
 elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
+  --html                Find entries in HTML
+  --json                Find entries in JSON
+  --list                Find entries in HTML <ul>-list (default)
   --version             show program's version number and exit
   --atom                Generate Atom feed
   --base-url BASE_URL   Base URL for the blog
-  --html                Find entries in HTML
   --html-entries HTML_ENTRIES
                         HTML selector for entries
   --html-url HTML_URL   HTML selector for URL
   --html-title HTML_TITLE
                         HTML selector for title
   --html-title-class HTML_TITLE_CLASS
                         Flag to specify title class (regex)
   --html-description HTML_DESCRIPTION
                         HTML selector for description
   --html-description-class HTML_DESCRIPTION_CLASS
                         Flag to specify description class (regex)
-  --json                Find entries in JSON
   --json-entries JSON_ENTRIES
                         JSON key for entries (default: 'entries')
   --json-url JSON_URL   JSON key for URL (default: 'url')
   --json-title JSON_TITLE
                         JSON key for title
   --json-description JSON_DESCRIPTION
                         JSON key for description
   --output OUTPUT       Name of the output file
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
-  --list                Find entries in HTML <ul>-list (default)
   --stdout              Print to stdout
 ```
 
 <!-- OUTPUT:END -->
 
 ## Command-line examples for some blogs
 
@@ -167,20 +172,14 @@
 ```
 
 ### nccgroup
 
 Url: [https://research.nccgroup.com/][ncc]
 
 ```bash
-rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com
-```
-
-or you can specify _--list__ to find the links in a list which is the default:
-
-```bash
 rssfixer --title nccgroup --output nccgroup.xml --quiet --list https://research.nccgroup.com
 ```
 
 ### Tripwire
 
 Url: [https://www.tripwire.com/state-of-security][tri]
```

