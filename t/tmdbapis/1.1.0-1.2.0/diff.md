# Comparing `tmp/tmdbapis-1.1.0.tar.gz` & `tmp/tmdbapis-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmdbapis-1.1.0.tar", last modified: Wed Jan  4 23:41:15 2023, max compression
+gzip compressed data, was "tmdbapis-1.2.0.tar", last modified: Tue Apr 25 18:26:46 2023, max compression
```

## Comparing `tmdbapis-1.1.0.tar` & `tmdbapis-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:41:15.018243 tmdbapis-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-01-04 23:41:15.018243 tmdbapis-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-04 23:41:15.018243 tmdbapis-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:41:15.018243 tmdbapis-1.1.0/tmdbapis/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144967 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/api3.py
--rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/api4.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:41:15.018243 tmdbapis-1.1.0/tmdbapis/objs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/objs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/objs/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/objs/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    38884 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/objs/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    58673 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/objs/reload.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/objs/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    71467 2023-01-04 23:41:05.000000 tmdbapis-1.1.0/tmdbapis/tmdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 23:41:15.018243 tmdbapis-1.1.0/tmdbapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-01-04 23:41:14.000000 tmdbapis-1.1.0/tmdbapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-04 23:41:14.000000 tmdbapis-1.1.0/tmdbapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 23:41:14.000000 tmdbapis-1.1.0/tmdbapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-04 23:41:14.000000 tmdbapis-1.1.0/tmdbapis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-04 23:41:14.000000 tmdbapis-1.1.0/tmdbapis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:26:46.102053 tmdbapis-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-25 18:26:46.102053 tmdbapis-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:26:46.102053 tmdbapis-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:26:46.098053 tmdbapis-1.2.0/tmdbapis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145094 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/api3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/api4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:26:46.102053 tmdbapis-1.2.0/tmdbapis/objs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/objs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/objs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/objs/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/objs/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39209 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/objs/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58341 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/objs/reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/objs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79861 2023-04-25 18:26:22.000000 tmdbapis-1.2.0/tmdbapis/tmdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:26:46.102053 tmdbapis-1.2.0/tmdbapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-25 18:26:46.000000 tmdbapis-1.2.0/tmdbapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 18:26:46.000000 tmdbapis-1.2.0/tmdbapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:26:46.000000 tmdbapis-1.2.0/tmdbapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 18:26:46.000000 tmdbapis-1.2.0/tmdbapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 18:26:46.000000 tmdbapis-1.2.0/tmdbapis.egg-info/top_level.txt
```

### Comparing `tmdbapis-1.1.0/LICENSE` & `tmdbapis-1.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 meisnate12
+Copyright (c) 2023 meisnate12
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tmdbapis-1.1.0/PKG-INFO` & `tmdbapis-1.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-Metadata-Version: 2.1
-Name: tmdbapis
-Version: 1.1.0
-Summary: A lightweight Python library for The V3 and V4 TMDb APIs.
-Home-page: https://github.com/meisnate12/TMDbAPIs
-Author: Nathan Taggart
-Author-email: meisnate12@gmail.com
-License: MIT License
-Project-URL: Documentation, https://tmdbapis.metamanager.wiki
-Project-URL: Funding, https://github.com/sponsors/meisnate12
-Project-URL: Source, https://github.com/meisnate12/TMDbAPIs
-Project-URL: Issues, https://github.com/meisnate12/TMDbAPIs/issues
-Keywords: tmdbapis,tmdbapi,tmdb,wrapper,api
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-License-File: LICENSE
-
 Welcome to TMDbAPIs Documentation!
 ==========================================================
 
-.. image:: https://img.shields.io/readthedocs/tmdbapis?style=plastic
-    :target: https://tmdbapis.metamanager.wiki
-    :alt: Read the Docs
-
 .. image:: https://img.shields.io/github/v/release/meisnate12/TMDbAPIs?style=plastic
     :target: https://github.com/meisnate12/TMDbAPIs/releases
     :alt: GitHub release (latest by date)
 
+.. image:: https://img.shields.io/github/actions/workflow/status/meisnate12/TMDbAPIs/tests.yml?branch=master&style=plastic
+    :target: https://github.com/meisnate12/TMDbAPIs/actions/workflows/tests.yml
+    :alt: Build Testing
+
+.. image:: https://img.shields.io/codecov/c/github/meisnate12/TMDbAPIs?color=greenred&style=plastic
+    :target: https://codecov.io/gh/meisnate12/TMDbAPIs
+    :alt: Build Coverage
+
+.. image:: https://img.shields.io/github/commits-since/meisnate12/TMDbAPIs/latest?style=plastic
+    :target: https://github.com/meisnate12/TMDbAPIs/commits/master
+    :alt: GitHub commits since latest release (by date) for a branch
+
 .. image:: https://img.shields.io/pypi/v/TMDbAPIs?style=plastic
     :target: https://pypi.org/project/tmdbapis/
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/dm/tmdbapis.svg?style=plastic
     :target: https://pypi.org/project/tmdbapis/
     :alt: Downloads
 
-.. image:: https://img.shields.io/github/commits-since/meisnate12/TMDbAPIs/latest?style=plastic
-    :target: https://github.com/meisnate12/TMDbAPIs/commits/master
-    :alt: GitHub commits since latest release (by date) for a branch
+|
+
+.. image:: https://img.shields.io/readthedocs/plex-meta-manager?color=%2300bc8c&style=plastic
+    :target: https://tmdbapis.metamanager.wiki/en/latest/
+    :alt: Wiki
+
+.. image:: https://img.shields.io/discord/822460010649878528?color=%2300bc8c&label=Discord&style=plastic
+    :target: https://discord.gg/NfH6mGFuAB
+    :alt: Discord
+
+.. image:: https://img.shields.io/reddit/subreddit-subscribers/PlexMetaManager?color=%2300bc8c&label=r%2FPlexMetaManager&style=plastic
+    :target: https://www.reddit.com/r/PlexMetaManager/
+    :alt: Reddit
+
+.. image:: https://img.shields.io/github/sponsors/meisnate12?color=%238a2be2&style=plastic
+    :target: https://github.com/sponsors/meisnate12
+    :alt: GitHub Sponsors
 
 .. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
     :target: https://github.com/sponsors/meisnate12
-    :alt: GitHub Sponsor
+    :alt: Sponsor or Donate
 
 
 Overview
 ----------------------------------------------------------
 Unofficial Python bindings for the TMDb API. The goal is to make interaction with the API as easy as possible while emulating the endpoints as much as possible
