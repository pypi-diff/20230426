# Comparing `tmp/ocean-model-skill-assessor-0.7.0.tar.gz` & `tmp/ocean-model-skill-assessor-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean-model-skill-assessor-0.7.0.tar", last modified: Wed Apr 26 15:24:07 2023, max compression
+gzip compressed data, was "ocean-model-skill-assessor-0.7.1.tar", last modified: Wed Apr 26 16:15:00 2023, max compression
```

## Comparing `ocean-model-skill-assessor-0.7.0.tar` & `ocean-model-skill-assessor-0.7.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.492940 ocean-model-skill-assessor-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.480940 ocean-model-skill-assessor-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.480940 ocean-model-skill-assessor-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/.github/workflows/linting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-26 15:24:07.492940 ocean-model-skill-assessor-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.480940 ocean-model-skill-assessor-0.7.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ci/environment-py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ci/environment-py3.9.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.484940 ocean-model-skill-assessor-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/add_vocab.md
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/cli_tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)   205378 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   304782 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/demo_cli.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/developer.md
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.488940 ocean-model-skill-assessor-0.7.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   295925 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/examples/ciofs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   256475 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/examples/gom_hycom.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   232328 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/examples/tbofs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)  1795175 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/vocab_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)  1388123 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/docs/vocab_widget.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.488940 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/CLI.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 15:24:07.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28970 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.492940 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14391 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/plot/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/plot/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.492940 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/erddap_coastwatch.json
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/erddap_ioos.json
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/general.json
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/standard_names.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.492940 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-26 15:24:07.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-26 15:24:07.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:24:07.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 15:24:07.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 15:24:07.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 15:24:07.000000 ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-26 15:24:07.492940 ocean-model-skill-assessor-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:07.492940 ocean-model-skill-assessor-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/tests/test_main_axds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/tests/test_main_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-26 15:23:57.000000 ocean-model-skill-assessor-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.530509 ocean-model-skill-assessor-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.518509 ocean-model-skill-assessor-0.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.518509 ocean-model-skill-assessor-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/.github/workflows/linting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-26 16:15:00.530509 ocean-model-skill-assessor-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.518509 ocean-model-skill-assessor-0.7.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ci/environment-py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ci/environment-py3.9.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.526509 ocean-model-skill-assessor-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/add_vocab.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/cli_tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   205378 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   304782 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/demo_cli.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/developer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.526509 ocean-model-skill-assessor-0.7.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   295925 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/examples/ciofs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   256475 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/examples/gom_hycom.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   232328 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/examples/tbofs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1795175 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/vocab_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1388123 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/docs/vocab_widget.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.530509 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 16:15:00.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28970 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.530509 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/plot/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/plot/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.530509 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/erddap_coastwatch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/erddap_ioos.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/general.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/standard_names.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.530509 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-26 16:15:00.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-26 16:15:00.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:15:00.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 16:15:00.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 16:15:00.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 16:15:00.000000 ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-26 16:15:00.534509 ocean-model-skill-assessor-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:15:00.530509 ocean-model-skill-assessor-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/tests/test_main_axds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/tests/test_main_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-26 16:14:53.000000 ocean-model-skill-assessor-0.7.1/tests/test_utils.py
```

### Comparing `ocean-model-skill-assessor-0.7.0/.github/workflows/release.yaml` & `ocean-model-skill-assessor-0.7.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/.github/workflows/test.yaml` & `ocean-model-skill-assessor-0.7.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/.pre-commit-config.yaml` & `ocean-model-skill-assessor-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/LICENSE.txt` & `ocean-model-skill-assessor-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/PKG-INFO` & `ocean-model-skill-assessor-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-model-skill-assessor
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package to fully run the comparison between data and model to assess model skill.
 Home-page: https://github.com/axiom-data-science/ocean-model-skill-assessor
 Author: Axiom Data Science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `ocean-model-skill-assessor-0.7.0/README.md` & `ocean-model-skill-assessor-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/Makefile` & `ocean-model-skill-assessor-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/add_vocab.md` & `ocean-model-skill-assessor-0.7.1/docs/add_vocab.md`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/cli.md` & `ocean-model-skill-assessor-0.7.1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/cli_tutorial.md` & `ocean-model-skill-assessor-0.7.1/docs/cli_tutorial.md`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/conf.py` & `ocean-model-skill-assessor-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/demo.ipynb` & `ocean-model-skill-assessor-0.7.1/docs/demo.ipynb`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/demo_cli.ipynb` & `ocean-model-skill-assessor-0.7.1/docs/demo_cli.ipynb`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/developer.md` & `ocean-model-skill-assessor-0.7.1/docs/developer.md`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/environment.yml` & `ocean-model-skill-assessor-0.7.1/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/examples/ciofs.ipynb` & `ocean-model-skill-assessor-0.7.1/docs/examples/ciofs.ipynb`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/examples/gom_hycom.ipynb` & `ocean-model-skill-assessor-0.7.1/docs/examples/gom_hycom.ipynb`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/examples/tbofs.ipynb` & `ocean-model-skill-assessor-0.7.1/docs/examples/tbofs.ipynb`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/index.rst` & `ocean-model-skill-assessor-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/vocab_widget.html` & `ocean-model-skill-assessor-0.7.1/docs/vocab_widget.html`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/docs/vocab_widget.ipynb` & `ocean-model-skill-assessor-0.7.1/docs/vocab_widget.ipynb`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/environment.yml` & `ocean-model-skill-assessor-0.7.1/environment.yml`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/CLI.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/CLI.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/__init__.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/__init__.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/accessor.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/accessor.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/main.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/main.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/paths.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/paths.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/plot/map.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/plot/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,24 +219,24 @@
             edgecolor="r",
             linestyle="-",
             linewidth=linewidth_poly,
         )
     else:
         bbox = [min(min_lons), min(min_lats), max(max_lons), max(max_lats)]
 
