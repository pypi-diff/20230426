# Comparing `tmp/timeseriesflattener-0.24.0.tar.gz` & `tmp/timeseriesflattener-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-0.24.0.tar", last modified: Thu Apr 20 09:05:05 2023, max compression
+gzip compressed data, was "timeseriesflattener-0.25.0.tar", last modified: Wed Apr 26 12:36:47 2023, max compression
```

## Comparing `timeseriesflattener-0.24.0.tar` & `timeseriesflattener-0.25.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/
--rw-r--r--   0 root         (0) root         (0)      489 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.083044 timeseriesflattener-0.24.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.083044 timeseriesflattener-0.24.0/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.087044 timeseriesflattener-0.24.0/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.087044 timeseriesflattener-0.24.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      877 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3027 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    53313 2023-04-20 09:04:52.000000 timeseriesflattener-0.24.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    11584 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/README.md
--rw-r--r--   0 root         (0) root         (0)      658 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.091044 timeseriesflattener-0.24.0/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.091044 timeseriesflattener-0.24.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4211 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      320 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.091044 timeseriesflattener-0.24.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   130812 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    68248 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    77800 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.095044 timeseriesflattener-0.24.0/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.095044 timeseriesflattener-0.24.0/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4418 2023-04-20 09:04:52.000000 timeseriesflattener-0.24.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.095044 timeseriesflattener-0.24.0/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      226 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6145 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
--rw-r--r--   0 root         (0) root         (0)    40328 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/feature_spec_objects.py
--rw-r--r--   0 root         (0) root         (0)    36771 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/resolve_multiple_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3168 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/load_synth_data.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/testing/utils_for_testing.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/src/timeseriesflattener/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11584 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-20 09:05:05.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-20 09:05:04.000000 timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9157 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/tests/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.079044 timeseriesflattener-0.24.0/tests/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.099044 timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1477 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.103044 timeseriesflattener-0.24.0/tests/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.115044 timeseriesflattener-0.24.0/tests/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      779 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-04-20 09:04:50.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_data/raw/synth_text_data.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.115044 timeseriesflattener-0.24.0/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3490 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7778 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:05:05.119045 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18335 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     6598 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)    15009 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_resolve_multiple.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-20 09:04:51.000000 timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.974283 timeseriesflattener-0.25.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.938280 timeseriesflattener-0.25.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.930280 timeseriesflattener-0.25.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.938280 timeseriesflattener-0.25.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.938280 timeseriesflattener-0.25.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.942280 timeseriesflattener-0.25.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      877 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    53821 2023-04-26 12:36:37.000000 timeseriesflattener-0.25.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-04-26 12:36:47.974283 timeseriesflattener-0.25.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9185 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      658 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.942280 timeseriesflattener-0.25.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.942280 timeseriesflattener-0.25.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.946281 timeseriesflattener-0.25.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   130812 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    68248 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    77800 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.946281 timeseriesflattener-0.25.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.950281 timeseriesflattener-0.25.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-04-26 12:36:37.000000 timeseriesflattener-0.25.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:36:47.974283 timeseriesflattener-0.25.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.934280 timeseriesflattener-0.25.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.950281 timeseriesflattener-0.25.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.954281 timeseriesflattener-0.25.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6145 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+-rw-r--r--   0 root         (0) root         (0)    40328 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/feature_spec_objects.py
+-rw-r--r--   0 root         (0) root         (0)    36771 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     5387 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/resolve_multiple_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.954281 timeseriesflattener-0.25.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/testing/load_synth_data.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/testing/utils_for_testing.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/src/timeseriesflattener/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.954281 timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-04-26 12:36:47.000000 timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-26 12:36:47.000000 timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:36:47.000000 timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-26 12:36:47.000000 timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-26 12:36:47.000000 timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9157 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.954281 timeseriesflattener-0.25.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.934280 timeseriesflattener-0.25.0/tests/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.934280 timeseriesflattener-0.25.0/tests/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.954281 timeseriesflattener-0.25.0/tests/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.958282 timeseriesflattener-0.25.0/tests/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.970282 timeseriesflattener-0.25.0/tests/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      779 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_data/raw/synth_text_data.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.970282 timeseriesflattener-0.25.0/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.974283 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     7778 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:36:47.974283 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18335 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     6598 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16795 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_resolve_multiple.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-26 12:36:35.000000 timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_utils.py
```

### Comparing `timeseriesflattener-0.24.0/.cruft.json` & `timeseriesflattener-0.25.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/actions/test/action.yml` & `timeseriesflattener-0.25.0/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-0.25.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/dependabot.yml` & `timeseriesflattener-0.25.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/recommended_repo_setup.md` & `timeseriesflattener-0.25.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-0.25.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/cruft.yml` & `timeseriesflattener-0.25.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-0.25.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/documentation.yml` & `timeseriesflattener-0.25.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-0.25.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-0.25.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/pre-commit.yml` & `timeseriesflattener-0.25.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/stalebot.yml` & `timeseriesflattener-0.25.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-0.25.0/.github/workflows/static_type_checks.yml`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,21 @@
         id: setup_python
         with:
           python-version: "3.8"
 
       - name: Install dependencies
         shell: bash
         run: |
-          pip install tox
+          pip install invoke tox
 
       - name: Run static type checker
         id: pyright
         continue-on-error: true
         run: |
-          if tox -e type; then
+          if inv static-type-checks; then
             echo "pyright check passed"
             echo "pyright_failed=0" >> $GITHUB_OUTPUT
           else
             echo "pyright check failed"
             echo "pyright_failed=1" >> $GITHUB_OUTPUT
           fi
 
@@ -81,8 +81,8 @@
           message: |
             🌟 pyright succeeds! 🌟
 
       - name: Show pyright output
         id: fail_run
         if: ${{steps.pyright.outputs.pyright_failed == 1}}
         run: |
-          tox -e type # Rerunning pyright isn't optimal computationally, but typically takes no more than a couple of seconds, and this ensures that the errors are in the failing step
+          inv static-type-checks # Rerunning pyright isn't optimal computationally, but typically takes no more than a couple of seconds, and this ensures that the errors are in the failing step
```

