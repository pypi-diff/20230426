# Comparing `tmp/invokelint-0.6.0.tar.gz` & `tmp/invokelint-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokelint-0.6.0.tar", last modified: Tue Mar 21 18:17:06 2023, max compression
+gzip compressed data, was "invokelint-0.7.0.tar", last modified: Wed Apr 26 14:04:41 2023, max compression
```

## Comparing `invokelint-0.6.0.tar` & `invokelint-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:06.012393 invokelint-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-21 18:16:09.000000 invokelint-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-21 18:16:09.000000 invokelint-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-03-21 18:17:06.012393 invokelint-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-03-21 18:16:09.000000 invokelint-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:06.008393 invokelint-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-21 18:16:09.000000 invokelint-0.6.0/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:06.008393 invokelint-0.6.0/invokelint/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:06.008393 invokelint-0.6.0/invokelint/path/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/path/filter_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/path/setuptools.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/ruff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-21 18:16:09.000000 invokelint-0.6.0/invokelint/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:06.008393 invokelint-0.6.0/invokelint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-03-21 18:17:06.000000 invokelint-0.6.0/invokelint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-21 18:17:06.000000 invokelint-0.6.0/invokelint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 18:17:06.000000 invokelint-0.6.0/invokelint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 18:17:05.000000 invokelint-0.6.0/invokelint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-21 18:17:06.000000 invokelint-0.6.0/invokelint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 18:17:06.000000 invokelint-0.6.0/invokelint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-03-21 18:16:09.000000 invokelint-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-21 18:17:06.012393 invokelint-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-21 18:16:09.000000 invokelint-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 18:17:06.012393 invokelint-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-21 18:16:09.000000 invokelint-0.6.0/tests/test__clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-21 18:16:09.000000 invokelint-0.6.0/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-03-21 18:16:09.000000 invokelint-0.6.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-21 18:16:09.000000 invokelint-0.6.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-21 18:16:09.000000 invokelint-0.6.0/tests/test_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-03-21 18:16:09.000000 invokelint-0.6.0/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 14:03:10.000000 invokelint-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 14:03:10.000000 invokelint-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-26 14:04:41.937033 invokelint-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-26 14:03:10.000000 invokelint-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.933033 invokelint-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-26 14:03:10.000000 invokelint-0.7.0/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/invokelint/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/invokelint/path/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/path/filter_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/path/setuptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/ruff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-26 14:03:10.000000 invokelint-0.7.0/invokelint/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/invokelint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 14:04:41.000000 invokelint-0.7.0/invokelint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-26 14:03:10.000000 invokelint-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 14:04:41.937033 invokelint-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 14:03:10.000000 invokelint-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:04:41.937033 invokelint-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test__clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-26 14:03:10.000000 invokelint-0.7.0/tests/test_test.py
```

### Comparing `invokelint-0.6.0/LICENSE` & `invokelint-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/PKG-INFO` & `invokelint-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.6.0
+Version: 0.7.0
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
```

### Comparing `invokelint-0.6.0/README.md` & `invokelint-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/docs/CONTRIBUTING.md` & `invokelint-0.7.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/_clean.py` & `invokelint-0.7.0/invokelint/_clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/dist.py` & `invokelint-0.7.0/invokelint/dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/lint.py` & `invokelint-0.7.0/invokelint/lint.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 def call_xenon(context: Context, **kwargs: Any) -> Result:  # noqa: ARG001
     return xenon(context)
 
 
 @task(
     help={
         "skip_format": "Lints without format style.",
-        "ruff": "Fix ruff warnings",
+        "ruff": "Leave ruff warnings",
     },
 )
 def fast(context: Context, *, skip_format: bool = False, ruff: bool = False) -> List[Result]:
     """Runs fast linting (ruff, bandit, dodgy, flake8, pydocstyle, xenon)."""
     list_result = [] if skip_format else fmt(context, ruff=ruff)
     tasks = [call_ruff, call_bandit, call_dodgy, call_flake8, call_pydocstyle, call_xenon]
     list_result.extend(run_in_order(tasks, context))
```

### Comparing `invokelint-0.6.0/invokelint/path/__init__.py` & `invokelint-0.7.0/invokelint/path/__init__.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/path/filter_duplication.py` & `invokelint-0.7.0/invokelint/path/filter_duplication.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/path/setuptools.py` & `invokelint-0.7.0/invokelint/path/setuptools.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/ruff.py` & `invokelint-0.7.0/invokelint/ruff.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/run.py` & `invokelint-0.7.0/invokelint/run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/invokelint/style.py` & `invokelint-0.7.0/invokelint/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,19 @@
         execute(context, show_fixes=True)
     return execute(context, fix=True, show_fixes=True)
 
 
 @task(
     help={
         "check": "Checks if source is formatted without applying changes",
-        "ruff": "Fix ruff warnings",
+        "ruff": "Leave ruff warnings",
     },
 )
 def fmt(context: Context, *, check: bool = False, ruff: bool = False) -> List[Result]:
     """Formats code by docformatter, isort, autoflake, and Black (option for only check available)."""
     tasks = [docformatter, isort, autoflake, black]
-    if check or ruff:
+    if check or not ruff:
         tasks.append(call_ruff)
     return run_in_order(tasks, context, check=check)
 
 
 ns.add_task(fmt, default=True)
