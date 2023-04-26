# Comparing `tmp/pytest-flask-ligand-0.1.8.tar.gz` & `tmp/pytest-flask-ligand-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-flask-ligand-0.1.8.tar", last modified: Fri Feb 10 20:42:46 2023, max compression
+gzip compressed data, was "pytest-flask-ligand-0.1.9.tar", last modified: Tue Apr 25 22:43:52 2023, max compression
```

## Comparing `pytest-flask-ligand-0.1.8.tar` & `pytest-flask-ligand-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.229444 pytest-flask-ligand-0.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.225444 pytest-flask-ligand-0.1.8/.github/
--rw-r--r--   0 root         (0) root         (0)      528 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.225444 pytest-flask-ligand-0.1.8/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      625 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.github/workflows/bump_and_publish_release.yml
--rw-r--r--   0 root         (0) root         (0)      797 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.github/workflows/coverage.yml
--rw-r--r--   0 root         (0) root         (0)      622 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.github/workflows/pull_request.yml
--rw-r--r--   0 root         (0) root         (0)      687 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.225444 pytest-flask-ligand-0.1.8/.run/
--rw-r--r--   0 root         (0) root         (0)      822 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.run/Unit (tox).run.xml
--rw-r--r--   0 root         (0) root         (0)      870 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.run/Unit (tox-fast).run.xml
--rw-r--r--   0 root         (0) root         (0)     1029 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/.run/Unit.run.xml
--rw-r--r--   0 root         (0) root         (0)       36 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6949 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     3933 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    35149 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5086 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/Makefile
--rw-r--r--   0 root         (0) root         (0)     4098 2023-02-10 20:42:46.229444 pytest-flask-ligand-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2776 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.225444 pytest-flask-ligand-0.1.8/docs/
--rw-r--r--   0 root         (0) root         (0)     2412 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/docs/release_process.rst
--rw-r--r--   0 root         (0) root         (0)      889 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.225444 pytest-flask-ligand-0.1.8/pytest_flask_ligand/
--rw-r--r--   0 root         (0) root         (0)     4921 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.225444 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4098 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      865 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       44 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-02-10 20:42:46.000000 pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      247 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1523 2023-02-10 20:42:46.229444 pytest-flask-ligand-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      737 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:42:46.229444 pytest-flask-ligand-0.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4221 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/tests/test_flask_ligand.py
--rw-r--r--   0 root         (0) root         (0)      364 2023-02-10 20:42:42.000000 pytest-flask-ligand-0.1.8/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/.github/
+-rw-r--r--   0 root         (0) root         (0)      528 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.github/workflows/bump_and_publish_release.yml
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.github/workflows/coverage.yml
+-rw-r--r--   0 root         (0) root         (0)      622 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.github/workflows/pull_request.yml
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/.run/
+-rw-r--r--   0 root         (0) root         (0)      822 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.run/Unit (tox).run.xml
+-rw-r--r--   0 root         (0) root         (0)      870 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.run/Unit (tox-fast).run.xml
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/.run/Unit.run.xml
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     9447 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/Makefile
+-rw-r--r--   0 root         (0) root         (0)     4098 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/docs/
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/docs/release_process.rst
+-rw-r--r--   0 root         (0) root         (0)      889 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/pytest_flask_ligand/
+-rw-r--r--   0 root         (0) root         (0)     4921 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4098 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      865 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-25 22:43:52.000000 pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:52.911808 pytest-flask-ligand-0.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/tests/test_flask_ligand.py
+-rw-r--r--   0 root         (0) root         (0)      364 2023-04-25 22:43:49.000000 pytest-flask-ligand-0.1.9/tox.ini
```

### Comparing `pytest-flask-ligand-0.1.8/.github/dependabot.yml` & `pytest-flask-ligand-0.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/.github/workflows/bump_and_publish_release.yml` & `pytest-flask-ligand-0.1.9/.github/workflows/bump_and_publish_release.yml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/.github/workflows/coverage.yml` & `pytest-flask-ligand-0.1.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/.github/workflows/pull_request.yml` & `pytest-flask-ligand-0.1.9/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/.pre-commit-config.yaml` & `pytest-flask-ligand-0.1.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     hooks:
     -   id: check-yaml
     -   id: check-toml
     -   id: detect-private-key
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.2.0
     hooks:
     -   id: mypy
         additional_dependencies: ["types-setuptools ~= 63.4", "types-python-dateutil ~= 2.8"]
 -   repo: https://github.com/rstcheck/rstcheck
