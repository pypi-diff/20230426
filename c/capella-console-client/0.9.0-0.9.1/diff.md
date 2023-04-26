# Comparing `tmp/capella-console-client-0.9.0.tar.gz` & `tmp/capella_console_client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capella-console-client-0.9.0.tar", max compression
+gzip compressed data, was "capella_console_client-0.9.1.tar", max compression
```

## Comparing `capella-console-client-0.9.0.tar` & `capella_console_client-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1111 2022-09-23 21:27:17.661601 capella-console-client-0.9.0/LICENSE
--rw-r--r--   0        0        0     2867 2022-09-23 21:27:17.662327 capella-console-client-0.9.0/README.md
--rw-r--r--   0        0        0       41 2021-07-16 22:27:41.503910 capella-console-client-0.9.0/capella_console_client/__init__.py
--rw-r--r--   0        0        0     8979 2022-09-23 21:27:17.663296 capella-console-client-0.9.0/capella_console_client/assets.py
--rw-r--r--   0        0        0        0 2021-08-17 22:29:19.808647 capella-console-client-0.9.0/capella_console_client/cli/__init__.py
--rw-r--r--   0        0        0     2686 2022-09-23 21:27:17.664104 capella-console-client-0.9.0/capella_console_client/cli/cache.py
--rw-r--r--   0        0        0     5503 2022-09-23 21:27:17.664700 capella-console-client-0.9.0/capella_console_client/cli/checkout.py
--rw-r--r--   0        0        0      115 2021-08-17 22:29:19.810397 capella-console-client-0.9.0/capella_console_client/cli/client_singleton.py
--rw-r--r--   0        0        0     2989 2022-09-23 21:27:17.665209 capella-console-client-0.9.0/capella_console_client/cli/config.py
--rw-r--r--   0        0        0      940 2022-01-05 19:30:55.208666 capella-console-client-0.9.0/capella_console_client/cli/info.py
--rw-r--r--   0        0        0     4159 2022-09-23 21:27:17.665668 capella-console-client-0.9.0/capella_console_client/cli/orders.py
--rw-r--r--   0        0        0      281 2022-09-23 21:27:17.666097 capella-console-client-0.9.0/capella_console_client/cli/prompt_helpers.py
--rw-r--r--   0        0        0      592 2022-09-23 21:27:17.666571 capella-console-client-0.9.0/capella_console_client/cli/sanitize.py
--rw-r--r--   0        0        0    10813 2022-09-23 21:27:17.667463 capella-console-client-0.9.0/capella_console_client/cli/search.py
--rw-r--r--   0        0        0     4257 2022-09-23 21:27:17.668170 capella-console-client-0.9.0/capella_console_client/cli/settings.py
--rw-r--r--   0        0        0        0 2021-08-17 22:29:19.813402 capella-console-client-0.9.0/capella_console_client/cli/user_searches/__init__.py
--rw-r--r--   0        0        0     2086 2022-09-23 21:27:17.668830 capella-console-client-0.9.0/capella_console_client/cli/user_searches/core.py
--rw-r--r--   0        0        0     2298 2022-09-23 21:27:17.669589 capella-console-client-0.9.0/capella_console_client/cli/user_searches/my_search_queries.py
--rw-r--r--   0        0        0     2378 2022-09-23 21:27:17.670373 capella-console-client-0.9.0/capella_console_client/cli/user_searches/my_search_results.py
--rw-r--r--   0        0        0      402 2022-09-23 21:27:17.671136 capella-console-client-0.9.0/capella_console_client/cli/user_searches/my_searches.py
--rw-r--r--   0        0        0     4675 2022-09-23 21:27:17.672064 capella-console-client-0.9.0/capella_console_client/cli/validate.py
--rw-r--r--   0        0        0     2761 2022-09-23 21:27:17.673302 capella-console-client-0.9.0/capella_console_client/cli/visualize.py
--rw-r--r--   0        0        0     2134 2021-11-18 00:11:05.287150 capella-console-client-0.9.0/capella_console_client/cli/wizard.py
--rw-r--r--   0        0        0      562 2022-01-05 19:30:55.209293 capella-console-client-0.9.0/capella_console_client/cli/workflows.py
--rw-r--r--   0        0        0    29505 2022-09-23 21:27:17.674380 capella-console-client-0.9.0/capella_console_client/client.py
--rw-r--r--   0        0        0     2314 2022-09-23 21:27:17.676323 capella-console-client-0.9.0/capella_console_client/config.py
--rw-r--r--   0        0        0     1166 2022-08-03 18:39:55.992257 capella-console-client-0.9.0/capella_console_client/enumerations.py
--rw-r--r--   0        0        0     2703 2022-09-23 21:27:17.678136 capella-console-client-0.9.0/capella_console_client/exceptions.py
--rw-r--r--   0        0        0     1408 2022-09-23 21:27:17.680642 capella-console-client-0.9.0/capella_console_client/hooks.py
--rw-r--r--   0        0        0      158 2021-10-08 17:07:19.790447 capella-console-client-0.9.0/capella_console_client/logconf.py
--rw-r--r--   0        0        0        0 2022-06-07 21:43:20.252574 capella-console-client-0.9.0/capella_console_client/py.typed
--rw-r--r--   0        0        0     7002 2022-09-23 21:27:17.681789 capella-console-client-0.9.0/capella_console_client/search.py
--rw-r--r--   0        0        0     6307 2022-09-23 21:27:17.682610 capella-console-client-0.9.0/capella_console_client/session.py
--rw-r--r--   0        0        0      933 2022-09-23 21:27:17.683667 capella-console-client-0.9.0/capella_console_client/sort.py
--rw-r--r--   0        0        0     2095 2022-09-23 21:27:17.684793 capella-console-client-0.9.0/capella_console_client/validate.py
--rw-r--r--   0        0        0       22 2022-09-23 21:27:17.686113 capella-console-client-0.9.0/capella_console_client/version.py
--rw-r--r--   0        0        0     2300 2022-09-23 21:28:31.454511 capella-console-client-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4422 2022-09-23 21:28:41.326132 capella-console-client-0.9.0/setup.py
--rw-r--r--   0        0        0     4723 2022-09-23 21:28:41.326451 capella-console-client-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1111 2022-09-23 21:27:17.661601 capella_console_client-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2867 2022-09-23 21:27:17.662327 capella_console_client-0.9.1/README.md
+-rw-r--r--   0        0        0       41 2021-07-16 22:27:41.503910 capella_console_client-0.9.1/capella_console_client/__init__.py
+-rw-r--r--   0        0        0     8979 2022-09-23 21:27:17.663296 capella_console_client-0.9.1/capella_console_client/assets.py
+-rw-r--r--   0        0        0        0 2021-08-17 22:29:19.808647 capella_console_client-0.9.1/capella_console_client/cli/__init__.py
+-rw-r--r--   0        0        0     2686 2022-09-23 21:27:17.664104 capella_console_client-0.9.1/capella_console_client/cli/cache.py
+-rw-r--r--   0        0        0     5503 2022-09-23 21:27:17.664700 capella_console_client-0.9.1/capella_console_client/cli/checkout.py
+-rw-r--r--   0        0        0      115 2021-08-17 22:29:19.810397 capella_console_client-0.9.1/capella_console_client/cli/client_singleton.py
+-rw-r--r--   0        0        0     2989 2022-09-23 21:27:17.665209 capella_console_client-0.9.1/capella_console_client/cli/config.py
+-rw-r--r--   0        0        0      940 2022-01-05 19:30:55.208666 capella_console_client-0.9.1/capella_console_client/cli/info.py
+-rw-r--r--   0        0        0     4159 2022-09-23 21:27:17.665668 capella_console_client-0.9.1/capella_console_client/cli/orders.py
+-rw-r--r--   0        0        0      281 2022-09-23 21:27:17.666097 capella_console_client-0.9.1/capella_console_client/cli/prompt_helpers.py
+-rw-r--r--   0        0        0      592 2022-09-23 21:27:17.666571 capella_console_client-0.9.1/capella_console_client/cli/sanitize.py
+-rw-r--r--   0        0        0    10813 2022-09-23 21:27:17.667463 capella_console_client-0.9.1/capella_console_client/cli/search.py
+-rw-r--r--   0        0        0     4257 2022-09-23 21:27:17.668170 capella_console_client-0.9.1/capella_console_client/cli/settings.py
+-rw-r--r--   0        0        0        0 2021-08-17 22:29:19.813402 capella_console_client-0.9.1/capella_console_client/cli/user_searches/__init__.py
+-rw-r--r--   0        0        0     2086 2022-09-23 21:27:17.668830 capella_console_client-0.9.1/capella_console_client/cli/user_searches/core.py
+-rw-r--r--   0        0        0     2298 2022-09-23 21:27:17.669589 capella_console_client-0.9.1/capella_console_client/cli/user_searches/my_search_queries.py
+-rw-r--r--   0        0        0     2378 2022-09-23 21:27:17.670373 capella_console_client-0.9.1/capella_console_client/cli/user_searches/my_search_results.py
+-rw-r--r--   0        0        0      402 2022-09-23 21:27:17.671136 capella_console_client-0.9.1/capella_console_client/cli/user_searches/my_searches.py
+-rw-r--r--   0        0        0     4675 2022-09-23 21:27:17.672064 capella_console_client-0.9.1/capella_console_client/cli/validate.py
+-rw-r--r--   0        0        0     2761 2022-09-23 21:27:17.673302 capella_console_client-0.9.1/capella_console_client/cli/visualize.py
+-rw-r--r--   0        0        0     2134 2021-11-18 00:11:05.287150 capella_console_client-0.9.1/capella_console_client/cli/wizard.py
+-rw-r--r--   0        0        0      562 2022-01-05 19:30:55.209293 capella_console_client-0.9.1/capella_console_client/cli/workflows.py
+-rw-r--r--   0        0        0    29505 2022-09-23 21:27:17.674380 capella_console_client-0.9.1/capella_console_client/client.py
+-rw-r--r--   0        0        0     2314 2022-09-23 21:27:17.676323 capella_console_client-0.9.1/capella_console_client/config.py
+-rw-r--r--   0        0        0     1166 2022-08-03 18:39:55.992257 capella_console_client-0.9.1/capella_console_client/enumerations.py
+-rw-r--r--   0        0        0     2703 2022-09-23 21:27:17.678136 capella_console_client-0.9.1/capella_console_client/exceptions.py
+-rw-r--r--   0        0        0     1408 2022-09-23 21:27:17.680642 capella_console_client-0.9.1/capella_console_client/hooks.py
+-rw-r--r--   0        0        0      158 2021-10-08 17:07:19.790447 capella_console_client-0.9.1/capella_console_client/logconf.py
+-rw-r--r--   0        0        0        0 2022-06-07 21:43:20.252574 capella_console_client-0.9.1/capella_console_client/py.typed
+-rw-r--r--   0        0        0     8161 2022-11-05 00:25:32.043203 capella_console_client-0.9.1/capella_console_client/search.py
+-rw-r--r--   0        0        0     6307 2022-09-23 21:27:17.682610 capella_console_client-0.9.1/capella_console_client/session.py
+-rw-r--r--   0        0        0      933 2022-09-23 21:27:17.683667 capella_console_client-0.9.1/capella_console_client/sort.py
+-rw-r--r--   0        0        0     1137 2022-11-04 23:15:33.285231 capella_console_client-0.9.1/capella_console_client/test-govcloud-cp.py
+-rw-r--r--   0        0        0     2095 2022-09-23 21:27:17.684793 capella_console_client-0.9.1/capella_console_client/validate.py
+-rw-r--r--   0        0        0      101 2022-11-05 00:25:32.044169 capella_console_client-0.9.1/capella_console_client/version.py
+-rw-r--r--   0        0        0     2346 2022-11-05 00:25:32.047501 capella_console_client-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 capella_console_client-0.9.1/setup.py
+-rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 capella_console_client-0.9.1/PKG-INFO
```

### Comparing `capella-console-client-0.9.0/LICENSE` & `capella_console_client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/README.md` & `capella_console_client-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/assets.py` & `capella_console_client-0.9.1/capella_console_client/assets.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/cache.py` & `capella_console_client-0.9.1/capella_console_client/cli/cache.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/checkout.py` & `capella_console_client-0.9.1/capella_console_client/cli/checkout.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/config.py` & `capella_console_client-0.9.1/capella_console_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/info.py` & `capella_console_client-0.9.1/capella_console_client/cli/info.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/orders.py` & `capella_console_client-0.9.1/capella_console_client/cli/orders.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/sanitize.py` & `capella_console_client-0.9.1/capella_console_client/cli/sanitize.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/search.py` & `capella_console_client-0.9.1/capella_console_client/cli/search.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/settings.py` & `capella_console_client-0.9.1/capella_console_client/cli/settings.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/user_searches/core.py` & `capella_console_client-0.9.1/capella_console_client/cli/user_searches/core.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/user_searches/my_search_queries.py` & `capella_console_client-0.9.1/capella_console_client/cli/user_searches/my_search_queries.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/user_searches/my_search_results.py` & `capella_console_client-0.9.1/capella_console_client/cli/user_searches/my_search_results.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/validate.py` & `capella_console_client-0.9.1/capella_console_client/cli/validate.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/visualize.py` & `capella_console_client-0.9.1/capella_console_client/cli/visualize.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/wizard.py` & `capella_console_client-0.9.1/capella_console_client/cli/wizard.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/cli/workflows.py` & `capella_console_client-0.9.1/capella_console_client/cli/workflows.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/client.py` & `capella_console_client-0.9.1/capella_console_client/client.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/config.py` & `capella_console_client-0.9.1/capella_console_client/config.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/enumerations.py` & `capella_console_client-0.9.1/capella_console_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/exceptions.py` & `capella_console_client-0.9.1/capella_console_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/hooks.py` & `capella_console_client-0.9.1/capella_console_client/hooks.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/search.py` & `capella_console_client-0.9.1/capella_console_client/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,21 +20,40 @@
 )
 from capella_console_client.hooks import retry_if_http_status_error, log_attempt_delay
 
 
 @dataclass
 class SearchResult:
 
