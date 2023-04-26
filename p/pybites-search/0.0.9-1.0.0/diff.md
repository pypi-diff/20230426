# Comparing `tmp/pybites_search-0.0.9.tar.gz` & `tmp/pybites_search-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybites_search-0.0.9.tar", last modified: Wed Apr 19 08:44:10 2023, from Unix
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pybites_search-0.0.9.tar` & `pybites_search-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/__main__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/article.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/base.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/bite.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/cli.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/podcast.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/tip.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pybites_search-0.0.9/src/pybites_search/youtube.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pybites_search-0.0.9/.gitignore
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pybites_search-0.0.9/LICENSE
--rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 pybites_search-0.0.9/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pybites_search-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    12133 2020-02-02 00:00:00.000000 pybites_search-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/__main__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/all_content.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/article.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/base.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/bite.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/cli.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/podcast.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/tip.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pybites_search-1.0.0/src/pybites_search/youtube.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 pybites_search-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pybites_search-1.0.0/LICENSE
+-rw-r--r--   0        0        0    16828 2020-02-02 00:00:00.000000 pybites_search-1.0.0/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybites_search-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17918 2020-02-02 00:00:00.000000 pybites_search-1.0.0/PKG-INFO
```

### Comparing `pybites_search-0.0.9/src/pybites_search/article.py` & `pybites_search-1.0.0/src/pybites_search/article.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import requests
-
 from .base import ContentPiece, PybitesSearch
 
 ARTICLE_ENDPOINT = "https://codechalleng.es/api/articles/"
 
 
 class ArticleSearch(PybitesSearch):
+    def __init__(self) -> None:
+        self.title = "Pybites Articles"
+
     def match_content(self, search: str) -> list[ContentPiece]:
-        entries = requests.get(ARTICLE_ENDPOINT, timeout=5).json()
+        entries = self.get_data(ARTICLE_ENDPOINT)
         results = []
         for entry in entries:
             if search.lower() in (entry["title"] + entry["summary"]).lower():
                 results.append(
                     ContentPiece(
-                        title=entry["title"],
-                        url=entry["link"],
+                        title=entry["title"], url=entry["link"], channel=self.title
                     )
                 )
         return results
 
 
 if __name__ == "__main__":
     searcher = ArticleSearch()
```

### Comparing `pybites_search-0.0.9/src/pybites_search/bite.py` & `pybites_search-1.0.0/src/pybites_search/bite.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import requests
-
 from .base import ContentPiece, PybitesSearch
 
 BITES_ENDPOINT = "https://codechalleng.es/api/bites/"
 PLATFORM_BASE_URL = "https://codechalleng.es/bites/"
 
 
 class BiteSearch(PybitesSearch):
+    def __init__(self) -> None:
+        self.title = "Pybites Bite Exercises"
+
     def match_content(self, search: str) -> list[ContentPiece]:
-        entries = requests.get(BITES_ENDPOINT, timeout=5).json()
+        entries = self.get_data(BITES_ENDPOINT)
         results = []
         for entry in entries:
             if search.lower() in (entry["title"] + entry["description"]).lower():
                 results.append(
                     ContentPiece(
                         title=entry["title"],
                         url=f"{PLATFORM_BASE_URL}{entry['number']}",
+                        channel=self.title,
                     )
                 )
         return results
 
 
 if __name__ == "__main__":
     searcher = BiteSearch()
```

### Comparing `pybites_search-0.0.9/src/pybites_search/cli.py` & `pybites_search-1.0.0/src/pybites_search/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typer
 
+from .all_content import AllSearch
 from .article import ArticleSearch
 from .bite import BiteSearch
 from .podcast import PodcastSearch
 from .tip import TipSearch
 from .youtube import YouTubeSearch
 
 app = typer.Typer()
@@ -38,7 +39,14 @@
 
 
 @app.command()
 def video(search: str):
     searcher = YouTubeSearch()
     results = searcher.match_content(search)
     searcher.show_matches(results)
+
+
+@app.command()
+def all(search: str):
+    searcher = AllSearch()
+    results = searcher.match_content(search)
+    searcher.show_matches(results)
```

### Comparing `pybites_search-0.0.9/src/pybites_search/podcast.py` & `pybites_search-1.0.0/src/pybites_search/podcast.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import requests
-
 from .base import ContentPiece, PybitesSearch
 
 PODCAST_ENDPOINT = "https://codechalleng.es/api/podcasts/"
 PODCAST_BASE_URL = "https://www.pybitespodcast.com/1501156/"
 
 
 class PodcastSearch(PybitesSearch):
