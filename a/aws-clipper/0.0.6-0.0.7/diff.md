# Comparing `tmp/aws_clipper-0.0.6.tar.gz` & `tmp/aws_clipper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_clipper-0.0.6.tar", max compression
+gzip compressed data, was "aws_clipper-0.0.7.tar", max compression
```

## Comparing `aws_clipper-0.0.6.tar` & `aws_clipper-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       75 2023-04-26 02:59:30.530693 aws_clipper-0.0.6/README.md
--rw-r--r--   0        0        0     1687 2023-04-26 02:59:30.530693 aws_clipper-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2789 2023-04-26 02:59:30.530693 aws_clipper-0.0.6/src/aws_clipper/__init__.py
--rw-r--r--   0        0        0       65 2023-04-26 02:59:30.530693 aws_clipper-0.0.6/src/aws_clipper/__main__.py
--rw-r--r--   0        0        0     1323 2023-04-26 02:59:30.530693 aws_clipper-0.0.6/src/aws_clipper/cli.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 aws_clipper-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2603 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      672 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/README.md
+-rw-r--r--   0        0        0     2059 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2789 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/src/aws_clipper/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/src/aws_clipper/__main__.py
+-rw-r--r--   0        0        0     1323 2023-04-26 05:12:52.020624 aws_clipper-0.0.7/src/aws_clipper/cli.py
+-rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 aws_clipper-0.0.7/PKG-INFO
```

### Comparing `aws_clipper-0.0.6/pyproject.toml` & `aws_clipper-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 [tool.poetry]
 name = "aws-clipper"
-version = "0.0.6"
-description = "Dump config for AWS CLI"
-authors = ["Tsunenobu Kai <kai2nenobu@gmail.com>"]
+version = "0.0.7"
+description = "`aws-clipper` dumps AWS CLI config from a simple YAML file."
+authors = ["kai2nenobu <kai2nenobu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_clipper", from = "src"}]
+homepage = "https://github.com/kai2nenobu/aws-clipper"
+repository = "https://github.com/kai2nenobu/aws-clipper"
+keywords = ["aws"]
+include = ["README.md", "CHANGELOG.md"]
+
+[tool.poetry.urls]
+"Changelog" = "https://github.com/kai2nenobu/aws-clipper/blob/main/CHANGELOG.md"
+"Bug Tracker" = "https://github.com/kai2nenobu/aws-clipper/issues"
 
 [tool.poetry.scripts]
 aws-clipper = 'aws_clipper.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyyaml = "^6.0"
```

### Comparing `aws_clipper-0.0.6/src/aws_clipper/__init__.py` & `aws_clipper-0.0.7/src/aws_clipper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import configparser
 from typing import Any, TextIO
 
 import yaml
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 
 def _expand_value(v: Any, variables: dict[str, Any] = {}) -> str:
     """
     In AWS CLI config, nested settings (like S3 settings) are indented as below.
 
     [default]
```

### Comparing `aws_clipper-0.0.6/src/aws_clipper/cli.py` & `aws_clipper-0.0.7/src/aws_clipper/cli.py`

 * *Files identical despite different names*