-    request_body: Dict[str, Any]
+    request_body: Dict[str, Any] = field(default_factory=dict)
     _pages: List[Dict[str, Any]] = field(default_factory=list)
     _features: List[Dict[str, Any]] = field(default_factory=list)
 
-    def add(self, page: Dict[str, Any]):
+    def add(self, page: Dict[str, Any], keep_duplicates: bool = False) -> int:
+        if not keep_duplicates:
+            page = self._filter_dupes(page)
         self._pages.append(page)
         self._features.extend(page["features"])
+        return len(page["features"])
+
+    def _filter_dupes(self, page: Dict[str, Any]) -> Dict[str, Any]:
+        # drop duplicates within page features
+        page_stac_ids = [feat["id"] for feat in page["features"]]
+        set_page_stac_ids = set(page_stac_ids)
+
+        if len(set_page_stac_ids) != len(page["features"]):
+            page["features"] = [page["features"][page_stac_ids.index(p_id)] for p_id in set_page_stac_ids]
+
+        # drop duplicates within SearchResult
+        dupes = set_page_stac_ids.intersection(self.stac_ids)
+
+        if dupes:
+            page["features"] = [p for p in page["features"] if p["id"] not in dupes]
+
+        return page
 
     # backwards compability
     def __getitem__(self, key):
         return self._features.__getitem__(key)
 
     def __iter__(self):
         return self._features.__iter__()
