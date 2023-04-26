# Comparing `tmp/balance-0.7.0.tar.gz` & `tmp/balance-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balance-0.7.0.tar", last modified: Mon Apr 10 08:02:05 2023, max compression
+gzip compressed data, was "balance-0.8.0.tar", last modified: Wed Apr 26 13:49:21 2023, max compression
```

## Comparing `balance-0.7.0.tar` & `balance-0.8.0.tar`

### file list

```diff
@@ -1,196 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 08:00:29.000000 balance-0.7.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.188347 balance-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 08:00:29.000000 balance-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-10 08:00:29.000000 balance-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.188347 balance-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-10 08:00:29.000000 balance-0.7.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-10 08:00:29.000000 balance-0.7.0/.github/workflows/deploy-website.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-10 08:00:29.000000 balance-0.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-10 08:00:29.000000 balance-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-10 08:00:29.000000 balance-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-10 08:00:29.000000 balance-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-10 08:00:29.000000 balance-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-04-10 08:00:29.000000 balance-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-04-10 08:00:29.000000 balance-0.7.0/LICENSE-DOCUMENTATION
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-10 08:02:05.216347 balance-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-10 08:00:29.000000 balance-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-10 08:00:29.000000 balance-0.7.0/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-04-10 08:00:29.000000 balance-0.7.0/balance/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    77711 2023-04-10 08:00:29.000000 balance-0.7.0/balance/balancedf_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    26001 2023-04-10 08:00:29.000000 balance-0.7.0/balance/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-04-10 08:00:29.000000 balance-0.7.0/balance/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-10 08:00:29.000000 balance-0.7.0/balance/datasets/sim_data_cbps.R
--rw-r--r--   0 runner    (1001) docker     (123)    55895 2023-04-10 08:00:29.000000 balance-0.7.0/balance/datasets/sim_data_cbps.csv
--rw-r--r--   0 runner    (1001) docker     (123)    52104 2023-04-10 08:00:29.000000 balance-0.7.0/balance/sample_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance/stats_and_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/general_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    59199 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weighted_comparisons_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weighted_comparisons_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    26952 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weighted_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-10 08:00:29.000000 balance-0.7.0/balance/stats_and_plots/weights_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-10 08:00:29.000000 balance-0.7.0/balance/testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-10 08:00:29.000000 balance-0.7.0/balance/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78678 2023-04-10 08:00:29.000000 balance-0.7.0/balance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/balance/weighting_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/adjust_null.py
--rw-r--r--   0 runner    (1001) docker     (123)    29249 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/cbps.py
--rw-r--r--   0 runner    (1001) docker     (123)    26505 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/ipw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-10 08:00:29.000000 balance-0.7.0/balance/weighting_methods/poststratify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.192347 balance-0.7.0/balance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-10 08:02:05.000000 balance-0.7.0/balance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:02:04.000000 balance-0.7.0/balance.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3373 2023-04-10 08:00:29.000000 balance-0.7.0/scripts/make_docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:02:05.216347 balance-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-10 08:00:29.000000 balance-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/sphinx/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/sphinx/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/sphinx/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.196347 balance-0.7.0/sphinx/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/balance.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-10 08:00:29.000000 balance-0.7.0/sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_adjust_null.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    43626 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_balancedf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_cbps.py
--rw-r--r--   0 runner    (1001) docker     (123)    38390 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_ipw.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_poststratify.py
--rw-r--r--   0 runner    (1001) docker     (123)    39114 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    32798 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_stats_and_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49276 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-04-10 08:00:29.000000 balance-0.7.0/tests/test_weighted_comparisons_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    22555 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/balance_quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   590306 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/balance_quickstart_cbps.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/balance_transformations_and_formulas.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-10 08:00:29.000000 balance-0.7.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/website/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 08:00:29.000000 balance-0.7.0/website/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-10 08:00:29.000000 balance-0.7.0/website/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 08:00:29.000000 balance-0.7.0/website/babel.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/blog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/blog/2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/blog/2023/01/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.200347 balance-0.7.0/website/blog/2023/01/09/
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-10 08:00:29.000000 balance-0.7.0/website/blog/2023/01/09/bringing-balance-to-your-data.md
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-04-10 08:00:29.000000 balance-0.7.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.204347 balance-0.7.0/website/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/api_reference/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.204347 balance-0.7.0/website/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.204347 balance-0.7.0/website/docs/docs/general_framework/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/adjusting_sample_to_population.md
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/evaluation_of_results.md
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/general_framework.md
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/docs/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_01_qqplot_income_before.png
--rw-r--r--   0 runner    (1001) docker     (123)    41572 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_02_barplot_age_before.png
--rw-r--r--   0 runner    (1001) docker     (123)    38449 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_03_barplot_gender_before.png
--rw-r--r--   0 runner    (1001) docker     (123)    61834 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_04_qqplot_income_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    45979 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_05_barplot_age_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    41950 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_06_barplot_gender_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    41877 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_07_seaborn_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_08_weights_kde.png
--rw-r--r--   0 runner    (1001) docker     (123)    28925 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png
--rw-r--r--   0 runner    (1001) docker     (123)   468436 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.png
--rw-r--r--   0 runner    (1001) docker     (123)    26229 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68569 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/img/total_survey_error_image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/docs/docs/statistical_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/cbps.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/ipw.md
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/docs/statistical_methods/poststratify.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/balance_transformations_and_formulas.mdx
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/index.mdx
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/quickstart.mdx
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-10 08:00:29.000000 balance-0.7.0/website/docs/tutorials/quickstart_cbps.mdx
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-10 08:00:29.000000 balance-0.7.0/website/docusaurus.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-10 08:00:29.000000 balance-0.7.0/website/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-10 08:00:29.000000 balance-0.7.0/website/sidebars.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/components/HTMLLoader.js
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/components/HomepageFeatures.js
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/components/HomepageFeatures.module.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/src/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.208347 balance-0.7.0/website/src/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/pages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/pages/index.module.css
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 08:00:29.000000 balance-0.7.0/website/src/pages/markdown-page.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/AI/
--rw-r--r--   0 runner    (1001) docker     (123)   460628 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/static/img/balance_logo/PNG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.212347 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.184347 balance-0.7.0/website/static/img/balance_logo/SVG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/balance_logo/vertical_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/docusaurus.png
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/fontawesome/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/fontawesome/layer-group.svg
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/fontawesome/users.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14679 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/meta_opensource_logo_negative.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:02:05.216347 balance-0.7.0/website/static/img/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/tutorial/docsVersionDropdown.png
--rw-r--r--   0 runner    (1001) docker     (123)    30020 2023-04-10 08:00:29.000000 balance-0.7.0/website/static/img/tutorial/localeDropdown.png
--rw-r--r--   0 runner    (1001) docker     (123)   537599 2023-04-10 08:00:29.000000 balance-0.7.0/website/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.239326 balance-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 13:47:47.000000 balance-0.8.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.195325 balance-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.211325 balance-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 13:47:47.000000 balance-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 13:47:47.000000 balance-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.211325 balance-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-26 13:47:47.000000 balance-0.8.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-26 13:47:47.000000 balance-0.8.0/.github/workflows/deploy-website.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-26 13:47:47.000000 balance-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 13:47:47.000000 balance-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-04-26 13:47:47.000000 balance-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-26 13:47:47.000000 balance-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-26 13:47:47.000000 balance-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-04-26 13:47:47.000000 balance-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-04-26 13:47:47.000000 balance-0.8.0/LICENSE-DOCUMENTATION
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-04-26 13:49:21.239326 balance-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-04-26 13:47:47.000000 balance-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.215325 balance-0.8.0/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-26 13:47:47.000000 balance-0.8.0/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-26 13:47:47.000000 balance-0.8.0/balance/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77711 2023-04-26 13:47:47.000000 balance-0.8.0/balance/balancedf_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26001 2023-04-26 13:47:47.000000 balance-0.8.0/balance/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.219325 balance-0.8.0/balance/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-04-26 13:47:47.000000 balance-0.8.0/balance/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-26 13:47:47.000000 balance-0.8.0/balance/datasets/sim_data_cbps.R
+-rw-r--r--   0 runner    (1001) docker     (123)    55895 2023-04-26 13:47:47.000000 balance-0.8.0/balance/datasets/sim_data_cbps.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    52140 2023-04-26 13:47:47.000000 balance-0.8.0/balance/sample_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.219325 balance-0.8.0/balance/stats_and_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 13:47:47.000000 balance-0.8.0/balance/stats_and_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-26 13:47:47.000000 balance-0.8.0/balance/stats_and_plots/general_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59199 2023-04-26 13:47:47.000000 balance-0.8.0/balance/stats_and_plots/weighted_comparisons_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-26 13:47:47.000000 balance-0.8.0/balance/stats_and_plots/weighted_comparisons_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26952 2023-04-26 13:47:47.000000 balance-0.8.0/balance/stats_and_plots/weighted_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-26 13:47:47.000000 balance-0.8.0/balance/stats_and_plots/weights_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-26 13:47:47.000000 balance-0.8.0/balance/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-26 13:47:47.000000 balance-0.8.0/balance/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78678 2023-04-26 13:47:47.000000 balance-0.8.0/balance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.219325 balance-0.8.0/balance/weighting_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 13:47:47.000000 balance-0.8.0/balance/weighting_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 13:47:47.000000 balance-0.8.0/balance/weighting_methods/adjust_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29249 2023-04-26 13:47:47.000000 balance-0.8.0/balance/weighting_methods/cbps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26591 2023-04-26 13:47:47.000000 balance-0.8.0/balance/weighting_methods/ipw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-26 13:47:47.000000 balance-0.8.0/balance/weighting_methods/poststratify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19388 2023-04-26 13:47:47.000000 balance-0.8.0/balance/weighting_methods/rake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.215325 balance-0.8.0/balance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-04-26 13:49:20.000000 balance-0.8.0/balance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-26 13:49:21.000000 balance-0.8.0/balance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:49:20.000000 balance-0.8.0/balance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-26 13:49:20.000000 balance-0.8.0/balance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 13:49:20.000000 balance-0.8.0/balance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.219325 balance-0.8.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3502 2023-04-26 13:47:47.000000 balance-0.8.0/scripts/make_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:49:21.239326 balance-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-26 13:47:47.000000 balance-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.219325 balance-0.8.0/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.199325 balance-0.8.0/sphinx/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.219325 balance-0.8.0/sphinx/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.199325 balance-0.8.0/sphinx/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.219325 balance-0.8.0/sphinx/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/balance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-26 13:47:47.000000 balance-0.8.0/sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.223326 balance-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_adjust_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43636 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_balancedf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_cbps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40813 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_ipw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_poststratify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18598 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_rake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39150 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32798 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_stats_and_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49276 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-04-26 13:47:47.000000 balance-0.8.0/tests/test_weighted_comparisons_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.223326 balance-0.8.0/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-04-26 13:47:47.000000 balance-0.8.0/tutorials/balance_quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   590295 2023-04-26 13:47:47.000000 balance-0.8.0/tutorials/balance_quickstart_cbps.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-04-26 13:47:47.000000 balance-0.8.0/tutorials/balance_quickstart_rake.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-04-26 13:47:47.000000 balance-0.8.0/tutorials/balance_transformations_and_formulas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-26 13:47:47.000000 balance-0.8.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.227326 balance-0.8.0/website/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 13:47:47.000000 balance-0.8.0/website/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 13:47:47.000000 balance-0.8.0/website/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 13:47:47.000000 balance-0.8.0/website/babel.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.199325 balance-0.8.0/website/blog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.199325 balance-0.8.0/website/blog/2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.199325 balance-0.8.0/website/blog/2023/01/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.227326 balance-0.8.0/website/blog/2023/01/09/
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-26 13:47:47.000000 balance-0.8.0/website/blog/2023/01/09/bringing-balance-to-your-data.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-04-26 13:47:47.000000 balance-0.8.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.203325 balance-0.8.0/website/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.227326 balance-0.8.0/website/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/api_reference/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.227326 balance-0.8.0/website/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.227326 balance-0.8.0/website/docs/docs/general_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/general_framework/adjusting_sample_to_population.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/general_framework/evaluation_of_results.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/general_framework/general_framework.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/docs/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_01_qqplot_income_before.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41572 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_02_barplot_age_before.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38449 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_03_barplot_gender_before.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61834 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_04_qqplot_income_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45979 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_05_barplot_age_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41950 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_06_barplot_gender_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41877 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_07_seaborn_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_08_weights_kde.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28925 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)   468436 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/total_survey_error_flow_v02.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26229 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/total_survey_error_flow_v02.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68569 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/total_survey_error_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/img/total_survey_error_image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/docs/docs/statistical_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/statistical_methods/cbps.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/statistical_methods/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/statistical_methods/ipw.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/statistical_methods/poststratify.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/docs/statistical_methods/rake.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/tutorials/balance_transformations_and_formulas.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/tutorials/index.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/tutorials/quickstart.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/tutorials/quickstart_cbps.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-26 13:47:47.000000 balance-0.8.0/website/docs/tutorials/quickstart_rake.mdx
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-26 13:47:47.000000 balance-0.8.0/website/docusaurus.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 13:47:47.000000 balance-0.8.0/website/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-26 13:47:47.000000 balance-0.8.0/website/sidebars.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.203325 balance-0.8.0/website/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-26 13:47:47.000000 balance-0.8.0/website/src/components/HTMLLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-26 13:47:47.000000 balance-0.8.0/website/src/components/HomepageFeatures.js
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 13:47:47.000000 balance-0.8.0/website/src/components/HomepageFeatures.module.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/src/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 13:47:47.000000 balance-0.8.0/website/src/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/src/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-26 13:47:47.000000 balance-0.8.0/website/src/pages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-26 13:47:47.000000 balance-0.8.0/website/src/pages/index.module.css
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-26 13:47:47.000000 balance-0.8.0/website/src/pages/markdown-page.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/static/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/static/img/balance_logo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.231326 balance-0.8.0/website/static/img/balance_logo/AI/
+-rw-r--r--   0 runner    (1001) docker     (123)   460628 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.203325 balance-0.8.0/website/static/img/balance_logo/PNG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.235326 balance-0.8.0/website/static/img/balance_logo/PNG/Horizontal/
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.235326 balance-0.8.0/website/static/img/balance_logo/PNG/Icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.235326 balance-0.8.0/website/static/img/balance_logo/PNG/Vertical/
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.207325 balance-0.8.0/website/static/img/balance_logo/SVG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.235326 balance-0.8.0/website/static/img/balance_logo/SVG/Horizontal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.235326 balance-0.8.0/website/static/img/balance_logo/SVG/Icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.235326 balance-0.8.0/website/static/img/balance_logo/SVG/Vertical/
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/balance_Social__1280x720.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27958 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/balance_Social__1920x1080.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo/vertical_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.239326 balance-0.8.0/website/static/img/balance_logo_hex_stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo_hex_stickers/balance_hex_fill.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68810 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo_hex_stickers/balance_hex_fill__3x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo_hex_stickers/balance_hex_outline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    88297 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/balance_logo_hex_stickers/balance_hex_outline__3x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/docusaurus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.239326 balance-0.8.0/website/static/img/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/fontawesome/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/fontawesome/layer-group.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/fontawesome/users.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14679 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/meta_opensource_logo_negative.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:49:21.239326 balance-0.8.0/website/static/img/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/tutorial/docsVersionDropdown.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30020 2023-04-26 13:47:47.000000 balance-0.8.0/website/static/img/tutorial/localeDropdown.png
+-rw-r--r--   0 runner    (1001) docker     (123)   537599 2023-04-26 13:47:47.000000 balance-0.8.0/website/yarn.lock
```

### Comparing `balance-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `balance-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `balance-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/.github/workflows/build-and-test.yml` & `balance-0.8.0/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/.github/workflows/deploy-website.yml` & `balance-0.8.0/.github/workflows/deploy-website.yml`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/.github/workflows/release.yml` & `balance-0.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/.gitignore` & `balance-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/CHANGELOG.md` & `balance-0.8.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+0.8.0 (2023-04-26)
+==================
+### New Features
+- Add `rake` method to .adjust (currently in beta, given that it doesn't handles marginal target as input).
+- Add a new function `prepare_marginal_dist_for_raking` - to take in a dict of marginal proportions and turn them into a pandas DataFrame. This can serve as an input target population for raking.
+
+## Misc
+- The `ipw` function now gets max_de=None as default (instead of 1.5). This version is faster, and the user can still choose a threshold as desired.
+- Adding hex stickers graphics files
+
+### Documentation
+- New section on [raking.](https://import-balance.org/docs/docs/statistical_methods/rake/)
+- New notebook (in the tutorial section):
+    - [**quickstart_rake**](https://import-balance.org/docs/tutorials/quickstart_rake/) - like the [**quickstart**](https://import-balance.org/docs/tutorials/quickstart/) tutorial, but shows how to use the rake (raking) algorithm and compares the results to IPW (logistic regression with LASSO).
+
+
 0.7.0 (2023-04-10)
 ==================
 ### New Features
 - Add `plotly_plot_density` function: Plots interactive density plots of the given variables using kernel density estimation.
 - Modified `plotly_plot_dist` and `plot_dist` to also support 'kde' plots. Also, these are now the default options. This automatically percolates to `BalanceDF.plot()` methods.
 - `Sample.from_frame` can now guess that a column called "weights" is a weight column (instead of only guessing so if the column is called "weight").
```

