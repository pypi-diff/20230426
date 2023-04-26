# Comparing `tmp/rssfixer-0.1.1.tar.gz` & `tmp/rssfixer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.1.1.tar", last modified: Wed Apr 26 11:15:08 2023, max compression
+gzip compressed data, was "rssfixer-0.1.2.tar", last modified: Wed Apr 26 18:22:47 2023, max compression
```

## Comparing `rssfixer-0.1.1.tar` & `rssfixer-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.524610 rssfixer-0.1.1/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.1/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     8201 2023-04-26 11:15:08.524389 rssfixer-0.1.1/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     7375 2023-04-25 13:13:18.000000 rssfixer-0.1.1/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-26 11:14:21.000000 rssfixer-0.1.1/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-26 11:15:08.524672 rssfixer-0.1.1/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.520047 rssfixer-0.1.1/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.521592 rssfixer-0.1.1/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.1/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)    10391 2023-04-26 10:13:53.000000 rssfixer-0.1.1/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.522807 rssfixer-0.1.1/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     8201 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      371 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-26 11:15:08.000000 rssfixer-0.1.1/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 11:15:08.523883 rssfixer-0.1.1/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-26 04:26:11.000000 rssfixer-0.1.1/src/tests/test_rss.py
--rw-r--r--   0 reuteras   (501) staff       (20)     2535 2023-04-26 10:13:53.000000 rssfixer-0.1.1/src/tests/test_rss_args.py
--rw-r--r--   0 reuteras   (501) staff       (20)     2098 2023-04-26 10:13:53.000000 rssfixer-0.1.1/src/tests/test_rss_main.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.494967 rssfixer-0.1.2/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.2/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:22:47.494778 rssfixer-0.1.2/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     8682 2023-04-26 18:07:49.000000 rssfixer-0.1.2/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-26 18:21:32.000000 rssfixer-0.1.2/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-26 18:22:47.495013 rssfixer-0.1.2/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.491680 rssfixer-0.1.2/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.493028 rssfixer-0.1.2/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.2/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)    12431 2023-04-26 18:06:57.000000 rssfixer-0.1.2/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.494007 rssfixer-0.1.2/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      371 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.494548 rssfixer-0.1.2/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-26 16:32:08.000000 rssfixer-0.1.2/src/tests/test_rss.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     4141 2023-04-26 18:16:41.000000 rssfixer-0.1.2/src/tests/test_rss_args.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     1980 2023-04-26 16:34:02.000000 rssfixer-0.1.2/src/tests/test_rss_main.py
```

### Comparing `rssfixer-0.1.1/LICENSE` & `rssfixer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.1/PKG-INFO` & `rssfixer-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: rssfixer
-Version: 0.1.1
-Summary: Generate RSS feed for Wordpress blog without it.
-Author-email: Peter Reuterås <peter@reuteras.net>
-Project-URL: Homepage, https://github.com/reuteras/rssfixer
-Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Information Technology
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: audit
-Provides-Extra: build
-Provides-Extra: lint
-Provides-Extra: test
-Provides-Extra: github
-Provides-Extra: dev
-License-File: LICENSE
-
 # rssfixer
 
 <!-- CODE:BASH:START -->
 <!-- echo '[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)' -->
 <!-- echo '![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)' -->
 <!-- echo '[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)' -->
 <!-- echo '[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)' -->
@@ -52,15 +28,15 @@
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
 ### Simple list
 