@@ -48,14 +67,21 @@
     def to_feature_collection(self):
         return {"type": "FeatureCollection", "features": self._features}
 
     @property
     def stac_ids(self):
         return [item["id"] for item in self._features]
 
+    def merge(self, other: "SearchResult", keep_duplicates: bool = False) -> "SearchResult":
+        copy = deepcopy(self)
+        for page in other._pages:
+            copy.add(page=page, keep_duplicates=keep_duplicates)
+
+        return copy
+
 
 class StacSearch:
     def __init__(self, session: CapellaConsoleSession, **kwargs) -> None:
         cur_kwargs = deepcopy(kwargs)
         self.session = session
         self.payload: Dict[str, Any] = {}
 
@@ -139,18 +165,21 @@
         search_result = SearchResult(request_body=self.payload)
         next_href = None
 
         while True:
             _log_page_query(page_cnt, len(search_result), self.payload["limit"])
             page_data = _page_search(self.session, self.payload, next_href)
             number_matched = page_data["numberMatched"]
-            search_result.add(page_data)
+            items_added = search_result.add(page_data)
 
             limit_reached = len(search_result) >= requested_limit or len(search_result) >= number_matched
-            if limit_reached:
+
+            # all dupes
+            size_unchanged = items_added == 0
+            if limit_reached or size_unchanged:
                 break
 
             next_href = _get_next_page_href(page_data)
             if next_href is None:
                 break
 
             if page_cnt == 1:
@@ -192,15 +221,14 @@
 @retry(
     retry_on_exception=retry_if_http_status_error,
     wait_func=log_attempt_delay,
     wait_exponential_multiplier=1000,
     stop_max_delay=16000,
 )
 def _page_search(session: CapellaConsoleSession, payload: Dict[str, Any], next_href: str = None) -> Dict[str, Any]:
-
     if next_href:
         # STAC API to return normalized asset hrefs, not api gateway - fixing this here ...
         url_parsed = urlparse(next_href)
         if url_parsed.netloc != urlparse(session.search_url).netloc:
             next_href = f"{session.search_url}?{url_parsed.query}"
 
     url = session.search_url if next_href is None else next_href
```

### Comparing `capella-console-client-0.9.0/capella_console_client/session.py` & `capella_console_client-0.9.1/capella_console_client/session.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/sort.py` & `capella_console_client-0.9.1/capella_console_client/sort.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/capella_console_client/validate.py` & `capella_console_client-0.9.1/capella_console_client/validate.py`

 * *Files identical despite different names*

### Comparing `capella-console-client-0.9.0/pyproject.toml` & `capella_console_client-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "capella-console-client"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python SDK for api.capellaspace.com (search, order, download)"
 authors = ["Thomas Beyer <thomas.beyer@capellaspace.com>"]
 repository = "https://github.com/capellaspace/console-client"
 documentation = "https://capella-console-client.readthedocs.io/"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     # supported python versions
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
     "Topic :: Scientific/Engineering :: Image Processing",
 ]
 keywords = [ "CapellaSpace", "Earth Observation", "Capella Console", "Synthetic Aperture Radar", "SAR" ]
 readme = "README.md"
 license = "MIT"
 
