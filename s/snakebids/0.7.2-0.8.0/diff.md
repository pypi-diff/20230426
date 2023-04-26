# Comparing `tmp/snakebids-0.7.2.tar.gz` & `tmp/snakebids-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakebids-0.7.2.tar", max compression
+gzip compressed data, was "snakebids-0.8.0.tar", max compression
```

## Comparing `snakebids-0.7.2.tar` & `snakebids-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0     1065 2023-02-06 22:13:42.824857 snakebids-0.7.2/LICENSE
--rw-r--r--   0        0        0     2305 2023-02-06 22:13:42.824857 snakebids-0.7.2/README.md
--rw-r--r--   0        0        0     2691 2023-02-06 22:14:12.244859 snakebids-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      564 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/__init__.py
--rw-r--r--   0        0        0     1817 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/admin.py
--rw-r--r--   0        0        0     9242 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/app.py
--rw-r--r--   0        0        0    10330 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/cli.py
--rw-r--r--   0        0        0      757 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/core/__init__.py
--rw-r--r--   0        0        0     7537 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/core/construct_bids.py
--rw-r--r--   0        0        0    10986 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/core/datasets.py
--rw-r--r--   0        0        0     9010 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/core/filtering.py
--rw-r--r--   0        0        0    24132 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/core/input_generation.py
--rw-r--r--   0        0        0      413 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/exceptions.py
--rw-r--r--   0        0        0      318 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/cookiecutter.json
--rw-r--r--   0        0        0       73 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/README.rst
--rw-r--r--   0        0        0     3253 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml
--rw-r--r--   0        0        0        7 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/.gitignore
--rw-r--r--   0        0        0      634 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile
--rw-r--r--   0        0        0     2002 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py
--rw-r--r--   0        0        0     3317 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst
--rw-r--r--   0        0        0      548 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst
--rw-r--r--   0        0        0       93 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/requirements.txt
--rw-r--r--   0        0        0      168 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/app_cli.rst
--rw-r--r--   0        0        0      155 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/snakemake_cli.rst
--rw-r--r--   0        0        0      814 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/pipeline_description.json
--rw-r--r--   0        0        0     1204 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/setup.py
--rw-r--r--   0        0        0     1732 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/workflow/Snakefile
--rw-r--r--   0        0        0      399 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}/run.py
--rw-r--r--   0        0        0       28 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/resources/__init__.py
--rw-r--r--   0        0        0     4237 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/resources/bids_tags.json
--rw-r--r--   0        0        0      333 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/types.py
--rw-r--r--   0        0        0       70 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/utils/__init__.py
--rw-r--r--   0        0        0     5613 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/utils/output.py
--rw-r--r--   0        0        0      821 2023-02-06 22:13:42.828857 snakebids-0.7.2/snakebids/utils/sb_itertools.py
--rw-r--r--   0        0        0      115 2023-02-06 22:13:42.832857 snakebids-0.7.2/snakebids/utils/sb_typing.py
--rw-r--r--   0        0        0      234 2023-02-06 22:13:42.832857 snakebids-0.7.2/snakebids/utils/sb_typing.pyi
--rw-r--r--   0        0        0     5032 2023-02-06 22:13:42.832857 snakebids-0.7.2/snakebids/utils/snakemake_io.py
--rw-r--r--   0        0        0     7148 2023-02-06 22:13:42.832857 snakebids-0.7.2/snakebids/utils/utils.py
--rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 snakebids-0.7.2/setup.py
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 snakebids-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-26 15:01:52.399305 snakebids-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2305 2023-04-26 15:01:52.399305 snakebids-0.8.0/README.md
+-rw-r--r--   0        0        0     2906 2023-04-26 15:02:22.455957 snakebids-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      654 2023-04-26 15:02:22.459957 snakebids-0.8.0/snakebids/__init__.py
+-rw-r--r--   0        0        0     2007 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/admin.py
+-rw-r--r--   0        0        0    10207 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/app.py
+-rw-r--r--   0        0        0    10775 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/cli.py
+-rw-r--r--   0        0        0      742 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/core/__init__.py
+-rw-r--r--   0        0        0     8118 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/construct_bids.py
+-rw-r--r--   0        0        0    18389 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/datasets.py
+-rw-r--r--   0        0        0     9128 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/filtering.py
+-rw-r--r--   0        0        0    24692 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/input_generation.py
+-rw-r--r--   0        0        0      519 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/exceptions.py
+-rw-r--r--   0        0        0     4219 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/io/console.py
+-rw-r--r--   0        0        0     3271 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/io/printing.py
+-rw-r--r--   0        0        0      317 2023-04-26 15:02:22.459957 snakebids-0.8.0/snakebids/project_template/cookiecutter.json
+-rw-r--r--   0        0        0       73 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/README.rst
+-rw-r--r--   0        0        0     3253 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml
+-rw-r--r--   0        0        0        7 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/.gitignore
+-rw-r--r--   0        0        0      634 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile
+-rw-r--r--   0        0        0     1978 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py
+-rw-r--r--   0        0        0     3317 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst
+-rw-r--r--   0        0        0      548 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst
+-rw-r--r--   0        0        0       93 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/requirements.txt
+-rw-r--r--   0        0        0      168 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/app_cli.rst
+-rw-r--r--   0        0        0      155 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/snakemake_cli.rst
+-rw-r--r--   0        0        0      570 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/pipeline_description.json
+-rw-r--r--   0        0        0     1194 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/setup.py
+-rw-r--r--   0        0        0     1592 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/workflow/Snakefile
+-rw-r--r--   0        0        0      399 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}/run.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/py.typed
+-rw-r--r--   0        0        0       13 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/resources/__init__.py
+-rw-r--r--   0        0        0     4216 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/resources/bids_tags.json
+-rw-r--r--   0        0        0     3489 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/types.py
+-rw-r--r--   0        0        0       70 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/__init__.py
+-rw-r--r--   0        0        0     5839 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/output.py
+-rw-r--r--   0        0        0      990 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/sb_itertools.py
+-rw-r--r--   0        0        0     4947 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/snakemake_io.py
+-rw-r--r--   0        0        0       91 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/user_property.py
+-rw-r--r--   0        0        0      242 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/user_property.pyi
+-rw-r--r--   0        0        0    10690 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/utils.py
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 snakebids-0.8.0/PKG-INFO
```

### Comparing `snakebids-0.7.2/LICENSE` & `snakebids-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakebids-0.7.2/README.md` & `snakebids-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `snakebids-0.7.2/pyproject.toml` & `snakebids-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 [tool.poetry]
 name = "snakebids"
-version = "0.7.2"
+version = "0.8.0"
 description = "BIDS integration into snakemake workflows"
 readme = "README.md"
 repository = "https://github.com/akhanf/snakebids"
 documentation = "https://snakebids.readthedocs.io/"
-authors = ["Ali Khan <alik@robarts.ca>"]
+authors = [
+    "Ali Khan <alik@robarts.ca>",
+    "Peter Van Dyken <pvandyk2@uwo.ca>",
+    "Tristan Kuehn <tkuehn@uwo.ca>",
+    "Jason Kai <tkai@uwo.ca>",
+]
 license = "MIT"
 packages = [
     { include = "snakebids" }
 ]
 exclude = ["snakebids/tests/**"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 dirty = true
 style = "pep440"
 bump = true
 
 [tool.poetry-dynamic-versioning.substitution]
-files = ['snakebids/project_template/cookiecutter.json']
-patterns = ["(^\\s+\"snakebids_version\":\\s*\")[^'\"](\")"]
+files = ['snakebids/project_template/cookiecutter.json', 'snakebids/__init__.py']
+patterns = ["(^\\s+\"snakebids_version\":\\s*\")[^'\"]*(\")", "(^__version__\\s*(?::.*?)?=\\s*['\"])[^'\"]*(['\"])"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 pybids = "^0.15.0"
 snakemake = [
     { version = ">=5.28.0", python = ">=3.7" },
     { version = ">=7.18.2", python = ">=3.11" },
@@ -33,14 +38,15 @@
 PyYAML = "^6"
 cookiecutter = "^2.1.1"
 typing-extensions = ">=3.10.0"
 attrs = ">=21.2.0,<23"
 boutiques = "^0.5.25"
 more-itertools = ">=8,<10"
 cached-property = "^1.5.2"
+pvandyken-deprecated = "0.0.3"
 
 #  Below are non-direct dependencies (i.e. dependencies of other depenencies)
 #  specified to ensure a version with a pre-built wheel is installed depending
 #  on the python version being used.
 pandas = [
     { version = ">=1.3", python = ">=3.7.1" },
     { version = ">=1.5", python = ">=3.11" }
@@ -51,52 +57,50 @@
 ]
 scipy = [
     { version = "<1.8", python = "3.7"},
     { version = ">=1.9.2", python = ">=3.11" }
 ]
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.1.0"
+black = "^23.1.0"
 pybids = "^0.15.2"
 pytest = "^7.0.0"
 pytest-mock = "^3.7.0"
-pylint = "^2.12.0"
 isort = "^5.10.1"
-flake8 = "^5.0.4"
-poethepoet = "^0.16.2"
+poethepoet = "^0.18.1"
+# pre-commit==3.0.0 requires py38 or greater
 pre-commit = "^2.17.0"
-mkinit = "^0.3.3"
+mkinit = "^1.0.0"
 hypothesis = "^6.34.1"
 pytest-benchmark = "^4.0.0"
-pyfakefs = "^4.6.1"
+pyfakefs = "^5.1.0"
+pyparsing = "^3.0.9"
+pyright = "^1.1.302"
+ruff = "^0.0.261"
 
 [tool.poetry.scripts]
 snakebids = "snakebids.admin:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poe.tasks]
 setup = "pre-commit install"
-quality = { shell = "isort snakebids && black snakebids && flake8 snakebids && pylint snakebids" }
+quality = { shell = "isort snakebids && black snakebids && ruff snakebids" }
 test = "pytest --doctest-modules --ignore=docs --ignore=snakebids/project_template --benchmark-disable"
 mkinit = "mkinit --recursive --nomods --black -i snakebids"
 benchmark = "pytest --benchmark-only --benchmark-autosave"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
-[tool.pylint.master]
-ignore-patterns = "^[0-9][0-9]+_,^test_,^__init__,"
-ignore-paths = ["typings"]
-
-[tool.pylint.format]
-good-names = "i,j,k,ex,_,x,y,f,d"
-
-[tool.pylint.messages_control]
-disable = """
-    missing-function-docstring,
-    missing-module-docstring,
-    fixme
-"""
+[tool.pyright]
+include = ["snakebids"]
+exclude = ["snakebids/project_template", "typings"]
+typeCheckingMode = "strict"
+reportPrivateUsage = false
+reportImportCycles = false
+
+[tool.ruff]
+select = ["E", "F", "PL", "RUF"]
```