```

### Comparing `tmdbapis-1.1.0/README.rst` & `tmdbapis-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,79 @@
+Metadata-Version: 2.1
+Name: tmdbapis
+Version: 1.2.0
+Summary: A lightweight Python library for The V3 and V4 TMDb APIs.
+Home-page: https://github.com/meisnate12/TMDbAPIs
+Author: Nathan Taggart
+Author-email: meisnate12@gmail.com
+License: MIT License
+Project-URL: Documentation, https://tmdbapis.metamanager.wiki
+Project-URL: Funding, https://github.com/sponsors/meisnate12
+Project-URL: Source, https://github.com/meisnate12/TMDbAPIs
+Project-URL: Issues, https://github.com/meisnate12/TMDbAPIs/issues
+Keywords: tmdbapis,tmdbapi,tmdb,wrapper,api
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+License-File: LICENSE
+
 Welcome to TMDbAPIs Documentation!
 ==========================================================
 
-.. image:: https://img.shields.io/readthedocs/tmdbapis?style=plastic
-    :target: https://tmdbapis.metamanager.wiki
-    :alt: Read the Docs
-
 .. image:: https://img.shields.io/github/v/release/meisnate12/TMDbAPIs?style=plastic
     :target: https://github.com/meisnate12/TMDbAPIs/releases
     :alt: GitHub release (latest by date)
 
+.. image:: https://img.shields.io/github/actions/workflow/status/meisnate12/TMDbAPIs/tests.yml?branch=master&style=plastic
+    :target: https://github.com/meisnate12/TMDbAPIs/actions/workflows/tests.yml
+    :alt: Build Testing
+
+.. image:: https://img.shields.io/codecov/c/github/meisnate12/TMDbAPIs?color=greenred&style=plastic
+    :target: https://codecov.io/gh/meisnate12/TMDbAPIs
+    :alt: Build Coverage
+
+.. image:: https://img.shields.io/github/commits-since/meisnate12/TMDbAPIs/latest?style=plastic
+    :target: https://github.com/meisnate12/TMDbAPIs/commits/master
+    :alt: GitHub commits since latest release (by date) for a branch
+
 .. image:: https://img.shields.io/pypi/v/TMDbAPIs?style=plastic
     :target: https://pypi.org/project/tmdbapis/
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/dm/tmdbapis.svg?style=plastic
     :target: https://pypi.org/project/tmdbapis/
     :alt: Downloads
 
-.. image:: https://img.shields.io/github/commits-since/meisnate12/TMDbAPIs/latest?style=plastic
-    :target: https://github.com/meisnate12/TMDbAPIs/commits/master
-    :alt: GitHub commits since latest release (by date) for a branch
+|
+
+.. image:: https://img.shields.io/readthedocs/plex-meta-manager?color=%2300bc8c&style=plastic
+    :target: https://tmdbapis.metamanager.wiki/en/latest/
+    :alt: Wiki
+
+.. image:: https://img.shields.io/discord/822460010649878528?color=%2300bc8c&label=Discord&style=plastic
+    :target: https://discord.gg/NfH6mGFuAB
+    :alt: Discord
+
+.. image:: https://img.shields.io/reddit/subreddit-subscribers/PlexMetaManager?color=%2300bc8c&label=r%2FPlexMetaManager&style=plastic
+    :target: https://www.reddit.com/r/PlexMetaManager/
+    :alt: Reddit
+
+.. image:: https://img.shields.io/github/sponsors/meisnate12?color=%238a2be2&style=plastic
+    :target: https://github.com/sponsors/meisnate12
+    :alt: GitHub Sponsors
 
 .. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
     :target: https://github.com/sponsors/meisnate12
-    :alt: GitHub Sponsor
+    :alt: Sponsor or Donate
 
 
 Overview
 ----------------------------------------------------------
 Unofficial Python bindings for the TMDb API. The goal is to make interaction with the API as easy as possible while emulating the endpoints as much as possible
```

### Comparing `tmdbapis-1.1.0/setup.py` & `tmdbapis-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.1.0/tmdbapis/__init__.py` & `tmdbapis-1.2.0/tmdbapis/__init__.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.1.0/tmdbapis/api3.py` & `tmdbapis-1.2.0/tmdbapis/api3.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,18 @@
         return self._request("put", path, json=json, **kwargs)
 
     def _request(self, request_type, path, json=None, **kwargs):
         """ process request. """
         url_params = {"api_key": f"{self.apikey}"}
         for key, value in kwargs.items():
             if value is not None:
-                url_params[key] = value
+                if isinstance(value, bool):
+                    url_params[key] = str(value).lower()
+                else:
+                    url_params[key] = value
         request_url = f"{base_url}{path}"
         logger.debug(f"Request URL: {request_url}")
         logger.debug(f"Request Params: {url_params}")
         if json is not None:
             logger.debug(f"Request JSON {json}")
         try:
             if request_type == "delete":
```

### Comparing `tmdbapis-1.1.0/tmdbapis/api4.py` & `tmdbapis-1.2.0/tmdbapis/api4.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.1.0/tmdbapis/exceptions.py` & `tmdbapis-1.2.0/tmdbapis/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.1.0/tmdbapis/objs/image.py` & `tmdbapis-1.2.0/tmdbapis/objs/image.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.1.0/tmdbapis/objs/mixin.py` & `tmdbapis-1.2.0/tmdbapis/objs/mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def remove_as_favorite(self: TMDbObj):
         """ Remove as a Favorite (Authentication Required) """
         self._api.account_mark_as_favorite(self._media_type(), self.id, False)
 
     @abstractmethod
     def _media_type(self):
