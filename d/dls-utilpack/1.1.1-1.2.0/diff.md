# Comparing `tmp/dls-utilpack-1.1.1.tar.gz` & `tmp/dls-utilpack-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-utilpack-1.1.1.tar", last modified: Thu Apr 20 13:51:39 2023, max compression
+gzip compressed data, was "dls-utilpack-1.2.0.tar", last modified: Wed Apr 26 07:55:28 2023, max compression
```

## Comparing `dls-utilpack-1.1.1.tar` & `dls-utilpack-1.2.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.805884 dls-utilpack-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.789884 dls-utilpack-1.1.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.785884 dls-utilpack-1.1.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-20 13:51:39.805884 dls-utilpack-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.793885 dls-utilpack-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.789884 dls-utilpack-1.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.797885 dls-utilpack-1.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.797885 dls-utilpack-1.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.797885 dls-utilpack-1.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:51:39.805884 dls-utilpack-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.789884 dls-utilpack-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.801885 dls-utilpack-1.1.1/src/dls_utilpack/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 13:51:39.000000 dls-utilpack-1.1.1/src/dls_utilpack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/global_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/isodatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/modify_process_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/qualname.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/require.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/search_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/things.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/visit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/src/dls_utilpack/whatenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.801885 dls-utilpack-1.1.1/src/dls_utilpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-20 13:51:39.000000 dls-utilpack-1.1.1/src/dls_utilpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-20 13:51:39.000000 dls-utilpack-1.1.1/src/dls_utilpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:51:39.000000 dls-utilpack-1.1.1/src/dls_utilpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 13:51:39.000000 dls-utilpack-1.1.1/src/dls_utilpack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-20 13:51:39.000000 dls-utilpack-1.1.1/src/dls_utilpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 13:51:39.000000 dls-utilpack-1.1.1/src/dls_utilpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.805884 dls-utilpack-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:51:39.805884 dls-utilpack-1.1.1/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_sigint1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_sigint2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_visit.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-20 13:51:26.000000 dls-utilpack-1.1.1/tests/test_whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.701139 dls-utilpack-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.697139 dls-utilpack-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.697139 dls-utilpack-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-26 07:55:28.701139 dls-utilpack-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.697139 dls-utilpack-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.697139 dls-utilpack-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.697139 dls-utilpack-1.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.697139 dls-utilpack-1.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:55:28.701139 dls-utilpack-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.693139 dls-utilpack-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.701139 dls-utilpack-1.2.0/src/dls_utilpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 07:55:28.000000 dls-utilpack-1.2.0/src/dls_utilpack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/global_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/isodatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/modify_process_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/qualname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/require.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/search_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/src/dls_utilpack/whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.701139 dls-utilpack-1.2.0/src/dls_utilpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-04-26 07:55:28.000000 dls-utilpack-1.2.0/src/dls_utilpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-26 07:55:28.000000 dls-utilpack-1.2.0/src/dls_utilpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:55:28.000000 dls-utilpack-1.2.0/src/dls_utilpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 07:55:28.000000 dls-utilpack-1.2.0/src/dls_utilpack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-26 07:55:28.000000 dls-utilpack-1.2.0/src/dls_utilpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 07:55:28.000000 dls-utilpack-1.2.0/src/dls_utilpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.701139 dls-utilpack-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:55:28.701139 dls-utilpack-1.2.0/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_sigint1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_sigint2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 07:55:20.000000 dls-utilpack-1.2.0/tests/test_whatenv.py
```

### Comparing `dls-utilpack-1.1.1/.dae-devops/Makefile` & `dls-utilpack-1.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.dae-devops/docs/conventions.rst` & `dls-utilpack-1.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.dae-devops/docs/developing.rst` & `dls-utilpack-1.2.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.dae-devops/docs/devops.rst` & `dls-utilpack-1.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.dae-devops/docs/docs_structure.rst` & `dls-utilpack-1.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.dae-devops/docs/installing.rst` & `dls-utilpack-1.2.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.dae-devops/docs/testing.rst` & `dls-utilpack-1.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.dae-devops/project.yaml` & `dls-utilpack-1.2.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.devcontainer/Dockerfile` & `dls-utilpack-1.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.devcontainer/devcontainer.json` & `dls-utilpack-1.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/CONTRIBUTING.rst` & `dls-utilpack-1.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/actions/install_requirements/action.yml` & `dls-utilpack-1.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/dependabot.yml` & `dls-utilpack-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/pages/make_switcher.py` & `dls-utilpack-1.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/workflows/code.yml` & `dls-utilpack-1.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/workflows/docs.yml` & `dls-utilpack-1.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/workflows/docs_clean.yml` & `dls-utilpack-1.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.github/workflows/linkcheck.yml` & `dls-utilpack-1.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.gitignore` & `dls-utilpack-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.gitlab-ci.yml` & `dls-utilpack-1.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/.vscode/launch.json` & `dls-utilpack-1.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/LICENSE` & `dls-utilpack-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/LICENSE.txt` & `dls-utilpack-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/Makefile` & `dls-utilpack-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/PKG-INFO` & `dls-utilpack-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.1.1
+Version: 1.2.0
 Summary: Collection of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-utilpack-1.1.1/README.rst` & `dls-utilpack-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/docs/api/modules.rst` & `dls-utilpack-1.2.0/docs/api/modules.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/docs/conf.py` & `dls-utilpack-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/docs/images/dls-favicon.ico` & `dls-utilpack-1.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/docs/images/dls-logo.svg` & `dls-utilpack-1.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/pyproject.toml` & `dls-utilpack-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/__main__.py` & `dls-utilpack-1.2.0/src/dls_utilpack/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/bash_composer.py` & `dls-utilpack-1.2.0/src/dls_utilpack/bash_composer.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/callsign.py` & `dls-utilpack-1.2.0/src/dls_utilpack/callsign.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/datatypes.py` & `dls-utilpack-1.2.0/src/dls_utilpack/datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/describe.py` & `dls-utilpack-1.2.0/src/dls_utilpack/describe.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/envvar.py` & `dls-utilpack-1.2.0/src/dls_utilpack/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/explain.py` & `dls-utilpack-1.2.0/src/dls_utilpack/explain.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/hazzathread.py` & `dls-utilpack-1.2.0/src/dls_utilpack/hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/ignore.py` & `dls-utilpack-1.2.0/src/dls_utilpack/ignore.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/import_class.py` & `dls-utilpack-1.2.0/src/dls_utilpack/import_class.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/module.py` & `dls-utilpack-1.2.0/src/dls_utilpack/module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/require.py` & `dls-utilpack-1.2.0/src/dls_utilpack/require.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/sanitize.py` & `dls-utilpack-1.2.0/src/dls_utilpack/sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/search_file.py` & `dls-utilpack-1.2.0/src/dls_utilpack/search_file.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/signal.py` & `dls-utilpack-1.2.0/src/dls_utilpack/signal.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/substitute.py` & `dls-utilpack-1.2.0/src/dls_utilpack/substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/thing.py` & `dls-utilpack-1.2.0/src/dls_utilpack/thing.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/things.py` & `dls-utilpack-1.2.0/src/dls_utilpack/things.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/version.py` & `dls-utilpack-1.2.0/src/dls_utilpack/version.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/visit.py` & `dls-utilpack-1.2.0/src/dls_utilpack/visit.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,10 +59,10 @@
 def get_xchem_directory(parent, visit):
 
     subdirectory = get_xchem_subdirectory(visit)
 
     full_path = Path(parent) / subdirectory
 
     if not full_path.is_dir():
