# Comparing `tmp/yarl-1.9.1.tar.gz` & `tmp/yarl-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yarl-1.9.1.tar", last modified: Fri Apr 21 14:28:38 2023, max compression
+gzip compressed data, was "yarl-1.9.2.tar", last modified: Tue Apr 25 17:43:54 2023, max compression
```

## Comparing `yarl-1.9.1.tar` & `yarl-1.9.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:28:38.097209 yarl-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-04-21 14:28:27.000000 yarl-1.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 14:28:27.000000 yarl-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-21 14:28:27.000000 yarl-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-04-21 14:28:38.097209 yarl-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-21 14:28:27.000000 yarl-1.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:28:38.093208 yarl-1.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:28:38.093208 yarl-1.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/_static/yarl-icon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38924 2023-04-21 14:28:27.000000 yarl-1.9.1/docs/yarl-icon-128x128.xcf
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 14:28:27.000000 yarl-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 14:28:38.097209 yarl-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-21 14:28:27.000000 yarl-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:28:38.097209 yarl-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_normalize_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_quoting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_update_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    44432 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_url_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_url_cmp_and_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_url_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_url_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-04-21 14:28:27.000000 yarl-1.9.1/tests/test_url_update_netloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:28:38.097209 yarl-1.9.1/yarl/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/_quoting.py
--rw-r--r--   0 runner    (1001) docker     (123)   467930 2023-04-21 14:28:37.000000 yarl-1.9.1/yarl/_quoting_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/_quoting_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/_quoting_c.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/_quoting_py.py
--rw-r--r--   0 runner    (1001) docker     (123)    37728 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/_url.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 14:28:27.000000 yarl-1.9.1/yarl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:28:38.097209 yarl-1.9.1/yarl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-04-21 14:28:38.000000 yarl-1.9.1/yarl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-21 14:28:38.000000 yarl-1.9.1/yarl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:28:38.000000 yarl-1.9.1/yarl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-21 14:28:38.000000 yarl-1.9.1/yarl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 14:28:38.000000 yarl-1.9.1/yarl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:43:54.632388 yarl-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-04-25 17:43:45.000000 yarl-1.9.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 17:43:45.000000 yarl-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 17:43:45.000000 yarl-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23222 2023-04-25 17:43:54.632388 yarl-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-25 17:43:45.000000 yarl-1.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:43:54.628388 yarl-1.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:43:54.628388 yarl-1.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/_static/yarl-icon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38924 2023-04-25 17:43:45.000000 yarl-1.9.2/docs/yarl-icon-128x128.xcf
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-25 17:43:45.000000 yarl-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 17:43:54.632388 yarl-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-25 17:43:45.000000 yarl-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:43:54.628388 yarl-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_normalize_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_quoting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_update_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44584 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_url_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_url_cmp_and_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_url_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_url_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-04-25 17:43:45.000000 yarl-1.9.2/tests/test_url_update_netloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:43:54.628388 yarl-1.9.2/yarl/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/_quoting.py
+-rw-r--r--   0 runner    (1001) docker     (123)   467930 2023-04-25 17:43:54.000000 yarl-1.9.2/yarl/_quoting_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/_quoting_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/_quoting_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/_quoting_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37935 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 17:43:45.000000 yarl-1.9.2/yarl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:43:54.632388 yarl-1.9.2/yarl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23222 2023-04-25 17:43:54.000000 yarl-1.9.2/yarl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-25 17:43:54.000000 yarl-1.9.2/yarl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:43:54.000000 yarl-1.9.2/yarl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 17:43:54.000000 yarl-1.9.2/yarl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 17:43:54.000000 yarl-1.9.2/yarl.egg-info/top_level.txt
```

### Comparing `yarl-1.9.1/CHANGES.rst` & `yarl-1.9.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,23 @@
     https://pip.pypa.io/en/latest/development/#adding-a-news-entry
     we named the news folder "changes".
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.9.2 (2023-04-25)
+==================
+
+Bugfixes
+--------
+
+- Fix regression with truediv and absolute URLs with empty paths causing the raw path to lack the leading ``/``. (`#854 <https://github.com/aio-libs/yarl/issues/854>`_)
+
+
 1.9.1 (2023-04-21)
 ==================
 
 Bugfixes
 --------
 
 - Marked tests that fail on older Python patch releases (< 3.7.10, < 3.8.8 and < 3.9.2) as expected to fail due to missing a security fix for CVE-2021-23336. (`#850 <https://github.com/aio-libs/yarl/issues/850>`_)
```

### Comparing `yarl-1.9.1/LICENSE` & `yarl-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/PKG-INFO` & `yarl-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarl
-Version: 1.9.1
+Version: 1.9.2
 Summary: Yet another URL library
 Home-page: https://github.com/aio-libs/yarl/
 Author: Andrew Svetlov
 Author-email: andrew.svetlov@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
@@ -238,14 +238,23 @@
     https://pip.pypa.io/en/latest/development/#adding-a-news-entry
     we named the news folder "changes".
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.9.2 (2023-04-25)
+==================
+
+Bugfixes
+--------
+
+- Fix regression with truediv and absolute URLs with empty paths causing the raw path to lack the leading ``/``. (`#854 <https://github.com/aio-libs/yarl/issues/854>`_)
+
+
 1.9.1 (2023-04-21)
 ==================
 
 Bugfixes
 --------
 
 - Marked tests that fail on older Python patch releases (< 3.7.10, < 3.8.8 and < 3.9.2) as expected to fail due to missing a security fix for CVE-2021-23336. (`#850 <https://github.com/aio-libs/yarl/issues/850>`_)