-        pass
+        """ abstract media type """
 
 
 class Rate(ABC):
     def rate(self, rating: float):
         """ Add a Rating (Authentication Required)
 
             Parameters:
@@ -33,26 +33,26 @@
 
     def delete_rating(self):
         """ Delete a Rating (Authentication Required) """
         self._delete_rate()
 
     @abstractmethod
     def _rate(self, rating):
-        pass
+        """ abstract rate """
 
     @abstractmethod
     def _delete_rate(self):
-        pass
+        """ abstract delete rate """
 
 
 class Watchlist(ABC):
     def add_to_watchlist(self: TMDbObj):
         """ Add to your Watchlist (Authentication Required) """
         self._api.account_add_to_watchlist(self._media_type(), self.id, True)
 
     def remove_from_watchlist(self: TMDbObj):
         """ Remove from your Watchlist (Authentication Required) """
         self._api.account_add_to_watchlist(self._media_type(), self.id, False)
 
     @abstractmethod
     def _media_type(self):
-        pass
+        """ abstract media type """
```

### Comparing `tmdbapis-1.1.0/tmdbapis/objs/pagination.py` & `tmdbapis-1.2.0/tmdbapis/objs/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod
 from typing import Optional, Union, List, Tuple
 from urllib.parse import urlparse, parse_qs
 
 from tmdbapis.objs.base import TMDbObj
 from tmdbapis.objs.reload import Movie, TVShow
-from tmdbapis.exceptions import NotFound, Invalid
+from tmdbapis.exceptions import NotFound, Invalid, TMDbException
 
 v3_sorts = ["created_at.asc", "created_at.desc"]
 v4_movie_sorts = ["created_at.asc", "created_at.desc", "release_date.asc", "release_date.desc", "title.asc", "title.desc", "vote_average.asc", "vote_average.desc"]
 v4_show_sorts = ["created_at.asc", "created_at.desc", "first_air_date.asc", "first_air_date.desc", "name.asc", "name.desc", "vote_average.asc", "vote_average.desc"]
 v4_list_sorts = ["original_order.asc", "original_order.desc", "vote_average.asc", "vote_average.desc", "primary_release_date.asc", "primary_release_date.desc", "title.asc", "title.desc"]
 
 class TMDbPagination(TMDbObj):
@@ -91,26 +91,26 @@
         return self.results[index]
 
     def __len__(self):
         return self.total_results
 
     @abstractmethod
     def _get_page(self, page):
-        pass
+        """ abstract get page """
 
-    def get_results(self, amount: int):
+    def get_results(self, amount: Optional[int] = None):
         """ Gets the amount of results asked for from multiple pages. This method can make alot of calls to the API if you're not careful.
 
             Parameters:
-                amount (int): Amount of Items you want returned.
+                amount (Optional[int]): Amount of Items you want returned.
 
             Raises:
                 :class:`~tmdbapis.exceptions.Invalid`: When ``amount`` is not greater than zero.
          """
-        if int(amount) > self.total_results:
+        if amount is None or int(amount) > self.total_results:
             amount = self.total_results
         if amount < 1:
             raise Invalid("amount must be greater then 0")
         results = []
         current_page = 0
         while len(results) < amount and current_page < self.total_pages:
             current_page += 1
@@ -435,15 +435,15 @@
     def __init__(self, tmdb, query):
         self._loading = True
         self.query = query
         self._loading = False
         super().__init__(tmdb, None, "collection", "SearchCollections")
 
     def _get_page(self, page):
-        results = self._api.search_search_collections(self.query, language=self._tmdb.language, page=self.page)
+        results = self._api.search_search_collections(self.query, language=self._tmdb.language, page=page)
         if int(results["total_results"]) > 0:
             return results
         raise NotFound("No Results Found")
 
 
 class SearchCompanies(TMDbPagination):
     """ Paginated Object of the Companies Search Results.
@@ -454,15 +454,15 @@
     def __init__(self, tmdb, query):
         self._loading = True
         self.query = query
         self._loading = False
         super().__init__(tmdb, None, "company", "SearchCompanies")
 
     def _get_page(self, page):
-        results = self._api.search_search_companies(self.query, page=self.page)
+        results = self._api.search_search_companies(self.query, page=page)
         if int(results["total_results"]) > 0:
             return results
         raise NotFound("No Results Found")
 
 
 class SearchKeywords(TMDbPagination):
     """ Paginated Object of the Keywords Search Results.
@@ -473,15 +473,15 @@
     def __init__(self, tmdb, query):
         self._loading = True
         self.query = query
         self._loading = False
         super().__init__(tmdb, None, "keyword", "SearchKeywords")
 
     def _get_page(self, page):
-        results = self._api.search_search_keywords(self.query, page=self.page)
+        results = self._api.search_search_keywords(self.query, page=page)
         if int(results["total_results"]) > 0:
             return results
         raise NotFound("No Results Found")
 
 
 class SearchMovies(TMDbPagination):
     """ Paginated Object of the Movies Search Results.
@@ -503,15 +503,15 @@
         self._loading = False
         super().__init__(tmdb, None, "movie", "SearchMovies")
 
     def _get_page(self, page):
         results = self._api.search_search_movies(
             self.query,
             language=self._tmdb.language,
-            page=self.page,
+            page=page,
             include_adult=self.include_adult,
             region=self.region,
             year=self.year,
             primary_release_year=self.primary_release_year
         )
         if int(results["total_results"]) > 0:
             return results
@@ -534,15 +534,15 @@
         self._loading = False
         super().__init__(tmdb, None, "media_type", "SearchMulti")
 
     def _get_page(self, page):
         results = self._api.search_multi_search(
             self.query,
             language=self._tmdb.language,
-            page=self.page,
+            page=page,
             include_adult=self.include_adult,
             region=self.region
         )
         if int(results["total_results"]) > 0:
             return results
         raise NotFound("No Results Found")
 
@@ -563,15 +563,15 @@
         self._loading = False
         super().__init__(tmdb, None, "person", "SearchPeople")
 
     def _get_page(self, page):
         results = self._api.search_search_people(
             self.query,
             language=self._tmdb.language,
-            page=self.page,
+            page=page,
             include_adult=self.include_adult,
             region=self.region
         )
         if int(results["total_results"]) > 0:
             return results
         raise NotFound("No Results Found")
 
@@ -592,15 +592,15 @@
         self._loading = False
         super().__init__(tmdb, None, "tv", "SearchTVShows")
 
     def _get_page(self, page):
         results = self._api.search_search_tv_shows(
             self.query,
             language=self._tmdb.language,
-            page=self.page,
+            page=page,
             include_adult=self.include_adult,
             first_air_date_year=self.first_air_date_year
         )
         if int(results["total_results"]) > 0:
             return results
         raise NotFound("No Results Found")
 
@@ -759,14 +759,15 @@
         self._tmdb._v4_check().list_update_list(
             self.id,
             name=name,
             description=description,
             public=public,
             sort_by=sort_by
         )
+        self.reload()
 
     def _check_item(self, item):
         if isinstance(item, Movie):
             item_id = item.id
             item_type = "movie"
         elif isinstance(item, TVShow):
             item_id = item.id
@@ -824,14 +825,15 @@
             item_ids.append({"media_type": item_type, "media_id": item_id})
 
         if self._api4 and self._api4.has_write_token:
             self._api4.list_add_items(self.id, item_ids)
         else:
             for item_id in item_ids:
                 self._api.lists_add_movie(self.id, item_id["media_id"])