### Comparing `snakebids-0.7.2/snakebids/__init__.py` & `snakebids-0.8.0/snakebids/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+"""Top-level namespace containing the core classes and functions"""
 __submodules__ = ["core"]
 
+__version__ = "0.8.0"
 
 # <AUTOGEN_INIT>
 from snakebids.core import (
     BidsComponent,
     BidsDataset,
     BidsDatasetDict,
     bids,
```

### Comparing `snakebids-0.7.2/snakebids/admin.py` & `snakebids-0.8.0/snakebids/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Script to generate a Snakebids project."""
 
 import argparse
 from pathlib import Path
 
-from cookiecutter.main import cookiecutter
+from cookiecutter.main import cookiecutter  # type: ignore
 
 import snakebids
 from snakebids.app import SnakeBidsApp
 from snakebids.cli import add_dynamic_args
 
 
-def create_app(args):
+def create_app(args: argparse.Namespace) -> None:
     cookiecutter(
-        str(Path(snakebids.__path__[0]) / "project_template"),
+        str(Path(list(snakebids.__path__)[0]) / "project_template"),
         output_dir=args.output_dir,
+        extra_context={"_output_dir": Path(args.output_dir).resolve().name},
     )
 
 
-def create_descriptor(args):
+def create_descriptor(args: argparse.Namespace) -> None:
     # pylint: disable=unsubscriptable-object
     app = SnakeBidsApp(args.app_dir.resolve())
     add_dynamic_args(app.parser, app.config["parse_args"], app.config["pybids_inputs"])
     app.create_descriptor(args.out_path)
     print(f"Boutiques descriptor created at {args.out_path}")
 
 
-def gen_parser():
+def gen_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description="Perform administrative Snakebids tasks."
     )
     subparsers = parser.add_subparsers(required=True, dest="command")
 
     parser_create = subparsers.add_parser("create", help="Create a new Snakebids app.")
     parser_create.add_argument("output_dir", nargs="?", default=".")
@@ -50,13 +51,13 @@
         default=".",
     )
     parser_boutiques.set_defaults(func=create_descriptor)
 
     return parser
 
 
-def main():
+def main() -> None:
     """Invoke Cookiecutter on the Snakebids project template."""
 
     parser = gen_parser()
     args = parser.parse_args()
     args.func(args)
```

### Comparing `snakebids-0.7.2/snakebids/app.py` & `snakebids-0.8.0/snakebids/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """Tools to generate a Snakemake-based BIDS app."""
+from __future__ import annotations
 
 import argparse
 import logging
 import sys
+from os import PathLike
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Any, Callable, Optional
 
 import attr
-import boutiques.creator as bc
+import boutiques.creator as bc  # type: ignore
 import snakemake
 from snakemake.io import load_configfile
 
 from snakebids.cli import (
     SnakebidsArgs,
     add_dynamic_args,
     create_parser,
     parse_snakebids_args,
 )
 from snakebids.exceptions import ConfigError, RunError
-from snakebids.utils.output import (
-    prepare_bidsapp_output,
-    write_config_file,
-    write_output_mode,
-)
+from snakebids.utils.output import write_config_file  # type: ignore
+from snakebids.utils.output import prepare_bidsapp_output, write_output_mode
 
 logger = logging.Logger(__name__)
 
 
 SNAKEFILE_CHOICES = [
     "Snakefile",
     "snakefile",
@@ -47,15 +46,17 @@
     "config.json",
     "config/config.json",
     "config/config.yml",
     "config/config.yaml",
 ]
 
 
-def _get_file_paths(choices: List[str], file_name: str):
+def _get_file_paths(
+    choices: list[str], file_name: str
+) -> Callable[[SnakeBidsApp], Path]:
     def wrapper(self: "SnakeBidsApp"):
         for path in choices:
             if (self.snakemake_dir / path).exists():
                 if file_name == "config":
                     return Path(path)
                 # else, snakefile
                 return Path(self.snakemake_dir, path)
@@ -63,65 +64,78 @@
         raise ConfigError(
             f"Error: no {file_name} file found, tried {', '.join(choices)}."
         )
 
     return wrapper
 
 
-# pylint: disable=unsubscriptable-object, unsupported-assignment-operation,
-# pylint: disable=too-few-public-methods
 @attr.define(slots=False)
 class SnakeBidsApp:
     """Snakebids app with config and arguments.
 
-    Attributes
+    Parameters
     ----------
-    snakemake_dir : str
+    snakemake_dir : str | Path
         Root directory of the snakebids app, containing the config file and workflow
         files.
-    parser : ArgumentParser, optional
+    parser
         Parser including only the arguments specific to this Snakebids app, as specified
         in the config file. By default, it will use `create_parser()` from `cli.py`
-    configfile_path : str, optional
+    configfile_path
         Relative path to config file (relative to snakemake_dir). By default,
         autocalculates based on snamake_dir
-    snakefile_path : str, optional
+    snakefile_path
         Absolute path to the input Snakefile. By default, autocalculates based on
         snakemake_dir::
 
             join(snakemake_dir, snakefile_path)
-    config : dict, optional
+    config
         Contains all the configuration variables parsed from the config file
         and generated during the initialization of the SnakeBidsApp.
-    args : SnakebidsArgs, optional
+    args
         Arguments to use when running the app. By default, generated using the parser
         attribute, autopopulated with args from `config.py`
+    plugins
+        List of methods to be called after CLI parsing.
+
+        Each callable in ``plugins`` should take, as a single argument, a reference to
+        the ``SnakeBidsApp``. Plugins may perform any arbitrary side effects, including
+        updates to the config dictionary, validation of inputs, optimization, or other
+        enhancements to the snakebids app.
+
+        CLI parameters may be read from ``SnakeBidsApp.config``. Plugins are responsible
+        for documenting what properties they expect to find in the config.
+
+        Every plugin should return either:
+
+        - Nothing, in which case any changes to the SnakeBidsApp will persist in the
+          workflow.
+        - A ``SnakeBidsApp``, which will replace the existing instance, so this option
+          should be used with care.
+
     """
 
     snakemake_dir: Path = attr.ib(converter=lambda path: Path(path).resolve())
+    plugins: list[Callable[[SnakeBidsApp], None | SnakeBidsApp]] = attr.Factory(list)
     skip_parse_args: bool = False
     parser: argparse.ArgumentParser = create_parser()
     configfile_path: Path = attr.Factory(
         _get_file_paths(CONFIGFILE_CHOICES, "config"), takes_self=True
     )
     snakefile_path: Path = attr.Factory(
         _get_file_paths(SNAKEFILE_CHOICES, "Snakefile"), takes_self=True
     )
-    config: Dict[str, Any] = attr.Factory(
+    config: dict[str, Any] = attr.Factory(
         lambda self: load_configfile(self.snakemake_dir / self.configfile_path),
         takes_self=True,
     )
     args: Optional[SnakebidsArgs] = None
 
-    def run_snakemake(self):
-        """Run snakemake with that config.
-
-        Workflow snakefile will read snakebids config, create inputs_config,
-        and read that in.
-        """
+    def run_snakemake(self) -> None:
+        """Run snakemake with the given config, after applying plugins"""
 
         # If no SnakebidsArgs were provided on class instantiation, we compute args
         # using the provided parser
         if self.args:
             args = self.args
         else:
             # Dynamic args include --filter-... and --wildcards-... . They depend on the
@@ -183,51 +197,57 @@
             except RunError as err:
                 print(err.msg)
                 sys.exit(1)
             cwd = args.outputdir
             new_config_file = args.outputdir / self.configfile_path
             self.config["root"] = ""
 
+        app = self
+        for plugin in self.plugins:
+            app = plugin(app) or app
+
         # Write the config file
         write_config_file(
             config_file=new_config_file,
-            data=self.config,
+            data=app.config,
             force_overwrite=True,
         )
 
         # Run snakemake (passing any leftover args from argparse)
         # Filter any blank strings before submitting
-        snakemake.main(
+        snakemake.main(  # type: ignore
             [
                 *filter(
                     None,
                     [
+                        *app.config["targets_by_analysis_level"][
+                            app.config["analysis_level"]
+                        ],
                         "--snakefile",
-                        str(self.snakefile_path),
+                        str(app.snakefile_path),
                         "--directory",
                         str(cwd),
                         "--configfile",
                         str(new_config_file.resolve()),
-                        *self.config["snakemake_args"],
-                        *self.config["targets_by_analysis_level"][
-                            self.config["analysis_level"]
-                        ],
+                        *app.config["snakemake_args"],
                     ],
                 )
             ]
         )
 
-    def create_descriptor(self, out_file):
+    def create_descriptor(self, out_file: PathLike[str] | str) -> None:
         """Generate a boutiques descriptor for this Snakebids app."""
-        new_descriptor = bc.CreateDescriptor(self.parser, execname="run.py")
-        new_descriptor.save(out_file)
+        new_descriptor = bc.CreateDescriptor(  # type: ignore
+            self.parser, execname="run.py"
+        )
+        new_descriptor.save(out_file)  # type: ignore
 
 
-def update_config(config: Dict[str, Any], snakebids_args: SnakebidsArgs):
-    # add snakemake arguments to config
+def update_config(config: dict[str, Any], snakebids_args: SnakebidsArgs) -> None:
+    """Add snakebids arguments to config in-place."""
     config.update({"snakemake_args": snakebids_args.snakemake_args})
 
     # argparse adds filter_{input_type}
     # we want to update the pybids_inputs dict with this, then remove the
     # filter_{input_type} dict
     pybids_inputs = config["pybids_inputs"]
     args = snakebids_args.args_dict
```

### Comparing `snakebids-0.7.2/snakebids/cli.py` & `snakebids-0.8.0/snakebids/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,65 @@
+from __future__ import annotations
+
 import argparse
 import logging
 import os
 import pathlib
 import re
-from typing import Any, Dict, List, Optional
+from collections.abc import Sequence
+from typing import Any, Iterable, Mapping, Optional
 
 import attr
 import snakemake
 
+from snakebids.types import InputsConfig
+
 # We define Path here in addition to pathlib to put both variables in globals()
 # This way, users specifying a path type in their config.yaml can indicate
 # either Path or pathlib.Path
 Path = pathlib.Path
 
 logger = logging.Logger(__name__)
 
 
-# pylint: disable=too-few-public-methods,
 class KeyValue(argparse.Action):
     """Class for accepting key=value pairs in argparse"""
 
     # Constructor calling
-    def __call__(self, parser, namespace, values, option_string=None):
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: str | Sequence[Any] | None,
+        option_string: str | None = None,
+    ):
         setattr(namespace, self.dest, {})
+        if not values:
+            return
 
-        for value in values:
+        for pair in values:
             # split it into key and value
-            key, value = value.split("=")
+            key, value = pair.split("=")
             # assign into dictionary
             getattr(namespace, self.dest)[key] = value
 
 
-# pylint: disable=too-few-public-methods
 class SnakemakeHelpAction(argparse.Action):
     """Class for printing snakemake usage in argparse"""
 
-    def __call__(self, parser, namespace, values, option_string=None):
-        snakemake.main(["-h"])
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: str | Sequence[Any] | None,
+        option_string: str | None = None,
+    ):
+        snakemake.main(["-h"])  # type: ignore
 
 
-# pylint: disable=missing-class-docstring
 @attr.frozen
 class SnakebidsArgs:
     """Arguments for Snakebids App
 
     Organizes the various options available for a generic Snakebids App, and store
     project specific arguments in a dict. Snakemake args are to be put in a list
 
@@ -53,46 +69,46 @@
         Force output in a directory that already has contents
     outputdir : Path
         Directory to place outputs
     pybidsdb_dir : Path
         Directory to place pybids database
     snakemake_args : list of strings
         Arguments to pass on to Snakemake
-    args_dict : Dict[str, Any]
+    args_dict : dict[str, Any]
         Contains all the snakebids specific args. Meant to contain custom user args
         defined in config, as well as dynamic --filter-xx and --wildcard-xx args.
         These will eventually be printed in the new config.
     """
 
     force: bool
     outputdir: Path = attr.ib(converter=lambda p: Path(p).resolve())
-    snakemake_args: List[str]
-    args_dict: Dict[str, Any]
+    snakemake_args: list[str]
+    args_dict: dict[str, Any]
     pybidsdb_dir: Optional[Path] = None
     reset_db: bool = False
 
 
-def create_parser(include_snakemake=False):
+def create_parser(include_snakemake: bool = False) -> argparse.ArgumentParser:
     """Generate basic Snakebids Parser
 
     Includes the standard Snakebids arguments.
     """
 
     # The snakemake parser functionality did not seem to be implemented in the original
     # factoring. I left the logic here, but it should probably be removed if it's not
     # needed.
     if include_snakemake:
         # get snakemake parser
-        smk_parser = snakemake.get_argument_parser()
+        smk_parser = snakemake.get_argument_parser()  # type: ignore
 
         # create parser
         parser = argparse.ArgumentParser(
             description="Snakebids helps build BIDS Apps with Snakemake",
             add_help=False,
-            parents=[smk_parser],
+            parents=[smk_parser],  # type: ignore
         )
     else:
         parser = argparse.ArgumentParser(
             description="Snakebids helps build BIDS Apps with Snakemake"
         )
 
     standard_group = parser.add_argument_group(
@@ -159,77 +175,75 @@
         ),
     )
     return parser
 
 
 def add_dynamic_args(
     parser: argparse.ArgumentParser,
-    parse_args: Dict[str, Dict[str, str]],
-    pybids_inputs: Dict[str, Dict[str, Dict[str, Any]]],
-):
+    parse_args: Mapping[str, Mapping[str, str | Iterable[str] | bool]],
+    pybids_inputs: InputsConfig,
+) -> None:
     # create parser group for app options
     app_group = parser.add_argument_group("SNAKEBIDS", "Options for snakebids app")
 
     # update the parser with config options
     for name, arg in parse_args.items():
         # Convert type annotations from strings to class types
         # We first check that the type annotation is, in fact,
         # a str to allow the edge case where it's already
         # been converted
-        if "type" in arg and isinstance(arg["type"], str):
+        arg_copy = dict(arg)
+        if "type" in arg:
             try:
-                arg["type"] = globals()[arg["type"]]
+                arg_copy["type"] = globals()[str(arg["type"])]
             except KeyError as err:
                 raise TypeError(
                     f"{arg['type']} is not available " + f"as a type for {name}"
                 ) from err
 
-        names = _make_underscore_dash_aliases(name)
-        app_group.add_argument(*names, **arg)
+        app_group.add_argument(*_make_underscore_dash_aliases(name), **arg_copy)
 
     # general parser for
     # --filter_{input_type} {key1}={value1} {key2}={value2}...
     # create filter parsers, one for each input_type
     filter_opts = parser.add_argument_group(
         "BIDS FILTERS",
         "Filters to customize PyBIDS get() as key=value pairs",
     )
 
     for input_type in pybids_inputs.keys():
         argnames = (f"--filter-{input_type}", f"--filter_{input_type}")
-        arglist_default = [
-            f"{key}={value}"
-            for (key, value) in pybids_inputs[input_type]["filters"].items()
-        ]
-        arglist_default_string = " ".join(arglist_default)
+        filters = pybids_inputs[input_type].get("filters", {})
+        arglist_default = [f"{key}={value}" for (key, value) in filters.items()]
 
         filter_opts.add_argument(
             *argnames,
             nargs="+",
             action=KeyValue,
-            help=f"(default: {arglist_default_string})",
+            help=f"(default: {' '.join(arglist_default)})",
         )
 
     # general parser for
     # --wildcards_{input_type} {wildcard1} {wildcard2} ...
     # create wildcards parsers, one for each input_type
     wildcards_opts = parser.add_argument_group(
         "INPUT WILDCARDS",
         "File path entities to use as wildcards in snakemake",
     )
 
     for input_type in pybids_inputs.keys():
         argnames = (f"--wildcards-{input_type}", f"--wildcards_{input_type}")
-        arglist_default = [f"{wc}" for wc in pybids_inputs[input_type]["wildcards"]]
-        arglist_default_string = " ".join(arglist_default)
+        arglist_default = [
+            f"{wc}" for wc in pybids_inputs[input_type].get("wildcards", [])
+        ]
 
         wildcards_opts.add_argument(
             *argnames,
             nargs="+",
-            help=f"(default: {arglist_default_string})",
+            help=f"(default: {' '.join(arglist_default)})",
         )
 
     override_opts = parser.add_argument_group(
         "PATH OVERRIDE",
         (
             "Options for overriding BIDS by specifying absolute paths "
             "that include wildcards, e.g.: "
@@ -239,15 +253,15 @@
 
     # create path override parser
     for input_type in pybids_inputs.keys():
         argnames = (f"--path-{input_type}", f"--path_{input_type}")
         override_opts.add_argument(*argnames, default=None)
 
 
-def parse_snakebids_args(parser: argparse.ArgumentParser):
+def parse_snakebids_args(parser: argparse.ArgumentParser) -> SnakebidsArgs:
     all_args = parser.parse_known_args()
     if all_args[0].workflow_mode:
         logger.warning(
             "--workflow-mode is deprecated, and no longer has any effect. Workflow "
             "mode is automatially activated when choosing the snakemake root "
             "directory, or a subfolder of root/results, as the output directory."
         )
@@ -270,42 +284,44 @@
             if all_args[0].pybidsdb_dir is None
             else Path(all_args[0].pybidsdb_dir).resolve()
         ),
         reset_db=all_args[0].reset_db,
     )
 
 
-def _make_underscore_dash_aliases(name: str):
+def _make_underscore_dash_aliases(name: str) -> set[str]:
     """Generate --dash-arg aliases for --dash_args and vice versa
 
     If no dashes or underscores are in the argument name, a tuple containing just the
     original arg name will be returned
 
     Parameters
     ----------
     name : str
         Argument to generate conversion for
 
     Returns
     -------
-    tuple of strings
+    set of strings
         Converted args
     """
     match = re.match(r"^--(.+)$", name)
     if match:
         name_part = match.group(1)
         return {
             name,
             re.sub(r"\_", "-", name),
             f"--{re.sub(r'-', '_', name_part)}",
         }
     return {name}
 
 
-def _resolve_path(path_candidate: Any) -> Any:
+def _resolve_path(
+    path_candidate: Iterable["os.PathLike[str] | str"] | "os.PathLike[str]" | str,
+) -> Any:
     """Helper function to resolve any paths or list
     of paths it's passed. Otherwise, returns the argument
     unchanged.
 
     Parameters
     ----------
     command : list, os.Pathlike, object
@@ -313,14 +329,15 @@
 
     Returns
     -------
     list, Path, object
         If os.Pathlike or list  of os.Pathlike, the same paths resolved.
         Otherwise, the argument unchanged.
     """
-    if isinstance(path_candidate, list):
+
+    if isinstance(path_candidate, Iterable) and not isinstance(path_candidate, str):
         return [_resolve_path(p) for p in path_candidate]
 
     if isinstance(path_candidate, os.PathLike):
         return Path(path_candidate).resolve()
 
     return path_candidate
```

### Comparing `snakebids-0.7.2/snakebids/core/__init__.py` & `snakebids-0.8.0/snakebids/core/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# flake8: noqa
 __submodules__ = ["construct_bids", "filtering", "input_generation", "datasets"]
 
 __ignore__ = ["T_co"]
 
 # <AUTOGEN_INIT>
 from snakebids.core.construct_bids import bids, print_boilerplate
 from snakebids.core.datasets import BidsComponent, BidsDataset, BidsDatasetDict
```

### Comparing `snakebids-0.7.2/snakebids/core/construct_bids.py` & `snakebids-0.8.0/snakebids/core/construct_bids.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Utilities for converting Snakemake apps to BIDS apps."""
+from __future__ import annotations
 
 from collections import OrderedDict
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional
 
 
-# pylint: disable=too-many-arguments
-def bids(
-    root: Union[str, Path] = None,
-    datatype: str = None,
-    prefix: str = None,
-    suffix: str = None,
-    subject: str = None,
-    session: str = None,
+def bids(  # noqa: PLR0913
+    root: Optional[str | Path] = None,
+    datatype: Optional[str] = None,
+    prefix: Optional[str] = None,
+    suffix: Optional[str] = None,
+    subject: Optional[str] = None,
+    session: Optional[str] = None,
     include_subject_dir: bool = True,
     include_session_dir: bool = True,
     **entities: str,
-):
+) -> str:
     """Helper function for generating bids paths for snakemake workflows.
 
     File path is of the form::
 
         [root]/[sub-{subject}]/[ses-{session]/
         [prefix]_[sub-{subject}]_[ses-{session}]_[{key}-{val}_ ... ]_[suffix]
 
@@ -46,15 +46,15 @@
         whether to include the ses-{session} folder if session defined
         (default: True)
     **entities : dict, optional
         dictionary of bids entities (e.g. space=T1w for space-T1w)
 
     Returns
     -------
-    Path
+    str
         bids-like file path
 
     Examples
     --------
 
     Below is a rule using bids naming for input and output::
 
@@ -69,76 +69,87 @@
             output: bids(
                 subject='{subject}',
                 space='snsx32',
                 desc='preproc',
                 suffix='T1w.nii.gz'
             )
 
-    Note that here we are not actually using "functions as inputs" in
-    snakemake, which would require a function definition with wildcards as
-    the argument, and restrict to input/params, but bids() is being used
-    simply to return a string.
-
-    Also note that space, desc and suffix are NOT wildcards here, only
-    {subject} is. This makes it easy to combine wildcards and non-wildcards
-    with bids-like naming.
-
-    However, you can still use bids() in a lambda function. This is
-    especially useful if your wildcards are named the same as bids entities
-    (e.g. {subject}, {session}, {task} etc..)::
+    Note that here we are not actually using "functions as inputs" in snakemake, which
+    would require a function definition with wildcards as the argument, and restrict to
+    input/params, but bids() is being used simply to return a string.
+
+    Also note that space, desc and suffix are NOT wildcards here, only {subject} is.
+    This makes it easy to combine wildcards and non-wildcards with bids-like naming.
+
+    However, you can still use bids() in a lambda function. This is especially useful if
+    your wildcards are named the same as bids entities (e.g. {subject}, {session},
+    {task} etc..)::
 
         rule proc_img:
             input: lambda wildcards: bids(**wildcards,suffix='T1w.nii.gz')
             output: bids(
                 subject='{subject}',
                 space='snsx32',
                 desc='preproc',
                 suffix='T1w.nii.gz'
             )
 
-    Or another example where you may have many bids-like wildcards used in
-    your workflow::
+    Or another example where you may have many bids-like wildcards used in your
+    workflow::
 
         rule denoise_func:
             input: lambda wildcards: bids(**wildcards, suffix='bold.nii.gz')
             output: bids(
                 subject='{subject}',
                 session='{session}',
                 task='{task}',
                 acq='{acq}',
                 desc='denoise',
                 suffix='bold.nii.gz'
             )
 
-    In this example, all the wildcards will be determined from the output
-    and passed on to bids() for inputs. The output filename will have a
-    'desc-denoise' flag added to it.
-
-    Also note that even if you supply entities in a different order, the
-    entities will be ordered based on the OrderedDict defined here.
-    If entities not known are provided, they will be just be placed
-    at the end (before the suffix), in the order you provide them in.
+    In this example, all the wildcards will be determined from the output and passed on
+    to bids() for inputs. The output filename will have a 'desc-denoise' flag added to
+    it.
+
+    Also note that even if you supply entities in a different order, the entities will
+    be ordered based on the OrderedDict defined here. If entities not known are
+    provided, they will be just be placed at the end (before the suffix), in the order
+    you provide them in.
 
     Notes
     -----
 
-    * For maximum flexibility all arguments are optional (if none are
-      specified, will return empty string)
+    * For maximum flexibility all arguments are optional (if none are specified, will
+      return empty string). Note that datatype and prefix may not be used in isolation,
+      but must be given with another entity.
 
     * Some code adapted from mne-bids, specifically
       https://mne.tools/mne-bids/stable/_modules/mne_bids/utils.html
     """
-    # BUG: Datatype as the only arg is ill-defined, but no error is raised
+    if not any([entities, suffix, subject, session]) and any([datatype, prefix]):
+        raise ValueError(
+            "At least one of subject, session, suffix, or an entity must be supplied.\n"
+            "\tGot only: "
+            + " and ".join(
+                filter(
+                    None,
+                    (
+                        f"datatype='{datatype}'" if datatype else None,
+                        f"prefix='{prefix}'" if prefix else None,
+                    ),
+                )
+            )
+        )
 
     # replace underscores in keys (needed so that users can use reserved
     # keywords by appending a _)
     entities = {k.replace("_", ""): v for k, v in entities.items()}
 
     # strict ordering of bids entities is specified here:
-    # pylint: disable=unsubscriptable-object
     order: OrderedDict[str, Optional[str]] = OrderedDict(
         [
             ("task", None),
             ("acq", None),
             ("ce", None),
             ("rec", None),
             ("dir", None),
@@ -194,15 +205,15 @@
             ],
         )
     )
 
     return str(folder / filename)
 
 
