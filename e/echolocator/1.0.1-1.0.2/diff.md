# Comparing `tmp/echolocator-1.0.1.tar.gz` & `tmp/echolocator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echolocator-1.0.1.tar", last modified: Tue Apr 25 05:07:33 2023, max compression
+gzip compressed data, was "echolocator-1.0.2.tar", last modified: Wed Apr 26 08:01:54 2023, max compression
```

## Comparing `echolocator-1.0.1.tar` & `echolocator-1.0.2.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.023209 echolocator-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.999209 echolocator-1.0.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.999209 echolocator-1.0.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-25 05:07:24.000000 echolocator-1.0.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-25 05:07:24.000000 echolocator-1.0.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.983209 echolocator-1.0.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 05:07:24.000000 echolocator-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-25 05:07:24.000000 echolocator-1.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-25 05:07:24.000000 echolocator-1.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 05:07:24.000000 echolocator-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-25 05:07:24.000000 echolocator-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-25 05:07:33.023209 echolocator-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-25 05:07:24.000000 echolocator-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 05:07:24.000000 echolocator-1.0.1/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/1_tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/1_tutorials/101_run_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/1_tutorials/102_update_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/1_tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/2_how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/2_how-to/201_add_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/2_how-to.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/3_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/3_explanations/301_naming_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/3_explanations/302_process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/3_explanations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/4_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/4_reference/402_building_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/4_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/image_details.png
--rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/image_list.png
--rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/swiss3.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/modulefiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-25 05:07:24.000000 echolocator-1.0.1/modulefiles/conda
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 05:07:24.000000 echolocator-1.0.1/modulefiles/paths
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-25 05:07:24.000000 echolocator-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 05:07:33.023209 echolocator-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.987209 echolocator-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_lib/composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/composers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/image_edit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/image_list_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/pixel_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/common/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/events.js
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/runtime.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.html
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.js
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.023209 echolocator-1.0.1/tests/example_images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.023209 echolocator-1.0.1/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_fetch_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_fetch_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.932341 echolocator-1.0.2/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-26 08:01:44.000000 echolocator-1.0.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-26 08:01:44.000000 echolocator-1.0.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.924341 echolocator-1.0.2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-26 08:01:44.000000 echolocator-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-26 08:01:44.000000 echolocator-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 08:01:44.000000 echolocator-1.0.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 08:01:44.000000 echolocator-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-26 08:01:44.000000 echolocator-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-26 08:01:54.968341 echolocator-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 08:01:44.000000 echolocator-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-26 08:01:44.000000 echolocator-1.0.2/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/1_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/1_tutorials/101_run_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/1_tutorials/102_update_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/1_tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/2_how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/2_how-to/201_add_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/2_how-to.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/3_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/3_explanations/301_naming_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/3_explanations/302_process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/3_explanations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/4_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/4_reference/402_building_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/4_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/excalidraw-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/git_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/image_details.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/image_list.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/swiss3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/modulefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-26 08:01:44.000000 echolocator-1.0.2/modulefiles/conda
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 08:01:44.000000 echolocator-1.0.2/modulefiles/paths
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-26 08:01:44.000000 echolocator-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:01:54.968341 echolocator-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/src/echolocator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/src/echolocator_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/src/echolocator_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_lib/composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/image_edit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/image_list_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/pixel_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/common/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.960341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.960341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/box/
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/chart_area/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/histogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/image_area/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/sprite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/example_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_fetch_images.py
```

### Comparing `echolocator-1.0.1/.dae-devops/Makefile` & `echolocator-1.0.2/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.dae-devops/docs/conventions.rst` & `echolocator-1.0.2/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.dae-devops/docs/developing.rst` & `echolocator-1.0.2/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.dae-devops/docs/devops.rst` & `echolocator-1.0.2/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.dae-devops/docs/docs_structure.rst` & `echolocator-1.0.2/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.dae-devops/docs/installing.rst` & `echolocator-1.0.2/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.dae-devops/docs/testing.rst` & `echolocator-1.0.2/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.dae-devops/project.yaml` & `echolocator-1.0.2/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.devcontainer/Dockerfile` & `echolocator-1.0.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.devcontainer/devcontainer.json` & `echolocator-1.0.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/CONTRIBUTING.rst` & `echolocator-1.0.2/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/actions/install_requirements/action.yml` & `echolocator-1.0.2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/dependabot.yml` & `echolocator-1.0.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/pages/make_switcher.py` & `echolocator-1.0.2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/workflows/code.yml` & `echolocator-1.0.2/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/workflows/docs.yml` & `echolocator-1.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/workflows/docs_clean.yml` & `echolocator-1.0.2/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.github/workflows/linkcheck.yml` & `echolocator-1.0.2/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.gitignore` & `echolocator-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.gitlab-ci.yml` & `echolocator-1.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/.vscode/launch.json` & `echolocator-1.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/LICENSE` & `echolocator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/Makefile` & `echolocator-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/PKG-INFO` & `echolocator-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.0.1
+Version: 1.0.2
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.0.1/README.rst` & `echolocator-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/configurations/development.yaml` & `echolocator-1.0.2/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/1_tutorials/101_run_conda.rst` & `echolocator-1.0.2/docs/1_tutorials/101_run_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/1_tutorials/102_update_image.rst` & `echolocator-1.0.2/docs/1_tutorials/102_update_image.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/2_how-to/201_add_fields.rst` & `echolocator-1.0.2/docs/2_how-to/201_add_fields.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/3_explanations/301_naming_conventions.rst` & `echolocator-1.0.2/docs/3_explanations/301_naming_conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/3_explanations/302_process.rst` & `echolocator-1.0.2/docs/3_explanations/302_process.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/4_reference/402_building_conda.rst` & `echolocator-1.0.2/docs/4_reference/402_building_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/_static/theme_overrides.css` & `echolocator-1.0.2/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/conf.py` & `echolocator-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/images/dls-favicon.ico` & `echolocator-1.0.2/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/images/dls-logo.svg` & `echolocator-1.0.2/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/images/excalidraw-example.svg` & `echolocator-1.0.2/docs/images/excalidraw-example.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/images/git_merge.png` & `echolocator-1.0.2/docs/images/git_merge.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/images/image_details.png` & `echolocator-1.0.2/docs/images/image_details.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/images/image_list.png` & `echolocator-1.0.2/docs/images/image_list.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/docs/images/swiss3.png` & `echolocator-1.0.2/docs/images/swiss3.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/modulefiles/conda` & `echolocator-1.0.2/modulefiles/conda`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/pyproject.toml` & `echolocator-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator.egg-info/PKG-INFO` & `echolocator-1.0.2/src/echolocator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.0.1
+Version: 1.0.2
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.0.1/src/echolocator.egg-info/SOURCES.txt` & `echolocator-1.0.2/src/echolocator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_api/context_base.py` & `echolocator-1.0.2/src/echolocator_api/context_base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_api/databases/constants.py` & `echolocator-1.0.2/src/echolocator_api/databases/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_api/exceptions.py` & `echolocator-1.0.2/src/echolocator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_api/guis/aiohttp.py` & `echolocator-1.0.2/src/echolocator_api/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_api/guis/context.py` & `echolocator-1.0.2/src/echolocator_api/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_api/guis/guis.py` & `echolocator-1.0.2/src/echolocator_api/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_cli/main.py` & `echolocator-1.0.2/src/echolocator_cli/main.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_cli/subcommands/base.py` & `echolocator-1.0.2/src/echolocator_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_cli/subcommands/service.py` & `echolocator-1.0.2/src/echolocator_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_cli/version.py` & `echolocator-1.0.2/src/echolocator_cli/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/__main__.py` & `echolocator-1.0.2/src/echolocator_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/composers/composers.py` & `echolocator-1.0.2/src/echolocator_lib/composers/composers.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/composers/html.py` & `echolocator-1.0.2/src/echolocator_lib/composers/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             {"text": "uuid", "class": "T_uuid"},
             {"text": "well", "class": "T_well"},
             {"text": "#Crystals", "class": "T_number_of_crystals"},
             {"text": "Offset x (\u03BCm)", "class": "T_real_space_target_x"},
             {"text": "Offset y (\u03BCm)", "class": "T_real_space_target_y"},
             {"text": "drop", "class": "T_is_drop"},
             {"text": "well centroid x,y", "class": "T_well_centroid_x_y"},
-            {"text": "auto x,y", "class": "T_auto_target__x_y"},
+            {"text": "auto x,y", "class": "T_auto_target_x_y"},
             {"text": "confirmed x,y", "class": "T_confirmed_target_x_y"},
             {"text": "echo coordinate x,y", "class": "T_echo_coordinate_x_y"},
             {"text": "use", "class": "T_is_usable"},
             {"text": "error", "class": "T_error"},
         ]
 
         html_lines = []
@@ -124,18 +124,24 @@
                 t = "-"
             elif t:
                 t = "yes"
             else:
                 t = "no"
             html_lines.append("<td class='T_is_drop'>" + str(t) + "</td>")
 
-            t = f"{model.well_centroid_x}, {model.well_centroid_y}"
+            if model.well_centroid_x is None or model.well_centroid_y is None:
+                t = "-"
+            else:
+                t = f"{model.well_centroid_x}, {model.well_centroid_y}"
             html_lines.append("<td class='T_well_centroid_x_y'>" + t + "</td>")
 
-            t = f"{model.auto_target_x}, {model.auto_target_y}"
+            if model.auto_target_x is None or model.auto_target_y is None:
+                t = "-"
+            else:
+                t = f"{model.auto_target_x}, {model.auto_target_y}"
             html_lines.append("<td class='T_auto_target_x_y'>" + t + "</td>")
 
             if model.confirmed_target_x is None or model.confirmed_target_y is None:
                 t = "-"
             else:
                 t = f"{model.confirmed_target_x}, {model.confirmed_target_y}"
             html_lines.append("<td class='T_confirmed_target_x_y'>" + t + "</td>")
```