### Comparing `timeseriesflattener-0.24.0/.gitignore` & `timeseriesflattener-0.25.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.pre-commit-config.yaml` & `timeseriesflattener-0.25.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/.zenodo.json` & `timeseriesflattener-0.25.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/CHANGELOG.md` & `timeseriesflattener-0.25.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.25.0 (2023-04-26)
+### Feature
+* Add type-token-ratio resolve multiple fn ([`12be531`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/12be531382e1702fe21d9698dfa3ecaf256be8bb))
+* Mean_len ([`3a38cd5`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3a38cd593f949c498fba2942b2b603a351389c05))
+
+### Fix
+* Remove undone test ([`07ecfca`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/07ecfca2af68a839c4a48d289a7677580b9214bf))
+
 ## v0.24.0 (2023-04-20)
 ### Feature
 * Modify invoke test command to take python-versions arg ([`4a9c5c2`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/4a9c5c2e672fc67bd56e57313588f09737b69f88))
 * Improve type hints ([`d53e61e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/d53e61e0b7037064b1cb4e0a29455c5523749dba))
 
 ### Fix
 * Support multiple python versions for testing ([`d929147`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/d929147cc14b59947b559501e31eec60f278f1fc))
```

### Comparing `timeseriesflattener-0.24.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-0.25.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/CONTRIBUTING.md` & `timeseriesflattener-0.25.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/LICENSE` & `timeseriesflattener-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/PKG-INFO` & `timeseriesflattener-0.25.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.24.0
+Version: 0.25.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.24.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.25.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-0.24.0/README.md` & `timeseriesflattener-0.25.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/citation.cff` & `timeseriesflattener-0.25.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/Makefile` & `timeseriesflattener-0.25.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/_static/favicon.ico` & `timeseriesflattener-0.25.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/_static/icon.png` & `timeseriesflattener-0.25.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/_static/icon_dark.png` & `timeseriesflattener-0.25.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/_static/terminology_figure.png` & `timeseriesflattener-0.25.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/conf.py` & `timeseriesflattener-0.25.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/faq.rst` & `timeseriesflattener-0.25.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/index.rst` & `timeseriesflattener-0.25.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-0.25.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-0.25.0/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-0.25.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-0.25.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-0.25.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-0.25.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-0.25.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/icon.png` & `timeseriesflattener-0.25.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/paper/paper.bib` & `timeseriesflattener-0.25.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/paper/paper.md` & `timeseriesflattener-0.25.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/pyproject.toml` & `timeseriesflattener-0.25.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "0.24.0"
+version = "0.25.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
@@ -19,15 +19,15 @@
 requires-python = ">=3.8.0,<3.12.0"
 dependencies = [
     "scipy>=1.8.0,<1.9.4",
     "scikit-learn>=1.1.2,<1.2.3",
     "pydantic>=1.9.0, <1.11.0",
     "pandas>=1.4.0,<2.1.0",
     "catalogue>=2.0.0, <2.1.0",
-    "numpy>=1.23.3,<1.24.2",
+    "numpy>=1.23.3,<1.24.4",
     "pyarrow>=9.0.0,<11.1.0",
     "protobuf<=4.22.3", # Other versions give errors with pytest, super weird!
     "frozendict>=2.3.4,<2.4.0",
     "coloredlogs>14.0.0,<15.1.0",
     "psycopmlutils>=0.5.0, <0.12.0",
 ]
 
@@ -48,15 +48,15 @@
 test = [
   "pytest>=7.1.3,<7.3.0",
   "pytest-cov>=3.0.0,<3.1.0",
   "pytest-xdist>=3.0.0,<3.2.0",
   "pytest-sugar>=0.9.4,<0.10.0",
 ]
 docs = [
-    "sphinx>=5.3.0,<6.2.0",
+    "sphinx>=5.3.0,<6.3.0",
     "furo==2023.3.27",
     "sphinx-copybutton>=0.5.1,<0.5.3",
     "sphinxext-opengraph>=0.7.3,<0.8.3",
     "myst-nb>=0.6.0,<1.17.0",
     "sphinx_design>=0.3.0,<0.3.1",
     "autodoc_pydantic>=1.1.0,<1.9.0",
 ]
```

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/feature_spec_objects.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/logger.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/resolve_multiple_functions.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/resolve_multiple_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -121,12 +121,69 @@
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
         DataFrame: Dataframe with value column containing the concatenated values.
     """
+
     return grouped_df.apply(
         lambda x: Series(
             {"value": " ".join(x.value)},
         ),
     )
+
+
+@resolve_multiple_fns.register("mean_len")
+def mean_number_of_characters(grouped_df: DataFrame) -> DataFrame:
+    """Returns the mean length of values. This is useful for text data.
+
+    Args:
+        grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
+
+    Returns:
+        DataFrame: Dataframe with value column containing the concatenated values.
+    """
+    return grouped_df.apply(
+        lambda x: Series(
+            {"value": x.value.str.len().mean()},
+        ),
+    )
+
+
+@resolve_multiple_fns.register("type_token_ratio")
+def type_token_ratio(grouped_df: DataFrame) -> DataFrame:
+    """Returns the type-token ratio. This is useful for text data.
+
+    Args:
+        grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
+
+    Returns:
+        DataFrame: Dataframe with value column containing the concatenated values.
+    """
+
+    return grouped_df.apply(
+        lambda x: Series(
+            {
+                "value": len(
+                    set(
+                        " ".join(
+                            x.value.replace(
+                                r"[^ÆØÅæøåA-Za-z0-9 ]+",
+                                "",
+                                regex=True,
+                            ).str.lower(),
+                        ).split(" "),
+                    ),
+                )
+                / len(
+                    " ".join(
+                        x.value.replace(
+                            r"[^ÆØÅæøåA-Za-z0-9 ]+",
+                            "",
+                            regex=True,
+                        ).str.lower(),
+                    ).split(" "),
+                ),
+            },
+        ),
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener/utils.py` & `timeseriesflattener-0.25.0/src/timeseriesflattener/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.24.0
+Version: 0.25.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.24.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.25.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-0.25.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 scipy<1.9.4,>=1.8.0
 scikit-learn<1.2.3,>=1.1.2
 pydantic<1.11.0,>=1.9.0
 pandas<2.1.0,>=1.4.0
 catalogue<2.1.0,>=2.0.0
-numpy<1.24.2,>=1.23.3
+numpy<1.24.4,>=1.23.3
 pyarrow<11.1.0,>=9.0.0
 protobuf<=4.22.3
 frozendict<2.4.0,>=2.3.4
 coloredlogs<15.1.0,>14.0.0
 psycopmlutils<0.12.0,>=0.5.0
 
 [dev]
@@ -17,15 +17,15 @@
 ruff==0.0.262
 black[jupyter]==22.8.0
 pandas-stubs
 invoke
 tox
 
 [docs]
-sphinx<6.2.0,>=5.3.0
+sphinx<6.3.0,>=5.3.0
 furo==2023.3.27
 sphinx-copybutton<0.5.3,>=0.5.1
 sphinxext-opengraph<0.8.3,>=0.7.3
 myst-nb<1.17.0,>=0.6.0
 sphinx_design<0.3.1,>=0.3.0
 autodoc_pydantic<1.9.0,>=1.1.0
```

### Comparing `timeseriesflattener-0.24.0/tasks.py` & `timeseriesflattener-0.25.0/tasks.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/conftest.py` & `timeseriesflattener-0.25.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-0.25.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-0.25.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-0.25.0/tests/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-0.25.0/tests/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-0.25.0/tests/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/create_synth_sex.py` & `timeseriesflattener-0.25.0/tests/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-0.25.0/tests/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-0.25.0/tests/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/synth_sex.csv` & `timeseriesflattener-0.25.0/tests/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_data/raw/synth_text_data.csv` & `timeseriesflattener-0.25.0/tests/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-0.25.0/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_resolve_multiple.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_resolve_multiple.py`

 * *Files 5% similar despite different names*

```diff
@@ -444,7 +444,56 @@
             resolve_multiple_fn="concatenate",
             interval_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=["the patient is feeling ill"],
     )
+
+
+def test_resolve_multiple_mean_len():
+    prediction_times_str = """entity_id,timestamp,
+                            1,2021-12-31 00:00:00
+                            """
+    event_times_str = """entity_id,timestamp,value,
+                        1,2022-01-01 00:00:00,the patient
+                        1,2022-01-02 00:00:00,is feeling ill
+                        """
+
+    assert_flattened_data_as_expected(
+        prediction_times_df=prediction_times_str,
+        output_spec=OutcomeSpec(
+            feature_name="value",
+            values_df=str_to_df(event_times_str),
+            resolve_multiple_fn="mean_number_of_characters",
+            interval_days=4,
+            fallback=np.NaN,
+            incident=False,
+        ),
+        expected_values=[12.5],
+    )
+
+
+def test_resolve_multiple_type_token_ratio():
+    prediction_times_str = """entity_id,timestamp,
+                            1,2021-12-31 00:00:00
+                            2,2021-12-31 00:00:00
+                            """
+    event_times_str = """entity_id,timestamp,value,
+                        1,2022-01-01 00:00:00,The patient feels very tired!
+                        1,2022-01-02 00:00:00,The patient is tired tired.
+                        2,2022-01-01 00:00:00,The patient feels very happy!
+                        2,2022-01-02 00:00:00,The patient is feeling tired.
+                        """
+
+    assert_flattened_data_as_expected(
+        prediction_times_df=prediction_times_str,
+        output_spec=OutcomeSpec(
+            feature_name="value",
+            values_df=str_to_df(event_times_str),
+            resolve_multiple_fn="type_token_ratio",
+            interval_days=4,
+            fallback=np.NaN,
+            incident=False,
+        ),
+        expected_values=[0.6, 0.8],
+    )
```

### Comparing `timeseriesflattener-0.24.0/tests/test_timeseriesflattener/test_utils.py` & `timeseriesflattener-0.25.0/tests/test_timeseriesflattener/test_utils.py`

 * *Files identical despite different names*

