# Comparing `tmp/spectrum_utils-0.4.1.tar.gz` & `tmp/spectrum_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_utils-0.4.1.tar", last modified: Mon Oct 10 17:01:34 2022, max compression
+gzip compressed data, was "spectrum_utils-0.4.2.tar", last modified: Wed Apr 26 07:47:29 2023, max compression
```

## Comparing `spectrum_utils-0.4.1.tar` & `spectrum_utils-0.4.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.550987 spectrum_utils-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.542986 spectrum_utils-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.546986 spectrum_utils-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)    11087 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-10-10 17:01:34.550987 spectrum_utils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.546986 spectrum_utils-0.4.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (121)      754 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.546986 spectrum_utils-0.4.1/docs/src/
--rw-r--r--   0 runner    (1001) docker     (121)   150758 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/annot_fmt.png
--rw-r--r--   0 runner    (1001) docker     (121)    12433 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/annotating.md
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/api.md
--rw-r--r--   0 runner    (1001) docker     (121)     6666 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/contact.md
--rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/install.md
--rw-r--r--   0 runner    (1001) docker     (121)    98756 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/ion_types.png
--rw-r--r--   0 runner    (1001) docker     (121)    60346 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/iplot_mirror.json
--rw-r--r--   0 runner    (1001) docker     (121)    26121 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/iplot_spectrum.json
--rw-r--r--   0 runner    (1001) docker     (121)    97596 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/mirror.png
--rw-r--r--   0 runner    (1001) docker     (121)    90737 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/neutral_losses_1.png
--rw-r--r--   0 runner    (1001) docker     (121)    90032 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/neutral_losses_2.png
--rw-r--r--   0 runner    (1001) docker     (121)     9627 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/plotting.md
--rw-r--r--   0 runner    (1001) docker     (121)   286706 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/proforma_ast.png
--rw-r--r--   0 runner    (1001) docker     (121)    78234 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/proforma_ex1.png
--rw-r--r--   0 runner    (1001) docker     (121)    81081 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/proforma_ex2.png
--rw-r--r--   0 runner    (1001) docker     (121)    78458 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/proforma_ex3.png
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (121)    70278 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/quickstart.png
--rw-r--r--   0 runner    (1001) docker     (121)     5977 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/runtime.md
--rw-r--r--   0 runner    (1001) docker     (121)    50212 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/docs/src/runtime.png
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-10-10 17:01:34.550987 spectrum_utils-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.550987 spectrum_utils-0.4.1/spectrum_utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)      481 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17262 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/fragment_annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5655 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/iplot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/monosaccharide.lark
--rwxr-xr-x   0 runner    (1001) docker     (121)     8553 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/proforma.ebnf
--rw-r--r--   0 runner    (1001) docker     (121)    30527 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/proforma.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    27142 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/spectrum_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.550987 spectrum_utils-0.4.1/spectrum_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-10-10 17:01:34.000000 spectrum_utils-0.4.1/spectrum_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-10-10 17:01:34.000000 spectrum_utils-0.4.1/spectrum_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 17:01:34.000000 spectrum_utils-0.4.1/spectrum_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-10 17:01:34.000000 spectrum_utils-0.4.1/spectrum_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-10 17:01:34.000000 spectrum_utils-0.4.1/spectrum_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:34.550987 spectrum_utils-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10956 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/tests/fragment_annotation_test.py
--rw-r--r--   0 runner    (1001) docker     (121)   113507 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/tests/proforma_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    21290 2022-10-10 17:01:19.000000 spectrum_utils-0.4.1/tests/spectrum_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.798618 spectrum_utils-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.790618 spectrum_utils-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.790618 spectrum_utils-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11087 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-26 07:47:29.798618 spectrum_utils-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.790618 spectrum_utils-0.4.2/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.794618 spectrum_utils-0.4.2/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   150758 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/annot_fmt.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/annotating.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/contact.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)    98756 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/ion_types.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60346 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/iplot_mirror.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/iplot_spectrum.json
+-rw-r--r--   0 runner    (1001) docker     (123)    97596 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/mirror.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90737 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/neutral_losses_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90032 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/neutral_losses_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (123)   286706 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/proforma_ast.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78234 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/proforma_ex1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81081 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/proforma_ex2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78458 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/proforma_ex3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)    70278 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/quickstart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/runtime.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50212 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/docs/src/runtime.png
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-26 07:47:29.798618 spectrum_utils-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.798618 spectrum_utils-0.4.2/spectrum_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/fragment_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/iplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/monosaccharide.lark
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8537 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/proforma.ebnf
+-rw-r--r--   0 runner    (1001) docker     (123)    30527 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/proforma.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27574 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/spectrum_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.798618 spectrum_utils-0.4.2/spectrum_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-26 07:47:29.000000 spectrum_utils-0.4.2/spectrum_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 07:47:29.000000 spectrum_utils-0.4.2/spectrum_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:47:29.000000 spectrum_utils-0.4.2/spectrum_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-26 07:47:29.000000 spectrum_utils-0.4.2/spectrum_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 07:47:29.000000 spectrum_utils-0.4.2/spectrum_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:29.798618 spectrum_utils-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/tests/fragment_annotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113507 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/tests/proforma_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21290 2023-04-26 07:47:08.000000 spectrum_utils-0.4.2/tests/spectrum_test.py
```

### Comparing `spectrum_utils-0.4.1/.github/workflows/black.yml` & `spectrum_utils-0.4.2/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/.github/workflows/publish.yml` & `spectrum_utils-0.4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/.github/workflows/tests.yml` & `spectrum_utils-0.4.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/.gitignore` & `spectrum_utils-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/CODE_OF_CONDUCT.md` & `spectrum_utils-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/CONTRIBUTING.md` & `spectrum_utils-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/LICENSE.txt` & `spectrum_utils-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/PKG-INFO` & `spectrum_utils-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Mass spectrometry utility functions
 Home-page: https://github.com/bittremieux/spectrum_utils
 Author: Wout Bittremieux
 Author-email: wbittremieux@health.ucsd.edu
 License: Apache 2.0
 Project-URL: Documentation, https://spectrum-utils.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/bittremieux/spectrum_utils/issues