-An example to generate a feed for [nccgroup][ncc] that have the links in a list:
+An example to generate a feed for [nccgroup][ncc] that have the links in a simple ul-list:
 
 ```bash
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
 
 You can specify a filename and silence output:
@@ -75,46 +51,59 @@
 
 ```bash
 32 * * * *      /home/user/src/rssfixer/bin/rssfixer --title nccgroup --output /var/www/html/feeds/nccgroup.xml --quiet https://research.nccgroup.com
 ```
 
 ### JSON
 
+Some blogs like [truesec.com][tru] have the links in a JSON object. You can use the `--json` option to parse the JSON object and generate a feed. The same is true for Apple's [security blog][app] page.
+
 An example for [truesec.com][tru]:
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
 ### General HTML
 
+Pages with a more general HTML structure can be parsed with the `--html` option. You can specify the HTML tag for the entries, the URL to the page and the title of the feed.
+
 An example for [tripwire.com][tri]:
 
 ```bash
 rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
 
 ```
 
+### Release
+
+Check for one entity on release pages like SQLite (h3) and generate RSS feed with links to the download page (required argument `--release-url`). Easy way to get notified when a new version is released.
+
+```bash
+rssfixer --release --output sqlite.xml --release-entries h3 --release-url https://sqlite.org/download.html https://sqlite.org/changes.html
+```
 
 ### Usage
 
 Command-line options:
 
 <!-- CODE:BASH:START -->
 <!-- echo '```Text' -->
 <!-- rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] (--html | --json | --list) [--version] [--atom]