+    def __init__(self) -> None:
+        self.title = "Pybites Podcast Episodes"
+
     def match_content(self, search: str) -> list[ContentPiece]:
-        entries = requests.get(PODCAST_ENDPOINT, timeout=5).json()
+        entries = self.get_data(PODCAST_ENDPOINT)
         results = []
         for entry in entries:
             if search.lower() in (entry["title"] + entry["description"]).lower():
                 results.append(
                     ContentPiece(
                         title=entry["title"],
                         url=PODCAST_BASE_URL + entry["slug"],
+                        channel=self.title,
                     )
                 )
         return results
 
 
 if __name__ == "__main__":
     searcher = PodcastSearch()
```

### Comparing `pybites_search-0.0.9/src/pybites_search/tip.py` & `pybites_search-1.0.0/src/pybites_search/tip.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import requests
-
 from .base import ContentPiece, PybitesSearch
 
 TIPS_ENDPOINT = "https://codechalleng.es/api/pytips/"
 
 
 class TipSearch(PybitesSearch):
+    def __init__(self) -> None:
+        self.title = "Pybites Python Tips"
+
     def match_content(self, search: str) -> list[ContentPiece]:
-        entries = requests.get(TIPS_ENDPOINT, timeout=5).json()
+        entries = self.get_data(TIPS_ENDPOINT)
         results = []
         for entry in entries:
             if search.lower() in (entry["title"] + entry["description"]).lower():
                 results.append(
                     ContentPiece(
-                        title=entry["title"],
-                        url=entry["link"],
+                        title=entry["title"], url=entry["link"], channel=self.title
                     )
                 )
         return results
 
 
 if __name__ == "__main__":
     searcher = TipSearch()
```

### Comparing `pybites_search-0.0.9/src/pybites_search/youtube.py` & `pybites_search-1.0.0/src/pybites_search/youtube.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import requests
-
 from .base import ContentPiece, PybitesSearch
 
 YOUTUBE_ENDPOINT = "https://codechalleng.es/api/videos/"
 YOUTUBE_BASE_URL = "https://www.youtube.com/watch?v="
 
 
 class YouTubeSearch(PybitesSearch):
+    def __init__(self) -> None:
+        self.title = "Pybites YouTube Videos"
+
     def match_content(self, search: str) -> list[ContentPiece]:
-        entries = requests.get(YOUTUBE_ENDPOINT, timeout=5).json()
+        entries = self.get_data(YOUTUBE_ENDPOINT)
         results = []
         for entry in entries:
             if search.lower() in (entry["title"] + entry["description"]).lower():
                 results.append(
                     ContentPiece(
                         title=entry["title"],
                         url=YOUTUBE_BASE_URL + entry["video_id"],
+                        channel=self.title,
                     )
                 )
         return results
 
 
 if __name__ == "__main__":
     searcher = YouTubeSearch()
```

### Comparing `pybites_search-0.0.9/.gitignore` & `pybites_search-1.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -155,7 +155,11 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+*.sqlite
+# isort configuration
+.isort.cfg
```

### Comparing `pybites_search-0.0.9/LICENSE` & `pybites_search-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybites_search-0.0.9/pyproject.toml` & `pybites_search-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pybites_search"
-version = "0.0.9"
+version = "1.0.0"
 authors = [
   { name="Pybites", email="info@pybit.es" },
 ]
 description = "A search engine for Pybites content"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+  "python-decouple",
   "requests",
+  "requests-cache",
   "typer[all]",
 ]
 
 [project.optional-dependencies]
 test = [
   "tox",
   "pytest",
   "pytest-cov",
-  "strip_ansi",
 ]
