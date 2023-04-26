# Comparing `tmp/kedro_snowflake-0.0.1.tar.gz` & `tmp/kedro_snowflake-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_snowflake-0.0.1.tar", max compression
+gzip compressed data, was "kedro_snowflake-0.1.0.tar", max compression
```

## Comparing `kedro_snowflake-0.0.1.tar` & `kedro_snowflake-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,66 @@
--rw-r--r--   0        0        0    11338 2022-11-25 10:50:17.200592 kedro_snowflake-0.0.1/LICENSE
--rw-r--r--   0        0        0     1442 2022-11-25 10:50:17.200592 kedro_snowflake-0.0.1/README.md
--rw-r--r--   0        0        0       22 2022-11-25 10:50:17.200592 kedro_snowflake-0.0.1/kedro_snowflake/__init__.py
--rw-r--r--   0        0        0     1095 2022-11-25 10:50:17.200592 kedro_snowflake-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 kedro_snowflake-0.0.1/setup.py
--rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 kedro_snowflake-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-04-26 14:02:37.309880 kedro_snowflake-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4510 2023-04-26 14:02:37.309880 kedro_snowflake-0.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-26 14:02:37.313881 kedro_snowflake-0.1.0/kedro_snowflake/__init__.py
+-rw-r--r--   0        0        0     4523 2023-04-26 14:02:37.313881 kedro_snowflake-0.1.0/kedro_snowflake/cli.py
+-rw-r--r--   0        0        0     2282 2023-04-26 14:02:37.313881 kedro_snowflake-0.1.0/kedro_snowflake/cli_functions.py
+-rw-r--r--   0        0        0     4444 2023-04-26 14:02:37.313881 kedro_snowflake-0.1.0/kedro_snowflake/config.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.313881 kedro_snowflake-0.1.0/kedro_snowflake/datasets/__init__.py
+-rw-r--r--   0        0        0     5483 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/datasets/internal.py
+-rw-r--r--   0        0        0     5660 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/datasets/native.py
+-rw-r--r--   0        0        0    14301 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/generator.py
+-rw-r--r--   0        0        0      119 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/misc.py
+-rw-r--r--   0        0        0     3504 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/pipeline.py
+-rw-r--r--   0        0        0     1526 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/runner.py
+-rw-r--r--   0        0        0     1612 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/README.md
+-rw-r--r--   0        0        0      524 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/cookiecutter.json
+-rw-r--r--   0        0        0   162747 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0   162747 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0     1927 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/prompts.yml
+-rw-r--r--   0        0        0     1785 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0        0        0     3958 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md
+-rw-r--r--   0        0        0     1083 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md
+-rw-r--r--   0        0        0     2778 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0        0        0      901 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_processing.yml
+-rw-r--r--   0        0        0      232 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_science.yml
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+-rw-r--r--   0        0        0     2073 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0        0        0      431 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+-rw-r--r--   0        0        0  1810602 2023-04-26 14:02:37.325881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv
+-rw-r--r--   0        0        0  2937144 2023-04-26 14:02:37.341881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv
+-rw-r--r--   0        0        0  4195290 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+-rw-r--r--   0        0        0     6967 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0        0        0      459 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/logs/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0        0        0      446 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/setup.cfg
+-rw-r--r--   0        0        0      395 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0        0        0     1198 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
+-rw-r--r--   0        0        0     1109 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py
+-rw-r--r--   0        0        0       60 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0        0        0     1527 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0        0        0      423 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rwxr-xr-x   0        0        0      117 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/__init__.py
+-rwxr-xr-x   0        0        0     2607 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py
+-rwxr-xr-x   0        0        0     1192 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py
+-rwxr-xr-x   0        0        0      114 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/__init__.py
+-rwxr-xr-x   0        0        0     1712 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py
+-rwxr-xr-x   0        0        0      866 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py
+-rw-r--r--   0        0        0     1363 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0        0        0      369 2023-04-26 14:02:37.317880 kedro_snowflake-0.1.0/kedro_snowflake/starters.py
+-rw-r--r--   0        0        0     5272 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/kedro_snowflake/utils.py
+-rw-r--r--   0        0        0     1697 2023-04-26 14:02:37.369881 kedro_snowflake-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 kedro_snowflake-0.1.0/PKG-INFO
```

### Comparing `kedro_snowflake-0.0.1/LICENSE` & `kedro_snowflake-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.0.1/pyproject.toml` & `kedro_snowflake-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-snowflake"
-version = "0.0.1"
+version = "0.1.0"
 description = "Kedro plugin with Snowflake / Snowpark support"
 readme = "README.md"
 authors = ['GetInData MLOPS <mlops@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-snowflake"
 repository = "https://github.com/getindata/kedro-snowflake"
 documentation = "https://kedro-snowflake.readthedocs.io/"
@@ -28,15 +28,30 @@
     "raise NotImplementedError"
 ]
 
 [tool.isort]
 known_third_party = ["pydantic","semver","setuptools"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.9"
+kedro = ">=0.18.7,<0.19"
+snowflake-snowpark-python = {version = ">=1.0.0,<1.1.0", extras = ["pandas"]}
+kedro-datasets = {version = ">=1.2.0,<1.3.0", extras = ["pandas-csvdataset", "pandas-exceldataset", "pandas-parquetdataset", "snowflake-snowparktabledataset"]}
+backoff = "^2.2.1"
+cloudpickle = ">=1.6.0,<=2.0.0"
+zstandard = "^0.20.0"
+pydantic = "^1.10.7"
+tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "<7"
 pytest-cov = ">=2.8.0, <4.0.0"
 tox = ">=3.25.1"
 pre-commit = "2.20.0"
 
+[tool.poetry.plugins] # Optional super table
+
+[tool.poetry.plugins."kedro.project_commands"]
+"snowflake" = "kedro_snowflake.cli:commands"
+
+[tool.poetry.plugins."kedro.starters"]
+"starter" = "kedro_snowflake.starters:starters"
```

