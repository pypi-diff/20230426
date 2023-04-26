# Comparing `tmp/git-open-1.2.2.tar.gz` & `tmp/git-open-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-open-1.2.2.tar", last modified: Tue Jan 18 13:51:30 2022, max compression
+gzip compressed data, was "git-open-1.3.0.tar", last modified: Wed Apr 26 18:24:11 2023, max compression
```

## Comparing `git-open-1.2.2.tar` & `git-open-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.239612 git-open-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-01-18 13:51:18.000000 git-open-1.2.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-01-18 13:51:18.000000 git-open-1.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-01-18 13:51:18.000000 git-open-1.2.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.235612 git-open-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-01-18 13:51:18.000000 git-open-1.2.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-18 13:51:18.000000 git-open-1.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.235612 git-open-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-01-18 13:51:18.000000 git-open-1.2.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-01-18 13:51:18.000000 git-open-1.2.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-01-18 13:51:18.000000 git-open-1.2.2/.github/workflows/merge-dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-01-18 13:51:18.000000 git-open-1.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-01-18 13:51:18.000000 git-open-1.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-01-18 13:51:18.000000 git-open-1.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-18 13:51:18.000000 git-open-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-01-18 13:51:18.000000 git-open-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-01-18 13:51:18.000000 git-open-1.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-01-18 13:51:30.239612 git-open-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-01-18 13:51:18.000000 git-open-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-01-18 13:51:18.000000 git-open-1.2.2/dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.235612 git-open-1.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-18 13:51:18.000000 git-open-1.2.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-01-18 13:51:18.000000 git-open-1.2.2/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-01-18 13:51:18.000000 git-open-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-01-18 13:51:30.239612 git-open-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3192 2022-01-18 13:51:18.000000 git-open-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.231612 git-open-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.235612 git-open-1.2.2/src/git_open/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-01-18 13:51:18.000000 git-open-1.2.2/src/git_open/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-01-18 13:51:18.000000 git-open-1.2.2/src/git_open/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2022-01-18 13:51:18.000000 git-open-1.2.2/src/git_open/git_open.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.239612 git-open-1.2.2/src/git_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-01-18 13:51:30.000000 git-open-1.2.2/src/git_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-01-18 13:51:30.000000 git-open-1.2.2/src/git_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-18 13:51:30.000000 git-open-1.2.2/src/git_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-18 13:51:30.000000 git-open-1.2.2/src/git_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-18 13:51:30.000000 git-open-1.2.2/src/git_open.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-01-18 13:51:30.000000 git-open-1.2.2/src/git_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-18 13:51:30.000000 git-open-1.2.2/src/git_open.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 13:51:30.239612 git-open-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-18 13:51:18.000000 git-open-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-01-18 13:51:18.000000 git-open-1.2.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-01-18 13:51:18.000000 git-open-1.2.2/tests/test__open_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-01-18 13:51:18.000000 git-open-1.2.2/tests/test__open_commit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3483 2022-01-18 13:51:18.000000 git-open-1.2.2/tests/test__open_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-01-18 13:51:18.000000 git-open-1.2.2/tests/test_git_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.292179 git-open-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-26 18:23:54.000000 git-open-1.3.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 18:23:54.000000 git-open-1.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-26 18:23:54.000000 git-open-1.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.288179 git-open-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-26 18:23:54.000000 git-open-1.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 18:23:54.000000 git-open-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.288179 git-open-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-26 18:23:54.000000 git-open-1.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 18:23:54.000000 git-open-1.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-26 18:23:54.000000 git-open-1.3.0/.github/workflows/merge-dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-26 18:23:54.000000 git-open-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-26 18:23:54.000000 git-open-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 18:23:54.000000 git-open-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 18:23:54.000000 git-open-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-26 18:23:54.000000 git-open-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-26 18:23:54.000000 git-open-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-26 18:24:11.292179 git-open-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-26 18:23:54.000000 git-open-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-26 18:23:54.000000 git-open-1.3.0/dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.288179 git-open-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 18:23:54.000000 git-open-1.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 18:23:54.000000 git-open-1.3.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 18:23:54.000000 git-open-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-26 18:24:11.292179 git-open-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-26 18:23:54.000000 git-open-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.288179 git-open-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.288179 git-open-1.3.0/src/git_open/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 18:23:54.000000 git-open-1.3.0/src/git_open/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-26 18:23:54.000000 git-open-1.3.0/src/git_open/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 18:23:54.000000 git-open-1.3.0/src/git_open/git_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.288179 git-open-1.3.0/src/git_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-26 18:24:11.000000 git-open-1.3.0/src/git_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-26 18:24:11.000000 git-open-1.3.0/src/git_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:24:11.000000 git-open-1.3.0/src/git_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 18:24:11.000000 git-open-1.3.0/src/git_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:24:11.000000 git-open-1.3.0/src/git_open.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-26 18:24:11.000000 git-open-1.3.0/src/git_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 18:24:11.000000 git-open-1.3.0/src/git_open.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:24:11.292179 git-open-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 18:23:54.000000 git-open-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-26 18:23:54.000000 git-open-1.3.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 18:23:54.000000 git-open-1.3.0/tests/test__open_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-26 18:23:54.000000 git-open-1.3.0/tests/test__open_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-26 18:23:54.000000 git-open-1.3.0/tests/test__open_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-26 18:23:54.000000 git-open-1.3.0/tests/test__open_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-26 18:23:54.000000 git-open-1.3.0/tests/test_git_open.py
```

### Comparing `git-open-1.2.2/.github/workflows/codeql-analysis.yml` & `git-open-1.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/.github/workflows/main.yml` & `git-open-1.3.0/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Test
 
