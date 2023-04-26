# Comparing `tmp/oikonomika-0.1.1.tar.gz` & `tmp/oikonomika-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oikonomika-0.1.1.tar", max compression
+gzip compressed data, was "oikonomika-0.1.2.tar", max compression
```

## Comparing `oikonomika-0.1.1.tar` & `oikonomika-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-24 19:25:40.326856 oikonomika-0.1.1/LICENSE
--rw-r--r--   0        0        0     3735 2023-04-24 19:25:40.326856 oikonomika-0.1.1/README.md
--rw-r--r--   0        0        0     2867 2023-04-24 19:26:05.383178 oikonomika-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      178 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/__cli__.py
--rw-r--r--   0        0        0      819 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/__init__.py
--rw-r--r--   0        0        0       22 2023-04-24 19:26:05.331177 oikonomika-0.1.1/src/oikonomika/_version.py
--rw-r--r--   0        0        0        0 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/__init__.py
--rw-r--r--   0        0        0      203 2023-04-24 19:26:05.331177 oikonomika-0.1.1/src/oikonomika/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/task/__init__.yaml
--rw-r--r--   0        0        0      204 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/project.toml
--rw-r--r--   0        0        0        0 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/py.typed
--rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 oikonomika-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-26 19:06:18.859751 oikonomika-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3735 2023-04-26 19:06:18.859751 oikonomika-0.1.2/README.md
+-rw-r--r--   0        0        0     2867 2023-04-26 19:06:53.391684 oikonomika-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      178 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/__cli__.py
+-rw-r--r--   0        0        0      891 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-26 19:06:53.331684 oikonomika-0.1.2/src/oikonomika/_version.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-26 19:06:53.331684 oikonomika-0.1.2/src/oikonomika/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      204 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/project.toml
+-rw-r--r--   0        0        0        0 2023-04-26 19:06:18.863751 oikonomika-0.1.2/src/oikonomika/py.typed
+-rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 oikonomika-0.1.2/PKG-INFO
```

### Comparing `oikonomika-0.1.1/LICENSE` & `oikonomika-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.1/README.md` & `oikonomika-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.1/pyproject.toml` & `oikonomika-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "oikonomika"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python Library for Economic Analysis"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://oikonomika.entelecheia.ai"
 repository = "https://github.com/entelecheia/oikonomika"
 readme = "README.md"
 packages = [{ include = "oikonomika", from = "src" }]
 
 [tool.poetry.scripts]
 oikonomika = 'oikonomika.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.13"
+hyfi = "^0.2.20"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
```

### Comparing `oikonomika-0.1.1/src/oikonomika/__init__.py` & `oikonomika-0.1.2/src/oikonomika/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Read and parse pyproject.toml
 current_dir = os.path.dirname(os.path.abspath(__file__))
 about_path = os.path.join(current_dir, "conf", "about", "__init__.yaml")
 
 about_data = HyFI.load(about_path)
 
 # Extract package information
+about._package_name_ = about_data.get("_package_name_", "package_name")
 about.name = about_data.get("name", "package name")
 about.authors = about_data.get("authors", ["Author name"])
 about.description = about_data.get("description", "package description")
 about.homepage = about_data.get("homepage", "https://package.homepage")
 about.license = about_data.get("license", "MIT")
 about.version = __version__
 global_config.hyfi_package_config_path = "pkg://oikonomika.conf"
```

### Comparing `oikonomika-0.1.1/src/oikonomika/conf/dotenv/__init__.yaml` & `oikonomika-0.1.2/src/oikonomika/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.1/src/oikonomika/conf/hydra/help/help.yaml` & `oikonomika-0.1.2/src/oikonomika/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.1/src/oikonomika/conf/mode/__init__.yaml` & `oikonomika-0.1.2/src/oikonomika/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.1/src/oikonomika/conf/path/__default__.yaml` & `oikonomika-0.1.2/src/oikonomika/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.1/src/oikonomika/conf/path/__init__.yaml` & `oikonomika-0.1.2/src/oikonomika/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.1/PKG-INFO` & `oikonomika-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: oikonomika
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python Library for Economic Analysis
 Home-page: https://oikonomika.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.13,<0.3.0)
+Requires-Dist: hyfi (>=0.2.20,<0.3.0)
 Project-URL: Repository, https://github.com/entelecheia/oikonomika
 Description-Content-Type: text/markdown
 
 # Oikonomika: A Python Library for Economic Analysis
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
```

