# Comparing `tmp/gitig-22.4.0.tar.gz` & `tmp/gitig-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitig-22.4.0.tar", max compression
+gzip compressed data, was "gitig-23.4.0.tar", max compression
```

## Comparing `gitig-22.4.0.tar` & `gitig-23.4.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1068 2022-04-10 06:47:08.275856 gitig-22.4.0/LICENSE
--rw-r--r--   0        0        0     4091 2022-04-10 06:47:08.275856 gitig-22.4.0/README.md
--rw-r--r--   0        0        0     1151 2022-04-10 06:47:08.275856 gitig-22.4.0/pyproject.toml
--rw-r--r--   0        0        0     6350 2022-04-10 06:47:08.275856 gitig-22.4.0/src/gitig.py
--rw-r--r--   0        0        0     4914 2022-04-10 06:47:23.420874 gitig-22.4.0/setup.py
--rw-r--r--   0        0        0     5221 2022-04-10 06:47:23.421208 gitig-22.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-26 08:06:41.406809 gitig-23.4.0/LICENSE
+-rw-r--r--   0        0        0     4832 2023-04-26 08:06:41.406809 gitig-23.4.0/README.md
+-rw-r--r--   0        0        0     1152 2023-04-26 08:06:41.406809 gitig-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6350 2023-04-26 08:06:41.406809 gitig-23.4.0/src/gitig.py
+-rw-r--r--   0        0        0     5917 1970-01-01 00:00:00.000000 gitig-23.4.0/PKG-INFO
```

### Comparing `gitig-22.4.0/LICENSE` & `gitig-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitig-22.4.0/README.md` & `gitig-23.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # gitig
 
 Generate `.gitignore` files from the command-line
 