```

### Comparing `spectrum_utils-0.4.1/README.md` & `spectrum_utils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/Makefile` & `spectrum_utils-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/make.bat` & `spectrum_utils-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/annot_fmt.png` & `spectrum_utils-0.4.2/docs/src/annot_fmt.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/annotating.md` & `spectrum_utils-0.4.2/docs/src/annotating.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/api.md` & `spectrum_utils-0.4.2/docs/src/api.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/conf.py` & `spectrum_utils-0.4.2/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/contact.md` & `spectrum_utils-0.4.2/docs/src/contact.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/index.md` & `spectrum_utils-0.4.2/docs/src/index.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/install.md` & `spectrum_utils-0.4.2/docs/src/install.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/ion_types.png` & `spectrum_utils-0.4.2/docs/src/ion_types.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/iplot_mirror.json` & `spectrum_utils-0.4.2/docs/src/iplot_mirror.json`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/iplot_spectrum.json` & `spectrum_utils-0.4.2/docs/src/iplot_spectrum.json`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/mirror.png` & `spectrum_utils-0.4.2/docs/src/mirror.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/neutral_losses_1.png` & `spectrum_utils-0.4.2/docs/src/neutral_losses_1.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/neutral_losses_2.png` & `spectrum_utils-0.4.2/docs/src/neutral_losses_2.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/plotting.md` & `spectrum_utils-0.4.2/docs/src/plotting.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/proforma_ast.png` & `spectrum_utils-0.4.2/docs/src/proforma_ast.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/proforma_ex1.png` & `spectrum_utils-0.4.2/docs/src/proforma_ex1.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/proforma_ex2.png` & `spectrum_utils-0.4.2/docs/src/proforma_ex2.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/proforma_ex3.png` & `spectrum_utils-0.4.2/docs/src/proforma_ex3.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/quickstart.md` & `spectrum_utils-0.4.2/docs/src/quickstart.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/quickstart.png` & `spectrum_utils-0.4.2/docs/src/quickstart.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/runtime.md` & `spectrum_utils-0.4.2/docs/src/runtime.md`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/docs/src/runtime.png` & `spectrum_utils-0.4.2/docs/src/runtime.png`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/pyproject.toml` & `spectrum_utils-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/setup.cfg` & `spectrum_utils-0.4.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	appdirs
 	fastobo
 	lark>=1.0
-	matplotlib
+	matplotlib>=3.5
 	numba>=0.47
 	numpy
 	pyteomics>=4.5
 
 [options.extras_require]
 dev = 
 	black