-                [--base-url BASE_URL] [--html-entries HTML_ENTRIES]
-                [--html-url HTML_URL] [--html-title HTML_TITLE]
+usage: rssfixer [-h] (--html | --json | --list | --release) [--version]
+                [--atom] [--base-url BASE_URL] [--release-url RELEASE_URL]
+                [--release-entries RELEASE_ENTRIES]
+                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
+                [--html-title HTML_TITLE]
                 [--html-title-class HTML_TITLE_CLASS]
                 [--html-description HTML_DESCRIPTION]
                 [--html-description-class HTML_DESCRIPTION_CLASS]
                 [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
                 [--json-title JSON_TITLE]
                 [--json-description JSON_DESCRIPTION] [--output OUTPUT]
                 [--title TITLE] [-q] [--stdout]
@@ -128,17 +117,22 @@
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --html                Find entries in HTML
   --json                Find entries in JSON
   --list                Find entries in HTML <ul>-list (default)
+  --release             Find releases in HTML
   --version             show program's version number and exit
   --atom                Generate Atom feed
   --base-url BASE_URL   Base URL for the blog
+  --release-url RELEASE_URL
+                        Release URL for downloads
+  --release-entries RELEASE_ENTRIES
+                        Release selector for entries
   --html-entries HTML_ENTRIES
                         HTML selector for entries
   --html-url HTML_URL   HTML selector for URL
   --html-title HTML_TITLE
                         HTML selector for title
   --html-title-class HTML_TITLE_CLASS
                         Flag to specify title class (regex)
@@ -191,21 +185,30 @@
 
 Url: [https://www.truesec.com/hub/blog][tru]
 
 ```bash
 rssfixer --title Truesec --output truesec.xml --quiet --json --json-description preamble https://www.truesec.com/hub/blog
 ```
 
+### Sqlite
+
+Url: [https://sqlite.org/changes.html][sql]
+
+```bash
+rssfixer --release --release-entries h3 --release-url https://sqlite.org/download.html https://sqlite.org/changes.html
+```
+
 ## Setup blogs
 
 During testing it is useful to use --stdout to see the generated feed.
 
 
   [app]: https://security.apple.com/blog/
   [bso]: https://www.crummy.com/software/BeautifulSoup/
   [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
   [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
+  [sql]: https://sqlite.org/changes.html
   [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

### Comparing `rssfixer-0.1.1/README.md` & `rssfixer-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: rssfixer
+Version: 0.1.2
+Summary: Generate RSS feed for Wordpress blog without it.
+Author-email: Peter Reuterås <peter@reuteras.net>
+Project-URL: Homepage, https://github.com/reuteras/rssfixer
+Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Information Technology
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: audit
+Provides-Extra: build
+Provides-Extra: lint
+Provides-Extra: test
+Provides-Extra: github
+Provides-Extra: dev
+License-File: LICENSE
+
 # rssfixer
 
 <!-- CODE:BASH:START -->
 <!-- echo '[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)' -->
 <!-- echo '![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)' -->
 <!-- echo '[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)' -->
 <!-- echo '[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)' -->
@@ -28,15 +52,15 @@
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
 ### Simple list
 
-An example to generate a feed for [nccgroup][ncc] that have the links in a list:
+An example to generate a feed for [nccgroup][ncc] that have the links in a simple ul-list:
 
 ```bash
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
 
 You can specify a filename and silence output:
@@ -51,46 +75,59 @@
 
 ```bash
 32 * * * *      /home/user/src/rssfixer/bin/rssfixer --title nccgroup --output /var/www/html/feeds/nccgroup.xml --quiet https://research.nccgroup.com
 ```
 
 ### JSON
 
+Some blogs like [truesec.com][tru] have the links in a JSON object. You can use the `--json` option to parse the JSON object and generate a feed. The same is true for Apple's [security blog][app] page.
+
 An example for [truesec.com][tru]:
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
 ### General HTML
 
+Pages with a more general HTML structure can be parsed with the `--html` option. You can specify the HTML tag for the entries, the URL to the page and the title of the feed.
+
 An example for [tripwire.com][tri]:
 
 ```bash
 rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
 
 ```
 
+### Release
+
+Check for one entity on release pages like SQLite (h3) and generate RSS feed with links to the download page (required argument `--release-url`). Easy way to get notified when a new version is released.
+
+```bash
+rssfixer --release --output sqlite.xml --release-entries h3 --release-url https://sqlite.org/download.html https://sqlite.org/changes.html
+```
 
 ### Usage
 
 Command-line options:
 
 <!-- CODE:BASH:START -->
 <!-- echo '```Text' -->
 <!-- rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] (--html | --json | --list) [--version] [--atom]
-                [--base-url BASE_URL] [--html-entries HTML_ENTRIES]
-                [--html-url HTML_URL] [--html-title HTML_TITLE]
+usage: rssfixer [-h] (--html | --json | --list | --release) [--version]
+                [--atom] [--base-url BASE_URL] [--release-url RELEASE_URL]
+                [--release-entries RELEASE_ENTRIES]
+                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
+                [--html-title HTML_TITLE]
                 [--html-title-class HTML_TITLE_CLASS]
                 [--html-description HTML_DESCRIPTION]
                 [--html-description-class HTML_DESCRIPTION_CLASS]
                 [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
                 [--json-title JSON_TITLE]
                 [--json-description JSON_DESCRIPTION] [--output OUTPUT]
                 [--title TITLE] [-q] [--stdout]
@@ -104,17 +141,22 @@
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --html                Find entries in HTML
   --json                Find entries in JSON
   --list                Find entries in HTML <ul>-list (default)
+  --release             Find releases in HTML
   --version             show program's version number and exit
   --atom                Generate Atom feed
   --base-url BASE_URL   Base URL for the blog
+  --release-url RELEASE_URL
+                        Release URL for downloads
+  --release-entries RELEASE_ENTRIES
+                        Release selector for entries
   --html-entries HTML_ENTRIES
                         HTML selector for entries
   --html-url HTML_URL   HTML selector for URL
   --html-title HTML_TITLE
                         HTML selector for title
   --html-title-class HTML_TITLE_CLASS
                         Flag to specify title class (regex)
@@ -167,21 +209,30 @@
 
 Url: [https://www.truesec.com/hub/blog][tru]
 
 ```bash
 rssfixer --title Truesec --output truesec.xml --quiet --json --json-description preamble https://www.truesec.com/hub/blog
 ```
 
+### Sqlite
+
+Url: [https://sqlite.org/changes.html][sql]
+
+```bash
+rssfixer --release --release-entries h3 --release-url https://sqlite.org/download.html https://sqlite.org/changes.html
+```
+
 ## Setup blogs
 
 During testing it is useful to use --stdout to see the generated feed.
 
 
   [app]: https://security.apple.com/blog/
   [bso]: https://www.crummy.com/software/BeautifulSoup/
   [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
   [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
+  [sql]: https://sqlite.org/changes.html
   [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

### Comparing `rssfixer-0.1.1/pyproject.toml` & `rssfixer-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rssfixer"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
 description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `rssfixer-0.1.1/src/rssfixer/rss.py` & `rssfixer-0.1.2/src/rssfixer/rss.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,28 @@
 class CheckJsonAction(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         if not namespace.json:
             parser.error(f"{option_string} requires --json to be specified.")
         setattr(namespace, self.dest, values)
 
 
+class CheckListAction(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        if not namespace.list:
+            parser.error(f"{option_string} requires --list to be specified.")
+        setattr(namespace, self.dest, values)
+
+
+class CheckReleaseAction(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        if not namespace.release:
+            parser.error(f"{option_string} requires --release to be specified.")
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
@@ -151,14 +165,38 @@
         if url not in unique_links:
             unique_links.add(url)
             links.append((url, title, description))
 
     return links
 
 
+def extract_links_release(soup, arguments):
+    """Extract links from an html page with one type of html entries."""
+    links = []
+    unique_titles = set()
+
+    # Iterate through all the elements of type html_entries in the page
+    for entry in soup.find_all(arguments.release_entries):
+        try:
+            title = entry.text.strip()
+            url = arguments.release_url
+        except (KeyError, AttributeError):
+            print("ERROR: Unable to title in HTML element")
+            sys.exit(1)
+        description = ""
+        if title not in unique_titles:
+            unique_titles.add(title)
+            links.append((url, title, description))
+
+    if not links:
+        print("ERROR: No titles found")
+        sys.exit(1)
+    return links
+
+
 def create_rss_feed(links, arguments):
     """Create an RSS feed from a list of links."""
     feed_description = f"RSS feed generated from the links at {arguments.url}"
 
     # Create the RSS feed
     fg = FeedGenerator()
     fg.id(arguments.url)
@@ -170,15 +208,19 @@
     for url, title, description in links:
         if arguments.base_url:
             url = arguments.base_url + url
         fe = fg.add_entry()
         fe.id(url)
         fe.title(title)
         fe.link(href=url)
-        fe.description(description)
+        if vars(arguments).get("atom", False):
+            fe.summary(description)
+            fe.content(content=description, src=url)
+        else:
+            fe.description(description)
 
     if vars(arguments).get("atom", False):
         return fg.atom_str(pretty=True).decode("utf-8")
     return fg.rss_str(pretty=True).decode("utf-8")
 
 
 def parse_arguments(arguments):
@@ -191,24 +233,33 @@
 
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument("--html", action="store_true", help="Find entries in HTML")
     group.add_argument("--json", action="store_true", help="Find entries in JSON")
     group.add_argument(
         "--list", action="store_true", help="Find entries in HTML <ul>-list (default)"
     )
+    group.add_argument("--release", action="store_true", help="Find releases in HTML")
 
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s " + __version__,
     )
     parser.add_argument("url", help="URL for the blog")
     parser.add_argument("--atom", action="store_true", help="Generate Atom feed")
     parser.add_argument("--base-url", help="Base URL for the blog")
     parser.add_argument(
+        "--release-url", action=CheckReleaseAction, help="Release URL for downloads"
+    )
+    parser.add_argument(
+        "--release-entries",
+        action=CheckReleaseAction,
+        help="Release selector for entries",
+    )
+    parser.add_argument(
         "--html-entries",
         action=CheckHtmlAction,
         default="article",
         help="HTML selector for entries",
     )
     parser.add_argument(
         "--html-url", action=CheckHtmlAction, default="a", help="HTML selector for URL"
@@ -311,16 +362,22 @@
     # Select function to handle different types of blogs
     if args.json:
         links = extract_links_json(soup, args)
     elif args.html:
         links = extract_links_html(soup, args)
     elif args.list:
         links = extract_links_ul(soup)
+    elif args.release:
+        if not vars(args).get("release_url", False):
+            print("ERROR: Release URL not specified")
+            sys.exit(1)
+        links = extract_links_release(soup, args)
     else:
-        links = extract_links_ul(soup)
+        print("ERROR: No valid blog type specified")
+        sys.exit(1)
 
     # Create RSS feed and save to file
     rss_feed = create_rss_feed(links, args)
     if args.stdout:
         print(rss_feed)
     else:
         save_rss_feed(rss_feed, args)
```

### Comparing `rssfixer-0.1.1/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.1.2/src/rssfixer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,15 +52,15 @@
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
 ### Simple list
 
-An example to generate a feed for [nccgroup][ncc] that have the links in a list:
+An example to generate a feed for [nccgroup][ncc] that have the links in a simple ul-list:
 
 ```bash
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
 
 You can specify a filename and silence output:
@@ -75,46 +75,59 @@
 
 ```bash
 32 * * * *      /home/user/src/rssfixer/bin/rssfixer --title nccgroup --output /var/www/html/feeds/nccgroup.xml --quiet https://research.nccgroup.com
 ```
 
 ### JSON
 
+Some blogs like [truesec.com][tru] have the links in a JSON object. You can use the `--json` option to parse the JSON object and generate a feed. The same is true for Apple's [security blog][app] page.
+
 An example for [truesec.com][tru]:
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
 ### General HTML
 
+Pages with a more general HTML structure can be parsed with the `--html` option. You can specify the HTML tag for the entries, the URL to the page and the title of the feed.
+
 An example for [tripwire.com][tri]:
 
 ```bash
 rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
 
 ```
 
+### Release
+
+Check for one entity on release pages like SQLite (h3) and generate RSS feed with links to the download page (required argument `--release-url`). Easy way to get notified when a new version is released.
+
+```bash
+rssfixer --release --output sqlite.xml --release-entries h3 --release-url https://sqlite.org/download.html https://sqlite.org/changes.html
+```
 
 ### Usage
 
 Command-line options:
 
 <!-- CODE:BASH:START -->
 <!-- echo '```Text' -->
 <!-- rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] (--html | --json | --list) [--version] [--atom]
-                [--base-url BASE_URL] [--html-entries HTML_ENTRIES]
-                [--html-url HTML_URL] [--html-title HTML_TITLE]
+usage: rssfixer [-h] (--html | --json | --list | --release) [--version]
+                [--atom] [--base-url BASE_URL] [--release-url RELEASE_URL]
+                [--release-entries RELEASE_ENTRIES]
+                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
+                [--html-title HTML_TITLE]
                 [--html-title-class HTML_TITLE_CLASS]
                 [--html-description HTML_DESCRIPTION]
                 [--html-description-class HTML_DESCRIPTION_CLASS]
                 [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
                 [--json-title JSON_TITLE]
                 [--json-description JSON_DESCRIPTION] [--output OUTPUT]
                 [--title TITLE] [-q] [--stdout]
@@ -128,17 +141,22 @@
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --html                Find entries in HTML
   --json                Find entries in JSON
   --list                Find entries in HTML <ul>-list (default)
+  --release             Find releases in HTML
   --version             show program's version number and exit
   --atom                Generate Atom feed
   --base-url BASE_URL   Base URL for the blog
+  --release-url RELEASE_URL
+                        Release URL for downloads
+  --release-entries RELEASE_ENTRIES
+                        Release selector for entries
   --html-entries HTML_ENTRIES
                         HTML selector for entries
   --html-url HTML_URL   HTML selector for URL
   --html-title HTML_TITLE
                         HTML selector for title
   --html-title-class HTML_TITLE_CLASS
                         Flag to specify title class (regex)
@@ -191,21 +209,30 @@
 
 Url: [https://www.truesec.com/hub/blog][tru]
 
 ```bash
 rssfixer --title Truesec --output truesec.xml --quiet --json --json-description preamble https://www.truesec.com/hub/blog
 ```
 
+### Sqlite
+
+Url: [https://sqlite.org/changes.html][sql]
+
+```bash
+rssfixer --release --release-entries h3 --release-url https://sqlite.org/download.html https://sqlite.org/changes.html
+```
+
 ## Setup blogs
 
 During testing it is useful to use --stdout to see the generated feed.
 
 
   [app]: https://security.apple.com/blog/
   [bso]: https://www.crummy.com/software/BeautifulSoup/
   [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
   [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
+  [sql]: https://sqlite.org/changes.html
   [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

### Comparing `rssfixer-0.1.1/src/tests/test_rss.py` & `rssfixer-0.1.2/src/tests/test_rss.py`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.1/src/tests/test_rss_args.py` & `rssfixer-0.1.2/src/tests/test_rss_args.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,14 +26,56 @@
                 "fail",
                 "http://www.tripwire.com/state-of-security",
             ]
         )
     assert pytest_wrapped_e.value.code == 2
 
 
+def test_rss_args_list_json_entries():
+    """Test rss_args function"""
+    with pytest.raises(SystemExit) as pytest_wrapped_e:
+        rss.parse_arguments(
+            [
+                "--list",
+                "--json-entries",
+                "fail",
+                "http://www.tripwire.com/state-of-security",
+            ]
+        )
+    assert pytest_wrapped_e.value.code == 2
+
+
+def test_rss_args_json_release_entries():
+    """Test rss_args function"""
+    with pytest.raises(SystemExit) as pytest_wrapped_e:
+        rss.parse_arguments(
+            [
+                "--json",
+                "--release-entries",
+                "fail",
+                "http://www.tripwire.com/state-of-security",
+            ]
+        )
+    assert pytest_wrapped_e.value.code == 2
+
+
+def test_rss_args_release_html_entries():
+    """Test rss_args function"""
+    with pytest.raises(SystemExit) as pytest_wrapped_e:
+        rss.parse_arguments(
+            [
+                "--release",
+                "--html-entries",
+                "fail",
+                "https://sqlite.org/changes.html",
+            ]
+        )
+    assert pytest_wrapped_e.value.code == 2
+
+
 def test_parse_arguments_required_args():
     arguments = ["--list", "https://example.com"]
     args = rss.parse_arguments(arguments)
     assert args.list
     assert args.url == "https://example.com"
 
 
@@ -83,10 +125,26 @@
     assert args.json_entries == "items"
     assert args.json_url == "link"
     assert args.json_title == "name"
     assert args.json_description == "summary"
     assert args.url == "https://example.com"
 
 
+def test_parse_arguments_release_args():
+    arguments = [
+        "--release",
+        "--release-entries",
+        "items",
+        "--release-url",
+        "https://example.com/download",
+        "https://example.com",
+    ]
+    args = rss.parse_arguments(arguments)
+    assert args.release
+    assert args.release_entries == "items"
+    assert args.release_url == "https://example.com/download"
+    assert args.url == "https://example.com"
+
+
 def test_parse_arguments_invalid_args():
     with pytest.raises(SystemExit):
         rss.parse_arguments(["--html", "--json", "https://example.com"])
```

### Comparing `rssfixer-0.1.1/src/tests/test_rss_main.py` & `rssfixer-0.1.2/src/tests/test_rss_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,34 +26,29 @@
         capsys.readouterr().out,
     )[:-1]
     assert captured == result
 
 
 def test_main_json(capsys, requests_mock):
     """Test the main function with json arguments."""
-    url = "https://security.apple.com/blog"
-    with open("src/tests/data/input/apple.html", "r", encoding="utf-8") as f:
+    url = "https://www.truesec.com/hub/blog"
+    with open("src/tests/data/input/truesec.html", "r", encoding="utf-8") as f:
         source = f.read()
-    with open("src/tests/data/output/apple.xml", "r", encoding="utf-8") as f:
+    with open("src/tests/data/output/truesec.xml", "r", encoding="utf-8") as f:
         result = f.read()
     requests_mock.get(url, text=source)
     arguments = [
         "--title",
-        "Apple Security",
+        "Truesec",
         "--atom",
         "--json",
-        "--json-entries",
-        "blogs",
-        "--json-url",
-        "slug",
+        "--json-description",
+        "preamble",
         "--stdout",
-        "--quiet",
-        "--base-url",
-        "https://security.apple.com/blog/",
-        "https://security.apple.com/blog",
+        "https://www.truesec.com/hub/blog",
     ]
     rss.main(arguments)
     captured = re.sub(
         r"<updated>.*</updated>",
         "<updated>TIME</updated>",
         capsys.readouterr().out,
     )[:-1]
@@ -62,12 +57,12 @@
         "<updated>TIME</updated>",
         result,
     )
     args = rss.parse_arguments(arguments)
 
     assert captured == result
     assert args.json
-    assert args.json_entries == "blogs"
-    assert args.json_url == "slug"
+    assert args.json_entries == "entries"
+    assert args.json_url == "url"
     assert args.json_title == "title"
-    assert args.json_description == "description"
-    assert args.url == "https://security.apple.com/blog"
+    assert args.json_description == "preamble"
+    assert args.url == "https://www.truesec.com/hub/blog"
```

