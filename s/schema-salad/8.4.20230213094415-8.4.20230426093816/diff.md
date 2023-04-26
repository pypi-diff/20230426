# Comparing `tmp/schema-salad-8.4.20230213094415.tar.gz` & `tmp/schema-salad-8.4.20230426093816.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-salad-8.4.20230213094415.tar", last modified: Mon Feb 13 10:17:49 2023, max compression
+gzip compressed data, was "schema-salad-8.4.20230426093816.tar", last modified: Wed Apr 26 10:11:35 2023, max compression
```

## Comparing `schema-salad-8.4.20230213094415.tar` & `schema-salad-8.4.20230426093816.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.051324 schema-salad-8.4.20230213094415/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.887320 schema-salad-8.4.20230213094415/.circleci/
--rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.circleci/config.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.flake8
--rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.git-blame-ignore-revs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.891320 schema-salad-8.4.20230213094415/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.891320 schema-salad-8.4.20230213094415/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     3859 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.github/workflows/quay-publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.github/workflows/wheel-prep.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.github/workflows/wheels.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.isort.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.mergify.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    17169 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.pylintrc
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     8324 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-02-13 10:17:49.055324 schema-salad-8.4.20230213094415/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/README.rst
--rwxr-xr-x   0 michael   (1000) michael   (1000)      438 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/build-schema_salad-docker.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/dev-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.899320 schema-salad-8.4.20230213094415/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.899320 schema-salad-8.4.20230213094415/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/docs/cli.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/docs/typeshed.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/lgtm.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/manual_wheel_publish.sh
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.855319 schema-salad-8.4.20230213094415/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.903321 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.903321 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.907321 schema-salad-8.4.20230213094415/mypy-stubs/mistune/
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/_types.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/block_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/inline_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/markdown.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.907321 schema-salad-8.4.20230213094415/mypy-stubs/mistune/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/plugins/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/plugins/table.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/renderers.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/scanner.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/mistune/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.923321 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/compare.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/exceptions.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.935321 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.935321 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.939321 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/term.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/rdflib/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.939321 schema-salad-8.4.20230213094415/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy-stubs/ruamel/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)     1061 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      292 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.959322 schema-salad-8.4.20230213094415/schema_salad/
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-02-13 10:17:48.000000 schema-salad-8.4.20230213094415/schema_salad/_version.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.963322 schema-salad-8.4.20230213094415/schema_salad/avro/
--rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/avro/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/avro/NOTICE
--rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/avro/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    24051 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/avro/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7270 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/codegen_base.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10930 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dlang_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.967322 schema-salad-8.4.20230213094415/schema_salad/dotnet/
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/AssemblyInfo.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.967322 schema-salad-8.4.20230213094415/schema_salad/dotnet/DocFx/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/DocFx/filterConfig.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/DocFx/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/DocFx/toc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Project.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Solution.sln
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.967322 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.967322 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/runsettings.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.971322 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/
--rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/ExampleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/FetcherTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/UtilitiesTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.971322 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.971322 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
--rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/Test.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/docfx.json
--rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/editorconfig
--rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.975322 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/
--rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Fetcher.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/LoaderInstances.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.979322 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/AnyLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/EnumLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/Loader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/NullLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/RecordLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/RootLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/UnionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/UriLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/LoadingOptions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Saveable.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/UriExtensions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Utilities.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/ValidationException.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Vocabs.cs
--rw-r--r--   0 michael   (1000) michael   (1000)    33304 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4185 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/exceptions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8027 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/fetcher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.983322 schema-salad-8.4.20230213094415/schema_salad/java/
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/MANIFEST.MF
--rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.991323 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/AnyLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/ArrayLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/ConstantMaps.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/DefaultFetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/EnumLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/ExpressionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Fetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/IdMapLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Loader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/LoaderInstances.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/LoadingOptions.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/LoadingOptionsBuilder.java
--rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/NullLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/OneOrListOf.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/OneOrListOfLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/OptionalLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/PrimitiveLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/RecordLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/RootLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Saveable.java
--rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/SaveableImpl.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/TypeDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/UnionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/UriLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Uris.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/ValidationException.java
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Validator.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/YamlUtils.java
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/main_utils/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/overview.html
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/pom.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.991323 schema-salad-8.4.20230213094415/schema_salad/java/test_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/test_utils/DefaultFetcherTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/test_utils/ExamplesTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/test_utils/ShortnameTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java/test_utils/YamlUtilsTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)    32358 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/java_codegen.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8506 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/jsonld_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14076 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/makedoc.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.003323 schema-salad-8.4.20230213094415/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3940 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    13475 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      830 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)   131045 2023-02-13 09:58:10.000000 schema-salad-8.4.20230213094415/schema_salad/metaschema.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)    23034 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/python_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28761 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/python_codegen_support.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46872 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/ref_resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30196 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9212 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/sourceline.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.023323 schema-salad-8.4.20230213094415/schema_salad/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/EDAM.owl
--rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/bad_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/bad_schema2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/basket.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/basket_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/class_field_test.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/cwl-pre.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.023323 schema-salad-8.4.20230213094415/schema_salad/tests/docimp/
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/docimp/d1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/docimp/d2.md
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/docimp/d3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/docimp/d4.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/docimp/d5.md
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/docimp/dpre.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.027324 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/foreign_prop1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/foreign_prop2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/foreign_prop3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/foreign_prop4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/foreign_prop5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/foreign_prop6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/foreign/foreign_prop7.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/frag.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/hello.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/inherited-attributes.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/inject-id1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/inject-id2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/inject-id3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/list.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/matcher.py
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/memory-leak-check.py
--rw-r--r--   0 michael   (1000) michael   (1000)    61408 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/metaschema-pre.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/missing_step_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/mixin.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/multidoc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/pt.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/revtool_bad_schema.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_avro_names.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_cg.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_cli_args.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2406 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_cwl11.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_dlang_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15557 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19849 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_fp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_java_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_makedoc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_pickling.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_print_oneline.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_python_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.027324 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.027324 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
--rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.031324 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/bio-cwl-tools/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.031324 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/h3agatk/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.031324 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/topmed/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_ref_resolver.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.043324 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/
--rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/avro_naming.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/avro_naming_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/avro_subtype.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/avro_subtype_bad.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/cwltest-schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/invocation.md
--rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/misc_schema_v1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/misc_schema_v2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/no_field_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/one_line_primary_doc.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test10.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test11.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test12.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test13.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test14.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test15.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test16.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test17.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test18.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test19.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test7.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test8.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/test9.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_schemas_directive.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_subtypes.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/test_typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/tests/util.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.043324 schema-salad-8.4.20230213094415/schema_salad/typescript/
--rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/index.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/package.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.047324 schema-salad-8.4.20230213094415/schema_salad/typescript/test/
--rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/AnyLoader.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/ExampleTest.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/Fetcher.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/IdMap.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/Typeguards.spec.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.047324 schema-salad-8.4.20230213094415/schema_salad/typescript/test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/data/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/test/utilities.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/tsconfig.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.051324 schema-salad-8.4.20230213094415/schema_salad/typescript/util/
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/Dict.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/Fetcher.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/Internal.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/LoaderInstances.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/LoadingOptions.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/Saveable.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/Typeguards.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/ValidationException.ts
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/Vocabs.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:49.051324 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/AnyLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/ArrayLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/EnumLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/ExpressionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/IdMapLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/Loader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/RecordLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/RootLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/UnionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/UriLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)    29355 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3692 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15994 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad/validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/schema_salad.Dockerfile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-02-13 10:17:48.963322 schema-salad-8.4.20230213094415/schema_salad.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-02-13 10:17:48.000000 schema-salad-8.4.20230213094415/schema_salad.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-02-13 10:17:48.000000 schema-salad-8.4.20230213094415/schema_salad.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-02-13 10:17:48.000000 schema-salad-8.4.20230213094415/schema_salad.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-02-13 10:17:48.000000 schema-salad-8.4.20230213094415/schema_salad.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-02-13 10:17:48.000000 schema-salad-8.4.20230213094415/schema_salad.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-02-13 10:17:48.000000 schema-salad-8.4.20230213094415/schema_salad.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-02-13 09:56:54.000000 schema-salad-8.4.20230213094415/schema_salad.egg-info/zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-02-13 10:17:49.055324 schema-salad-8.4.20230213094415/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     5699 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/test-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2721 2023-02-13 09:56:19.000000 schema-salad-8.4.20230213094415/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/.circleci/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.circleci/config.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.flake8
+-rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.git-blame-ignore-revs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3859 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/quay-publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/wheel-prep.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.github/workflows/wheels.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.isort.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.mergify.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21223 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.pylintrc
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     8324 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/README.rst
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      438 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/build-schema_salad-docker.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/dev-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/cli.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/make.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/docs/typeshed.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/lgtm.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/manual_wheel_publish.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.315565 schema-salad-8.4.20230426093816/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.323566 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/mistune/
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/_types.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/block_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/inline_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/markdown.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/table.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/renderers.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/scanner.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/mistune/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.327566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/compare.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/exceptions.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.331566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.331566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.331566 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/term.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/rdflib/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.335566 schema-salad-8.4.20230426093816/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy-stubs/ruamel/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)     1061 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      292 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad/_version.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad/avro/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/NOTICE
+-rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23815 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/avro/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7237 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/codegen_base.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10930 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dlang_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad/dotnet/
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/AssemblyInfo.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/filterConfig.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/DocFx/toc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Project.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Solution.sln
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/runsettings.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/
+-rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/ExampleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/FetcherTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/UtilitiesTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.343566 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/Test.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/docfx.json
+-rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/editorconfig
+-rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.347566 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Fetcher.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/LoaderInstances.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.347566 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/AnyLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/EnumLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/Loader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/NullLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RecordLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RootLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UnionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UriLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/LoadingOptions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Saveable.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/UriExtensions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Utilities.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ValidationException.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Vocabs.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)    33304 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4175 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/exceptions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8025 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/fetcher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.347566 schema-salad-8.4.20230426093816/schema_salad/java/
+-rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/MANIFEST.MF
+-rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.355566 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/AnyLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ArrayLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ConstantMaps.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/DefaultFetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/EnumLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ExpressionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Fetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/IdMapLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Loader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoaderInstances.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptions.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptionsBuilder.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/NullLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOf.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOfLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OptionalLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/PrimitiveLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RecordLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RootLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Saveable.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/SaveableImpl.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/TypeDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UnionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UriLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Uris.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ValidationException.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Validator.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/YamlUtils.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/main_utils/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/overview.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/pom.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.355566 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/DefaultFetcherTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/ExamplesTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/ShortnameTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java/test_utils/YamlUtilsTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)    32358 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/java_codegen.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8476 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/jsonld_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14154 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/makedoc.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.359567 schema-salad-8.4.20230426093816/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3940 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    13475 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      830 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)   130989 2023-04-26 10:03:15.000000 schema-salad-8.4.20230426093816/schema_salad/metaschema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)    23034 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/python_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28705 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/python_codegen_support.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46610 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/ref_resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29944 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9031 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/sourceline.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.371567 schema-salad-8.4.20230426093816/schema_salad/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/EDAM.owl
+-rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/bad_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/bad_schema2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/basket.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/basket_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/class_field_test.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/cwl-pre.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.371567 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d2.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d4.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/d5.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/docimp/dpre.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/foreign/foreign_prop7.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/frag.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/hello.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inherited-attributes.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inject-id1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inject-id2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/inject-id3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/list.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/matcher.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/memory-leak-check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    61408 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/metaschema-pre.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/missing_step_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/mixin.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/multidoc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/pt.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/revtool_bad_schema.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_avro_names.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cg.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cli_args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2406 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_cwl11.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_dlang_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15557 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19849 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_fp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_java_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_makedoc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_misc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_pickling.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_print_oneline.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_python_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
+-rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.375567 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/topmed/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_ref_resolver.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.379567 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/
+-rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_naming.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_naming_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype_bad.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/cwltest-schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/invocation.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/no_field_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/one_line_primary_doc.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test10.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test11.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test12.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test13.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test14.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test15.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test16.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test17.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test18.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test19.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test7.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test8.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/test9.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_schemas_directive.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_subtypes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/test_typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/index.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/package.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/test/
+-rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/AnyLoader.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/ExampleTest.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/Fetcher.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/IdMap.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/Typeguards.spec.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/data/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/test/utilities.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/tsconfig.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.383567 schema-salad-8.4.20230426093816/schema_salad/typescript/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Dict.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Fetcher.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Internal.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/LoaderInstances.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/LoadingOptions.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Saveable.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Typeguards.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/ValidationException.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/Vocabs.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/AnyLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/ArrayLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/EnumLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/ExpressionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/IdMapLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/Loader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RecordLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RootLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UnionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UriLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)    29355 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3640 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15546 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad/validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/schema_salad.Dockerfile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 10:11:35.339566 schema-salad-8.4.20230426093816/schema_salad.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-04-26 10:11:35.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-26 10:02:44.000000 schema-salad-8.4.20230426093816/schema_salad.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-04-26 10:11:35.387567 schema-salad-8.4.20230426093816/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     5699 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/test-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2721 2023-04-26 10:02:30.000000 schema-salad-8.4.20230426093816/tox.ini
```

### Comparing `schema-salad-8.4.20230213094415/.circleci/config.yml` & `schema-salad-8.4.20230426093816/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/.github/dependabot.yml` & `schema-salad-8.4.20230426093816/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/.github/workflows/ci-tests.yml` & `schema-salad-8.4.20230426093816/.github/workflows/ci-tests.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/.github/workflows/codeql-analysis.yml` & `schema-salad-8.4.20230426093816/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/.github/workflows/quay-publish.yml` & `schema-salad-8.4.20230426093816/.github/workflows/quay-publish.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/.github/workflows/wheels.yml` & `schema-salad-8.4.20230426093816/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/.mergify.yml` & `schema-salad-8.4.20230426093816/.mergify.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/.pylintrc` & `schema-salad-8.4.20230426093816/.pylintrc`

 * *Files 19% similar despite different names*

```diff
@@ -1,303 +1,229 @@
-[MASTER]
+[MAIN]
+
+# Analyse import fallback blocks. This can be used to support both Python 2 and
+# 3 compatible code, which means that the block might have code that exists
+# only in one or another interpreter, leading to false positives when analysed.
+analyse-fallback-blocks=no
+
+# Clear in-memory caches upon conclusion of linting. Useful if running pylint
+# in a server-like mode.
+clear-cache-post-run=no
+
+# Load and enable all available extensions. Use --list-extensions to see a list
+# all available extensions.
+#enable-all-extensions=
+
+# In error mode, messages with a category besides ERROR or FATAL are
+# suppressed, and no reports are done by default. Error mode is compatible with
+# disabling specific errors.
+#errors-only=
+
+# Always return a 0 (non-error) status code, even if lint errors are found.
+# This is primarily useful in continuous integration scripts.
+#exit-zero=
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code.
+extension-pkg-allow-list=black,
+                         black.mode
+
+# A comma-separated list of package or module names from where C extensions may
+# be loaded. Extensions are loading into the active Python interpreter and may
+# run arbitrary code. (This is an alternative name to extension-pkg-allow-list
+# for backward compatibility.)
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
-# paths.
+# Return non-zero exit code if any of these messages/categories are detected,
+# even if score is above --fail-under value. Syntax same as enable. Messages
+# specified are enabled, while categories only check already-enabled messages.
+fail-on=
+
+# Specify a score threshold under which the program will exit with error.
+fail-under=10
+
+# Interpret the stdin as a python script, whose filename needs to be passed as
+# the module_or_package argument.
+#from-stdin=
+
+# Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
-# regex matches against base names, not paths.
+# Add files or directories matching the regular expressions patterns to the
+# ignore-list. The regex matches against paths and can be in Posix or Windows
+# format. Because '\\' represents the directory delimiter on Windows systems,
+# it can't be used as an escape character.
+ignore-paths=
+
+# Files or directories matching the regular expression patterns are skipped.
+# The regex matches against base names, not paths. The default value ignores
+# Emacs file locks
 ignore-patterns=
 
+# List of module names for which member attributes should not be checked
+# (useful for modules/projects where namespaces are manipulated during runtime
+# and thus existing member attributes cannot be deduced by static analysis). It
+# supports qualified module names, as well as Unix pattern matching.
+ignored-modules=
+
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
-# number of processors available to use.
+# number of processors available to use, and will cap the count on Windows to
+# avoid hangs.
 jobs=1
 
 # Control the amount of potential inferred values when inferring a single
 # object. This can help the performance when dealing with large functions or
 # complex, nested conditions.
 limit-inference-results=100
 
-# List of plugins (as comma separated values of python modules names) to load,
+# List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
 load-plugins=
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
-# Specify a configuration file.
-#rcfile=
+# Minimum Python version to use for version dependent checks. Will default to
+# the version used to run pylint.
+py-version=3.11
+
+# Discover python modules and packages in the file system subtree.
+recursive=no
+
+# Add paths to the list of the source roots. Supports globbing patterns. The
+# source root is an absolute path or a path relative to the current working
+# directory used to determine a package namespace for modules located under the
+# source root.
+source-roots=
 
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
 unsafe-load-any-extension=no
 