```

### Comparing `yarl-1.9.1/README.rst` & `yarl-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/docs/Makefile` & `yarl-1.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/docs/_static/yarl-icon-128x128.png` & `yarl-1.9.2/docs/_static/yarl-icon-128x128.png`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/docs/api.rst` & `yarl-1.9.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/docs/conf.py` & `yarl-1.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/docs/index.rst` & `yarl-1.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/docs/make.bat` & `yarl-1.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/docs/yarl-icon-128x128.xcf` & `yarl-1.9.2/docs/yarl-icon-128x128.xcf`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/setup.py` & `yarl-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_cache.py` & `yarl-1.9.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_cached_property.py` & `yarl-1.9.2/tests/test_cached_property.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_normalize_path.py` & `yarl-1.9.2/tests/test_normalize_path.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_quoting.py` & `yarl-1.9.2/tests/test_quoting.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_update_query.py` & `yarl-1.9.2/tests/test_update_query.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_url.py` & `yarl-1.9.2/tests/test_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -686,31 +686,35 @@
     assert URL("http://example.com/") == url.parent
 
 
 # truediv
 
 
 def test_div_root():
-    url = URL("http://example.com")
-    assert str(url / "path" / "to") == "http://example.com/path/to"
+    url = URL("http://example.com") / "path" / "to"
+    assert str(url) == "http://example.com/path/to"
+    assert url.raw_path == "/path/to"
 
 
 def test_div_root_with_slash():
-    url = URL("http://example.com/")
-    assert str(url / "path" / "to") == "http://example.com/path/to"
+    url = URL("http://example.com/") / "path" / "to"
+    assert str(url) == "http://example.com/path/to"
+    assert url.raw_path == "/path/to"
 
 
 def test_div():
-    url = URL("http://example.com/path")
-    assert str(url / "to") == "http://example.com/path/to"
+    url = URL("http://example.com/path") / "to"
+    assert str(url) == "http://example.com/path/to"
+    assert url.raw_path == "/path/to"
 
 
 def test_div_with_slash():
-    url = URL("http://example.com/path/")
-    assert str(url / "to") == "http://example.com/path/to"
+    url = URL("http://example.com/path/") / "to"
+    assert str(url) == "http://example.com/path/to"
+    assert url.raw_path == "/path/to"
 
 
 def test_div_path_starting_from_slash_is_forbidden():
     url = URL("http://example.com/path/")
     with pytest.raises(ValueError):
         url / "/to/others"
```

### Comparing `yarl-1.9.1/tests/test_url_build.py` & `yarl-1.9.2/tests/test_url_build.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_url_cmp_and_hash.py` & `yarl-1.9.2/tests/test_url_cmp_and_hash.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_url_parsing.py` & `yarl-1.9.2/tests/test_url_parsing.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_url_query.py` & `yarl-1.9.2/tests/test_url_query.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/tests/test_url_update_netloc.py` & `yarl-1.9.2/tests/test_url_update_netloc.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/yarl/__init__.pyi` & `yarl-1.9.2/yarl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/yarl/_quoting.py` & `yarl-1.9.2/yarl/_quoting.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/yarl/_quoting_c.c` & `yarl-1.9.2/yarl/_quoting_c.c`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/yarl/_quoting_c.pyx` & `yarl-1.9.2/yarl/_quoting_c.pyx`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/yarl/_quoting_py.py` & `yarl-1.9.2/yarl/_quoting_py.py`

 * *Files identical despite different names*

### Comparing `yarl-1.9.1/yarl/_url.py` & `yarl-1.9.2/yarl/_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -730,14 +730,18 @@
                 parsed.append(seg)
         parsed.reverse()
         old_path = self._val.path
         if old_path:
             parsed = [*old_path.rstrip("/").split("/"), *parsed]
         if self.is_absolute():
             parsed = _normalize_path_segments(parsed)
+            if parsed and parsed[0] != "":
+                # inject a leading slash when adding a path to an absolute URL
+                # where there was none before
+                parsed = ["", *parsed]
         new_path = "/".join(parsed)
         return URL(
             self._val._replace(path=new_path, query="", fragment=""), encoded=True
         )
 
     @classmethod
     def _normalize_path(cls, path):
```

### Comparing `yarl-1.9.1/yarl.egg-info/PKG-INFO` & `yarl-1.9.2/yarl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarl
-Version: 1.9.1
+Version: 1.9.2
 Summary: Yet another URL library
 Home-page: https://github.com/aio-libs/yarl/
 Author: Andrew Svetlov
 Author-email: andrew.svetlov@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
@@ -238,14 +238,23 @@
     https://pip.pypa.io/en/latest/development/#adding-a-news-entry
     we named the news folder "changes".
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.9.2 (2023-04-25)
+==================
+
+Bugfixes
+--------
+
+- Fix regression with truediv and absolute URLs with empty paths causing the raw path to lack the leading ``/``. (`#854 <https://github.com/aio-libs/yarl/issues/854>`_)
+
+
 1.9.1 (2023-04-21)
 ==================
 
 Bugfixes
 --------
 
 - Marked tests that fail on older Python patch releases (< 3.7.10, < 3.8.8 and < 3.9.2) as expected to fail due to missing a security fix for CVE-2021-23336. (`#850 <https://github.com/aio-libs/yarl/issues/850>`_)
```

### Comparing `yarl-1.9.1/yarl.egg-info/SOURCES.txt` & `yarl-1.9.2/yarl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