-def print_boilerplate():
+def print_boilerplate() -> None:
     """Function to print out boilerplate to add to Snakefile. (not used
     anywhere yet)"""
 
     print(
         """
 # ---- begin snakebids boilerplate ------------------------------------------
```

### Comparing `snakebids-0.7.2/snakebids/core/filtering.py` & `snakebids-0.8.0/snakebids/core/filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,67 @@
+from __future__ import annotations
+
 import operator as op
 import re
-from typing import Dict, List, TypeVar, Union, overload
+from collections.abc import Iterator, Mapping
+from typing import List, Sequence, TypeVar, Union, overload
 
 import more_itertools as itx
 from typing_extensions import Literal
 
-from snakebids.utils.utils import matches_any
+from snakebids.types import ZipList, ZipListLike
+from snakebids.utils.utils import MultiSelectDict, matches_any
 
-# pylint: disable=invalid-name
 T_co = TypeVar("T_co", bound=Union[List[str], str], covariant=True)
 
 
 @overload
 def filter_list(
-    zip_list,
-    filters: Dict[str, T_co],
+    zip_list: ZipListLike,
+    filters: Mapping[str, Sequence[str] | str],
     return_indices_only: Literal[False] = ...,
     regex_search: bool = ...,
-) -> Dict[str, List[str]]:
+) -> ZipList:
     ...
 
 
 @overload
 def filter_list(
-    zip_list,
-    filters: Dict[str, T_co],
+    zip_list: ZipListLike,
+    filters: Mapping[str, Sequence[str] | str],
     return_indices_only: Literal[True] = ...,
     regex_search: bool = ...,
-) -> List[int]:
+) -> list[int]:
     ...
 
 
 def filter_list(
-    zip_list: Dict[str, List[str]],
-    filters: Dict[str, T_co],
+    zip_list: ZipListLike,
+    filters: Mapping[str, Sequence[str] | str],
     return_indices_only: bool = False,
-    regex_search=False,
-):
+    regex_search: bool = False,
+) -> ZipList | list[int]:
     """This function is used when you are expanding over some subset of the
     wildcards i.e. if your output file doesn't contain all the wildcards in
     :attr:`BidsComponent.wildcards <snakebids.BidsComponent.wildcards>`
 
     Parameters
     ----------
-    zip_list : dict
+    zip_list
         generated zip lists dict from config file to filter
 
-    filters : dict
+    filters
         wildcard values to filter the zip lists
 
-    return_indices_only : bool, default=False
+    return_indices_only
         return the indices of the matching wildcards
 
-    regex_search : bool, default=False
+    regex_search
         Use regex matching to filter instead of the default equality check.
 
-    Returns
-    -------
-    dict
-        zip list with non-matching elements removed
 
     Examples
     --------
     ::
 
         >>> import snakebids
 
@@ -131,36 +130,41 @@
         True
     """
     if regex_search:
         match_func = re.match
     else:
         match_func = op.eq
 
-    keep_indices = set.intersection(
-        # Get a set {0,1,2,3...n-1} where n is the length of any one of the lists in
-        # zip_list
-        {*_get_zip_list_indices(zip_list)},
+    # Get a set {0,1,2,3...n-1} where n is the length of any one of the lists in
+    # zip_list
+    keep_indices = set(_get_zip_list_indices(zip_list)).intersection(
         *(
             {
                 i
                 for i, v in enumerate(zip_list[key])
                 if matches_any(v, itx.always_iterable(val), match_func)
             }
             for key, val in filters.items()
             if key in zip_list
         )
     )
 
     # Now we have the indices, so filter the lists
     if return_indices_only:
         return list(keep_indices)
-    return {key: [val[i] for i in keep_indices] for key, val in zip_list.items()}
+    return MultiSelectDict(
+        {key: [val[i] for i in keep_indices] for key, val in zip_list.items()}
+    )
 
 
-def get_filtered_ziplist_index(zip_list, wildcards, subj_wildcards):
+def get_filtered_ziplist_index(
+    zip_list: ZipList,
+    wildcards: dict[str, str],
+    subj_wildcards: dict[str, str],
+) -> int | list[int]:
     """Use this function when you have wildcards for a single scan instance,
     and want to know the index of that scan, amongst that subject's scan
     instances.
 
     Parameters
     ----------
     zip_list : dict
@@ -249,15 +253,15 @@
     # get the index of the wildcard from this filtered list
     indices = filter_list(zip_list_filtered, wildcards, return_indices_only=True)
     if len(indices) == 1:
         return indices[0]
     return indices
 
 
-def _get_zip_list_indices(zip_list: Dict[str, List[str]]):
+def _get_zip_list_indices(zip_list: ZipListLike) -> Iterator[int]:
     """Convert a zip_list into its indices
 
     Generates a sequence of numbers from 0 up to the length of the zip_lists. For
     example, the zip list:
 
     zip_list = {
         "subject": ["001", "002", "001", "002"],
@@ -266,27 +270,26 @@
 
     would lead to:
 
     (0, 1, 2, 3)
 
     Parameters
     ----------
-    zip_list : Dict[str, List[str]]
+    zip_list : dict[str, list[str]]
         Zip_list to be converted
 
     Yields
     -------
     integers
         The indices of the zip_list
     """
 
     if not zip_list:
         return
 
     # Retrieve the first zip_list (all zip_lists should be the same, so it doesn't
     # matter which one we take)
-    # pylint: disable=stop-iteration-return
     sample_zip_list = zip_list[next(iter(zip_list))]
 
     # Return a sequence of numbers 0, 1, 2, 3, ... n-1 where n is the length of the
     # zip list
     yield from range(len(sample_zip_list))
```

### Comparing `snakebids-0.7.2/snakebids/core/input_generation.py` & `snakebids-0.8.0/snakebids/core/input_generation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 """Utilities for converting Snakemake apps to BIDS apps."""
+from __future__ import annotations
 
 import json
 import logging
 import re
 from collections import defaultdict
 from pathlib import Path
-from typing import Dict, Generator, Iterable, List, Optional, Tuple, Union, overload
+from typing import Any, Generator, Iterable, Optional, Sequence, overload
 
 import more_itertools as itx
 from bids import BIDSLayout, BIDSLayoutIndexer
-from bids.layout import Query
+from bids.layout import BIDSFile, Query
+from snakemake.script import Snakemake
 from typing_extensions import Literal
 
 from snakebids.core.datasets import BidsComponent, BidsDataset, BidsDatasetDict
 from snakebids.core.filtering import filter_list
-from snakebids.exceptions import ConfigError
-from snakebids.types import InputsConfig
+from snakebids.exceptions import ConfigError, PybidsError
+from snakebids.types import InputsConfig, ZipList
 from snakebids.utils.snakemake_io import glob_wildcards
-from snakebids.utils.utils import BidsEntity, BidsParseError, surround
+from snakebids.utils.utils import BidsEntity, BidsParseError, MultiSelectDict, surround
 
 _logger = logging.getLogger(__name__)
 
 
-# pylint: disable=too-many-arguments
 @overload
-def generate_inputs(
-    bids_dir,
+def generate_inputs(  # noqa: PLR0913
+    bids_dir: Path | str,
     pybids_inputs: InputsConfig,
-    pybids_database_dir=...,
-    pybids_reset_database=...,
-    derivatives=...,
-    pybids_config=...,
-    limit_to=...,
-    participant_label=...,
-    exclude_participant_label=...,
-    use_bids_inputs: Union[Literal[False], None] = ...,
-) -> BidsDatasetDict:
+    pybids_database_dir: Path | str | None = ...,
+    pybids_reset_database: bool = ...,
+    derivatives: bool | Path | str = ...,
+    pybids_config: str | None = ...,
+    limit_to: Iterable[str] | None = ...,
+    participant_label: Iterable[str] | str | None = ...,
+    exclude_participant_label: Iterable[str] | str | None = ...,
+    use_bids_inputs: Literal[True] | None = ...,
+) -> BidsDataset:
     ...
 
 
-# pylint: disable=too-many-arguments
 @overload
-def generate_inputs(
-    bids_dir,
+def generate_inputs(  # noqa: PLR0913
+    bids_dir: Path | str,
     pybids_inputs: InputsConfig,
-    pybids_database_dir=...,
-    pybids_reset_database=...,
-    derivatives=...,
-    pybids_config=...,
-    limit_to=...,
-    participant_label=...,
-    exclude_participant_label=...,
-    use_bids_inputs: Literal[True] = ...,
-) -> BidsDataset:
+    pybids_database_dir: Path | str | None = ...,
+    pybids_reset_database: bool = ...,
+    derivatives: bool | Path | str = ...,
+    pybids_config: str | None = ...,
+    limit_to: Iterable[str] | None = ...,
+    participant_label: Iterable[str] | str | None = ...,
+    exclude_participant_label: Iterable[str] | str | None = ...,
+    use_bids_inputs: Literal[False] = ...,
+) -> BidsDatasetDict:
     ...
 
 
-# pylint: disable=too-many-arguments, too-many-locals
-def generate_inputs(
-    bids_dir,
+def generate_inputs(  # noqa: PLR0913
+    bids_dir: Path | str,
     pybids_inputs: InputsConfig,
-    pybids_database_dir=None,
-    pybids_reset_database=False,
-    derivatives=False,
-    pybids_config=None,
-    limit_to=None,
-    participant_label=None,
-    exclude_participant_label=None,
-    use_bids_inputs=None,
-):
+    pybids_database_dir: Path | str | None = None,
+    pybids_reset_database: bool = False,
+    derivatives: bool | Path | str = False,
+    pybids_config: str | None = None,
+    limit_to: Iterable[str] | None = None,
+    participant_label: Iterable[str] | str | None = None,
+    exclude_participant_label: Iterable[str] | str | None = None,
+    use_bids_inputs: bool | None = None,
+) -> BidsDataset | BidsDatasetDict:
     """Dynamically generate snakemake inputs using pybids_inputs
 
     Pybids is used to parse the bids_dir. Custom paths can also be parsed by including
     the custom_paths entry under the pybids_inputs descriptor.
 
     Parameters
     ----------
-    bids_dir : str
+    bids_dir
         Path to bids directory
 
-    pybids_inputs : dict
+    pybids_inputs
         Configuration for bids inputs, with keys as the names (``str``)
 
-        Nested `dicts` with the following required keys:
+        Nested `dicts` with the following required keys (for complete info, see
+        :class:`~snakebids.types.InputConfig`):
 
         * ``"filters"``: Dictionary of entity: "values" (dict of str -> str or list of
           str). The entity keywords should the bids tags on which to filter. The values
           should be an acceptable str value for that entity, or a list of acceptable str
           values.
 
         * ``"wildcards"``: List of (str) bids tags to include as wildcards in
@@ -96,90 +96,102 @@
           in the output paths. Any wildcards in this list that are not in the
           filename will just be ignored.
 
         * ``"custom_path"``: Custom path to be parsed with wildcards wrapped in braces,
           as in ``/path/to/sub-{subject}/{wildcard_1}-{wildcard_2}``. This path will be
           parsed without pybids, allowing the use of non-bids-compliant paths.
 
-    pybids_database_dir : str
+    pybids_database_dir
         Path to database directory. If None is provided, database
         is not used
 
-    pybids_reset_database : bool
+    pybids_reset_database
         A boolean that determines whether to reset / overwrite
         existing database.
 
-    derivatives : bool
+    derivatives
         Indicates whether pybids should look for derivative datasets under bids_dir.
         These datasets must be properly formatted according to bids specs to be
         recognized. Defaults to False.
 
-    limit_to : list of str, optional
+    limit_to
         If provided, indicates which input descriptors from pybids_inputs should be
         parsed. For example, if pybids_inputs describes ``"bold"`` and ``"dwi"`` inputs,
         and ``limit_to = ["bold"]``, only the "bold" inputs will be parsed. "dwi" will
         be ignored
 
-    participant_label : str or list of str, optional
+    participant_label
         Indicate one or more participants to be included from input parsing. This may
         cause errors if subject filters are also specified in pybids_inputs. It may not
         be specified if exclude_participant_label is specified
 
-    exclude_participant_label : str or list of str, optional
+    exclude_participant_label
         Indicate one or more participants to be excluded from input parsing. This may
         cause errors if subject filters are also specified in pybids_inputs. It may not
         be specified if participant_label is specified
 
-    use_bids_inputs : bool, optional
-        If True, opts in to the new :class:`BidsDataset` output, otherwise returns the
-        classic dict. Currently, the classic dict will be returned by default, however,
-        this will change in a future release. If you do not wish to migrate to the new
-        BidsDataset, we recommend you explictely set this parameter to False
+    use_bids_inputs
+        If False, returns the classic :class:`BidsDatasetDict` instead of
+        :class`BidsDataset`. Setting to True is deprecated as of v0.8, as this is now
+        the default behaviour
 
     Returns
     -------
-    BidsDataset or BidsDatasetDict:
+    BidsDataset | BidsDatasetDict
         Object containing organized information about the bids inputs for consumption in
         snakemake. See the documentation of :class:`BidsDataset` for details and
         examples.
 
     Example
     -------
     As an example, consider the following BIDS dataset::
 
-        bids-example/
+        example
+        ├── README.md
         ├── dataset_description.json
-        ├── participants.tsv
-        ├── README
-        └── sub-control01
-            ├── anat
-            │   ├── sub-control01_T1w.json
-            │   ├── sub-control01_T1w.nii.gz
-            │   ├── sub-control01_T2w.json
-            │   └── sub-control01_T2w.nii.gz
-            ├── dwi
-            │   ├── sub-control01_dwi.bval
-            │   ├── sub-control01_dwi.bvec
-            │   └── sub-control01_dwi.nii.gz
-            ├── fmap
-            │   ├── sub-control01_magnitude1.nii.gz
-            │   ├── sub-control01_phasediff.json
-            │   ├── sub-control01_phasediff.nii.gz
-            │   └── sub-control01_scans.tsv
-            └── func
-                ├── sub-control01_task-nback_bold.json
-                ├── sub-control01_task-nback_bold.nii.gz
-                ├── sub-control01_task-nback_events.tsv
-                ├── sub-control01_task-nback_physio.json
-                ├── sub-control01_task-nback_physio.tsv.gz
-                ├── sub-control01_task-nback_sbref.nii.gz
-                ├── sub-control01_task-rest_bold.json
-                ├── sub-control01_task-rest_bold.nii.gz
-                ├── sub-control01_task-rest_physio.json
-                └── sub-control01_task-rest_physio.tsv.gz
+        ├── participant.tsv
+        ├── sub-001
+        │   ├── ses-01
+        │   │   ├── anat
+        │   │   │   ├── sub-001_ses-01_run-01_T1w.json
+        │   │   │   ├── sub-001_ses-01_run-01_T1w.nii.gz
+        │   │   │   ├── sub-001_ses-01_run-02_T1w.json
+        │   │   │   └── sub-001_ses-01_run-02_T1w.nii.gz
+        │   │   └── func
+        │   │       ├── sub-001_ses-01_task-nback_bold.json
+        │   │       ├── sub-001_ses-01_task-nback_bold.nii.gz
+        │   │       ├── sub-001_ses-01_task-rest_bold.json
+        │   │       └── sub-001_ses-01_task-rest_bold.nii.gz
+        │   └── ses-02
+        │       ├── anat
+        │       │   ├── sub-001_ses-02_run-01_T1w.json
+        │       │   └── sub-001_ses-02_run-01_T1w.nii.gz
+        │       └── func
+        │           ├── sub-001_ses-02_task-nback_bold.json
+        │           ├── sub-001_ses-02_task-nback_bold.nii.gz
+        │           ├── sub-001_ses-02_task-rest_bold.json
+        │           └── sub-001_ses-02_task-rest_bold.nii.gz
+        └── sub-002
+            ├── ses-01
+            │   ├── anat
+            │   │   ├── sub-002_ses-01_run-01_T1w.json
+            │   │   ├── sub-002_ses-01_run-01_T1w.nii.gz
+            │   │   ├── sub-002_ses-01_run-02_T1w.json
+            │   │   └── sub-002_ses-01_run-02_T1w.nii.gz
+            │   └── func
+            │       ├── sub-002_ses-01_task-nback_bold.json
+            │       ├── sub-002_ses-01_task-nback_bold.nii.gz
+            │       ├── sub-002_ses-01_task-rest_bold.json
+            │       └── sub-002_ses-01_task-rest_bold.nii.gz
+            └── ses-02
+                └── anat
+                    ├── sub-002_ses-02_run-01_T1w.json
+                    ├── sub-002_ses-02_run-01_T1w.nii.gz
+                    ├── sub-002_ses-02_run-02_T1w.json
+                    └── sub-002_ses-02_run-02_T1w.nii.gz
 
     With the following ``pybids_inputs`` defined in the config file::
 
         pybids_inputs:
           bold:
             filters:
               suffix: 'bold'
@@ -188,73 +200,38 @@
             wildcards:
               - subject
               - session
               - acquisition
               - task
               - run
 
-    Then ``generate_inputs(bids_dir, pybids_input)`` would return the
-    following values::
+    Then ``generate_inputs(bids_dir, pybids_input)`` would return the following values::
 
-        {
-            "input_path": {
-                "bold": "bids-example/sub-{subject}/func/sub-{subject}_task-{task}_bold\
-                    .nii.gz"
-            },
-            "input_zip_lists": {
-                "bold": {
-                    "subject": ["control01", "control01"],
-                    "task": ["nback", "rest"]
-                }
-            },
-            "input_lists": {
-                "bold": {
-                    "subject": ["control01"],
-                    "task": ["nback", "rest"]
-                }
-            },
-            "input_wildcards": {
-                "bold": {
-                    "subject": "{subject}",
-                    "task": "{task}"
-                }
-            },
-            "subjects": ["subject01"],
-            "sessions": [],
-            "subj_wildcards": {"subject": "{subject}"}
-        }
-
-    Or, if :class:`BidsDataset` is enabled::
-
-        <class BidsDataset>
-            path: {
-                "bold": "bids-example/sub-{subject}/func/sub-{subject}_task-{task}_bold\
-                    .nii.gz"
-            }
-            zip_lists: {
-                "bold": {
-                    "subject": ["control01", "control01"],
-                    "task": ["nback", "rest"]
-                }
-            }
-            entities: {
-                "bold": {
-                    "subject": ["control01"],
-                    "task": ["nback", "rest"]
-                }
-            }
-            wildcards: {
-                "bold": {
-                    "subject": "{subject}",
-                    "task": "{task}"
-                }
-            }
-            subjects: ["subject01"]
-            sessions: []
-            subj_wildcards: {"subject": "{subject}"}
+        BidsDataset({
+            "bold": BidsComponent(
+                name="bold",
+                path="bids/sub-{subject}/ses-{session}/func/sub-{subject}_ses-{session}\
+_task-{task}_bold.nii.gz",
+                zip_lists={
+                    "subject": ["001",   "001",  "001",   "001",  "002",   "002" ],
+                    "session": ["01",    "01",   "02",    "02",   "01",    "01"  ],
+                    "task":    ["nback", "rest", "nback", "rest", "nback", "rest"],
+                },
+            ),
+            "t1w": BidsComponent(
+                name="t1w",
+                path="example/sub-{subject}/ses-{session}/anat/sub-{subject}_\
+ses-{session}_run-{run}_T1w.nii.gz",
+                zip_lists={
+                    "subject": ["001", "001", "001", "002", "002", "002", "002"],
+                    "session": ["01",  "01",  "02",  "01",  "01",  "02",  "02" ],
+                    "run":     ["01",  "02",  "01",  "01",  "02",  "01",  "02" ],
+                },
+            ),
+        })
     """
 
     subject_filter, regex_search = _generate_filters(
         participant_label, exclude_participant_label
     )
 
     # Generates a BIDSLayout
@@ -275,31 +252,25 @@
         bids_layout=layout,
         pybids_inputs=pybids_inputs,
         limit_to=limit_to,
         regex_search=regex_search,
         **(filters),
     )
 