+        self.reload()
 
     def remove_items(self, items: List[Union[Movie, TVShow, Tuple[int, str]]]):
         """ Adds the items given to the list.
 
             Parameters:
                 items (List[Union[Movie, TVShow, Tuple[int, str]]]): Item you want to remove from the list. If not using a Movie or Show object then you must use a Tuple with the ID and either ``movie`` or ``tv``.
 
@@ -846,14 +848,15 @@
             item_ids.append({"media_type": item_type, "media_id": item_id})
 
         if self._api4 and self._api4.has_write_token:
             self._api4.list_remove_items(self.id, item_ids)
         else:
             for item_id in item_ids:
                 self._api.lists_remove_movie(self.id, item_id["media_id"])
+        self.reload()
 
     def update_items(self, items: List[Tuple[Union[Movie, TVShow, Tuple[int, str]], str]]):
         """ Updates the items on the list.
 
             Parameters:
                 items (List[Tuple[Union[Movie, TVShow, Tuple[int, str]], str]]): Tuples of the items you want updated on the list and their description. If not using a Movie or Show object then you must use a Tuple of the ID and either ``movie`` or ``tv``.
 
@@ -864,28 +867,34 @@
         if not isinstance(items, list):
             items = [items]
         for item in items:
             item_id, item_type = self._check_item(item[0])
             comment = item[1]
             item_ids.append({"media_type": item_type, "media_id": item_id, "comment": comment})
         self._tmdb._v4_check(write=True).list_update_items(self.id, item_ids)
+        self.reload()
 
     def clear(self):
         """ Clear all items from the list. """
         if self._api4 and self._api4.has_write_token:
             self._api4.list_clear_list(self.id)
         else:
-            self._api.lists_clear_list(self.id, True)
+            self._api.lists_clear_list(self.id, confirm=True)
+        self.reload()
 
     def delete(self):
         """ Delete the list. """
         if self._api4 and self._api4.has_write_token:
             self._api4.list_delete_list(self.id)
         else:
-            self._api.lists_delete_list(self.id)
+            try:
+                self._api.lists_delete_list(self.id)
+            except TMDbException as e:
+                if not str(e).startswith("(500 [Internal Server Error])"):
+                    raise
 
 
 class TopRatedMovies(TMDbPagination):
     """ Paginated Object of the top rated movies on TMDB.
 
         Attributes:
             region (str): ISO 3166-1 code used to filter release dates.
```

### Comparing `tmdbapis-1.1.0/tmdbapis/objs/reload.py` & `tmdbapis-1.2.0/tmdbapis/objs/reload.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return None
 
     def _append_load(self, partial=False):
         return self._full_load(partial=self._append_str() if partial is False else partial)
 
     @abstractmethod
     def _full_load(self, partial=None):
-        pass
+        """ Abstract Full Load """
 
     def reload(self, partial: Optional[Union[bool, str]] = False):
         """ Reloads the object.
 
             Parameters:
                 partial (Optional[Union[bool, str]]): leave False for a full load otherwise specify the endpoints you want added.
         """
@@ -352,15 +352,15 @@
             guest_stars (List[:class:`~tmdbapis.objs.reload.Credit`]): List of Episode Guest Stars Credits.
             id (int): Episode ID.
             imdb_id (str): Episode IMDb ID.
             name (str): Episode Name.
             order (int): Episode Order in Group.
             overview (str): Episode Overview.
             production_code (str): Episode Production Code.
-            rated (Union[float, bool]): Either your TMDb Rating for the Episode or False if there is no rating.
+            rated (float): Either your TMDb Rating for the Episode or None if there is no rating.
             season_number (int): Season the Episode is in.
             still_path (str): Still Path.
             still_url (str): Still Full URL.
             stills (List[:class:`~tmdbapis.objs.image.Still`]): List of other Stills for the Episode.
             title (str): alias of name.
             translations (List[:class:`~tmdbapis.objs.simple.Translation`]): List of Translations for the Episode.
             tv_id (int): TMDb TV Show ID the contains the Episode.
@@ -386,18 +386,15 @@
         self.guest_stars = self._parse(attrs="guest_stars", value_type="tv_cast", is_list=True)
         self.id = self._parse(attrs="id", value_type="int")
         self.imdb_id = self._parse(attrs=["external_ids", "imdb_id"])
         self.name = self._parse(attrs="name")
         self.order = self._parse(attrs="order", value_type="int") if "order" in self._data else None
         self.overview = self._parse(attrs="overview")
         self.production_code = self._parse(attrs="production_code")
-        try:
-            self.rated = self._parse(attrs=["account_states", "rated"], value_type="float")
-        except ValueError:
-            self.rated = self._parse(attrs=["account_states", "rated"], value_type="bool")
+        self.rated = self._parse(attrs=["account_states", "rated", "value"], value_type="float", default_is_none=True)
         self.season_number = self._parse(attrs="season_number", value_type="int")
         self.still_path = self._parse(attrs="still_path")
         self.still_url = self._image_url(self.still_path)
         self.stills = self._parse(attrs=["images", "stills"], value_type="still", is_list=True)
         self.title = self.name
         self.translations = self._parse(attrs=["translations", "translations"], value_type="translation", is_list=True)
         self.tv_id = self._parse(attrs="show_id", value_type="int") if "show_id" in self._data else self._tv_id
@@ -521,15 +518,15 @@
             original_language (:class:`~tmdbapis.objs.simple.Language`): Original Language of the Movie.
             original_title (str): Movie's Original Title.
             overview (str): Movie Overview.
             popularity (float): Movie's Popularity.
             poster_path (str): Poster Path.
             poster_url (str): Poster Full URL.
             posters (List[:class:`~tmdbapis.objs.image.Poster`]): List of other Posters for the Movie.
-            rated (Union[float, bool]): Your rating for this Movie or false if you have not rated it. (Authentication Required)
+            rated (float): Your rating for this Movie or None if you have not rated it. (Authentication Required)
             recommendations (:class:`~tmdbapis.objs.pagination.RecommendedMovies`): Pagination Object of Recommended Movies based on this Movie.
             release_date (datetime): Movie's Primary Release Date.
             release_dates (Dict[str, List[:class:`~tmdbapis.objs.simple.ReleaseDate`]]): Dictionary of Release Dates where the keys are the ISO 3166-1 Alpha-2 Country Codes.
             revenue (int): Movie's Revenue.
             reviews (class:`~tmdbapis.objs.pagination.MovieReviews`): Pagination Object of Movie Reviews for this Movie.
             runtime (int) Movie's Runtime.
             similar (class:`~tmdbapis.objs.pagination.SimilarMovies`): Pagination Object of Similar Movie to this Movie.
@@ -576,18 +573,15 @@
         self.original_language = self._parse(attrs="original_language", value_type="language")
         self.original_title = self._parse(attrs="original_title")
         self.overview = self._parse(attrs="overview")
         self.popularity = self._parse(attrs="popularity", value_type="float")
         self.poster_path = self._parse(attrs="poster_path")
         self.poster_url = self._image_url(self.poster_path)
         self.posters = self._parse(attrs=["images", "posters"], value_type="poster", is_list=True)
-        try:
-            self.rated = self._parse(attrs=["account_states", "rated"], value_type="float")
-        except ValueError:
-            self.rated = self._parse(attrs=["account_states", "rated"], value_type="bool")
+        self.rated = self._parse(attrs=["account_states", "rated", "value"], value_type="float", default_is_none=True)
         self.recommendations = self._parse(attrs="recommendations", value_type="recommended_movies", key=self.id)
         self.release_date = self._parse(attrs="release_date", value_type="date")
         self.release_dates = {}
         if "release_dates" in self._data and "results" in self._data["release_dates"]:
             for iso in self._data["release_dates"]["results"]:
                 self.release_dates[iso["iso_3166_1"]] = self._parse(data=iso, attrs="release_dates",
                                                                     value_type="release_date", is_list=True)
@@ -907,15 +901,15 @@
             original_language (:class:`~tmdbapis.objs.simple.Language`): Original Language of the TV Show.
             original_name (str): TV Show's Original Name.
             overview (str): TV Show Overview.
             popularity (float): TV Show's Popularity.
             poster_path (str): Poster Path.
             poster_url (str): Poster Full URL.
             posters (List[:class:`~tmdbapis.objs.image.Poster`]): List of other Posters for the TV Show.
-            rated (Union[float, bool]): Your rating for this TV Show or false if you have not rated it. (Authentication Required)
+            rated (float): Your rating for this TV Show or None if you have not rated it. (Authentication Required)
             recommendations (:class:`~tmdbapis.objs.pagination.RecommendedTVShows`): Pagination Object of Recommended TV Show based on this TV Show.
             seasons (List[:class:`~tmdbapis.objs.reload.Season`]): List of Seasons in the TV Show.
             similar (class:`~tmdbapis.objs.pagination.SimilarTVShows`): Pagination Object of Similar TV Show to this TV Show.
             spoken_languages (List[:class:`~tmdbapis.objs.simple.Language`]): List of Spoken Languages for the TV Show.
             status (str): TV Show's Status.
             tagline (str): TV Show's Tagline.
             title (str): alias of name.
@@ -973,18 +967,15 @@
         self.original_language = self._parse(attrs="original_language", value_type="language")
         self.original_name = self._parse(attrs="original_name")
         self.overview = self._parse(attrs="overview")
         self.popularity = self._parse(attrs="popularity", value_type="float")
         self.poster_path = self._parse(attrs="poster_path")
         self.poster_url = self._image_url(self.poster_path)
         self.posters = self._parse(attrs=["images", "posters"], value_type="poster", is_list=True)
-        try:
-            self.rated = self._parse(attrs=["account_states", "rated"], value_type="float")
-        except ValueError:
-            self.rated = self._parse(attrs=["account_states", "rated"], value_type="bool")
+        self.rated = self._parse(attrs=["account_states", "rated", "value"], value_type="float", default_is_none=True)
         self.recommendations = self._parse(attrs="recommendations", value_type="recommended_tv", key=self.id)
         self.seasons = self._parse(attrs="seasons", value_type="season", is_list=True, key=self.id)
         self.similar = self._parse(attrs="similar", value_type="similar_tv", key=self.id)
         self.spoken_languages = self._parse(attrs="spoken_languages", value_type="language", is_list=True)
         self.status = self._parse(attrs="status")
         self.tagline = self._parse(attrs="tagline")
         self.title = self.name
```

### Comparing `tmdbapis-1.1.0/tmdbapis/objs/simple.py` & `tmdbapis-1.2.0/tmdbapis/objs/simple.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.1.0/tmdbapis/tmdb.py` & `tmdbapis-1.2.0/tmdbapis/tmdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import logging
 from datetime import datetime
-from typing import Optional, Union, List, Dict
+from typing import Optional, Union, List, Dict, Any
 from requests import Session
 from tmdbapis.api3 import API3
 from tmdbapis.api4 import API4
 from tmdbapis.exceptions import Authentication, Invalid
-from tmdbapis.objs.pagination import NowPlayingMovies, PopularMovies, TopRatedMovies, UpcomingMovies, Trending, PopularPeople, \
-    TVShowsAiringToday, TVShowsOnTheAir, PopularTVShows, TopRatedTVShows, MovieRecommendations, TVShowRecommendations, \
-    SearchCompanies, SearchCollections, SearchKeywords, SearchMovies, SearchMulti, SearchPeople, SearchTVShows, \
-    CreatedLists, FavoriteMovies, FavoriteTVShows, RatedMovies, RatedTVShows, RatedEpisodes, MovieWatchlist, \
-    TVShowWatchlist, DiscoverMovies, DiscoverTVShows, TMDbList
-from tmdbapis.objs.reload import Account, Collection, Configuration, Company, Credit, Keyword, Movie, \
-    Network, Person, Review, TVShow, Season, Episode, EpisodeGroup
-from tmdbapis.objs.simple import Country, CountryCertifications, Genre, WatchProvider, FindResults, Language
+from tmdbapis.objs.image import Backdrop, Logo, Poster, Profile, Still, Tagged
+from tmdbapis.objs.pagination import NowPlayingMovies, PopularMovies, TopRatedMovies, UpcomingMovies, Trending, \
+    PopularPeople, TVShowsAiringToday, TVShowsOnTheAir, PopularTVShows, TopRatedTVShows, MovieRecommendations, \
+    TVShowRecommendations, SearchCompanies, SearchCollections, SearchKeywords, SearchMovies, SearchMulti, \
+    SearchPeople, SearchTVShows, CreatedLists, FavoriteMovies, FavoriteTVShows, RatedMovies, RatedTVShows, \
+    RatedEpisodes, MovieWatchlist, TVShowWatchlist, DiscoverMovies, DiscoverTVShows, TMDbList, MovieReviews, \
+    MovieLists, RecommendedMovies, SimilarMovies, RecommendedTVShows, SimilarTVShows, TaggedImages
+from tmdbapis.objs.reload import Account, Collection, Configuration, Company, Credit, Keyword, Movie, Network, \
+    Person, Review, TVShow, Season, Episode, EpisodeGroup
+from tmdbapis.objs.simple import Country, CountryCertifications, Genre, WatchProvider, FindResults, Language, \
+    AlternativeName, AlternativeTitle, Certification, CountryWatchProviders, Department, Group, ReleaseDate, Timezones, \
+    Trailer, Translation, User, Video
 
 logger = logging.getLogger(__name__)
 
 discover_movie_options = [
     "region", "sort_by", "certification_country", "certification", "certification.lte", "certification.gte",
     "include_adult", "include_video", "primary_release_year", "primary_release_date.gte", "primary_release_date.lte",
     "release_date.gte", "release_date.lte", "with_release_type", "year", "vote_count.gte", "vote_count.lte",
@@ -109,14 +113,205 @@
         elif obj_type == "movie_genre":
             return object_check(lookup, "id", self._movie_genre_lookup, is_int=True)
         elif obj_type == "tv_genre":
             return object_check(lookup, "id", self._tv_genre_lookup, is_int=True)
         else:
             return None
 
+    def _parse(self, data=None, attrs: Optional[Union[str, list]] = None, value_type: str = "str",
+               default_is_none: bool = False, is_list: bool = False, is_dict: bool = False, extend: bool = False,
+               key: Any = None):
+        """ Validate the value given from the options given.
+
+            Parameters:
+                attrs (Optional[Union[str, list]]): check data for these attributes.
+                value_type (str): Type that the value is.
+                default_is_none (bool): Makes default None.
+                is_list (bool): value is list of values.
+                is_dict (bool): value is dict of values.
+                extend (bool): value is list of values.
+                key (Any): extra key.
+
+            Returns:
+                Any: Parsed Value
+        """
+
+        if default_is_none is False and value_type in ["int", "float"]:
+            default = 0
+        elif default_is_none is False and is_list:
+            default = []
+        else:
+            default = None
+
+        value = data
+        if attrs:
+            if not isinstance(attrs, list):
+                attrs = [attrs]
+            for attr in attrs:
+                if isinstance(value, dict) and attr in value:
+                    value = value[attr]
+                else:
+                    return default
+
+        if value is None:
+            return default
+        elif extend:
+            export_list = []
+            for v in value:
+                export_list.extend(self._parse(data=v, value_type=value_type, default_is_none=default_is_none, key=key))
+            return export_list
+        elif is_list:
+            return [self._parse(data=v, value_type=value_type, default_is_none=default_is_none, key=key) for v in value]
+        elif is_dict:
+            return {k: self._parse(data=v, value_type=value_type, default_is_none=default_is_none, key=k)
+                    for k, v in value.items()}
+        elif value_type == "int":
+            return int(value)
+        elif value_type == "float":
+            return float(value)
+        elif value_type == "bool":
+            if isinstance(value, bool):
+                return value
+            elif str(value).lower() in ["t", "true", "1", "y", "yes"]:
+                return True
+            elif str(value).lower() in ["f", "false", "0", "n", "no"]:
+                return False
+            else:
+                return default
+        elif value_type == "date":
+            if not value:
+                return None
+            elif "T" in value:
+                return datetime.strptime(value[:-1].split(".")[0], "%Y-%m-%dT%H:%M:%S")
+            else:
+                return datetime.strptime(value, "%Y-%m-%d")
+        elif value_type == "dict":
+            return value
+        elif value_type == "alternative_name":
+            return AlternativeName(self, value)
+        elif value_type == "alternative_title":
+            return AlternativeTitle(self, value)
+        elif value_type == "certification":
+            return Certification(self, value)
+        elif value_type == "load_country":
+            return Country(self, value)
+        elif value_type == "country_certification":
+            return CountryCertifications(self, value, key)
+        elif value_type == "country_watch_provider":
+            return CountryWatchProviders(self, value, key)
+        elif value_type == "load_department":
+            return Department(self, value)
+        elif value_type == "load_genre":
+            return Genre(self, value)
+        elif value_type == "group":
+            return Group(self, value)
+        elif value_type == "load_language":
+            return Language(self, value)
+        elif value_type == "release_date":
+            return ReleaseDate(self, value)
+        elif value_type == "load_timezone":
+            return Timezones(self, value)
+        elif value_type == "trailer":
+            return Trailer(self, value)
+        elif value_type == "translation":
+            return Translation(self, value)
+        elif value_type == "user":
+            return User(self, value)
+        elif value_type == "video":
+            return Video(self, value)
+        elif value_type == "watch_provider":
+            return WatchProvider(self, value)
+        elif value_type == "backdrop":
+            return Backdrop(self, value)
+        elif value_type == "logo":
+            return Logo(self, value)
+        elif value_type == "poster":
+            return Poster(self, value)
+        elif value_type == "profile":
+            return Profile(self, value)
+        elif value_type == "still":
+            return Still(self, value)
+        elif value_type == "tagged":
+            return Tagged(self, value)
+        elif value_type == "collection":
+            return Collection(self, value)
+        elif value_type == "company":
+            return Company(self, value)
+        elif value_type == "movie_cast":
+            return Credit(self, value, credit_type="cast", media_type="movie")
+        elif value_type == "movie_crew":
+            return Credit(self, value, credit_type="crew", media_type="movie")
+        elif value_type == "tv_cast":
+            return Credit(self, value, credit_type="cast", media_type="tv")
+        elif value_type == "tv_crew":
+            return Credit(self, value, credit_type="crew", media_type="tv")
+        elif value_type == "agg_tv_cast":
+            cast = []
+            for role in value["roles"]:
+                new_dict = value.copy()
+                for k, v in role.items():
+                    new_dict[k] = v
+                cast.append(Credit(self, new_dict, credit_type="cast", media_type="tv"))
+            return cast
+        elif value_type == "agg_tv_crew":
+            crew = []
+            for role in value["jobs"]:
+                new_dict = value.copy()
+                for k, v in role.items():
+                    new_dict[k] = v
+                crew.append(Credit(self, new_dict, credit_type="crew", media_type="tv"))
+            return crew
+        elif value_type == "keyword":
+            return Keyword(self, value)
+        elif value_type == "movie":
+            return Movie(self, value)
+        elif value_type == "network":
+            return Network(self, value)
+        elif value_type == "person":
+            return Person(self, value)
+        elif value_type == "review":
+            return Review(self, value)
+        elif value_type == "tv":
+            return TVShow(self, value)
+        elif value_type == "season":
+            return Season(self, value, key)
+        elif value_type == "episode":
+            return Episode(self, value, key)
+        elif value_type == "episode_group":
+            return EpisodeGroup(self, value, key)
+        elif value_type == "media_type":
+            if value["media_type"] == "movie":
+                return Movie(self, value)
+            elif value["media_type"] == "tv":
+                return TVShow(self, value)
+            elif value["media_type"] == "person":
+                return Person(self, value)
+        elif value_type == "list":
+            return TMDbList(self, value)
+        elif value_type == "movie_reviews":
+            return MovieReviews(self, value, key)
+        elif value_type == "lists":
+            return MovieLists(self, value, key)
+        elif value_type == "recommended_movies":
+            return RecommendedMovies(self, value, key)
+        elif value_type == "similar_movies":
+            return SimilarMovies(self, value, key)
+        elif value_type == "recommended_tv":
+            return RecommendedTVShows(self, value, key)
+        elif value_type == "similar_tv":
+            return SimilarTVShows(self, value, key)
+        elif value_type == "tagged_images":
+            return TaggedImages(self, value, key)
+        elif value_type == "content_rating":
+            return {v["iso_3166_1"]: v["rating"] for v in value}
+        elif value_type in ["country", "language", "movie_genre", "tv_genre"]:
+            return self._get_object(value, value_type)
+        else:
+            return str(value)
+
     def _validate_language(self, language):
         if isinstance(language, Language):
             return language.iso_639_1
         elif str(language).lower() in self._iso_639_1:
             return str(language).lower()
         else:
             raise Invalid(f"Language: {language} is invalid see Configuration.languages for the options.")
@@ -142,15 +337,15 @@
             return None
         elif isinstance(data, datetime):
             return data.strftime(date_format)
         else:
             try:
                 return datetime.strptime(str(data), date_format).strftime(date_format)
             except ValueError:
-                raise Invalid(f"date: {data} must be a datetime or in the format YYYY-MM-DD")
+                raise Invalid(f"date: {data} must be a datetime or in the format YYYY-MM-DD (e.g. 2020-12-25)")
 
     def _validate_discover(self, is_movie, **kwargs):
         validated = {}
         for k, v in kwargs.items():
             if is_movie and k not in discover_movie_options or not is_movie and k not in discover_tv_options:
                 raise Invalid(f"{k} is not a valid parameter")
             elif k == "sort_by":
@@ -164,41 +359,37 @@
                     raise Invalid("certification_country must be used with either certification, certification.lte, or certification.gte")
                 validated[k] = str(v)
             elif k in ["certification", "certification.lte", "certification.gte"]:
                 if "certification_country" not in kwargs:
                     raise Invalid("certification must be used with certification_country")
                 validated[k] = str(v)
             elif k in ["include_adult", "include_video", "include_null_first_air_dates", "screened_theatrically"]:
-                if not isinstance(v, bool):
+                data = self._parse(data=v, value_type="bool")
+                if data is None:
                     raise Invalid(f"{k} must be either True or False")
                 validated[k] = v
             elif k in ["primary_release_date.gte", "primary_release_date.lte", "release_date.gte", "release_date.lte",
                        "air_date.gte", "air_date.lte", "first_air_date.gte", "first_air_date.lte"]:
-                if isinstance(v, datetime):
-                    date_obj = v
-                else:
-                    try:
-                        date_obj = datetime.strptime(str(v), "%Y-%m-%d")
-                    except ValueError:
-                        raise Invalid(f"{k} must be a datetime object or match pattern YYYY-MM-DD (e.g. 2020-12-25)")
-                validated[k] = datetime.strftime(date_obj, "%Y-%m-%d")
+                data = self._validate_date(v)
+                if data:
+                    validated[k] = data
             elif k in ["primary_release_year", "first_air_date_year", "vote_count.gte", "vote_count.lte",
                        "with_runtime.gte", "with_runtime.lte"]:
-                if not isinstance(v, int) or v < 1:
+                if not isinstance(v, int) or v <= 0:
                     raise Invalid(f"{k} must be an integer greater then 0")
                 validated[k] = v
             elif k in ["vote_average.gte", "vote_average.lte"]:
-                if not isinstance(v, float) or v < 1:
+                if not isinstance(v, (int, float)) or v <= 0:
                     raise Invalid(f"{k} must be a number greater then 0.0")
-                validated[k] = v
+                validated[k] = float(v)
             elif k == "with_watch_monetization_types":
-                if "watch_region" not in kwargs:
-                    raise Invalid("with_watch_monetization_types must be used with watch_region")
                 if v not in ["flatrate", "free", "ads", "rent", "buy"]:
                     raise Invalid(f"{v} is not a valid with_watch_monetization_types option. Options: [flatrate, free, ads, rent, or buy]")
+                if "watch_region" not in kwargs:
+                    raise Invalid("with_watch_monetization_types must be used with watch_region")
                 validated[k] = v
             else:
                 validated[k] = ",".join([str(x) for x in v]) if isinstance(v, list) else str(v)
         return validated
 
     @property
     def include_language(self):
@@ -211,34 +402,36 @@
         else:
             final = []
             for lang in str(include_language).split(","):
                 if str(lang).lower() in ["null", "none"]:
                     final.append("null")
                 elif str(lang).lower() in self._iso_639_1:
                     final.append(str(lang).lower())
-                elif str(lang).lower() in self._translations:
-                    final.append(self._translations[str(lang).lower()])
                 else:
-                    raise Invalid(f"Language: {lang} is invalid see Configuration.languages and Configuration.primary_translations for the options.")
+                    try:
+                        final.append(self._validate_translation(lang))
+                    except Invalid:
+                        raise Invalid(f"Language: {lang} is invalid see Configuration.languages and Configuration.primary_translations for the options.")
             self._include_language = ",".join(final)
 
     @property
     def language(self):
         return self._language
 
     @language.setter
     def language(self, lang):
         if lang is None:
             self._language = None
         elif str(lang).lower() in self._iso_639_1:
             self._language = str(lang).lower()
-        elif str(lang).lower() in self._translations:
-            self._language = self._translations[str(lang).lower()]
         else:
-            raise Invalid(f"Language: {lang} is invalid see Configuration.languages and Configuration.primary_translations for the options.")
+            try:
+                self._language = self._validate_translation(lang)
+            except Invalid:
+                raise Invalid(f"Language: {lang} is invalid see Configuration.languages and Configuration.primary_translations for the options.")
 
     @property
     def account_id(self):
         return self._api.account_id
 
     @property
     def session_id(self):
@@ -582,34 +775,30 @@
             Parameters:
                 reload (bool): Reload the cached movie certifications
 
             Returns:
                 Dict[str, :class:`~tmdbapis.objs.simple.CountryCertifications`]
         """
         if reload or self._movie_certifications is None:
