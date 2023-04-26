# Comparing `tmp/gdptools_pygeoapi_plugin-0.0.5.dev0.tar.gz` & `tmp/gdptools_pygeoapi_plugin-0.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdptools_pygeoapi_plugin-0.0.5.dev0.tar", max compression
+gzip compressed data, was "gdptools_pygeoapi_plugin-0.0.6.dev0.tar", max compression
```

## Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0.tar` & `gdptools_pygeoapi_plugin-0.0.6.dev0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1640 2022-09-08 23:56:38.751663 gdptools_pygeoapi_plugin-0.0.5.dev0/LICENSE.md
--rw-r--r--   0        0        0     2556 2022-09-08 23:56:38.701663 gdptools_pygeoapi_plugin-0.0.5.dev0/README.md
--rw-r--r--   0        0        0     2909 2023-04-04 15:17:00.572540 gdptools_pygeoapi_plugin-0.0.5.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-08 15:57:52.951663 gdptools_pygeoapi_plugin-0.0.5.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/__init__.py
--rw-r--r--   0        0        0     9014 2023-03-16 15:57:07.478580 gdptools_pygeoapi_plugin-0.0.5.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py
--rw-r--r--   0        0        0     2046 2023-03-16 16:50:55.466982 gdptools_pygeoapi_plugin-0.0.5.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py
--rw-r--r--   0        0        0     9261 2023-03-16 15:55:31.368763 gdptools_pygeoapi_plugin-0.0.5.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py
--rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 gdptools_pygeoapi_plugin-0.0.5.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1640 2022-09-08 23:56:38.751663 gdptools_pygeoapi_plugin-0.0.6.dev0/LICENSE.md
+-rw-r--r--   0        0        0     2556 2022-09-08 23:56:38.701663 gdptools_pygeoapi_plugin-0.0.6.dev0/README.md
+-rw-r--r--   0        0        0     2911 2023-04-26 14:30:24.126025 gdptools_pygeoapi_plugin-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-08 15:57:52.951663 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/__init__.py
+-rw-r--r--   0        0        0     9014 2023-03-16 15:57:07.478580 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py
+-rw-r--r--   0        0        0     2046 2023-03-16 16:50:55.466982 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py
+-rw-r--r--   0        0        0     9261 2023-03-16 15:55:31.368763 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py
+-rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 gdptools_pygeoapi_plugin-0.0.6.dev0/PKG-INFO
```

### Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0/LICENSE.md` & `gdptools_pygeoapi_plugin-0.0.6.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0/README.md` & `gdptools_pygeoapi_plugin-0.0.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0/pyproject.toml` & `gdptools_pygeoapi_plugin-0.0.6.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "gdptools-pygeoapi-plugin"
-version = "0.0.5-dev0"
+version = "0.0.6-dev0"
 description = "Gdptools Pygeoapi Plugin"
 authors = ["Richard McDonald <rmcd@usgs.gov>"]
 license = "LICENSE.md"
 readme = "README.md"
 homepage = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin"
 repository = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin"
 documentation = "https://gdptools-pygeoapi-plugin.readthedocs.io"
@@ -24,15 +24,15 @@
 Changelog = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin/releases"
 
 [tool.poetry.dependencies]
 python = "<3.10,>=3.9"
 click = "<8"
 pygeoapi = ">0.11.0"
 numpy = "^1.21.0"
-gdptools = "0.0.32"
+gdptools = ">=0.0.32"
 
 [tool.poetry.dev-dependencies]
 advbumpversion = "^1.2.0"
 pytest = "^6.2.4"
 coverage = {extras = ["toml"], version = "^5.4"}
 safety = "^1.10.3"
 mypy = "^0.910"
```

### Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py` & `gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py` & `gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py` & `gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.5.dev0/PKG-INFO` & `gdptools_pygeoapi_plugin-0.0.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gdptools-pygeoapi-plugin
-Version: 0.0.5.dev0
+Version: 0.0.6.dev0
 Summary: Gdptools Pygeoapi Plugin
 Home-page: https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin
 License: LICENSE.md
 Author: Richard McDonald
 Author-email: rmcd@usgs.gov
 Requires-Python: >=3.9,<3.10
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (<8)
-Requires-Dist: gdptools (==0.0.32)
+Requires-Dist: gdptools (>=0.0.32)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pygeoapi (>0.11.0)
 Project-URL: Changelog, https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin/releases
 Project-URL: Documentation, https://gdptools-pygeoapi-plugin.readthedocs.io
 Project-URL: Repository, https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin
 Description-Content-Type: text/markdown
```

