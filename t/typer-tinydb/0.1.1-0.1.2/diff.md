# Comparing `tmp/typer_tinydb-0.1.1.tar.gz` & `tmp/typer_tinydb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_tinydb-0.1.1.tar", max compression
+gzip compressed data, was "typer_tinydb-0.1.2.tar", max compression
```

## Comparing `typer_tinydb-0.1.1.tar` & `typer_tinydb-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0      778 2023-04-23 21:36:45.377246 typer_tinydb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3847 2023-04-23 20:34:49.890491 typer_tinydb-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-04-23 20:14:19.153661 typer_tinydb-0.1.1/typer_tinydb/__init__.py
--rw-r--r--   0        0        0     5922 2023-04-23 20:29:06.944652 typer_tinydb-0.1.1/typer_tinydb/typerdb.py
--rw-r--r--   0        0        0     4851 1970-01-01 00:00:00.000000 typer_tinydb-0.1.1/setup.py
--rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 typer_tinydb-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-24 09:25:26.352787 typer_tinydb-0.1.2/LICENSE
+-rw-r--r--   0        0        0      909 2023-04-24 08:38:44.364321 typer_tinydb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2659 2023-04-24 14:01:43.062943 typer_tinydb-0.1.2/README.md
+-rw-r--r--   0        0        0       67 2023-04-24 08:17:32.671020 typer_tinydb-0.1.2/typer_tinydb/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-24 08:39:15.333006 typer_tinydb-0.1.2/typer_tinydb/static/config.json
+-rw-r--r--   0        0        0       23 2023-04-24 05:58:42.137034 typer_tinydb-0.1.2/typer_tinydb/tests/__init__.py
+-rw-r--r--   0        0        0     4959 2023-04-24 06:40:12.321673 typer_tinydb-0.1.2/typer_tinydb/tests/test_upsert.py
+-rw-r--r--   0        0        0    10881 2023-04-24 08:38:08.056830 typer_tinydb-0.1.2/typer_tinydb/typerdb.py
+-rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 typer_tinydb-0.1.2/setup.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 typer_tinydb-0.1.2/PKG-INFO
```

### Comparing `typer_tinydb-0.1.1/pyproject.toml` & `typer_tinydb-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-[tool.poetry]
-name = "typer-tinydb"
-version = "0.1.1"
-description = "A Python Typer CLI subcommand boilerplate to manage config files using tinydb"
-authors = ["arnos-stuff <bcda0276@gmail.com>"]
-readme = "README.md"
-packages = [{include = "typer_tinydb"}]
-homepage = "https://arnos-stuff.github.io/typer-tinydb/"
-
-[tool.poetry.dependencies]
-python = "^3.9"
-typer = {extras = ["all"], version = "^0.7.0"}
-tinydb = "^4.7.1"
-
-
-[tool.poetry.scripts]
-typer-tinydb-config = 'typer_tinydb.typerdb:config'
-typer-configure = 'typer_tinydb.typerdb:config'
-tcfg = 'typer_tinydb.typerdb:cfg'
-
-[tool.poetry.group.dev.dependencies]
-mkdocs = "^1.4.2"
-mkdocs-dracula-theme = "^1.0.4"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "typer-tinydb"
+version = "0.1.2"
+description = "A Python Typer CLI subcommand boilerplate to manage config files using tinydb"
+authors = ["arnos-stuff <bcda0276@gmail.com>"]
+readme = "README.md"
+packages = [{include = "typer_tinydb"}]
+homepage = "https://arnos-stuff.github.io/typer-tinydb/"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+typer = {extras = ["all"], version = "^0.7.0"}
+tinydb = "^4.7.1"
+
+
+[tool.poetry.scripts]
+typer-tinydb-config = 'typer_tinydb.typerdb:config'
+tcfg = 'typer_tinydb.typerdb:cfg'
+
+[tool.poetry.group.dev.dependencies]
+mkdocs = "^1.4.2"
+mkdocs-dracula-theme = "^1.0.4"
+mkdocs-material = "^9.1.7"
+pillow = "^9.5.0"
+cairosvg = "^2.7.0"
+mike = "^1.1.2"
+shtab = "^1.6.1"
+mkdocs-glightbox = "^0.3.3"
+flake8 = "^6.0.0"
+pytest = "^7.3.1"
+codecov = "^2.1.13"
+pytest-cov = "^4.0.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `typer_tinydb-0.1.1/setup.py` & `typer_tinydb-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['typer_tinydb']
+['typer_tinydb', 'typer_tinydb.tests']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'typer_tinydb': ['static/*']}
 
 install_requires = \
 ['tinydb>=4.7.1,<5.0.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['tcfg = typer_tinydb.typerdb:cfg',
-                     'typer-configure = typer_tinydb.typerdb:config',
                      'typer-tinydb-config = typer_tinydb.typerdb:config']}
 
 setup_kwargs = {
     'name': 'typer-tinydb',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A Python Typer CLI subcommand boilerplate to manage config files using tinydb',
-    'long_description': '# A Typer config file get/set boilerplate\n\n# Using the boilerplate\n\n## Aliases and subcommands\n\nWe recommand the following aliases, which are readily available out of the box.\n\n- `config`\n- `cfg`\n- `c`\n\nThis way, if your app is named `super-app`\n\nAnd is defined in `super_app.py` roughly as follows:\n\n```python\n\nimport typer\n\n# ... some imports\n\napp = typer.Typer(\n    name=\'super-app\',\n    # ... other args\n)\n```\n\nYou just have to add the following below:\n\n```python\nfrom typer_tinydb import cfg, config # those are typer apps\n\napp.add_typer(cfg) # the cfg app\napp.add_typer(config) # the config app\n```\n\nYou can rename them however you like by using\n\n```python\napp.add_typer(cfg, name=\'my-super-config\')\n```\n\n## Using it on the command line\n\nWith the same configuration as above, your new app can now run the commands:\n\n```bash\nsuper-app cfg list # list config key:value pairs\nsuper-app cfg get some-key # get the values linked to the key \'some-key\'\nsuper-app cfg set some-key \'20-hS407zuqYKQ8tPP2r5\' # store some hash or token into your settings file\nsuper-app cfg set some-key \'20-hS407zuqYKQ8tPP2r5\'\n```\n\nYou can obviously use `super-app config get` and others, or any name you attribute to it.\n\n## Using it within python modules\n\nThe CLI key-values are stored in a tinydb instance that is available by just importing the table named `globals`:\n\n```python\nfrom typer_tinydb import db, globals, where\n```\n\nYou can create any table using the database object `db`, please [check out the tinydb docs !](https://tinydb.readthedocs.io/)\n\nTo get the key just use `where` :\n\n```python\nreturns = globals.search(where(\'param\') == param)\n```\n\nTo insert new values or update existing, use the `upsert` function:\n\n```python\nParam = Query()\n\nglobals.upsert({\n    "param": param,\n    "value": value,\n    "timestamp": datetime.now().strftime("%d/%m/%Y %H:%M:%S"),\n    "machine": socket.gethostname(),\n    },\n    Param.param == param\n)\n```\n\n# Commands\n\n## Command `typer-tinydb-config`\n\nConfigure the app 🛠️.\n\n**Usage**:\n\n```console\n$ typer-tinydb-config [OPTIONS] COMMAND [ARGS]...\n```\n\n**Options**:\n\n* `--install-completion`: Install completion for the current shell.\n* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n* `--help`: Show this message and exit.\n\n**Commands**:\n\n* `get`: Get a config value.\n* `list`: List all config values.\n* `reset`: Reset all config values.\n* `set`: Set a config value.\n\n### Command `typer-tinydb-config get`\n\nGet a config value.\n\n**Usage**:\n\n```console\n$ typer-tinydb-config get [OPTIONS] PARAM\n```\n\n**Arguments**:\n\n* `PARAM`: The parameter to get.  [required]\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n### Command `typer-tinydb-config list`\n\nList all config values.\n\n**Usage**:\n\n```console\n$ typer-tinydb-config list [OPTIONS]\n```\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n### Command `typer-tinydb-config reset`\n\nReset all config values.\n\n**Usage**:\n\n```console\n$ typer-tinydb-config reset [OPTIONS]\n```\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n### Command `typer-tinydb-config set`\n\nSet a config value.\n\n**Usage**:\n\n```console\n$ typer-tinydb-config set [OPTIONS] PARAM VALUE\n```\n\n**Arguments**:\n\n* `PARAM`: The parameter to set.  [required]\n* `VALUE`: The value to set the parameter to.  [required]\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n\n# Future updates\n\nThe idea is to add some extra features like\n\n- [ ] Creating your own tables from the CLI\n- [ ] Adding some customization (in terms of colors) for the printing\n- [ ] Adding obfuscation so that your `.json` config file cannot be easily glanced at by bypassers\n\n',
+    'long_description': '\n[![PyPI version](https://badge.fury.io/py/typer-tinydb.svg)](https://badge.fury.io/py/typer-tinydb) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/arnos-stuff/typer-tinydb/master/LICENSE)\n[![codecov](https://codecov.io/gh/arnos-stuff/typer-tinydb/branch/master/graph/badge.svg?token=7MP5WBU8GI)](https://codecov.io/gh/arnos-stuff/typer-tinydb)\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/arnos-stuff/typer-tinydb/tree/master.svg?style=shield "CircleCI Build Status")](https://dl.circleci.com/status-badge/redirect/gh/arnos-stuff/typer-tinydb/tree/master)\n\n# A Typer config file get/set boilerplate\n\n# Using the boilerplate\n\n## Aliases and subcommands\n\nWe recommand the following aliases, which are readily available out of the box.\n\n- `config`\n- `cfg`\n- `c`\n\nThis way, if your app is named `super-app`\n\nAnd is defined in `super_app.py` roughly as follows:\n\n```python\n\nimport typer\n\n# ... some imports\n\napp = typer.Typer(\n    name=\'super-app\',\n    # ... other args\n)\n```\n\nYou just have to add the following below:\n\n```python\nfrom typer_tinydb import cfg, config # those are typer apps\n\napp.add_typer(cfg) # the cfg app\napp.add_typer(config) # the config app\n```\n\nYou can rename them however you like by using\n\n```python\napp.add_typer(cfg, name=\'my-super-config\')\n```\n\n## Using it on the command line\n\nWith the same configuration as above, your new app can now run the commands:\n\n```bash\nsuper-app cfg list # list config key:value pairs\nsuper-app cfg get some-key # get the values linked to the key \'some-key\'\nsuper-app cfg set some-key \'20-hS407zuqYKQ8tPP2r5\' # store some hash or token into your settings file\nsuper-app cfg set some-key \'20-hS407zuqYKQ8tPP2r5\'\n```\n\nYou can obviously use `super-app config get` and others, or any name you attribute to it.\n\n## Using it within python modules\n\nThe CLI key-values are stored in a tinydb instance that is available by just importing the table named `globals`:\n\n```python\nfrom typer_tinydb import db, globals, where\n```\n\nYou can create any table using the database object `db`, please [check out the tinydb docs !](https://tinydb.readthedocs.io/)\n\nTo get the key just use `where` :\n\n```python\nreturns = globals.search(where(\'param\') == param)\n```\n\nTo insert new values or update existing, use the `upsert` function:\n\n```python\nParam = Query()\n\nglobals.upsert({\n    "param": param,\n    "value": value,\n    "timestamp": datetime.now().strftime("%d/%m/%Y %H:%M:%S"),\n    "machine": socket.gethostname(),\n    },\n    Param.param == param\n)\n```\n# Commands\n\nGo check out the [documentation page 🚀](https://arnos-stuff.github.io/typer-tinydb)',
     'author': 'arnos-stuff',
     'author_email': 'bcda0276@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://arnos-stuff.github.io/typer-tinydb/',
     'packages': packages,
     'package_data': package_data,
```