-    if use_bids_inputs is None:
+    if use_bids_inputs is True:
         _logger.warning(
-            "The dictionary returned by generate_inputs() will soon be deprecated in "
-            "favour of the new BidsDataset class. BidsDataset provides the same "
-            "functionality of the dict, but with attribute access and new convience "
-            "methods. In a future release, generate_inputs() will return this class "
-            "by default. You can opt into this behaviour now by setting the "
-            "`use_bids_inputs` argument in generate_inputs() to True. If you do not "
-            "wish to migrate your code to BidsDataset at this time, we recommend you "
-            "explicately set `use_bids_inputs` to False. This will preserve the "
-            "current behaviour of returning a Dict in future releases, and will "
-            "silence this warning."
+            "The parameter `use_bids_inputs` in generate_inputs() is now set, by "
+            "default, to True. Manually setting it to True is deprecated as of version "
+            "0.8. "
         )
-        use_bids_inputs = False
+    elif use_bids_inputs is None:
+        use_bids_inputs = True
 
     try:
-        dataset = BidsDataset.from_iterable(bids_inputs)
+        dataset = BidsDataset.from_iterable(bids_inputs, layout)
     except ValueError as err:
         raise ConfigError(
             "Multiple components found with the same name: "
             + ", ".join(surround(err.args[0], "'"))
         ) from err
 
     if use_bids_inputs:
@@ -309,70 +280,68 @@
 
 def _all_custom_paths(config: InputsConfig):
     """Check that all input components have a custom path"""
     return all(comp.get("custom_path") for comp in config.values())
 
 
 def _gen_bids_layout(
-    bids_dir: Union[Path, str],
-    derivatives: bool,
-    pybids_database_dir: Union[Path, str, None],
+    bids_dir: Path | str,
+    derivatives: Path | str | bool,
+    pybids_database_dir: Path | str | None,
     pybids_reset_database: bool,
-    pybids_config: Union[Path, str, None] = None,
-):
+    pybids_config: Path | str | None = None,
+) -> BIDSLayout:
     """Create (or reindex) the BIDSLayout if one doesn't exist,
     which is only saved if a database directory path is provided
 
      Parameters
     ----------
-    bids_dir : str
+    bids_dir
         Path to bids directory
 
-    derivatives : bool
+    derivatives
         A boolean (or path(s) to derivatives datasets) that
         determines whether snakebids will search in the
         derivatives subdirectory of the input dataset.
 
-    pybids_database_dir : str
+    pybids_database_dir
         Path to database directory. If None is provided, database
         is not used
 
-    pybids_reset_database : bool
+    pybids_reset_database
         A boolean that determines whether to reset / overwrite
         existing database.
 
     Returns
     -------
     layout : BIDSLayout
         Layout from pybids for accessing the BIDS dataset to grab paths
     """
 
     # Check for database_dir
     # If blank, assume db not to be used
