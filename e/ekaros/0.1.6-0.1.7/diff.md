# Comparing `tmp/ekaros-0.1.6.tar.gz` & `tmp/ekaros-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekaros-0.1.6.tar", max compression
+gzip compressed data, was "ekaros-0.1.7.tar", max compression
```

## Comparing `ekaros-0.1.6.tar` & `ekaros-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-24 19:26:56.357921 ekaros-0.1.6/LICENSE
--rw-r--r--   0        0        0     3345 2023-04-24 19:26:56.357921 ekaros-0.1.6/README.md
--rw-r--r--   0        0        0     2835 2023-04-24 19:27:23.441757 ekaros-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/__cli__.py
--rw-r--r--   0        0        0      815 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/__init__.py
--rw-r--r--   0        0        0       22 2023-04-24 19:27:23.393757 ekaros-0.1.6/src/ekaros/_version.py
--rw-r--r--   0        0        0        0 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/__init__.py
--rw-r--r--   0        0        0      195 2023-04-24 19:27:23.393757 ekaros-0.1.6/src/ekaros/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/task/__init__.yaml
--rw-r--r--   0        0        0      196 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/project.toml
--rw-r--r--   0        0        0        0 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/py.typed
--rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 ekaros-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-26 19:07:51.621558 ekaros-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3345 2023-04-26 19:07:51.621558 ekaros-0.1.7/README.md
+-rw-r--r--   0        0        0     2835 2023-04-26 19:08:24.203860 ekaros-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/__cli__.py
+-rw-r--r--   0        0        0      887 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-26 19:08:24.143856 ekaros-0.1.7/src/ekaros/_version.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-26 19:08:24.143856 ekaros-0.1.7/src/ekaros/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      196 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/project.toml
+-rw-r--r--   0        0        0        0 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/py.typed
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 ekaros-0.1.7/PKG-INFO
```

### Comparing `ekaros-0.1.6/LICENSE` & `ekaros-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.6/README.md` & `ekaros-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.6/pyproject.toml` & `ekaros-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ekaros"
-version = "0.1.6"
+version = "0.1.7"
 description = "A Python Library for Generative AI Art"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://ekaros.entelecheia.ai"
 repository = "https://github.com/entelecheia/ekaros"
 readme = "README.md"
 packages = [{ include = "ekaros", from = "src" }]
 
 [tool.poetry.scripts]
 ekaros = 'ekaros.__cli__:main'
 
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

### Comparing `ekaros-0.1.6/src/ekaros/__init__.py` & `ekaros-0.1.7/src/ekaros/__init__.py`

 * *Files 8% similar despite different names*

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
 global_config.hyfi_package_config_path = "pkg://ekaros.conf"
```

### Comparing `ekaros-0.1.6/src/ekaros/conf/dotenv/__init__.yaml` & `ekaros-0.1.7/src/ekaros/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.6/src/ekaros/conf/hydra/help/help.yaml` & `ekaros-0.1.7/src/ekaros/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.6/src/ekaros/conf/mode/__init__.yaml` & `ekaros-0.1.7/src/ekaros/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.6/src/ekaros/conf/path/__default__.yaml` & `ekaros-0.1.7/src/ekaros/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.6/src/ekaros/conf/path/__init__.yaml` & `ekaros-0.1.7/src/ekaros/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.6/PKG-INFO` & `ekaros-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ekaros
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python Library for Generative AI Art
 Home-page: https://ekaros.entelecheia.ai
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
 Project-URL: Repository, https://github.com/entelecheia/ekaros
 Description-Content-Type: text/markdown
 
 # Ekaros: A Python Library for Generative AI Art
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
```

