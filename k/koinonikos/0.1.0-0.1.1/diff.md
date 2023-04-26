# Comparing `tmp/koinonikos-0.1.0.tar.gz` & `tmp/koinonikos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koinonikos-0.1.0.tar", max compression
+gzip compressed data, was "koinonikos-0.1.1.tar", max compression
```

## Comparing `koinonikos-0.1.0.tar` & `koinonikos-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 21:32:57.316775 koinonikos-0.1.0/LICENSE
--rw-r--r--   0        0        0     3967 2023-04-21 21:32:57.316775 koinonikos-0.1.0/README.md
--rw-r--r--   0        0        0     2999 2023-04-21 21:33:24.612684 koinonikos-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      178 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/__cli__.py
--rw-r--r--   0        0        0      879 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/__init__.py
--rw-r--r--   0        0        0       22 2023-04-21 21:33:24.560684 koinonikos-0.1.0/src/koinonikos/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/conf/task/__init__.yaml
--rw-r--r--   0        0        0      210 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 21:32:57.320775 koinonikos-0.1.0/src/koinonikos/py.typed
--rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 koinonikos-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-26 19:01:21.304374 koinonikos-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3855 2023-04-26 19:01:21.308374 koinonikos-0.1.1/README.md
+-rw-r--r--   0        0        0     2873 2023-04-26 19:01:50.624841 koinonikos-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      178 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/__cli__.py
+-rw-r--r--   0        0        0      891 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-26 19:01:50.572840 koinonikos-0.1.1/src/koinonikos/_version.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-26 19:01:50.576840 koinonikos-0.1.1/src/koinonikos/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      210 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/project.toml
+-rw-r--r--   0        0        0        0 2023-04-26 19:01:21.308374 koinonikos-0.1.1/src/koinonikos/py.typed
+-rw-r--r--   0        0        0     4511 1970-01-01 00:00:00.000000 koinonikos-0.1.1/PKG-INFO
```

### Comparing `koinonikos-0.1.0/LICENSE` & `koinonikos-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koinonikos-0.1.0/README.md` & `koinonikos-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 pip install koinonikos
 ```
 
 ## Getting Started
 
 To get started with Koinonikos, visit the [official documentation][docs-url] and the [GitHub repository][repo-url] for examples, tutorials, and more information.
 
-Join the Koinonikos community today and advance the field of social science research with the power of Python!
-
 ## Changelog
 
 See the [CHANGELOG] for more information.
 
 ## Contributing
 
 Contributions are welcome! Please see the [contributing guidelines] for more information.
```

### Comparing `koinonikos-0.1.0/pyproject.toml` & `koinonikos-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "koinonikos"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python Library for Social Science Research"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://koinonikos.entelecheia.ai"
+repository = "https://github.com/entelecheia/koinonikos"
 readme = "README.md"
 packages = [{ include = "koinonikos", from = "src" }]
 
 [tool.poetry.scripts]
 koinonikos = 'koinonikos.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.11"
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
 version_variable = "src/koinonikos/_version.py:__version__"
+version_pattern = 'src/koinonikos/conf/about/__init__.yaml:version: "{version}"'
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

### Comparing `koinonikos-0.1.0/src/koinonikos/conf/dotenv/__init__.yaml` & `koinonikos-0.1.1/src/koinonikos/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `koinonikos-0.1.0/src/koinonikos/conf/hydra/help/help.yaml` & `koinonikos-0.1.1/src/koinonikos/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `koinonikos-0.1.0/src/koinonikos/conf/mode/__init__.yaml` & `koinonikos-0.1.1/src/koinonikos/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `koinonikos-0.1.0/src/koinonikos/conf/path/__default__.yaml` & `koinonikos-0.1.1/src/koinonikos/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `koinonikos-0.1.0/src/koinonikos/conf/path/__init__.yaml` & `koinonikos-0.1.1/src/koinonikos/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `koinonikos-0.1.0/PKG-INFO` & `koinonikos-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: koinonikos
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Library for Social Science Research
 Home-page: https://koinonikos.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.11,<0.3.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: hyfi (>=0.2.20,<0.3.0)
+Project-URL: Repository, https://github.com/entelecheia/koinonikos
 Description-Content-Type: text/markdown
 
 # Koinonikos: A Python Library for Social Science Research
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
 [![version-image]][release-url]
@@ -68,16 +68,14 @@
 pip install koinonikos
 ```
 
 ## Getting Started
 
 To get started with Koinonikos, visit the [official documentation][docs-url] and the [GitHub repository][repo-url] for examples, tutorials, and more information.
 
-Join the Koinonikos community today and advance the field of social science research with the power of Python!
-
 ## Changelog
 
 See the [CHANGELOG] for more information.
 
 ## Contributing
 
 Contributions are welcome! Please see the [contributing guidelines] for more information.
```