-    if pybids_database_dir == "":
+    if not pybids_database_dir:
         pybids_database_dir = None
     # Otherwise check for relative path and update
-    elif (
-        pybids_database_dir is not None and not Path(pybids_database_dir).is_absolute()
-    ):
+    elif not Path(pybids_database_dir).is_absolute():
         pybids_database_dir = None
         _logger.warning("Absolute path must be provided, database will not be used")
 
     return BIDSLayout(
-        bids_dir,
+        str(bids_dir),
         derivatives=derivatives,
         validate=False,
         config=pybids_config,
         database_path=pybids_database_dir,
         reset_database=pybids_reset_database,
         indexer=BIDSLayoutIndexer(validate=False, index_metadata=False),
     )
 
 
-def write_derivative_json(snakemake, **kwargs):
+def write_derivative_json(snakemake: Snakemake, **kwargs: dict[str, Any]) -> None:
     """Snakemake function to read a json file, and write to a new one,
     adding BIDS derivatives fields for Sources and Parameters.
 
     Parameters
     ----------
     snakemake : struct Snakemake
         structure passed to snakemake python scripts, containing input,
@@ -393,17 +362,17 @@
     )
 
     with open(snakemake.output.json, "w", encoding="utf-8") as outfile:
         json.dump(sidecar, outfile, indent=4)
 
 
 def _generate_filters(
-    include: Union[List[str], str, None] = None,
-    exclude: Union[List[str], str, None] = None,
-) -> Tuple[List[str], bool]:
+    include: Iterable[str] | str | None = None,
+    exclude: Iterable[str] | str | None = None,
+) -> tuple[list[str], bool]:
     """Generate Pybids filter based on inclusion or exclusion criteria
 
     Converts either a list of values to include or exclude in a list of Pybids
     compatible filters. Unlike inclusion values, exclusion requires regex filtering. The
     necessity for regex will be indicated by the boolean value of the second returned
     item: True if regex is needed, False otherwise. Raises an exception if both include
     and exclude are stipulated
@@ -438,29 +407,27 @@
     # we make the item key in search_terms a list so we can have both
     # include and exclude defined
     if include is not None:
         return [*itx.always_iterable(include)], False
 
     if exclude is not None:
         # if multiple items to exclude, combine with with item1|item2|...
-        if isinstance(exclude, list):
-            exclude_string = "|".join(re.escape(label) for label in exclude)
-        # if not, then string is the label itself
-        else:
-            exclude_string = re.escape(exclude)
+        exclude_string = "|".join(
+            re.escape(label) for label in itx.always_iterable(exclude)
+        )
         # regex to exclude subjects
         return [f"^((?!({exclude_string})$).*)$"], True
     return [], False
 
 
 def _parse_custom_path(
-    input_path: Union[Path, str],
+    input_path: Path | str,
     regex_search: bool = False,
-    **filters: Union[List[str], str],
-):
+    **filters: list[str] | str,
+) -> ZipList:
     """Glob wildcards from a custom path and apply filters
 
     This replicates pybids path globbing for any custom path. Input path should have
     wildcards in braces as in "path/of/{wildcard_1}/{wildcard_2}_{wildcard_3}" Output
     will be arranged into a zip list of matches, list of matches, and Snakemake wildcard
     for each wildcard.
 
@@ -478,36 +445,28 @@
         Values to keep. Each argument is the name of the entity to search
 
     Returns
     -------
     input_zip_list, input_list, input_wildcards
     """
     wildcards = glob_wildcards(input_path)
-    wildcard_names = list(wildcards._fields)
 
