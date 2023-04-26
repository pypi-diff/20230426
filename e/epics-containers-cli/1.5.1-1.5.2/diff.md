# Comparing `tmp/epics-containers-cli-1.5.1.tar.gz` & `tmp/epics-containers-cli-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epics-containers-cli-1.5.1.tar", last modified: Fri Apr 21 13:39:45 2023, max compression
+gzip compressed data, was "epics-containers-cli-1.5.2.tar", last modified: Wed Apr 26 11:40:29 2023, max compression
```

## Comparing `epics-containers-cli-1.5.1.tar` & `epics-containers-cli-1.5.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.856371 epics-containers-cli-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.844371 epics-containers-cli-1.5.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-21 13:39:45.856371 epics-containers-cli-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/tutorials/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    11156 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/get_helm.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:39:45.856371 epics-containers-cli-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/src/epics_containers_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.595972 epics-containers-cli-1.5.2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.599972 epics-containers-cli-1.5.2/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/docs/user/tutorials/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11156 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/get_helm.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.595972 epics-containers-cli-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/src/epics_containers_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 11:40:29.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/cmd_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/cmd_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/src/epics_containers_cli/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-26 11:40:29.000000 epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-26 11:40:29.000000 epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:40:29.000000 epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-26 11:40:29.000000 epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 11:40:29.000000 epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 11:40:29.000000 epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:40:29.603972 epics-containers-cli-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 11:40:21.000000 epics-containers-cli-1.5.2/tests/test_cli.py
```

### Comparing `epics-containers-cli-1.5.1/.devcontainer/devcontainer.json` & `epics-containers-cli-1.5.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/CONTRIBUTING.rst` & `epics-containers-cli-1.5.2/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/actions/install_requirements/action.yml` & `epics-containers-cli-1.5.2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/dependabot.yml` & `epics-containers-cli-1.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/pages/make_switcher.py` & `epics-containers-cli-1.5.2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/workflows/code.yml` & `epics-containers-cli-1.5.2/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/workflows/docs.yml` & `epics-containers-cli-1.5.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/workflows/docs_clean.yml` & `epics-containers-cli-1.5.2/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.github/workflows/linkcheck.yml` & `epics-containers-cli-1.5.2/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.gitignore` & `epics-containers-cli-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/.vscode/launch.json` & `epics-containers-cli-1.5.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/Dockerfile` & `epics-containers-cli-1.5.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/LICENSE` & `epics-containers-cli-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/PKG-INFO` & `epics-containers-cli-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epics-containers-cli
-Version: 1.5.1
+Version: 1.5.2
 Summary: One line description of your module
 Author-email: Giles Knap <giles.knap@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `epics-containers-cli-1.5.1/README.rst` & `epics-containers-cli-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/conf.py` & `epics-containers-cli-1.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `epics-containers-cli-1.5.2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/explanations/decisions.rst` & `epics-containers-cli-1.5.2/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/how-to/build-docs.rst` & `epics-containers-cli-1.5.2/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/how-to/lint.rst` & `epics-containers-cli-1.5.2/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/how-to/make-release.rst` & `epics-containers-cli-1.5.2/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/how-to/pin-requirements.rst` & `epics-containers-cli-1.5.2/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/how-to/test-container.rst` & `epics-containers-cli-1.5.2/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/how-to/update-tools.rst` & `epics-containers-cli-1.5.2/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/index.rst` & `epics-containers-cli-1.5.2/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/reference/standards.rst` & `epics-containers-cli-1.5.2/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/developer/tutorials/dev-install.rst` & `epics-containers-cli-1.5.2/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/images/dls-favicon.ico` & `epics-containers-cli-1.5.2/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/images/dls-logo.svg` & `epics-containers-cli-1.5.2/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/index.rst` & `epics-containers-cli-1.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/user/explanations/docs-structure.rst` & `epics-containers-cli-1.5.2/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/user/index.rst` & `epics-containers-cli-1.5.2/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/docs/user/tutorials/installation.rst` & `epics-containers-cli-1.5.2/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/get_helm.sh` & `epics-containers-cli-1.5.2/get_helm.sh`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/pyproject.toml` & `epics-containers-cli-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli/__main__.py` & `epics-containers-cli-1.5.2/src/epics_containers_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_dev.py` & `epics-containers-cli-1.5.2/src/epics_containers_cli/cmd_dev.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import shutil
 from os import environ
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from .context import Context
@@ -19,30 +20,31 @@
 REPOS = f" -v {REPOS_FOLDER}:/repos "
 OPTS = "--security-opt=label=type:container_runtime_t --net=host"
 
 
 def all_params():
     env = "-e DISPLAY -e USER -e SHELL"
     volumes = (
-        " -v=/tmp:/tmp"
         " -v=/home/$USER:/home/$USER"
-        " -v=/home/$USER/.bashrc_dev:/root/.bashrc"
-        " -v=/home/$USER/.inputrc:/root/.inputrc"
-        " -v=/home/$USER/.bash_history:/root/.bash_history"
+        " -v=/home/$USER/.bashrc_dev_container:/root/.bashrc"
+        " -v=/home/$USER/.inputrc_container:/root/.inputrc"
+        " -v=/home/$USER/.bash_eternal_history:/root/.bash_eternal_history"
     )
 
-    # To make containers in containers nice we need to have some consitency
+    # To make containers in containers nice we need to have some consistency
     # with prompt and history - but we need to get files for that from the
-    # host filesystem - hence this slightly ugly check:
-    for f in [".bashrc_dev", ".inputrc", ".bash_history"]:
-        p = Path("/home") / environ.get("USER") / f
-        if not p.exists():
-            raise RuntimeError(
-                f"Missing file {p}, please copy from .devcontainer or create your own"
-            )
+    # host filesystem - hence this slightly ugly logic:
+
+    # copy this container's shell config into the host user's home folder
+    # so they can be mounted into the new container
+    user = environ["USER"]
+    shutil.copyfile("/root/.inputrc", f"/home/{user}/.inputrc_container")
+    shutil.copyfile("/root/.bashrc", f"/home/{user}/.bashrc_dev_container")
+    # make sure .bash_eternal_history exists
+    Path(f"/home/{user}/.bash_eternal_history").touch()
 
     return f"{env} {volumes} {OPTS}"
 
 
 def prepare(folder: Path, arch: Architecture = Architecture.linux):
     """
     Prepare a generic IOC project folder for launching
@@ -109,77 +111,74 @@
     )
 
 
 @dev.command()
 def ioc_launch(
     ctx: typer.Context,
     helm_chart: Path = typer.Argument(..., help="root folder of local IOC helm chart"),
-    folder: Path = typer.Argument(".", help="folder for generic IOC project"),
-    tag: str = typer.Option(IMAGE_TAG, help="version of the generic IOC to use"),
+    folder: Path = typer.Argument(None, help="folder for generic IOC project"),
     debug: bool = typer.Option(False, help="start a remote debug session"),
 ):
     """Launch an IOC instance using a local helm chart definition.
     Set folder for a locally editable generic IOC or supply a tag to choose any
     version from the registry."""
 
-    if tag == IMAGE_TAG and folder is None:
-        print(
-            "You must specify a version tag for the generic IOC\n"
-            "or a folder with a local clone of the generic IOC project"
-        )
-        raise (typer.Exit(1))
-
     ioc_name, image = get_helm_chart(helm_chart)
-    # switch to the developer target and requested tag for generic IOC image
-    image = re.findall(r"[^:]*", image)[0].replace("runtime", "developer") + f":{tag}"
+    # switch to the developer target and separate the tag for generic IOC image
+    match = re.match(r"([^:]*):(.*)$", image)
+    if match is None:
+        raise ValueError(f"invalid image name in {helm_chart}")
+
+    image = match.group(1).replace("runtime", "developer")
+    org_tag = match.group(2)
 
     # work out which architecture to use for prepare
     arch = Architecture.rtems if "rtems" in image else Architecture.linux
 
     # make sure there are not 2 copies running
     run_command(f"podman rm -f {ioc_name}", show_cmd=True)
 
     helm_chart = helm_chart.absolute()
     start_script = "/repos/epics/ioc/start.sh"
     config_folder = "/repos/epics/ioc/config"
     config = f'-v {helm_chart / "config"}:{config_folder}'
 
-    if tag != IMAGE_TAG:
-        # launch the requested version of the generic IOC only
+    if folder is None:
+        # launch generic IOC from the registry with tag specified in helm chart
         run_command(
             f"podman run --rm -it --name {ioc_name} {config} {all_params()}"
-            f" {image} bash {start_script}",
+            f" {image}:{org_tag} bash {start_script}",
             show_cmd=True,
             interactive=True,
         )
     else:
         # launch the local work version of the generic IOC with locally mounted
         # /repos folder - useful for testing changes to repos folder
         repos = REPOS.format(folder=folder.absolute())
 
         folder_image = prepare(folder, arch)
 
-        if folder_image != image:
+        if folder_image != f"{image}:local":
             print(
                 f"""
 ERROR: the specified Generic IOC image: {folder_image}
-does not match the helm chart image: {image}
+does not match the helm chart image: {image}:{org_tag}
 you must specify a folder for the local generic IOC project
 or a tag for the generic IOC image to use from the registry"""
             )
             raise (typer.Exit(1))
 
         command = (
             f"bash {start_script}; "
             f"echo IOC EXITED - hit ctrl D to leave IOC container; "
             f"bash"
         )
         run_command(
             f"podman run -it --name {ioc_name} {repos} {config} {all_params()}"
-            f" {image} bash -c '{command}'",
+            f" {folder_image} bash -c '{command}'",
             show_cmd=True,
             interactive=True,
         )
 
     # TODO look into debugging
```

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_ioc.py` & `epics-containers-cli-1.5.2/src/epics_containers_cli/cmd_ioc.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli/kubectl.py` & `epics-containers-cli-1.5.2/src/epics_containers_cli/kubectl.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli/logging.py` & `epics-containers-cli-1.5.2/src/epics_containers_cli/logging.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli/shell.py` & `epics-containers-cli-1.5.2/src/epics_containers_cli/shell.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/PKG-INFO` & `epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epics-containers-cli
-Version: 1.5.1
+Version: 1.5.2
 Summary: One line description of your module
 Author-email: Giles Knap <giles.knap@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/SOURCES.txt` & `epics-containers-cli-1.5.2/src/epics_containers_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