-    rev: v6.1.1
+    rev: v6.1.2
     hooks:
     -   id: rstcheck
```

### Comparing `pytest-flask-ligand-0.1.8/.run/Unit (tox).run.xml` & `pytest-flask-ligand-0.1.9/.run/Unit (tox).run.xml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/.run/Unit (tox-fast).run.xml` & `pytest-flask-ligand-0.1.9/.run/Unit (tox-fast).run.xml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/.run/Unit.run.xml` & `pytest-flask-ligand-0.1.9/.run/Unit.run.xml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/CHANGELOG.md` & `pytest-flask-ligand-0.1.9/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 Changelog
 =========
 
 <!--next-version-placeholder-->
 
+## v0.1.9 (2023-04-25)
+### Fix
+* :arrow_up: Update types-setuptools requirement from ~=67.5 to ~=67.6 ([`dc7fe76`](https://github.com/cowofevil/pytest-flask-ligand/commit/dc7fe76654bf21e3f70ca76e7a7543f875135a55))
+* :arrow_up: Update mypy requirement from ~=1.0 to ~=1.1 ([`ad7e49b`](https://github.com/cowofevil/pytest-flask-ligand/commit/ad7e49bc94d75244f70559e42328a5c85d1aaf7e))
+* :arrow_up: Update pre-commit requirement from ~=3.0 to ~=3.1 ([`9b3fc95`](https://github.com/cowofevil/pytest-flask-ligand/commit/9b3fc95a0015d54ef9bc77da7b98215b69be52ef))
+* :arrow_up: Update coverage[toml] requirement from ~=7.1 to ~=7.2 ([`d60cbc7`](https://github.com/cowofevil/pytest-flask-ligand/commit/d60cbc77f92e360f8df731c5af51a1006543c8a4))
+* :arrow_up: Update ipython requirement from ~=8.10 to ~=8.11 ([`d3a822c`](https://github.com/cowofevil/pytest-flask-ligand/commit/d3a822c4425411eec5ef23579c68d96b820b5fff))
+* :arrow_up: Update types-setuptools requirement from ~=67.3 to ~=67.5 ([`c7c1f28`](https://github.com/cowofevil/pytest-flask-ligand/commit/c7c1f28d40b2ac7c507c4ae21b0df69d44563b3b))
+* :arrow_up: Update types-setuptools requirement from ~=67.1 to ~=67.3 ([`4c2b838`](https://github.com/cowofevil/pytest-flask-ligand/commit/4c2b838f1cc5f8a254a9da1d3c98ae8416b3c58d))
+* :arrow_up: Update mypy requirement from ~=0.991 to ~=1.0 ([#58](https://github.com/cowofevil/pytest-flask-ligand/issues/58)) ([`e9fdaa2`](https://github.com/cowofevil/pytest-flask-ligand/commit/e9fdaa2e05e74327e224a3a8209643d95785d257))
+* :arrow_up: Update black requirement from ~=22.12 to ~=23.1 ([`cfaeb58`](https://github.com/cowofevil/pytest-flask-ligand/commit/cfaeb58bd937e4459a5ea03d2100dc3874574790))
+* :arrow_up: Update python-semantic-release requirement ([`94d9c84`](https://github.com/cowofevil/pytest-flask-ligand/commit/94d9c847332b2624a5feab72a0636b23fcdf499e))
+* :arrow_up: Update ipython requirement from ~=8.8 to ~=8.10 ([`8a5e413`](https://github.com/cowofevil/pytest-flask-ligand/commit/8a5e413aefa41eff25d580a0339277adae6ccbb1))
+
+### Other
+* [pre-commit.ci] pre-commit autoupdate ([`09833b9`](https://github.com/cowofevil/pytest-flask-ligand/commit/09833b96d8d2d0e762da4db01db3d68319f9298f))
+* [pre-commit.ci] pre-commit autoupdate ([`6557bf0`](https://github.com/cowofevil/pytest-flask-ligand/commit/6557bf044b339bd7ccd33b2b66382a51779f8dbf))
+* [pre-commit.ci] pre-commit autoupdate ([`93a56d7`](https://github.com/cowofevil/pytest-flask-ligand/commit/93a56d79c5eba8ee4b567e576c9482e403d0b6b1))
+
 ## v0.1.8 (2023-02-10)
 ### Fix
 * [560:robot:] Fix Packaging Issues ([`7452032`](https://github.com/cowofevil/pytest-flask-ligand/commit/74520324358a4dd63f5a264c4fd02c9c7472f4d7))
 
 ### Other
 * [pre-commit.ci] pre-commit autoupdate ([`69088d0`](https://github.com/cowofevil/pytest-flask-ligand/commit/69088d003b39fe0b568199798cc2a2f65fcc01d4))
```

### Comparing `pytest-flask-ligand-0.1.8/CONTRIBUTING.rst` & `pytest-flask-ligand-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/LICENSE` & `pytest-flask-ligand-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/Makefile` & `pytest-flask-ligand-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/PKG-INFO` & `pytest-flask-ligand-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-flask-ligand
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pytest fixtures and helper functions to use for testing flask-ligand microservices.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Changelog, https://github.com/cowofevil/pytest-flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/pytest-flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/pytest-flask-ligand/issues
```

### Comparing `pytest-flask-ligand-0.1.8/README.rst` & `pytest-flask-ligand-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/docs/release_process.rst` & `pytest-flask-ligand-0.1.9/docs/release_process.rst`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/pyproject.toml` & `pytest-flask-ligand-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/pytest_flask_ligand/__init__.py` & `pytest-flask-ligand-0.1.9/pytest_flask_ligand/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Any
 
 
 # ======================================================================================================================
 # Globals
 # ======================================================================================================================
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 DUMMY_ID = str(uuid.UUID("00000000-0000-0000-0000-000000000000"))
 DUMMY_ETAG = "0000000000000000000000000000000000000000"
 USER_ID = DUMMY_ID
 USER_DEFAULT_ROLES = ["admin", "user"]
 OPEN_API_CLIENT_NAME = "ligand-client"
 ISO_8601_REGEX = (
     r"^(?:[1-9]\d{3}-(?:(?:0[1-9]|1[0-2])-(?:0[1-9]|1\d|2[0-8])|(?:0[13-9]|1[0-2])-(?:29|30)|"
```

### Comparing `pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/PKG-INFO` & `pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-flask-ligand
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pytest fixtures and helper functions to use for testing flask-ligand microservices.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Changelog, https://github.com/cowofevil/pytest-flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/pytest-flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/pytest-flask-ligand/issues
```

### Comparing `pytest-flask-ligand-0.1.8/pytest_flask_ligand.egg-info/SOURCES.txt` & `pytest-flask-ligand-0.1.9/pytest_flask_ligand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/setup.cfg` & `pytest-flask-ligand-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest-flask-ligand
-version = 0.1.8
+version = 0.1.9
 summary = Pytest fixtures and helper functions to use for testing flask-ligand microservices.
 description_file = README.rst
 author = Ryan Gard
 author_email = ryan@gardiancapitol.com
 description_content_type = text/x-rst; charset=UTF-8
 keywords = test, unittest
 license = GNU General Public License v3 (GPLv3)
```

### Comparing `pytest-flask-ligand-0.1.8/setup.py` & `pytest-flask-ligand-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-flask-ligand-0.1.8/tests/test_flask_ligand.py` & `pytest-flask-ligand-0.1.9/tests/test_flask_ligand.py`

 * *Files identical despite different names*

