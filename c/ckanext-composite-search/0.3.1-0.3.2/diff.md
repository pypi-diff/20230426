# Comparing `tmp/ckanext-composite-search-0.3.1.tar.gz` & `tmp/ckanext-composite-search-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-composite-search-0.3.1.tar", last modified: Tue Aug  9 18:38:33 2022, max compression
+gzip compressed data, was "ckanext-composite-search-0.3.2.tar", last modified: Wed Apr 26 17:03:24 2023, max compression
```

## Comparing `ckanext-composite-search-0.3.1.tar` & `ckanext-composite-search-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      217 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2102 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1594 2022-08-09 14:25:57.000000 ckanext-composite-search-0.3.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/ckanext/composite_search/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/ckanext/composite_search/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9716 2022-08-09 13:57:10.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/assets/bundle.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)    54209 2022-08-09 13:57:10.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/assets/bundle.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2538 2022-08-09 18:34:00.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/assets/composite_search-module.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      390 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      358 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/ckanext/composite_search/plugin/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/plugin/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/plugin/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2265 2022-08-09 15:24:46.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/plugin/default.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/ckanext/composite_search/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       79 2022-08-09 13:56:06.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      685 2022-08-09 15:18:28.000000 ckanext-composite-search-0.3.1/ckanext/composite_search/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/ckanext/example_composite_search/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/example_composite_search/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      329 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.1/ckanext/example_composite_search/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2102 2022-08-09 18:38:33.000000 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1034 2022-08-09 18:38:33.000000 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-08-09 18:38:33.000000 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2022-08-09 18:38:33.000000 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-08-09 18:38:33.000000 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       20 2022-08-09 18:38:33.000000 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-08-09 18:38:33.000000 ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2022-08-09 13:54:08.000000 ckanext-composite-search-0.3.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1741 2022-08-09 18:38:33.912918 ckanext-composite-search-0.3.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      259 2022-08-09 14:00:45.000000 ckanext-composite-search-0.3.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      217 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2102 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1594 2022-08-09 14:25:57.000000 ckanext-composite-search-0.3.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/ckanext/composite_search/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/ckanext/composite_search/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9716 2022-08-09 13:57:10.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/assets/bundle.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    54209 2022-08-09 13:57:10.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/assets/bundle.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2538 2022-08-09 18:34:00.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/assets/composite_search-module.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      390 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      358 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/ckanext/composite_search/plugin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/plugin/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1954 2023-04-26 17:01:53.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/plugin/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2265 2022-08-09 15:24:46.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/plugin/default.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/ckanext/composite_search/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       79 2022-08-09 13:56:06.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      685 2022-08-09 15:18:28.000000 ckanext-composite-search-0.3.2/ckanext/composite_search/utils.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/ckanext/example_composite_search/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/example_composite_search/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      329 2022-08-04 11:50:40.000000 ckanext-composite-search-0.3.2/ckanext/example_composite_search/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2102 2023-04-26 17:03:24.000000 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1034 2023-04-26 17:03:24.000000 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-26 17:03:24.000000 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2023-04-26 17:03:24.000000 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-26 17:03:24.000000 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       20 2023-04-26 17:03:24.000000 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-26 17:03:24.000000 ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2022-08-09 13:54:08.000000 ckanext-composite-search-0.3.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1741 2023-04-26 17:03:24.922666 ckanext-composite-search-0.3.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      259 2022-08-09 14:00:45.000000 ckanext-composite-search-0.3.2/setup.py
```

### Comparing `ckanext-composite-search-0.3.1/LICENSE` & `ckanext-composite-search-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/PKG-INFO` & `ckanext-composite-search-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-composite-search
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/DataShades/ckanext-composite-search
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-composite-search-0.3.1/README.md` & `ckanext-composite-search-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/ckanext/composite_search/assets/bundle.css` & `ckanext-composite-search-0.3.2/ckanext/composite_search/assets/bundle.css`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/ckanext/composite_search/assets/bundle.js` & `ckanext-composite-search-0.3.2/ckanext/composite_search/assets/bundle.js`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/ckanext/composite_search/assets/composite_search-module.js` & `ckanext-composite-search-0.3.2/ckanext/composite_search/assets/composite_search-module.js`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/ckanext/composite_search/plugin/base.py` & `ckanext-composite-search-0.3.2/ckanext/composite_search/plugin/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,7 +55,9 @@
         ]
 
         for plugin in plugins.PluginImplementations(ICompositeSearch):
             search_params, params = plugin.before_composite_search(
                 search_params, params
             )
         return search_params
+
+    before_dataset_search = before_search
```

### Comparing `ckanext-composite-search-0.3.1/ckanext/composite_search/plugin/default.py` & `ckanext-composite-search-0.3.2/ckanext/composite_search/plugin/default.py`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/ckanext/composite_search/utils.py` & `ckanext-composite-search-0.3.2/ckanext/composite_search/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/PKG-INFO` & `ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-composite-search
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/DataShades/ckanext-composite-search
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-composite-search-0.3.1/ckanext_composite_search.egg-info/SOURCES.txt` & `ckanext-composite-search-0.3.2/ckanext_composite_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-composite-search-0.3.1/setup.cfg` & `ckanext-composite-search-0.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-composite-search
-version = 0.3.1
+version = 0.3.2
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-composite-search
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

