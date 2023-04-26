# Comparing `tmp/pydantic-kedro-0.1.1.tar.gz` & `tmp/pydantic-kedro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.1.1.tar", last modified: Thu Mar 30 11:06:31 2023, max compression
+gzip compressed data, was "pydantic-kedro-0.1.2.tar", last modified: Wed Apr 26 16:29:31 2023, max compression
```

## Comparing `pydantic-kedro-0.1.1.tar` & `pydantic-kedro-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.320063 pydantic-kedro-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.312063 pydantic-kedro-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.312063 pydantic-kedro-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-03-30 11:06:31.320063 pydantic-kedro-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.312063 pydantic-kedro-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.312063 pydantic-kedro-0.1.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 11:06:31.320063 pydantic-kedro-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.312063 pydantic-kedro-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.316064 pydantic-kedro-0.1.1/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.316064 pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.316064 pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-03-30 11:06:31.000000 pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-30 11:06:31.000000 pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:06:31.000000 pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:05:30.000000 pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-30 11:06:31.000000 pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 11:06:31.000000 pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.316064 pydantic-kedro-0.1.1/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.316064 pydantic-kedro-0.1.1/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.312063 pydantic-kedro-0.1.1/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.316064 pydantic-kedro-0.1.1/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.320063 pydantic-kedro-0.1.1/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:06:31.320063 pydantic-kedro-0.1.1/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-30 11:05:17.000000 pydantic-kedro-0.1.1/src/test/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.447972 pydantic-kedro-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:28:41.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.447972 pydantic-kedro-0.1.2/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_import.py
```

### Comparing `pydantic-kedro-0.1.1/.github/dependabot.yml` & `pydantic-kedro-0.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.1/.github/workflows/python-publish.yml` & `pydantic-kedro-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.1/.pre-commit-config.yaml` & `pydantic-kedro-0.1.2/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -9,44 +9,43 @@
         args: ["--maxkb=1024"]
         # 1 MB - Don't commit notebooks with output!
       - id: trailing-whitespace
       - id: check-yaml
       - id: check-toml
       - id: end-of-file-fixer
       - id: detect-private-key
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    # Ruff version.
+    rev: "v0.0.263"
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pycqa/isort
     rev: "5.12.0"
     hooks:
       - id: isort
         name: isort (python)
   - repo: https://github.com/psf/black
     # docs: https://black.readthedocs.io/en/stable/integrations/source_version_control.html
-    rev: "22.6.0"
+    rev: "23.3.0"
     hooks:
       - id: black
     # consider also black-jupyter
-  - repo: https://github.com/pycqa/flake8
-    # docs: https://flake8.pycqa.org/en/latest/user/using-hooks.html?highlight=commit
-    rev: "5.0.4"
-    hooks:
-      - id: flake8
-        additional_dependencies: [flake8-pyproject]
-  # - repo: https://github.com/john-hen/flake8-pyproject
-  #   # alternate to above, however it should work with flake8-pyproject as an additional dep
-  #   rev: "1.0.1"
-  #   hooks:
-  #     - id: flake8-pyproject
   - repo: https://github.com/pre-commit/mirrors-mypy
     # NOTE: This passes ALL files to `mypy`. mypy will cache these.
     # However, we must ignore all missing imports, because pre-commit runs in a separate env
-    rev: "v1.0.0"
+    rev: "v1.2.0"
     hooks:
       - id: mypy
         pass_filenames: false
         args: [--config-file, pyproject.toml, --ignore-missing-imports]
+  - repo: https://github.com/DavidAnson/markdownlint-cli2
+    rev: v0.7.0
+    hooks:
+      - id: markdownlint-cli2
   # SEE: https://pre-commit.com/#repository-local-hooks
   # - repo: local
   #   hooks:
   #     - id: foo
   #       name: foo
   #       entry: foo
   #       language: system