-    kwargs_plot = {}
+    kwargs_plot: Dict[str, Union[str, list]] = {}
 
     # plot stations
     inds = (min_lons == max_lons) | (types == "point")
     if inds.sum() > 0:
         if legend:
             kwargs_plot["label"] = list(station_names[inds])
+            assert isinstance(colors_data, list)
             ax.set_prop_cycle(color=colors_data)
         else:
-            assert isinstance(colors_data, list)
             kwargs_plot["color"] = colors_data
         # # import pdb; pdb.set_trace()
         # ax.scatter(
         #      min_lons[inds][:,np.newaxis],
         #     # min_lons[inds],
         #      min_lats[inds][:,np.newaxis],
         #     # min_lats[inds],
@@ -267,15 +267,14 @@
     # plot lines
     inds = types == "line"
     if inds.sum() > 0:
         if legend:
             kwargs_plot["label"] = list(station_names[inds])
             ax.set_prop_cycle(color=colors_data)
         else:
-            assert isinstance(colors_data, list)
             kwargs_plot["color"] = colors_data  # [inds]
         ax.plot(
             [min_lons[inds], max_lons[inds]],
             [min_lats[inds], max_lats[inds]],
             linestyle="-",
             linewidth=linewidth_data,
             transform=pc,
@@ -285,15 +284,14 @@
     # plot boxes
     inds = types == "box"
     if inds.sum() > 0:
         if legend:
             kwargs_plot["label"] = list(station_names[inds])
             ax.set_prop_cycle(color=colors_data)
         else:
-            assert isinstance(colors_data, list)
             kwargs_plot["color"] = colors_data  # [inds]
         ax.plot(
             [
                 min_lons[inds],
                 max_lons[inds],
                 max_lons[inds],
                 min_lons[inds],
```

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/plot/time_series.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/plot/time_series.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/stats.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/stats.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/utils.py` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/utils.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/erddap_coastwatch.json` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/erddap_coastwatch.json`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/erddap_ioos.json` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/erddap_ioos.json`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/general.json` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/general.json`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor/vocab/standard_names.json` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor/vocab/standard_names.json`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/PKG-INFO` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-model-skill-assessor
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package to fully run the comparison between data and model to assess model skill.
 Home-page: https://github.com/axiom-data-science/ocean-model-skill-assessor
 Author: Axiom Data Science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `ocean-model-skill-assessor-0.7.0/ocean_model_skill_assessor.egg-info/SOURCES.txt` & `ocean-model-skill-assessor-0.7.1/ocean_model_skill_assessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/pyproject.toml` & `ocean-model-skill-assessor-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/setup.cfg` & `ocean-model-skill-assessor-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/tests/test_main.py` & `ocean-model-skill-assessor-0.7.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/tests/test_main_axds.py` & `ocean-model-skill-assessor-0.7.1/tests/test_main_axds.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/tests/test_main_local.py` & `ocean-model-skill-assessor-0.7.1/tests/test_main_local.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/tests/test_plot.py` & `ocean-model-skill-assessor-0.7.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/tests/test_stats.py` & `ocean-model-skill-assessor-0.7.1/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `ocean-model-skill-assessor-0.7.0/tests/test_utils.py` & `ocean-model-skill-assessor-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

