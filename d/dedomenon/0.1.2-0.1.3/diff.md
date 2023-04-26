# Comparing `tmp/dedomenon-0.1.2.tar.gz` & `tmp/dedomenon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedomenon-0.1.2.tar", max compression
+gzip compressed data, was "dedomenon-0.1.3.tar", max compression
```

## Comparing `dedomenon-0.1.2.tar` & `dedomenon-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 11:42:12.606234 dedomenon-0.1.2/LICENSE
--rw-r--r--   0        0        0     3131 2023-04-21 11:42:12.606234 dedomenon-0.1.2/README.md
--rw-r--r--   0        0        0     2977 2023-04-21 11:42:38.986796 dedomenon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      177 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/__cli__.py
--rw-r--r--   0        0        0      878 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/__init__.py
--rw-r--r--   0        0        0       21 2023-04-21 11:42:38.934795 dedomenon-0.1.2/src/dedomenon/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/conf/task/__init__.yaml
--rw-r--r--   0        0        0      193 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 11:42:12.606234 dedomenon-0.1.2/src/dedomenon/py.typed
--rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 dedomenon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-25 23:50:16.588895 dedomenon-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3131 2023-04-25 23:50:16.588895 dedomenon-0.1.3/README.md
+-rw-r--r--   0        0        0     2850 2023-04-25 23:50:48.192146 dedomenon-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/__cli__.py
+-rw-r--r--   0        0        0      818 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-25 23:50:48.132144 dedomenon-0.1.3/src/dedomenon/_version.py
+-rw-r--r--   0        0        0        0 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-25 23:50:48.132144 dedomenon-0.1.3/src/dedomenon/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      193 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/project.toml
+-rw-r--r--   0        0        0        0 2023-04-25 23:50:16.592895 dedomenon-0.1.3/src/dedomenon/py.typed
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 dedomenon-0.1.3/PKG-INFO
```

### Comparing `dedomenon-0.1.2/LICENSE` & `dedomenon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.2/README.md` & `dedomenon-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.2/pyproject.toml` & `dedomenon-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "dedomenon"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Python Library for Datasets"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://dedomenom.entelecheia.ai"
+repository = "https://github.com/entelecheia/dedomenon"
 readme = "README.md"
 packages = [{ include = "dedomenon", from = "src" }]
 
 [tool.poetry.scripts]
 dedomenon = 'dedomenon.__cli__:main'
 
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
 version_variable = "src/dedomenon/_version.py:__version__"
+version_pattern = 'src/dedomenon/conf/about/__init__.yaml:version: "{version}"'
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

### Comparing `dedomenon-0.1.2/src/dedomenon/__init__.py` & `dedomenon-0.1.3/src/dedomenon/__init__.py`

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
 global_config.hyfi_package_config_path = "pkg://dedomenon.conf"
 
 
 def get_version() -> str:
     """This is the cli function of the package"""
     return __version__
```

### Comparing `dedomenon-0.1.2/src/dedomenon/conf/dotenv/__init__.yaml` & `dedomenon-0.1.3/src/dedomenon/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.2/src/dedomenon/conf/hydra/help/help.yaml` & `dedomenon-0.1.3/src/dedomenon/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.2/src/dedomenon/conf/mode/__init__.yaml` & `dedomenon-0.1.3/src/dedomenon/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.2/src/dedomenon/conf/path/__default__.yaml` & `dedomenon-0.1.3/src/dedomenon/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.2/src/dedomenon/conf/path/__init__.yaml` & `dedomenon-0.1.3/src/dedomenon/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `dedomenon-0.1.2/PKG-INFO` & `dedomenon-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dedomenon
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python Library for Datasets
 Home-page: https://dedomenom.entelecheia.ai
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
+Project-URL: Repository, https://github.com/entelecheia/dedomenon
 Description-Content-Type: text/markdown
 
 # Dedomenon: A Python Library for Datasets
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
 [![version-image]][release-url]
```