### Comparing `balance-0.7.0/CODE_OF_CONDUCT.md` & `balance-0.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/CONTRIBUTING.md` & `balance-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/LICENSE` & `balance-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/LICENSE-DOCUMENTATION` & `balance-0.8.0/LICENSE-DOCUMENTATION`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/PKG-INFO` & `balance-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balance
-Version: 0.7.0
+Version: 0.8.0
 Summary: balance is a Python package offering a simple workflow and methods for dealing with biased data samples when looking to infer from them to some target population of interest.
 Home-page: https://github.com/facebookresearch/balance
 Author: Facebook, Inc.
 License: GPLv2
 Description: [![balance_logo_horizontal](https://raw.githubusercontent.com/facebookresearch/balance/main/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png)](https://import-balance.org/)
         
         
@@ -128,15 +128,15 @@
         
         *You can read more on evaluation of the pre-adjusted data in the [Pre-Adjustment Diagnostics](https://import-balance.org/docs/docs/general_framework/pre_adjustment_diagnostics/) page.*
         
         Next, we adjust the sample to the population by fitting balancing survey weights:
         
         ```python
         # Using ipw to fit survey weights
-        adjusted = sample_with_target.adjust(max_de=None)
+        adjusted = sample_with_target.adjust()
         ```
         
         *You can read more on adjustment process in the [Adjusting Sample to Population](https://import-balance.org/docs/docs/general_framework/adjusting_sample_to_population/) page.*
         
         The above code gets us an `adjusted` object with weights. We can evaluate the benefit of the weights to the covariate balance, for example by running:
         
         ```python
@@ -177,24 +177,25 @@
         
         Finally, the adjusted data can be downloaded using:
         ```python
         adjusted.to_download()  # Or:
         # adjusted.to_csv()
         ```
         
-        To see a more detailed step-by-step code example with code output prints and plots (both static and interactive), please go over to the [quickstart tutorial](https://import-balance.org/docs/tutorials/quickstart/).
+        To see a more detailed step-by-step code example with code output prints and plots (both static and interactive), please go over to the [tutorials section](https://import-balance.org/docs/tutorials/).
         
         
         ## Implemented methods for adjustments
         
         *balance* currently implements various adjustment methods. Click the links to learn more about each:
         
         1. [Logistic regression using L1 (LASSO) penalization.](https://import-balance.org/docs/docs/statistical_methods/ipw/)
         2. [Covariate Balancing Propensity Score (CBPS).](https://import-balance.org/docs/docs/statistical_methods/cbps/)
         3. [Post-stratification.](https://import-balance.org/docs/docs/statistical_methods/poststratify/)
+        4. [Raking.](https://import-balance.org/docs/docs/statistical_methods/rake/)
         
         ## Implemented methods for diagnostics/evaluation
         
         For diagnostics the main tools (comparing before, after applying weights, and the target population) are:
         
         1. Plots
             1. barplots
@@ -237,15 +238,15 @@
         
         The *balance* package is actively maintained by people from the [Core Data Science](https://research.facebook.com/teams/core-data-science/) team (in Tel Aviv and Boston), by [Tal Sarig](https://research.facebook.com/people/sarig-tal/), [Tal Galili](https://research.facebook.com/people/galili-tal/) and [Steve Mandala](https://research.facebook.com/people/mandala-steve/).
         
         The *balance* package was (and is) developed by many people, including: [Roee Eilat](https://research.facebook.com/people/eilat-roee/), [Tal Galili](https://research.facebook.com/people/galili-tal/), [Daniel Haimovich](https://research.facebook.com/people/haimovich-daniel/), [Kevin Liou](https://www.linkedin.com/in/kevinycliou), [Steve Mandala](https://research.facebook.com/people/mandala-steve/), [Adam Obeng](https://adamobeng.com/) (author of the initial internal Meta version), [Tal Sarig](https://research.facebook.com/people/sarig-tal/),  [Luke Sonnet](https://www.linkedin.com/in/luke-sonnet), [Sean Taylor](https://seanjtaylor.com), [Barak Yair Reif](https://www.linkedin.com/in/barak-yair-reif-2154365/), and others. If you worked on balance in the past, please email us to be added to this list.
         
         The *balance* package was open-sourced by [Tal Sarig](https://research.facebook.com/people/sarig-tal/), [Tal Galili](https://research.facebook.com/people/galili-tal/) and [Steve Mandala](https://research.facebook.com/people/mandala-steve/) in late 2022.
         
-        Branding created by [Dana Beaty](https://www.danabeaty.com/), from the Meta AI Design and Marketing Team.
+        Branding created by [Dana Beaty](https://www.danabeaty.com/), from the Meta AI Design and Marketing Team. For logo files, see [here](https://github.com/facebookresearch/balance/tree/main/website/static/img/).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balance-0.7.0/README.md` & `balance-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 *You can read more on evaluation of the pre-adjusted data in the [Pre-Adjustment Diagnostics](https://import-balance.org/docs/docs/general_framework/pre_adjustment_diagnostics/) page.*
 
 Next, we adjust the sample to the population by fitting balancing survey weights:
 
 ```python
 # Using ipw to fit survey weights
-adjusted = sample_with_target.adjust(max_de=None)
+adjusted = sample_with_target.adjust()
 ```
 
 *You can read more on adjustment process in the [Adjusting Sample to Population](https://import-balance.org/docs/docs/general_framework/adjusting_sample_to_population/) page.*
 
 The above code gets us an `adjusted` object with weights. We can evaluate the benefit of the weights to the covariate balance, for example by running:
 
 ```python
@@ -170,24 +170,25 @@
 
 Finally, the adjusted data can be downloaded using:
 ```python
 adjusted.to_download()  # Or:
 # adjusted.to_csv()
 ```
 
-To see a more detailed step-by-step code example with code output prints and plots (both static and interactive), please go over to the [quickstart tutorial](https://import-balance.org/docs/tutorials/quickstart/).
+To see a more detailed step-by-step code example with code output prints and plots (both static and interactive), please go over to the [tutorials section](https://import-balance.org/docs/tutorials/).
 
 
 ## Implemented methods for adjustments
 
 *balance* currently implements various adjustment methods. Click the links to learn more about each:
 
 1. [Logistic regression using L1 (LASSO) penalization.](https://import-balance.org/docs/docs/statistical_methods/ipw/)
 2. [Covariate Balancing Propensity Score (CBPS).](https://import-balance.org/docs/docs/statistical_methods/cbps/)
 3. [Post-stratification.](https://import-balance.org/docs/docs/statistical_methods/poststratify/)
+4. [Raking.](https://import-balance.org/docs/docs/statistical_methods/rake/)
 
 ## Implemented methods for diagnostics/evaluation
 
 For diagnostics the main tools (comparing before, after applying weights, and the target population) are:
 
 1. Plots
     1. barplots
@@ -230,8 +231,8 @@
 
 The *balance* package is actively maintained by people from the [Core Data Science](https://research.facebook.com/teams/core-data-science/) team (in Tel Aviv and Boston), by [Tal Sarig](https://research.facebook.com/people/sarig-tal/), [Tal Galili](https://research.facebook.com/people/galili-tal/) and [Steve Mandala](https://research.facebook.com/people/mandala-steve/).
 
 The *balance* package was (and is) developed by many people, including: [Roee Eilat](https://research.facebook.com/people/eilat-roee/), [Tal Galili](https://research.facebook.com/people/galili-tal/), [Daniel Haimovich](https://research.facebook.com/people/haimovich-daniel/), [Kevin Liou](https://www.linkedin.com/in/kevinycliou), [Steve Mandala](https://research.facebook.com/people/mandala-steve/), [Adam Obeng](https://adamobeng.com/) (author of the initial internal Meta version), [Tal Sarig](https://research.facebook.com/people/sarig-tal/),  [Luke Sonnet](https://www.linkedin.com/in/luke-sonnet), [Sean Taylor](https://seanjtaylor.com), [Barak Yair Reif](https://www.linkedin.com/in/barak-yair-reif-2154365/), and others. If you worked on balance in the past, please email us to be added to this list.
 
 The *balance* package was open-sourced by [Tal Sarig](https://research.facebook.com/people/sarig-tal/), [Tal Galili](https://research.facebook.com/people/galili-tal/) and [Steve Mandala](https://research.facebook.com/people/mandala-steve/) in late 2022.
 
-Branding created by [Dana Beaty](https://www.danabeaty.com/), from the Meta AI Design and Marketing Team.
+Branding created by [Dana Beaty](https://www.danabeaty.com/), from the Meta AI Design and Marketing Team. For logo files, see [here](https://github.com/facebookresearch/balance/tree/main/website/static/img/).
```

### Comparing `balance-0.7.0/balance/__init__.py` & `balance-0.8.0/balance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from balance.sample_class import Sample  # noqa
 from balance.util import TruncationFormatter  # noqa
 
 # TODO: which objects do we want to explicitly externalize?
 # TODO: verify this works.
 
 global __version__
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 
 def setup_logging(
     logger_name: Optional[str] = __package__,
     level: str = "INFO",
     removeHandler: bool = True,
 ) -> logging.Logger:
```

### Comparing `balance-0.7.0/balance/adjustment.py` & `balance-0.8.0/balance/adjustment.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 
 from balance import util as balance_util
 from balance.weighting_methods import (
     adjust_null as balance_adjust_null,
     cbps as balance_cbps,
     ipw as balance_ipw,
     poststratify as balance_poststratify,
+    rake as balance_rake,
 )
 from pandas.api.types import is_bool_dtype, is_numeric_dtype
 
 logger: logging.Logger = logging.getLogger(__package__)
 
 
 BALANCE_WEIGHTING_METHODS = {
     "ipw": balance_ipw.ipw,
     "cbps": balance_cbps.cbps,
     "null": balance_adjust_null.adjust_null,
     "poststratify": balance_poststratify.poststratify,
+    "rake": balance_rake.rake,
 }
 
 
 def trim_weights(
     weights: Union[pd.Series, np.ndarray],
     # TODO: add support to more types of input weights? (e.g. list? other?)
     weight_trimming_mean_ratio: Union[float, int, None] = None,
@@ -303,21 +305,21 @@
     res = tuple(out[i:j] for (i, j) in boundaries)
     res = tuple(x.set_index(i) for x, i in zip(res, indices))
 
     return res
 
 
 def _find_adjustment_method(
-    method: Literal["cbps", "ipw", "null", "poststratify"],
+    method: Literal["cbps", "ipw", "null", "poststratify", "rake"],
     WEIGHTING_METHODS: Dict[str, Callable] = BALANCE_WEIGHTING_METHODS,
 ) -> Callable:
     """This function translates a string method argument to the function itself.
 
     Args:
-        method (Literal["cbps", "ipw", "null", "poststratify"]): method for adjustment: cbps, ipw, null, poststratify
+        method (Literal["cbps", "ipw", "null", "poststratify", "rake"]): method for adjustment: cbps, ipw, null, poststratify
         WEIGHTING_METHODS (Dict[str, Callable]): A dict where keys are strings of function names, and the values are
             the functions themselves.
 
     Returns:
         Callable: The function for adjustment
     """
     if method in WEIGHTING_METHODS.keys():
```

### Comparing `balance-0.7.0/balance/balancedf_class.py` & `balance-0.8.0/balance/balancedf_class.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/cli.py` & `balance-0.8.0/balance/cli.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/datasets/__init__.py` & `balance-0.8.0/balance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/datasets/sim_data_cbps.R` & `balance-0.8.0/balance/datasets/sim_data_cbps.R`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/datasets/sim_data_cbps.csv` & `balance-0.8.0/balance/datasets/sim_data_cbps.csv`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/sample_class.py` & `balance-0.8.0/balance/sample_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,26 +392,28 @@
 
     ############################################
     # Adjusting and adapting weights of a sample
     ############################################
     def adjust(
         self: "Sample",
         target: Optional["Sample"] = None,
-        method: Union[Literal["cbps", "ipw", "null", "poststratify"], Callable] = "ipw",
+        method: Union[
+            Literal["cbps", "ipw", "null", "poststratify", "rake"], Callable
+        ] = "ipw",
         *args,
         **kwargs,
     ) -> "Sample":
         """
         Perform adjustment of one sample to match another.
         This function returns a new sample.
 
         Args:
             target (Optional["Sample"]): Second sample object which should be matched.
                 If None, the set target of the object is used for matching.
-            method (str): method for adjustment: cbps, ipw, null, poststratify
+            method (str): method for adjustment: cbps, ipw, null, poststratify, rake
 
         Returns:
             Sample: an adjusted Sample object
         """
         if target is None:
             self._no_target_error()
             target = self._links["target"]
```

### Comparing `balance-0.7.0/balance/stats_and_plots/general_stats.py` & `balance-0.8.0/balance/stats_and_plots/general_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/stats_and_plots/weighted_comparisons_plots.py` & `balance-0.8.0/balance/stats_and_plots/weighted_comparisons_plots.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/stats_and_plots/weighted_comparisons_stats.py` & `balance-0.8.0/balance/stats_and_plots/weighted_comparisons_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/stats_and_plots/weighted_stats.py` & `balance-0.8.0/balance/stats_and_plots/weighted_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/stats_and_plots/weights_stats.py` & `balance-0.8.0/balance/stats_and_plots/weights_stats.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/testutil.py` & `balance-0.8.0/balance/testutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         yield sys.stdout, sys.stderr
     finally:
         sys.stdout, sys.stderr = original_out, original_err
 
 
 class BalanceTestCase(unittest.TestCase):
     # Some Warns
-    def assertWarns(self, callable, *args, **kwargs) -> None:
+    def assertIfWarns(self, callable, *args, **kwargs) -> None:
         with self.assertLogs(level="NOTSET") as cm:
             callable(*args, **kwargs)
             self.assertTrue(len(cm.output) > 0, "No warning produced.")
 
     def assertNotWarns(self, callable, *args, **kwargs) -> None:
         output = None
         try:
```

### Comparing `balance-0.7.0/balance/util.py` & `balance-0.8.0/balance/util.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/weighting_methods/adjust_null.py` & `balance-0.8.0/balance/weighting_methods/adjust_null.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/weighting_methods/cbps.py` & `balance-0.8.0/balance/weighting_methods/cbps.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance/weighting_methods/ipw.py` & `balance-0.8.0/balance/weighting_methods/ipw.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
         keep_sum_of_weights=keep_sum_of_weights,
     )
     # Normalize weights such that the sum will be the sum of the weights of target
     weights = weights * np.sum(target_weights) / np.sum(weights)
     return weights
 
 
+# TODO: Update choose_regularization function to be based on mse (instead of grid search)
 def choose_regularization(
     fit,
     sample_df: pd.DataFrame,
     target_df: pd.DataFrame,
     sample_weights: pd.Series,
     target_weights: pd.Series,
     X_matrix_sample,
@@ -344,16 +345,15 @@
     variables: Optional[List[str]] = None,
     model: str = "glmnet",
     weight_trimming_mean_ratio: Optional[Union[int, float]] = 20,
     weight_trimming_percentile: Optional[float] = None,
     balance_classes: bool = True,
     transformations: str = "default",
     na_action: str = "add_indicator",
-    # TODO: set max_de to None as default
-    max_de: Optional[float] = 1.5,
+    max_de: Optional[float] = None,
     formula: Union[str, List[str], None] = None,
     penalty_factor: Optional[List[float]] = None,
     one_hot_encoding: bool = False,
     # TODO: This is set to be false in order to keep reproducibility of works that uses balance.
     # The best practice is for this to be true.
     random_seed: int = 2020,
     *args,
@@ -557,14 +557,15 @@
         raise NotImplementedError()
     logger.debug(f"fit['lambda_1se']: {fit['lambda_1se']}")
 
     X_matrix_sample = X_matrix[
         :sample_n,
     ].toarray()
 
+    logger.info(f"max_de: {max_de}")
     if max_de is not None:
         regularisation_perf = choose_regularization(
             fit,
             sample_df,
             target_df,
             sample_weights,
             target_weights,
```

### Comparing `balance-0.7.0/balance/weighting_methods/poststratify.py` & `balance-0.8.0/balance/weighting_methods/poststratify.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/balance.egg-info/PKG-INFO` & `balance-0.8.0/balance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balance
-Version: 0.7.0
+Version: 0.8.0
 Summary: balance is a Python package offering a simple workflow and methods for dealing with biased data samples when looking to infer from them to some target population of interest.
 Home-page: https://github.com/facebookresearch/balance
 Author: Facebook, Inc.
 License: GPLv2
 Description: [![balance_logo_horizontal](https://raw.githubusercontent.com/facebookresearch/balance/main/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png)](https://import-balance.org/)
         
         
@@ -128,15 +128,15 @@
         
         *You can read more on evaluation of the pre-adjusted data in the [Pre-Adjustment Diagnostics](https://import-balance.org/docs/docs/general_framework/pre_adjustment_diagnostics/) page.*
         
         Next, we adjust the sample to the population by fitting balancing survey weights:
         
         ```python
         # Using ipw to fit survey weights
-        adjusted = sample_with_target.adjust(max_de=None)
+        adjusted = sample_with_target.adjust()
         ```
         
         *You can read more on adjustment process in the [Adjusting Sample to Population](https://import-balance.org/docs/docs/general_framework/adjusting_sample_to_population/) page.*
         
         The above code gets us an `adjusted` object with weights. We can evaluate the benefit of the weights to the covariate balance, for example by running:
         
         ```python
@@ -177,24 +177,25 @@
         
         Finally, the adjusted data can be downloaded using:
         ```python
         adjusted.to_download()  # Or:
         # adjusted.to_csv()
         ```
         
-        To see a more detailed step-by-step code example with code output prints and plots (both static and interactive), please go over to the [quickstart tutorial](https://import-balance.org/docs/tutorials/quickstart/).
+        To see a more detailed step-by-step code example with code output prints and plots (both static and interactive), please go over to the [tutorials section](https://import-balance.org/docs/tutorials/).
         
         
         ## Implemented methods for adjustments
         
         *balance* currently implements various adjustment methods. Click the links to learn more about each:
         
         1. [Logistic regression using L1 (LASSO) penalization.](https://import-balance.org/docs/docs/statistical_methods/ipw/)
         2. [Covariate Balancing Propensity Score (CBPS).](https://import-balance.org/docs/docs/statistical_methods/cbps/)
         3. [Post-stratification.](https://import-balance.org/docs/docs/statistical_methods/poststratify/)
+        4. [Raking.](https://import-balance.org/docs/docs/statistical_methods/rake/)
         
         ## Implemented methods for diagnostics/evaluation
         
         For diagnostics the main tools (comparing before, after applying weights, and the target population) are:
         
         1. Plots
             1. barplots
@@ -237,15 +238,15 @@
         
         The *balance* package is actively maintained by people from the [Core Data Science](https://research.facebook.com/teams/core-data-science/) team (in Tel Aviv and Boston), by [Tal Sarig](https://research.facebook.com/people/sarig-tal/), [Tal Galili](https://research.facebook.com/people/galili-tal/) and [Steve Mandala](https://research.facebook.com/people/mandala-steve/).
         
         The *balance* package was (and is) developed by many people, including: [Roee Eilat](https://research.facebook.com/people/eilat-roee/), [Tal Galili](https://research.facebook.com/people/galili-tal/), [Daniel Haimovich](https://research.facebook.com/people/haimovich-daniel/), [Kevin Liou](https://www.linkedin.com/in/kevinycliou), [Steve Mandala](https://research.facebook.com/people/mandala-steve/), [Adam Obeng](https://adamobeng.com/) (author of the initial internal Meta version), [Tal Sarig](https://research.facebook.com/people/sarig-tal/),  [Luke Sonnet](https://www.linkedin.com/in/luke-sonnet), [Sean Taylor](https://seanjtaylor.com), [Barak Yair Reif](https://www.linkedin.com/in/barak-yair-reif-2154365/), and others. If you worked on balance in the past, please email us to be added to this list.
         
         The *balance* package was open-sourced by [Tal Sarig](https://research.facebook.com/people/sarig-tal/), [Tal Galili](https://research.facebook.com/people/galili-tal/) and [Steve Mandala](https://research.facebook.com/people/mandala-steve/) in late 2022.
         
-        Branding created by [Dana Beaty](https://www.danabeaty.com/), from the Meta AI Design and Marketing Team.
+        Branding created by [Dana Beaty](https://www.danabeaty.com/), from the Meta AI Design and Marketing Team. For logo files, see [here](https://github.com/facebookresearch/balance/tree/main/website/static/img/).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balance-0.7.0/balance.egg-info/SOURCES.txt` & `balance-0.8.0/balance.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 balance/stats_and_plots/weighted_stats.py
 balance/stats_and_plots/weights_stats.py
 balance/weighting_methods/__init__.py
 balance/weighting_methods/adjust_null.py
 balance/weighting_methods/cbps.py
 balance/weighting_methods/ipw.py
 balance/weighting_methods/poststratify.py
+balance/weighting_methods/rake.py
 scripts/make_docs.sh
 sphinx/Makefile
 sphinx/balance.rst
 sphinx/conf.py
 sphinx/index.rst
 sphinx/make.bat
 sphinx/_static/css/custom.css
@@ -53,21 +54,23 @@
 tests/test_balancedf.py
 tests/test_cbps.py
 tests/test_cli.py
 tests/test_datasets.py
 tests/test_ipw.py
 tests/test_logging.py
 tests/test_poststratify.py
+tests/test_rake.py
 tests/test_sample.py
 tests/test_stats_and_plots.py
 tests/test_testutil.py
 tests/test_util.py
 tests/test_weighted_comparisons_plots.py
 tutorials/balance_quickstart.ipynb
 tutorials/balance_quickstart_cbps.ipynb
+tutorials/balance_quickstart_rake.ipynb
 tutorials/balance_transformations_and_formulas.ipynb
 tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb
 website/.npmrc
 website/README.md
 website/babel.config.js
 website/docusaurus.config.js
 website/package.json
@@ -95,32 +98,36 @@
 website/docs/docs/img/total_survey_error_flow_v02.svg
 website/docs/docs/img/total_survey_error_image.png
 website/docs/docs/img/total_survey_error_image.svg
 website/docs/docs/statistical_methods/cbps.md
 website/docs/docs/statistical_methods/index.md
 website/docs/docs/statistical_methods/ipw.md
 website/docs/docs/statistical_methods/poststratify.md
+website/docs/docs/statistical_methods/rake.md
 website/docs/tutorials/balance_transformations_and_formulas.mdx
 website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx
 website/docs/tutorials/index.mdx
 website/docs/tutorials/quickstart.mdx
 website/docs/tutorials/quickstart_cbps.mdx
+website/docs/tutorials/quickstart_rake.mdx
 website/src/components/HTMLLoader.js
 website/src/components/HomepageFeatures.js
 website/src/components/HomepageFeatures.module.css
 website/src/css/custom.css
 website/src/pages/index.js
 website/src/pages/index.module.css
 website/src/pages/markdown-page.md
 website/static/.nojekyll
 website/static/CNAME
 website/static/img/docusaurus.png
 website/static/img/favicon.ico
 website/static/img/logo.svg
 website/static/img/meta_opensource_logo_negative.svg
+website/static/img/balance_logo/balance_Social__1280x720.png
+website/static/img/balance_logo/balance_Social__1920x1080.png
 website/static/img/balance_logo/icon.png
 website/static/img/balance_logo/icon.svg
 website/static/img/balance_logo/vertical.svg
 website/static/img/balance_logo/vertical_white.svg
 website/static/img/balance_logo/AI/balance_Logo_FINAL.ai
 website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png
 website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png
@@ -136,12 +143,16 @@
 website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg
 website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg
 website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg
 website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg
 website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg
 website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg
 website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg
+website/static/img/balance_logo_hex_stickers/balance_hex_fill.svg
+website/static/img/balance_logo_hex_stickers/balance_hex_fill__3x.png
+website/static/img/balance_logo_hex_stickers/balance_hex_outline.svg
+website/static/img/balance_logo_hex_stickers/balance_hex_outline__3x.png
 website/static/img/fontawesome/code.svg
 website/static/img/fontawesome/layer-group.svg
 website/static/img/fontawesome/users.svg
 website/static/img/tutorial/docsVersionDropdown.png
 website/static/img/tutorial/localeDropdown.png
```

### Comparing `balance-0.7.0/scripts/make_docs.sh` & `balance-0.8.0/scripts/make_docs.sh`

 * *Files 11% similar despite different names*

```diff
@@ -75,14 +75,16 @@
   echo "-----------------------------------"
   echo "Building tutorial HTML"
   echo "-----------------------------------"
   jupyter nbconvert tutorials/balance_quickstart.ipynb --execute --to html \
     --output-dir website/static/html/tutorials
   jupyter nbconvert tutorials/balance_quickstart_cbps.ipynb --execute --to html \
     --output-dir website/static/html/tutorials
+  jupyter nbconvert tutorials/balance_quickstart_rake.ipynb --execute --to html \
+    --output-dir website/static/html/tutorials
   jupyter nbconvert tutorials/balance_transformations_and_formulas.ipynb --execute --to html \
     --output-dir website/static/html/tutorials
   jupyter nbconvert tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb --execute --to html \
     --output-dir website/static/html/tutorials
 fi
 
 echo "-----------------------------------"
```

### Comparing `balance-0.7.0/setup.py` & `balance-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/sphinx/Makefile` & `balance-0.8.0/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/sphinx/_templates/autosummary/class.rst` & `balance-0.8.0/sphinx/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/sphinx/conf.py` & `balance-0.8.0/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/sphinx/make.bat` & `balance-0.8.0/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_adjust_null.py` & `balance-0.8.0/tests/test_adjust_null.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_adjustment.py` & `balance-0.8.0/tests/test_adjustment.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_balancedf.py` & `balance-0.8.0/tests/test_balancedf.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,15 +961,15 @@
         # d = d.assign(a=lambda x: pd.cut(x.a,[0,.25,.5,.75,1]))
         d["a"] = pd.cut(d["a"], [0, 0.25, 0.5, 0.75, 1]).astype(str)
         t = Sample.from_frame(d)
 
         st = s.set_target(t)
 
         # Fit IPW
-        a = st.adjust()
+        a = st.adjust(max_de=1.5)
 
         # Check ASMD
         tmp_asmd_default = a.covars().asmd()
         tmp_asmd_main_covar = a.covars().asmd(aggregate_by_main_covar=True)
 
         outcome_default = tmp_asmd_default.round(2).to_dict()
         outcome_main_covar = tmp_asmd_main_covar.round(2).to_dict()
```

### Comparing `balance-0.7.0/tests/test_cbps.py` & `balance-0.8.0/tests/test_cbps.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_cli.py` & `balance-0.8.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -593,14 +593,15 @@
                     "--output_file",
                     output_file,
                     "--diagnostics_output_file",
                     diagnostics_output_file,
                     "--covariate_columns",
                     features,
                     "--method=ipw",
+                    "--max_de=1.5",
                 ]
             )
             # run cli
             cli = BalanceCLI(args)
             cli.update_attributes_for_main_used_by_adjust()
             cli.main()
             # get the files created from cli to pandas to check them
@@ -608,14 +609,75 @@
             self.assertEqual(
                 diagnostics_output[diagnostics_output["metric"] == "adjustment_method"][
                     "var"
                 ].values,
                 np.array(["ipw"]),
             )
 
+    def test_method_works_with_rake(self):
+        # TODO: ideally we'll have the example outside, and a different function for each of the methods (ipw, cbps, raking)
+        np.random.seed(2021)
+        n_sample = 1000
+        n_target = 2000
+        sample_df = pd.DataFrame(
+            {
+                "age": np.random.uniform(0, 100, n_sample),
+                "gender": np.random.choice((1, 2, 3, 4), n_sample),
+                "id": range(n_sample),
+                "weight": pd.Series((1,) * n_sample),
+            }
+        )
+        sample_df["is_respondent"] = True
+        target_df = pd.DataFrame(
+            {
+                "age": np.random.uniform(0, 100, n_target),
+                "gender": np.random.choice((1, 2, 3, 4), n_target),
+                "id": range(n_target),
+                "weight": pd.Series((1,) * n_target),
+            }
+        )
+        target_df["is_respondent"] = False
+        input_dataset = pd.concat([sample_df, target_df])
+
+        with tempfile.TemporaryDirectory() as temp_dir, tempfile.NamedTemporaryFile(
+            "w", suffix=".csv", delete=False
+        ) as input_file:
+            input_dataset.to_csv(path_or_buf=input_file)
+            input_file.close()
+            output_file = os.path.join(temp_dir, "weights_out.csv")
+            diagnostics_output_file = os.path.join(temp_dir, "diagnostics_out.csv")
+            features = "age,gender"
+
+            parser = make_parser()
+            args = parser.parse_args(
+                [
+                    "--input_file",
+                    input_file.name,
+                    "--output_file",
+                    output_file,
+                    "--diagnostics_output_file",
+                    diagnostics_output_file,
+                    "--covariate_columns",
+                    features,
+                    "--method=rake",
+                ]
+            )
+            # run cli
+            cli = BalanceCLI(args)
+            cli.update_attributes_for_main_used_by_adjust()
+            cli.main()
+            # get the files created from cli to pandas to check them
+            diagnostics_output = pd.read_csv(diagnostics_output_file, sep=",")
+            self.assertEqual(
+                diagnostics_output[diagnostics_output["metric"] == "adjustment_method"][
+                    "var"
+                ].values,
+                np.array(["rake"]),
+            )
+
     def test_one_hot_encoding_works(self):
         with tempfile.TemporaryDirectory() as temp_dir, tempfile.NamedTemporaryFile(
             "w", suffix=".tsv", delete=False
         ) as in_file:
 
             # Assert value is False when "False" is passed
             out_file = os.path.join(temp_dir, "out.csv")
```

### Comparing `balance-0.7.0/tests/test_datasets.py` & `balance-0.8.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_ipw.py` & `balance-0.8.0/tests/test_ipw.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
         result = balance_ipw.ipw(
             sample_df=sample,
             sample_weights=pd.Series((1,) * 9),
             target_df=target,
             target_weights=pd.Series((1,) * 9),
             transformations=None,
+            max_de=1.5,
         )
 
         w = result["weight"].values
 
         self.assertEqual(w[0], w[8])
         self.assertTrue(w[0] < w[1])
         self.assertTrue(w[0] < w[7])
@@ -359,15 +360,17 @@
             axis=1,
         )
         target_df = target_df.rename(columns={i: "abcdefghij"[i] for i in range(0, 10)})
 
         sample_weights = pd.Series(np.random.uniform(0, 1, size=n_sample))
         target_weights = pd.Series(np.random.uniform(0, 1, size=n_target))
 
-        res = balance_ipw.ipw(sample_df, sample_weights, target_df, target_weights)
+        res = balance_ipw.ipw(
+            sample_df, sample_weights, target_df, target_weights, max_de=1.5
+        )
 
         # Compare output weights (examples and distribution)
         self.assertEqual(round(res["weight"][15], 4), 0.0886)
         self.assertEqual(round(res["weight"][995], 4), 0.2363)
         self.assertEqual(
             np.around(res["weight"].describe().values, 4),
             np.array([1000, 1.0167, 0.7108, 0.0001, 0.2349, 1.2151, 1.7077, 1.7077]),
```

### Comparing `balance-0.7.0/tests/test_logging.py` & `balance-0.8.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_poststratify.py` & `balance-0.8.0/tests/test_poststratify.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_sample.py` & `balance-0.8.0/tests/test_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,15 +501,15 @@
 
         d = pd.DataFrame(np.random.rand(1000, 11))
         d["id"] = range(0, d.shape[0])
         d = d.rename(columns={i: "abcdefghijk"[i] for i in range(0, 11)})
         d["b"] = np.sqrt(d["b"])
 
         a_with_outcome = Sample.from_frame(d, outcome_columns=["k"])
-        a_with_outcome_adjusted = a_with_outcome.adjust(t)
+        a_with_outcome_adjusted = a_with_outcome.adjust(t, max_de=1.5)
 
         # verifying this does what we expact it does:
         self.assertEqual(
             round(a_with_outcome_adjusted.outcome_variance_ratio()[0], 5),
             round(
                 (
                     weighted_var(
@@ -682,15 +682,15 @@
         s = Sample.from_frame(d)
 
         d = pd.DataFrame(np.random.rand(1000, 10))
         d["id"] = range(0, d.shape[0])
         d = d.rename(columns={i: "abcdefghij"[i] for i in range(0, 10)})
         t = Sample.from_frame(d)
 
-        a = s.adjust(t)
+        a = s.adjust(t, max_de=1.5)
 
         # if both rows_to_keep = None, columns_to_keep = None - then keep_only_some_rows_columns returns the same object
         self.assertTrue(
             a is a.keep_only_some_rows_columns(rows_to_keep=None, columns_to_keep=None)
         )
 
         # let's remove some columns and rows:
@@ -809,15 +809,15 @@
         np.random.seed(112358)
 
         d = pd.DataFrame(np.random.rand(1000, 11))
         d["id"] = range(0, d.shape[0])
         d = d.rename(columns={i: "abcdefghijk"[i] for i in range(0, 11)})
         d["b"] = np.sqrt(d["b"])
         a_with_outcome = Sample.from_frame(d, outcome_columns=["k"])
-        a_with_outcome_adjusted = a_with_outcome.adjust(t)
+        a_with_outcome_adjusted = a_with_outcome.adjust(t, max_de=1.5)
 
         # We can also filter using an outcome variable (althought this would NOT filter on target)
         # a proper logger warning is issued
         self.assertEqual(
             a_with_outcome_adjusted.keep_only_some_rows_columns(
                 rows_to_keep="k>0.5"
             ).df.shape,
```

### Comparing `balance-0.7.0/tests/test_stats_and_plots.py` & `balance-0.8.0/tests/test_stats_and_plots.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_testutil.py` & `balance-0.8.0/tests/test_testutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 class TestTestUtil_BalanceTestCase_Warns(
     balance.testutil.BalanceTestCase,
 ):
     def test_unit_test_warning_mixin(self):
         logger = logging.getLogger(__package__)
 
-        self.assertWarns(lambda: logger.warning("test"))
+        self.assertIfWarns(lambda: logger.warning("test"))
         self.assertNotWarns(lambda: "x")
 
         self.assertWarnsRegexp("abc", lambda: logger.warning("abcde"))
         self.assertRaises(
             AssertionError,
             self.assertWarnsRegexp,
             "abcdef",
```

### Comparing `balance-0.7.0/tests/test_util.py` & `balance-0.8.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tests/test_weighted_comparisons_plots.py` & `balance-0.8.0/tests/test_weighted_comparisons_plots.py`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/tutorials/balance_quickstart.ipynb` & `balance-0.8.0/tutorials/balance_quickstart.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998511904761904%*

 * *Differences: {"'cells'": "{30: {'source': {insert: [(1, 'adjusted = sample_with_target.adjust()')], delete: "*

 * *            '[1]}}}'}*

```diff
@@ -454,15 +454,15 @@
                 "originalKey": "8fa4914c-2064-4021-8b2b-9e15fccaae71",
                 "requestMsgId": "b51693a1-e63a-4481-b932-49282c1ab185",
                 "showInput": true
             },
             "outputs": [],
             "source": [
                 "# Using ipw to fit survey weights\n",
-                "adjusted = sample_with_target.adjust(max_de=None)"
+                "adjusted = sample_with_target.adjust()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "customInput": null,
```

### Comparing `balance-0.7.0/tutorials/balance_quickstart_cbps.ipynb` & `balance-0.8.0/tutorials/balance_quickstart_cbps.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998611111111111%*

 * *Differences: {"'cells'": "{30: {'source': {insert: [(1, 'adjusted_ipw = sample_with_target.adjust()')], delete: "*

 * *            '[1]}}}'}*

```diff
@@ -7378,15 +7378,15 @@
                     "text": [
                         "INFO (2022-11-22 02:23:03,091) [ipw/ipw (line 581)]: Proportion null deviance explained [0.17374302]\n"
                     ]
                 }
             ],
             "source": [
                 "# Using ipw to fit survey weights\n",
-                "adjusted_ipw = sample_with_target.adjust(max_de=None)"
+                "adjusted_ipw = sample_with_target.adjust()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
                 "collapsed": false,
```

### Comparing `balance-0.7.0/tutorials/balance_transformations_and_formulas.ipynb` & `balance-0.8.0/tutorials/balance_transformations_and_formulas.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994451334098073%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(5, '    # max_de=None,\\n')], delete: [5]}}, 7: {'source': "*

 * *            "{insert: [(5, '    # max_de=None,\\n')], delete: [5]}}, 9: {'source': {insert: [(13, "*

 * *            "'    # max_de=None,\\n')], delete: [13]}}, 11: {'source': {insert: [(11, '    # "*

 * *            "max_de=None,\\n')], delete: [11]}}, 15: {'source': {insert: [(15, '    # "*

 * *            "max_de=None,\\n')], delete: [15]}}, 17: {'source': {insert: [(16, '    # "*

 * *            "max_de=None,\\n')], delete:  […]*

```diff
@@ -93,15 +93,15 @@
             "outputs": [],
             "source": [
                 "adjusted = sample_with_target.adjust(\n",
                 "    # method=\"ipw\", # default method\n",
                 "    # transformations=None,\n",
                 "    # formula=None,\n",
                 "    # penalty_factor=None, # all 1s\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -136,15 +136,15 @@
             "outputs": [],
             "source": [
                 "adjusted = sample_with_target.adjust(\n",
                 "    # method=\"ipw\",\n",
                 "    transformations=None,\n",
                 "    # formula=formula,\n",
                 "    # penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -187,15 +187,15 @@
                 "}\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    # method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    # formula=formula,\n",
                 "    # penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -232,15 +232,15 @@
                 "}\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    # method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    # formula=formula,\n",
                 "    # penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -317,15 +317,15 @@
                 "}\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    # method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    # formula=formula,\n",
                 "    # penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -369,15 +369,15 @@
                 "# penalty_factor = [0.1, 0.1, 0.1]\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    formula=formula,\n",
                 "    # penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")\n",
                 ""
             ]
         },
@@ -433,15 +433,15 @@
                 "penalty_factor = [10, 0.1]\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    formula=formula,\n",
                 "    penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")\n",
                 ""
             ]
         },
@@ -481,15 +481,15 @@
                 "penalty_factor = [0.1, 10]  # this is flipped\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    formula=formula,\n",
                 "    penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")\n",
                 ""
             ]
         },
@@ -534,15 +534,15 @@
                 "penalty_factor = [1, 2, 2]\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    formula=formula,\n",
                 "    penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")\n",
                 ""
             ]
         },
@@ -585,15 +585,15 @@
                 "penalty_factor = [1, 1, 1]\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    formula=formula,\n",
                 "    penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "adj_diag = adjusted.diagnostics()\n",
                 "adj_diag.query(\"metric == 'model_coef'\")\n",
                 ""
             ]
         },
@@ -626,15 +626,15 @@
                 "showInput": true
             },
             "outputs": [],
             "source": [
                 "# Defaults from the package\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "print(adjusted.summary())\n",
                 "print(adjusted.outcomes().summary())\n",
                 "adjusted.covars().plot(library = \"seaborn\", dist_type = \"kde\")"
             ]
         },
@@ -663,15 +663,15 @@
                 "# }\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=None,\n",
                 "    # formula=formula,\n",
                 "    # penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "print(adjusted.summary())\n",
                 "print(adjusted.outcomes().summary())\n",
                 "adjusted.covars().plot(library = \"seaborn\", dist_type = \"kde\")\n",
                 "\n",
                 "# slightly smaller design effect, slightly better ASMD reduction."
@@ -700,15 +700,15 @@
                 "# penalty_factor = [1]\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    formula=formula,\n",
                 "    # penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "print(adjusted.summary())\n",
                 "print(adjusted.outcomes().summary())\n",
                 "adjusted.covars().plot(library = \"seaborn\", dist_type = \"kde\")\n",
                 "\n",
                 "# Adding income**2 to the formula led to lower Deff but also lower ASMD reduction."
@@ -740,15 +740,15 @@
                 "penalty_factor = [1, 0.1]\n",
                 "\n",
                 "adjusted = sample_with_target.adjust(\n",
                 "    method=\"ipw\",\n",
                 "    transformations=transformations,\n",
                 "    formula=formula,\n",
                 "    penalty_factor=penalty_factor,\n",
-                "    max_de=None,\n",
+                "    # max_de=None,\n",
                 ")\n",
                 "\n",
                 "print(adjusted.summary())\n",
                 "print(adjusted.outcomes().summary())\n",
                 "adjusted.covars().plot(library = \"seaborn\", dist_type = \"kde\")\n",
                 "\n",
                 "# By adding income_buckets and using it instead of income, as well as putting more weight in it in terms of panelty\n",
```

### Comparing `balance-0.7.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb` & `balance-0.8.0/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.ipynb`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/README.md` & `balance-0.8.0/website/README.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/blog/2023/01/09/bringing-balance-to-your-data.md` & `balance-0.8.0/website/blog/2023/01/09/bringing-balance-to-your-data.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp` & `balance-0.8.0/website/blog/2023/01/09/sample_vs_target_bar_chart.webp`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/general_framework/adjusting_sample_to_population.md` & `balance-0.8.0/website/docs/docs/general_framework/adjusting_sample_to_population.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,19 @@
 2. **Fitting the model** and calculating the weights: the model fitted depends on the ```method``` chosen by the user. Current options are [inverse propensity score weighting](../statistical_methods/ipw.md) using regularized logistic regression (```ipw```), [covariate balancing propensity score](../statistical_methods/cbps.md) (```cbps```) and [post-stratification](../statistical_methods/poststratify.md) (```poststratify```).
 3. **Post-processing** of the weights:
     * Trimming weights - balance trims the weights in order to avoid over fitting of the model and unnecessary variance inflation.
     * Normalizing weights to population size. The resulting weights of balance can be described as approximating the number of unit in the population this unit of the sample represents.
 
 ## Optional arguments
 
-* **`method`**: `ipw`, `poststratify`, or `cbps`.  Default is `ipw`.
+* **`method`**: `ipw`, `poststratify`, `rake`, or `cbps`.  Default is `ipw`.
     * `ipw`: stands for [Inverse Propensity Weighting](https://en.wikipedia.org/wiki/Inverse_probability_weighting). The propensity scores are calculated with [LASSO](https://en.wikipedia.org/wiki/Lasso_(statistics)) [logistic regression](https://en.wikipedia.org/wiki/Logistic_regression).  Details about the implementation can be found [here](../../statistical_methods/ipw/).
    * `cbps`: stands for [Covariate Balancing Propensity Score](https://imai.fas.harvard.edu/software/CBPS.html). The CBPS algorithm estimates the propensity score in a way that optimizes prediction of the probability of sample inclusion as well as the covariates balance. Its main advantage is in cases when the researcher wants better balance on the covariates than traditional propensity score methods - because one believes the assignment model might be misspecified and would like to avoid an iterative procedure of balancing the covariates. Details about the implementation can be found [here](../../statistical_methods/cbps/).
    * `poststratify`: stands for post-stratification. Details about the implementation can be found [here](../../statistical_methods/poststratify/).
+   * `rake`: TODO: add details.
 
 * **`variables`**: allows user to pass a list of the covariates that they want to adjust for; if variables argument is not specified, all joint variables in sample and target are used.
 
 * **`transformations`**: which transformations to apply to data before fitting the model. Default is cutting numeric variables into 10 quantile buckets and lumping together infrequent levels with less than 5% prevalence into `lumped_other` category. The transformations are done on both the sample dataframe and the target dataframe together. User can also specify specific transformations in a dictionary format.
 
 * **`max_de`**: (for `ipw` and `cbps` methods): The default value is 1.5. It limits the [**design effect**](https://en.wikipedia.org/wiki/Design_effect) to be within 1.5. If set to None, the optimization is performed by cross-validation of the logistic model for ipw (see the `choose_regularization` function for more details) or without constrained optimization for cbps. Setting `max_de` to `None` can sometimes significantly improve the running time of the code.
```

### Comparing `balance-0.7.0/website/docs/docs/general_framework/evaluation_of_results.md` & `balance-0.8.0/website/docs/docs/general_framework/evaluation_of_results.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/general_framework/general_framework.md` & `balance-0.8.0/website/docs/docs/general_framework/general_framework.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md` & `balance-0.8.0/website/docs/docs/general_framework/pre_adjustment_diagnostics.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_01_qqplot_income_before.png` & `balance-0.8.0/website/docs/docs/img/fig_01_qqplot_income_before.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_02_barplot_age_before.png` & `balance-0.8.0/website/docs/docs/img/fig_02_barplot_age_before.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_03_barplot_gender_before.png` & `balance-0.8.0/website/docs/docs/img/fig_03_barplot_gender_before.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_04_qqplot_income_after.png` & `balance-0.8.0/website/docs/docs/img/fig_04_qqplot_income_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_05_barplot_age_after.png` & `balance-0.8.0/website/docs/docs/img/fig_05_barplot_age_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_06_barplot_gender_after.png` & `balance-0.8.0/website/docs/docs/img/fig_06_barplot_gender_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_07_seaborn_after.png` & `balance-0.8.0/website/docs/docs/img/fig_07_seaborn_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_08_weights_kde.png` & `balance-0.8.0/website/docs/docs/img/fig_08_weights_kde.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png` & `balance-0.8.0/website/docs/docs/img/fig_09_seaborn_outcome_kde_after.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.png` & `balance-0.8.0/website/docs/docs/img/total_survey_error_flow_v02.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/total_survey_error_flow_v02.svg` & `balance-0.8.0/website/docs/docs/img/total_survey_error_flow_v02.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/total_survey_error_image.png` & `balance-0.8.0/website/docs/docs/img/total_survey_error_image.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/img/total_survey_error_image.svg` & `balance-0.8.0/website/docs/docs/img/total_survey_error_image.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/statistical_methods/cbps.md` & `balance-0.8.0/website/docs/docs/statistical_methods/cbps.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/statistical_methods/ipw.md` & `balance-0.8.0/website/docs/docs/statistical_methods/ipw.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/docs/statistical_methods/poststratify.md` & `balance-0.8.0/website/docs/docs/statistical_methods/poststratify.md`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx` & `balance-0.8.0/website/docs/tutorials/comparing_cbps_in_r_vs_python_using_sim_data.mdx`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
 title: Comparing_cbps_in_r_vs_python_using_sim_data
-sidebar_position: 4
+sidebar_position: 6
 hide_table_of_contents: true
 hide_title: true
 ---
 
 import HTMLLoader from '@site/src/components/HTMLLoader';
 import useBaseUrl from '@docusaurus/useBaseUrl';
```

### Comparing `balance-0.7.0/website/docs/tutorials/index.mdx` & `balance-0.8.0/website/docs/tutorials/index.mdx`

 * *Files 10% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 **Requirements**: You will need a [Jupyter installation](https://jupyter.org/) to run these notebooks yourselves. We also assume you have the [balance pkg](/docs/docs/overview) installed.
 
 If you are new to balance, we suggest getting started with the [balance Quickstart](./quickstart) tutorial.
 
 ## Tutorials list (more tutorials to be added soon):
 1. [**quickstart**](./quickstart) - this is based on a simulated data and presents the simple end-to-end workflow of balance package with default arguments. It demonstrates the process from reading the data, through understanding the biases in the sample, producing weights, evaluating the results and producing the population estimations.
 2. [**quickstart_cbps**](./quickstart_cbps) - like the [**quickstart**](./quickstart) tutorial, but shows how to use the CBPS algorithm and compares the results to IPW (logistic regression with LASSO).
-3. [**balance_transformations_and_formulas**](./balance_transformations_and_formulas) - This tutorial showcases ways in which transformations, formulas and penalty can be included in your pre-processing of the covariates before adjusting for them.
-4. [**comparing_cbps_in_r_vs_python_using_sim_data**](./comparing_cbps_in_r_vs_python_using_sim_data) - This notebook compares the results of running CBPS in R and Python. In R using the `BCPS` package, and in Python using the `balance` package. The results are almost identical.
+3. [**quickstart_rake**](./quickstart_rake) - like the [**quickstart**](./quickstart) tutorial, but shows how to use the rake (raking) algorithm and compares the results to IPW (logistic regression with LASSO).
+4. [**balance_transformations_and_formulas**](./balance_transformations_and_formulas) - This tutorial showcases ways in which transformations, formulas and penalty can be included in your pre-processing of the covariates before adjusting for them.
+5. [**comparing_cbps_in_r_vs_python_using_sim_data**](./comparing_cbps_in_r_vs_python_using_sim_data) - This notebook compares the results of running CBPS in R and Python. In R using the `BCPS` package, and in Python using the `balance` package. The results are almost identical.
```

### Comparing `balance-0.7.0/website/docusaurus.config.js` & `balance-0.8.0/website/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/package.json` & `balance-0.8.0/website/package.json`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/sidebars.js` & `balance-0.8.0/website/sidebars.js`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/src/components/HTMLLoader.js` & `balance-0.8.0/website/src/components/HTMLLoader.js`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/src/components/HomepageFeatures.js` & `balance-0.8.0/website/src/components/HomepageFeatures.js`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/src/css/custom.css` & `balance-0.8.0/website/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/src/pages/index.js` & `balance-0.8.0/website/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/src/pages/index.module.css` & `balance-0.8.0/website/src/pages/index.module.css`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai` & `balance-0.8.0/website/static/img/balance_logo/AI/balance_Logo_FINAL.ai`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_Black_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Horizontal/balance_Logo_Horizontal_White_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_Black_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_FullColor_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Icon/balance_Logo_Icon_White_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_Black_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_FullColor_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png` & `balance-0.8.0/website/static/img/balance_logo/PNG/Vertical/balance_Logo_Vertical_White_RGB.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_Black_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_FullColor_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Horizontal/balance_Logo_Horizontal_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_Black_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_FullColor_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Icon/balance_Logo_Icon_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_Black_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_FullColor_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg` & `balance-0.8.0/website/static/img/balance_logo/SVG/Vertical/balance_Logo_Vertical_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/icon.png` & `balance-0.8.0/website/static/img/balance_logo/icon.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/icon.svg` & `balance-0.8.0/website/static/img/balance_logo/icon.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/vertical.svg` & `balance-0.8.0/website/static/img/balance_logo/vertical.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/balance_logo/vertical_white.svg` & `balance-0.8.0/website/static/img/balance_logo/vertical_white.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/docusaurus.png` & `balance-0.8.0/website/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/favicon.ico` & `balance-0.8.0/website/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/fontawesome/code.svg` & `balance-0.8.0/website/static/img/fontawesome/code.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/fontawesome/layer-group.svg` & `balance-0.8.0/website/static/img/fontawesome/layer-group.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/fontawesome/users.svg` & `balance-0.8.0/website/static/img/fontawesome/users.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/logo.svg` & `balance-0.8.0/website/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/meta_opensource_logo_negative.svg` & `balance-0.8.0/website/static/img/meta_opensource_logo_negative.svg`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/tutorial/docsVersionDropdown.png` & `balance-0.8.0/website/static/img/tutorial/docsVersionDropdown.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/static/img/tutorial/localeDropdown.png` & `balance-0.8.0/website/static/img/tutorial/localeDropdown.png`

 * *Files identical despite different names*

### Comparing `balance-0.7.0/website/yarn.lock` & `balance-0.8.0/website/yarn.lock`

 * *Files identical despite different names*

