# Comparing `tmp/jinja2-arrow-0.1.2.tar.gz` & `tmp/jinja2-arrow-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2-arrow-0.1.2.tar", last modified: Thu Apr 20 10:08:10 2023, max compression
+gzip compressed data, was "jinja2-arrow-0.1.3.tar", last modified: Wed Apr 26 17:32:14 2023, max compression
```

## Comparing `jinja2-arrow-0.1.2.tar` & `jinja2-arrow-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       45 2023-04-16 08:32:09.829609 jinja2-arrow-0.1.2/README.md
--rw-r--r--   0        0        0      852 2023-04-20 10:05:39.692340 jinja2-arrow-0.1.2/jinja2_arrow/__init__.py
--rw-r--r--   0        0        0      787 2023-04-20 10:04:46.112409 jinja2-arrow-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      240 1970-01-01 00:00:00.000000 jinja2-arrow-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-04-26 17:30:24.003706 jinja2-arrow-0.1.3/README.md
+-rw-r--r--   0        0        0      860 2023-04-26 17:30:31.788812 jinja2-arrow-0.1.3/jinja2_arrow/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-26 17:31:53.932668 jinja2-arrow-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 jinja2-arrow-0.1.3/PKG-INFO
```

### Comparing `jinja2-arrow-0.1.2/jinja2_arrow/__init__.py` & `jinja2-arrow-0.1.3/jinja2_arrow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import arrow
 from jinja2.ext import Extension
 
 
 class ArrowExtension(Extension):
-    def __init__(self, environment):
+    def __init__(self, environment) -> None:
         super(ArrowExtension, self).__init__(environment)
 
         def year(datetime_obj):
             return arrow.get(datetime_obj).year
 
         def humanize(datetime_obj):
             a = arrow.get(datetime_obj)
```

### Comparing `jinja2-arrow-0.1.2/pyproject.toml` & `jinja2-arrow-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

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
 name = "jinja2-arrow"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
-authors = [
-    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
-]
 dependencies = [
     "arrow>=1.2.3",
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
     "pdm-pep517>=1.0",
```