-on: [push, pull_request]
+on: [push, pull_request, workflow_dispatch]
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.8]
@@ -26,15 +26,15 @@
       - name: Check manifest
         run: check-manifest
 
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9, pypy3]
+        python-version: [3.9]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `git-open-1.2.2/.github/workflows/release.yml` & `git-open-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/CHANGELOG.md` & `git-open-1.3.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Changelog
 =========
 
 **unreleased**
 
+v1.3.0
+-----
+- Adds the `actions` command
+
 v1.2.2
 -----
 - Bumps dependencies
 - Fixes the issue with `git+ssh://` in remotes <https://github.com/cfarvidson/git-open/pull/267>
 
 v1.2.1
 -----
```

### Comparing `git-open-1.2.2/CONTRIBUTING.md` & `git-open-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/LICENSE` & `git-open-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/Makefile` & `git-open-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/PKG-INFO` & `git-open-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 Metadata-Version: 2.1
 Name: git-open
-Version: 1.2.2
+Version: 1.3.0
 Summary: Open a git repo in the browser from the terminal.
 Home-page: https://github.com/cfp2000/git-open
 Author: 
 Author-email: cfp@highball.se
 Maintainer: 
 Maintainer-email: cfp@highball.se
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/cfp2000/git-open/issues
 Project-URL: Source Code, https://github.com/cfp2000/git-open
 Keywords: terminal,git,web
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: setup
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
@@ -100,14 +94,18 @@
 
 
 Changelog
 =========
 
 **unreleased**
 
+v1.3.0
+-----
+- Adds the `actions` command
+
 v1.2.2
 -----
 - Bumps dependencies
 - Fixes the issue with `git+ssh://` in remotes <https://github.com/cfarvidson/git-open/pull/267>
 
 v1.2.1
 -----
@@ -181,9 +179,7 @@
 -----
 - Update the install description
 
 v0.0.1
 -----
 * Implemented tox testing
 * Created
-
-
```

### Comparing `git-open-1.2.2/README.md` & `git-open-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/setup.py` & `git-open-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,21 +19,16 @@
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Utilities",
 ]
 INSTALL_REQUIRES = ["Click>=6.7", "sh>=1.12.14", "six>=1.11.0"]
 EXTRAS_REQUIRE = {
     "docs": ["sphinx"],
     "setup": ["wheel"],
     "tests": ["pytest", "coverage", "flake8", "six"],
```

### Comparing `git-open-1.2.2/src/git_open/git_open.py` & `git-open-1.3.0/src/git_open/git_open.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,17 @@
             prefix = "/-"
         self.url += "%s/compare/%s...%s" % (prefix, target, current_commit_hash)
 
     def add_branch_to_url(self):
         branch = GitOpen.get_current_branch()
         self.url += "/tree/%s" % branch
 
+    def add_actions_to_url(self):
+        self.url += "/actions"
+
     @staticmethod
     def get_remotes():
         try:
             remotes = sh.git("remote", "-v").stdout
             if isinstance(remotes, six.binary_type):
                 remotes = remotes.decode()
             return remotes
```

### Comparing `git-open-1.2.2/src/git_open.egg-info/PKG-INFO` & `git-open-1.3.0/src/git_open.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 Metadata-Version: 2.1
 Name: git-open
-Version: 1.2.2
+Version: 1.3.0
 Summary: Open a git repo in the browser from the terminal.
 Home-page: https://github.com/cfp2000/git-open
 Author: 
 Author-email: cfp@highball.se
 Maintainer: 
 Maintainer-email: cfp@highball.se
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/cfp2000/git-open/issues
 Project-URL: Source Code, https://github.com/cfp2000/git-open
 Keywords: terminal,git,web
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: setup
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
@@ -100,14 +94,18 @@
 
 
 Changelog
 =========
 
 **unreleased**
 
+v1.3.0
+-----
+- Adds the `actions` command
+
 v1.2.2
 -----
 - Bumps dependencies
 - Fixes the issue with `git+ssh://` in remotes <https://github.com/cfarvidson/git-open/pull/267>
 
 v1.2.1
 -----
@@ -181,9 +179,7 @@
 -----
 - Update the install description
 
 v0.0.1
 -----
 * Implemented tox testing
 * Created
-
-
```

### Comparing `git-open-1.2.2/src/git_open.egg-info/SOURCES.txt` & `git-open-1.3.0/src/git_open.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,11 +27,12 @@
 src/git_open.egg-info/dependency_links.txt
 src/git_open.egg-info/entry_points.txt
 src/git_open.egg-info/not-zip-safe
 src/git_open.egg-info/requires.txt
 src/git_open.egg-info/top_level.txt
 tests/__init__.py
 tests/helpers.py
+tests/test__open_actions.py
 tests/test__open_branch.py
 tests/test__open_commit.py
 tests/test__open_compare.py
 tests/test_git_open.py
```

### Comparing `git-open-1.2.2/tests/test__open_branch.py` & `git-open-1.3.0/tests/test__open_branch.py`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/tests/test__open_commit.py` & `git-open-1.3.0/tests/test__open_commit.py`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/tests/test__open_compare.py` & `git-open-1.3.0/tests/test__open_compare.py`

 * *Files identical despite different names*

### Comparing `git-open-1.2.2/tests/test_git_open.py` & `git-open-1.3.0/tests/test_git_open.py`

 * *Files identical despite different names*