-[![PyPI Version](https://img.shields.io/pypi/v/gitig.svg)](https://pypi.org/project/gitig/)
+[![PyPI](https://img.shields.io/pypi/v/gitig)](https://pypi.org/project/gitig/) [![Crates.io](https://img.shields.io/crates/v/gitig-rs)](https://crates.io/crates/gitig-rs)
 
 `gitig` writes its output to stdout. Redirect the results to wherever makes sense for you, for example:
 
 ```bash
 gi python > .gitignore
 ```
 
 ## Installation
 
+### With `cargo`
+
+`gitig` has an implementation in Rust (and an implementation in Python) and can be installed via `cargo`:
+
+```bash
+cargo install gitig-rs
+```
+
 ### With `pipx`
 
-`gitig` is intended to be used as an **end-user command-line application** (i.e. not as a package's dependecy). The easiest way to get started is with `pipx`:
+`gitig` is intended to be used as an **end-user command-line application** (i.e. not as a package's dependency). The easiest way to get started is with `pipx`:
 
 ```bash
 pipx install gitig
 ```
 
 ### With `pip`
 
@@ -131,28 +139,49 @@
 $ gi python j<TAB><TAB>
 jabref  jboss6          jekyll         jetbrains+iml  joe     jupyternotebooks
 java    jboss-4-2-3-ga  jenv           jgiven         joomla  justcode
 jboss   jboss-6-x       jetbrains      jigsaw         jspm
 jboss4  jdeveloper      jetbrains+all  jmeter         julia
 ```
 
+### Rust API
+
+```rust
+gitig::list_templates();  // same as `gi`
+gitig::create(vec!['python', 'jupyter']);  // same as `gi python jupyter`
+gitig::bash_completion();  // same as `gi --completion bash`
+gitig::fish_completion();  // same as `gi --completion fish`
+gitig::VERSION;
+```
+
 ### Python API
 
 ```python
 import gitig
 
-gitig.list()  # same as `gi`
+gitig.list_templates()  # same as `gi`
 gitig.create(['python', 'jupyter'])  # same as `gi python jupyter`
 gitig.bash_completion()  # same as `gi --completion bash`
 gitig.fish_completion()  # same as `gi --completion fish`
 gitig.__version__
 ```
 
 ## Contributing
 
+### Rust
+
+1. Fork the repo
+1. Run `cargo build`
+1. Run `pre-commit install`
+1. Add your changes (adding/updating tests is always nice too)
+1. Commit your changes + push to your fork
+1. Open a PR
+
+### Python
+
 1. Have or install a recent version of `poetry` (version >= 1.1)
 1. Fork the repo
 1. Setup a virtual environment (however you prefer)
 1. Run `poetry install`
 1. Run `pre-commit install`
 1. Add your changes (adding/updating tests is always nice too)
 1. Commit your changes + push to your fork
```

### Comparing `gitig-22.4.0/pyproject.toml` & `gitig-23.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitig"
-version = "22.4.0"
+version = "23.4.0"
 description = "Generate .gitignore files from the command-line"
 authors = ["Andrew Ross <andrew.ross.mail@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 
 keywords = ["cli", "git", "gitignore", "config"]
@@ -22,23 +22,23 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
-flake8 = "^4.0.1"
-pylint = "^2.13.4"
-reorder-python-imports = "^3.0.1"
+black = "^23.3.0"
+flake8 = "^6.0.0"
+pylint = "^2.17.2"
+reorder-python-imports = "^3.9.0"
 bump2version = "^1.0.1"
-pre-commit = "^2.18.1"
+pre-commit = "^3.2.2"
 
 [tool.poetry.scripts]
 gi = 'gitig:cli'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gitig-22.4.0/src/gitig.py` & `gitig-23.4.0/src/gitig.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Sequence
 from urllib.error import HTTPError
 from urllib.parse import urljoin
 from urllib.request import Request
 from urllib.request import urlopen
 
 
-__version__ = "22.4.0"
+__version__ = "23.4.0"
 
 REQUEST_TIMEOUT = 10  # seconds
 
 
 class Defaults:
     completion_shells = ("bash", "fish")
     api_url = "https://www.toptal.com/developers/gitignore/api"
```

### Comparing `gitig-22.4.0/PKG-INFO` & `gitig-23.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 Metadata-Version: 2.1
 Name: gitig
-Version: 22.4.0
+Version: 23.4.0
 Summary: Generate .gitignore files from the command-line
 Home-page: https://github.com/andrewrosss/gitig
 License: MIT
 Keywords: cli,git,gitignore,config
 Author: Andrew Ross
 Author-email: andrew.ross.mail@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.0
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Project-URL: Documentation, https://github.com/andrewrosss/gitig
 Project-URL: Repository, https://github.com/andrewrosss/gitig
 Description-Content-Type: text/markdown
 
 # gitig
 
 Generate `.gitignore` files from the command-line
 
-[![PyPI Version](https://img.shields.io/pypi/v/gitig.svg)](https://pypi.org/project/gitig/)
+[![PyPI](https://img.shields.io/pypi/v/gitig)](https://pypi.org/project/gitig/) [![Crates.io](https://img.shields.io/crates/v/gitig-rs)](https://crates.io/crates/gitig-rs)
 
 `gitig` writes its output to stdout. Redirect the results to wherever makes sense for you, for example:
 
 ```bash
 gi python > .gitignore
 ```
 
 ## Installation
 
+### With `cargo`
+
+`gitig` has an implementation in Rust (and an implementation in Python) and can be installed via `cargo`:
+
+```bash
+cargo install gitig-rs
+```
+
 ### With `pipx`
 
-`gitig` is intended to be used as an **end-user command-line application** (i.e. not as a package's dependecy). The easiest way to get started is with `pipx`:
+`gitig` is intended to be used as an **end-user command-line application** (i.e. not as a package's dependency). The easiest way to get started is with `pipx`:
 
 ```bash
 pipx install gitig
 ```
 
 ### With `pip`
 
@@ -159,28 +166,49 @@
 $ gi python j<TAB><TAB>
 jabref  jboss6          jekyll         jetbrains+iml  joe     jupyternotebooks
 java    jboss-4-2-3-ga  jenv           jgiven         joomla  justcode
 jboss   jboss-6-x       jetbrains      jigsaw         jspm
 jboss4  jdeveloper      jetbrains+all  jmeter         julia
 ```
 
+### Rust API
+
+```rust
+gitig::list_templates();  // same as `gi`
+gitig::create(vec!['python', 'jupyter']);  // same as `gi python jupyter`
+gitig::bash_completion();  // same as `gi --completion bash`
+gitig::fish_completion();  // same as `gi --completion fish`
+gitig::VERSION;
+```
+
 ### Python API
 
 ```python
 import gitig
 
-gitig.list()  # same as `gi`
+gitig.list_templates()  # same as `gi`
 gitig.create(['python', 'jupyter'])  # same as `gi python jupyter`
 gitig.bash_completion()  # same as `gi --completion bash`
 gitig.fish_completion()  # same as `gi --completion fish`
 gitig.__version__
 ```
 
 ## Contributing
 
+### Rust
+
+1. Fork the repo
+1. Run `cargo build`
+1. Run `pre-commit install`
+1. Add your changes (adding/updating tests is always nice too)
+1. Commit your changes + push to your fork
+1. Open a PR
+
+### Python
+
 1. Have or install a recent version of `poetry` (version >= 1.1)
 1. Fork the repo
 1. Setup a virtual environment (however you prefer)
 1. Run `poetry install`
 1. Run `pre-commit install`
 1. Add your changes (adding/updating tests is always nice too)
 1. Commit your changes + push to your fork
```