-
-[MESSAGES CONTROL]
-
-# Only show warnings with the listed confidence levels. Leave empty to show
-# all. Valid levels: HIGH, INFERENCE, INFERENCE_FAILURE, UNDEFINED.
-confidence=
-
-# Disable the message, report, category or checker with the given id(s). You
-# can either give multiple identifiers separated by comma (,) or put this
-# option multiple times (only on the command line, not in the configuration
-# file where it should appear only once). You can also use "--disable=all" to
-# disable everything first and then reenable specific checks. For example, if
-# you want to run only the similarities checker, you can use "--disable=all
-# --enable=similarities". If you want to run only the classes checker, but have
-# no Warning level messages displayed, use "--disable=all --enable=classes
-# --disable=W".
-disable=print-statement,
-        parameter-unpacking,
-        unpacking-in-except,
-        old-raise-syntax,
-        backtick,
-        long-suffix,
-        old-ne-operator,
-        old-octal-literal,
-        import-star-module-level,
-        non-ascii-bytes-literal,
-        raw-checker-failed,
-        bad-inline-option,
-        locally-disabled,
-        locally-enabled,
-        file-ignored,
-        suppressed-message,
-        useless-suppression,
-        deprecated-pragma,
-        use-symbolic-message-instead,
-        apply-builtin,
-        basestring-builtin,
-        buffer-builtin,
-        cmp-builtin,
-        coerce-builtin,
-        execfile-builtin,
-        file-builtin,
-        long-builtin,
-        raw_input-builtin,
-        reduce-builtin,
-        standarderror-builtin,
-        unicode-builtin,
-        xrange-builtin,
-        coerce-method,
-        delslice-method,
-        getslice-method,
-        setslice-method,
-        no-absolute-import,
-        old-division,
-        dict-iter-method,
-        dict-view-method,
-        next-method-called,
-        metaclass-assignment,
-        indexing-exception,
-        raising-string,
-        reload-builtin,
-        oct-method,
-        hex-method,
-        nonzero-method,
-        cmp-method,
-        input-builtin,
-        round-builtin,
-        intern-builtin,
-        unichr-builtin,
-        map-builtin-not-iterating,
-        zip-builtin-not-iterating,
-        range-builtin-not-iterating,
-        filter-builtin-not-iterating,
-        using-cmp-argument,
-        eq-without-hash,
-        div-method,
-        idiv-method,
-        rdiv-method,
-        exception-message-attribute,
-        invalid-str-codec,
-        sys-max-int,
-        bad-python3-import,
-        deprecated-string-function,
-        deprecated-str-translate-call,
-        deprecated-itertools-function,
-        deprecated-types-field,
-        next-method-defined,
-        dict-items-not-iterating,
-        dict-keys-not-iterating,
-        dict-values-not-iterating,
-        deprecated-operator-function,
-        deprecated-urllib-function,
-        xreadlines-attribute,
-        deprecated-sys-function,
-        exception-escape,
-        comprehension-escape,
-        useless-object-inheritance,
-	bad-continuation,
-        bad-whitespace
-
-# Enable the message, report, category or checker with the given id(s). You can
-# either give multiple identifier separated by comma (,) or put this option
-# multiple time (only on the command line, not in the configuration file where
-# it should appear only once). See also the "--disable" option for examples.
-enable=c-extension-no-member
-
-
-[REPORTS]
-
-# Python expression which should return a note less than 10 (10 is the highest
-# note). You have access to the variables errors warning, statement which
-# respectively contain the number of errors / warnings messages and the total
-# number of statements analyzed. This is used by the global evaluation report
-# (RP0004).
-evaluation=10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10)
-
-# Template used to display messages. This is a python new-style format string
-# used to format the message information. See doc for all details.
-#msg-template=
-
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
-# mypackage.mymodule.MyReporterClass.
-output-format=text
-
-# Tells whether to display a full report or only the messages.
-reports=no
-
-# Activate the evaluation score.
-score=yes
-
-
-[REFACTORING]
-
-# Maximum number of nested blocks for function / method body
-max-nested-blocks=5
-
-# Complete name of functions that never returns. When checking for
-# inconsistent-return-statements if a never returning function is called then
-# it will be considered as an explicit return statement and no message will be
-# printed.
-never-returning-functions=sys.exit
-
-
-[SPELLING]
-
-# Limits count of emitted suggestions for spelling mistakes.
-max-spelling-suggestions=4
-
-# Spelling dictionary name. Available dictionaries: none. To make it working
-# install python-enchant package..
-spelling-dict=
-
-# List of comma separated words that should not be checked.
-spelling-ignore-words=
-
-# A path to a file that contains private dictionary; one word per line.
-spelling-private-dict-file=
-
-# Tells whether to store unknown words to indicated private dictionary in
-# --spelling-private-dict-file option instead of raising a message.
-spelling-store-unknown-words=no
+# In verbose mode, extra non-checker-related info will be displayed.
+#verbose=
 
 
 [BASIC]
 
 # Naming style matching correct argument names.
 argument-naming-style=snake_case
 
 # Regular expression matching correct argument names. Overrides argument-
-# naming-style.
+# naming-style. If left empty, argument names will be checked with the set
+# naming style.
 #argument-rgx=
 
 # Naming style matching correct attribute names.
 attr-naming-style=snake_case
 
 # Regular expression matching correct attribute names. Overrides attr-naming-
+# style. If left empty, attribute names will be checked with the set naming
 # style.
 #attr-rgx=
 
 # Bad variable names which should always be refused, separated by a comma.
 bad-names=foo,
           bar,
           baz,
           toto,
           tutu,
           tata
 
+# Bad variable names regexes, separated by a comma. If names match any regex,
+# they will always be refused
+bad-names-rgxs=
+
 # Naming style matching correct class attribute names.
 class-attribute-naming-style=any
 
 # Regular expression matching correct class attribute names. Overrides class-
-# attribute-naming-style.
+# attribute-naming-style. If left empty, class attribute names will be checked
+# with the set naming style.
 #class-attribute-rgx=
 
+# Naming style matching correct class constant names.
+class-const-naming-style=UPPER_CASE
+
+# Regular expression matching correct class constant names. Overrides class-
+# const-naming-style. If left empty, class constant names will be checked with
+# the set naming style.
+#class-const-rgx=
+
 # Naming style matching correct class names.
 class-naming-style=PascalCase
 
 # Regular expression matching correct class names. Overrides class-naming-
-# style.
+# style. If left empty, class names will be checked with the set naming style.
 #class-rgx=
 
 # Naming style matching correct constant names.
 const-naming-style=UPPER_CASE
 
 # Regular expression matching correct constant names. Overrides const-naming-
+# style. If left empty, constant names will be checked with the set naming
 # style.
 #const-rgx=
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
 # Naming style matching correct function names.
 function-naming-style=snake_case
 
 # Regular expression matching correct function names. Overrides function-
-# naming-style.
+# naming-style. If left empty, function names will be checked with the set
+# naming style.
 #function-rgx=
 
 # Good variable names which should always be accepted, separated by a comma.
 good-names=i,
            j,
            k,
            ex,
            Run,
            _
 
+# Good variable names regexes, separated by a comma. If names match any regex,
+# they will always be accepted
+good-names-rgxs=
+
 # Include a hint for the correct naming format with invalid-name.
 include-naming-hint=no
 
 # Naming style matching correct inline iteration names.
 inlinevar-naming-style=any
 
 # Regular expression matching correct inline iteration names. Overrides
-# inlinevar-naming-style.
+# inlinevar-naming-style. If left empty, inline iteration names will be checked
+# with the set naming style.
 #inlinevar-rgx=
 
 # Naming style matching correct method names.
 method-naming-style=snake_case
 
 # Regular expression matching correct method names. Overrides method-naming-
-# style.
+# style. If left empty, method names will be checked with the set naming style.
 #method-rgx=
 
 # Naming style matching correct module names.
 module-naming-style=snake_case
 
 # Regular expression matching correct module names. Overrides module-naming-
-# style.
+# style. If left empty, module names will be checked with the set naming style.
 #module-rgx=
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
 # Regular expression which should only match function or class names that do
@@ -305,257 +231,405 @@
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 # These decorators are taken in consideration only for invalid-name.
 property-classes=abc.abstractproperty
 
+# Regular expression matching correct type alias names. If left empty, type
+# alias names will be checked with the set naming style.
+#typealias-rgx=
+
+# Regular expression matching correct type variable names. If left empty, type
+# variable names will be checked with the set naming style.
+#typevar-rgx=
+
 # Naming style matching correct variable names.
 variable-naming-style=snake_case
 
 # Regular expression matching correct variable names. Overrides variable-
-# naming-style.
+# naming-style. If left empty, variable names will be checked with the set
+# naming style.
 #variable-rgx=
 
 
-[LOGGING]
-
-# Logging modules to check that the string format arguments are in logging
-# function parameter format.
-logging-modules=logging
-
-
-[VARIABLES]
-
-# List of additional names supposed to be defined in builtins. Remember that
-# you should avoid to define new builtins when possible.
-additional-builtins=
-
-# Tells whether unused global variables should be treated as a violation.
-allow-global-unused-variables=yes
-
-# List of strings which can identify a callback function by name. A callback
-# name must start or end with one of those strings.
-callbacks=cb_,
-          _cb
-
-# A regular expression matching the name of dummy variables (i.e. expected to
-# not be used).
-dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
-
-# Argument names that match this expression will be ignored. Default to name
-# with leading underscore.
-ignored-argument-names=_.*|^ignored_|^unused_
+[CLASSES]
 
-# Tells whether we should check for unused import in __init__ files.
-init-import=no
-
-# List of qualified module names which can have objects that can redefine
-# builtins.
-redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
+# Warn about protected attribute access inside special methods
+check-protected-access-in-special-methods=no
 
+# List of method names used to declare (i.e. assign) instance attributes.
+defining-attr-methods=__init__,
+                      __new__,
+                      setUp
 
-[SIMILARITIES]
+# List of member names, which should be excluded from the protected access
+# warning.
+exclude-protected=_asdict,
+                  _fields,
+                  _replace,
+                  _source,
+                  _make
 
-# Ignore comments when computing similarities.
-ignore-comments=yes
+# List of valid names for the first argument in a class method.
+valid-classmethod-first-arg=cls
 
-# Ignore docstrings when computing similarities.
-ignore-docstrings=yes
+# List of valid names for the first argument in a metaclass class method.
+valid-metaclass-classmethod-first-arg=cls
 
-# Ignore imports when computing similarities.
-ignore-imports=no
 
-# Minimum lines number of a similarity.
-min-similarity-lines=4
+[DESIGN]
 
+# List of regular expressions of class ancestor names to ignore when counting
+# public methods (see R0903)
+exclude-too-few-public-methods=
+
+# List of qualified class names to ignore when counting class parents (see
+# R0901)
+ignored-parents=
 
-[TYPECHECK]
+# Maximum number of arguments for function / method.
+max-args=5
 
-# List of decorators that produce context managers, such as
-# contextlib.contextmanager. Add to this list to register other decorators that
-# produce valid context managers.
-contextmanager-decorators=contextlib.contextmanager
+# Maximum number of attributes for a class (see R0902).
+max-attributes=7
 
-# List of members which are set dynamically and missed by pylint inference
-# system, and so shouldn't trigger E1101 when accessed. Python regular
-# expressions are accepted.
-generated-members=
+# Maximum number of boolean expressions in an if statement (see R0916).
+max-bool-expr=5
 
-# Tells whether missing members accessed in mixin class should be ignored. A
-# mixin class is detected if its name ends with "mixin" (case insensitive).
-ignore-mixin-members=yes
+# Maximum number of branch for function / method body.
+max-branches=12
 
-# Tells whether to warn about missing members when the owner of the attribute
-# is inferred to be None.
-ignore-none=yes
+# Maximum number of locals for function / method body.
+max-locals=15
 
-# This flag controls whether pylint should warn about no-member and similar
-# checks whenever an opaque object is returned when inferring. The inference
-# can return multiple potential results while evaluating a Python object, but
-# some branches might not be evaluated, which results in partial inference. In
-# that case, it might be useful to still emit no-member and other checks for
-# the rest of the inferred objects.
-ignore-on-opaque-inference=yes
+# Maximum number of parents for a class (see R0901).
+max-parents=7
 
-# List of class names for which member attributes should not be checked (useful
-# for classes with dynamically set attributes). This supports the use of
-# qualified names.
-ignored-classes=optparse.Values,thread._local,_thread._local
+# Maximum number of public methods for a class (see R0904).
+max-public-methods=20
 
-# List of module names for which member attributes should not be checked
-# (useful for modules/projects where namespaces are manipulated during runtime
-# and thus existing member attributes cannot be deduced by static analysis. It
-# supports qualified module names, as well as Unix pattern matching.
-ignored-modules=
+# Maximum number of return / yield for function / method body.
+max-returns=6
 
-# Show a hint with possible names when a member name was not found. The aspect
-# of finding the hint is based on edit distance.
-missing-member-hint=yes
+# Maximum number of statements in function / method body.
+max-statements=50
 
-# The minimum edit distance a name should have in order to be considered a
-# similar match for a missing member name.
-missing-member-hint-distance=1
+# Minimum number of public methods for a class (see R0903).
+min-public-methods=2
 
-# The total number of similar names that should be taken in consideration when
-# showing a hint for a missing member.
-missing-member-max-choices=1
 
+[EXCEPTIONS]
 
-[MISCELLANEOUS]
-
-# List of note tags to take in consideration, separated by a comma.
-notes=FIXME,
-      XXX,
-      TODO
+# Exceptions that will emit a warning when caught.
+overgeneral-exceptions=builtins.BaseException,builtins.Exception
 
 
 [FORMAT]
 
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 expected-line-ending-format=
 
 # Regexp for a line that is allowed to be longer than the limit.
 ignore-long-lines=^\s*(# )?<?https?://\S+>?$
 
-# Number of spaces of indent required inside a hanging  or continued line.
+# Number of spaces of indent required inside a hanging or continued line.
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,
-               dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
 
 
 [IMPORTS]
 
+# List of modules that can be imported at any level, not just the top level
+# one.
+allow-any-import-level=
+
+# Allow explicit reexports by alias from a package __init__.
+allow-reexport-from-package=no
+
 # Allow wildcard imports from modules that define __all__.
 allow-wildcard-with-all=no
 
-# Analyse import fallback blocks. This can be used to support both Python 2 and
-# 3 compatible code, which means that the block might have code that exists
-# only in one or another interpreter, leading to false positives when analysed.
-analyse-fallback-blocks=no
-
 # Deprecated modules which should not be used, separated by a comma.
 deprecated-modules=optparse,tkinter.tix
 
-# Create a graph of external dependencies in the given file (report RP0402 must
-# not be disabled).
+# Output a graph (.gv or any supported image format) of external dependencies
+# to the given file (report RP0402 must not be disabled).
 ext-import-graph=
 
-# Create a graph of every (i.e. internal and external) dependencies in the
-# given file (report RP0402 must not be disabled).
+# Output a graph (.gv or any supported image format) of all (i.e. internal and
+# external) dependencies to the given file (report RP0402 must not be
+# disabled).
 import-graph=
 
-# Create a graph of internal dependencies in the given file (report RP0402 must
-# not be disabled).
+# Output a graph (.gv or any supported image format) of internal dependencies
+# to the given file (report RP0402 must not be disabled).
 int-import-graph=
 
 # Force import order to recognize a module as part of the standard
 # compatibility libraries.
 known-standard-library=
 
 # Force import order to recognize a module as part of a third party library.
 known-third-party=enchant
 
+# Couples of modules and preferred modules, separated by a comma.
+preferred-modules=
 
-[DESIGN]
 
-# Maximum number of arguments for function / method.
-max-args=5
+[LOGGING]
 
-# Maximum number of attributes for a class (see R0902).
-max-attributes=7
+# The type of string formatting that logging methods do. `old` means using %
+# formatting, `new` is for `{}` formatting.
+logging-format-style=old
 
-# Maximum number of boolean expressions in an if statement.
-max-bool-expr=5
+# Logging modules to check that the string format arguments are in logging
+# function parameter format.
+logging-modules=logging
 
-# Maximum number of branch for function / method body.
-max-branches=12
 
-# Maximum number of locals for function / method body.
-max-locals=15
+[MESSAGES CONTROL]
 
-# Maximum number of parents for a class (see R0901).
-max-parents=7
+# Only show warnings with the listed confidence levels. Leave empty to show
+# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
+# UNDEFINED.
+confidence=HIGH,
+           CONTROL_FLOW,
+           INFERENCE,
+           INFERENCE_FAILURE,
+           UNDEFINED
 
-# Maximum number of public methods for a class (see R0904).
-max-public-methods=20
+# Disable the message, report, category or checker with the given id(s). You
+# can either give multiple identifiers separated by comma (,) or put this
+# option multiple times (only on the command line, not in the configuration
+# file where it should appear only once). You can also use "--disable=all" to
+# disable everything first and then re-enable specific checks. For example, if
+# you want to run only the similarities checker, you can use "--disable=all
+# --enable=similarities". If you want to run only the classes checker, but have
+# no Warning level messages displayed, use "--disable=all --enable=classes
+# --disable=W".
+disable=raw-checker-failed,
+        bad-inline-option,
+        locally-disabled,
+        file-ignored,
+        suppressed-message,
+        useless-suppression,
+        deprecated-pragma,
+        use-symbolic-message-instead,
+        useless-object-inheritance
 
-# Maximum number of return / yield for function / method body.
-max-returns=6
+# Enable the message, report, category or checker with the given id(s). You can
+# either give multiple identifier separated by comma (,) or put this option
+# multiple time (only on the command line, not in the configuration file where
+# it should appear only once). See also the "--disable" option for examples.
+enable=c-extension-no-member
 
-# Maximum number of statements in function / method body.
-max-statements=50
 
-# Minimum number of public methods for a class (see R0903).
-min-public-methods=2
+[METHOD_ARGS]
 
+# List of qualified names (i.e., library.method) which require a timeout
+# parameter e.g. 'requests.api.get,requests.api.post'
+timeout-methods=requests.api.delete,requests.api.get,requests.api.head,requests.api.options,requests.api.patch,requests.api.post,requests.api.put,requests.api.request
 
-[CLASSES]
 
-# List of method names used to declare (i.e. assign) instance attributes.
-defining-attr-methods=__init__,
-                      __new__,
-                      setUp
+[MISCELLANEOUS]
 
-# List of member names, which should be excluded from the protected access
-# warning.
-exclude-protected=_asdict,
-                  _fields,
-                  _replace,
-                  _source,
-                  _make
+# List of note tags to take in consideration, separated by a comma.
+notes=FIXME,
+      XXX,
+      TODO
 
-# List of valid names for the first argument in a class method.
-valid-classmethod-first-arg=cls
+# Regular expression of note tags to take in consideration.
+notes-rgx=
 
-# List of valid names for the first argument in a metaclass class method.
-valid-metaclass-classmethod-first-arg=cls
 
+[REFACTORING]
 
-[EXCEPTIONS]
+# Maximum number of nested blocks for function / method body
+max-nested-blocks=5
+
+# Complete name of functions that never returns. When checking for
+# inconsistent-return-statements if a never returning function is called then
+# it will be considered as an explicit return statement and no message will be
+# printed.
+never-returning-functions=sys.exit
+
+
+[REPORTS]
+
+# Python expression which should return a score less than or equal to 10. You
+# have access to the variables 'fatal', 'error', 'warning', 'refactor',
+# 'convention', and 'info' which contain the number of messages in each
+# category, as well as 'statement' which is the total number of statements
+# analyzed. This score is used by the global evaluation report (RP0004).
+evaluation=10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10)
+
+# Template used to display messages. This is a python new-style format string
+# used to format the message information. See doc for all details.
+msg-template=
+
+# Set the output format. Available formats are text, parseable, colorized, json
+# and msvs (visual studio). You can also give a reporter class, e.g.
+# mypackage.mymodule.MyReporterClass.
+#output-format=
+
+# Tells whether to display a full report or only the messages.
+reports=no
+
+# Activate the evaluation score.
+score=yes
 