```

### Comparing `spectrum_utils-0.4.1/spectrum_utils/fragment_annotation.py` & `spectrum_utils-0.4.2/spectrum_utils/fragment_annotation.py`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/spectrum_utils/iplot.py` & `spectrum_utils-0.4.2/spectrum_utils/iplot.py`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/spectrum_utils/monosaccharide.lark` & `spectrum_utils-0.4.2/spectrum_utils/monosaccharide.lark`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/spectrum_utils/plot.py` & `spectrum_utils-0.4.2/spectrum_utils/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,17 +171,17 @@
     ax.set_ylim(*(0, 1) if not mirror_intensity else (-1, 0))
 
     ax.xaxis.set_minor_locator(mticker.AutoLocator())
     ax.yaxis.set_minor_locator(mticker.AutoLocator())
     ax.xaxis.set_minor_locator(mticker.AutoMinorLocator())
     ax.yaxis.set_minor_locator(mticker.AutoMinorLocator())
     if grid in (True, "both", "major"):
-        ax.grid(b=True, which="major", color="#9E9E9E", linewidth=0.2)
+        ax.grid(True, "major", color="#9E9E9E", linewidth=0.2)
     if grid in (True, "both", "minor"):
-        ax.grid(b=True, which="minor", color="#9E9E9E", linewidth=0.2)
+        ax.grid(True, "minor", color="#9E9E9E", linewidth=0.2)
     ax.set_axisbelow(True)
 
     ax.tick_params(axis="both", which="both", labelsize="small")
 
     ax.set_xlabel("m/z", style="italic")
     ax.set_ylabel("Intensity")
```

### Comparing `spectrum_utils-0.4.1/spectrum_utils/proforma.ebnf` & `spectrum_utils-0.4.2/spectrum_utils/proforma.ebnf`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/spectrum_utils/proforma.py` & `spectrum_utils-0.4.2/spectrum_utils/proforma.py`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/spectrum_utils/spectrum.py` & `spectrum_utils-0.4.2/spectrum_utils/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,14 +514,19 @@
             The number of precursor isotopic peaks to be checked (the default
             is 0 to check only the mono-isotopic peaks).
 
         Returns
         -------
         MsmsSpectrum
         """
+        if fragment_tol_mode not in ("Da", "ppm"):
+            raise ValueError(
+                "Unknown fragment mass tolerance unit specified. Supported "
+                'values are "Da" or "ppm".'
+            )
         self.proforma, self._annotation = None, None
         self._inner.remove_precursor_peak(
             fragment_tol_mass, fragment_tol_mode, isotope
         )
         return self
 
     def filter_intensity(
@@ -668,14 +673,19 @@
             - Loss of mercaptoacetic acid (C2H4O2S): -91.993211.
             - Loss of phosphoric acid (H3PO4): -97.976896.
 
         Returns
         -------
         MsmsSpectrum
         """
+        if fragment_tol_mode not in ("Da", "ppm"):
+            raise ValueError(
+                "Unknown fragment mass tolerance unit specified. Supported "
+                'values are "Da" or "ppm".'
+            )
         mass_diff = functools.partial(
             utils.mass_diff, mode_is_da=fragment_tol_mode == "Da"
         )
 
         self.proforma = proforma_str
         self._annotation = np.full_like(self.mz, None, object)
         # By default, peak charges are assumed to be smaller than the precursor
```

### Comparing `spectrum_utils-0.4.1/spectrum_utils.egg-info/PKG-INFO` & `spectrum_utils-0.4.2/spectrum_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Mass spectrometry utility functions
 Home-page: https://github.com/bittremieux/spectrum_utils
 Author: Wout Bittremieux
 Author-email: wbittremieux@health.ucsd.edu
 License: Apache 2.0
 Project-URL: Documentation, https://spectrum-utils.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/bittremieux/spectrum_utils/issues
```

### Comparing `spectrum_utils-0.4.1/spectrum_utils.egg-info/SOURCES.txt` & `spectrum_utils-0.4.2/spectrum_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/tests/fragment_annotation_test.py` & `spectrum_utils-0.4.2/tests/fragment_annotation_test.py`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/tests/proforma_test.py` & `spectrum_utils-0.4.2/tests/proforma_test.py`

 * *Files identical despite different names*

### Comparing `spectrum_utils-0.4.1/tests/spectrum_test.py` & `spectrum_utils-0.4.2/tests/spectrum_test.py`

 * *Files identical despite different names*

