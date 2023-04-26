# Comparing `tmp/nuke-2.5.3.tar.gz` & `tmp/nuke-2.5.4.tar.gz`

## Comparing `nuke-2.5.3.tar` & `nuke-2.5.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 nuke-2.5.3/.DS_Store
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nuke-2.5.3/.travis.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 nuke-2.5.3/DEV.md
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 nuke-2.5.3/HISTORY.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 nuke-2.5.3/Makefile
--rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 nuke-2.5.3/poetry.lock
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 nuke-2.5.3/setup.cfg
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nuke-2.5.3/setup.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nuke-2.5.3/tox.ini
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 nuke-2.5.3/.vscode/settings.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/__init__.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/dirtree.py
--rwxr-xr-x   0        0        0     5310 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/nuke.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuke-2.5.3/tests/__init__.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 nuke-2.5.3/tests/test_nuke.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 nuke-2.5.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nuke-2.5.3/LICENSE
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 nuke-2.5.3/README.md
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nuke-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 nuke-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nuke-2.5.4/.travis.yml
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nuke-2.5.4/DEV.md
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 nuke-2.5.4/HISTORY.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 nuke-2.5.4/Makefile
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 nuke-2.5.4/poetry.lock
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 nuke-2.5.4/setup.cfg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 nuke-2.5.4/tox.ini
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 nuke-2.5.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 nuke-2.5.4/.vscode/settings.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nuke-2.5.4/nuke/__init__.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 nuke-2.5.4/nuke/dirtree.py
+-rwxr-xr-x   0        0        0     5310 2020-02-02 00:00:00.000000 nuke-2.5.4/nuke/nuke.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 nuke-2.5.4/nuke/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuke-2.5.4/tests/__init__.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 nuke-2.5.4/tests/test_nuke.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nuke-2.5.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nuke-2.5.4/LICENSE
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 nuke-2.5.4/README.md
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 nuke-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 nuke-2.5.4/PKG-INFO
```

### Comparing `nuke-2.5.3/DEV.md` & `nuke-2.5.4/DEV.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 - tox
 
 ## Running Tests
 
 `tox` is currently set up to read the tests from the `tests` directory and as such, one only needs to run the `tox` command.
 
 ```shell
-# runs all the tests against Python 3.6, 3.7 & 3.8
+# runs all the tests against Python 3.7, 3.8, 3.9, 3.10 & 3.11
 tox
 
-# test only against Python 3.6
-tox -e 36
+# test only against Python 3.7
+tox -e 37
 ```
 
 ## Makefile
 
 There is also a `Makefile` set up to ease various repetitive tasks.
 
 - Default: The default `make` command runs the `tox` tests.
