# Comparing `tmp/jinja2_inflection-0.1.2.tar.gz` & `tmp/jinja2_inflection-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_inflection-0.1.2.tar", last modified: Thu Apr 20 10:08:46 2023, max compression
+gzip compressed data, was "jinja2_inflection-0.1.3.tar", last modified: Wed Apr 26 17:37:34 2023, max compression
```

## Comparing `jinja2_inflection-0.1.2.tar` & `jinja2_inflection-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       56 2023-04-16 08:32:09.839714 jinja2_inflection-0.1.2/README.md
--rw-r--r--   0        0        0     1092 2023-04-20 09:32:01.990583 jinja2_inflection-0.1.2/jinja2_inflection/__init__.py
--rw-r--r--   0        0        0      790 2023-04-20 10:08:46.478728 jinja2_inflection-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 jinja2_inflection-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-04-26 17:35:55.976076 jinja2_inflection-0.1.3/README.md
+-rw-r--r--   0        0        0     1100 2023-04-26 17:36:02.707150 jinja2_inflection-0.1.3/jinja2_inflection/__init__.py
+-rw-r--r--   0        0        0      877 2023-04-26 17:37:34.519737 jinja2_inflection-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 jinja2_inflection-0.1.3/PKG-INFO
```

### Comparing `jinja2_inflection-0.1.2/jinja2_inflection/__init__.py` & `jinja2_inflection-0.1.3/jinja2_inflection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from inflection import transliterate
 from inflection import underscore
 
 from jinja2.ext import Extension
 
 
 class InflectionExtension(Extension):
-    def __init__(self, environment):
+    def __init__(self, environment) -> None:
         super(InflectionExtension, self).__init__(environment)
         inflection_filters = dict(
             camelize=camelize,
             dasherize=dasherize,
             humanize_inflection=humanize,
             ordinal=ordinal,
             ordinalize=ordinalize,
```

### Comparing `jinja2_inflection-0.1.2/pyproject.toml` & `jinja2_inflection-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 [tool.pdm.dev-dependencies]
 dev = [
-    "isort>=5.12.0",
-    "ruff>=0.0.262",
+    "crackerjack>=0.1.7",
+    "pre-commit>=3.2.2",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
+fix = true
+show-fixes = true
+show-source = true
 
 [tool.ruff.isort]
-split-on-trailing-comma = true
-force-wrap-aliases = true
 force-single-line = true
 
+[tool.ruff.mccabe]
+max-complexity = 10
+
 [tool.ruff.pydocstyle]
 convention = "google"
 
-[tool.isort]
-profile = "black"
-py_version = 311
-multiple-lines-output = 3
-
 [tool.black]
 target-version = [
     "py311",
 ]
 
+[tool.mypy]
+strict = true
+pretty = true
+
+[tool.refurb]
+enable_all = true
+
+[tool.pytype]
+inputs = [
+    "package_name",
+]
+
 [project]
 name = "jinja2-inflection"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
-authors = [
-    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
-]
 dependencies = [
     "inflection>=0.5.1",
     "jinja2>=3.1.2",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
+authors = [
+    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
+]
 
 [project.license]
 text = "BSD-3-Clause"
 
 [build-system]
 requires = [
     "pdm-backend",
```