@@ -42,15 +43,15 @@
 sphinx-autodoc-typehints = {version = "^1.19.2", optional = true}
 
 [tool.poetry.extras]
 wizard = ["typer", "questionary", "tabulate"]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinx-autobuild", "sphinx-copybutton", "sphinx-autodoc-typehints"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
+pytest = "^7.2.0"
 pytest-cov = "^3.0.0"
 pytest-httpx = "^0.21.0"
 pytest-html = "^3.1.1"
 coveralls = "^3.3.1"
 black = "^22.8.0"
 mypy = "^0.971"
 rope = "^1.3.0"
```

### Comparing `capella-console-client-0.9.0/setup.py` & `capella_console_client-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 
 entry_points = \
 {'console_scripts': ['capella-console-wizard = '
                      'capella_console_client.cli.wizard:main']}
 
 setup_kwargs = {
     'name': 'capella-console-client',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Python SDK for api.capellaspace.com (search, order, download)',
     'long_description': '# 🛰️ capella-console-client 🐐\n\n[![Version](https://img.shields.io/pypi/v/capella-console-client.svg)](https://pypi.org/project/capella-console-client/)\n[![License](https://img.shields.io/pypi/l/capella-console-client.svg)](#)\n[![CI](https://github.com/capellaspace/console-client/workflows/CI/badge.svg)](#)\n[![Coverage](https://coveralls.io/repos/github/capellaspace/console-client/badge.svg?branch=main)](https://coveralls.io/github/capellaspace/console-client)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/capella-console-client.svg)](https://pypi.org/project/capella-console-client/)\n[![Documentation](https://readthedocs.org/projects/capella-console-client/badge/?version=main)](https://capella-console-client.readthedocs.io)\n\nPython SDK for api.capellaspace.com (search, order, download)\n\n\n## Installation\n\n```bash\npip install capella-console-client\n```\n\n## Requirements\n\n* python >= 3.7\n* `capella-console-client` requires an active account on [console.capellaspace.com](https://console.capellaspace.com/). Sign up for an account at [https://www.capellaspace.com/community/](https://www.capellaspace.com/community/).\n\n\n## Usage\n\n![Quickstart](docs/images/quickstart.gif)\n\n```python\nfrom capella_console_client import CapellaConsoleClient\n\n# you will be prompted for console user (user@email.com)/ password before authenticating\nclient = CapellaConsoleClient(\n    verbose=True\n)\n\n# search for 2 open-data products\nstac_items = client.search(\n    instrument_mode="spotlight",\n    product_type__in=["SLC", "GEO"],\n    collections=["capella-open-data"],\n    limit=2\n)\n\n# order\norder_id = client.submit_order(items=stac_items, omit_search=True)\n\n# download\nproduct_paths = client.download_products(\n    order_id=order_id, \n    local_dir=\'/tmp\',\n    show_progress=True\n)\n```\n\n\n## Documentation\n\nThe documentation for `capella-console-client` can be found [here](https://capella-console-client.readthedocs.io).\n\n## 🧙\u200d capella-console-wizard 🧙\u200d♂️\nstarting with `capella-console-client>=0.8.0` the SDK ships with an interactive wizard-like CLI: `capella-console-wizard` \n\n### Installation\n```\npip install capella-console-client[wizard]\n```\n\n### Usage\n```\ncapella-console-wizard --help\n```\n\nsee \n\n\n## Support\n\nPlease [open an issue](https://github.com/capellaspace/console-client/issues/new)\nwith enough information for us to reproduce your problem.\nA [minimal, reproducible example](https://stackoverflow.com/help/minimal-reproducible-example)\nwould be very helpful.\n\n## Contributing\n\nContributions are very much welcomed and appreciated. See [how to contribute](https://capella-console-client.readthedocs.io/en/main/pages/contributors.html) for more information.\n\n\n## License\n• Licensed under the [MIT License](https://github.com/capellaspace/console-client/blob/master/LICENSE) • Copyright 2022 • Capella Space •\n',
     'author': 'Thomas Beyer',
     'author_email': 'thomas.beyer@capellaspace.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/capellaspace/console-client',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
```

### Comparing `capella-console-client-0.9.0/PKG-INFO` & `capella_console_client-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: capella-console-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python SDK for api.capellaspace.com (search, order, download)
 Home-page: https://github.com/capellaspace/console-client
 License: MIT
 Keywords: CapellaSpace,Earth Observation,Capella Console,Synthetic Aperture Radar,SAR
 Author: Thomas Beyer
 Author-email: thomas.beyer@capellaspace.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Provides-Extra: wizard
```

