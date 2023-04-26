# Comparing `tmp/letsbuilda-pypi-3.2.0.tar.gz` & `tmp/letsbuilda-pypi-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsbuilda-pypi-3.2.0.tar", last modified: Wed Apr 26 02:25:59 2023, max compression
+gzip compressed data, was "letsbuilda-pypi-4.0.0.tar", last modified: Wed Apr 26 02:39:53 2023, max compression
```

## Comparing `letsbuilda-pypi-3.2.0.tar` & `letsbuilda-pypi-4.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:25:59.487751 letsbuilda-pypi-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 02:25:46.000000 letsbuilda-pypi-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 02:25:59.487751 letsbuilda-pypi-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 02:25:46.000000 letsbuilda-pypi-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-26 02:25:46.000000 letsbuilda-pypi-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:25:59.487751 letsbuilda-pypi-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:25:59.483751 letsbuilda-pypi-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:25:59.483751 letsbuilda-pypi-3.2.0/src/letsbuilda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:25:59.483751 letsbuilda-pypi-3.2.0/src/letsbuilda/pypi/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 02:25:46.000000 letsbuilda-pypi-3.2.0/src/letsbuilda/pypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-26 02:25:46.000000 letsbuilda-pypi-3.2.0/src/letsbuilda/pypi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-26 02:25:46.000000 letsbuilda-pypi-3.2.0/src/letsbuilda/pypi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:25:59.487751 letsbuilda-pypi-3.2.0/src/letsbuilda_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 02:25:59.000000 letsbuilda-pypi-3.2.0/src/letsbuilda_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 02:25:59.000000 letsbuilda-pypi-3.2.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:25:59.000000 letsbuilda-pypi-3.2.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 02:25:59.000000 letsbuilda-pypi-3.2.0/src/letsbuilda_pypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 02:25:59.000000 letsbuilda-pypi-3.2.0/src/letsbuilda_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:25:59.487751 letsbuilda-pypi-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-26 02:25:46.000000 letsbuilda-pypi-3.2.0/tests/test_rss_feed_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/letsbuilda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/tests/test_rss_feed_parsing.py
```

### Comparing `letsbuilda-pypi-3.2.0/LICENSE` & `letsbuilda-pypi-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-3.2.0/PKG-INFO` & `letsbuilda-pypi-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 3.2.0
+Version: 4.0.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-3.2.0/pyproject.toml` & `letsbuilda-pypi-4.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "letsbuilda-pypi"
-version = "3.2.0"
+version = "4.0.0"
 description = "A wrapper for PyPI's API and RSS feed"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `letsbuilda-pypi-3.2.0/src/letsbuilda/pypi/client.py` & `letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     async def get_rss_feed(self, feed_url: str) -> list[RSSPackageMetadata]:
         """Get the new packages RSS feed"""
         async with self.http_session.get(feed_url) as response:
             response_text = await response.text()
             rss_data = xmltodict.parse(response_text)["rss"]["channel"]["item"]
             return [RSSPackageMetadata.build_from(package_data) for package_data in rss_data]
 
-    async def get_package_metadata(self, package_name: str) -> PackageMetadata:
-        """Get the new packages RSS feed"""
-        async with self.http_session.get(f"https://pypi.org/pypi/{package_name}/json") as response:
-            return PackageMetadata.from_dict(await response.json())
-
-    async def get_package_metadata_for_release(self, package_name: str, package_version: str) -> PackageMetadata:
-        """Get the new packages RSS feed"""
-        async with self.http_session.get(f"https://pypi.org/pypi/{package_name}/{package_version}/json") as response:
+    async def get_package_metadata(self, package_name: str, package_version: str | None = None) -> PackageMetadata:
+        """Get metadata for a package"""
+        if package_version is not None:
+            url = f"https://pypi.org/pypi/{package_name}/{package_version}/json"
+        else:
+            url = f"https://pypi.org/pypi/{package_name}/json"
+        async with self.http_session.get(url) as response:
             return PackageMetadata.from_dict(await response.json())
```

### Comparing `letsbuilda-pypi-3.2.0/src/letsbuilda/pypi/models.py` & `letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/models.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-3.2.0/src/letsbuilda_pypi.egg-info/PKG-INFO` & `letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 3.2.0
+Version: 4.0.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-3.2.0/tests/test_rss_feed_parsing.py` & `letsbuilda-pypi-4.0.0/tests/test_rss_feed_parsing.py`

 * *Files identical despite different names*

