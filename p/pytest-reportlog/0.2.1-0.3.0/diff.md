# Comparing `tmp/pytest-reportlog-0.2.1.tar.gz` & `tmp/pytest-reportlog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reportlog-0.2.1.tar", last modified: Sat Mar 11 14:58:06 2023, max compression
+gzip compressed data, was "pytest-reportlog-0.3.0.tar", last modified: Wed Apr 26 21:45:12 2023, max compression
```

## Comparing `pytest-reportlog-0.2.1.tar` & `pytest-reportlog-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:58:06.885446 pytest-reportlog-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:58:06.877446 pytest-reportlog-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:58:06.881446 pytest-reportlog-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/HOWTORELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-03-11 14:58:06.885446 pytest-reportlog-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 14:58:06.885446 pytest-reportlog-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:58:06.877446 pytest-reportlog-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:58:06.881446 pytest-reportlog-0.2.1/src/pytest_reportlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/src/pytest_reportlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-11 14:58:06.000000 pytest-reportlog-0.2.1/src/pytest_reportlog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/src/pytest_reportlog/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:58:06.885446 pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-03-11 14:58:06.000000 pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-11 14:58:06.000000 pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 14:58:06.000000 pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-11 14:58:06.000000 pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-11 14:58:06.000000 pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-11 14:58:06.000000 pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:58:06.885446 pytest-reportlog-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/tests/test_reportlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-11 14:57:44.000000 pytest-reportlog-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/src/pytest_reportlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/src/pytest_reportlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/src/pytest_reportlog/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/tests/test_reportlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/tox.ini
```

### Comparing `pytest-reportlog-0.2.1/.github/workflows/test.yml` & `pytest-reportlog-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pytest-reportlog-0.2.1/.gitignore` & `pytest-reportlog-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-reportlog-0.2.1/CHANGELOG.rst` & `pytest-reportlog-0.3.0/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.3.0 (2023-04-26)
+------------------
+
+* `#20 <https://github.com/pytest-dev/pytest-reportlog/issues/20>`_: Warnings are now included in the logs.
+
+
 0.2.1 (2023-03-11)
 ------------------
 
 * Added support for Python 3.10 and 3.11.
 * Dropped support for Python 3.5 and 3.6.
 
 0.1.2 (2020-12-11)
```

### Comparing `pytest-reportlog-0.2.1/LICENSE` & `pytest-reportlog-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reportlog-0.2.1/PKG-INFO` & `pytest-reportlog-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportlog
-Version: 0.2.1
+Version: 0.3.0
 Summary: Replacement for the --resultlog option, focused in simplicity and extensibility
 Home-page: https://github.com/pytest-dev/pytest-reportlog
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 License: MIT
 Keywords: pytest
 Platform: any
```

### Comparing `pytest-reportlog-0.2.1/README.rst` & `pytest-reportlog-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-reportlog-0.2.1/setup.py` & `pytest-reportlog-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/PKG-INFO` & `pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportlog
-Version: 0.2.1
+Version: 0.3.0
 Summary: Replacement for the --resultlog option, focused in simplicity and extensibility
 Home-page: https://github.com/pytest-dev/pytest-reportlog
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 License: MIT
 Keywords: pytest
 Platform: any
```

### Comparing `pytest-reportlog-0.2.1/src/pytest_reportlog.egg-info/SOURCES.txt` & `pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.rst
-HOWTORELEASE.rst
 LICENSE
 README.rst
+RELEASING.rst
 setup.py
 tox.ini
 .github/workflows/deploy.yml
 .github/workflows/test.yml
 src/pytest_reportlog/__init__.py
 src/pytest_reportlog/_version.py
 src/pytest_reportlog/plugin.py
```

### Comparing `pytest-reportlog-0.2.1/tests/test_reportlog.py` & `pytest-reportlog-0.3.0/tests/test_reportlog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import json
+from collections import defaultdict
 
 import pytest
 from _pytest.reports import BaseReport
 
 from pytest_reportlog.plugin import cleanup_unserializable
 
 
 def test_basics(testdir, tmp_path, pytestconfig):
     """Basic testing of the report log functionality.
 
     We don't test the test reports extensively because they have been
     tested already in ``test_reports``.
     """
-    testdir.makepyfile(
+    p = testdir.makepyfile(
         """
+        import warnings
+
         def test_ok():
             pass
 
         def test_fail():
             assert 0
-    """
+
+        def test_warning():
+            warnings.warn("message", UserWarning)
+        """
     )
 
     log_file = tmp_path / "log.json"
 
     result = testdir.runpytest("--report-log", str(log_file))
     assert result.ret == pytest.ExitCode.TESTS_FAILED
     result.stdout.fnmatch_lines([f"* generated report log file: {log_file}*"])
 
     json_objs = [json.loads(x) for x in log_file.read_text().splitlines()]
-    assert len(json_objs) == 10
+    assert len(json_objs) == 14
 
     # first line should be the session_start
     session_start = json_objs[0]
     assert session_start == {
         "pytest_version": pytest.__version__,
         "$report_type": "SessionStart",
     }
@@ -41,14 +47,30 @@
     # last line should be the session_finish
     session_start = json_objs[-1]
     assert session_start == {
         "exitstatus": pytest.ExitCode.TESTS_FAILED,
         "$report_type": "SessionFinish",
     }
 
+    split = defaultdict(list)
+    for obj in json_objs:
+        split[obj["$report_type"] == "WarningMessage"].append(obj)
+    [warning] = split[True]
+    json_objs = split[False]
+
+    assert warning == {
+        "$report_type": "WarningMessage",
+        "category": "UserWarning",
+        "when": "runtest",
+        "message": "message",
+        "lineno": 10,
+        "location": None,  # seems to be hard-coded to None
+        "filename": str(p),
+    }
+
     # rest of the json objects should be unserialized into report objects; we don't test
     # the actual report object extensively because it has been tested in ``test_reports``
     # already.
     pm = pytestconfig.pluginmanager
     for json_obj in json_objs[1:-1]:
         rep = pm.hook.pytest_report_from_serializable(
             config=pytestconfig, data=json_obj
@@ -56,24 +78,29 @@
         assert isinstance(rep, BaseReport)
 
 
 def test_xdist_integration(testdir, tmp_path):
     pytest.importorskip("xdist")
     testdir.makepyfile(
         """
+        import warnings
+
         def test_ok():
             pass
 
         def test_fail():
             assert 0
-    """
+
+        def test_warning():
+            warnings.warn("message", UserWarning)
+        """
     )
     fn = tmp_path / "result.log"
     result = testdir.runpytest("-n2", f"--report-log={fn}")
-    result.stdout.fnmatch_lines("*1 failed, 1 passed*")
+    result.stdout.fnmatch_lines("*1 failed, 2 passed, 1 warning*")
 
     lines = fn.read_text("UTF-8").splitlines()
     data = json.loads(lines[0])
     assert data == {
         "pytest_version": pytest.__version__,
         "$report_type": "SessionStart",
     }
```