-    if len(wildcard_names) == 0:
+    if not wildcards:
         _logger.warning("No wildcards defined in %s", input_path)
 
-    # Initialize output values
-    zip_lists: Dict[str, List[str]] = {}
-
     # Log an error if no matches found
-    if len(wildcards[0]) == 0:
+    if len(next(iter(wildcards.values()))) == 0:
         _logger.error("No matching files for %s", input_path)
-        return zip_lists
-
-    # Loop through every wildcard name
-    for i, wildcard in enumerate(wildcard_names):
-        zip_lists[wildcard] = wildcards[i]
+        return wildcards
 
     # Return the output values, running filtering on the zip_lists
-    return filter_list(zip_lists, filters, regex_search=regex_search)
+    return filter_list(wildcards, filters, regex_search=regex_search)
 
 
-def _parse_bids_path(path: str, entities: Iterable[str]) -> Tuple[str, Dict[str, str]]:
+def _parse_bids_path(path: str, entities: Iterable[str]) -> tuple[str, dict[str, str]]:
     """Replace parameters in an bids path with the given wildcard {tags}.
 
     Parameters
     ----------
     path : str
         BIDS path
         (e.g. "root/sub-01/ses-01/sub-01_ses-01_T1w.nii.gz")
@@ -519,15 +478,15 @@
     path : str
         Original path with the original entities replaced with wildcards.
         (e.g. "root/sub-{subject}/ses-{session}/sub-{subject}_ses-{session}_{suffix}")
     matches : iterable of (wildcard, value)
         The values matched with each wildcard
     """
 
-    wildcard_values: Dict[str, str] = {}
+    wildcard_values: dict[str, str] = {}
 
     for entity in map(BidsEntity, entities):
         # Iterate over wildcards, slowly updating the path as each entity is replaced
 
         wildcard = entity.wildcard
         match = re.search(entity.regex, path)
         if not match or not match.group(2):
@@ -537,21 +496,21 @@
         path = re.sub(entity.regex, rf"\1{{{wildcard}}}\3", path)
         value = match.group(2)
         wildcard_values[wildcard] = value
 
     return path, wildcard_values
 
 
-# pylint: disable=too-many-locals
 def _get_lists_from_bids(
     bids_layout: Optional[BIDSLayout],
     pybids_inputs: InputsConfig,
     *,
-    limit_to: "list[str] | None" = None,
-    **filters,
+    limit_to: Iterable[str] | None = None,
+    regex_search: bool = False,
+    **filters: str | Sequence[str],
 ) -> Generator[BidsComponent, None, None]:
     """Grabs files using pybids and creates snakemake-friendly lists
 
     Parameters
     ----------
     bids_layout : BIDSLayout
         Layout from pybids for accessing the BIDS dataset to grab paths
@@ -568,51 +527,61 @@
         Pybids filters to apply globally to all inputs.
 
     Yields
     ------
     BidsComponent:
         One BidsComponent is yielded for each modality described by ``pybids_inputs``.
     """
-    if limit_to is None:
-        limit_to = list(pybids_inputs)
-
-    for input_name in limit_to:
+    for input_name in limit_to or list(pybids_inputs):
         _logger.debug("Grabbing inputs for %s...", input_name)
         component = pybids_inputs[input_name]
 
         if "custom_path" in component:
             # a custom path was specified for this input, skip pybids:
             # get input_wildcards by parsing path for {} entries (using a set
             # to get unique only)
             # get zip_lists by using glob_wildcards (but need to modify
             # to deal with multiple wildcards
 
             path = component["custom_path"]
             zip_lists = _parse_custom_path(
-                path, **pybids_inputs[input_name].get("filters", {}), **filters
+                path,
+                regex_search=regex_search,
+                **pybids_inputs[input_name].get("filters", {}),
+                **filters,
             )
-            yield BidsComponent(input_name, path, zip_lists)
+            yield BidsComponent(input_name, path, MultiSelectDict(zip_lists))
             continue
 
         if bids_layout is None:
             _logger.warning(
                 "No valid bids dir given, but %s does not have a custom_path specified "
                 "and will be skipped.",
                 input_name,
             )
             continue
 
-        zip_lists = defaultdict(list)
-        paths = set()
+        zip_lists: dict[str, list[str]] = defaultdict(list)
+        paths: set[str] = set()
         pybids_filters = {
             key: Query.ANY if val is True else Query.NONE if val is False else val
             for key, val in component.get("filters", {}).items()
         }