```

### Comparing `pydantic-kedro-0.1.1/LICENSE` & `pydantic-kedro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.1/PKG-INFO` & `pydantic-kedro-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -43,65 +43,37 @@
 Advanced serialization for [Pydantic](https://docs.pydantic.dev/) models
 via [Kedro](https://kedro.readthedocs.io/en/stable/index.html) and
 [fsspec](https://filesystem-spec.readthedocs.io/en/latest/).
 
 This package implements custom Kedro "datasets" for both "pure" and "arbitrary"
 Pydantic models.
 
-## Examples
+Please see the [docs](https://pydantic-kedro.rtfd.io) for a tutorial and
+more examples.
 
-### "Pure" Pydantic Models
+## Minimal Example
 
 This example works for "pure", JSON-safe Pydantic models via
 `PydanticJsonDataSet`:
 
 ```python
 from pydantic import BaseModel
 from pydantic_kedro import PydanticJsonDataSet
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
+
     x: int
     y: str
 
 
 obj = MyPureModel(x=1, y="why?")
 
 # Create an in-memory (temporary) file via `fsspec` and save it
 ds = PydanticJsonDataSet("memory://temporary-file.json")
 ds.save(obj)
 
 # We can re-load it from the same file
 read_obj = ds.load()
 assert read_obj.x == 1
 ```
-
-Note that specifying custom JSON encoders also will work.
-
-### Models with Arbitrary Types
-
-Pydantic [supports models with arbitrary types](https://docs.pydantic.dev/usage/types/#arbitrary-types-allowed)
-if you specify it in the model's config.
-You can't save/load these via JSON, but you can use the other dataset types,
-`PydanticFolderDataSet` and
-`PydanticZipDataSet`:
-
-```python
-from pydantic import BaseModel
-from pydantic_kedro import PydanticJsonDataSet
-
-# TODO
-
-class MyArbitraryModel(BaseModel):
-    """Your custom Pydantic model with JSON-unsafe fields."""
-    x: int
-    y: str
-
-# TODO
-```
-
-## Further Reading
-
-See the [configuration](docs/configuration.md)...
-
-Check out the [API Reference](docs/reference/index.md) for auto-generated docs.
```

### Comparing `pydantic-kedro-0.1.1/README.md` & `pydantic-kedro-0.1.2/docs/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 # `pydantic-kedro`
 
 Advanced serialization for [Pydantic](https://docs.pydantic.dev/) models
 via [Kedro](https://kedro.readthedocs.io/en/stable/index.html) and
 [fsspec](https://filesystem-spec.readthedocs.io/en/latest/).
 
-This package implements custom Kedro "datasets" for both "pure" and "arbitrary"
-Pydantic models.
+This package implements custom Kedro DataSet types for not only "pure" (JSON-serializable)
+Pydantic models, but also models with [`arbitrary_types_allowed`](https://docs.pydantic.dev/usage/types/#arbitrary-types-allowed).
 
-## Examples
+Keep reading for a basic tutorial,
+or check out the [API Reference](reference/index.md) for auto-generated docs.
 
-### "Pure" Pydantic Models
+## Pre-requisites
 
-This example works for "pure", JSON-safe Pydantic models via
-`PydanticJsonDataSet`:
+To simplify the documentation, we will refer to JSON-serializable Pydantic models
+as "pure" models, while all others will be "arbitrary" models.
+
+We also assume you are familiar with [Kedro's Data Catalog](https://docs.kedro.org/en/stable/data/data_catalog.html)
+and [Datasets](https://docs.kedro.org/en/stable/data/kedro_io.html).
+
+## "Pure" Pydantic Models
+
+If you have a JSON-safe Pydantic model, you can use a
+[PydanticJsonDataSet][pydantic_kedro.PydanticJsonDataSet]
+to save your model to any `fsspec`-supported location:
 
 ```python
 from pydantic import BaseModel
 from pydantic_kedro import PydanticJsonDataSet
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
+
     x: int
     y: str
 
 
 obj = MyPureModel(x=1, y="why?")
 
 # Create an in-memory (temporary) file via `fsspec` and save it
@@ -32,36 +43,11 @@
 ds.save(obj)
 
 # We can re-load it from the same file
 read_obj = ds.load()
 assert read_obj.x == 1
 ```
 
-Note that specifying custom JSON encoders also will work.
-
-### Models with Arbitrary Types
-
-Pydantic [supports models with arbitrary types](https://docs.pydantic.dev/usage/types/#arbitrary-types-allowed)
-if you specify it in the model's config.
-You can't save/load these via JSON, but you can use the other dataset types,
-`PydanticFolderDataSet` and
-`PydanticZipDataSet`:
-
-```python
-from pydantic import BaseModel
-from pydantic_kedro import PydanticJsonDataSet
-
-# TODO
-
-class MyArbitraryModel(BaseModel):
-    """Your custom Pydantic model with JSON-unsafe fields."""
-    x: int
-    y: str
-
-# TODO
-```
-
-## Further Reading
-
-See the [configuration](docs/configuration.md)...
+Note that specifying [custom JSON encoders](https://docs.pydantic.dev/usage/exporting_models/#json_encoders) will work as usual.
 
-Check out the [API Reference](docs/reference/index.md) for auto-generated docs.
+However, if your custom type is difficult or impossible to encode/decode via
+JSON, read on to [Arbitrary Types](./arbitrary_types.md).
```

### Comparing `pydantic-kedro-0.1.1/docs/index.md` & `pydantic-kedro-0.1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -3,65 +3,37 @@
 Advanced serialization for [Pydantic](https://docs.pydantic.dev/) models
 via [Kedro](https://kedro.readthedocs.io/en/stable/index.html) and
 [fsspec](https://filesystem-spec.readthedocs.io/en/latest/).
 
 This package implements custom Kedro "datasets" for both "pure" and "arbitrary"
 Pydantic models.
 
-## Examples
+Please see the [docs](https://pydantic-kedro.rtfd.io) for a tutorial and
+more examples.
 
-### "Pure" Pydantic Models
+## Minimal Example
 
 This example works for "pure", JSON-safe Pydantic models via
-[PydanticJsonDataSet][pydantic_kedro.PydanticJsonDataSet]:
+`PydanticJsonDataSet`:
 
 ```python
 from pydantic import BaseModel
 from pydantic_kedro import PydanticJsonDataSet
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
+
     x: int
     y: str
 
 
 obj = MyPureModel(x=1, y="why?")
 
 # Create an in-memory (temporary) file via `fsspec` and save it
 ds = PydanticJsonDataSet("memory://temporary-file.json")
 ds.save(obj)
 
 # We can re-load it from the same file
 read_obj = ds.load()
 assert read_obj.x == 1
 ```
-
-Note that specifying custom JSON encoders also will work.
-
-### Models with Arbitrary Types
-
-Pydantic [supports models with arbitrary types](https://docs.pydantic.dev/usage/types/#arbitrary-types-allowed)
-if you specify it in the model's config.
-You can't save/load these via JSON, but you can use the other dataset types,
-[PydanticFolderDataSet][pydantic_kedro.PydanticFolderDataSet] and
-[PydanticZipDataSet][pydantic_kedro.PydanticZipDataSet]:
-
-```python
-from pydantic import BaseModel
-from pydantic_kedro import PydanticJsonDataSet
-
-# TODO
-
-class MyArbitraryModel(BaseModel):
-    """Your custom Pydantic model with JSON-unsafe fields."""
-    x: int
-    y: str
-
-# TODO
-```
-
-## Further Reading
-
-See the [configuration](configuration.md)...
-
-Check out the [API Reference](reference/index.md) for auto-generated docs.
```

### Comparing `pydantic-kedro-0.1.1/mkdocs.yml` & `pydantic-kedro-0.1.2/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 # NOTE: This allows looking at docs locally
 # See https://www.mkdocs.org/user-guide/configuration/#use_directory_urls
 site_url: ""
 use_directory_urls: false
 
 nav:
   - Overview: index.md
-  - Configuration: configuration.md
-  - Reference: reference/index.md
+  - Arbitrary Types: arbitrary_types.md
+  - API Reference: reference/index.md
+  - Implementation Details: implementation_details.md
 
 theme:
   name: "material"
   palette:
     - media: "(prefers-color-scheme: light)"
       scheme: default
       primary: pink
```

### Comparing `pydantic-kedro-0.1.1/pyproject.toml` & `pydantic-kedro-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -28,21 +28,20 @@
 ]
 urls = { github = "https://github.com/NowanIlfideme/pydantic-kedro" }
 
 [project.optional-dependencies]
 dev = [
     "setuptools>=61.0.0",
     "setuptools-scm[toml]>=6.2",
-    "pre-commit>=2.20.0",
-    "black>=22.6.0",
-    "flake8>=5.0.4",
-    "flake8-pyproject>=1.1.0",
-    "mypy>=1.0",
-    "pytest>=7.1.2",
-    "isort>=5.10.1",
+    "pre-commit==3.2.2",
+    "black==23.3.0",
+    "isort==5.12.0",
+    "ruff==0.0.263",
+    "mypy==1.2.0",
+    "pytest==7.3.1",
     # required for testing
     "kedro[pandas]",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]",
@@ -60,26 +59,32 @@
 [tool.setuptools.package-data]
 
 [tool.setuptools.dynamic]
 version = { attr = "pydantic_kedro.version.__version__" }
 
 [tool.setuptools_scm]
 
-[tool.flake8]
-ignore = ['E203', 'E231', 'W503']
-exclude = [".git", "src/test"]
-max-line-length = 105
-max-doc-length = 105
-per-file-ignores = "__init__.py:F401"
-count = true
+[tool.ruff]
+line-length = 105
+src = ["src"]
+select = [
+    "E", # pycodestyle
+    "F", # pyflakes
+    # "UP", # pyupgrade
+    "D", # pydocstyle
+]
+ignore = ["D203", "D213"] # conflicting
+
+[tool.ruff.pydocstyle]
+convention = "numpy"
+
 
 [tool.black]
 line-length = 105
 target-version = ['py39']
-extend-exclude = [".git"]
 
 [tool.isort]
 profile = "black"
 skip = [".git"]
 
 [tool.pytest.ini_options]
 # Docs: https://docs.pytest.org/en/7.1.x/reference/customize.html#pyproject-toml
```

### Comparing `pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         allow_population_by_field_name = True
         extra = Extra.allow
         smart_union = True
 
     @classmethod
     def from_dataset(cls, ds: AbstractDataSet, relative_path: str) -> "KedroDataSetSpec":
-        """Gets class from dataset."""
+        """Create spec class from dataset."""
         raw_args = ds._describe()
         # We need to actually look at the kwargs to ensure we don't pass any extra args...
         # ... because these implementations don't describe themselves correctly. Ugh.
         sig = inspect.signature(type(ds))
         clean_args: Dict[str, Any] = {}
         for k, v in raw_args.items():
             if k in sig.parameters:
@@ -61,15 +61,15 @@
             else:
                 logger.info(f"Ignoring dataset {type(ds).__name__} keyword {k!r} = {v!r}")
         return cls(type=get_import_name(type(ds)), relative_path=relative_path, args=clean_args)
 
     def to_dataset(
         self, base_path: str, load_version: Optional[str] = None, save_version: Optional[str] = None
     ) -> AbstractDataSet:
-        """Builds the DataSet object.
+        """Build the DataSet object.
 
         This assumes the local path is called `filepath`.
         """
         fsp = strip_protocol(base_path)  # I mean, this should be a local path...
         new_path = f"{fsp}/{self.relative_path}"
         config = self.dict(exclude={"relative_path"}, by_alias=True)
         config = {"type": self.type_, **self.args}
@@ -128,50 +128,50 @@
         else:
             mutate_jsp(struct[idx], jsp[1:], obj)
     else:
         raise TypeError(f"Unknown struct passed: {struct!r}")
 
 
 def get_import_name(obj: Any) -> str:
-    """Gets the import name for a type."""
+    """Get the import name for a type."""
     module_i = inspect.getmodule(obj)
     if module_i is None:
         raise TypeError(f"Could not find module for {obj!r}")
     r_name: str = getattr(obj, "__qualname__", obj.__name__)  # type: ignore
     return f"{module_i.__name__}.{r_name}"
 
 
 class PydanticFolderDataSet(AbstractDataSet[BaseModel, BaseModel]):
     """A Pydantic model with folder-based load/save.
 
     This allows fields with arbitrary types.
 
-    Example
+    Example:
     -------
     ```python
     class MyModel(BaseModel):
         x: str
 
     ds = PydanticFolderDataSet('memory://path/to/model')  # using in-memory to avoid tempfile
     ds.save(MyModel(x="example"))
     assert ds.load().x == "example"
     ```
     """
 
     def __init__(self, filepath: str) -> None:
-        """Creates a new instance of PydanticFolderDataSet to load/save Pydantic models for given path.
+        """Create a new instance of PydanticFolderDataSet to load/save Pydantic models for given path.
 
-        Args
+        Args:
         ----
         filepath : The location of the folder.
         """
         self._filepath = filepath
 
     def _save(self, data: BaseModel) -> None:
-        """Saves Pydantic model to the filepath."""
+        """Save Pydantic model to the filepath."""
         fs: AbstractFileSystem = fsspec.open(self._filepath).fs  # type: ignore
         if isinstance(fs, LocalFileSystem):
             self._save_local(data, self._filepath)
         else:
             from tempfile import TemporaryDirectory
 
             with TemporaryDirectory(prefix="pyd_kedro_") as tmpdir:
@@ -185,15 +185,15 @@
             # Close (this might be required for some filesystems)
             try:
                 fs.close()  # type: ignore
             except AttributeError:
                 pass
 
     def _load(self) -> BaseModel:
-        """Loads Pydantic model from the filepath.
+        """Load Pydantic model from the filepath.
 
         Returns
         -------
         Pydantic model.
         """
         fs: AbstractFileSystem = fsspec.open(self._filepath).fs  # type: ignore
         if isinstance(fs, LocalFileSystem):
@@ -208,15 +208,15 @@
                 for k, v in m_remote.items():
                     m_local[k] = v
 
                 # Load locally
                 return self._load_local(tmpdir)
 
     def _load_local(self, filepath: str) -> BaseModel:
-        """Loads Pydantic model from the local filepath.
+        """Load Pydantic model from the local filepath.
 
         Returns
         -------
         Pydantic model.
         """
         with fsspec.open(f"{filepath}/meta.json") as f:
             meta = FolderFormatMetadata.parse_raw(f.read())  # type: ignore
@@ -279,15 +279,15 @@
 
         # Roundtrip to apply the encoder and get UUID
         rt = json.loads(data.json(encoder=fake_encoder))
 
         # This will map the data to a dataset and actually save it
 
         def visit3(obj: Any, jsp: str, base_path: str) -> Any:
-            """Maps the data to a dataset in `catalog` and actually saves it."""
+            """Map the data to a dataset in `catalog` and actually saves it."""
             if isinstance(obj, str):
                 if obj in data_map:
                     # We got a data point
                     data = data_map[obj]
                     # Make a dataset for it
                     full_path = f"{base_path}/{jsp}"
                     ds = make_ds_for(data, full_path)
```

### Comparing `pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,41 +14,41 @@
 
 
 class PydanticJsonDataSet(AbstractDataSet[BaseModel, BaseModel]):
     """A Pydantic model with JSON-based load/save.
 
     Please note that the Pydantic model must not have any JSON-unfriendly fields.
 
-    Example
+    Example:
     -------
     ```python
     class MyModel(BaseModel):
         x: str
 
     ds = PydanticJsonDataSet('memory://path/to/model.json')  # using memory to avoid tempfile
     ds.save(MyModel(x="example"))
     assert ds.load().x == "example"
     ```
     """
 
     def __init__(self, filepath: str) -> None:
-        """Creates a new instance of PydanticJsonDataSet to load/save Pydantic models for given filepath.
+        """Create a new instance of PydanticJsonDataSet to load/save Pydantic models for given filepath.
 
-        Args
+        Args:
         ----
         filepath : The location of the JSON file.
         """
         # parse the path and protocol (e.g. file, http, s3, etc.)
         protocol, path = get_protocol_and_path(filepath)
         self._protocol = protocol
         self._filepath = PurePosixPath(path)
         self._fs: AbstractFileSystem = fsspec.filesystem(self._protocol)
 
     def _load(self) -> BaseModel:
-        """Loads Pydantic model from the filepath.
+        """Load Pydantic model from the filepath.
 
         Returns
         -------
         Pydantic model.
         """
         # using get_filepath_str ensures that the protocol and path
         # are appended correctly for different filesystems
@@ -62,15 +62,15 @@
         assert issubclass(pyd_kls, BaseModel), f"Type must be a Pydantic model, got {type(pyd_kls)!r}."
         dct.pop(KLS_MARK_STR)  # don't accidentally pass to proper model
         res = parse_obj_as(pyd_kls, dct)
         return res  # type: ignore
 
     @no_type_check
     def _save(self, data: BaseModel) -> None:
-        """Saves Pydantic model to the filepath."""
+        """Save Pydantic model to the filepath."""
         # Add metadata to our Pydantic model
         pyd_kls = type(data)
         if KLS_MARK_STR in pyd_kls.__fields__.keys():
             raise ValueError(f"Marker {KLS_MARK_STR!r} already exists as a field; can't dump model.")
         pyd_kls_path = f"{pyd_kls.__module__}.{pyd_kls.__qualname__}"
         tmp_kls = create_model(
             pyd_kls.__name__,
@@ -82,9 +82,9 @@
 
         # Open file and write to it
         save_path = get_filepath_str(self._filepath, self._protocol)
         with self._fs.open(save_path, mode="w") as f:
             f.write(tmp_obj.json())
 
     def _describe(self) -> Dict[str, Any]:
-        """Returns a dict that describes the attributes of the dataset."""
+        """Return a dict that describes the attributes of the dataset."""
         return dict(filepath=self._filepath, protocol=self._protocol)
```

### Comparing `pydantic-kedro-0.1.1/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,37 +12,37 @@
 
 
 class PydanticZipDataSet(AbstractDataSet[BaseModel, BaseModel]):
     """A Pydantic model with Zip-file-based load/save.
 
     This allows fields with arbitrary types.
 
-    Example
+    Example:
     -------
     ```python
     class MyModel(BaseModel):
         x: str
 
     ds = PydanticZipDataSet('memory://path/to/model.zip')  # using memory to avoid tempfile
     ds.save(MyModel(x="example"))
     assert ds.load().x == "example"
     ```
     """
 
     def __init__(self, filepath: str) -> None:
-        """Creates a new instance of PydanticZipDataSet to load/save Pydantic models for given filepath.
+        """Create a new instance of PydanticZipDataSet to load/save Pydantic models for given filepath.
 
-        Args
+        Args:
         ----
         filepath : The location of the Zip file.
         """
         self._filepath = filepath
 
     def _load(self) -> BaseModel:
-        """Loads Pydantic model from the filepath.
+        """Load Pydantic model from the filepath.
 
         Returns
         -------
         Pydantic model.
         """
         filepath = self._filepath
         with TemporaryDirectory(prefix="pyd_kedro_") as tmpdir:
@@ -56,15 +56,15 @@
                 zip_fs.close()
             # Load folder dataset
             pfds = PydanticFolderDataSet(tmpdir)
             res = pfds.load()
         return res
 
     def _save(self, data: BaseModel) -> None:
-        """Saves Pydantic model to the filepath."""
+        """Save Pydantic model to the filepath."""
         filepath = self._filepath
         with TemporaryDirectory(prefix="pyd_kedro_") as tmpdir:
             # Save folder dataset
             pfds = PydanticFolderDataSet(tmpdir)
             pfds.save(data)
             # Zip via copying to folder
             m_local = fsspec.get_mapper(tmpdir)
```

### Comparing `pydantic-kedro-0.1.1/src/pydantic_kedro/models.py` & `pydantic-kedro-0.1.2/src/pydantic_kedro/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from kedro.extras.datasets.pickle import PickleDataSet
 from kedro.io import AbstractDataSet
 from pydantic import BaseConfig, BaseModel
 
 
 class ArbConfig(BaseConfig):
-    """Configuration with arbitrary types allowed; see [pydantic_kedro.ArbModel][]"""
+    """Configuration with arbitrary types allowed; see [pydantic_kedro.ArbModel][]."""
 
     arbitrary_types_allowed = True
 
     kedro_map: Dict[Type, Callable[[str], AbstractDataSet]] = {}
     kedro_default: Callable[[str], AbstractDataSet] = PickleDataSet
```

### Comparing `pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -43,65 +43,37 @@
 Advanced serialization for [Pydantic](https://docs.pydantic.dev/) models
 via [Kedro](https://kedro.readthedocs.io/en/stable/index.html) and
 [fsspec](https://filesystem-spec.readthedocs.io/en/latest/).
 
 This package implements custom Kedro "datasets" for both "pure" and "arbitrary"
 Pydantic models.
 
-## Examples
+Please see the [docs](https://pydantic-kedro.rtfd.io) for a tutorial and
+more examples.
 
-### "Pure" Pydantic Models
+## Minimal Example
 
 This example works for "pure", JSON-safe Pydantic models via
 `PydanticJsonDataSet`:
 
 ```python
 from pydantic import BaseModel
 from pydantic_kedro import PydanticJsonDataSet
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
+
     x: int
     y: str
 
 
 obj = MyPureModel(x=1, y="why?")
 
 # Create an in-memory (temporary) file via `fsspec` and save it
 ds = PydanticJsonDataSet("memory://temporary-file.json")
 ds.save(obj)
 
 # We can re-load it from the same file
 read_obj = ds.load()
 assert read_obj.x == 1
 ```
-
-Note that specifying custom JSON encoders also will work.
-
-### Models with Arbitrary Types
-
-Pydantic [supports models with arbitrary types](https://docs.pydantic.dev/usage/types/#arbitrary-types-allowed)
-if you specify it in the model's config.
-You can't save/load these via JSON, but you can use the other dataset types,
-`PydanticFolderDataSet` and
-`PydanticZipDataSet`:
-
-```python
-from pydantic import BaseModel
-from pydantic_kedro import PydanticJsonDataSet
-
-# TODO
-
-class MyArbitraryModel(BaseModel):
-    """Your custom Pydantic model with JSON-unsafe fields."""
-    x: int
-    y: str
-
-# TODO
-```
-
-## Further Reading
-
-See the [configuration](docs/configuration.md)...
-
-Check out the [API Reference](docs/reference/index.md) for auto-generated docs.
```

### Comparing `pydantic-kedro-0.1.1/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 .gitignore
+.markdownlint.yaml
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 README.md
 environment.yml
 mkdocs.yml
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-testing.yml
-docs/configuration.md
+docs/arbitrary_types.md
+docs/implementation_details.md
 docs/index.md
 docs/reference/index.md
 src/pydantic_kedro/__init__.py
 src/pydantic_kedro/models.py
 src/pydantic_kedro/py.typed
 src/pydantic_kedro/version.py
 src/pydantic_kedro.egg-info/PKG-INFO
```

### Comparing `pydantic-kedro-0.1.1/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.1.2/src/test/catalogs/test_basic_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 # # Create an in-memory (temporary) file via `fsspec` and save it
 obj = MyPureModel(x=1, y="why?")
 # ds = PydanticJsonDataSet(local_dir / "data/tst1.json")
 # ds.save(obj)
 
 
 def test_basic_catalog():
-    """Basic test to ensure"""
+    """Basic test to ensure."""
     os.chdir(local_dir)
     conf_loader = ConfigLoader(str(local_dir / "conf"))
     catalog = DataCatalog.from_config(conf_loader.get("catalog.yml"))
     obj2 = catalog.load("tst1")
     assert isinstance(catalog.datasets.tst1, PydanticJsonDataSet)  # type: ignore
     assert obj2 == obj
```

### Comparing `pydantic-kedro-0.1.1/src/test/test_ds_extended.py` & `pydantic-kedro-0.1.2/src/test/test_ds_extended.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 Kls = Union[PydanticFolderDataSet, PydanticZipDataSet]
 
 
 class Singleton:
     """Class that is always equal to itself (for ease of testing)."""
 
     def __eq__(self, __o: object) -> bool:
+        """Check for equality of the singleton."""
         return isinstance(__o, Singleton)
 
 
 class MyStr:
     """Custom string thingy. Equality via string.
 
     This is NOT serialized as `str` in Pydantic, but as an object via Pickle.
     """
 
     def __init__(self, v: str):
+        """Initialize."""
         self.v = v
 
     def __eq__(self, x):
+        """Check for string equality."""
         return str(x) == str(self)
 
     def __str__(self):
+        """Return the internal string."""
         return self.v
 
 
 class MyStrDs(TextDataSet):
     """Custom dataset for loading MyStr type."""
 
     def _load(self) -> MyStr:
@@ -42,14 +46,16 @@
         return super()._save(str(data))
 
 
 class UserExtendedModel(ArbModel):
     """Arbitrary model, extended with the user model."""
 
     class Config(ArbModel.Config):
+        """Arbitrary model configuration."""
+
         kedro_map = {MyStr: MyStrDs}
 
     sing: Singleton = Singleton()
     ms: MyStr = MyStr("foobar")
     dct: Dict[str, Any] = {}
```

### Comparing `pydantic-kedro-0.1.1/src/test/test_ds_pandas.py` & `pydantic-kedro-0.1.2/src/test/test_ds_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test dataset for Pandas specifically."""
+
 from typing import Any, Dict, Union
 
 import pandas as pd
 import pytest
 from kedro.extras.datasets.pandas import ParquetDataSet
 
 from pydantic_kedro import ArbModel, PydanticFolderDataSet, PydanticZipDataSet
```

### Comparing `pydantic-kedro-0.1.1/src/test/test_ds_simple.py` & `pydantic-kedro-0.1.2/src/test/test_ds_simple.py`

 * *Files identical despite different names*