-# Exceptions that will emit a warning when being caught. Defaults to
-# "Exception".
-overgeneral-exceptions=Exception
+
+[SIMILARITIES]
+
+# Comments are removed from the similarity computation
+ignore-comments=yes
+
+# Docstrings are removed from the similarity computation
+ignore-docstrings=yes
+
+# Imports are removed from the similarity computation
+ignore-imports=no
+
+# Signatures are removed from the similarity computation
+ignore-signatures=yes
+
+# Minimum lines number of a similarity.
+min-similarity-lines=4
+
+
+[SPELLING]
+
+# Limits count of emitted suggestions for spelling mistakes.
+max-spelling-suggestions=4
+
+# Spelling dictionary name. No available dictionaries : You need to install
+# both the python package and the system dependency for enchant to work..
+spelling-dict=
+
+# List of comma separated words that should be considered directives if they
+# appear at the beginning of a comment and should not be checked.
+spelling-ignore-comment-directives=fmt: on,fmt: off,noqa:,noqa,nosec,isort:skip,mypy:
+
+# List of comma separated words that should not be checked.
+spelling-ignore-words=
+
+# A path to a file that contains the private dictionary; one word per line.
+spelling-private-dict-file=
+
+# Tells whether to store unknown words to the private dictionary (see the
+# --spelling-private-dict-file option) instead of raising a message.
+spelling-store-unknown-words=no
+
+
+[STRING]
+
+# This flag controls whether inconsistent-quotes generates a warning when the
+# character used as a quote delimiter is used inconsistently within a module.
+check-quote-consistency=no
+
+# This flag controls whether the implicit-str-concat should generate a warning
+# on implicit string concatenation in sequences defined over several lines.
+check-str-concat-over-line-jumps=no
+
+
+[TYPECHECK]
+
+# List of decorators that produce context managers, such as
+# contextlib.contextmanager. Add to this list to register other decorators that
+# produce valid context managers.
+contextmanager-decorators=contextlib.contextmanager
+
+# List of members which are set dynamically and missed by pylint inference
+# system, and so shouldn't trigger E1101 when accessed. Python regular
+# expressions are accepted.
+generated-members=
+
+# Tells whether to warn about missing members when the owner of the attribute
+# is inferred to be None.
+ignore-none=yes
+
+# This flag controls whether pylint should warn about no-member and similar
+# checks whenever an opaque object is returned when inferring. The inference
+# can return multiple potential results while evaluating a Python object, but
+# some branches might not be evaluated, which results in partial inference. In
+# that case, it might be useful to still emit no-member and other checks for
+# the rest of the inferred objects.
+ignore-on-opaque-inference=yes
+
+# List of symbolic message names to ignore for Mixin members.
+ignored-checks-for-mixins=no-member,
+                          not-async-context-manager,
+                          not-context-manager,
+                          attribute-defined-outside-init
+
+# List of class names for which member attributes should not be checked (useful
+# for classes with dynamically set attributes). This supports the use of
+# qualified names.
+ignored-classes=optparse.Values,thread._local,_thread._local
+
+# Show a hint with possible names when a member name was not found. The aspect
+# of finding the hint is based on edit distance.
+missing-member-hint=yes
+
+# The minimum edit distance a name should have in order to be considered a
+# similar match for a missing member name.
+missing-member-hint-distance=1
+
+# The total number of similar names that should be taken in consideration when
+# showing a hint for a missing member.
+missing-member-max-choices=1
+
+# Regex pattern to define which classes are considered mixins.
+mixin-class-rgx=.*[Mm]ixin
+
+# List of decorators that change the signature of a decorated function.
+signature-mutators=
+
+
+[VARIABLES]
+
+# List of additional names supposed to be defined in builtins. Remember that
+# you should avoid defining new builtins when possible.
+additional-builtins=
+
+# Tells whether unused global variables should be treated as a violation.
+allow-global-unused-variables=yes
+
+# List of names allowed to shadow builtins
+allowed-redefined-builtins=
+
+# List of strings which can identify a callback function by name. A callback
+# name must start or end with one of those strings.
+callbacks=cb_,
+          _cb
+
+# A regular expression matching the name of dummy variables (i.e. expected to
+# not be used).
+dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
+
+# Argument names that match this expression will be ignored.
+ignored-argument-names=_.*|^ignored_|^unused_
+
+# Tells whether we should check for unused import in __init__ files.
+init-import=no
+
+# List of qualified module names which can have objects that can redefine
+# builtins.
+redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
```

### Comparing `schema-salad-8.4.20230213094415/.readthedocs.yml` & `schema-salad-8.4.20230426093816/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/CONTRIBUTING.md` & `schema-salad-8.4.20230426093816/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/LICENSE.txt` & `schema-salad-8.4.20230426093816/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/MANIFEST.in` & `schema-salad-8.4.20230426093816/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/Makefile` & `schema-salad-8.4.20230426093816/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/PKG-INFO` & `schema-salad-8.4.20230426093816/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230213094415
+Version: 8.4.20230426093816
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.4.20230213094415/README.rst` & `schema-salad-8.4.20230426093816/README.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/docs/Makefile` & `schema-salad-8.4.20230426093816/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/docs/_static/favicon.ico` & `schema-salad-8.4.20230426093816/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/docs/conf.py` & `schema-salad-8.4.20230426093816/docs/conf.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/docs/make.bat` & `schema-salad-8.4.20230426093816/docs/make.bat`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/docs/typeshed.rst` & `schema-salad-8.4.20230426093816/docs/typeshed.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/manual_wheel_publish.sh` & `schema-salad-8.4.20230426093816/manual_wheel_publish.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/cachecontrol/wrapper.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/cachecontrol/wrapper.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/mistune/__init__.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/mistune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/mistune/block_parser.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/mistune/block_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/mistune/inline_parser.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/mistune/inline_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/mistune/markdown.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/mistune/markdown.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/mistune/plugins/table.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/mistune/plugins/table.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/mistune/renderers.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/mistune/renderers.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/mistune/scanner.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/mistune/scanner.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/__init__.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/collection.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/graph.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_ORG.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_OWL.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_PROV.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_QB.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_RDF.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SDO.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SH.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_SSN.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_TIME.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_VOID.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/_XSD.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/namespace/__init__.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/paths.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/plugin.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/plugin.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/query.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/resource.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/mypy-stubs/rdflib/term.pyi` & `schema-salad-8.4.20230426093816/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/pyproject.toml` & `schema-salad-8.4.20230426093816/pyproject.toml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/release-test.sh` & `schema-salad-8.4.20230426093816/release-test.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/avro/LICENSE` & `schema-salad-8.4.20230426093816/schema_salad/avro/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/avro/__init__.py` & `schema-salad-8.4.20230426093816/schema_salad/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/avro/schema.py` & `schema-salad-8.4.20230426093816/schema_salad/avro/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     def __init__(self, atype: str, other_props: Optional[PropsType] = None) -> None:
         # Ensure valid ctor args
         if not isinstance(atype, str):
             raise SchemaParseException(
                 f"Schema type {atype!r} must be a string, was {type(atype)!r}."
             )
-        elif atype not in VALID_TYPES:
+        if atype not in VALID_TYPES:
             fail_msg = f"{atype} is not a valid type."
             raise SchemaParseException(fail_msg)
 
         # add members
         if not hasattr(self, "_props"):
             self._props: PropsType = {}
         self.set_prop("type", atype)
@@ -173,16 +173,15 @@
     def get_space(self) -> Optional[str]:
         """Back out a namespace from full name."""
         if self._full is None:
             return None
 
         if self._full.find(".") > 0:
             return self._full.rsplit(".", 1)[0]
-        else:
-            return None
+        return None
 
 
 class Names:
     """Track name set and default namespace during parsing."""
 
     def __init__(self, default_namespace: Optional[str] = None) -> None:
         self.names: Dict[str, NamedSchema] = {}
@@ -211,18 +210,18 @@
         :returns: the Name that was just added.
         """
         to_add = Name(name_attr, space_attr, self.default_namespace)
 
         if to_add.fullname in VALID_TYPES:
             fail_msg = f"{to_add.fullname} is a reserved type name."
             raise SchemaParseException(fail_msg)
-        elif to_add.fullname in self.names:
+        if to_add.fullname in self.names:
             fail_msg = f"The name {to_add.fullname!r} is already in use."
             raise SchemaParseException(fail_msg)
-        elif to_add.fullname is None:
+        if to_add.fullname is None:
             fail_msg = f"{to_add.fullname} is missing, but this is impossible."
             raise SchemaParseException(fail_msg)
 
         self.names[to_add.fullname] = new_schema
         return to_add
 
 
@@ -236,17 +235,17 @@
         namespace: Optional[str] = None,
         names: Optional[Names] = None,
         other_props: Optional[PropsType] = None,
     ) -> None:
         # Ensure valid ctor args
         if not name:
             raise SchemaParseException("Named Schemas must have a non-empty name.")
-        elif not isinstance(name, str):
+        if not isinstance(name, str):
             raise SchemaParseException("The name property must be a string.")
-        elif namespace is not None and not isinstance(namespace, str):
+        if namespace is not None and not isinstance(namespace, str):
             raise SchemaParseException("The namespace property must be a string.")
         if names is None:
             raise SchemaParseException("Must provide Names.")
 
         # Call parent ctor
         Schema.__init__(self, atype, other_props)
 
@@ -280,18 +279,18 @@
         doc: Optional[Union[str, List[str]]] = None,
         other_props: Optional[PropsType] = None,
     ) -> None:
         # Ensure valid ctor args
         if not name:
             fail_msg = "Fields must have a non-empty name."
             raise SchemaParseException(fail_msg)
-        elif not isinstance(name, str):
+        if not isinstance(name, str):
             fail_msg = "The name property must be a string."  # type: ignore[unreachable]
             raise SchemaParseException(fail_msg)
-        elif order is not None and order not in VALID_FIELD_SORT_ORDERS:
+        if order is not None and order not in VALID_FIELD_SORT_ORDERS:
             fail_msg = f"The order property {order} is not valid."
             raise SchemaParseException(fail_msg)
 
         # add members
         self._props: PropsType = {}
         self._has_default = has_default
         self._props.update(other_props or {})
@@ -361,17 +360,17 @@
         names: Optional[Names] = None,
         doc: Optional[Union[str, List[str]]] = None,
         other_props: Optional[PropsType] = None,
     ) -> None:
         # Ensure valid ctor args
         if not isinstance(symbols, list):
             raise AvroException("Enum Schema requires a JSON array for the symbols property.")
-        elif False in [isinstance(s, str) for s in symbols]:
+        if False in [isinstance(s, str) for s in symbols]:
             raise AvroException("Enum Schema requires all symbols to be JSON strings.")
-        elif len(set(symbols)) < len(symbols):
+        if len(set(symbols)) < len(symbols):
             raise AvroException(f"Duplicate symbol: {symbols}")
 
         # Call parent ctor
         NamedSchema.__init__(self, "enum", name, namespace, names, other_props)
 
         # Add class members
         self.set_prop("symbols", symbols)
@@ -453,18 +452,17 @@
             # check the new schema
             if (
                 new_schema.type in VALID_TYPES
                 and new_schema.type not in NAMED_TYPES
                 and new_schema.type in [schema.type for schema in schema_objects]
             ):
                 raise SchemaParseException(f"{new_schema.type} type already in Union")
-            elif new_schema.type == "union":
+            if new_schema.type == "union":
                 raise SchemaParseException("Unions cannot contain other unions.")
-            else:
-                schema_objects.append(new_schema)
+            schema_objects.append(new_schema)
         self._schemas = schema_objects
 
     # read-only properties
     @property
     def schemas(self) -> List[Schema]:
         return self._schemas
 
@@ -486,18 +484,17 @@
                 if "default" in field:
                     has_default = True
                     default = field.get("default")
                 order = field.get("order")
                 if not (order is None or isinstance(order, str)):
                     raise SchemaParseException('"order" must be a string or None')
                 doc = field.get("doc")
-                if not (doc is None or isinstance(doc, str) or isinstance(doc, list)):
+                if not (doc is None or isinstance(doc, (list, str))):
                     raise SchemaParseException('"doc" must be a string, list of strings, or None')
-                else:
-                    doc = cast(Union[str, List[str], None], doc)
+                doc = cast(Union[str, List[str], None], doc)
                 other_props = get_other_props(field, FIELD_RESERVED_PROPS)
                 new_field = Field(atype, name, has_default, default, order, names, doc, other_props)
                 parsed_fields[new_field.name] = field
             else:
                 raise SchemaParseException(f"Not a valid field: {field}")
             field_objects.append(new_field)
         return field_objects
@@ -579,38 +576,34 @@
             doc = json_data.get("doc")
             if not isinstance(name, str):
                 raise SchemaParseException(f'"name" for type {atype} must be a string: {json_data}')
             if not (namespace is None or isinstance(namespace, str)):
                 raise SchemaParseException(
                     f'"namespace" for type {atype} must be a string or None: {json_data}'
                 )
-            if not (doc is None or isinstance(doc, str) or isinstance(doc, list)):
+            if not (doc is None or isinstance(doc, (str, list))):
                 raise SchemaParseException(
                     f'"doc" for type {atype} must be a string, '
                     f"a list of strings, or None: {json_data}"
                 )
             if atype == "enum":
                 symbols = json_data.get("symbols")
                 if not isinstance(symbols, list):
                     raise SchemaParseException(
                         f'"symbols" for type enum must be a list of strings: {json_data}'
                     )
-                else:
-                    symbols = cast(List[str], symbols)
+                symbols = cast(List[str], symbols)
                 return EnumSchema(name, namespace, symbols, names, doc, other_props)
             if atype in ["record", "error"]:
                 fields = json_data.get("fields", [])
                 if not isinstance(fields, list):
                     raise SchemaParseException(
-                        '"fields" for type {} must be a list of mappings: {}'.format(
-                            atype, json_data
-                        )
+                        f'"fields" for type {atype} must be a list of mappings: {json_data}'
                     )
-                else:
-                    fields = cast(List[PropsType], fields)
+                fields = cast(List[PropsType], fields)
                 return RecordSchema(name, namespace, fields, names, atype, doc, other_props)
             raise SchemaParseException(f"Unknown Named Type: {atype}")
         if atype in VALID_TYPES:
             if atype == "array":
                 items = json_data.get("items")
                 return ArraySchema(items, names, other_props)
         if atype is None:
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/codegen.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,42 +53,41 @@
     sp = urlsplit(base)
     pkg = (
         package
         if package
         else ".".join(list(reversed(sp.netloc.split("."))) + sp.path.strip("/").split("/"))
     )
     info = parser_info or pkg
-    if lang == "python" or lang == "cpp" or lang == "dlang":
+    if lang in set(["python", "cpp", "dlang"]):
         if target:
             dest: Union[TextIOWrapper, TextIO] = open(target, mode="w", encoding="utf-8")
         else:
             dest = sys.stdout
         if lang == "cpp":
             gen = CppCodeGen(
                 base,
                 dest,
                 examples,
                 pkg,
                 copyright,
             )
             gen.parse(j)
             return
-        elif lang == "dlang":
+        if lang == "dlang":
             gen = DlangCodeGen(
                 base,
                 dest,
                 examples,
                 pkg,
                 copyright,
                 info,
             )
             gen.parse(j)
             return
-        else:
-            gen = PythonCodeGen(dest, copyright=copyright, parser_info=info)
+        gen = PythonCodeGen(dest, copyright=copyright, parser_info=info)
 
     elif lang == "java":
         gen = JavaCodeGen(
             base,
             target=target,
             examples=examples,
             package=pkg,
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/codegen_base.py` & `schema-salad-8.4.20230426093816/schema_salad/codegen_base.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/cpp_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dlang_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/LICENSE` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Project.csproj.template` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Project.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Solution.sln` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Solution.sln`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/FetcherTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/FetcherTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/UtilitiesTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/UtilitiesTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/Test.csproj.template` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/Test.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/docfx.json` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/docfx.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/editorconfig` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/editorconfig`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/gitignore` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Fetcher.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Fetcher.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/ArrayLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ArrayLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/EnumLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/EnumLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/IdMapLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/IdMapLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/Loader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/Loader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/RecordLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RecordLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/RootLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/RootLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/UnionLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UnionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Loaders/UriLoader.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Loaders/UriLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/LoadingOptions.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/LoadingOptions.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Saveable.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Saveable.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/Utilities.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/Utilities.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet/util/ValidationException.cs` & `schema-salad-8.4.20230426093816/schema_salad/dotnet/util/ValidationException.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/dotnet_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/exceptions.py` & `schema-salad-8.4.20230426093816/schema_salad/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         else:
             self.file = None
             self.start = None
             self.end = None
         return self
 
     def leaves(self) -> List["SchemaSaladException"]:
-        if len(self.children):
+        if len(self.children) > 0:
             return sum((c.leaves() for c in self.children), [])
         if len(self.message):
             return [self]
         return []
 
     def prefix(self) -> str:
         pre: str = ""
@@ -89,31 +89,30 @@
             pre = f"{self.file}:{linecol0}:{linecol1}: "
 
         return pre + "Warning: " if self.is_warning else pre
 
     def summary(self, level: int = 0, with_bullet: bool = False) -> str:
         indent_per_level = 2
         spaces = (level * indent_per_level) * " "
-        bullet = self.bullet + " " if len(self.bullet) and with_bullet else ""
+        bullet = self.bullet + " " if len(self.bullet) > 0 and with_bullet else ""
         return f"{self.prefix()}{spaces}{bullet}{self.message}"
 
     def __str__(self) -> str:
         """Convert to a string using :py:meth:`pretty_str`."""
         return str(self.pretty_str())
 
     def pretty_str(self, level: int = 0) -> str:
         messages = len(self.message)
         my_summary = [self.summary(level, True)] if messages else []
         next_level = level + 1 if messages else level
 
         ret = "\n".join(e for e in my_summary + [c.pretty_str(next_level) for c in self.children])
         if level == 0:
             return strip_duplicated_lineno(reflow_all(ret))
-        else:
-            return ret
+        return ret
 
 
 class SchemaException(SchemaSaladException):
     """Indicates error with the provided schema definition."""
 
 
 class ValidationException(SchemaSaladException):
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/fetcher.py` & `schema-salad-8.4.20230426093816/schema_salad/fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 
 class Fetcher(ABC):
     """Fetch resources from URIs."""
 
     @abstractmethod
     def fetch_text(self, url: str, content_types: Optional[List[str]] = None) -> str:
         """Retrieve the given resource as a string."""
-        ...
 
     @abstractmethod
     def check_exists(self, url: str) -> bool:
         """Check if the given resource exists."""
-        ...
 
     @abstractmethod
     def urljoin(self, base_url: str, url: str) -> str:
         ...
 
     schemes = ["file", "http", "https", "mailto"]
 
@@ -78,16 +76,18 @@
                 resp.raise_for_status()
             except Exception as e:
                 raise ValidationException(f"Error fetching {url}: {e}") from e
             if content_types and "content-type" in resp.headers:
                 content_type = resp.headers["content-type"].split(";")[:1][0]
                 if content_type not in content_types:
                     _logger.warning(
-                        f"While fetching {url}, got content-type of "
-                        f"{content_type!r}. Expected one of {content_types}."
+                        "While fetching %s, got content-type of %r. Expected one of %s.",
+                        url,
+                        content_type,
+                        content_types,
                     )
             return resp.text
         if scheme == "file":
             try:
                 # On Windows, url.path will be /drive:/path ; on Unix systems,
                 # /path. As we want drive:/path instead of /drive:/path on Windows,
                 # remove the leading /.
@@ -97,16 +97,15 @@
                     path = path[1:]
                 with open(urllib.request.url2pathname(str(path)), encoding="utf-8") as fp:
                     return str(fp.read())
 
             except OSError as err:
                 if err.filename == path:
                     raise ValidationException(str(err)) from err
-                else:
-                    raise ValidationException(f"Error reading {url}: {err}") from err
+                raise ValidationException(f"Error reading {url}: {err}") from err
         raise ValidationException(f"Unsupported scheme in url: {url}")
 
     def check_exists(self, url: str) -> bool:
         if url in self.cache:
             return True
 
         split = urllib.parse.urlsplit(url)
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/README.md` & `schema-salad-8.4.20230426093816/schema_salad/java/README.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/ArrayLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ArrayLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/DefaultFetcher.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/DefaultFetcher.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/EnumLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/EnumLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/IdMapLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/IdMapLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Loader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Loader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/LoadingOptions.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptions.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/LoadingOptionsBuilder.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/LoadingOptionsBuilder.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/OneOrListOf.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOf.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/OneOrListOfLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OneOrListOfLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/OptionalLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/OptionalLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/RecordLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RecordLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/RootLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/RootLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/SecondaryFilesDslLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/SecondaryFilesDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/TypeDslLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/TypeDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/UnionLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UnionLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/UriLoader.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/UriLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Uris.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Uris.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/ValidationException.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/ValidationException.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/Validator.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/Validator.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/main_utils/YamlUtils.java` & `schema-salad-8.4.20230426093816/schema_salad/java/main_utils/YamlUtils.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/pom.xml` & `schema-salad-8.4.20230426093816/schema_salad/java/pom.xml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/test_utils/DefaultFetcherTest.java` & `schema-salad-8.4.20230426093816/schema_salad/java/test_utils/DefaultFetcherTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java/test_utils/ShortnameTest.java` & `schema-salad-8.4.20230426093816/schema_salad/java/test_utils/ShortnameTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/java_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/jsonld_context.py` & `schema-salad-8.4.20230426093816/schema_salad/jsonld_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,16 @@
                 predicate = recordname
                 recordname = ln
             else:
                 predicate = f"{defaultPrefix}:{recordname}"
 
         if context.get(recordname, predicate) != predicate:
             raise SchemaException(
-                "Predicate collision on '{}', '{}' != '{}'".format(
-                    recordname, context[recordname], predicate
-                )
+                f"Predicate collision on {recordname!r}, "
+                f"{context[recordname]!r} != {predicate!r}"
             )
 
         if not recordname:
             raise SchemaException(f"Unable to find/derive recordname for {t}")
 
         _logger.debug("Adding to context '%s' %s (%s)", recordname, predicate, type(predicate))
         context[recordname] = predicate
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/main.py` & `schema-salad-8.4.20230426093816/schema_salad/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from . import codegen, jsonld_context, schema
 from .avro.schema import SchemaParseException
 from .exceptions import ValidationException, to_one_line_messages
 from .makedoc import makedoc
 from .ref_resolver import Loader, file_uri
 from .utils import json_dump, stdout
 