```

### Comparing `invokelint-0.6.0/invokelint/test.py` & `invokelint-0.7.0/invokelint/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     xml: bool = False,
     html: bool = False,
 ) -> Result:
     """Runs all tests and report coverage (options for create xml / html available)."""
     run_in_pty(context, build_coverage_run_command(is_all=all))
     # Reason: Note.
     # result = run_in_pty(context, "coverage combine")  # noqa: ERA001
-    result = run_in_pty(context, "coverage report -m")
+    result = run_in_pty(context, "coverage report --show-missing")
     if publish:
         # Publish the results via coveralls
         return run_in_pty(context, "coveralls")
     # Build a local report
     if xml:
         result = run_in_pty(context, "coverage xml")
     if html:
```

### Comparing `invokelint-0.6.0/invokelint.egg-info/PKG-INFO` & `invokelint-0.7.0/invokelint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.6.0
+Version: 0.7.0
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
```

### Comparing `invokelint-0.6.0/invokelint.egg-info/SOURCES.txt` & `invokelint-0.7.0/invokelint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/pyproject.toml` & `invokelint-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invokelint"
-version = "0.6.0"
+version = "0.7.0"
 description = "Invokes Python dev tools at once."
 readme = "README.md"
 # Dependency: setuptools>=61.0.0 requires Python 3.7
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
     "autoflake",
```

### Comparing `invokelint-0.6.0/tests/test__clean.py` & `invokelint-0.7.0/tests/test__clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/tests/test_dist.py` & `invokelint-0.7.0/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/tests/test_lint.py` & `invokelint-0.7.0/tests/test_lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     radon,
     radon_cc,
     radon_mi,
     ruff_task,
     semgrep,
     xenon,
 )
-from tests.test_style import LIST_COMMAND_EXPECTED_STYLE
+from tests.test_style import LIST_COMMAND_EXPECTED_STYLE, LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF
 from tests.testlibraries import check_list_result, check_result
 
 if TYPE_CHECKING:
     from invoke import Context
 
 PYTHON_DIR = "invokelint setup.py tasks.py tests"
 TEST_DIR = "tests"
@@ -107,14 +107,20 @@
 
 def test_fast(context: "Context") -> None:
     """Command should success and run appropriate commands."""
     list_result = fast(context)
     check_list_result(list_result, LIST_COMMAND_EXPECTED_STYLE + LIST_COMMAND_EXPECTED)
 
 
+def test_fast_ruff(context: "Context") -> None:
+    """Command should success and run appropriate commands."""
+    list_result = fast(context, ruff=True)
+    check_list_result(list_result, LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF + LIST_COMMAND_EXPECTED)
+
+
 def test_fast_skip_format(context: "Context") -> None:
     """Command should success and run appropriate commands."""
     list_result = fast(context, skip_format=True)
     check_list_result(list_result, LIST_COMMAND_EXPECTED)
 
 
 @pytest.mark.slow()
```

### Comparing `invokelint-0.6.0/tests/test_run.py` & `invokelint-0.7.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.6.0/tests/test_style.py` & `invokelint-0.7.0/tests/test_style.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 from tests.testlibraries import check_list_result
 
 if TYPE_CHECKING:
     from invoke import Context
 
 PYTHON_DIR = "invokelint setup.py tasks.py tests"
 
-LIST_COMMAND_EXPECTED_STYLE = [
+LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF = [
     f"docformatter --recursive --wrap-summaries 119 --wrap-descriptions 119 --in-place {PYTHON_DIR}",
     f"isort {PYTHON_DIR}",
     f"autoflake --recursive --in-place {PYTHON_DIR}",
     f"black {PYTHON_DIR}",
 ]
+LIST_COMMAND_EXPECTED_STYLE = [
+    *LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF,
+    "ruff --fix --show-fixes --ignore S101 tests",
+]
 LIST_COMMAND_EXPECTED_STYLE_CHECK = [
     f"docformatter --recursive --wrap-summaries 119 --wrap-descriptions 119 --check {PYTHON_DIR}",
     f"isort --check-only --diff {PYTHON_DIR}",
     f"autoflake --recursive --check {PYTHON_DIR}",
     f"black --check --diff {PYTHON_DIR}",
     "ruff --show-fixes --ignore S101 tests",
 ]
@@ -33,11 +37,8 @@
 def test_style_check(context: "Context") -> None:
     """Command should success and run appropriate commands."""
     check_list_result(fmt(context, check=True), LIST_COMMAND_EXPECTED_STYLE_CHECK)
 
 
 def test_style_ruff(context: "Context") -> None:
     """Command should success and run appropriate commands."""
-    check_list_result(
-        fmt(context, ruff=True),
-        [*LIST_COMMAND_EXPECTED_STYLE, "ruff --fix --show-fixes --ignore S101 tests"],
-    )
+    check_list_result(fmt(context, ruff=True), LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF)
```

### Comparing `invokelint-0.6.0/tests/test_test.py` & `invokelint-0.7.0/tests/test_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         invokelint/style.py         33      0   100%
         invokelint/test.py          28      0   100%
         ------------------------------------------------------
         TOTAL                      149     11   100%
     """,
 )
 EXPECTED_COMMAND_RUN = "coverage run --source invokelint -m pytest"
-EXPECTED_COMMAND_REPORT = "coverage report -m"
+EXPECTED_COMMAND_REPORT = "coverage report --show-missing"
 
 
 def test_build_coverage_run_command() -> None:
     assert build_coverage_run_command(is_all=True) == "coverage run --source invokelint,setup,tasks -m pytest"
 
 
 def test_coverage(mocker: "MockFixture") -> None:
```