-        for img in bids_layout.get(**pybids_filters, **filters):
-            wildcards: List[str] = [
+        try:
+            matching_files: Iterable[BIDSFile] = bids_layout.get(
+                regex_search=regex_search, **pybids_filters, **filters
+            )
+        except AttributeError as err:
+            raise PybidsError(
+                "Pybids has encountered a problem that Snakebids cannot handle. This "
+                "may indicate a missing or invalid dataset_description.json for this "
+                "dataset."
+            ) from err
+        for img in matching_files:
+            wildcards: list[str] = [
                 wildcard
                 for wildcard in component.get("wildcards", [])
                 if wildcard in img.entities
             ]
             _logger.debug("Wildcards %s found entities for %s", wildcards, img.path)
 
             try:
@@ -639,29 +608,46 @@
             for wildcard_name, value in parsed_wildcards.items():
                 zip_lists[wildcard_name].append(value)
 
             paths.add(path)
 
         # now, check to see if unique
         if len(paths) == 0:
-            _logger.warning("No input file found for %s", input_name)
+            _logger.warning(
+                "No input files found for snakebids component %s:\n"
+                "    filters:\n%s\n"
+                "    wildcards:\n%s",
+                input_name,
+                "\n".join(
+                    [
+                        f"       {key}: {val}"
+                        for key, val in component.get("filters", {}).items()
+                    ]
+                ),
+                "\n".join(
+                    [
+                        f"       {wildcard}"
+                        for wildcard in component.get("wildcards", [])
+                    ]
+                ),
+            )
             continue
         try:
             path = itx.one(paths)
         except ValueError:
-            raise ConfigError(  # pylint: disable=raise-missing-from
+            raise ConfigError(
                 f"More than one snakemake filename for {input_name}, taking the "
                 f"first. To correct this, use the --filter_{input_name} option to "
                 f"narrow the search. Found filenames: {paths}"
             )
 
-        yield BidsComponent(input_name, path, zip_lists)
+        yield BidsComponent(input_name, path, MultiSelectDict(zip_lists))
 
 
-def get_wildcard_constraints(image_types):
+def get_wildcard_constraints(image_types: InputsConfig) -> dict[str, str]:
     """Return a wildcard_constraints dict for snakemake to use, containing
     all the wildcards that are in the dynamically grabbed inputs
 
     Parameters
     ----------
     image_types : dict
```

### Comparing `snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml` & `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml`

 * *Files identical despite different names*

### Comparing `snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile` & `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py` & `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
-import sphinx_rtd_theme
 
 # -- Project information -----------------------------------------------------
 
 
 project = "{{cookiecutter.app_name}}"
 copyright = "2021, {{cookiecutter.full_name}}"
 author = "{{cookiecutter.full_name}}"
```

### Comparing `snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst` & `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst` & `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst`

 * *Files identical despite different names*

### Comparing `snakebids-0.7.2/snakebids/project_template/{{cookiecutter.app_name}}/setup.py` & `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import json
 
 import setuptools
 
-with open("README.rst", "r") as fh:
+with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-with open("pipeline_description.json", "r") as fh:
+with open("pipeline_description.json", "r", encoding="utf-8") as fh:
     pipeline = json.load(fh)
-    name = pipeline["GeneratedBy"][0]["Name"]
-    description = pipeline["Name"]
-    version = pipeline["GeneratedBy"][0]["Version"]
-    url = pipeline["GeneratedBy"][0]["CodeURL"]
-    author = pipeline["GeneratedBy"][0]["Author"]
-    author_email = pipeline["GeneratedBy"][0]["AuthorEmail"]
+name = pipeline["GeneratedBy"][0]["Name"]
+description = pipeline["Name"]
+version = pipeline["GeneratedBy"][0]["Version"]
+optional_vals = {
+    attr: pipeline["GeneratedBy"][0].get(key)
+    for attr, key in [
+        ("url", "CodeURL"),
+        ("author", "Author"),
+        ("author_email", "AuthorEmail"),
+    ]
+    if key in pipeline
+}
 
 setuptools.setup(
     name=name,
     version=version,
-    author=author,
-    author_email=author_email,
     description=description,
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    url=url,
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
             "{{cookiecutter.app_name}}={{cookiecutter.app_name}}.run:main"
         ]
     },
     install_requires=["snakebids>={{cookiecutter.snakebids_version}}", "snakemake"],
     python_requires=">=3.7",
+    **optional_vals,
 )
```

### Comparing `snakebids-0.7.2/snakebids/resources/bids_tags.json` & `snakebids-0.8.0/snakebids/resources/bids_tags.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977477477477479%*

 * *Differences: {"'extension'": "{'match': '\\\\.[^/\\\\\\\\]+'}"}*

```diff
@@ -43,15 +43,15 @@
         "before": "[_/\\\\]+echo-",
         "match": "[0-9]{1,5}",
         "tag": "echo"
     },
     "extension": {
         "after": "$",
         "before": "[._]*[a-zA-Z0-9]*?",
-        "match": "[._]*[a-zA-Z0-9]*?(\\.[^/\\\\]+)$"
+        "match": "\\.[^/\\\\]+"
     },
     "flip": {
         "before": "[_/\\\\]+flip-",
         "match": "[0-9]{1,5}",
         "tag": "flip"
     },
     "from": {
```

### Comparing `snakebids-0.7.2/snakebids/utils/output.py` & `snakebids-0.8.0/snakebids/utils/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Tools to manage generation and interconversion of bidsapps and snakemake outputs."""
 
+from __future__ import annotations
+
 import hashlib
 import json
 import time
 from collections import OrderedDict
 from pathlib import Path, PosixPath, WindowsPath
-from typing import Dict, Union
+from typing import Any
 
 import more_itertools as itx
 import yaml
 from typing_extensions import Literal
 
 from snakebids.exceptions import RunError
 
-Mode = Union[Literal["workflow"], Literal["bidsapp"]]
+Mode = Literal["workflow", "bidsapp"]
 
 
-def prepare_bidsapp_output(outputdir: Path, force_output: bool = False):
+def prepare_bidsapp_output(outputdir: Path, force_output: bool = False) -> None:
     """Ensure output directory is in the correct mode and is ready for snakemake to run
 
     Checks for existing output at the directory, creating it if necessary. Creates a
     .snakebids file to track output mode and other workflow information. If outputdir
     already has contents but no .snakebids file, it raises an exception unless
     force_output == True.
 
@@ -53,15 +55,15 @@
             raise err
 
     outputdir.mkdir(exist_ok=True)
 
     write_output_mode(outputdir / ".snakebids", "bidsapp")
 
 
-def write_output_mode(dotfile: Path, mode: Mode):
+def write_output_mode(dotfile: Path, mode: Mode) -> None:
     """Write output mode to .snakebids
 
     Parameters
     ----------
     dotfile: Path
         Path to .snakebids file to be written
     mode: Mode
@@ -73,15 +75,15 @@
     else:
         data = {}
     data["mode"] = mode
     with (dotfile).open("w") as f:
         json.dump(data, f)
 
 
-def _get_snakebids_file(outputdir: Path):
+def _get_snakebids_file(outputdir: Path) -> dict[str, str] | None:
     """Ensure populated dir contains .snakebids file, retrieving it if it does.
 
     First checks if outputdir doesn't exist or is completely empty, returing None if so.
     If it does have data, it checks for a .snakebids file, returning its contents if
     found. If no .snakebids file is found, it raises an exception.
 
     Parameters
@@ -113,15 +115,15 @@
     if (outputdir / ".snakebids").exists():
         malformed_err = RunError(
             f"Found malformed .snakebids file in `{outputdir.resolve()}. Please "
             "remove this file and check the integrity of previous outputs."
         )
         with (outputdir / ".snakebids").open("r") as f:
             try:
-                snakebids_data: Dict[str, str] = json.load(f)
+                snakebids_data: dict[str, str] = json.load(f)
             except json.JSONDecodeError as err:
                 raise malformed_err from err
         if "mode" not in snakebids_data:
             raise malformed_err
 
         return snakebids_data
 
@@ -130,23 +132,25 @@
     raise RunError(
         f"Output dir `{outputdir.resolve()}` exists, but it doesn't look like this "
         "app has been run there before. If you're sure you got the directory correct, "
         "run the app again using `--force-output`",
     )
 
 
-def get_time_hash():
+def get_time_hash() -> str:
     """currently unused"""
 
     time_hash = hashlib.sha1()
     time_hash.update(str(time.time()).encode("utf-8"))
     return time_hash.hexdigest()[:8]
 
 
-def write_config_file(config_file: Path, data: dict, force_overwrite: bool = False):
+def write_config_file(
+    config_file: Path, data: dict[str, Any], force_overwrite: bool = False
+) -> None:
     if (config_file.exists()) and not force_overwrite:
         raise RunError(
             f"A config file named {config_file.name} already exists:\n"
             f"\t- {config_file.resolve()}\n"
             "Please move or rename either the existing or incoming config."
         )
     config_file.parent.mkdir(exist_ok=True)
@@ -162,20 +166,22 @@
             return
 
         # if not json, then should be yaml or yml
 
         # this is needed to make the output yaml clean
         yaml.add_representer(
             OrderedDict,
-            lambda dumper, data: dumper.represent_mapping(
-                "tag:yaml.org,2002:map", data.items()
+            lambda dumper, data: dumper.represent_mapping(  # type: ignore
+                "tag:yaml.org,2002:map", data.items()  # type: ignore
             ),
         )
 
         # Represent any PathLikes as str.
-        def path2str(dumper, data):
-            return dumper.represent_scalar("tag:yaml.org,2002:str", str(data))
+        def path2str(dumper, data):  # type: ignore
+            return dumper.represent_scalar(  # type: ignore
+                "tag:yaml.org,2002:str", str(data)  # type: ignore
+            )
 
-        yaml.add_representer(PosixPath, path2str)
-        yaml.add_representer(WindowsPath, path2str)
+        yaml.add_representer(PosixPath, path2str)  # type: ignore
+        yaml.add_representer(WindowsPath, path2str)  # type: ignore
 
         yaml.dump(data, f, default_flow_style=False, sort_keys=False)
```

### Comparing `snakebids-0.7.2/snakebids/utils/snakemake_io.py` & `snakebids-0.8.0/snakebids/utils/snakemake_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-""" Minor modification to allow glob_wildcards() to have multiple occurence of
-same wildcard """
+"""File globbing functions based on snakemake.io library"""
+from __future__ import annotations
 
 import collections
 import os
 import re
 from itertools import chain
+from pathlib import Path
+from typing import Sequence
 
+from snakebids.types import ZipList
+from snakebids.utils.utils import MultiSelectDict
 
-def regex(filepattern):
+
+def regex(filepattern: str) -> str:
     """Build Snakebids regex based on the given file pattern."""
-    regex_list = []
+    regex_list: list[str] = []
     last = 0
-    wildcards = set()
+    wildcards: set[str] = set()
     for match in _wildcard_regex.finditer(filepattern):
         regex_list.append(re.escape(filepattern[last : match.start()]))
         wildcard = match.group("name")
         if wildcard in wildcards:
             if match.group("constraint"):
                 raise ValueError(
                     "Constraint regex must be defined only in the first "
@@ -49,92 +54,91 @@
         ))\1
     \}
     """,
     re.VERBOSE,
 )
 
 
-def glob_wildcards(pattern, files=None, followlinks=False):
+def glob_wildcards(
+    pattern: str | Path,
+    files: Sequence[str | Path] | None = None,
+    followlinks: bool = False,
+) -> ZipList:
     """Glob the values of wildcards by matching a pattern to the filesystem.
 
+    Returns a zip_list of field names with matched wildcard values.
+
     Parameters
     ----------
-    pattern : str
+    pattern
         Path including wildcards to glob on the filesystem.
-    files : list of str, optional
+    files
         Files from which to glob wildcards. If None (default), the directory
         corresponding to the first wildcard in the pattern is walked, and
         wildcards are globbed from all files.
-    followlinks : bool, optional
-        Whether to follow links when globbing wildcards. Default: False.
-
-    Returns
-    -------
-    namedtuple
-        "Wildcards" named tuple where each field name is the name of a
-        wildcard and the value of each field is a list of values for the
-        corresponding wildcard.
+    followlinks
+        Whether to follow links when globbing wildcards.
     """
     pattern = os.path.normpath(pattern)
     first_wildcard = re.search("{[^{]", pattern)
     dirname = (
         os.path.dirname(pattern[: first_wildcard.start()])
         if first_wildcard
         else os.path.dirname(pattern)
     )
     if not dirname:
-        dirname = "."
+        dirname = Path(".")
 
     names = [match.group("name") for match in _wildcard_regex.finditer(pattern)]
 
     # remove duplicates while preserving ordering
-    names = list(collections.OrderedDict.fromkeys(names))
-
-    # TODO: using namedtuple prevents python keywords (as, from, etc) from being used
-    #       as wildcards. A Dict would be more appropriate here
-    # pylint: disable-msg=invalid-name
-    Wildcards = collections.namedtuple("Wildcards", names)
+    names = list(dict.fromkeys(names))
 
-    wildcards = Wildcards(*[[] for _ in names])
+    wildcards: dict[str, list[str]] = collections.defaultdict(list)
 
-    pattern = re.compile(regex(pattern))
+    re_pattern = re.compile(regex(pattern))
 
-    if files is None:
-        files = (
-            os.path.normpath(os.path.join(dirpath, f))
+    file_iter = (
+        (
+            Path(dirpath, f)
             for dirpath, dirnames, filenames in os.walk(
                 dirname, followlinks=followlinks
             )
             for f in chain(filenames, dirnames)
         )
+        if files is None
+        else iter(files)
+    )
 
-    for f in files:
-        match = re.match(pattern, f)
+    for f in file_iter:
+        match = re.match(re_pattern, str(f))
         if match:
             for name, value in match.groupdict().items():
-                getattr(wildcards, name).append(value)
-    return wildcards
+                wildcards[name].append(value)
+    return MultiSelectDict(wildcards)
 
 
 def update_wildcard_constraints(
-    pattern, wildcard_constraints, global_wildcard_constraints
-):
+    pattern: str,
+    wildcard_constraints: dict[str, str],
+    global_wildcard_constraints: dict[str, str],
+) -> str:
     """Update wildcard constraints.
 
     Parameters
     ----------
     pattern : str
         Pattern on which to update constraints.
     wildcard_constraints : dict
         Dictionary of wildcard:constraint key-value pairs.
     global_wildcard_constraints : dict
         Dictionary of wildcard:constraint key-value pairs.
     """
 
-    def replace_constraint(match):
+    def replace_constraint(match: re.Match[str]):
         name = match.group("name")
         constraint = match.group("constraint")
         newconstraint = wildcard_constraints.get(
             name, global_wildcard_constraints.get(name)
         )
         if name in examined_names:
             return match.group(0)
@@ -143,11 +147,11 @@
         if constraint is not None:
             return match.group(0)
         # Only update if a new constraint has actually been set
         if newconstraint is not None:
             return f"{{{name},{newconstraint}}}"
         return match.group(0)
 
-    examined_names = set()
+    examined_names: set[str] = set()
     updated = _wildcard_regex.sub(replace_constraint, pattern)
 
     return updated
```

### Comparing `snakebids-0.7.2/PKG-INFO` & `snakebids-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakebids
-Version: 0.7.2
+Version: 0.8.0
 Summary: BIDS integration into snakemake workflows
 Home-page: https://github.com/akhanf/snakebids
 License: MIT
 Author: Ali Khan
 Author-email: alik@robarts.ca
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,15 @@
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: more-itertools (>=8,<10)
 Requires-Dist: numpy (>=1.21.2) ; python_version == "3.10"
 Requires-Dist: numpy (>=1.23.2) ; python_version >= "3.11"
 Requires-Dist: pandas (>=1.3) ; python_full_version >= "3.7.1"
 Requires-Dist: pandas (>=1.5) ; python_version >= "3.11"
+Requires-Dist: pvandyken-deprecated (==0.0.3)
 Requires-Dist: pybids (>=0.15.0,<0.16.0)
 Requires-Dist: scipy (<1.8) ; python_version == "3.7"
 Requires-Dist: scipy (>=1.9.2) ; python_version >= "3.11"
 Requires-Dist: snakemake (>=5.28.0) ; python_version >= "3.7"
 Requires-Dist: snakemake (>=7.18.2) ; python_version >= "3.11"
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Documentation, https://snakebids.readthedocs.io/
```

