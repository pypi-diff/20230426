# Comparing `tmp/lexikanon-0.1.2.tar.gz` & `tmp/lexikanon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.1.2.tar", max compression
+gzip compressed data, was "lexikanon-0.1.3.tar", max compression
```

## Comparing `lexikanon-0.1.2.tar` & `lexikanon-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 11:36:40.388643 lexikanon-0.1.2/LICENSE
--rw-r--r--   0        0        0     3572 2023-04-21 11:36:40.388643 lexikanon-0.1.2/README.md
--rw-r--r--   0        0        0     2979 2023-04-21 11:37:06.394825 lexikanon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      177 2023-04-21 11:36:40.388643 lexikanon-0.1.2/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      878 2023-04-21 11:36:40.388643 lexikanon-0.1.2/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       21 2023-04-21 11:37:06.346821 lexikanon-0.1.2/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 11:36:40.388643 lexikanon-0.1.2/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 11:36:40.388643 lexikanon-0.1.2/src/lexikanon/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 11:36:40.388643 lexikanon-0.1.2/src/lexikanon/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 11:36:40.388643 lexikanon-0.1.2/src/lexikanon/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/conf/task/__init__.yaml
--rw-r--r--   0        0        0      195 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 11:36:40.392643 lexikanon-0.1.2/src/lexikanon/py.typed
--rw-r--r--   0        0        0     4184 1970-01-01 00:00:00.000000 lexikanon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-26 10:16:01.950589 lexikanon-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3572 2023-04-26 10:16:01.950589 lexikanon-0.1.3/README.md
+-rw-r--r--   0        0        0     2852 2023-04-26 10:16:28.279084 lexikanon-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      890 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-26 10:16:28.223083 lexikanon-0.1.3/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-26 10:16:28.223083 lexikanon-0.1.3/src/lexikanon/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      195 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-04-26 10:16:01.954589 lexikanon-0.1.3/src/lexikanon/py.typed
+-rw-r--r--   0        0        0     4212 1970-01-01 00:00:00.000000 lexikanon-0.1.3/PKG-INFO
```

### Comparing `lexikanon-0.1.2/LICENSE` & `lexikanon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.2/README.md` & `lexikanon-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.2/pyproject.toml` & `lexikanon-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
+repository = "https://github.com/entelecheia/lexikanon"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
 
 [tool.poetry.scripts]
 lexikanon = 'lexikanon.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.6"
-toml = "^0.10.2"
+hyfi = "^0.2.20"
 
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
 version_variable = "src/lexikanon/_version.py:__version__"
+version_pattern = 'src/lexikanon/conf/about/__init__.yaml:version: "{version}"'
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

### Comparing `lexikanon-0.1.2/src/lexikanon/conf/dotenv/__init__.yaml` & `lexikanon-0.1.3/src/lexikanon/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.2/src/lexikanon/conf/hydra/help/help.yaml` & `lexikanon-0.1.3/src/lexikanon/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.2/src/lexikanon/conf/mode/__init__.yaml` & `lexikanon-0.1.3/src/lexikanon/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.2/src/lexikanon/conf/path/__default__.yaml` & `lexikanon-0.1.3/src/lexikanon/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.2/src/lexikanon/conf/path/__init__.yaml` & `lexikanon-0.1.3/src/lexikanon/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.1.2/PKG-INFO` & `lexikanon-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python Library for Tokenizers
 Home-page: https://lexikanon.entelecheia.ai
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
+Requires-Dist: hyfi (>=0.2.20,<0.3.0)
+Project-URL: Repository, https://github.com/entelecheia/lexikanon
 Description-Content-Type: text/markdown
 
 # Lexikanon: A Python Library for Tokenizers
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
 [![version-image]][release-url]
```