-            self._movie_certifications = {
-                k: CountryCertifications(self, v, k) for k, v in
-                self._api.certifications_get_movie_certifications()["certifications"].items()
-            }
+            self._movie_certifications = self._parse(data=self._api.certifications_get_movie_certifications(),
+                                                     attrs="certifications", value_type="country_certification", is_dict=True)
         return self._movie_certifications
 
     def tv_certifications(self, reload: bool = False) -> Dict[str, CountryCertifications]:
         """ Get an up to date list of the officially supported TV show certifications on TMDB.
 
             Parameters:
                 reload (bool): Reload the cached tv certifications
 
             Returns:
                 Dict[str, :class:`~tmdbapis.objs.simple.CountryCertifications`]
         """
         if reload or self._tv_certifications is None:
-            self._tv_certifications = {
-                k: CountryCertifications(self, v, k) for k, v in
-                self._api.certifications_get_tv_certifications()["certifications"].items()
-            }
+            self._tv_certifications = self._parse(data=self._api.certifications_get_tv_certifications(),
+                                                  attrs="certifications", value_type="country_certification", is_dict=True)
         return self._tv_certifications
 
     def movie_change_list(self,
                           start_date: Optional[Union[datetime, str]] = None,
                           end_date: Optional[Union[datetime, str]] = None
                           ) -> List[Movie]:
         """ Get a list of :class:`~tmdbapis.objs.reload.Movie` that have been changed in the past 24 hours.
@@ -906,28 +1095,30 @@
             Parameters:
                 reload (bool): Reload the cached movie genres.
 
             Returns:
                 List[:class:`~tmdbapis.objs.simple.Genre`]
         """
         if reload or self._movie_genres is None:
-            self._movie_genres = [Genre(self, g) for g in self._api.genres_get_movie_list()["genres"]]
+            self._movie_genres = self._parse(data=self._api.genres_get_movie_list(),
+                                             attrs="genres", value_type="load_genre", is_list=True)
         return self._movie_genres
 
     def tv_genres(self, reload: bool = False) -> List[Genre]:
         """ Gets a list of all TV show :class:`~tmdbapis.objs.simple.Genre`.
 
             Parameters:
                 reload (bool): Reload the cached movie genres.
 
             Returns:
                 List[:class:`~tmdbapis.objs.simple.Genre`]
         """
         if reload or self._tv_genres is None:
-            self._tv_genres = [Genre(self, g) for g in self._api.genres_get_tv_list()["genres"]]
+            self._tv_genres = self._parse(data=self._api.genres_get_tv_list(),
+                                          attrs="genres", value_type="load_genre", is_list=True)
         return self._tv_genres
 
     def keyword(self, keyword_id: int, load: bool = True) -> Keyword:
         """ Gets the :class:`~tmdbapis.objs.reload.Keyword` for the given id.
 
             Parameters:
                 keyword_id (int): Keyword ID of the keyword you want.
```

### Comparing `tmdbapis-1.1.0/tmdbapis.egg-info/PKG-INFO` & `tmdbapis-1.2.0/tmdbapis.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmdbapis
-Version: 1.1.0
+Version: 1.2.0
 Summary: A lightweight Python library for The V3 and V4 TMDb APIs.
 Home-page: https://github.com/meisnate12/TMDbAPIs
 Author: Nathan Taggart
 Author-email: meisnate12@gmail.com
 License: MIT License
 Project-URL: Documentation, https://tmdbapis.metamanager.wiki
 Project-URL: Funding, https://github.com/sponsors/meisnate12
@@ -21,37 +21,59 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Welcome to TMDbAPIs Documentation!
 ==========================================================
 
-.. image:: https://img.shields.io/readthedocs/tmdbapis?style=plastic
-    :target: https://tmdbapis.metamanager.wiki
-    :alt: Read the Docs
-
 .. image:: https://img.shields.io/github/v/release/meisnate12/TMDbAPIs?style=plastic
     :target: https://github.com/meisnate12/TMDbAPIs/releases
     :alt: GitHub release (latest by date)
 
+.. image:: https://img.shields.io/github/actions/workflow/status/meisnate12/TMDbAPIs/tests.yml?branch=master&style=plastic
+    :target: https://github.com/meisnate12/TMDbAPIs/actions/workflows/tests.yml
+    :alt: Build Testing
+
+.. image:: https://img.shields.io/codecov/c/github/meisnate12/TMDbAPIs?color=greenred&style=plastic
+    :target: https://codecov.io/gh/meisnate12/TMDbAPIs
+    :alt: Build Coverage
+
+.. image:: https://img.shields.io/github/commits-since/meisnate12/TMDbAPIs/latest?style=plastic
+    :target: https://github.com/meisnate12/TMDbAPIs/commits/master
+    :alt: GitHub commits since latest release (by date) for a branch
+
 .. image:: https://img.shields.io/pypi/v/TMDbAPIs?style=plastic
     :target: https://pypi.org/project/tmdbapis/
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/dm/tmdbapis.svg?style=plastic
     :target: https://pypi.org/project/tmdbapis/
     :alt: Downloads
 
-.. image:: https://img.shields.io/github/commits-since/meisnate12/TMDbAPIs/latest?style=plastic
-    :target: https://github.com/meisnate12/TMDbAPIs/commits/master
-    :alt: GitHub commits since latest release (by date) for a branch
+|
+
+.. image:: https://img.shields.io/readthedocs/plex-meta-manager?color=%2300bc8c&style=plastic
+    :target: https://tmdbapis.metamanager.wiki/en/latest/
+    :alt: Wiki
+
+.. image:: https://img.shields.io/discord/822460010649878528?color=%2300bc8c&label=Discord&style=plastic
+    :target: https://discord.gg/NfH6mGFuAB
+    :alt: Discord
+
+.. image:: https://img.shields.io/reddit/subreddit-subscribers/PlexMetaManager?color=%2300bc8c&label=r%2FPlexMetaManager&style=plastic
+    :target: https://www.reddit.com/r/PlexMetaManager/
+    :alt: Reddit
+
+.. image:: https://img.shields.io/github/sponsors/meisnate12?color=%238a2be2&style=plastic
+    :target: https://github.com/sponsors/meisnate12
+    :alt: GitHub Sponsors
 
 .. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
     :target: https://github.com/sponsors/meisnate12
-    :alt: GitHub Sponsor
+    :alt: Sponsor or Donate
 
 
 Overview
 ----------------------------------------------------------
 Unofficial Python bindings for the TMDb API. The goal is to make interaction with the API as easy as possible while emulating the endpoints as much as possible
```