```

### Comparing `nuke-2.5.3/HISTORY.md` & `nuke-2.5.4/HISTORY.md`

 * *Files identical despite different names*

### Comparing `nuke-2.5.3/poetry.lock` & `nuke-2.5.4/poetry.lock`

 * *Files identical despite different names*

### Comparing `nuke-2.5.3/setup.py` & `nuke-2.5.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-"""
-Command line tool for nuking a directory..
-"""
-from os import path
-
-from setuptools import find_packages, setup
-
-import nuke
-
-dependencies = ["click>=6.7", "crayons>=0.1.2", "rich>=12.6.0"]
-
-here = path.abspath(path.dirname(__file__))
-
-setup(
-    name='nuke',
-    version=nuke.__version__,
-    url='https://github.com/varunagrawal/nuke',
-    license=nuke.__license__,
-    author=nuke.__author__,
-    author_email=nuke.__email__,
-    description='Command line tool for nuking a directory 💥',
-    long_description=open("README.md", 'r').read(),
-    long_description_content_type="text/markdown",
-    packages=find_packages(exclude=['tests']),
-    include_package_data=True,
-    zip_safe=False,
-    platforms='any',
-    install_requires=dependencies,
-    entry_points={
-        'console_scripts': [
-            'nuke = nuke.nuke:main',
-        ],
-    },
-    classifiers=[
-        # As from http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        # 'Development Status :: 1 - Planning',
-        # 'Development Status :: 2 - Pre-Alpha',
-        # 'Development Status :: 3 - Alpha',
-        # 'Development Status :: 4 - Beta',
-        'Development Status :: 5 - Production/Stable',
-        # 'Development Status :: 6 - Mature',
-        # 'Development Status :: 7 - Inactive',
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: POSIX',
-        'Operating System :: MacOS',
-        'Operating System :: Unix',
-        'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ])
+[project]
+name = "nuke"
+version = "2.5.4"
+authors = [
+  { name="Varun Agrawal", email="varagrawal@gmail.com" },
+]
+description = "Command line tool for nuking a directory 💥"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: BSD License",
+    "Operating System :: POSIX",
+    "Operating System :: MacOS",
+    "Operating System :: Unix",
+    "Operating System :: Microsoft :: Windows",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+dependencies = [
+  "click >= 6.7",
+  "crayons >= 0.1.2",
+  "rich ~= 12.6.0"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/varunagrawal/nuke"
+"Bug Tracker" = "https://github.com/varunagrawal/nuke/issues"
+
+[project.scripts]
+nuke = "nuke.nuke:main"
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.poetry]
+name = "nuke"
+version = "2.5.4"
+description = "Command line tool for nuking a directory 💥"
+authors = ["Varun Agrawal <varagrawal@gmail.com>"]
+license = "MIT"
+
+[tool.poetry.dependencies]
+python = ">=3.7,<4.0.0"
+click = ">=6.7"
+crayons = ">=0.1.2"
+rich = "^12.6.0"
+
+[tool.poetry.dev-dependencies]
+tox = "^3.27.0"
+pypandoc = ">=1.4"
```

### Comparing `nuke-2.5.3/nuke/dirtree.py` & `nuke-2.5.4/nuke/dirtree.py`

 * *Files identical despite different names*

### Comparing `nuke-2.5.3/nuke/nuke.py` & `nuke-2.5.4/nuke/nuke.py`

 * *Files identical despite different names*

### Comparing `nuke-2.5.3/nuke/utils.py` & `nuke-2.5.4/nuke/utils.py`

 * *Files identical despite different names*

### Comparing `nuke-2.5.3/tests/test_nuke.py` & `nuke-2.5.4/tests/test_nuke.py`

 * *Files identical despite different names*

### Comparing `nuke-2.5.3/.gitignore` & `nuke-2.5.4/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -97,8 +97,10 @@
 # Rope project settings
 .ropeproject
 
 # End of https://www.gitignore.io/api/python
 
 .idea
 
-.pytest_cache
+.pytest_cache
+
+.DS_Store
```

### Comparing `nuke-2.5.3/LICENSE` & `nuke-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nuke-2.5.3/README.md` & `nuke-2.5.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Nuke
 
 
 [![version](https://img.shields.io/pypi/v/nuke.svg)](https://pypi.python.org/pypi/nuke)
 [![license](https://img.shields.io/pypi/l/nuke.svg)](https://pypi.python.org/pypi/nuke)
 [![wheel](https://img.shields.io/pypi/wheel/nuke.svg)](https://pypi.python.org/pypi/nuke)
 [![python](https://img.shields.io/pypi/pyversions/nuke.svg)](https://pypi.python.org/pypi/nuke)
-[![Build Status](https://travis-ci.org/varunagrawal/nuke.svg?branch=master)](https://travis-ci.org/varunagrawal/nuke)
+[![CI](https://github.com/varunagrawal/nuke/actions/workflows/ci.yml/badge.svg)](https://github.com/varunagrawal/nuke/actions/workflows/ci.yml)
+
 [![say-thanks](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/varunagrawal)
 
 Command line tool for nuking a directory 💥.
 
 ## Installation
 
 Installing `nuke` is intended to be super easy. The only dependency is a supported Python interpreter. You can get `nuke` via `pip`:
 
 ```shell
 $ pip install nuke
 ```
-`nuke` is supported for Python 3.6+.
+`nuke` is supported for Python 3.7+.
 
 
 ## Usage
 
 The most common usage of `nuke` is when you wish to recreate a build directory for a build program such as CMake.
 
 To use `nuke`, you just call `nuke` from the command line and specify the directory you wish to nuke:
```

### Comparing `nuke-2.5.3/PKG-INFO` & `nuke-2.5.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 Metadata-Version: 2.1
 Name: nuke
-Version: 2.5.3
+Version: 2.5.4
 Summary: Command line tool for nuking a directory 💥
 Project-URL: Homepage, https://github.com/varunagrawal/nuke
 Project-URL: Bug Tracker, https://github.com/varunagrawal/nuke/issues
 Author-email: Varun Agrawal <varagrawal@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+Requires-Dist: click>=6.7
+Requires-Dist: crayons>=0.1.2
+Requires-Dist: rich~=12.6.0
 Description-Content-Type: text/markdown
 
 # Nuke
 
 
 [![version](https://img.shields.io/pypi/v/nuke.svg)](https://pypi.python.org/pypi/nuke)
 [![license](https://img.shields.io/pypi/l/nuke.svg)](https://pypi.python.org/pypi/nuke)
 [![wheel](https://img.shields.io/pypi/wheel/nuke.svg)](https://pypi.python.org/pypi/nuke)
 [![python](https://img.shields.io/pypi/pyversions/nuke.svg)](https://pypi.python.org/pypi/nuke)
-[![Build Status](https://travis-ci.org/varunagrawal/nuke.svg?branch=master)](https://travis-ci.org/varunagrawal/nuke)
+[![CI](https://github.com/varunagrawal/nuke/actions/workflows/ci.yml/badge.svg)](https://github.com/varunagrawal/nuke/actions/workflows/ci.yml)
+
 [![say-thanks](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/varunagrawal)
 
 Command line tool for nuking a directory 💥.
 
 ## Installation
 
 Installing `nuke` is intended to be super easy. The only dependency is a supported Python interpreter. You can get `nuke` via `pip`:
 
 ```shell
 $ pip install nuke
 ```
-`nuke` is supported for Python 3.6+.
+`nuke` is supported for Python 3.7+.
 
 
 ## Usage
 
 The most common usage of `nuke` is when you wish to recreate a build directory for a build program such as CMake.
 
 To use `nuke`, you just call `nuke` from the command line and specify the directory you wish to nuke:
```

