# Comparing `tmp/tof-23.4.0.tar.gz` & `tmp/tof-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tof-23.4.0.tar", last modified: Wed Apr 26 09:37:30 2023, max compression
+gzip compressed data, was "tof-23.4.1.tar", last modified: Wed Apr 26 13:30:02 2023, max compression
```

## Comparing `tof-23.4.0.tar` & `tof-23.4.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.541543 tof-23.4.0/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      148 2023-04-20 16:01:14.000000 tof-23.4.0/.flake8
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.533542 tof-23.4.0/.github/
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.537543 tof-23.4.0/.github/workflows/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1720 2023-04-26 08:16:40.000000 tof-23.4.0/.github/workflows/ci.yml
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     2139 2023-04-26 09:30:07.000000 tof-23.4.0/.github/workflows/release.yml
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      266 2023-04-20 07:32:35.000000 tof-23.4.0/.gitignore
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1775 2023-04-20 07:32:35.000000 tof-23.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      169 2023-04-20 16:26:46.000000 tof-23.4.0/.readthedocs.yaml
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1492 2023-04-19 10:45:19.000000 tof-23.4.0/LICENSE
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3139 2023-04-26 09:37:30.541543 tof-23.4.0/PKG-INFO
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     2700 2023-04-26 09:30:07.000000 tof-23.4.0/README.md
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.537543 tof-23.4.0/conda/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      798 2023-04-26 09:30:07.000000 tof-23.4.0/conda/meta.yaml
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.537543 tof-23.4.0/docs/
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.537543 tof-23.4.0/docs/_static/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    22254 2023-04-20 07:32:35.000000 tof-23.4.0/docs/_static/detector.png
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)   137750 2023-04-20 11:10:19.000000 tof-23.4.0/docs/_static/favicon.ico
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    10069 2023-04-20 11:07:17.000000 tof-23.4.0/docs/_static/logo.svg
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    96012 2023-04-20 07:32:35.000000 tof-23.4.0/docs/_static/model.png
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    32531 2023-04-20 07:32:35.000000 tof-23.4.0/docs/_static/pulse.png
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      158 2023-04-21 12:31:50.000000 tof-23.4.0/docs/api.rst
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1917 2023-04-20 16:30:49.000000 tof-23.4.0/docs/conf.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      745 2023-04-26 09:30:07.000000 tof-23.4.0/docs/index.rst
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      103 2023-04-26 08:16:40.000000 tof-23.4.0/docs/requirements.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     8486 2023-04-26 08:16:40.000000 tof-23.4.0/docs/user-guide.ipynb
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1069 2023-04-26 09:37:24.000000 tof-23.4.0/pyproject.toml
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.537543 tof-23.4.0/requirements/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       23 2023-04-20 07:32:35.000000 tof-23.4.0/requirements/ci.in
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      958 2023-04-26 08:16:40.000000 tof-23.4.0/requirements/ci.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       98 2023-04-26 08:16:40.000000 tof-23.4.0/requirements/docs.in
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     4472 2023-04-26 08:16:40.000000 tof-23.4.0/requirements/docs.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       11 2023-04-20 07:32:35.000000 tof-23.4.0/requirements/static.in
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      586 2023-04-26 08:16:40.000000 tof-23.4.0/requirements/static.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        7 2023-04-20 07:32:35.000000 tof-23.4.0/requirements/test.in
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      360 2023-04-25 16:15:32.000000 tof-23.4.0/requirements/test.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        6 2023-04-20 07:32:35.000000 tof-23.4.0/requirements/wheels.in
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      295 2023-04-25 16:15:33.000000 tof-23.4.0/requirements/wheels.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       38 2023-04-26 09:37:30.541543 tof-23.4.0/setup.cfg
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.533542 tof-23.4.0/src/
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.537543 tof-23.4.0/src/tof/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      239 2023-04-21 12:31:50.000000 tof-23.4.0/src/tof/__init__.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1341 2023-04-21 09:00:07.000000 tof-23.4.0/src/tof/chopper.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3384 2023-04-25 16:01:41.000000 tof-23.4.0/src/tof/component.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      457 2023-04-25 15:15:46.000000 tof-23.4.0/src/tof/detector.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    21215 2023-04-20 16:01:14.000000 tof-23.4.0/src/tof/facilities.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     7020 2023-04-25 16:01:41.000000 tof-23.4.0/src/tof/model.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3678 2023-04-21 12:31:50.000000 tof-23.4.0/src/tof/pulse.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      662 2023-04-25 15:13:48.000000 tof-23.4.0/src/tof/utils.py
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-26 09:37:30.537543 tof-23.4.0/src/tof.egg-info/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3139 2023-04-26 09:37:30.000000 tof-23.4.0/src/tof.egg-info/PKG-INFO
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1081 2023-04-26 09:37:30.000000 tof-23.4.0/src/tof.egg-info/SOURCES.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        1 2023-04-26 09:37:30.000000 tof-23.4.0/src/tof.egg-info/dependency_links.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       38 2023-04-26 09:37:30.000000 tof-23.4.0/src/tof.egg-info/requires.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        4 2023-04-26 09:37:30.000000 tof-23.4.0/src/tof.egg-info/top_level.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      949 2023-04-25 16:23:25.000000 tof-23.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.731097 tof-23.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-26 13:29:48.000000 tof-23.4.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.723097 tof-23.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.727097 tof-23.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-26 13:29:48.000000 tof-23.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-26 13:29:48.000000 tof-23.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-26 13:29:48.000000 tof-23.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-26 13:29:48.000000 tof-23.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 13:29:48.000000 tof-23.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-26 13:29:48.000000 tof-23.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-26 13:30:02.731097 tof-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-26 13:29:48.000000 tof-23.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.727097 tof-23.4.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-26 13:29:48.000000 tof-23.4.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.727097 tof-23.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.727097 tof-23.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-04-26 13:29:48.000000 tof-23.4.1/docs/_static/detector.png
+-rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-04-26 13:29:48.000000 tof-23.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-26 13:29:48.000000 tof-23.4.1/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    96012 2023-04-26 13:29:48.000000 tof-23.4.1/docs/_static/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-04-26 13:29:48.000000 tof-23.4.1/docs/_static/pulse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 13:29:48.000000 tof-23.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-26 13:29:48.000000 tof-23.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-26 13:29:48.000000 tof-23.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 13:29:48.000000 tof-23.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-26 13:29:48.000000 tof-23.4.1/docs/user-guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 13:29:48.000000 tof-23.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.731097 tof-23.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-26 13:29:48.000000 tof-23.4.1/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:30:02.731097 tof-23.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.723097 tof-23.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.727097 tof-23.4.1/src/tof/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/facilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 13:29:48.000000 tof-23.4.1/src/tof/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:30:02.727097 tof-23.4.1/src/tof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-26 13:30:02.000000 tof-23.4.1/src/tof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-26 13:30:02.000000 tof-23.4.1/src/tof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:30:02.000000 tof-23.4.1/src/tof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:30:02.000000 tof-23.4.1/src/tof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 13:30:02.000000 tof-23.4.1/src/tof.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 13:29:48.000000 tof-23.4.1/tox.ini
```

### Comparing `tof-23.4.0/.github/workflows/ci.yml` & `tof-23.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/.github/workflows/release.yml` & `tof-23.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/.pre-commit-config.yaml` & `tof-23.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/LICENSE` & `tof-23.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/PKG-INFO` & `tof-23.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.4.0
+Version: 23.4.1
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tof-23.4.0/README.md` & `tof-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/conda/meta.yaml` & `tof-23.4.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/_static/detector.png` & `tof-23.4.1/docs/_static/detector.png`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/_static/favicon.ico` & `tof-23.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/_static/logo.svg` & `tof-23.4.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/_static/model.png` & `tof-23.4.1/docs/_static/model.png`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/_static/pulse.png` & `tof-23.4.1/docs/_static/pulse.png`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/conf.py` & `tof-23.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/index.rst` & `tof-23.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/docs/user-guide.ipynb` & `tof-23.4.1/docs/user-guide.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/pyproject.toml` & `tof-23.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tof"
-version = "23.04.0"
+dynamic = ["version"]
 description = "A simple tool to create time-of-flight chopper cascade diagrams"
 license = {text = "BSD-3-Clause"}
 authors = [{name = "Neil Vaytet"}]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
```

