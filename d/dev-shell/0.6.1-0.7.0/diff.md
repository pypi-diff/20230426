# Comparing `tmp/dev-shell-0.6.1.tar.gz` & `tmp/dev_shell-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-shell-0.6.1.tar", max compression
+gzip compressed data, was "dev_shell-0.7.0.tar", max compression
```

## Comparing `dev-shell-0.6.1.tar` & `dev_shell-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    35149 2021-03-18 17:19:27.789315 dev-shell-0.6.1/LICENSE
--rw-r--r--   0        0        0     5954 2022-09-02 14:50:24.702915 dev-shell-0.6.1/README.md
--rw-r--r--   0        0        0       22 2022-09-02 14:51:11.686586 dev-shell-0.6.1/dev_shell/__init__.py
--rw-r--r--   0        0        0     2478 2022-04-15 13:17:10.986971 dev-shell-0.6.1/dev_shell/base_cmd2_app.py
--rw-r--r--   0        0        0     4464 2022-09-02 14:37:19.924382 dev-shell-0.6.1/dev_shell/bootstrap-source.py
--rw-r--r--   0        0        0      222 2022-04-15 13:17:10.986971 dev-shell-0.6.1/dev_shell/command_sets/__init__.py
--rw-r--r--   0        0        0     4511 2022-09-02 14:37:19.924382 dev-shell-0.6.1/dev_shell/command_sets/dev_shell_commands.py
--rw-r--r--   0        0        0      934 2022-04-15 13:17:10.986971 dev-shell-0.6.1/dev_shell/config.py
--rw-r--r--   0        0        0      463 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/constants.py
--rw-r--r--   0        0        0      976 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/dev_shell_app.py
--rw-r--r--   0        0        0        0 2021-03-18 18:25:58.094467 dev-shell-0.6.1/dev_shell/tests/__init__.py
--rw-r--r--   0        0        0      513 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/tests/constants.py
--rw-r--r--   0        0        0     1584 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/tests/fixtures.py
--rw-r--r--   0        0        0     4162 2022-09-02 14:37:47.848189 dev-shell-0.6.1/dev_shell/tests/test_bootstrap.py
--rw-r--r--   0        0        0     4182 2022-09-02 14:42:54.938056 dev-shell-0.6.1/dev_shell/tests/test_dev_shell_app.py
--rw-r--r--   0        0        0     1390 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/tests/test_source_file.py
--rw-r--r--   0        0        0     6838 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/tests/test_subprocess_utils.py
--rw-r--r--   0        0        0     1824 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/tests/utils.py
--rw-r--r--   0        0        0        0 2021-03-18 17:46:36.232284 dev-shell-0.6.1/dev_shell/utils/__init__.py
--rw-r--r--   0        0        0      534 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/utils/assertion.py
--rw-r--r--   0        0        0     1669 2022-04-15 13:17:10.990970 dev-shell-0.6.1/dev_shell/utils/colorful.py
--rw-r--r--   0        0        0     5306 2022-09-02 14:37:19.924382 dev-shell-0.6.1/dev_shell/utils/subprocess_utils.py
--rw-r--r--   0        0        0     2388 2022-09-02 14:51:52.058303 dev-shell-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     7047 2022-09-02 14:51:57.049705 dev-shell-0.6.1/setup.py
--rw-r--r--   0        0        0     6636 2022-09-02 14:51:57.050347 dev-shell-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-16 07:34:18.881453 dev_shell-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6154 2023-04-25 15:15:45.398151 dev_shell-0.7.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-25 15:20:04.837368 dev_shell-0.7.0/dev_shell/__init__.py
+-rw-r--r--   0        0        0     2478 2023-03-16 07:34:18.881453 dev_shell-0.7.0/dev_shell/base_cmd2_app.py
+-rw-r--r--   0        0        0     4464 2023-03-16 07:34:18.881453 dev_shell-0.7.0/dev_shell/bootstrap-source.py
+-rw-r--r--   0        0        0      222 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/command_sets/__init__.py
+-rw-r--r--   0        0        0     4511 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/command_sets/dev_shell_commands.py
+-rw-r--r--   0        0        0      934 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/config.py
+-rw-r--r--   0        0        0      463 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/constants.py
+-rw-r--r--   0        0        0      976 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/dev_shell_app.py
+-rw-r--r--   0        0        0        0 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/__init__.py
+-rw-r--r--   0        0        0      513 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/constants.py
+-rw-r--r--   0        0        0     1584 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/fixtures.py
+-rw-r--r--   0        0        0     4162 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_bootstrap.py
+-rw-r--r--   0        0        0     4182 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_dev_shell_app.py
+-rw-r--r--   0        0        0     1390 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_source_file.py
+-rw-r--r--   0        0        0     6838 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_subprocess_utils.py
+-rw-r--r--   0        0        0     1884 2023-04-25 15:15:45.406151 dev_shell-0.7.0/dev_shell/tests/utils.py
+-rw-r--r--   0        0        0        0 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/__init__.py
+-rw-r--r--   0        0        0      534 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/assertion.py
+-rw-r--r--   0        0        0     1669 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/colorful.py
+-rw-r--r--   0        0        0     5306 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/subprocess_utils.py
+-rw-r--r--   0        0        0     2359 2023-04-25 15:20:58.233206 dev_shell-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6788 1970-01-01 00:00:00.000000 dev_shell-0.7.0/PKG-INFO
```

### Comparing `dev-shell-0.6.1/LICENSE` & `dev_shell-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/README.md` & `dev_shell-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ![Python Versions](https://img.shields.io/pypi/pyversions/dev-shell)
 ![License GPL V3+](https://img.shields.io/pypi/l/dev-shell)](https://pypi.org/project/dev-shell/)
 
 This small project is intended to improve the start-up for collaborators.
 
 The idea is to make the project setup as simple as possible. Just clone the sources and start a script and you're done ;)
 
-Why in hell not just a `Makefile`? Because it doesn't out-of-the-box under Windows and MacOS, the dev-shell does ;) 
+Why in hell not just a `Makefile`? Because it doesn't out-of-the-box under Windows and MacOS, the dev-shell does ;)
 
 Run Tests? Just start the script and call the "run test command".
 
 The "dev-shell" is the base to create a CLI and a shell. It also shows how to make a project bootstrap as simply as possible, e.g.:
 
 ```bash
 ~$ git clone https://github.com/jedie/dev-shell.git
@@ -92,23 +92,27 @@
 (Using `--update` is not to be confused with the call of "update" command.)
 
 
 ## compatibility
 
 | dev-shell version | OS                      | Python version      |
 |-------------------|-------------------------|---------------------|
+| >=v0.7.0          | Linux + MacOS + Windows | 3.11, 3.10, 3.9     |
 | >=v0.5.0          | Linux + MacOS + Windows | 3.10, 3.9, 3.8, 3.7 |
 | >=v0.0.1          | Linux + MacOS + Windows | 3.9, 3.8, 3.7       |
 
 See also github test configuration: [.github/workflows/test.yml](https://github.com/jedie/dev-shell/blob/main/.github/workflows/test.yml)
 
 ## History
 
-* [*dev*](https://github.com/jedie/dev-shell/compare/v.6.1...main)
+* [*dev*](https://github.com/jedie/dev-shell/compare/v0.7.0...main)
   * TBC
+* [0.7.0 - 2023-04-25](https://github.com/jedie/dev-shell/compare/v0.6.1...v0.7.0)
+  * Update test matrix
+  * update requirements
 * [0.6.1 - 2022-09-02](https://github.com/jedie/dev-shell/compare/v0.6.0...v0.6.1)
   * Set default subprocess timeout to 5 Min.
   * Skip buggy Poetry v1.2.0
   * Update requirements
 * [0.6.0 - 2022-07-19](https://github.com/jedie/dev-shell/compare/v0.5.0...v0.6.0)
   * Add "pyupgrade" as shell command
 * [0.5.0 - 2022-05-29](https://github.com/jedie/dev-shell/compare/v0.4.0...v0.5.0)
```

### Comparing `dev-shell-0.6.1/dev_shell/base_cmd2_app.py` & `dev_shell-0.7.0/dev_shell/base_cmd2_app.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/bootstrap-source.py` & `dev_shell-0.7.0/dev_shell/bootstrap-source.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/command_sets/dev_shell_commands.py` & `dev_shell-0.7.0/dev_shell/command_sets/dev_shell_commands.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/config.py` & `dev_shell-0.7.0/dev_shell/config.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/dev_shell_app.py` & `dev_shell-0.7.0/dev_shell/dev_shell_app.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/tests/constants.py` & `dev_shell-0.7.0/dev_shell/tests/constants.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/tests/fixtures.py` & `dev_shell-0.7.0/dev_shell/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/tests/test_bootstrap.py` & `dev_shell-0.7.0/dev_shell/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/tests/test_dev_shell_app.py` & `dev_shell-0.7.0/dev_shell/tests/test_dev_shell_app.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/tests/test_source_file.py` & `dev_shell-0.7.0/dev_shell/tests/test_source_file.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/tests/test_subprocess_utils.py` & `dev_shell-0.7.0/dev_shell/tests/test_subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/tests/utils.py` & `dev_shell-0.7.0/dev_shell/tests/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,16 +40,18 @@
     """
 
     def __init__(self):
         self._buffer = io.StringIO()
         self._output = None
 
     def __enter__(self):
-        self._stdout_redirect = redirect_stdout(self._buffer).__enter__()
-        self._stderr_redirect = redirect_stderr(self._buffer).__enter__()
+        self._stdout_redirect = redirect_stdout(self._buffer)
+        self._stdout_redirect.__enter__()
+        self._stderr_redirect = redirect_stderr(self._buffer)
+        self._stderr_redirect.__enter__()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             self._output = self._buffer.getvalue()
         finally:
             self._stdout_redirect.__exit__(exc_type, exc_val, exc_tb)
```

### Comparing `dev-shell-0.6.1/dev_shell/utils/assertion.py` & `dev_shell-0.7.0/dev_shell/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/utils/colorful.py` & `dev_shell-0.7.0/dev_shell/utils/colorful.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/dev_shell/utils/subprocess_utils.py` & `dev_shell-0.7.0/dev_shell/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dev-shell-0.6.1/pyproject.toml` & `dev_shell-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "dev-shell"
-version = "0.6.1"
+version = "0.7.0"
 description = "Devloper shell for easy startup..."
 readme = "README.md"
 authors = ["Jens Diemer <python@jensdiemer.de>"]
 homepage = "https://github.com/jedie/dev-shell"
 license = "GNU General Public License v3.0"
 packages = [
     { include = "dev_shell" },
 ]
 
 [tool.poetry.scripts]
 devshell = 'dev_shell.dev_shell_app:devshell_cmdloop'
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0.0"
+python = ">=3.9,<4.0.0"
 cmd2 = "*"  # https://github.com/python-cmd2/cmd2
 
 # fix completion for Mac OS:
 gnureadline = { version = "*", markers = "sys_platform == 'darwin'" }
 
 
 [tool.poetry.dev-dependencies]
 cmd2_ext_test = "*"
 poetry-publish = "*"  # https://github.com/jedie/poetry-publish
 pytest = "*"
 pytest-randomly = "*"
 pytest-cov = "*"
-pytest-darker = "*"  # https://github.com/akaihola/pytest-darker
+darker = "*"  # https://github.com/akaihola/darker
 # TODO: pytest-mypy = "*"
 tox = "*"
 pyupgrade = "*"  # https://github.com/asottile/pyupgrade
 flake8 = "*"
 isort = "*"
 
 [build-system]
@@ -82,29 +82,28 @@
 addopts = """
     --cov=.
     --cov-report term-missing
     --cov-report html
     --cov-report xml
     --no-cov-on-fail
     --showlocals
-    --darker
     --doctest-modules
     --failed-first
     --last-failed-no-failures all
     --new-first
 """
 # TODO: --mypy
 
 
 [tool.tox]
 # https://tox.wiki/en/latest/example/basic.html#pyproject-toml-tox-legacy-ini
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py{37,38,39,310}
+envlist = py{39,310,311}
 skip_missing_interpreters = True
 
 [testenv]
 passenv = *
 commands =
     python --version
     python devshell.py pytest
```

### Comparing `dev-shell-0.6.1/setup.py` & `dev_shell-0.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,174 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dev-shell
+Version: 0.7.0
+Summary: Devloper shell for easy startup...
+Home-page: https://github.com/jedie/dev-shell
+License: GNU General Public License v3.0
+Author: Jens Diemer
+Author-email: python@jensdiemer.de
+Requires-Python: >=3.9,<4.0.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cmd2
+Requires-Dist: gnureadline ; sys_platform == "darwin"
+Description-Content-Type: text/markdown
 
-packages = \
-['dev_shell', 'dev_shell.command_sets', 'dev_shell.tests', 'dev_shell.utils']
+# A "dev-shell" for Python projects ;)
 
-package_data = \
-{'': ['*']}
+[![Test](https://github.com/jedie/dev-shell/actions/workflows/test.yml/badge.svg?branch=bugfix-path)](https://github.com/jedie/dev-shell/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/jedie/dev-shell/branch/main/graph/badge.svg)](https://codecov.io/gh/jedie/dev-shell)
 
-install_requires = \
-['cmd2']
-
-extras_require = \
-{':sys_platform == "darwin"': ['gnureadline']}
-
-entry_points = \
-{'console_scripts': ['devshell = dev_shell.dev_shell_app:devshell_cmdloop']}
-
-setup_kwargs = {
-    'name': 'dev-shell',
-    'version': '0.6.1',
-    'description': 'Devloper shell for easy startup...',
-    'long_description': '# A "dev-shell" for Python projects ;)\n\n[![Test](https://github.com/jedie/dev-shell/actions/workflows/test.yml/badge.svg?branch=bugfix-path)](https://github.com/jedie/dev-shell/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/jedie/dev-shell/branch/main/graph/badge.svg)](https://codecov.io/gh/jedie/dev-shell)\n\n[![ddev-shell @ PyPi](https://img.shields.io/pypi/v/dev-shell?label=dev-shell%20%40%20PyPi)\n![Python Versions](https://img.shields.io/pypi/pyversions/dev-shell)\n![License GPL V3+](https://img.shields.io/pypi/l/dev-shell)](https://pypi.org/project/dev-shell/)\n\nThis small project is intended to improve the start-up for collaborators.\n\nThe idea is to make the project setup as simple as possible. Just clone the sources and start a script and you\'re done ;)\n\nWhy in hell not just a `Makefile`? Because it doesn\'t out-of-the-box under Windows and MacOS, the dev-shell does ;) \n\nRun Tests? Just start the script and call the "run test command".\n\nThe "dev-shell" is the base to create a CLI and a shell. It also shows how to make a project bootstrap as simply as possible, e.g.:\n\n```bash\n~$ git clone https://github.com/jedie/dev-shell.git\n~$ cd dev-shell\n~/dev-shell$ ./devshell.py pytest\n```\n\n\n## How it works\n\nFirst start of the Python script [./devshell.py](https://github.com/jedie/dev-shell/blob/main/devshell.py) will bootstrap:\n\n* Generate a Python virtual environment (in short: `venv`)\n* Install poetry\n* Install project dependencies and the project himself\n\nThe output on first bootstrap start looks like:\n\n```bash\n~/dev-shell$ ./devshell.py\nCreate venv here: ~/dev-shell/.venv\nCollecting pip\n...\nSuccessfully installed pip-21.0.1\nCollecting poetry\n...\nInstalling dependencies from lock file\n\nPackage operations: 31 installs, 1 update, 0 removals\n\n...\n\nInstalling the current project: dev-shell (0.0.1alpha0)\n\n\n+ .venv/bin/python .venv/bin/devshell\n\n\nDeveloper shell - dev_shell - v0.2.0\n\n\nDocumented commands (use \'help -v\' for verbose/\'help <topic>\' for details):\n\ndev-shell commands\n==================\nfix_code_style  linting  list_venv_packages  publish  pytest  update\n\n...\n\n(dev_shell) quit\n~/dev-shell$\n```\n\nThe first bootstrap start takes a few seconds. Each later startup detects the existing virtualenv and is very fast:\n\n```bash\n~/dev-shell$ ./devshell.py\n\nDeveloper shell - dev_shell - v0.2.0\n\n(dev_shell) help\n```\n\nInfo: The `.venv` will be automatically updated via `poetry install` call if the `poetry.lock` file has been changed.\n\nA call with `--update` will force to call some create/update steps, e.g.:\n\n```bash\n~/dev-shell$ ./devshell.py --update\n```\n\nYou can also just delete `/.venv/` and start `devshell.py` again ;)\n\n(Using `--update` is not to be confused with the call of "update" command.)\n\n\n## compatibility\n\n| dev-shell version | OS                      | Python version      |\n|-------------------|-------------------------|---------------------|\n| >=v0.5.0          | Linux + MacOS + Windows | 3.10, 3.9, 3.8, 3.7 |\n| >=v0.0.1          | Linux + MacOS + Windows | 3.9, 3.8, 3.7       |\n\nSee also github test configuration: [.github/workflows/test.yml](https://github.com/jedie/dev-shell/blob/main/.github/workflows/test.yml)\n\n## History\n\n* [*dev*](https://github.com/jedie/dev-shell/compare/v.6.1...main)\n  * TBC\n* [0.6.1 - 2022-09-02](https://github.com/jedie/dev-shell/compare/v0.6.0...v0.6.1)\n  * Set default subprocess timeout to 5 Min.\n  * Skip buggy Poetry v1.2.0\n  * Update requirements\n* [0.6.0 - 2022-07-19](https://github.com/jedie/dev-shell/compare/v0.5.0...v0.6.0)\n  * Add "pyupgrade" as shell command\n* [0.5.0 - 2022-05-29](https://github.com/jedie/dev-shell/compare/v0.4.0...v0.5.0)\n  * Add "tox" and "poetry" commands to call them installed in created ```.venv```\n  * Update requirements\n* [v0.4.0 - 2022-02-28](https://github.com/jedie/dev-shell/compare/v0.3.0...v0.4.0)\n  * Update to new cmd2, colorama and pytest versions\n* [v0.3.0 - 2022-01-30](https://github.com/jedie/dev-shell/compare/v0.2.4...v0.3.0)\n  * Remove "flynt" form linting/fix code style\n* [v0.2.4 - 2022-01-30](https://github.com/jedie/dev-shell/compare/v0.2.3...v0.2.4)\n  * Update requirements\n  * Use darker as code formatter and pytest-darker for linting\n* [v0.2.3 - 2021-11-15](https://github.com/jedie/dev-shell/compare/v0.2.2...v0.2.3)\n  * Update requirements\n  * [Flynt arguments can be changes via CommandSet](https://github.com/jedie/dev-shell/issues/29)\n* [v0.2.2 - 2021-04-13](https://github.com/jedie/dev-shell/compare/v0.2.1...v0.2.2)\n  * Include bootstrap file, to it\'s possible to use it in external projects, too.\n* [v0.2.1 - 2021-04-12](https://github.com/jedie/dev-shell/compare/v0.2.0...v0.2.1)\n  * Handle if "poetry-publish" is not installed, so a project that used "dev-shell" must not install it.\n* [v0.2.0 - 2021-04-11](https://github.com/jedie/dev-shell/compare/v0.1.0...v0.2.0)\n  * Rename: "dev-shell.py => devshell.py" because of better autocomplete\n  * Add `DevShellConfig.base_path` and use it in own commands like, `pytest`, `linting` etc. (So they are usable in external project, too.)\n  * recognize "--update" and "--help" arguments better in `./devshell.py` calls.\n  * Update `setuptools` on `.venv` creation, too.\n  * Fix Bugs/tests under Windows\n* [v0.1.0 - 2021-03-22](https://github.com/jedie/dev-shell/compare/v0.0.2...v0.1.0)\n  * Fix CI usage: Exit with correct return code if tests failed\n  * Better "run as CLI" implementation via new `run_cmd2_app()`\n  * Bugfix errors that only occur on Windows.\n  * Simplify `devshell.py` boot script and fix raise error if `ensurepip` missing\n* [v0.0.2 - 2021-03-19](https://github.com/jedie/dev-shell/compare/v0.0.1...v0.0.2)\n  * refactor colorful shortcuts\n  * display subprocess calls with separated colors\n* [v0.0.1 - 2021-03-19](https://github.com/jedie/dev-shell/compare/ad5dca...v0.0.1)\n  * first "useable" version\n\n## Project links\n\n* Github: https://github.com/jedie/dev-shell/\n* PyPi: https://pypi.org/project/dev-shell/\n',
-    'author': 'Jens Diemer',
-    'author_email': 'python@jensdiemer.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/jedie/dev-shell',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0.0',
-}
+[![ddev-shell @ PyPi](https://img.shields.io/pypi/v/dev-shell?label=dev-shell%20%40%20PyPi)
+![Python Versions](https://img.shields.io/pypi/pyversions/dev-shell)
+![License GPL V3+](https://img.shields.io/pypi/l/dev-shell)](https://pypi.org/project/dev-shell/)
 
+This small project is intended to improve the start-up for collaborators.
+
+The idea is to make the project setup as simple as possible. Just clone the sources and start a script and you're done ;)
+
+Why in hell not just a `Makefile`? Because it doesn't out-of-the-box under Windows and MacOS, the dev-shell does ;)
+
+Run Tests? Just start the script and call the "run test command".
+
+The "dev-shell" is the base to create a CLI and a shell. It also shows how to make a project bootstrap as simply as possible, e.g.:
+
+```bash
+~$ git clone https://github.com/jedie/dev-shell.git
+~$ cd dev-shell
+~/dev-shell$ ./devshell.py pytest
+```
+
+
+## How it works
+
+First start of the Python script [./devshell.py](https://github.com/jedie/dev-shell/blob/main/devshell.py) will bootstrap:
+
+* Generate a Python virtual environment (in short: `venv`)
+* Install poetry
+* Install project dependencies and the project himself
+
+The output on first bootstrap start looks like:
+
+```bash
+~/dev-shell$ ./devshell.py
+Create venv here: ~/dev-shell/.venv
+Collecting pip
+...
+Successfully installed pip-21.0.1
+Collecting poetry
+...
+Installing dependencies from lock file
+
+Package operations: 31 installs, 1 update, 0 removals
+
+...
+
+Installing the current project: dev-shell (0.0.1alpha0)
+
+
++ .venv/bin/python .venv/bin/devshell
+
+
+Developer shell - dev_shell - v0.2.0
+
+
+Documented commands (use 'help -v' for verbose/'help <topic>' for details):
+
+dev-shell commands
+==================
+fix_code_style  linting  list_venv_packages  publish  pytest  update
+
+...
+
+(dev_shell) quit
+~/dev-shell$
+```
+
+The first bootstrap start takes a few seconds. Each later startup detects the existing virtualenv and is very fast:
+
+```bash
+~/dev-shell$ ./devshell.py
+
+Developer shell - dev_shell - v0.2.0
+
+(dev_shell) help
+```
+
+Info: The `.venv` will be automatically updated via `poetry install` call if the `poetry.lock` file has been changed.
+
+A call with `--update` will force to call some create/update steps, e.g.:
+
+```bash
+~/dev-shell$ ./devshell.py --update
+```
+
+You can also just delete `/.venv/` and start `devshell.py` again ;)
+
+(Using `--update` is not to be confused with the call of "update" command.)
+
+
+## compatibility
+
+| dev-shell version | OS                      | Python version      |
+|-------------------|-------------------------|---------------------|
+| >=v0.7.0          | Linux + MacOS + Windows | 3.11, 3.10, 3.9     |
+| >=v0.5.0          | Linux + MacOS + Windows | 3.10, 3.9, 3.8, 3.7 |
+| >=v0.0.1          | Linux + MacOS + Windows | 3.9, 3.8, 3.7       |
+
+See also github test configuration: [.github/workflows/test.yml](https://github.com/jedie/dev-shell/blob/main/.github/workflows/test.yml)
+
+## History
+
+* [*dev*](https://github.com/jedie/dev-shell/compare/v0.7.0...main)
+  * TBC
+* [0.7.0 - 2023-04-25](https://github.com/jedie/dev-shell/compare/v0.6.1...v0.7.0)
+  * Update test matrix
+  * update requirements
+* [0.6.1 - 2022-09-02](https://github.com/jedie/dev-shell/compare/v0.6.0...v0.6.1)
+  * Set default subprocess timeout to 5 Min.
+  * Skip buggy Poetry v1.2.0
+  * Update requirements
+* [0.6.0 - 2022-07-19](https://github.com/jedie/dev-shell/compare/v0.5.0...v0.6.0)
+  * Add "pyupgrade" as shell command
+* [0.5.0 - 2022-05-29](https://github.com/jedie/dev-shell/compare/v0.4.0...v0.5.0)
+  * Add "tox" and "poetry" commands to call them installed in created ```.venv```
+  * Update requirements
+* [v0.4.0 - 2022-02-28](https://github.com/jedie/dev-shell/compare/v0.3.0...v0.4.0)
+  * Update to new cmd2, colorama and pytest versions
+* [v0.3.0 - 2022-01-30](https://github.com/jedie/dev-shell/compare/v0.2.4...v0.3.0)
+  * Remove "flynt" form linting/fix code style
+* [v0.2.4 - 2022-01-30](https://github.com/jedie/dev-shell/compare/v0.2.3...v0.2.4)
+  * Update requirements
+  * Use darker as code formatter and pytest-darker for linting
+* [v0.2.3 - 2021-11-15](https://github.com/jedie/dev-shell/compare/v0.2.2...v0.2.3)
+  * Update requirements
+  * [Flynt arguments can be changes via CommandSet](https://github.com/jedie/dev-shell/issues/29)
+* [v0.2.2 - 2021-04-13](https://github.com/jedie/dev-shell/compare/v0.2.1...v0.2.2)
+  * Include bootstrap file, to it's possible to use it in external projects, too.
+* [v0.2.1 - 2021-04-12](https://github.com/jedie/dev-shell/compare/v0.2.0...v0.2.1)
+  * Handle if "poetry-publish" is not installed, so a project that used "dev-shell" must not install it.
+* [v0.2.0 - 2021-04-11](https://github.com/jedie/dev-shell/compare/v0.1.0...v0.2.0)
+  * Rename: "dev-shell.py => devshell.py" because of better autocomplete
+  * Add `DevShellConfig.base_path` and use it in own commands like, `pytest`, `linting` etc. (So they are usable in external project, too.)
+  * recognize "--update" and "--help" arguments better in `./devshell.py` calls.
+  * Update `setuptools` on `.venv` creation, too.
+  * Fix Bugs/tests under Windows
+* [v0.1.0 - 2021-03-22](https://github.com/jedie/dev-shell/compare/v0.0.2...v0.1.0)
+  * Fix CI usage: Exit with correct return code if tests failed
+  * Better "run as CLI" implementation via new `run_cmd2_app()`
+  * Bugfix errors that only occur on Windows.
+  * Simplify `devshell.py` boot script and fix raise error if `ensurepip` missing
+* [v0.0.2 - 2021-03-19](https://github.com/jedie/dev-shell/compare/v0.0.1...v0.0.2)
+  * refactor colorful shortcuts
+  * display subprocess calls with separated colors
+* [v0.0.1 - 2021-03-19](https://github.com/jedie/dev-shell/compare/ad5dca...v0.0.1)
+  * first "useable" version
+
+## Project links
+
+* Github: https://github.com/jedie/dev-shell/
+* PyPi: https://pypi.org/project/dev-shell/
 
-setup(**setup_kwargs)
```

