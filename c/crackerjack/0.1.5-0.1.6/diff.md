# Comparing `tmp/crackerjack-0.1.5.tar.gz` & `tmp/crackerjack-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.1.5.tar", last modified: Wed Apr 26 13:02:37 2023, max compression
+gzip compressed data, was "crackerjack-0.1.6.tar", last modified: Wed Apr 26 13:13:07 2023, max compression
```

## Comparing `crackerjack-0.1.5.tar` & `crackerjack-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.1.5/LICENSE
--rw-r--r--   0        0        0     2856 2023-04-26 12:28:28.914334 crackerjack-0.1.5/README.md
--rw-r--r--   0        0        0      171 2023-04-26 13:01:24.398093 crackerjack-0.1.5/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-04-26 13:01:24.429098 crackerjack-0.1.5/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2055 2023-04-26 13:01:24.414613 crackerjack-0.1.5/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.1.5/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.1.5/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.1.5/crackerjack/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-26 12:28:28.914593 crackerjack-0.1.5/crackerjack/__main__.py
--rw-r--r--   0        0        0     4230 2023-04-26 12:59:50.864140 crackerjack-0.1.5/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1522 2023-04-26 13:01:24.443650 crackerjack-0.1.5/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     5606 2023-04-25 20:30:39.178113 crackerjack-0.1.5/crackerjack/test1.py
--rw-r--r--   0        0        0     1630 2023-04-26 13:02:37.332952 crackerjack-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3827 1970-01-01 00:00:00.000000 crackerjack-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2856 2023-04-26 12:28:28.914334 crackerjack-0.1.6/README.md
+-rw-r--r--   0        0        0      171 2023-04-26 13:11:55.664862 crackerjack-0.1.6/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-04-26 13:11:55.693154 crackerjack-0.1.6/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2055 2023-04-26 13:11:55.678389 crackerjack-0.1.6/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.1.6/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.1.6/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.1.6/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1039 2023-04-26 12:28:28.914593 crackerjack-0.1.6/crackerjack/__main__.py
+-rw-r--r--   0        0        0     4344 2023-04-26 13:10:12.914439 crackerjack-0.1.6/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1522 2023-04-26 13:11:55.707956 crackerjack-0.1.6/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     5606 2023-04-25 20:30:39.178113 crackerjack-0.1.6/crackerjack/test1.py
+-rw-r--r--   0        0        0     1630 2023-04-26 13:13:07.038425 crackerjack-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3827 1970-01-01 00:00:00.000000 crackerjack-0.1.6/PKG-INFO
```

### Comparing `crackerjack-0.1.5/LICENSE` & `crackerjack-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.5/README.md` & `crackerjack-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.5/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.1.6/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.5/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.1.6/crackerjack/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.5/crackerjack/__main__.py` & `crackerjack-0.1.6/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.5/crackerjack/crackerjack.py` & `crackerjack-0.1.6/crackerjack/crackerjack.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
                 await file.unlink()
 
     async def update_pyproject_configs(self) -> None:
         toml = await load.toml(self.toml_path)
         pkg_toml = await load.toml(self.pkg_toml_path)
         if self.poetry_pip_env:
             del pkg_toml.tool.poetry
+        old_deps = pkg_toml.tool.pdm["dev-dependencies"]
         pkg_toml.tool = toml.tool
+        pkg_toml.tool.pdm["dev-dependencies"] = old_deps
         await dump.toml(pkg_toml, self.pkg_toml_path)
 
     async def copy_configs(self) -> None:
         for config in (
             ".gitignore",
             ".pre-commit-config.yaml",
             ".libcst.codemod.yaml",
```

### Comparing `crackerjack-0.1.5/crackerjack/pyproject.toml` & `crackerjack-0.1.6/crackerjack/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 enable_all = true
 
 [tool.pytype]
 inputs = ["package_name"]
 
 [project]
 name = "Crackerjack"
-version = "0.1.4"
+version = "0.1.5"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = ["black", "ruff", "mypy", "creosote", "refurb"]
 classifiers = ["Environment :: Console", "Operating System :: OS Independent", "Programming Language :: Python", "Programming Language :: Python :: 3.11"]
 dependencies = ["click>=8.1.3", "pdoc3>=0.10.0", "pdm-bump>=0.7.0", "pydantic>=1.10.7", "aiopath>=0.6.11", "acb>=0.1.2", "aioconsole>=0.6.1"]
```

### Comparing `crackerjack-0.1.5/crackerjack/test1.py` & `crackerjack-0.1.6/crackerjack/test1.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.5/pyproject.toml` & `crackerjack-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "Crackerjack"
-version = "0.1.5"
+version = "0.1.6"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.1.5/PKG-INFO` & `crackerjack-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.1.5
+Version: 0.1.6
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