-lint = [
+tools = [
   "flake8",
   "black",
   "isort",
   "pyupgrade",
   "mypy",
+  "pre-commit",
+  "build",
+  "twine",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pybites/search"
 "Bug Tracker" = "https://github.com/pybites/search/issues"
 
 [project.scripts]
```

### Comparing `pybites_search-0.0.9/PKG-INFO` & `pybites_search-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,15 @@
-Metadata-Version: 2.1
-Name: pybites_search
-Version: 0.0.9
-Summary: A search engine for Pybites content
-Project-URL: Homepage, https://github.com/pybites/search
-Project-URL: Bug Tracker, https://github.com/pybites/search/issues
-Author-email: Pybites <info@pybit.es>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Requires-Dist: requests
-Requires-Dist: typer[all]
-Provides-Extra: lint
-Requires-Dist: black; extra == 'lint'
-Requires-Dist: flake8; extra == 'lint'
-Requires-Dist: isort; extra == 'lint'
-Requires-Dist: mypy; extra == 'lint'
-Requires-Dist: pyupgrade; extra == 'lint'
-Provides-Extra: test
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
-Requires-Dist: strip-ansi; extra == 'test'
-Requires-Dist: tox; extra == 'test'
-Description-Content-Type: text/markdown
-
 # Pybites Search
 
 A command line tool to easily search across Pybites content.
 
 ## Installation
 
+`pybites-search` is hosted on PyPI and you can install it in a virtual environment like this:
+
 ```
 $ pip install pybites-search
 ```
 
 ## How to run it:
 
 ```
@@ -44,14 +19,15 @@
 
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --install-completion          Install completion for the current shell.                                                                                     │
 │ --show-completion             Show completion for the current shell, to copy it or customize the installation.                                              │
 │ --help                        Show this message and exit.                                                                                                   │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ all                                                                                                                                                         │
 │ article                                                                                                                                                     │
 │ bite                                                                                                                                                        │
 │ podcast                                                                                                                                                     │
 │ tip                                                                                                                                                         │
 │ video                                                                                                                                                       │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
@@ -98,22 +74,76 @@
 
 $ search video property
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
 ┃ Title                                ┃ Url                                         ┃
 ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
 │ Python @property decorator explained │ https://www.youtube.com/watch?v=8BbngXWouzo │
 └──────────────────────────────────────┴─────────────────────────────────────────────┘
+
+# and to search across all content channels:
+
+$ search all decouple
+                                                                           Pybites All Content
+┌────────────────────────────────────────────────────────────────────┬───────────────────────────────────────────────────────────────────────────────────────────────────┐
+│ Pybites Podcast Episodes                                           │ Url                                                                                               │
+├────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────────────────────────────────────────┤
+│ #025 - Building Dreams with Python - The AskAGuru Story            │ https://www.pybitespodcast.com/1501156/8476666-025-building-dreams-with-python-the-askaguru-story │
+├────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────────────────────────────────────────┤
+│ Pybites Python Tips                                                │ Url                                                                                               │
+├────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────────────────────────────────────────┤
+│ configuration variables                                            │ https://codechalleng.es/tips/configuration-variables                                              │
+├────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────────────────────────────────────────┤
+│ Pybites YouTube Videos                                             │ Url                                                                                               │
+├────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────────────────────────────────────────┤
+│ How to manage environment variables in Django with python-decouple │ https://www.youtube.com/watch?v=LkyhTqDrSxA                                                       │
+└────────────────────────────────────────────────────────────────────┴───────────────────────────────────────────────────────────────────────────────────────────────────┘
 ```
 
+## Caching
+
+By default any requests calls to the different Pybites API endpoints are cached for 24 hours, you can change that setting the `CACHE_EXPIRATION_SECONDS` environment variable.
+
 ## Changelog
 
-| Version | Features                                    |
-| ------- | ------------------------------------------- |
-| 0.0.1   | Initial package creation on PDM code clinic |
-| 0.0.2   | ditto                                       |
-| 0.0.3   | ditto                                       |
-| 0.0.4   | Add Pybites Youtube search                  |
-| 0.0.5   | Add platform Bite (exercise) search         |
-| 0.0.6   | Add Pybites Podcast search                  |
-| 0.0.7   | Add Pybites tips search                     |
-| 0.0.8   | Move podcast feed parsing to our platform   |
-| 0.0.9   | Add tox + testing to support 3.9 + 3.10     |
+Check out the changelog [here](CHANGELOG.md)
+
+## Developer setup instructions
+
+To do dev work on this repo:
+
+1. Check out the repo and make a virtual environment and activate it:
+
+```
+# original repo or make a fork and clone that if you want to contribute
+
+$ git clone git@github.com:PyBites-Open-Source/search.git
+
+$ cd search
+√ search (main) $ python3 -m venv venv && source venv/bin/activate
+
+# for Windows this would be something like:
+py -3 -m venv venv && venv\scripts\activate
+```
+
+2. Install the regular + test + tooling dependencies:
+
+```
+(venv) √ search (main) $ python -m pip install .
+(venv) √ search (main) $ python -m pip install ".[test,tools]"
+```
+
+3. Use the tool / run the tests
+
+```
+(venv) √ search (main) $ search ...
+...
+
+(venv) √ search (main) $ tox
+...
+...
+  py39: OK (15.89=setup[14.49]+cmd[1.40] seconds)
+  py310: OK (13.22=setup[11.80]+cmd[1.42] seconds)
+  py311: OK (10.42=setup[9.41]+cmd[1.01] seconds)
+  congratulations :) (39.61 seconds)
+```
+
+4. Code, have fun, contribute ... 💪 🙏
```