### Comparing `tof-23.4.0/requirements/ci.txt` & `tof-23.4.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/requirements/docs.txt` & `tof-23.4.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/requirements/static.txt` & `tof-23.4.1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/src/tof/chopper.py` & `tof-23.4.1/src/tof/chopper.py`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/src/tof/component.py` & `tof-23.4.1/src/tof/component.py`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/src/tof/facilities.py` & `tof-23.4.1/src/tof/facilities.py`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/src/tof/model.py` & `tof-23.4.1/src/tof/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,34 +35,30 @@
             chain(self.choppers, self.detectors),
             key=lambda c: c.distance.value,
         )
 
         initial_mask = sc.ones(
             sizes=self.pulse.birth_times.sizes, unit=None, dtype=bool
         )
-        previous_mask = sc.zeros(
-            sizes=self.pulse.birth_times.sizes, unit=None, dtype=bool
-        )
         for comp in components:
             comp._wavelengths = self.pulse.wavelengths
             t = self.pulse.birth_times + comp.distance / self.pulse.speeds
             comp._arrival_times = t
             if isinstance(comp, Detector):
                 comp._mask = initial_mask
                 continue
             m = sc.zeros(sizes=t.sizes, unit=None, dtype=bool)
             to = comp.open_times
             tc = comp.close_times
             for i in range(len(to)):
                 m |= (t > to[i]) & (t < tc[i])
             combined = initial_mask & m
             comp._mask = combined
-            comp._own_mask = ~m & ~previous_mask
+            comp._own_mask = ~m & initial_mask
             initial_mask = combined
-            previous_mask = ~m
 
     def _add_rays(self, ax, tofs, birth_times, distances, wavelengths=None):
         x0 = birth_times.to(unit='us', copy=False).values.reshape(-1, 1)
         x1 = tofs.to(unit='us', copy=False).values.reshape(-1, 1)
         y0 = np.zeros(x0.size).reshape(-1, 1)
         y1 = distances.values.reshape(-1, 1)
         segments = np.concatenate(
```

### Comparing `tof-23.4.0/src/tof/utils.py` & `tof-23.4.1/src/tof/utils.py`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/src/tof.egg-info/PKG-INFO` & `tof-23.4.1/src/tof.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.4.0
+Version: 23.4.1
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tof-23.4.0/src/tof.egg-info/SOURCES.txt` & `tof-23.4.1/src/tof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tof-23.4.0/tox.ini` & `tof-23.4.1/tox.ini`

 * *Files identical despite different names*

