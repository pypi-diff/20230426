# Comparing `tmp/parasect-1.1.1.tar.gz` & `tmp/parasect-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parasect-1.1.1.tar", max compression
+gzip compressed data, was "parasect-1.1.2.tar", max compression
```

## Comparing `parasect-1.1.1.tar` & `parasect-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1080 2023-04-23 17:58:42.205257 parasect-1.1.1/LICENSE.rst
--rw-r--r--   0        0        0     4351 2023-04-23 17:58:42.205257 parasect-1.1.1/README.rst
--rw-r--r--   0        0        0     2234 2023-04-23 17:58:59.229601 parasect-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      193 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/__init__.py
--rw-r--r--   0        0        0     3502 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/__main__.py
--rw-r--r--   0        0        0    27529 2023-04-23 17:58:59.233601 parasect-1.1.1/src/parasect/_helpers.py
--rwxr-xr-x   0        0        0    28187 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/build_lib.py
--rwxr-xr-x   0        0        0    15184 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/compare_lib.py
--rw-r--r--   0        0        0        0 2023-04-23 17:58:42.213257 parasect-1.1.1/src/parasect/py.typed
--rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 parasect-1.1.1/setup.py
--rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 parasect-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-26 11:56:51.177681 parasect-1.1.2/LICENSE.rst
+-rw-r--r--   0        0        0     4351 2023-04-26 11:56:51.177681 parasect-1.1.2/README.rst
+-rw-r--r--   0        0        0     2233 2023-04-26 11:57:09.569968 parasect-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/__init__.py
+-rw-r--r--   0        0        0     3502 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/__main__.py
+-rw-r--r--   0        0        0    27635 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/_helpers.py
+-rwxr-xr-x   0        0        0    28340 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/build_lib.py
+-rwxr-xr-x   0        0        0    15184 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/compare_lib.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:56:51.181681 parasect-1.1.2/src/parasect/py.typed
+-rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 parasect-1.1.2/PKG-INFO
```

### Comparing `parasect-1.1.1/LICENSE.rst` & `parasect-1.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `parasect-1.1.1/README.rst` & `parasect-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `parasect-1.1.1/pyproject.toml` & `parasect-1.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parasect"
-version = "1.1.1"
+version = "1.1.2"
 description = "Utility for manipulating parameter sets for autopilots."
 authors = ["George Zogopoulos <geo.zogop.papal@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/AvyFly/parasect"
 repository = "https://github.com/AvyFly/parasect"
 documentation = "https://parasect.readthedocs.io"
@@ -23,32 +23,32 @@
 pydantic = "^1.9.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 coverage = {extras = ["toml"], version = "^7.2"}
 safety = "^2.2.0"
 mypy = "^1.0.1"
-typeguard = "^2.13.2"
+typeguard = "^2.13.3"
 xdoctest = {extras = ["colors"], version = "^1.0.0"}
-sphinx = "^6.1.3"
+sphinx = "^6.2.1"
 sphinx-autobuild = ">=2021.3.14"
-pre-commit = "^2.15.0"
+pre-commit = "^3.2.2"
 flake8 = "^4.0.1"
 black = ">=21.10b0"
 flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.4.25"
+flake8-bugbear = "^23.3.12"
 flake8-docstrings = "^1.6.0"
 flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.0"
 darglint = "^1.8.1"
 reorder-python-imports = "^3.1.0"
 pre-commit-hooks = "^4.3.0"
 sphinx-click = "^4.4.0"
 Pygments = "^2.10.0"
-pyupgrade = "^3.3.1"
+pyupgrade = "^3.3.2"
 furo = ">=2022.12.7"
 
 [tool.poetry.scripts]
 parasect = "parasect.__main__:cli"
 
 [tool.poetry.group.dev.dependencies]
 directory-tree = "^0.0.3.1"
```

### Comparing `parasect-1.1.1/src/parasect/__main__.py` & `parasect-1.1.2/src/parasect/__main__.py`

 * *Files identical despite different names*

### Comparing `parasect-1.1.1/src/parasect/_helpers.py` & `parasect-1.1.2/src/parasect/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
     default_value: Union[int, float]
     min_value = float("-inf")
     max_value = float("inf")
     increment = None  # Instruction for increments for UIs
     unit = None
     decimal = None  # Suggested increment by the parameter documentation
     reboot_required = False
-    group = None
+    group: Optional[str] = None
     vid: int  # Vehicle ID, default 1
     cid: int  # Component ID, default 1
 
     def __init__(
         self,
         name: str,
         value: Union[int, float],
@@ -576,16 +576,15 @@
         for param_name in sorted(self.params.keys()):
             yield self.params[param_name]
 
     def __sub__(self, other: "ParameterList") -> "ParameterList":
         """Subtract a ParameterList from another ParameterList."""
         param_list = ParameterList(self)
         for param in param_list:
-            param_hash = self.build_param_hash_from_param(param)
-            if param_hash in other.keys():
+            if param in other:
                 param_list.remove_param(param)
         return param_list
 
     def __str__(self) -> str:
         """__str__ dunder method."""
         param_strings = []
         for param_name in sorted(self.params.keys()):
@@ -635,17 +634,19 @@
         param_hash = self.build_param_hash_from_param(param)
         if safe and param_hash not in self.params.keys():
             raise KeyError(f"{param.name} with cid={param.cid} is not an existing key")
         if not overwrite and param_hash in self.params.keys():
             raise KeyError(f"Tried to overwrite key {param.name} with cid={param.cid}")
         # If parameter doesn't exist, create it
         if param_hash not in self.params:
+            get_logger().debug(f"Creating new {param.name}")
             self.params[param_hash] = param
         # otherwise copy only the value
         else:
+            get_logger().debug(f"Overwriting {param.name}")
             # Try to deduce parameter type
             if param.param_type is not None:
                 # If we know the new parameter type
                 new_value = param.value
             elif self.params[param_hash].param_type is None:
                 # If we don't know the existing parameter type
                 new_value = param.value
@@ -656,16 +657,17 @@
             self.params[param_hash].value = new_value
 
     def remove_param(self, param: Parameter, safe: bool = True) -> None:
         """Remove a Parameter from the list."""
         # param: The parameter object
         # safe: don't try to remove not existing parameters
         param_hash = self.build_param_hash_from_param(param)
-        if safe and param_hash not in self.params.keys():
+        if safe and param_hash not in self.params:
             raise KeyError(f"{param.name} with cid={param.cid} is not an existing key")
+        get_logger().debug(f"Removing {param.name}.")
         self.params.pop(param_hash, None)
 
 
 # Construct parameters from structured input
 ############################################
```

### Comparing `parasect-1.1.1/src/parasect/build_lib.py` & `parasect-1.1.2/src/parasect/build_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,20 +381,22 @@
         return edited_param_list, black_param_list, black_group_list
 
     def remove_blacklist(
         self, black_param_list: ParameterList, black_group_list: ParameterList
     ) -> None:
         """Remove the blacklisted parameters from the recipe."""
         for param in self.param_list:
-            if (
-                param.group in black_group_list.keys()
-                or param.name in black_param_list.keys()
-            ):
+            if param.group and param.group in black_group_list:
                 get_logger().debug(
-                    f"Removing parameter {param} because it is blacklisted"
+                    f"Removing parameter {param} because its group is blacklisted."
+                )
+                self.param_list.remove_param(param)
+            if param in black_param_list:
+                get_logger().debug(
+                    f"Removing parameter {param} because it is blacklisted."
                 )
                 self.param_list.remove_param(param)
 
     def remove_calibration(self) -> None:
         """Remove calibration parameter from the blacklist."""
         if self.remove_calibration_flag:
             get_logger().debug(f"Removing calibration for {self.name}")
```

### Comparing `parasect-1.1.1/src/parasect/compare_lib.py` & `parasect-1.1.2/src/parasect/compare_lib.py`

 * *Files identical despite different names*

### Comparing `parasect-1.1.1/setup.py` & `parasect-1.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,173 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: parasect
+Version: 1.1.2
+Summary: Utility for manipulating parameter sets for autopilots.
+Home-page: https://github.com/AvyFly/parasect
+License: MIT
+Author: George Zogopoulos
+Author-email: geo.zogop.papal@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: click (>=8.0.1,<9.0.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
+Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Project-URL: Changelog, https://github.com/AvyFly/parasect/releases
+Project-URL: Documentation, https://parasect.readthedocs.io
+Project-URL: Repository, https://github.com/AvyFly/parasect
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+Parasect
+========
 
-packages = \
-['parasect']
+.. badges-begin
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'click>=8.0.1,<9.0.0',
- 'defusedxml>=0.7.1,<0.8.0',
- 'pydantic>=1.9.1,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['parasect = parasect.__main__:cli']}
-
-setup_kwargs = {
-    'name': 'parasect',
-    'version': '1.1.1',
-    'description': 'Utility for manipulating parameter sets for autopilots.',
-    'long_description': "Parasect\n========\n\n.. badges-begin\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/parasect.svg\n   :target: https://pypi.org/project/parasect/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/parasect.svg\n   :target: https://pypi.org/project/parasect/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/parasect\n   :target: https://pypi.org/project/parasect\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/github/license/AvyFly/parasect\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/parasect/latest.svg?label=Read%20the%20Docs\n   :target: https://parasect.readthedocs.io/\n   :alt: Read the documentation at https://parasect.readthedocs.io/\n.. |Tests| image:: https://github.com/AvyFly/parasect/workflows/Tests/badge.svg\n   :target: https://github.com/AvyFly/parasect/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/AvyFly/parasect/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/AvyFly/parasect\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. badges-end\n\n.. image:: docs/_static/logo.svg\n   :alt: parasect logo\n   :width: 320\n   :align: center\n\n.. logo-end\n\n\nWelcome to *Parasect*, a utility for manipulating parameter sets for autopilots!\n\nFeatures\n--------\n\n*Parasect* has two-fold capabilities:\n\n1. Compare two parameter sets and highlighting their differences.\n2. Parsing from user-defined content and generating new parameter sets, ready for loading into an autopilot.\n\nList of currently supported autopilots:\n\n* PX4_\n\nRequirements\n------------\n\n*Parasect* is a pure-Python project. Its requirements are managed by the Poetry_ dependency manager.\nWhen you install *Parasect* via pip_ its requirements will also be installed automatically.\n\nCurrently *Parasect* has been tested:\n\n* in Continuous Integration servers for **Ubuntu Linux**, **Windows**\n* manually in **Ubuntu Linux**.\n\n\nInstallation\n------------\n\nYou can install *Parasect* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install parasect\n\n\nUsage\n-----\n\n*Parasect* is primarily used as a command-line program.\nIn its simplest form, two parameter files can be compared via:\n\n.. code:: console\n\n   $ parasect compare <FILE_1> <FILE_2>\n\nThe usage for building parameter sets is more involved.\nPlease see the `Command-line Reference <CLI usage_>`_ for details.\n\nAdditionally, it exposes a minimal API, enabling automated operations.\nThis is described in the `API Reference <API usage_>`_.\n\nIt is strongly recommended that you read the Concepts_ that *Parasect* employs, if you plan to make full use of it.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_,\n*Parasect* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was sponsored by `Avy B.V. <Avy_>`_, a UAV company in Amsterdam.\n\nThis project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _file an issue: https://github.com/AvyFly/parasect/issues\n.. _pip: https://pip.pypa.io/\n.. _CLI usage: https://parasect.readthedocs.io/en/latest/reference.html#cli-reference\n.. _API usage: https://parasect.readthedocs.io/en/latest/reference.html#api-reference\n.. _Concepts: https://parasect.readthedocs.io/en/latest/concepts.html\n.. _PX4: https://px4.io/\n.. _Poetry: https://python-poetry.org/\n.. _Avy: https://avy.eu\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n",
-    'author': 'George Zogopoulos',
-    'author_email': 'geo.zogop.papal@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/AvyFly/parasect',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+|PyPI| |Status| |Python Version| |License|
 
+|Read the Docs| |Tests| |Codecov|
+
+|pre-commit| |Black|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/parasect.svg
+   :target: https://pypi.org/project/parasect/
+   :alt: PyPI
+.. |Status| image:: https://img.shields.io/pypi/status/parasect.svg
+   :target: https://pypi.org/project/parasect/
+   :alt: Status
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/parasect
+   :target: https://pypi.org/project/parasect
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/github/license/AvyFly/parasect
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+.. |Read the Docs| image:: https://img.shields.io/readthedocs/parasect/latest.svg?label=Read%20the%20Docs
+   :target: https://parasect.readthedocs.io/
+   :alt: Read the documentation at https://parasect.readthedocs.io/
+.. |Tests| image:: https://github.com/AvyFly/parasect/workflows/Tests/badge.svg
+   :target: https://github.com/AvyFly/parasect/actions?workflow=Tests
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/AvyFly/parasect/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/AvyFly/parasect
+   :alt: Codecov
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Black
+
+.. badges-end
+
+.. image:: docs/_static/logo.svg
+   :alt: parasect logo
+   :width: 320
+   :align: center
+
+.. logo-end
+
+
+Welcome to *Parasect*, a utility for manipulating parameter sets for autopilots!
+
+Features
+--------
+
+*Parasect* has two-fold capabilities:
+
+1. Compare two parameter sets and highlighting their differences.
+2. Parsing from user-defined content and generating new parameter sets, ready for loading into an autopilot.
+
+List of currently supported autopilots:
+
+* PX4_
+
+Requirements
+------------
+
+*Parasect* is a pure-Python project. Its requirements are managed by the Poetry_ dependency manager.
+When you install *Parasect* via pip_ its requirements will also be installed automatically.
+
+Currently *Parasect* has been tested:
+
+* in Continuous Integration servers for **Ubuntu Linux**, **Windows**
+* manually in **Ubuntu Linux**.
+
+
+Installation
+------------
+
+You can install *Parasect* via pip_ from PyPI_:
+
+.. code:: console
+
+   $ pip install parasect
+
+
+Usage
+-----
+
+*Parasect* is primarily used as a command-line program.
+In its simplest form, two parameter files can be compared via:
+
+.. code:: console
+
+   $ parasect compare <FILE_1> <FILE_2>
+
+The usage for building parameter sets is more involved.
+Please see the `Command-line Reference <CLI usage_>`_ for details.
+
+Additionally, it exposes a minimal API, enabling automated operations.
+This is described in the `API Reference <API usage_>`_.
+
+It is strongly recommended that you read the Concepts_ that *Parasect* employs, if you plan to make full use of it.
+
+
+Contributing
+------------
+
+Contributions are very welcome.
+To learn more, see the `Contributor Guide`_.
+
+
+License
+-------
+
+Distributed under the terms of the `MIT license`_,
+*Parasect* is free and open source software.
+
+
+Issues
+------
+
+If you encounter any problems,
+please `file an issue`_ along with a detailed description.
+
+
+Credits
+-------
+
+This project was sponsored by `Avy B.V. <Avy_>`_, a UAV company in Amsterdam.
+
+This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
+
+.. _@cjolowicz: https://github.com/cjolowicz
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _MIT license: https://opensource.org/licenses/MIT
+.. _PyPI: https://pypi.org/
+.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+.. _file an issue: https://github.com/AvyFly/parasect/issues
+.. _pip: https://pip.pypa.io/
+.. _CLI usage: https://parasect.readthedocs.io/en/latest/reference.html#cli-reference
+.. _API usage: https://parasect.readthedocs.io/en/latest/reference.html#api-reference
+.. _Concepts: https://parasect.readthedocs.io/en/latest/concepts.html
+.. _PX4: https://px4.io/
+.. _Poetry: https://python-poetry.org/
+.. _Avy: https://avy.eu
+.. github-only
+.. _Contributor Guide: CONTRIBUTING.rst
 
-setup(**setup_kwargs)
```