### Comparing `echolocator-1.0.1/src/echolocator_lib/composers/prettyhelper.py` & `echolocator-1.0.2/src/echolocator_lib/composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/composers/text.py` & `echolocator-1.0.2/src/echolocator_lib/composers/text.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/contexts/base.py` & `echolocator-1.0.2/src/echolocator_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/envvar.py` & `echolocator-1.0.2/src/echolocator_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/aiohttp.py` & `echolocator-1.0.2/src/echolocator_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/constants.py` & `echolocator-1.0.2/src/echolocator_lib/guis/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/context.py` & `echolocator-1.0.2/src/echolocator_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/guis.py` & `echolocator-1.0.2/src/echolocator_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/css/image_list_ux.css` & `echolocator-1.0.2/src/echolocator_lib/guis/html/css/image_list_ux.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/css/styles.css` & `echolocator-1.0.2/src/echolocator_lib/guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/images/radial1.666.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/index.html` & `echolocator-1.0.2/src/echolocator_lib/guis/html/index.html`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/index.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/index.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/common/base.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/common/base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/events.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/events.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/spreader.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/transformer.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.html` & `echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.html`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.js` & `echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/src/echolocator_lib/version.py` & `echolocator-1.0.2/src/echolocator_lib/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/base.py` & `echolocator-1.0.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/configurations/service.yaml` & `echolocator-1.0.2/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/conftest.py` & `echolocator-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/example_images/1.jpg` & `echolocator-1.0.2/tests/example_images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/example_images/2.jpg` & `echolocator-1.0.2/tests/example_images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/example_images/3.jpg` & `echolocator-1.0.2/tests/example_images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/example_images/4.png` & `echolocator-1.0.2/tests/example_images/4.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/images/1.jpg` & `echolocator-1.0.2/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/images/2.jpg` & `echolocator-1.0.2/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/images/3.jpg` & `echolocator-1.0.2/tests/images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/test_droplocation.py` & `echolocator-1.0.2/tests/test_droplocation.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/test_export.py` & `echolocator-1.0.2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/test_fetch_image.py` & `echolocator-1.0.2/tests/test_fetch_image.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.1/tests/test_fetch_images.py` & `echolocator-1.0.2/tests/test_fetch_images.py`

 * *Files identical despite different names*

