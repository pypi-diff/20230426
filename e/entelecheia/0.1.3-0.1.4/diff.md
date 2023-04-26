# Comparing `tmp/entelecheia-0.1.3.tar.gz` & `tmp/entelecheia-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.1.3.tar", max compression
+gzip compressed data, was "entelecheia-0.1.4.tar", max compression
```

## Comparing `entelecheia-0.1.3.tar` & `entelecheia-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-04-22 21:41:24.555870 entelecheia-0.1.3/LICENSE
--rw-r--r--   0        0        0     1016 2023-04-22 21:41:24.559870 entelecheia-0.1.3/README.md
--rw-r--r--   0        0        0     2981 2023-04-22 21:41:59.809132 entelecheia-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      179 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      820 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-04-22 21:41:59.741129 entelecheia-0.1.3/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      321 2023-04-22 21:41:59.741129 entelecheia-0.1.3/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/conf/task/__init__.yaml
--rw-r--r--   0        0        0        0 2023-04-22 21:41:24.559870 entelecheia-0.1.3/src/entelecheia/py.typed
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 entelecheia-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-26 10:27:06.308644 entelecheia-0.1.4/LICENSE
+-rw-r--r--   0        0        0      915 2023-04-26 10:27:06.308644 entelecheia-0.1.4/README.md
+-rw-r--r--   0        0        0     2981 2023-04-26 10:27:31.192546 entelecheia-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      179 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      892 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-26 10:27:31.144546 entelecheia-0.1.4/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      351 2023-04-26 10:27:31.144546 entelecheia-0.1.4/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/task/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 entelecheia-0.1.4/PKG-INFO
```

### Comparing `entelecheia-0.1.3/LICENSE` & `entelecheia-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.3/README.md` & `entelecheia-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
+
 [![home-img]][home-url]
 [![course-img]][course-url]
 [![lecture-img]][lecture-url]
 [![research-img]][research-url]
 [![linkedin-img]][linkedin-url]
 
 [home-img]: https://img.shields.io/badge/home-entelecheia.me-blue
@@ -13,9 +14,7 @@
 [lecture-url]: https://lecture.entelecheia.ai
 [research-img]: https://img.shields.io/badge/research-entelecheia.ai-blue
 [research-url]: https://research.entelecheia.ai
 [linkedin-img]: https://img.shields.io/badge/LinkedIn-blue?logo=linkedin
 [linkedin-url]: https://www.linkedin.com/in/entelecheia/
 
 Coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
-
-https://user-images.githubusercontent.com/1177283/224186183-4f1fe765-d2f9-4c37-8d7b-078bf9c879c6.mp4
```

### Comparing `entelecheia-0.1.3/pyproject.toml` & `entelecheia-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.1.3"
+version = "0.1.4"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 repository = "https://github.com/entelecheia/entelecheia"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
 
 [tool.poetry.scripts]
 entelecheia = 'entelecheia.__cli__:main'
 
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

### Comparing `entelecheia-0.1.3/src/entelecheia/__init__.py` & `entelecheia-0.1.4/src/entelecheia/__init__.py`

 * *Files 23% similar despite different names*

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
 global_config.hyfi_package_config_path = "pkg://entelecheia.conf"
```

### Comparing `entelecheia-0.1.3/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.1.4/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.3/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.1.4/src/entelecheia/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.3/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.1.4/src/entelecheia/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.3/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.1.4/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.3/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.1.4/src/entelecheia/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.3/PKG-INFO` & `entelecheia-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.1.3
+Version: 0.1.4
 Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 Home-page: https://entelecheia.me
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
 Project-URL: Repository, https://github.com/entelecheia/entelecheia
 Description-Content-Type: text/markdown
 
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
+
 [![home-img]][home-url]
 [![course-img]][course-url]
 [![lecture-img]][lecture-url]
 [![research-img]][research-url]
 [![linkedin-img]][linkedin-url]
 
 [home-img]: https://img.shields.io/badge/home-entelecheia.me-blue
@@ -32,9 +33,7 @@
 [research-img]: https://img.shields.io/badge/research-entelecheia.ai-blue
 [research-url]: https://research.entelecheia.ai
 [linkedin-img]: https://img.shields.io/badge/LinkedIn-blue?logo=linkedin
 [linkedin-url]: https://www.linkedin.com/in/entelecheia/
 
 Coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 
-https://user-images.githubusercontent.com/1177283/224186183-4f1fe765-d2f9-4c37-8d7b-078bf9c879c6.mp4
-
```