-        raise RuntimeError(f"the visit directory {str(full_path)} does not exist")
+        raise VisitNotFound(f"the visit directory {str(full_path)} does not exist")
 
     return str(full_path)
```

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack/whatenv.py` & `dls-utilpack-1.2.0/src/dls_utilpack/whatenv.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack.egg-info/PKG-INFO` & `dls-utilpack-1.2.0/src/dls_utilpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.1.1
+Version: 1.2.0
 Summary: Collection of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-utilpack-1.1.1/src/dls_utilpack.egg-info/SOURCES.txt` & `dls-utilpack-1.2.0/src/dls_utilpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/base.py` & `dls-utilpack-1.2.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/base_tester.py` & `dls-utilpack-1.2.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/conftest.py` & `dls-utilpack-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_bash_composer.py` & `dls-utilpack-1.2.0/tests/test_bash_composer.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_callsign.py` & `dls-utilpack-1.2.0/tests/test_callsign.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_datatypes.py` & `dls-utilpack-1.2.0/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_hazzathread.py` & `dls-utilpack-1.2.0/tests/test_hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_import.py` & `dls-utilpack-1.2.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_module.py` & `dls-utilpack-1.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_sanitize.py` & `dls-utilpack-1.2.0/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_sigint1.py` & `dls-utilpack-1.2.0/tests/test_sigint1.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_sigint2.py` & `dls-utilpack-1.2.0/tests/test_sigint2.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_substitute.py` & `dls-utilpack-1.2.0/tests/test_substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.1.1/tests/test_visit.py` & `dls-utilpack-1.2.0/tests/test_visit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 from pathlib import Path
 
 import pytest
 
-from dls_utilpack.visit import get_xchem_directory, get_xchem_subdirectory
+from dls_utilpack.visit import (
+    VisitNotFound,
+    get_xchem_directory,
+    get_xchem_subdirectory,
+)
 
 # Base class for the tester.
 from tests.base_tester import BaseTester
 
 logger = logging.getLogger(__name__)
 
 
@@ -55,10 +59,10 @@
         parent = Path(output_directory) / "processing/lab36"
         full_path = parent / "aa12345/aa12345-1"
         full_path.mkdir(parents=True, exist_ok=True)
 
         assert get_xchem_directory(str(parent), "aa12345-1") == str(full_path)
 
         # Check invalid directory.
-        with pytest.raises(RuntimeError) as excinfo:
+        with pytest.raises(VisitNotFound) as excinfo:
             get_xchem_directory("something", "aa12345-1")
         assert "does not exist" in str(excinfo.value)
```

### Comparing `dls-utilpack-1.1.1/tests/test_whatenv.py` & `dls-utilpack-1.2.0/tests/test_whatenv.py`

 * *Files identical despite different names*

