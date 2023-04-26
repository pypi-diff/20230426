# Comparing `tmp/thematos-0.1.3.tar.gz` & `tmp/thematos-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thematos-0.1.3.tar", max compression
+gzip compressed data, was "thematos-0.1.4.tar", max compression
```

## Comparing `thematos-0.1.3.tar` & `thematos-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 11:37:07.054945 thematos-0.1.3/LICENSE
--rw-r--r--   0        0        0     3479 2023-04-21 11:37:07.054945 thematos-0.1.3/README.md
--rw-r--r--   0        0        0     2977 2023-04-21 11:37:42.020224 thematos-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      176 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/__cli__.py
--rw-r--r--   0        0        0      877 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/__init__.py
--rw-r--r--   0        0        0       21 2023-04-21 11:37:41.964222 thematos-0.1.3/src/thematos/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 11:37:07.054945 thematos-0.1.3/src/thematos/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/conf/task/__init__.yaml
--rw-r--r--   0        0        0      197 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 11:37:07.058945 thematos-0.1.3/src/thematos/py.typed
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 thematos-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-25 23:56:45.162489 thematos-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3479 2023-04-25 23:56:45.162489 thematos-0.1.4/README.md
+-rw-r--r--   0        0        0     2848 2023-04-25 23:57:20.862580 thematos-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/__cli__.py
+-rw-r--r--   0        0        0      817 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-25 23:57:20.802580 thematos-0.1.4/src/thematos/_version.py
+-rw-r--r--   0        0        0        0 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/__init__.py
+-rw-r--r--   0        0        0      196 2023-04-25 23:57:20.802580 thematos-0.1.4/src/thematos/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      197 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/project.toml
+-rw-r--r--   0        0        0        0 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/py.typed
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 thematos-0.1.4/PKG-INFO
```

### Comparing `thematos-0.1.3/LICENSE` & `thematos-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thematos-0.1.3/README.md` & `thematos-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `thematos-0.1.3/pyproject.toml` & `thematos-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "thematos"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Python Library for Topic Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://thematos.entelecheia.ai"
+repository = "https://github.com/entelecheia/thematos"
 readme = "README.md"
 packages = [{ include = "thematos", from = "src" }]
 
 [tool.poetry.scripts]
 thematos = 'thematos.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.6"
-toml = "^0.10.2"
+hyfi = "^0.2.15"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
-setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
@@ -74,31 +73,27 @@
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version = "1.0.1"
 tag_format = "v$version"
 
-[tool.setuptools_scm]
-write_to_template = '__version__ = "{version}"'
-tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
-
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/thematos/_version.py:__version__"
+version_pattern = 'src/thematos/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
-pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools>=45", "setuptools_scm[toml]>=6.2"]
-build-backend = 'setuptools.build_meta'
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `thematos-0.1.3/src/thematos/__init__.py` & `thematos-0.1.4/src/thematos/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import os
 
-import toml
 from hyfi import HyFI, about, global_config
 
 from ._version import __version__
 
 # Read and parse pyproject.toml
 current_dir = os.path.dirname(os.path.abspath(__file__))
-pyproject_path = os.path.join(current_dir, "project.toml")
+about_path = os.path.join(current_dir, "conf", "about", "__init__.yaml")
 
-with open(pyproject_path) as f:
-    pyproject_data = toml.load(f)
+about_data = HyFI.load(about_path)
 
-# Extract package information from pyproject.toml
-project_data = pyproject_data.get("metadata", {})
-about.name = project_data.get("name", "package name")
-about.author = project_data.get("authors", ["Author name"])[0]
-about.description = project_data.get("description", "package description")
-about.homepage = project_data.get("homepage", "https://package.homepage")
+# Extract package information
+about.name = about_data.get("name", "package name")
+about.authors = about_data.get("authors", ["Author name"])
+about.description = about_data.get("description", "package description")
+about.homepage = about_data.get("homepage", "https://package.homepage")
+about.license = about_data.get("license", "MIT")
 about.version = __version__
 global_config.hyfi_package_config_path = "pkg://thematos.conf"
 
 
 def get_version() -> str:
     """This is the cli function of the package"""
     return __version__
```

### Comparing `thematos-0.1.3/src/thematos/conf/dotenv/__init__.yaml` & `thematos-0.1.4/src/thematos/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.3/src/thematos/conf/hydra/help/help.yaml` & `thematos-0.1.4/src/thematos/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.3/src/thematos/conf/mode/__init__.yaml` & `thematos-0.1.4/src/thematos/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.3/src/thematos/conf/path/__default__.yaml` & `thematos-0.1.4/src/thematos/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.3/src/thematos/conf/path/__init__.yaml` & `thematos-0.1.4/src/thematos/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `thematos-0.1.3/PKG-INFO` & `thematos-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thematos
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python Library for Topic Modeling
 Home-page: https://thematos.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.6,<0.3.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: hyfi (>=0.2.15,<0.3.0)
+Project-URL: Repository, https://github.com/entelecheia/thematos
 Description-Content-Type: text/markdown
 
 # ThematOS: A Python Library for Topic Modeling
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
 [![version-image]][release-url]
```