-if int(rdflib_version.split(".")[0]) < 6:
+if int(rdflib_version.split(".", maxsplit=1)[0]) < 6:
     register("json-ld", Parser, "rdflib_jsonld.parser", "JsonLDParser")
 _logger = logging.getLogger("salad")
 
 
 def printrdf(
     workflow: str,
     wf: Union[CommentedMap, CommentedSeq],
@@ -197,15 +197,15 @@
     parser.add_argument(
         "--primtype",
         default="#PrimitiveType",
         help="Use with --print-doc, link to use for primitive types (string, int etc)",
     )
 
     parser.add_argument("schema", type=str, nargs="?", default=None)
-    parser.add_argument("document", type=str, nargs="?", default=None)
+    parser.add_argument("document", type=str, nargs="*", default=None)
     parser.add_argument("--version", "-v", action="store_true", help="Print version", default=None)
     return parser
 
 
 def main(argsl: Optional[List[str]] = None) -> int:
     if argsl is None:
         argsl = sys.argv[1:]
@@ -222,16 +222,15 @@
         _logger.setLevel(logging.DEBUG)
 
     pkg = pkg_resources.require("schema_salad")
     if pkg:
         if args.version:
             print(f"{sys.argv[0]} Current version: {pkg[0].version}")
             return 0
-        else:
-            _logger.info("%s Current version: %s", sys.argv[0], pkg[0].version)
+        _logger.info("%s Current version: %s", sys.argv[0], pkg[0].version)
 
     # Get the metaschema to validate the schema
     metaschema_names, metaschema_doc, metaschema_loader = schema.get_metaschema()
 
     # Load schema document and resolve refs
 
     schema_uri = args.schema
@@ -239,28 +238,28 @@
         schema_uri = file_uri(os.path.abspath(schema_uri))
     schema_raw_doc = metaschema_loader.fetch(schema_uri)
 
     try:
         schema_doc, schema_metadata = metaschema_loader.resolve_all(schema_raw_doc, schema_uri)
     except ValidationException as e:
         _logger.error(
-            "Schema `%s` failed link checking:\n%s",
+            "Schema %r failed link checking:\n%s",
             args.schema,
             str(e),
-            exc_info=(True if args.debug else False),
+            exc_info=bool(args.debug),
         )
         _logger.debug("Index is %s", list(metaschema_loader.idx.keys()))
         _logger.debug("Vocabulary is %s", list(metaschema_loader.vocab.keys()))
         return 1
     except RuntimeError as e:
         _logger.error(
-            "Schema `%s` read error:\n%s",
+            "Schema %r read error:\n%s",
             args.schema,
             str(e),
-            exc_info=(True if args.debug else False),
+            exc_info=bool(args.debug),
         )
         return 1
 
     if args.print_doc:
         makedoc(
             sys.stdout,
             args.schema,
@@ -283,15 +282,15 @@
         json_dump(list(metaschema_loader.idx.keys()), fp=sys.stdout, indent=4, default=str)
         return 0
 
     # Validate the schema document against the metaschema
     try:
         schema.validate_doc(metaschema_names, schema_doc, metaschema_loader, args.strict)
     except ValidationException as e:
-        _logger.error("While validating schema `%s`:\n%s", args.schema, str(e))
+        _logger.error("While validating schema %r:\n%s", args.schema, str(e))
         return 1
 
     # Get the json-ld context and RDFS representation from the schema
     metactx = schema.collect_namespaces(schema_metadata)
     if "$base" in schema_metadata:
         metactx["@base"] = schema_metadata["$base"]
     if isinstance(schema_doc, CommentedSeq):
@@ -320,24 +319,24 @@
     # document
     if isinstance(schema_doc, MutableSequence):
         avsc_obj = schema.make_avro(schema_doc, document_loader)
         try:
             avsc_names = schema.make_avro_schema_from_avro(avsc_obj)
         except SchemaParseException as err:
             _logger.error(
-                "Schema `%s` error:\n%s",
+                "Schema %r error:\n%s",
                 args.schema,
                 str(err),
                 exc_info=((type(err), err, None) if args.debug else None),
             )
             if args.print_avro:
                 json_dump(avsc_obj, fp=sys.stdout, indent=4, default=str)
             return 1
     else:
-        _logger.error("Schema `%s` must be a list.", args.schema)  # type: ignore[unreachable]
+        _logger.error("Schema %r must be a list.", args.schema)  # type: ignore[unreachable]
         return 1
 
     # Optionally print Avro-compatible schema from schema
     if args.print_avro:
         json_dump(avsc_obj, fp=sys.stdout, indent=4, default=str)
         return 0
 
@@ -362,69 +361,68 @@
 
     if args.print_fieldrefs_dot:
         schema.print_fieldrefs(schema_doc, document_loader, sys.stdout)
         return 0
 
     # If no document specified, all done.
     if not args.document:
-        print(f"Schema `{args.schema}` is valid")
+        print(f"Schema {args.schema!r} is valid")
         return 0
 
     # Load target document and resolve refs
-    try:
-        uri = args.document
-        document, doc_metadata = document_loader.resolve_ref(
-            uri, strict_foreign_properties=args.strict_foreign_properties
-        )
-    except ValidationException as e:
-        msg = to_one_line_messages(e) if args.print_oneline else str(e)
-        _logger.error(
-            "Document `%s` failed validation:\n%s",
-            args.document,
-            msg,
-            exc_info=args.debug,
-        )
-        return 1
+    for uri in args.document:
+        try:
+            document, doc_metadata = document_loader.resolve_ref(
+                uri, strict_foreign_properties=args.strict_foreign_properties
+            )
+        except ValidationException as e:
+            msg = to_one_line_messages(e) if args.print_oneline else str(e)
+            _logger.error(
+                "Document %r failed validation:\n%s",
+                args.document,
+                msg,
+                exc_info=args.debug,
+            )
+            return 1
 
-    # Optionally print the document after ref resolution
-    if args.print_pre:
-        json_dump(document, fp=sys.stdout, indent=4, default=str)
-        return 0
+        # Optionally print the document after ref resolution
+        if args.print_pre:
+            json_dump(document, fp=sys.stdout, indent=4, default=str)
+            return 0
 
-    if args.print_index:
-        json_dump(list(document_loader.idx.keys()), fp=sys.stdout, indent=4, default=str)
-        return 0
+        if args.print_index:
+            json_dump(list(document_loader.idx.keys()), fp=sys.stdout, indent=4, default=str)
+            return 0
 
-    # Validate the user document against the schema
-    try:
-        schema.validate_doc(
-            avsc_names,
-            document,
-            document_loader,
-            args.strict,
-            strict_foreign_properties=args.strict_foreign_properties,
-        )
-    except ValidationException as e:
-        msg2 = to_one_line_messages(e) if args.print_oneline else str(e)
-        _logger.error(f"While validating document `{args.document}`:\n{msg2}")
-        return 1
+        # Validate the user document against the schema
+        try:
+            schema.validate_doc(
+                avsc_names,
+                document,
+                document_loader,
+                args.strict,
+                strict_foreign_properties=args.strict_foreign_properties,
+            )
+        except ValidationException as e:
+            msg2 = to_one_line_messages(e) if args.print_oneline else str(e)
+            _logger.error("While validating document %r:\n%s", uri, msg2)
+            return 1
 
-    # Optionally convert the document to RDF
-    if args.print_rdf:
-        if isinstance(document, (Mapping, MutableSequence)):
-            printrdf(args.document, document, schema_ctx, args.rdf_serializer)
-            return 0
-        else:
+        # Optionally convert the document to RDF
+        if args.print_rdf:
+            if isinstance(document, (Mapping, MutableSequence)):
+                printrdf(uri, document, schema_ctx, args.rdf_serializer)
+                return 0
             print("Document must be a dictionary or list.")
             return 1
 
-    if args.print_metadata:
-        json_dump(doc_metadata, fp=sys.stdout, indent=4, default=str)
-        return 0
+        if args.print_metadata:
+            json_dump(doc_metadata, fp=sys.stdout, indent=4, default=str)
+            return 0
 
-    _logger.info(f"Document `{args.document}` is valid")
+        _logger.info("Document %r is valid", uri)
 
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main(sys.argv[1:]))
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/makedoc.py` & `schema-salad-8.4.20230426093816/schema_salad/makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/field_name.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/ident_res.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/import_include.md` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/link_res.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/map_res.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/map_res_schema.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/metaschema.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/metaschema_base.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/salad.md` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/sfdsl_res.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/typedsl_res.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema/vocab_res.yml` & `schema-salad-8.4.20230426093816/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/metaschema.py` & `schema-salad-8.4.20230426093816/schema_salad/metaschema.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             result, metadata = _document_load_by_url(
                 fieldtype,
                 url,
                 loadingOptions,
             )
             loadingOptions.imports.append(url)
             return result
-        elif "$include" in val:
+        if "$include" in val:
             if loadingOptions.fileuri is None:
                 raise SchemaSaladException("Cannot load $import without fileuri")
             url = loadingOptions.fetcher.urljoin(loadingOptions.fileuri, val["$include"])
             val = loadingOptions.fetcher.fetch_text(url)
             loadingOptions.includes.append(url)
     return fieldtype.load(val, baseuri, loadingOptions)
 
@@ -413,16 +413,15 @@
         self.symbols = symbols
         self.name = name
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if doc in self.symbols:
             return doc
-        else:
-            raise ValidationException(f"Expected one of {self.symbols}")
+        raise ValidationException(f"Expected one of {self.symbols}")
 
     def __repr__(self):  # type: () -> str
         return self.name
 
 
 class _SecondaryDSLLoader(_Loader):
     def __init__(self, inner):
@@ -771,16 +770,15 @@
         frag = "#" + quote(str(pathsp[1])) if len(pathsp) == 2 else ""
         urlpath = pathname2url(str(pathsp[0]))
     else:
         urlpath = pathname2url(path)
         frag = ""
     if urlpath.startswith("//"):
         return f"file:{urlpath}{frag}"
-    else:
-        return f"file://{urlpath}{frag}"
+    return f"file://{urlpath}{frag}"
 
 
 def prefix_url(url: str, namespaces: Dict[str, str]) -> str:
     """Expand short forms into full URLs using the given namespace dictionary."""
     for k, v in namespaces.items():
         if url.startswith(v):
             return k + ":" + url[len(v) :]
@@ -816,16 +814,15 @@
                 while i < ref_scope:
                     sp.pop()
                     i += 1
                 basefrag = "/".join(sp)
 
             if urisplit.fragment.startswith(basefrag):
                 return urisplit.fragment[len(basefrag) :]
-            else:
-                return urisplit.fragment
+            return urisplit.fragment
         return uri
     else:
         return save(uri, top=False, base_url=base_url, relative_uris=relative_uris)
 
 
 def shortname(inputid: str) -> str:
     """
@@ -905,15 +902,15 @@
                     uri_strtype_True_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `name` field is not valid because:",
+                        "the 'name' field is not valid because:",
                         SourceLine(_doc, "name", str),
                         [e],
                     )
                 )
         else:
             name = None
 
@@ -932,15 +929,15 @@
                     union_of_None_type_or_strtype_or_array_of_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `doc` field is not valid because:",
+                        "the 'doc' field is not valid because:",
                         SourceLine(_doc, "doc", str),
                         [e],
                     )
                 )
         else:
             doc = None
         try:
@@ -949,15 +946,15 @@
                 typedsl_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_or_array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         extension_fields: Dict[str, Any] = {}
         for k in _doc.keys():
             if k not in cls.attrs:
@@ -1071,15 +1068,15 @@
                     idmap_fields_union_of_None_type_or_array_of_RecordFieldLoader,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `fields` field is not valid because:",
+                        "the 'fields' field is not valid because:",
                         SourceLine(_doc, "fields", str),
                         [e],
                     )
                 )
         else:
             fields = None
         try:
@@ -1088,15 +1085,15 @@
                 typedsl_Record_nameLoader_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         extension_fields: Dict[str, Any] = {}
         for k in _doc.keys():
             if k not in cls.attrs:
@@ -1216,15 +1213,15 @@
                     uri_union_of_None_type_or_strtype_True_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `name` field is not valid because:",
+                        "the 'name' field is not valid because:",
                         SourceLine(_doc, "name", str),
                         [e],
                     )
                 )
         else:
             name = None
 
@@ -1242,30 +1239,30 @@
                 uri_array_of_strtype_True_False_None,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `symbols` field is not valid because:",
+                    "the 'symbols' field is not valid because:",
                     SourceLine(_doc, "symbols", str),
                     [e],
                 )
             )
         try:
             type = load_field(
                 _doc.get("type"),
                 typedsl_Enum_nameLoader_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         extension_fields: Dict[str, Any] = {}
         for k in _doc.keys():
             if k not in cls.attrs:
@@ -1377,30 +1374,30 @@
                 uri_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_or_array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_False_True_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `items` field is not valid because:",
+                    "the 'items' field is not valid because:",
                     SourceLine(_doc, "items", str),
                     [e],
                 )
             )
         try:
             type = load_field(
                 _doc.get("type"),
                 typedsl_Array_nameLoader_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         extension_fields: Dict[str, Any] = {}
         for k in _doc.keys():
             if k not in cls.attrs:
@@ -1558,15 +1555,15 @@
                     uri_union_of_None_type_or_strtype_True_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `_id` field is not valid because:",
+                        "the '_id' field is not valid because:",
                         SourceLine(_doc, "_id", str),
                         [e],
                     )
                 )
         else:
             _id = None
         if "_type" in _doc:
@@ -1576,15 +1573,15 @@
                     union_of_None_type_or_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `_type` field is not valid because:",
+                        "the '_type' field is not valid because:",
                         SourceLine(_doc, "_type", str),
                         [e],
                     )
                 )
         else:
             _type = None
         if "_container" in _doc:
@@ -1594,15 +1591,15 @@
                     union_of_None_type_or_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `_container` field is not valid because:",
+                        "the '_container' field is not valid because:",
                         SourceLine(_doc, "_container", str),
                         [e],
                     )
                 )
         else:
             _container = None
         if "identity" in _doc:
@@ -1612,15 +1609,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `identity` field is not valid because:",
+                        "the 'identity' field is not valid because:",
                         SourceLine(_doc, "identity", str),
                         [e],
                     )
                 )
         else:
             identity = None
         if "noLinkCheck" in _doc:
@@ -1630,15 +1627,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `noLinkCheck` field is not valid because:",
+                        "the 'noLinkCheck' field is not valid because:",
                         SourceLine(_doc, "noLinkCheck", str),
                         [e],
                     )
                 )
         else:
             noLinkCheck = None
         if "mapSubject" in _doc:
@@ -1648,15 +1645,15 @@
                     union_of_None_type_or_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `mapSubject` field is not valid because:",
+                        "the 'mapSubject' field is not valid because:",
                         SourceLine(_doc, "mapSubject", str),
                         [e],
                     )
                 )
         else:
             mapSubject = None
         if "mapPredicate" in _doc:
@@ -1666,15 +1663,15 @@
                     union_of_None_type_or_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `mapPredicate` field is not valid because:",
+                        "the 'mapPredicate' field is not valid because:",
                         SourceLine(_doc, "mapPredicate", str),
                         [e],
                     )
                 )
         else:
             mapPredicate = None
         if "refScope" in _doc:
@@ -1684,15 +1681,15 @@
                     union_of_None_type_or_inttype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `refScope` field is not valid because:",
+                        "the 'refScope' field is not valid because:",
                         SourceLine(_doc, "refScope", str),
                         [e],
                     )
                 )
         else:
             refScope = None
         if "typeDSL" in _doc:
@@ -1702,15 +1699,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `typeDSL` field is not valid because:",
+                        "the 'typeDSL' field is not valid because:",
                         SourceLine(_doc, "typeDSL", str),
                         [e],
                     )
                 )
         else:
             typeDSL = None
         if "secondaryFilesDSL" in _doc:
@@ -1720,15 +1717,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `secondaryFilesDSL` field is not valid because:",
+                        "the 'secondaryFilesDSL' field is not valid because:",
                         SourceLine(_doc, "secondaryFilesDSL", str),
                         [e],
                     )
                 )
         else:
             secondaryFilesDSL = None
         if "subscope" in _doc:
@@ -1738,15 +1735,15 @@
                     union_of_None_type_or_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `subscope` field is not valid because:",
+                        "the 'subscope' field is not valid because:",
                         SourceLine(_doc, "subscope", str),
                         [e],
                     )
                 )
         else:
             subscope = None
         extension_fields: Dict[str, Any] = {}
@@ -1932,30 +1929,30 @@
                 uri_strtype_False_False_1,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `specializeFrom` field is not valid because:",
+                    "the 'specializeFrom' field is not valid because:",
                     SourceLine(_doc, "specializeFrom", str),
                     [e],
                 )
             )
         try:
             specializeTo = load_field(
                 _doc.get("specializeTo"),
                 uri_strtype_False_False_1,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `specializeTo` field is not valid because:",
+                    "the 'specializeTo' field is not valid because:",
                     SourceLine(_doc, "specializeTo", str),
                     [e],
                 )
             )
         extension_fields: Dict[str, Any] = {}
         for k in _doc.keys():
             if k not in cls.attrs:
@@ -2099,15 +2096,15 @@
                     uri_strtype_True_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `name` field is not valid because:",
+                        "the 'name' field is not valid because:",
                         SourceLine(_doc, "name", str),
                         [e],
                     )
                 )
         else:
             name = None
 
@@ -2126,15 +2123,15 @@
                     union_of_None_type_or_strtype_or_array_of_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `doc` field is not valid because:",
+                        "the 'doc' field is not valid because:",
                         SourceLine(_doc, "doc", str),
                         [e],
                     )
                 )
         else:
             doc = None
         try:
@@ -2143,15 +2140,15 @@
                 typedsl_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_or_array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         if "jsonldPredicate" in _doc:
             try:
                 jsonldPredicate = load_field(
@@ -2159,15 +2156,15 @@
                     union_of_None_type_or_strtype_or_JsonldPredicateLoader,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `jsonldPredicate` field is not valid because:",
+                        "the 'jsonldPredicate' field is not valid because:",
                         SourceLine(_doc, "jsonldPredicate", str),
                         [e],
                     )
                 )
         else:
             jsonldPredicate = None
         if "default" in _doc:
@@ -2177,15 +2174,15 @@
                     union_of_None_type_or_Any_type,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `default` field is not valid because:",
+                        "the 'default' field is not valid because:",
                         SourceLine(_doc, "default", str),
                         [e],
                     )
                 )
         else:
             default = None
         extension_fields: Dict[str, Any] = {}
@@ -2366,15 +2363,15 @@
                     uri_strtype_True_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `name` field is not valid because:",
+                        "the 'name' field is not valid because:",
                         SourceLine(_doc, "name", str),
                         [e],
                     )
                 )
         else:
             name = None
 
@@ -2393,15 +2390,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `inVocab` field is not valid because:",
+                        "the 'inVocab' field is not valid because:",
                         SourceLine(_doc, "inVocab", str),
                         [e],
                     )
                 )
         else:
             inVocab = None
         if "fields" in _doc:
@@ -2411,15 +2408,15 @@
                     idmap_fields_union_of_None_type_or_array_of_SaladRecordFieldLoader,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `fields` field is not valid because:",
+                        "the 'fields' field is not valid because:",
                         SourceLine(_doc, "fields", str),
                         [e],
                     )
                 )
         else:
             fields = None
         try:
@@ -2428,15 +2425,15 @@
                 typedsl_Record_nameLoader_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         if "doc" in _doc:
             try:
                 doc = load_field(
@@ -2444,15 +2441,15 @@
                     union_of_None_type_or_strtype_or_array_of_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `doc` field is not valid because:",
+                        "the 'doc' field is not valid because:",
                         SourceLine(_doc, "doc", str),
                         [e],
                     )
                 )
         else:
             doc = None
         if "docParent" in _doc:
@@ -2462,15 +2459,15 @@
                     uri_union_of_None_type_or_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docParent` field is not valid because:",
+                        "the 'docParent' field is not valid because:",
                         SourceLine(_doc, "docParent", str),
                         [e],
                     )
                 )
         else:
             docParent = None
         if "docChild" in _doc:
@@ -2480,15 +2477,15 @@
                     uri_union_of_None_type_or_strtype_or_array_of_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docChild` field is not valid because:",
+                        "the 'docChild' field is not valid because:",
                         SourceLine(_doc, "docChild", str),
                         [e],
                     )
                 )
         else:
             docChild = None
         if "docAfter" in _doc:
@@ -2498,15 +2495,15 @@
                     uri_union_of_None_type_or_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docAfter` field is not valid because:",
+                        "the 'docAfter' field is not valid because:",
                         SourceLine(_doc, "docAfter", str),
                         [e],
                     )
                 )
         else:
             docAfter = None
         if "jsonldPredicate" in _doc:
@@ -2516,15 +2513,15 @@
                     union_of_None_type_or_strtype_or_JsonldPredicateLoader,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `jsonldPredicate` field is not valid because:",
+                        "the 'jsonldPredicate' field is not valid because:",
                         SourceLine(_doc, "jsonldPredicate", str),
                         [e],
                     )
                 )
         else:
             jsonldPredicate = None
         if "documentRoot" in _doc:
@@ -2534,15 +2531,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `documentRoot` field is not valid because:",
+                        "the 'documentRoot' field is not valid because:",
                         SourceLine(_doc, "documentRoot", str),
                         [e],
                     )
                 )
         else:
             documentRoot = None
         if "abstract" in _doc:
@@ -2552,15 +2549,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `abstract` field is not valid because:",
+                        "the 'abstract' field is not valid because:",
                         SourceLine(_doc, "abstract", str),
                         [e],
                     )
                 )
         else:
             abstract = None
         if "extends" in _doc:
@@ -2570,15 +2567,15 @@
                     uri_union_of_None_type_or_strtype_or_array_of_strtype_False_False_1,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `extends` field is not valid because:",
+                        "the 'extends' field is not valid because:",
                         SourceLine(_doc, "extends", str),
                         [e],
                     )
                 )
         else:
             extends = None
         if "specialize" in _doc:
@@ -2588,15 +2585,15 @@
                     idmap_specialize_union_of_None_type_or_array_of_SpecializeDefLoader,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `specialize` field is not valid because:",
+                        "the 'specialize' field is not valid because:",
                         SourceLine(_doc, "specialize", str),
                         [e],
                     )
                 )
         else:
             specialize = None
         extension_fields: Dict[str, Any] = {}
@@ -2835,15 +2832,15 @@
                     uri_union_of_None_type_or_strtype_True_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `name` field is not valid because:",
+                        "the 'name' field is not valid because:",
                         SourceLine(_doc, "name", str),
                         [e],
                     )
                 )
         else:
             name = None
 
@@ -2862,15 +2859,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `inVocab` field is not valid because:",
+                        "the 'inVocab' field is not valid because:",
                         SourceLine(_doc, "inVocab", str),
                         [e],
                     )
                 )
         else:
             inVocab = None
         try:
@@ -2879,30 +2876,30 @@
                 uri_array_of_strtype_True_False_None,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `symbols` field is not valid because:",
+                    "the 'symbols' field is not valid because:",
                     SourceLine(_doc, "symbols", str),
                     [e],
                 )
             )
         try:
             type = load_field(
                 _doc.get("type"),
                 typedsl_Enum_nameLoader_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         if "doc" in _doc:
             try:
                 doc = load_field(
@@ -2910,15 +2907,15 @@
                     union_of_None_type_or_strtype_or_array_of_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `doc` field is not valid because:",
+                        "the 'doc' field is not valid because:",
                         SourceLine(_doc, "doc", str),
                         [e],
                     )
                 )
         else:
             doc = None
         if "docParent" in _doc:
@@ -2928,15 +2925,15 @@
                     uri_union_of_None_type_or_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docParent` field is not valid because:",
+                        "the 'docParent' field is not valid because:",
                         SourceLine(_doc, "docParent", str),
                         [e],
                     )
                 )
         else:
             docParent = None
         if "docChild" in _doc:
@@ -2946,15 +2943,15 @@
                     uri_union_of_None_type_or_strtype_or_array_of_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docChild` field is not valid because:",
+                        "the 'docChild' field is not valid because:",
                         SourceLine(_doc, "docChild", str),
                         [e],
                     )
                 )
         else:
             docChild = None
         if "docAfter" in _doc:
@@ -2964,15 +2961,15 @@
                     uri_union_of_None_type_or_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docAfter` field is not valid because:",
+                        "the 'docAfter' field is not valid because:",
                         SourceLine(_doc, "docAfter", str),
                         [e],
                     )
                 )
         else:
             docAfter = None
         if "jsonldPredicate" in _doc:
@@ -2982,15 +2979,15 @@
                     union_of_None_type_or_strtype_or_JsonldPredicateLoader,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `jsonldPredicate` field is not valid because:",
+                        "the 'jsonldPredicate' field is not valid because:",
                         SourceLine(_doc, "jsonldPredicate", str),
                         [e],
                     )
                 )
         else:
             jsonldPredicate = None
         if "documentRoot" in _doc:
@@ -3000,15 +2997,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `documentRoot` field is not valid because:",
+                        "the 'documentRoot' field is not valid because:",
                         SourceLine(_doc, "documentRoot", str),
                         [e],
                     )
                 )
         else:
             documentRoot = None
         if "extends" in _doc:
@@ -3018,15 +3015,15 @@
                     uri_union_of_None_type_or_strtype_or_array_of_strtype_False_False_1,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `extends` field is not valid because:",
+                        "the 'extends' field is not valid because:",
                         SourceLine(_doc, "extends", str),
                         [e],
                     )
                 )
         else:
             extends = None
         extension_fields: Dict[str, Any] = {}
@@ -3231,15 +3228,15 @@
                     uri_strtype_True_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `name` field is not valid because:",
+                        "the 'name' field is not valid because:",
                         SourceLine(_doc, "name", str),
                         [e],
                     )
                 )
         else:
             name = None
 
@@ -3258,15 +3255,15 @@
                     union_of_None_type_or_booltype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `inVocab` field is not valid because:",
+                        "the 'inVocab' field is not valid because:",
                         SourceLine(_doc, "inVocab", str),
                         [e],
                     )
                 )
         else:
             inVocab = None
         if "doc" in _doc:
@@ -3276,15 +3273,15 @@
                     union_of_None_type_or_strtype_or_array_of_strtype,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `doc` field is not valid because:",
+                        "the 'doc' field is not valid because:",
                         SourceLine(_doc, "doc", str),
                         [e],
                     )
                 )
         else:
             doc = None
         if "docParent" in _doc:
@@ -3294,15 +3291,15 @@
                     uri_union_of_None_type_or_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docParent` field is not valid because:",
+                        "the 'docParent' field is not valid because:",
                         SourceLine(_doc, "docParent", str),
                         [e],
                     )
                 )
         else:
             docParent = None
         if "docChild" in _doc:
@@ -3312,15 +3309,15 @@
                     uri_union_of_None_type_or_strtype_or_array_of_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docChild` field is not valid because:",
+                        "the 'docChild' field is not valid because:",
                         SourceLine(_doc, "docChild", str),
                         [e],
                     )
                 )
         else:
             docChild = None
         if "docAfter" in _doc:
@@ -3330,15 +3327,15 @@
                     uri_union_of_None_type_or_strtype_False_False_None,
                     baseuri,
                     loadingOptions,
                 )
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
-                        "the `docAfter` field is not valid because:",
+                        "the 'docAfter' field is not valid because:",
                         SourceLine(_doc, "docAfter", str),
                         [e],
                     )
                 )
         else:
             docAfter = None
         try:
@@ -3347,15 +3344,15 @@
                 typedsl_Documentation_nameLoader_2,
                 baseuri,
                 loadingOptions,
             )
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
-                    "the `type` field is not valid because:",
+                    "the 'type' field is not valid because:",
                     SourceLine(_doc, "type", str),
                     [e],
                 )
             )
         extension_fields: Dict[str, Any] = {}
         for k in _doc.keys():
             if k not in cls.attrs:
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/python_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/python_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,15 +530,15 @@
 {spc}                {fieldtype},
 {spc}                {baseurivar},
 {spc}                loadingOptions,
 {spc}            )
 {spc}        except ValidationException as e:
 {spc}            _errors__.append(
 {spc}                ValidationException(
-{spc}                    \"the `{fieldname}` field is not valid because:\",
+{spc}                    \"the {fieldname!r} field is not valid because:\",
 {spc}                    SourceLine(_doc, "{fieldname}", str),
 {spc}                    [e],
 {spc}                )
 {spc}            )
 """.format(
                 safename=self.safe_name(name),
                 fieldname=shortname(name),
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/python_codegen_support.py` & `schema-salad-8.4.20230426093816/schema_salad/python_codegen_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             result, metadata = _document_load_by_url(
                 fieldtype,
                 url,
                 loadingOptions,
             )
             loadingOptions.imports.append(url)
             return result
-        elif "$include" in val:
+        if "$include" in val:
             if loadingOptions.fileuri is None:
                 raise SchemaSaladException("Cannot load $import without fileuri")
             url = loadingOptions.fetcher.urljoin(loadingOptions.fileuri, val["$include"])
             val = loadingOptions.fetcher.fetch_text(url)
             loadingOptions.includes.append(url)
     return fieldtype.load(val, baseuri, loadingOptions)
 
@@ -410,16 +410,15 @@
         self.symbols = symbols
         self.name = name
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if doc in self.symbols:
             return doc
-        else:
-            raise ValidationException(f"Expected one of {self.symbols}")
+        raise ValidationException(f"Expected one of {self.symbols}")
 
     def __repr__(self):  # type: () -> str
         return self.name
 
 
 class _SecondaryDSLLoader(_Loader):
     def __init__(self, inner):
@@ -768,16 +767,15 @@
         frag = "#" + quote(str(pathsp[1])) if len(pathsp) == 2 else ""
         urlpath = pathname2url(str(pathsp[0]))
     else:
         urlpath = pathname2url(path)
         frag = ""
     if urlpath.startswith("//"):
         return f"file:{urlpath}{frag}"
-    else:
-        return f"file://{urlpath}{frag}"
+    return f"file://{urlpath}{frag}"
 
 
 def prefix_url(url: str, namespaces: Dict[str, str]) -> str:
     """Expand short forms into full URLs using the given namespace dictionary."""
     for k, v in namespaces.items():
         if url.startswith(v):
             return k + ":" + url[len(v) :]
@@ -813,16 +811,15 @@
                 while i < ref_scope:
                     sp.pop()
                     i += 1
                 basefrag = "/".join(sp)
 
             if urisplit.fragment.startswith(basefrag):
                 return urisplit.fragment[len(basefrag) :]
-            else:
-                return urisplit.fragment
+            return urisplit.fragment
         return uri
     else:
         return save(uri, top=False, base_url=base_url, relative_uris=relative_uris)
 
 
 def shortname(inputid: str) -> str:
     """
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/ref_resolver.py` & `schema-salad-8.4.20230426093816/schema_salad/ref_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,23 +454,21 @@
                 lref = None
                 for identifier in self.identifiers:
                     if identifier in obj:
                         lref = obj[identifier]
                         break
                 if not lref:
                     raise ValidationException(
-                        "Object `{}` does not have identifier field in {}".format(
-                            obj, self.identifiers
-                        ),
+                        f"Object {obj!r} does not have identifier field in {self.identifiers}",
                         SourceLine(obj),
                     )
 
         if not isinstance(lref, str):
             raise ValidationException(
-                f"Expected CommentedMap or string, got {type(lref)}: `{lref}`"
+                f"Expected CommentedMap or string, got {type(lref)}: {lref!r}"
             )
 
         if isinstance(lref, str) and os.sep == "\\":
             # Convert Windows path separator in ref
             lref = lref.replace("\\", "/")
 
         url = self.expand_url(lref, base_url, scoped_id=(obj is not None))
@@ -485,29 +483,28 @@
                     if "$graph" in resolved_obj:
                         metadata = _copy_dict_without_key(resolved_obj, "$graph")
                         return resolved_obj["$graph"], metadata
                     else:
                         return resolved_obj, metadata
                 else:
                     raise ValidationException(
-                        f"Expected CommentedMap, got {type(metadata)}: `{metadata}`"
+                        f"Expected CommentedMap, got {type(metadata)}: {metadata!r}"
                     )
             elif isinstance(resolved_obj, MutableSequence):
                 metadata = self.idx.get(urllib.parse.urldefrag(url)[0], CommentedMap())
                 if isinstance(metadata, MutableMapping):
                     return resolved_obj, metadata
                 else:
                     return resolved_obj, CommentedMap()
             elif isinstance(resolved_obj, str):
                 return resolved_obj, CommentedMap()
             else:
                 raise ValidationException(
-                    "Expected MutableMapping or MutableSequence, got {}: `{}`".format(
-                        type(resolved_obj), resolved_obj
-                    )
+                    f"Expected MutableMapping or MutableSequence, got "
+                    f"{type(resolved_obj)}: {resolved_obj!r}"
                 )
 
         # "$include" directive means load raw text
         if inc:
             # Make a note in the index that this was an included string
             self.idx["include:" + url] = url
             return self.fetch_text(url), CommentedMap()
@@ -520,17 +517,16 @@
         else:
             # Load structured document
             doc_url, frg = urllib.parse.urldefrag(url)
             if doc_url in self.idx and (not mixin):
                 # If the base document is in the index, it was already loaded,
                 # so if we didn't find the reference earlier then it must not
                 # exist.
-                raise ValidationException(
-                    f"Reference `#{frg}` not found in file `{doc_url}`.",
-                    SourceLine(self.idx[doc_url]),
+                raise SourceLine(self.idx, doc_url, ValidationException).makeError(
+                    f"Reference '#{frg}' not found in file {doc_url!r}.",
                 )
             doc = self.fetch(doc_url, inject_ids=(not mixin), content_types=content_types)
 
         if imp:
             # Make a note in the index that this was an imported fragment
             self.idx["import:" + url] = url
 
@@ -558,17 +554,15 @@
         # Requested reference should be in the index now, otherwise it's a bad
         # reference
         if not bool(mixin):
             if url in self.idx:
                 resolved_obj = self.idx[url]
             else:
                 raise ValidationException(
-                    "Reference `{}` is not in the index. Index contains: {}".format(
-                        url, ", ".join(self.idx)
-                    )
+                    f"Reference {url!r} is not in the index. Index contains: {' '.join(self.idx)}"
                 )
 
         if isinstance(resolved_obj, CommentedMap):
             if "$graph" in resolved_obj:
                 metadata = _copy_dict_without_key(resolved_obj, "$graph")
                 return resolved_obj["$graph"], metadata
             else:
@@ -601,16 +595,16 @@
                                 v.lc.add_kv_line_col(
                                     loader.mapPredicate[idmapField],
                                     document[idmapField].lc.data[k],
                                 )
                                 v.lc.filename = document.lc.filename
                             else:
                                 raise ValidationException(
-                                    "mapSubject '{}' value '{}' is not a dict "
-                                    "and does not have a mapPredicate.".format(k, v),
+                                    f"mapSubject {k!r} value {v!r} is not a dict "
+                                    "and does not have a mapPredicate.",
                                     SourceLine(document, idmapField),
                                 )
                         else:
                             v = val
 
                         v[loader.idmap[idmapField]] = k
                         v.lc.add_kv_line_col(
@@ -675,18 +669,17 @@
         d: str,
         loader: "Loader",
         lc: LineCol,
         filename: str,
     ) -> Union[str, CommentedMap, CommentedSeq]:
         if d in loader.type_dsl_fields:
             return self._type_dsl(datum, lc, filename)
-        elif d in loader.secondaryFile_dsl_fields:
+        if d in loader.secondaryFile_dsl_fields:
             return self._secondaryFile_dsl(datum, lc, filename)
-        else:
-            return datum
+        return datum
 
     def _resolve_dsl(
         self,
         document: CommentedMap,
         loader: "Loader",
     ) -> None:
         fields = list(loader.type_dsl_fields)
@@ -829,15 +822,15 @@
             if "$import" in document or "$include" in document:
                 return self.resolve_ref(
                     document,
                     base_url=file_base,
                     checklinks=checklinks,
                     strict_foreign_properties=strict_foreign_properties,
                 )
-            elif "$mixin" in document:
+            if "$mixin" in document:
                 return self.resolve_ref(
                     document,
                     base_url=base_url,
                     checklinks=checklinks,
                     strict_foreign_properties=strict_foreign_properties,
                 )
         elif isinstance(document, CommentedSeq):
@@ -1030,17 +1023,15 @@
             sp.pop()
             if len(sp) == 0:
                 break
             sp.pop()
         if onWindows() and link.startswith("file:"):
             link = link.lower()
         raise ValidationException(
-            "Field `{}` references unknown identifier `{}`, tried {}".format(
-                field, link, ", ".join(tried)
-            )
+            f"Field {field!r} references unknown identifier {link!r}, tried {' '.join(tried)}"
         )
 
     def validate_link(
         self,
         field: str,
         link: Union[str, CommentedSeq, CommentedMap],
         # link also can be None, but that results in
@@ -1053,22 +1044,22 @@
         if isinstance(link, str):
             if field in self.vocab_fields:
                 if link not in self.vocab and link not in self.idx and link not in self.rvocab:
                     if field in self.scoped_ref_fields:
                         return self.validate_scoped(field, link, docid)
                     elif not self.check_exists(link):
                         raise ValidationException(
-                            f"Field `{field}` contains undefined reference to `{link}`"
+                            f"Field {field!r} contains undefined reference to {link!r}"
                         )
             elif link not in self.idx and link not in self.rvocab:
                 if field in self.scoped_ref_fields:
                     return self.validate_scoped(field, link, docid)
                 elif not self.check_exists(link):
                     raise ValidationException(
-                        f"Field `{field}` contains undefined reference to `{link}`"
+                        f"Field {field!r} contains undefined reference to {link!r}"
                     )
         elif isinstance(link, CommentedSeq):
             errors = []
             for n, i in enumerate(link):
                 try:
                     link[n] = self.validate_link(field, i, docid, all_doc_ids)
                 except ValidationException as v:
@@ -1130,15 +1121,15 @@
                     if identifier in document:
                         sl = SourceLine(document, identifier, str)
                         if (
                             document[identifier] in all_doc_ids
                             and sl.makeLead() != all_doc_ids[document[identifier]]
                         ):
                             _logger.warning(
-                                "%s object %s `%s` previously defined",
+                                "%s object %s %r previously defined",
                                 all_doc_ids[document[identifier]],
                                 identifier,
                                 relname(document[identifier]),
                             )
                         else:
                             all_doc_ids[document[identifier]] = sl.makeLead()
                             break
@@ -1161,26 +1152,25 @@
             except ValidationException as v:
                 if key in self.nolinkcheck or (isinstance(key, str) and ":" in key):
                     _logger.warning(v.as_warning())
                 else:
                     docid2 = self.getid(val)
                     if docid2 is not None:
                         errors.append(
-                            ValidationException(f"checking object `{relname(docid2)}`", sl, [v])
+                            ValidationException(f"checking object {relname(docid2)!r}", sl, [v])
                         )
                     else:
                         if isinstance(key, str):
-                            errors.append(ValidationException(f"checking field `{key}`", sl, [v]))
+                            errors.append(ValidationException(f"checking field {key!r}", sl, [v]))
                         else:
                             errors.append(ValidationException("checking item", sl, [v]))
         if bool(errors):
             if len(errors) > 1:
                 raise ValidationException("", None, errors)
-            else:
-                raise errors[0]
+            raise errors[0]
         return
 
 
 def _copy_dict_without_key(
     from_dict: Union[CommentedMap, ContextType], filtered_key: str
 ) -> CommentedMap:
     new_dict = CommentedMap(from_dict.items())
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/schema.py` & `schema-salad-8.4.20230426093816/schema_salad/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,15 @@
     j = yaml.load(loader.cache["https://w3id.org/cwl/salad"])
     add_lc_filename(j, "metaschema.yml")
     j2 = loader.resolve_all(j, saladp)[0]
 
     if not isinstance(j2, list):
         _logger.error("%s", j2)
         raise SchemaParseException(f"Not a list: {j2}")
-    else:
-        sch_obj = make_avro(j2, loader, loader.vocab)
+    sch_obj = make_avro(j2, loader, loader.vocab)
     try:
         sch_names = make_avro_schema_from_avro(sch_obj)
     except SchemaParseException:
         _logger.error("Metaschema error, avro was:\n%s", json_dumps(sch_obj, indent=4))
         raise
     validate_doc(sch_names, j2, loader, strict=True)
     cached_metaschema = (sch_names, j2, loader)
@@ -210,16 +209,16 @@
 def add_namespaces(metadata: Mapping[str, Any], namespaces: MutableMapping[str, str]) -> None:
     """Collect the provided namespaces, checking for conflicts."""
     for key, value in metadata.items():
         if key not in namespaces:
             namespaces[key] = value
         elif namespaces[key] != value:
             raise ValidationException(
-                "Namespace prefix '{}' has conflicting definitions '{}'"
-                " and '{}'.".format(key, namespaces[key], value)
+                f"Namespace prefix {key!r} has conflicting definitions {namespaces[key]!r}"
+                " and {value!r}."
             )
 
 
 def collect_namespaces(metadata: Mapping[str, Any]) -> Dict[str, str]:
     """Walk through the metadata object, collecting namespace declarations."""
     namespaces = {}  # type: Dict[str, str]
     if "$import_metadata" in metadata:
@@ -383,29 +382,29 @@
                         skip_foreign_properties=loader.skip_schemas,
                         strict_foreign_properties=strict_foreign_properties,
                         vocab=loader.vocab,
                     )
                 except ClassValidationException as exc1:
                     errors = [
                         ClassValidationException(
-                            f"tried `{validate.friendly(name)}` but", sourceline, [exc1]
+                            f"tried {validate.friendly(name)!r} but", sourceline, [exc1]
                         )
                     ]
                     break
                 except ValidationException as exc2:
                     errors.append(
                         ValidationException(
-                            f"tried `{validate.friendly(name)}` but", sourceline, [exc2]
+                            f"tried {validate.friendly(name)!r} but", sourceline, [exc2]
                         )
                     )
 
             objerr = "Invalid"
             for ident in loader.identifiers:
                 if ident in item:
-                    objerr = f"Object `{relname(item[ident])}` is not valid because"
+                    objerr = f"Object {relname(item[ident])!r} is not valid because"
                     break
             anyerrors.append(ValidationException(objerr, sourceline, errors, "-"))
     if anyerrors:
         raise ValidationException("", None, anyerrors, "*")
 
 
 def get_anon_name(rec: MutableMapping[str, Union[str, Dict[str, str], List[str]]]) -> str:
@@ -427,15 +426,15 @@
             else:
                 raise ValidationException(
                     f"Expected entries in 'fields' to also be maps, was {field}."
                 )
         return "record_" + hashlib.sha1(anon_name.encode("UTF-8")).hexdigest()  # nosec
     if rec["type"] in ("array", saladp + "array"):
         return ""
-    raise ValidationException("Expected enum or record, was {}".format(rec["type"]))
+    raise ValidationException("Expected enum or record, was {rec['type'])}")
 
 
 def replace_type(
     items: Any,
     spec: Dict[str, Any],
     loader: Loader,
     found: Set[str],
@@ -566,18 +565,16 @@
             )
         return ret
     if union and isinstance(items, str):
         if items in alltypes and validate.avro_type_name(items) not in found:
             return make_valid_avro(alltypes[items], alltypes, found, union=union, vocab=vocab)
         if items in vocab:
             return validate.avro_type_name(vocab[items])
-        else:
-            return validate.avro_type_name(items)
-    else:
-        return items
+        return validate.avro_type_name(items)
+    return items
 
 
 def deepcopy_strip(item: Any) -> Any:
     """
     Make a deep copy of list and dict objects.
 
     Intentionally do not copy attributes.  This is to discard CommentedMap and
@@ -604,17 +601,15 @@
                     specs[spec["specializeFrom"]] = spec["specializeTo"]
 
             exfields = []  # type: List[Any]
             exsym = []  # type: List[str]
             for ex in aslist(stype["extends"]):
                 if ex not in types:
                     raise ValidationException(
-                        "Extends {} in {} refers to invalid base type.".format(
-                            stype["extends"], stype["name"]
-                        )
+                        f"Extends {stype['extends']} in {stype['name']} refers to invalid base type."
                     )
 
                 basetype = copy.copy(types[ex])
 
                 if stype["type"] == "record":
                     if specs:
                         basetype["fields"] = replace_type(
@@ -670,18 +665,17 @@
 
                 stype["fields"] = combined_fields
 
                 fieldnames = set()  # type: Set[str]
                 for field in stype["fields"]:
                     if field["name"] in fieldnames:
                         raise ValidationException(
-                            "Field name {} appears twice in {}".format(field["name"], stype["name"])
+                            f"Field name {field['name']} appears twice in {stype['name']}"
                         )
-                    else:
-                        fieldnames.add(field["name"])
+                    fieldnames.add(field["name"])
             elif stype["type"] == "enum":
                 stype = copy.copy(stype)
                 exsym.extend(stype.get("symbols", []))
                 stype["symbols"] = exsym
 
             types[stype["name"]] = stype
 
@@ -698,15 +692,15 @@
                 if ex_types[ex].get("abstract"):
                     add_dictlist(extended_by, ex, ex_types[result["name"]])
                     add_dictlist(extended_by, validate.avro_type_name(ex), ex_types[ex])
 
     for result in results:
         if result.get("abstract") and result["name"] not in extended_by:
             raise ValidationException(
-                "{} is abstract but missing a concrete subtype".format(result["name"])
+                f"{result['name']} is abstract but missing a concrete subtype"
             )
 
     for result in results:
         if "fields" in result:
             result["fields"] = replace_type(result["fields"], extended_by, loader, set())
 
     return results
@@ -807,12 +801,10 @@
             for field in entry.get("fields", []):
                 found = set()  # type: Set[str]
                 field_name = shortname(field["name"])
                 replace_type(field["type"], {}, loader, found, find_embeds=False)
                 for each_type in found:
                     if each_type not in primitives:
                         stream.write(
-                            '"{}" -> "{}" [label="{}"];\n'.format(
-                                label, shortname(each_type), field_name
-                            )
+                            f"{label!r} -> {shortname(each_type)!r} [label={field_name!r}];\n"
                         )
     stream.write("}\n")
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/sourceline.py` & `schema-salad-8.4.20230426093816/schema_salad/sourceline.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,51 +64,47 @@
         assert group2 is not None  # nosec
         reflowed = reflow(group2, maxno_text, g.group(3)).splitlines()
         msg.extend([pre.ljust(maxno, " ") + r for r in reflowed])
     return "\n".join(msg)
 
 
 def reflow(text: str, maxline: int, shift: Optional[str] = "") -> str:
-    if maxline < 20:
-        maxline = 20
+    maxline = max(maxline, 20)
     if len(text) > maxline:
         sp = text.rfind(" ", 0, maxline)
         if sp < 1:
             sp = text.find(" ", sp + 1)
             if sp == -1:
                 sp = len(text)
         if sp < len(text):
             return f"{text[0:sp]}\n{shift}{reflow(text[sp + 1 :], maxline, shift)}"
     return text
 
 
 def indent(v: str, nolead: bool = False, shift: str = "  ", bullet: str = "  ") -> str:
     if nolead:
         return v.splitlines()[0] + "\n".join([shift + line for line in v.splitlines()[1:]])
-    else:
 
-        def lineno(i: int, line: str) -> str:
-            r = lineno_re.match(line)
-            if r is not None:
-                group1 = r.group(1)
-                group2 = r.group(2)
-                assert group1 is not None  # nosec
-                assert group2 is not None  # nosec
-                return group1 + (bullet if i == 0 else shift) + group2
-            else:
-                return (bullet if i == 0 else shift) + line
+    def lineno(i: int, line: str) -> str:
+        r = lineno_re.match(line)
+        if r is not None:
+            group1 = r.group(1)
+            group2 = r.group(2)
+            assert group1 is not None  # nosec
+            assert group2 is not None  # nosec
+            return group1 + (bullet if i == 0 else shift) + group2
+        return (bullet if i == 0 else shift) + line
 
-        return "\n".join([lineno(i, line) for i, line in enumerate(v.splitlines())])
+    return "\n".join([lineno(i, line) for i, line in enumerate(v.splitlines())])
 
 
 def bullets(textlist: List[str], bul: str) -> str:
     if len(textlist) == 1:
         return textlist[0]
-    else:
-        return "\n".join(indent(t, bullet=bul) for t in textlist)
+    return "\n".join(indent(t, bullet=bul) for t in textlist)
 
 
 def strip_duplicated_lineno(text: str) -> str:
     """
     Strip duplicated line numbers.
 
     Same as :py:meth:`strip_dup_lineno` but without reflow.
@@ -116,15 +112,15 @@
     pre = None  # type: Optional[str]
     msg = []
     for line in text.splitlines():
         g = lineno_re.match(line)
         if not g:
             msg.append(line)
             continue
-        elif g.group(1) != pre:
+        if g.group(1) != pre:
             msg.append(line)
             pre = g.group(1)
         else:
             group1 = g.group(1)
             group2 = g.group(2)
             assert group1 is not None  # nosec
             assert group2 is not None  # nosec
@@ -220,16 +216,15 @@
             else:
                 uselc = lc
                 vfn = fn
             cs.append(cmap(v3, lc=uselc, fn=vfn))
             cs.lc.add_kv_line_col(k3, uselc)
             cs.lc.filename = fn
         return cs
-    else:
-        return d
+    return d
 
 
 class SourceLine:
     def __init__(
         self,
         item: Any,
         key: Optional[Any] = None,
@@ -253,38 +248,35 @@
         if not exc_value:
             return
         raise self.makeError(str(exc_value)) from exc_value
 
     def file(self) -> Optional[str]:
         if hasattr(self.item, "lc") and hasattr(self.item.lc, "filename"):
             return str(self.item.lc.filename)
-        else:
-            return None
+        return None
 
     def start(self) -> Optional[Tuple[int, int]]:
         if self.file() is None:
             return None
-        elif self.key is None or self.item.lc.data is None or self.key not in self.item.lc.data:
+        if self.key is None or self.item.lc.data is None or self.key not in self.item.lc.data:
             return ((self.item.lc.line or 0) + 1, (self.item.lc.col or 0) + 1)
-        else:
-            return (
-                (self.item.lc.data[self.key][0] or 0) + 1,
-                (self.item.lc.data[self.key][1] or 0) + 1,
-            )
+        return (
+            (self.item.lc.data[self.key][0] or 0) + 1,
+            (self.item.lc.data[self.key][1] or 0) + 1,
+        )
 
     def end(self) -> Optional[Tuple[int, int]]:
         return None
 
     def makeLead(self) -> str:
         if self.file():
             lcol = self.start()
             line, col = lcol if lcol else ("", "")
             return f"{self.file()}:{line}:{col}:"
-        else:
-            return ""
+        return ""
 
     def makeError(self, msg: str) -> Any:
         if not isinstance(self.item, ruamel.yaml.comments.CommentedBase):
             return self.raise_type(msg)
         errs = []
         lead = self.makeLead()
         for m in msg.splitlines():
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/EDAM.owl` & `schema-salad-8.4.20230426093816/schema_salad/tests/EDAM.owl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/Process.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/basket_schema.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/basket_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/class_field_test.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/class_field_test.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/cwl-pre.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/cwl-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/inherited-attributes.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/inherited-attributes.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/matcher.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/metaschema-pre.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/metaschema-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/pt.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/pt.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/revtool_bad_schema.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_avro_names.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_avro_names.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_cg.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_cg.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_cli_args.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_cpp_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_cwl11.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_cwl11.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_dlang_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_dotnet_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_errors.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,19 +53,19 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test1.cwl"
     match = (
-        r"""^.+test1\.cwl:2:1: Object\s+`.+test1\.cwl`\s+is\s+not valid """
-        + r"""because\s+tried `Workflow`\s+but
-\s+\* missing\s+required\s+field\s+`inputs`
-\s+\* missing\s+required\s+field\s+`outputs`
-\s+\* missing\s+required\s+field\s+`steps`$"""
+        r"""^.+test1\.cwl:2:1: Object\s+'.+test1\.cwl'\s+is\s+not valid """
+        + r"""because\s+tried 'Workflow'\s+but
+\s+\* missing\s+required\s+field\s+'inputs'
+\s+\* missing\s+required\s+field\s+'outputs'
+\s+\* missing\s+required\s+field\s+'steps'$"""
     )
     path2 = get_data("tests/" + t)
     assert path2
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, path2, True)
 
 
@@ -75,15 +75,15 @@
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test2.cwl"
     match = (
         r"""
 ^.+test2\.cwl:2:1: Field """
-        r"""`class`\s+contains\s+undefined\s+reference\s+to\s+`file://.+/schema_salad/tests/test_schema/xWorkflow`$"""[
+        r"""'class'\s+contains\s+undefined\s+reference\s+to\s+'file://.+/schema_salad/tests/test_schema/xWorkflow'$"""[
             1:
         ]
     )
     path2 = get_data("tests/" + t)
     assert path2
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, path2, True)
@@ -93,17 +93,17 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test3.cwl"
     match = r"""
-^.+test3\.cwl:5:1: checking field\s+`outputs`
-.+test3\.cwl:6:3:   checking object\s+`.+test3\.cwl#bar`
-\s+Field `type`\s+references\s+unknown\s+identifier\s+`xstring`,\s+tried
+^.+test3\.cwl:5:1: checking field\s+'outputs'
+.+test3\.cwl:6:3:   checking object\s+'.+test3\.cwl#bar'
+\s+Field 'type'\s+references\s+unknown\s+identifier\s+'xstring',\s+tried
 \s+file://.+/tests/test_schema/test3\.cwl#xstring$"""[
         1:
     ]
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
@@ -111,16 +111,16 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test4.cwl"
     match = r"""
-^.+test4\.cwl:5:1: checking field\s+`outputs`
-.+test4\.cwl:6:3:   checking object\s+`.+test4\.cwl#bar`
+^.+test4\.cwl:5:1: checking field\s+'outputs'
+.+test4\.cwl:6:3:   checking object\s+'.+test4\.cwl#bar'
 \s+'type'\s+field\s+is\s+int,\s+expected\s+string,\s+list,\s+or\s+a\s+dict.$"""[
         1:
     ]
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
@@ -128,17 +128,17 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test5.cwl"
     match = r"""
-^.+test5\.cwl:2:1: Object\s+`.+test5\.cwl`\s+is\s+not valid because
-\s+tried `Workflow`\s+but
-.+test5\.cwl:7:1:     the `steps`\s+field\s+is\s+not\s+valid\s+because
+^.+test5\.cwl:2:1: Object\s+'.+test5\.cwl'\s+is\s+not valid because
+\s+tried 'Workflow'\s+but
+.+test5\.cwl:7:1:     the 'steps'\s+field\s+is\s+not\s+valid\s+because
 \s+tried array\s+of\s+<WorkflowStep>\s+but
 .+test5\.cwl:7:9:         item is\s+invalid\s+because
 \s+is not a\s+dict$"""[
         1:
     ]
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
@@ -148,21 +148,21 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test7.cwl"
     match = (
-        r"""^.+test7\.cwl:2:1: Object\s+`.+test7\.cwl`\s+is\s+not valid because
-\s+tried `Workflow`\s+but
-.+test7\.cwl:7:1:     the `steps`\s+field\s+is\s+not\s+valid\s+because
+        r"""^.+test7\.cwl:2:1: Object\s+'.+test7\.cwl'\s+is\s+not valid because
+\s+tried 'Workflow'\s+but
+.+test7\.cwl:7:1:     the 'steps'\s+field\s+is\s+not\s+valid\s+because
 \s+tried array\s+of\s+<WorkflowStep>\s+but
 .+test7\.cwl:8:3:         item is\s+invalid\s+because
-\s+\* missing\s+required\s+field\s+`run`
-.+test7\.cwl:9:5:           \* invalid\s+field\s+`scatter_method`,\s+expected\s+one """
+\s+\* missing\s+required\s+field\s+'run'
+.+test7\.cwl:9:5:           \* invalid\s+field\s+'scatter_method',\s+expected\s+one """
         + r"""of:\s+'id',\s+'in', 'out',\s+'requirements',\s+'hints',\s+"""
         + r"""'label',\s+'doc',\s+'run',\s+'scatter',\s+'scatterMethod'$"""
     )
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
@@ -171,18 +171,18 @@
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test8.cwl"
     match = (
         r"""
-^.+test8\.cwl:7:1: checking field\s+`steps`
-.+test8\.cwl:8:3:   checking object\s+`.+test8\.cwl#step1`
+^.+test8\.cwl:7:1: checking field\s+'steps'
+.+test8\.cwl:8:3:   checking object\s+'.+test8\.cwl#step1'
 .+test8\.cwl:9:5:     """
-        r"""Field\s+`scatterMethod`\s+contains\s+undefined\s+reference\s+to\s+`file:///.+/tests/test_schema/abc`$"""[
+        r"""Field\s+'scatterMethod'\s+contains\s+undefined\s+reference\s+to\s+'file:///.+/tests/test_schema/abc'$"""[
             1:
         ]
     )
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
@@ -190,16 +190,16 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test9.cwl"
     match = (
-        r"""^.+test9\.cwl:7:1: checking field\s+`steps`
-.+test9\.cwl:8:3:   checking object\s+`.+test9\.cwl#step1`
+        r"""^.+test9\.cwl:7:1: checking field\s+'steps'
+.+test9\.cwl:8:3:   checking object\s+'.+test9\.cwl#step1'
 .+test9\.cwl:9:5:     'scatterMethod'\s+field\s+is\s+"""
         + r"""int,\s+expected\s+string,\s+list,\s+or a\s+dict.$"""
     )
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
@@ -207,21 +207,21 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test10.cwl"
     match = r"""
-^.+test10\.cwl:2:1: Object\s+`.+test10\.cwl`\s+is\s+not\s+valid\s+because
-\s+tried `Workflow`\s+but
-.+test10\.cwl:7:1:     the `steps`\s+field\s+is\s+not\s+valid\s+because
+^.+test10\.cwl:2:1: Object\s+'.+test10\.cwl'\s+is\s+not\s+valid\s+because
+\s+tried 'Workflow'\s+but
+.+test10\.cwl:7:1:     the 'steps'\s+field\s+is\s+not\s+valid\s+because
 \s+tried array\s+of\s+<WorkflowStep>\s+but
 .+test10\.cwl:8:3:         item is\s+invalid\s+because
-\s+\* missing\s+required\s+field\s+`run`
-.+test10\.cwl:9:5:           \* the\s+`scatterMethod`\s+field\s+is\s+not\s+valid\s+because
+\s+\* missing\s+required\s+field\s+'run'
+.+test10\.cwl:9:5:           \* the\s+'scatterMethod'\s+field\s+is\s+not\s+valid\s+because
 \s+value\s+is\s+a\s+CommentedSeq,\s+expected\s+null\s+or\s+ScatterMethod$"""[
         1:
     ]
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
@@ -230,18 +230,18 @@
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test11.cwl"
     match = (
         r"""
-^.+test11\.cwl:7:1: checking field\s+`steps`
-.+test11\.cwl:8:3:   checking object\s+`.+test11\.cwl#step1`
+^.+test11\.cwl:7:1: checking field\s+'steps'
+.+test11\.cwl:8:3:   checking object\s+'.+test11\.cwl#step1'
 .+test11\.cwl:9:5:     """
-        r"""Field `run`\s+contains\s+undefined\s+reference\s+to\s+`file://.+/tests/test_schema/blub\.cwl`$"""[
+        r"""Field 'run'\s+contains\s+undefined\s+reference\s+to\s+'file://.+/tests/test_schema/blub\.cwl'$"""[
             1:
         ]
     )
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
 
 
@@ -249,24 +249,24 @@
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
     assert path
     document_loader, avsc_names, schema_metadata, metaschema_loader = load_schema(path)
     assert isinstance(avsc_names, Names)
 
     t = "test_schema/test15.cwl"
     match = (
-        r"""^.+test15\.cwl:3:1:\s+Object\s+`.+test15\.cwl`\s+is not valid because
-\s+tried\s+`CommandLineTool`\s+but
-.+test15\.cwl:6:1:\s+the `inputs`\s+field\s+is\s+not valid\s+because
+        r"""^.+test15\.cwl:3:1:\s+Object\s+'.+test15\.cwl'\s+is not valid because
+\s+tried\s+'CommandLineTool'\s+but
+.+test15\.cwl:6:1:\s+the 'inputs'\s+field\s+is\s+not valid\s+because
 .+test15\.cwl:7:3:\s+item is\s+invalid\s+because
-.+test15\.cwl:9:5:\s+the\s+`inputBinding`\s+field\s+is\s+not\s+valid\s+because
+.+test15\.cwl:9:5:\s+the\s+'inputBinding'\s+field\s+is\s+not\s+valid\s+because
 .+tried\s+CommandLineBinding\s+but
-.+test15\.cwl:11:7:             \*\s+invalid\s+field\s+`invalid_field`,\s+expected\s+"""
+.+test15\.cwl:11:7:             \*\s+invalid\s+field\s+'invalid_field',\s+expected\s+"""
         + r"""one\s+of:\s+'loadContents',\s+'position',\s+'prefix',\s+'separate',"""
         + r"""\s+'itemSeparator',\s+'valueFrom',\s+'shellQuote'
-.+test15\.cwl:12:7:             \*\s+invalid\s+field\s+`another_invalid_field`,"""
+.+test15\.cwl:12:7:             \*\s+invalid\s+field\s+'another_invalid_field',"""
         + r"""\s+expected one\s+of:\s+'loadContents',\s+'position',\s+'prefix',"""
         + r"""\s+'separate',\s+'itemSeparator',\s+'valueFrom',\s+'shellQuote'$"""
     )
     with pytest.raises(ValidationException, match=match):
         load_and_validate(document_loader, avsc_names, str(get_data("tests/" + t)), True)
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_examples.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_fetch.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_fp.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_java_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_makedoc.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_misc.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_pickling.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_print_oneline.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_print_oneline.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
                 path,
                 True,
             )
         except ValidationException as e:
             msgs = to_one_line_messages(e).splitlines()
             assert len(msgs) == 2
             assert msgs[0].endswith(
-                src + ":11:7: invalid field `invalid_field`, expected one of: "
+                src + ":11:7: invalid field 'invalid_field', expected one of: "
                 "'loadContents', 'position', 'prefix', 'separate', "
                 "'itemSeparator', 'valueFrom', 'shellQuote'"
             )
             assert msgs[1].endswith(
-                src + ":12:7: invalid field `another_invalid_field`, expected one of: "
+                src + ":12:7: invalid field 'another_invalid_field', expected one of: "
                 "'loadContents', 'position', 'prefix', 'separate', 'itemSeparator', "
                 "'valueFrom', 'shellQuote'"
             )
             print("\n", e)
             raise
 
 
@@ -87,17 +87,17 @@
                 avsc_names,
                 path,
                 True,
             )
         except ValidationException as e:
             msgs = to_one_line_messages(e).splitlines()
             assert len(msgs) == 2, msgs
-            assert msgs[0].endswith(src + ":14:5: missing required field `id`")
+            assert msgs[0].endswith(src + ":14:5: missing required field 'id'")
             assert msgs[1].endswith(
-                src + ":14:5: invalid field `aa`, expected one of: 'label', "
+                src + ":14:5: invalid field 'aa', expected one of: 'label', "
                 "'secondaryFiles', 'format', 'streamable', 'doc', 'id', "
                 "'outputBinding', 'type'"
             )
             print("\n", e)
             raise
 
 
@@ -118,16 +118,16 @@
         except ValidationException as e:
             msg = to_one_line_messages(e)
             # convert Windows path to Posix path
             if "\\" in fullpath:
                 fullpath = "/" + fullpath.lower().replace("\\", "/")
             print("\n", e)
             assert msg.endswith(
-                src + ":14:5: Field `type` references unknown identifier "
-                "`Filea`, tried file://{}#Filea".format(fullpath)
+                src + ":14:5: Field 'type' references unknown identifier "
+                "'Filea', tried file://{}#Filea".format(fullpath)
             )
             raise
 
 
 def test_for_invalid_yaml1() -> None:
     # Issue 143
     path = get_data("tests/test_schema/CommonWorkflowLanguage.yml")
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_python_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_real_cwl.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_real_cwl.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_ref_resolver.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_ref_resolver.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/CommandLineTool.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/Process.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/Workflow.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/Workflow.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/avro_naming_base.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_naming_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/avro_subtype.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/avro_subtype_bad.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/avro_subtype_bad.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/cwltest-schema.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/cwltest-schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/metaschema_base.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/misc_schema_v1.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v1.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema/misc_schema_v2.yml` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema/misc_schema_v2.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schema.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_schemas_directive.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_schemas_directive.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_subtypes.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_subtypes.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/test_typescript_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/test_typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/tests/util.py` & `schema-salad-8.4.20230426093816/schema_salad/tests/util.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/.gitignore` & `schema-salad-8.4.20230426093816/schema_salad/typescript/.gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/LICENSE` & `schema-salad-8.4.20230426093816/schema_salad/typescript/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/package.json` & `schema-salad-8.4.20230426093816/schema_salad/typescript/package.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/test/AnyLoader.spec.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/test/AnyLoader.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/test/Fetcher.spec.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/test/Fetcher.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/test/IdMap.spec.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/test/IdMap.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/test/Typeguards.spec.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/test/Typeguards.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/test/utilities.spec.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/test/utilities.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/tsconfig.json` & `schema-salad-8.4.20230426093816/schema_salad/typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/Fetcher.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Fetcher.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/Internal.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Internal.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/LoadingOptions.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/LoadingOptions.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/Saveable.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Saveable.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/Typeguards.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/Typeguards.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/ValidationException.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/ValidationException.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/ArrayLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/ArrayLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/IdMapLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/IdMapLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/Loader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/Loader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/RecordLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RecordLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/RootLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/RootLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/TypeDSLLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/TypeDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/UnionLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UnionLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript/util/loaders/UriLoader.ts` & `schema-salad-8.4.20230426093816/schema_salad/typescript/util/loaders/UriLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/typescript_codegen.py` & `schema-salad-8.4.20230426093816/schema_salad/typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad/utils.py` & `schema-salad-8.4.20230426093816/schema_salad/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     """
     Wrap single items and lists.
 
     Return lists unchanged.
     """
     if isinstance(thing, MutableSequence):
         return thing
-    else:
-        return [thing]
+    return [thing]
 
 
 def flatten(thing, ltypes=(list, tuple)):
     # type: (Any, Any) -> Any
     # http://rightfootin.blogspot.com/2006/09/more-on-python-flatten.html
     if thing is None:
         return []
@@ -71,33 +70,31 @@
     i = 0
     while i < len(lst):
         while isinstance(lst[i], ltypes):
             if not lst[i]:
                 lst.pop(i)
                 i -= 1
                 break
-            else:
-                lst[i : i + 1] = lst[i]
+            lst[i : i + 1] = lst[i]
         i += 1
     return ltype(lst)
 
 
 # Check if we are on windows OS
 def onWindows():
     # type: () -> (bool)
     return os.name == "nt"
 
 
 def convert_to_dict(j4):  # type: (Any) -> Any
     if isinstance(j4, Mapping):
         return {k: convert_to_dict(v) for k, v in j4.items()}
-    elif isinstance(j4, MutableSequence):
+    if isinstance(j4, MutableSequence):
         return [convert_to_dict(v) for v in j4]
-    else:
-        return j4
+    return j4
 
 
 def json_dump(obj: Any, fp: IO[str], **kwargs: Any) -> None:
     """Force use of unicode."""
     json.dump(convert_to_dict(obj), fp, **kwargs)
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad/validate.py` & `schema-salad-8.4.20230426093816/schema_salad/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,19 @@
 
 
 def friendly(v):  # type: (Any) -> Any
     if isinstance(v, avro.schema.NamedSchema):
         return avro_shortname(v.name)
     if isinstance(v, avro.schema.ArraySchema):
         return f"array of <{friendly(v.items)}>"
-    elif isinstance(v, avro.schema.PrimitiveSchema):
+    if isinstance(v, avro.schema.PrimitiveSchema):
         return v.type
-    elif isinstance(v, avro.schema.UnionSchema):
+    if isinstance(v, avro.schema.UnionSchema):
         return " or ".join([friendly(s) for s in v.schemas])
-    else:
-        return avro_shortname(v)
+    return avro_shortname(v)
 
 
 def vpformat(datum):  # type: (Any) -> str
     a = pprint.pformat(datum)
     if len(a) > 160:
         a = a[0:160] + "[...]"
     return a
@@ -134,47 +133,47 @@
 
     if schema_type == "null":
         if datum is None:
             return True
         if raise_ex:
             raise ValidationException("the value is not null")
         return False
-    elif schema_type == "boolean":
+    if schema_type == "boolean":
         if isinstance(datum, bool):
             return True
         if raise_ex:
             raise ValidationException("the value is not boolean")
         return False
-    elif schema_type == "string":
+    if schema_type == "string":
         if isinstance(datum, str):
             return True
         if isinstance(datum, bytes):
             return True
         if raise_ex:
             raise ValidationException("the value is not string")
         return False
-    elif schema_type == "int":
+    if schema_type == "int":
         if isinstance(datum, int) and INT_MIN_VALUE <= datum <= INT_MAX_VALUE:
             return True
         if raise_ex:
-            raise ValidationException(f"`{vpformat(datum)}` is not int")
+            raise ValidationException(f"{vpformat(datum)!r} is not int")
         return False
-    elif schema_type == "long":
+    if schema_type == "long":
         if (isinstance(datum, int)) and LONG_MIN_VALUE <= datum <= LONG_MAX_VALUE:
             return True
         if raise_ex:
-            raise ValidationException(f"the value `{vpformat(datum)}` is not long")
+            raise ValidationException(f"the value {vpformat(datum)!r} is not long")
         return False
-    elif schema_type in ["float", "double"]:
-        if isinstance(datum, int) or isinstance(datum, float):
+    if schema_type in ["float", "double"]:
+        if isinstance(datum, (int, float)):
             return True
         if raise_ex:
-            raise ValidationException(f"the value `{vpformat(datum)}` is not float or double")
+            raise ValidationException(f"the value {vpformat(datum)!r} is not float or double")
         return False
-    elif isinstance(expected_schema, avro.schema.EnumSchema):
+    if isinstance(expected_schema, avro.schema.EnumSchema):
         if expected_schema.name in ("org.w3id.cwl.salad.Any", "Any"):
             if datum is not None:
                 return True
             if raise_ex:
                 raise ValidationException("'Any' type must be non-null")
             return False
         if not isinstance(datum, str):
@@ -184,33 +183,30 @@
                 )
             return False
         if expected_schema.name == "org.w3id.cwl.cwl.Expression":
             if "$(" in datum or "${" in datum:
                 return True
             if raise_ex:
                 raise ValidationException(
-                    "value `{}` does not contain an expression in the form $() or ${{}}".format(
-                        datum
-                    )
+                    f"value {datum!r} does not contain an expression in the form $() or ${{}}"
                 )
             return False
         if datum in expected_schema.symbols:
             return True
-        else:
-            if raise_ex:
-                raise ValidationException(
-                    "the value {} is not a valid {}, expected {}{}".format(
-                        vpformat(datum),
-                        expected_schema.name,
-                        "one of " if len(expected_schema.symbols) > 1 else "",
-                        "'" + "', '".join(expected_schema.symbols) + "'",
-                    )
+        if raise_ex:
+            raise ValidationException(
+                "the value {} is not a valid {}, expected {}{}".format(
+                    vpformat(datum),
+                    expected_schema.name,
+                    "one of " if len(expected_schema.symbols) > 1 else "",
+                    "'" + "', '".join(expected_schema.symbols) + "'",
                 )
-            return False
-    elif isinstance(expected_schema, avro.schema.ArraySchema):
+            )
+        return False
+    if isinstance(expected_schema, avro.schema.ArraySchema):
         if isinstance(datum, MutableSequence):
             for i, d in enumerate(datum):
                 try:
                     sl = SourceLine(datum, i, ValidationException)
                     if not validate_ex(
                         expected_schema.items,
                         d,
@@ -226,23 +222,21 @@
                         return False
                 except ValidationException as v:
                     if raise_ex:
                         source = v if debug else None
                         raise ValidationException("item is invalid because", sl, [v]) from source
                     return False
             return True
-        else:
-            if raise_ex:
-                raise ValidationException(
-                    "the value {} is not a list, expected list of {}".format(
-                        vpformat(datum), friendly(expected_schema.items)
-                    )
-                )
-            return False
-    elif isinstance(expected_schema, avro.schema.UnionSchema):
+        if raise_ex:
+            raise ValidationException(
+                f"the value {vpformat(datum)} is not a list, "
+                f"expected list of {friendly(expected_schema.items)}"
+            )
+        return False
+    if isinstance(expected_schema, avro.schema.UnionSchema):
         for s in expected_schema.schemas:
             if validate_ex(
                 s,
                 datum,
                 identifiers,
                 strict=strict,
                 raise_ex=False,
@@ -257,21 +251,21 @@
             return False
 
         errors: List[SchemaSaladException] = []
         checked = []
         for s in expected_schema.schemas:
             if isinstance(datum, MutableSequence) and not isinstance(s, avro.schema.ArraySchema):
                 continue
-            elif isinstance(datum, MutableMapping) and not isinstance(s, avro.schema.RecordSchema):
+            if isinstance(datum, MutableMapping) and not isinstance(s, avro.schema.RecordSchema):
                 continue
-            elif isinstance(datum, (bool, int, float, str)) and isinstance(
+            if isinstance(datum, (bool, int, float, str)) and isinstance(
                 s, (avro.schema.ArraySchema, avro.schema.RecordSchema)
             ):
                 continue
-            elif datum is not None and s.type == "null":
+            if datum is not None and s.type == "null":
                 continue
 
             checked.append(s)
             try:
                 validate_ex(
                     s,
                     datum,
@@ -294,45 +288,41 @@
                 None,
                 [
                     ValidationException(f"tried {friendly(check)} but", None, [err])
                     for (check, err) in zip(checked, errors)
                 ],
                 "-",
             )
-        else:
-            raise ValidationException(
-                f"value is a {type(datum).__name__}, expected {friendly(expected_schema)}"
-            )
+        raise ValidationException(
+            f"value is a {type(datum).__name__}, expected {friendly(expected_schema)}"
+        )
 
-    elif isinstance(expected_schema, avro.schema.RecordSchema):
+    if isinstance(expected_schema, avro.schema.RecordSchema):
         if not isinstance(datum, MutableMapping):
             if raise_ex:
                 raise ValidationException("is not a dict")
-            else:
-                return False
+            return False
 
         classmatch = None
         for f in expected_schema.fields:
             if f.name in ("class",):
                 d = datum.get(f.name)
                 if not d:
                     if raise_ex:
                         raise ValidationException(f"Missing {f.name!r} field")
-                    else:
-                        return False
+                    return False
                 avroname = None
                 if d in vocab:
                     avroname = avro_type_name(vocab[d])
-                if expected_schema.name != d and expected_schema.name != avroname:
+                if expected_schema.name not in (d, avroname):
                     if raise_ex:
                         raise ValidationException(
                             f"Expected class {expected_schema.name!r} but this is {d!r}"
                         )
-                    else:
-                        return False
+                    return False
                 classmatch = d
                 break
 
         errors = []
         for f in expected_schema.fields:
             if f.name in ("class",):
                 continue
@@ -358,19 +348,19 @@
                     logger=logger,
                     skip_foreign_properties=skip_foreign_properties,
                     vocab=vocab,
                 ):
                     return False
             except ValidationException as v:
                 if f.name not in datum:
-                    errors.append(ValidationException(f"missing required field `{f.name}`"))
+                    errors.append(ValidationException(f"missing required field {f.name!r}"))
                 else:
                     errors.append(
                         ValidationException(
-                            f"the `{f.name}` field is not valid because",
+                            f"the {f.name!r} field is not valid because",
                             sl,
                             [v],
                         )
                     )
 
         for d in datum:
             found = False
@@ -397,15 +387,15 @@
                         and not raise_ex
                     ):
                         return False
                     split = urlsplit(d)
                     if split.scheme:
                         if not skip_foreign_properties:
                             err = ValidationException(
-                                "unrecognized extension field `{}`{}.{}".format(
+                                "unrecognized extension field {!r}{}.{}".format(
                                     d,
                                     " and strict_foreign_properties checking is enabled"
                                     if strict_foreign_properties
                                     else "",
                                     "\nForeign properties from $schemas:\n  {}".format(
                                         "\n  ".join(sorted(foreign_properties))
                                     )
@@ -416,32 +406,28 @@
                             )
                             if strict_foreign_properties:
                                 errors.append(err)
                             elif len(foreign_properties) > 0:
                                 logger.warning(err.as_warning())
                     else:
                         err = ValidationException(
-                            "invalid field `{}`, expected one of: {}".format(
+                            "invalid field {!r}, expected one of: {}".format(
                                 d,
                                 ", ".join(f"{fn.name!r}" for fn in expected_schema.fields),
                             ),
                             sl,
                         )
                         if strict:
                             errors.append(err)
                         else:
                             logger.warning(err.as_warning())
 
         if bool(errors):
             if raise_ex:
                 if classmatch:
                     raise ClassValidationException("", None, errors, "*")
-                else:
-                    raise ValidationException("", None, errors, "*")
-            else:
-                return False
-        else:
-            return True
+                raise ValidationException("", None, errors, "*")
+            return False
+        return True
     if raise_ex:
         raise ValidationException(f"Unrecognized schema_type {schema_type}")
-    else:
-        return False
+    return False
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad.Dockerfile` & `schema-salad-8.4.20230426093816/schema_salad.Dockerfile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/schema_salad.egg-info/PKG-INFO` & `schema-salad-8.4.20230426093816/schema_salad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230213094415
+Version: 8.4.20230426093816
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.4.20230213094415/schema_salad.egg-info/SOURCES.txt` & `schema-salad-8.4.20230426093816/schema_salad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/setup.py` & `schema-salad-8.4.20230426093816/setup.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230213094415/tox.ini` & `schema-salad-8.4.20230426093816/tox.ini`

 * *Files identical despite different names*

