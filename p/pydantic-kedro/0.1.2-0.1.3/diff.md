# Comparing `tmp/pydantic-kedro-0.1.2.tar.gz` & `tmp/pydantic-kedro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.1.2.tar", last modified: Wed Apr 26 16:29:31 2023, max compression
+gzip compressed data, was "pydantic-kedro-0.1.3.tar", last modified: Wed Apr 26 18:00:38 2023, max compression
```

## Comparing `pydantic-kedro-0.1.2.tar` & `pydantic-kedro-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/arbitrary_types.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.447972 pydantic-kedro-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.451972 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:28:41.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 16:29:31.000000 pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.447972 pydantic-kedro-0.1.2/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:29:31.455972 pydantic-kedro-0.1.2/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 16:28:25.000000 pydantic-kedro-0.1.2/src/test/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.596019 pydantic-kedro-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:00:38.596019 pydantic-kedro-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.580019 pydantic-kedro-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.588019 pydantic-kedro-0.1.3/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.588019 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:59:47.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.580019 pydantic-kedro-0.1.3/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_import.py
```

### Comparing `pydantic-kedro-0.1.2/.github/dependabot.yml` & `pydantic-kedro-0.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/.github/workflows/python-publish.yml` & `pydantic-kedro-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/.github/workflows/python-testing.yml` & `pydantic-kedro-0.1.3/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/.pre-commit-config.yaml` & `pydantic-kedro-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/LICENSE` & `pydantic-kedro-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/PKG-INFO` & `pydantic-kedro-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.1.2/README.md` & `pydantic-kedro-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/docs/arbitrary_types.md` & `pydantic-kedro-0.1.3/docs/arbitrary_types.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/docs/implementation_details.md` & `pydantic-kedro-0.1.3/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/docs/index.md` & `pydantic-kedro-0.1.3/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 We also assume you are familiar with [Kedro's Data Catalog](https://docs.kedro.org/en/stable/data/data_catalog.html)
 and [Datasets](https://docs.kedro.org/en/stable/data/kedro_io.html).
 
 ## "Pure" Pydantic Models
 
 If you have a JSON-safe Pydantic model, you can use a
 [PydanticJsonDataSet][pydantic_kedro.PydanticJsonDataSet]
+or [PydanticYamlDataSet][pydantic_kedro.PydanticYamlDataSet]
 to save your model to any `fsspec`-supported location:
 
 ```python
 from pydantic import BaseModel
 from pydantic_kedro import PydanticJsonDataSet
 
 
@@ -43,11 +44,14 @@
 ds.save(obj)
 
 # We can re-load it from the same file
 read_obj = ds.load()
 assert read_obj.x == 1
 ```
 
-Note that specifying [custom JSON encoders](https://docs.pydantic.dev/usage/exporting_models/#json_encoders) will work as usual.
+> Note: YAML support is enabled by [`pydantic-yaml`](https://pydantic-yaml.readthedocs.io/en/latest/).
+
+Note that specifying [custom JSON encoders](https://docs.pydantic.dev/usage/exporting_models/#json_encoders)
+will work as usual, even for YAML models.
 
 However, if your custom type is difficult or impossible to encode/decode via
 JSON, read on to [Arbitrary Types](./arbitrary_types.md).
```

### Comparing `pydantic-kedro-0.1.2/mkdocs.yml` & `pydantic-kedro-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/pyproject.toml` & `pydantic-kedro-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 dependencies = [
     "pydantic>=1.10.0,<2",
-    # "pydantic-yaml",  # not currently needed
+    "pydantic-yaml>=1.0.0a2",
     "kedro",
     "fsspec",
 ]
 urls = { github = "https://github.com/NowanIlfideme/pydantic-kedro" }
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/yaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,53 @@
-"""JSON dataset definition for Pydantic."""
+"""YAML dataset definition for Pydantic."""
 
-import json
 from pathlib import PurePosixPath
 from typing import Any, Dict, no_type_check
 
 import fsspec
 from fsspec import AbstractFileSystem
 from kedro.io.core import AbstractDataSet, get_filepath_str, get_protocol_and_path
-from pydantic import BaseModel, create_model, parse_obj_as
+from pydantic import BaseModel, Field, create_model
 from pydantic.utils import import_string
+from pydantic_yaml import parse_yaml_file_as, to_yaml_file
 
 KLS_MARK_STR = "class"
 
 
-class PydanticJsonDataSet(AbstractDataSet[BaseModel, BaseModel]):
-    """A Pydantic model with JSON-based load/save.
+class _YamlPreLoader(BaseModel):
+    """YAML pre-loader model."""
 
-    Please note that the Pydantic model must not have any JSON-unfriendly fields.
+    kls_mark_str: str = Field(alias=KLS_MARK_STR)  # type: ignore
+
+
+class PydanticYamlDataSet(AbstractDataSet[BaseModel, BaseModel]):
+    """A Pydantic model with YAML-based load/save.
+
+    Please note that the Pydantic model must be JSON-serializable.
+    That means the fields are "pure" Pydantic fields,
+    or you have added `json_encoders` to the model config.
 
     Example:
     -------
     ```python
     class MyModel(BaseModel):
         x: str
 
-    ds = PydanticJsonDataSet('memory://path/to/model.json')  # using memory to avoid tempfile
+    ds = PydanticYamlDataSet('memory://path/to/model.yaml')  # using memory to avoid tempfile
     ds.save(MyModel(x="example"))
     assert ds.load().x == "example"
     ```
     """
 
     def __init__(self, filepath: str) -> None:
-        """Create a new instance of PydanticJsonDataSet to load/save Pydantic models for given filepath.
+        """Create a new instance of PydanticYamlDataSet to load/save Pydantic models for given filepath.
 
         Args:
         ----
-        filepath : The location of the JSON file.
+        filepath : The location of the YAML file.
         """
         # parse the path and protocol (e.g. file, http, s3, etc.)
         protocol, path = get_protocol_and_path(filepath)
         self._protocol = protocol
         self._filepath = PurePosixPath(path)
         self._fs: AbstractFileSystem = fsspec.filesystem(self._protocol)
 
@@ -50,22 +58,19 @@
         -------
         Pydantic model.
         """
         # using get_filepath_str ensures that the protocol and path
         # are appended correctly for different filesystems
         load_path = get_filepath_str(self._filepath, self._protocol)
         with self._fs.open(load_path, mode="r") as f:
-            dct = json.load(f)
-        assert isinstance(dct, dict), "JSON root must be a mapping."
-        if KLS_MARK_STR not in dct.keys():
-            raise TypeError(f"Cannot determine pydantic model type, missing {KLS_MARK_STR!r}")
-        pyd_kls = import_string(dct[KLS_MARK_STR])
+            preloader = parse_yaml_file_as(_YamlPreLoader, f)
+        pyd_kls = import_string(preloader.kls_mark_str)
         assert issubclass(pyd_kls, BaseModel), f"Type must be a Pydantic model, got {type(pyd_kls)!r}."
-        dct.pop(KLS_MARK_STR)  # don't accidentally pass to proper model
-        res = parse_obj_as(pyd_kls, dct)
+        with self._fs.open(load_path, mode="r") as f:
+            res = parse_yaml_file_as(pyd_kls, f)
         return res  # type: ignore
 
     @no_type_check
     def _save(self, data: BaseModel) -> None:
         """Save Pydantic model to the filepath."""
         # Add metadata to our Pydantic model
         pyd_kls = type(data)
@@ -79,12 +84,12 @@
             **{KLS_MARK_STR: (str, pyd_kls_path)},
         )
         tmp_obj = tmp_kls(**data.dict())
 
         # Open file and write to it
         save_path = get_filepath_str(self._filepath, self._protocol)
         with self._fs.open(save_path, mode="w") as f:
-            f.write(tmp_obj.json())
+            to_yaml_file(f, tmp_obj)
 
     def _describe(self) -> Dict[str, Any]:
         """Return a dict that describes the attributes of the dataset."""
         return dict(filepath=self._filepath, protocol=self._protocol)
```

### Comparing `pydantic-kedro-0.1.2/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/zip.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/src/pydantic_kedro/models.py` & `pydantic-kedro-0.1.3/src/pydantic_kedro/models.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.1.2/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/pydantic_kedro.egg-info/dependency_links.txt
 src/pydantic_kedro.egg-info/not-zip-safe
 src/pydantic_kedro.egg-info/requires.txt
 src/pydantic_kedro.egg-info/top_level.txt
 src/pydantic_kedro/datasets/__init__.py
 src/pydantic_kedro/datasets/folder.py
 src/pydantic_kedro/datasets/json.py
+src/pydantic_kedro/datasets/yaml.py
 src/pydantic_kedro/datasets/zip.py
 src/test/test_ds_extended.py
 src/test/test_ds_pandas.py
 src/test/test_ds_simple.py
 src/test/test_import.py
 src/test/catalogs/test_basic_catalog.py
 src/test/catalogs/conf/base/catalog.yml
```

### Comparing `pydantic-kedro-0.1.2/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.1.3/src/test/catalogs/test_basic_catalog.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/src/test/test_ds_extended.py` & `pydantic-kedro-0.1.3/src/test/test_ds_extended.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/src/test/test_ds_pandas.py` & `pydantic-kedro-0.1.3/src/test/test_ds_pandas.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.2/src/test/test_ds_simple.py` & `pydantic-kedro-0.1.3/src/test/test_ds_simple.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-"""Tests the JSON dataset on a simple model."""
+"""Tests the datasets on a simple model."""
 
-from typing import Optional, Union
+from typing import Optional
 
 import pytest
+from kedro.io.core import AbstractDataSet
 from pydantic import BaseModel
 
 from pydantic_kedro import (
     PydanticFolderDataSet,
     PydanticJsonDataSet,
+    PydanticYamlDataSet,
     PydanticZipDataSet,
 )
 
 
 class SimpleTestModel(BaseModel):
     """My very own model.
 
-    NOTE: Since this is defined in `__main__`, this can only be loaded if ran in this notebook.
+    NOTE: Since this is defined in `__main__`, this can only be loaded if ran in this file.
     """
 
     name: str
     alter_ego: Optional[str] = None
 
 
-Kls = Union[PydanticFolderDataSet, PydanticJsonDataSet, PydanticZipDataSet]
+types = [PydanticJsonDataSet, PydanticYamlDataSet, PydanticFolderDataSet, PydanticZipDataSet]
 
 
 @pytest.mark.parametrize(
     "mdl", [SimpleTestModel(name="user"), SimpleTestModel(name="Dr. Jekyll", alter_ego="Mr. Hyde")]
 )
-@pytest.mark.parametrize("kls", [PydanticJsonDataSet, PydanticFolderDataSet, PydanticZipDataSet])
-def test_simple_model_rt(mdl: SimpleTestModel, kls: Kls, tmpdir):
+@pytest.mark.parametrize("kls", types)
+def test_simple_model_rt(mdl: SimpleTestModel, kls: AbstractDataSet, tmpdir):  # type: ignore
     """Tests whether a simple model survives roundtripping."""
     paths = [f"{tmpdir}/model_on_disk", f"memory://{tmpdir}/model_in_memory"]
     for path in paths:
-        ds: Kls = kls(path)  # type: ignore
+        ds: AbstractDataSet = kls(path)  # type: ignore
         ds.save(mdl)
         m2 = ds.load()
         assert isinstance(m2, SimpleTestModel)
         assert m2 == mdl
```

