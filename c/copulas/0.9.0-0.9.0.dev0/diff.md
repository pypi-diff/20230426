# Comparing `tmp/copulas-0.9.0.tar.gz` & `tmp/copulas-0.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copulas-0.9.0.tar", last modified: Wed Apr 26 20:54:33 2023, max compression
+gzip compressed data, was "copulas-0.9.0.dev0.tar", last modified: Wed Apr 26 20:48:40 2023, max compression
```

## Comparing `copulas-0.9.0.tar` & `copulas-0.9.0.dev0.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.840180 copulas-0.9.0/
--rw-r--r--   0 pacho      (501) staff       (20)       60 2022-12-22 00:00:14.000000 copulas-0.9.0/AUTHORS.rst
--rw-r--r--   0 pacho      (501) staff       (20)     6966 2022-09-25 13:36:10.000000 copulas-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 pacho      (501) staff       (20)    10381 2023-04-26 20:54:29.000000 copulas-0.9.0/HISTORY.md
--rw-r--r--   0 pacho      (501) staff       (20)     4822 2022-12-22 00:00:14.000000 copulas-0.9.0/LICENSE
--rw-r--r--   0 pacho      (501) staff       (20)      284 2022-09-25 13:36:10.000000 copulas-0.9.0/MANIFEST.in
--rw-r--r--   0 pacho      (501) staff       (20)    16599 2023-04-26 20:54:33.840345 copulas-0.9.0/PKG-INFO
--rw-r--r--   0 pacho      (501) staff       (20)     5226 2022-12-20 14:09:06.000000 copulas-0.9.0/README.md
--rw-r--r--   0 pacho      (501) staff       (20)     6616 2022-09-25 13:36:10.000000 copulas-0.9.0/RELEASE.md
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.809285 copulas-0.9.0/copulas/
--rw-r--r--   0 pacho      (501) staff       (20)     7047 2023-04-26 20:54:29.000000 copulas-0.9.0/copulas/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)      823 2023-04-26 20:54:29.000000 copulas-0.9.0/copulas/_addons.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.811827 copulas-0.9.0/copulas/bivariate/
--rw-r--r--   0 pacho      (501) staff       (20)     5087 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/bivariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)    13952 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/bivariate/base.py
--rw-r--r--   0 pacho      (501) staff       (20)     4536 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/bivariate/clayton.py
--rw-r--r--   0 pacho      (501) staff       (20)     4641 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/bivariate/frank.py
--rw-r--r--   0 pacho      (501) staff       (20)     4216 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/bivariate/gumbel.py
--rw-r--r--   0 pacho      (501) staff       (20)     2069 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/bivariate/independence.py
--rw-r--r--   0 pacho      (501) staff       (20)      347 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/bivariate/utils.py
--rw-r--r--   0 pacho      (501) staff       (20)     6831 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/datasets.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.813207 copulas-0.9.0/copulas/multivariate/
--rw-r--r--   0 pacho      (501) staff       (20)      362 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/multivariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)     5600 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/multivariate/base.py
--rw-r--r--   0 pacho      (501) staff       (20)    11166 2023-04-26 20:54:29.000000 copulas-0.9.0/copulas/multivariate/gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)    22020 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/multivariate/tree.py
--rw-r--r--   0 pacho      (501) staff       (20)    12913 2022-12-26 16:35:43.000000 copulas-0.9.0/copulas/multivariate/vine.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.813473 copulas-0.9.0/copulas/optimize/
--rw-r--r--   0 pacho      (501) staff       (20)     4927 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/optimize/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.815987 copulas-0.9.0/copulas/univariate/
--rw-r--r--   0 pacho      (501) staff       (20)      825 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)    19976 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/base.py
--rw-r--r--   0 pacho      (501) staff       (20)     1016 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/beta.py
--rw-r--r--   0 pacho      (501) staff       (20)      906 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/gamma.py
--rw-r--r--   0 pacho      (501) staff       (20)      728 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)     6093 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/gaussian_kde.py
--rw-r--r--   0 pacho      (501) staff       (20)      921 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/log_laplace.py
--rw-r--r--   0 pacho      (501) staff       (20)      944 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/selection.py
--rw-r--r--   0 pacho      (501) staff       (20)      823 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/student_t.py
--rw-r--r--   0 pacho      (501) staff       (20)     1932 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/truncated_gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)      754 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/univariate/uniform.py
--rw-r--r--   0 pacho      (501) staff       (20)     4665 2022-09-25 13:36:10.000000 copulas-0.9.0/copulas/visualization.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.810219 copulas-0.9.0/copulas.egg-info/
--rw-r--r--   0 pacho      (501) staff       (20)    16599 2023-04-26 20:54:33.000000 copulas-0.9.0/copulas.egg-info/PKG-INFO
--rw-r--r--   0 pacho      (501) staff       (20)     7643 2023-04-26 20:54:33.000000 copulas-0.9.0/copulas.egg-info/SOURCES.txt
--rw-r--r--   0 pacho      (501) staff       (20)        1 2023-04-26 20:54:33.000000 copulas-0.9.0/copulas.egg-info/dependency_links.txt
--rw-r--r--   0 pacho      (501) staff       (20)        1 2023-04-26 20:54:33.000000 copulas-0.9.0/copulas.egg-info/not-zip-safe
--rw-r--r--   0 pacho      (501) staff       (20)     1693 2023-04-26 20:54:33.000000 copulas-0.9.0/copulas.egg-info/requires.txt
--rw-r--r--   0 pacho      (501) staff       (20)        8 2023-04-26 20:54:33.000000 copulas-0.9.0/copulas.egg-info/top_level.txt
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.817546 copulas-0.9.0/docs/
--rw-r--r--   0 pacho      (501) staff       (20)      608 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/Makefile
--rw-r--r--   0 pacho      (501) staff       (20)       28 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/authors.rst
--rwxr-xr-x   0 pacho      (501) staff       (20)     5852 2022-12-22 00:00:14.000000 copulas-0.9.0/docs/conf.py
--rw-r--r--   0 pacho      (501) staff       (20)       33 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/contributing.rst
--rw-r--r--   0 pacho      (501) staff       (20)       29 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/history.rst
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.821437 copulas-0.9.0/docs/images/
--rw-r--r--   0 pacho      (501) staff       (20)    15307 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/images/copulas-200.png
--rw-r--r--   0 pacho      (501) staff       (20)    26688 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/images/copulas.png
--rw-r--r--   0 pacho      (501) staff       (20)    52079 2022-12-20 13:34:50.000000 copulas-0.9.0/docs/images/copulas_sample_dataset.png
--rw-r--r--   0 pacho      (501) staff       (20)   886153 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/images/dai-logo-white.png
--rw-r--r--   0 pacho      (501) staff       (20)     4753 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/images/dice_cdf.png
--rw-r--r--   0 pacho      (501) staff       (20)    23772 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/images/pdf_cdf.png
--rw-r--r--   0 pacho      (501) staff       (20)     9447 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/images/pit.png
--rw-r--r--   0 pacho      (501) staff       (20)   128308 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/images/quickstart.png
--rw-r--r--   0 pacho      (501) staff       (20)      651 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/index.rst
--rw-r--r--   0 pacho      (501) staff       (20)       29 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/install.rst
--rw-r--r--   0 pacho      (501) staff       (20)      769 2022-09-25 13:36:10.000000 copulas-0.9.0/docs/make.bat
--rw-r--r--   0 pacho      (501) staff       (20)     1441 2023-04-26 20:54:33.840829 copulas-0.9.0/setup.cfg
--rw-r--r--   0 pacho      (501) staff       (20)     4015 2023-04-26 20:54:29.000000 copulas-0.9.0/setup.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.821906 copulas-0.9.0/tests/
--rw-r--r--   0 pacho      (501) staff       (20)     4710 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.822514 copulas-0.9.0/tests/end-to-end/
--rw-r--r--   0 pacho      (501) staff       (20)     1663 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/README.md
--rw-r--r--   0 pacho      (501) staff       (20)       41 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.822811 copulas-0.9.0/tests/end-to-end/bivariate/
--rw-r--r--   0 pacho      (501) staff       (20)       51 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/bivariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)     1301 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/bivariate/test_base.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.823410 copulas-0.9.0/tests/end-to-end/multivariate/
--rw-r--r--   0 pacho      (501) staff       (20)       54 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/multivariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)     1146 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/multivariate/test_base.py
--rw-r--r--   0 pacho      (501) staff       (20)     6948 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/multivariate/test_gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)     1910 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/multivariate/test_vine.py
--rw-r--r--   0 pacho      (501) staff       (20)     1670 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/test___init__.py
--rw-r--r--   0 pacho      (501) staff       (20)      184 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/test_visualization.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.824458 copulas-0.9.0/tests/end-to-end/univariate/
--rw-r--r--   0 pacho      (501) staff       (20)       52 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/univariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)     5170 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/univariate/test_beta.py
--rw-r--r--   0 pacho      (501) staff       (20)     5090 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/univariate/test_gamma.py
--rw-r--r--   0 pacho      (501) staff       (20)     5032 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/univariate/test_gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)     5576 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/univariate/test_gaussian_kde.py
--rw-r--r--   0 pacho      (501) staff       (20)     5210 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/univariate/test_student_t.py
--rw-r--r--   0 pacho      (501) staff       (20)     5276 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/end-to-end/univariate/test_truncated_gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)     9510 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/large_scale_evaluation.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.824755 copulas-0.9.0/tests/numerical/
--rw-r--r--   0 pacho      (501) staff       (20)     3795 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/README.md
--rw-r--r--   0 pacho      (501) staff       (20)       40 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.825035 copulas-0.9.0/tests/numerical/cdf/
--rw-r--r--   0 pacho      (501) staff       (20)       44 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.825201 copulas-0.9.0/tests/numerical/cdf/input/
--rw-r--r--   0 pacho      (501) staff       (20)      120 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/input/bivariate_cdf_input.csv
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.827520 copulas-0.9.0/tests/numerical/cdf/output/
--rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      223 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      223 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      216 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      216 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      217 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      217 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_R.csv
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.828006 copulas-0.9.0/tests/numerical/cdf/scripts/
--rw-r--r--   0 pacho      (501) staff       (20)      604 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/scripts/bivariate_cdf_input.py
--rw-r--r--   0 pacho      (501) staff       (20)     2090 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/scripts/bivariate_cdf_output.R
--rw-r--r--   0 pacho      (501) staff       (20)     1678 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/scripts/bivariate_cdf_output.m
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.805371 copulas-0.9.0/tests/numerical/cdf/test_cases/
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.828442 copulas-0.9.0/tests/numerical/cdf/test_cases/clayton/
--rw-r--r--   0 pacho      (501) staff       (20)      808 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      744 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json
--rw-r--r--   0 pacho      (501) staff       (20)      743 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.828865 copulas-0.9.0/tests/numerical/cdf/test_cases/frank/
--rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      737 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json
--rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.829151 copulas-0.9.0/tests/numerical/cdf/test_cases/gumbel/
--rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json
--rw-r--r--   0 pacho      (501) staff       (20)     1077 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/cdf/test_cdf.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.829421 copulas-0.9.0/tests/numerical/fit/
--rw-r--r--   0 pacho      (501) staff       (20)       44 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.829701 copulas-0.9.0/tests/numerical/fit/input/
--rw-r--r--   0 pacho      (501) staff       (20)       54 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/input/bivariate_fit_test_case_1_input.csv
--rw-r--r--   0 pacho      (501) staff       (20)       72 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/input/bivariate_fit_test_case_2_input.csv
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.829998 copulas-0.9.0/tests/numerical/fit/scripts/
--rw-r--r--   0 pacho      (501) staff       (20)     1008 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/scripts/bivariate_fit_output.R
--rw-r--r--   0 pacho      (501) staff       (20)      780 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/scripts/bivariate_fit_output.m
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.805877 copulas-0.9.0/tests/numerical/fit/test_cases/
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.830301 copulas-0.9.0/tests/numerical/fit/test_cases/clayton/
--rw-r--r--   0 pacho      (501) staff       (20)      826 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      828 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.830592 copulas-0.9.0/tests/numerical/fit/test_cases/frank/
--rw-r--r--   0 pacho      (501) staff       (20)      820 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      820 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.830883 copulas-0.9.0/tests/numerical/fit/test_cases/gumbel/
--rw-r--r--   0 pacho      (501) staff       (20)      823 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      823 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json
--rw-r--r--   0 pacho      (501) staff       (20)      966 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/fit/test_fit.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.831163 copulas-0.9.0/tests/numerical/pdf/
--rw-r--r--   0 pacho      (501) staff       (20)       44 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.831320 copulas-0.9.0/tests/numerical/pdf/input/
--rw-r--r--   0 pacho      (501) staff       (20)      120 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/input/bivariate_pdf_input.csv
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.833659 copulas-0.9.0/tests/numerical/pdf/output/
--rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      214 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      214 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      208 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      208 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_R.csv
--rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_R.csv
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.834092 copulas-0.9.0/tests/numerical/pdf/scripts/
--rw-r--r--   0 pacho      (501) staff       (20)      603 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/scripts/bivariate_pdf_input.py
--rw-r--r--   0 pacho      (501) staff       (20)     2070 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/scripts/bivariate_pdf_output.R
--rw-r--r--   0 pacho      (501) staff       (20)     1694 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/scripts/bivariate_pdf_output.m
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.806442 copulas-0.9.0/tests/numerical/pdf/test_cases/
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.834514 copulas-0.9.0/tests/numerical/pdf/test_cases/clayton/
--rw-r--r--   0 pacho      (501) staff       (20)      743 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      744 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json
--rw-r--r--   0 pacho      (501) staff       (20)      743 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.834934 copulas-0.9.0/tests/numerical/pdf/test_cases/frank/
--rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      737 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json
--rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.835233 copulas-0.9.0/tests/numerical/pdf/test_cases/gumbel/
--rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json
--rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json
--rw-r--r--   0 pacho      (501) staff       (20)     1086 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/numerical/pdf/test_pdf.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.835678 copulas-0.9.0/tests/unit/
--rw-r--r--   0 pacho      (501) staff       (20)       35 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/__init__.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.836718 copulas-0.9.0/tests/unit/bivariate/
--rw-r--r--   0 pacho      (501) staff       (20)       45 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/bivariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)      490 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/bivariate/test___init__.py
--rw-r--r--   0 pacho      (501) staff       (20)     3907 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/bivariate/test_base.py
--rw-r--r--   0 pacho      (501) staff       (20)     3549 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/bivariate/test_clayton.py
--rw-r--r--   0 pacho      (501) staff       (20)     3583 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/bivariate/test_frank.py
--rw-r--r--   0 pacho      (501) staff       (20)     3567 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/bivariate/test_gumbel.py
--rw-r--r--   0 pacho      (501) staff       (20)     1412 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/bivariate/test_independence.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.837854 copulas-0.9.0/tests/unit/multivariate/
--rw-r--r--   0 pacho      (501) staff       (20)       48 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/multivariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)      382 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/multivariate/test_base.py
--rw-r--r--   0 pacho      (501) staff       (20)    18721 2023-04-26 20:54:29.000000 copulas-0.9.0/tests/unit/multivariate/test_gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)    24177 2022-12-20 16:51:04.000000 copulas-0.9.0/tests/unit/multivariate/test_tree.py
--rw-r--r--   0 pacho      (501) staff       (20)     6015 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/multivariate/test_vine.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.838270 copulas-0.9.0/tests/unit/optimize/
--rw-r--r--   0 pacho      (501) staff       (20)       53 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/optimize/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)      899 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/optimize/test___init__.py
--rw-r--r--   0 pacho      (501) staff       (20)    12972 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/test___init__.py
--rw-r--r--   0 pacho      (501) staff       (20)     1379 2023-04-26 20:54:29.000000 copulas-0.9.0/tests/unit/test__addons.py
-drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:54:33.840030 copulas-0.9.0/tests/unit/univariate/
--rw-r--r--   0 pacho      (501) staff       (20)       46 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/__init__.py
--rw-r--r--   0 pacho      (501) staff       (20)     7497 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_base.py
--rw-r--r--   0 pacho      (501) staff       (20)     2432 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_beta.py
--rw-r--r--   0 pacho      (501) staff       (20)     1428 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_gamma.py
--rw-r--r--   0 pacho      (501) staff       (20)     1305 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)     6788 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_gaussian_kde.py
--rw-r--r--   0 pacho      (501) staff       (20)     1412 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_log_laplace.py
--rw-r--r--   0 pacho      (501) staff       (20)     3059 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_selection.py
--rw-r--r--   0 pacho      (501) staff       (20)     1197 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_student_t.py
--rw-r--r--   0 pacho      (501) staff       (20)     1532 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_truncated_gaussian.py
--rw-r--r--   0 pacho      (501) staff       (20)     1387 2022-09-25 13:36:10.000000 copulas-0.9.0/tests/unit/univariate/test_uniform.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.018644 copulas-0.9.0.dev0/
+-rw-r--r--   0 pacho      (501) staff       (20)       60 2022-12-22 00:00:14.000000 copulas-0.9.0.dev0/AUTHORS.rst
+-rw-r--r--   0 pacho      (501) staff       (20)     6966 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 pacho      (501) staff       (20)    10381 2023-04-26 20:46:41.000000 copulas-0.9.0.dev0/HISTORY.md
+-rw-r--r--   0 pacho      (501) staff       (20)     4822 2022-12-22 00:00:14.000000 copulas-0.9.0.dev0/LICENSE
+-rw-r--r--   0 pacho      (501) staff       (20)      284 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/MANIFEST.in
+-rw-r--r--   0 pacho      (501) staff       (20)    16604 2023-04-26 20:48:40.018747 copulas-0.9.0.dev0/PKG-INFO
+-rw-r--r--   0 pacho      (501) staff       (20)     5226 2022-12-20 14:09:06.000000 copulas-0.9.0.dev0/README.md
+-rw-r--r--   0 pacho      (501) staff       (20)     6616 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/RELEASE.md
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.988782 copulas-0.9.0.dev0/copulas/
+-rw-r--r--   0 pacho      (501) staff       (20)     7052 2023-04-26 20:47:55.000000 copulas-0.9.0.dev0/copulas/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)      823 2023-04-20 16:53:47.000000 copulas-0.9.0.dev0/copulas/_addons.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.990691 copulas-0.9.0.dev0/copulas/bivariate/
+-rw-r--r--   0 pacho      (501) staff       (20)     5087 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/bivariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)    13952 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/bivariate/base.py
+-rw-r--r--   0 pacho      (501) staff       (20)     4536 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/bivariate/clayton.py
+-rw-r--r--   0 pacho      (501) staff       (20)     4641 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/bivariate/frank.py
+-rw-r--r--   0 pacho      (501) staff       (20)     4216 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/bivariate/gumbel.py
+-rw-r--r--   0 pacho      (501) staff       (20)     2069 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/bivariate/independence.py
+-rw-r--r--   0 pacho      (501) staff       (20)      347 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/bivariate/utils.py
+-rw-r--r--   0 pacho      (501) staff       (20)     6831 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/datasets.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.991554 copulas-0.9.0.dev0/copulas/multivariate/
+-rw-r--r--   0 pacho      (501) staff       (20)      362 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/multivariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)     5600 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/multivariate/base.py
+-rw-r--r--   0 pacho      (501) staff       (20)    11166 2023-04-20 16:53:47.000000 copulas-0.9.0.dev0/copulas/multivariate/gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)    22020 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/multivariate/tree.py
+-rw-r--r--   0 pacho      (501) staff       (20)    12913 2022-12-26 16:35:43.000000 copulas-0.9.0.dev0/copulas/multivariate/vine.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.991816 copulas-0.9.0.dev0/copulas/optimize/
+-rw-r--r--   0 pacho      (501) staff       (20)     4927 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/optimize/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.993618 copulas-0.9.0.dev0/copulas/univariate/
+-rw-r--r--   0 pacho      (501) staff       (20)      825 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)    19976 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/base.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1016 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/beta.py
+-rw-r--r--   0 pacho      (501) staff       (20)      906 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/gamma.py
+-rw-r--r--   0 pacho      (501) staff       (20)      728 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)     6093 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/gaussian_kde.py
+-rw-r--r--   0 pacho      (501) staff       (20)      921 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/log_laplace.py
+-rw-r--r--   0 pacho      (501) staff       (20)      944 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/selection.py
+-rw-r--r--   0 pacho      (501) staff       (20)      823 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/student_t.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1932 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/truncated_gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)      754 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/univariate/uniform.py
+-rw-r--r--   0 pacho      (501) staff       (20)     4665 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/copulas/visualization.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.989716 copulas-0.9.0.dev0/copulas.egg-info/
+-rw-r--r--   0 pacho      (501) staff       (20)    16604 2023-04-26 20:48:39.000000 copulas-0.9.0.dev0/copulas.egg-info/PKG-INFO
+-rw-r--r--   0 pacho      (501) staff       (20)     7643 2023-04-26 20:48:39.000000 copulas-0.9.0.dev0/copulas.egg-info/SOURCES.txt
+-rw-r--r--   0 pacho      (501) staff       (20)        1 2023-04-26 20:48:39.000000 copulas-0.9.0.dev0/copulas.egg-info/dependency_links.txt
+-rw-r--r--   0 pacho      (501) staff       (20)        1 2023-04-26 20:48:39.000000 copulas-0.9.0.dev0/copulas.egg-info/not-zip-safe
+-rw-r--r--   0 pacho      (501) staff       (20)     1693 2023-04-26 20:48:39.000000 copulas-0.9.0.dev0/copulas.egg-info/requires.txt
+-rw-r--r--   0 pacho      (501) staff       (20)        8 2023-04-26 20:48:39.000000 copulas-0.9.0.dev0/copulas.egg-info/top_level.txt
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.994959 copulas-0.9.0.dev0/docs/
+-rw-r--r--   0 pacho      (501) staff       (20)      608 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/Makefile
+-rw-r--r--   0 pacho      (501) staff       (20)       28 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/authors.rst
+-rwxr-xr-x   0 pacho      (501) staff       (20)     5852 2022-12-22 00:00:14.000000 copulas-0.9.0.dev0/docs/conf.py
+-rw-r--r--   0 pacho      (501) staff       (20)       33 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/contributing.rst
+-rw-r--r--   0 pacho      (501) staff       (20)       29 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/history.rst
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.998778 copulas-0.9.0.dev0/docs/images/
+-rw-r--r--   0 pacho      (501) staff       (20)    15307 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/images/copulas-200.png
+-rw-r--r--   0 pacho      (501) staff       (20)    26688 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/images/copulas.png
+-rw-r--r--   0 pacho      (501) staff       (20)    52079 2022-12-20 13:34:50.000000 copulas-0.9.0.dev0/docs/images/copulas_sample_dataset.png
+-rw-r--r--   0 pacho      (501) staff       (20)   886153 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/images/dai-logo-white.png
+-rw-r--r--   0 pacho      (501) staff       (20)     4753 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/images/dice_cdf.png
+-rw-r--r--   0 pacho      (501) staff       (20)    23772 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/images/pdf_cdf.png
+-rw-r--r--   0 pacho      (501) staff       (20)     9447 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/images/pit.png
+-rw-r--r--   0 pacho      (501) staff       (20)   128308 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/images/quickstart.png
+-rw-r--r--   0 pacho      (501) staff       (20)      651 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/index.rst
+-rw-r--r--   0 pacho      (501) staff       (20)       29 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/install.rst
+-rw-r--r--   0 pacho      (501) staff       (20)      769 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/docs/make.bat
+-rw-r--r--   0 pacho      (501) staff       (20)     1446 2023-04-26 20:48:40.019194 copulas-0.9.0.dev0/setup.cfg
+-rw-r--r--   0 pacho      (501) staff       (20)     4020 2023-04-26 20:47:55.000000 copulas-0.9.0.dev0/setup.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.999179 copulas-0.9.0.dev0/tests/
+-rw-r--r--   0 pacho      (501) staff       (20)     4710 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.999761 copulas-0.9.0.dev0/tests/end-to-end/
+-rw-r--r--   0 pacho      (501) staff       (20)     1663 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/README.md
+-rw-r--r--   0 pacho      (501) staff       (20)       41 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.000041 copulas-0.9.0.dev0/tests/end-to-end/bivariate/
+-rw-r--r--   0 pacho      (501) staff       (20)       51 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/bivariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1301 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/bivariate/test_base.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.000607 copulas-0.9.0.dev0/tests/end-to-end/multivariate/
+-rw-r--r--   0 pacho      (501) staff       (20)       54 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/multivariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1146 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/multivariate/test_base.py
+-rw-r--r--   0 pacho      (501) staff       (20)     6948 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/multivariate/test_gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1910 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/multivariate/test_vine.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1670 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/test___init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)      184 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/test_visualization.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.001694 copulas-0.9.0.dev0/tests/end-to-end/univariate/
+-rw-r--r--   0 pacho      (501) staff       (20)       52 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/univariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)     5170 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/univariate/test_beta.py
+-rw-r--r--   0 pacho      (501) staff       (20)     5090 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/univariate/test_gamma.py
+-rw-r--r--   0 pacho      (501) staff       (20)     5032 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/univariate/test_gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)     5576 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/univariate/test_gaussian_kde.py
+-rw-r--r--   0 pacho      (501) staff       (20)     5210 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/univariate/test_student_t.py
+-rw-r--r--   0 pacho      (501) staff       (20)     5276 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)     9510 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/large_scale_evaluation.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.002018 copulas-0.9.0.dev0/tests/numerical/
+-rw-r--r--   0 pacho      (501) staff       (20)     3795 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/README.md
+-rw-r--r--   0 pacho      (501) staff       (20)       40 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.002333 copulas-0.9.0.dev0/tests/numerical/cdf/
+-rw-r--r--   0 pacho      (501) staff       (20)       44 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.002488 copulas-0.9.0.dev0/tests/numerical/cdf/input/
+-rw-r--r--   0 pacho      (501) staff       (20)      120 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/input/bivariate_cdf_input.csv
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.005199 copulas-0.9.0.dev0/tests/numerical/cdf/output/
+-rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      220 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      223 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      223 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      219 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      216 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      216 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      217 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      217 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_R.csv
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.005806 copulas-0.9.0.dev0/tests/numerical/cdf/scripts/
+-rw-r--r--   0 pacho      (501) staff       (20)      604 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py
+-rw-r--r--   0 pacho      (501) staff       (20)     2090 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R
+-rw-r--r--   0 pacho      (501) staff       (20)     1678 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.984909 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.006341 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/clayton/
+-rw-r--r--   0 pacho      (501) staff       (20)      808 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      744 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json
+-rw-r--r--   0 pacho      (501) staff       (20)      743 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.006829 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/frank/
+-rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      737 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json
+-rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.007157 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/gumbel/
+-rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json
+-rw-r--r--   0 pacho      (501) staff       (20)     1077 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/cdf/test_cdf.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.007450 copulas-0.9.0.dev0/tests/numerical/fit/
+-rw-r--r--   0 pacho      (501) staff       (20)       44 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.007761 copulas-0.9.0.dev0/tests/numerical/fit/input/
+-rw-r--r--   0 pacho      (501) staff       (20)       54 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/input/bivariate_fit_test_case_1_input.csv
+-rw-r--r--   0 pacho      (501) staff       (20)       72 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/input/bivariate_fit_test_case_2_input.csv
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.008058 copulas-0.9.0.dev0/tests/numerical/fit/scripts/
+-rw-r--r--   0 pacho      (501) staff       (20)     1008 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R
+-rw-r--r--   0 pacho      (501) staff       (20)      780 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.985348 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.008356 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/clayton/
+-rw-r--r--   0 pacho      (501) staff       (20)      826 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      828 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.008638 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/frank/
+-rw-r--r--   0 pacho      (501) staff       (20)      820 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      820 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.008942 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/gumbel/
+-rw-r--r--   0 pacho      (501) staff       (20)      823 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      823 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json
+-rw-r--r--   0 pacho      (501) staff       (20)      966 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/fit/test_fit.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.009276 copulas-0.9.0.dev0/tests/numerical/pdf/
+-rw-r--r--   0 pacho      (501) staff       (20)       44 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.009420 copulas-0.9.0.dev0/tests/numerical/pdf/input/
+-rw-r--r--   0 pacho      (501) staff       (20)      120 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/input/bivariate_pdf_input.csv
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.011740 copulas-0.9.0.dev0/tests/numerical/pdf/output/
+-rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      211 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      214 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      214 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      208 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      208 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      212 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_R.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 pacho      (501) staff       (20)      218 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_R.csv
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.012158 copulas-0.9.0.dev0/tests/numerical/pdf/scripts/
+-rw-r--r--   0 pacho      (501) staff       (20)      603 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py
+-rw-r--r--   0 pacho      (501) staff       (20)     2070 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R
+-rw-r--r--   0 pacho      (501) staff       (20)     1694 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:39.985862 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.012607 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/clayton/
+-rw-r--r--   0 pacho      (501) staff       (20)      743 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      744 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json
+-rw-r--r--   0 pacho      (501) staff       (20)      743 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.013038 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/frank/
+-rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      737 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json
+-rw-r--r--   0 pacho      (501) staff       (20)      733 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.013322 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/gumbel/
+-rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json
+-rw-r--r--   0 pacho      (501) staff       (20)      738 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json
+-rw-r--r--   0 pacho      (501) staff       (20)     1086 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/numerical/pdf/test_pdf.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.013764 copulas-0.9.0.dev0/tests/unit/
+-rw-r--r--   0 pacho      (501) staff       (20)       35 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.014970 copulas-0.9.0.dev0/tests/unit/bivariate/
+-rw-r--r--   0 pacho      (501) staff       (20)       45 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/bivariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)      490 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/bivariate/test___init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)     3907 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/bivariate/test_base.py
+-rw-r--r--   0 pacho      (501) staff       (20)     3549 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/bivariate/test_clayton.py
+-rw-r--r--   0 pacho      (501) staff       (20)     3583 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/bivariate/test_frank.py
+-rw-r--r--   0 pacho      (501) staff       (20)     3567 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/bivariate/test_gumbel.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1412 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/bivariate/test_independence.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.016276 copulas-0.9.0.dev0/tests/unit/multivariate/
+-rw-r--r--   0 pacho      (501) staff       (20)       48 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/multivariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)      382 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/multivariate/test_base.py
+-rw-r--r--   0 pacho      (501) staff       (20)    18721 2023-04-26 10:31:32.000000 copulas-0.9.0.dev0/tests/unit/multivariate/test_gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)    24177 2022-12-20 16:51:04.000000 copulas-0.9.0.dev0/tests/unit/multivariate/test_tree.py
+-rw-r--r--   0 pacho      (501) staff       (20)     6015 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/multivariate/test_vine.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.016690 copulas-0.9.0.dev0/tests/unit/optimize/
+-rw-r--r--   0 pacho      (501) staff       (20)       53 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/optimize/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)      899 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/optimize/test___init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)    12972 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1379 2023-04-20 16:53:47.000000 copulas-0.9.0.dev0/tests/unit/test__addons.py
+drwxr-xr-x   0 pacho      (501) staff       (20)        0 2023-04-26 20:48:40.018492 copulas-0.9.0.dev0/tests/unit/univariate/
+-rw-r--r--   0 pacho      (501) staff       (20)       46 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/__init__.py
+-rw-r--r--   0 pacho      (501) staff       (20)     7497 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_base.py
+-rw-r--r--   0 pacho      (501) staff       (20)     2432 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_beta.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1428 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_gamma.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1305 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)     6788 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_gaussian_kde.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1412 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_log_laplace.py
+-rw-r--r--   0 pacho      (501) staff       (20)     3059 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_selection.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1197 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_student_t.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1532 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_truncated_gaussian.py
+-rw-r--r--   0 pacho      (501) staff       (20)     1387 2022-09-25 13:36:10.000000 copulas-0.9.0.dev0/tests/unit/univariate/test_uniform.py
```

### Comparing `copulas-0.9.0/CONTRIBUTING.rst` & `copulas-0.9.0.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/HISTORY.md` & `copulas-0.9.0.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/LICENSE` & `copulas-0.9.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/PKG-INFO` & `copulas-0.9.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copulas
-Version: 0.9.0
+Version: 0.9.0.dev0
 Summary: Create tabular synthetic data using copulas-based modeling.
 Home-page: https://github.com/sdv-dev/Copulas
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: copulas
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copulas Version: 0.9.0 Summary: Create tabular
+Metadata-Version: 2.1 Name: copulas Version: 0.9.0.dev0 Summary: Create tabular
 synthetic data using copulas-based modeling. Home-page: https://github.com/sdv-
 dev/Copulas Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: copulas Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `copulas-0.9.0/README.md` & `copulas-0.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/RELEASE.md` & `copulas-0.9.0.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/__init__.py` & `copulas-0.9.0.dev0/copulas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for Copulas."""
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '0.9.0'
+__version__ = '0.9.0.dev0'
 
 import contextlib
 import importlib
 from copy import deepcopy
 
 import numpy as np
 import pandas as pd
```

### Comparing `copulas-0.9.0/copulas/_addons.py` & `copulas-0.9.0.dev0/copulas/_addons.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/bivariate/__init__.py` & `copulas-0.9.0.dev0/copulas/bivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/bivariate/base.py` & `copulas-0.9.0.dev0/copulas/bivariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/bivariate/clayton.py` & `copulas-0.9.0.dev0/copulas/bivariate/clayton.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/bivariate/frank.py` & `copulas-0.9.0.dev0/copulas/bivariate/frank.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/bivariate/gumbel.py` & `copulas-0.9.0.dev0/copulas/bivariate/gumbel.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/bivariate/independence.py` & `copulas-0.9.0.dev0/copulas/bivariate/independence.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/datasets.py` & `copulas-0.9.0.dev0/copulas/datasets.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/multivariate/base.py` & `copulas-0.9.0.dev0/copulas/multivariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/multivariate/gaussian.py` & `copulas-0.9.0.dev0/copulas/multivariate/gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/multivariate/tree.py` & `copulas-0.9.0.dev0/copulas/multivariate/tree.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/multivariate/vine.py` & `copulas-0.9.0.dev0/copulas/multivariate/vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/optimize/__init__.py` & `copulas-0.9.0.dev0/copulas/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/__init__.py` & `copulas-0.9.0.dev0/copulas/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/base.py` & `copulas-0.9.0.dev0/copulas/univariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/beta.py` & `copulas-0.9.0.dev0/copulas/univariate/beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/gamma.py` & `copulas-0.9.0.dev0/copulas/univariate/gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/gaussian.py` & `copulas-0.9.0.dev0/copulas/univariate/gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/gaussian_kde.py` & `copulas-0.9.0.dev0/copulas/univariate/gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/log_laplace.py` & `copulas-0.9.0.dev0/copulas/univariate/log_laplace.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/selection.py` & `copulas-0.9.0.dev0/copulas/univariate/selection.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/student_t.py` & `copulas-0.9.0.dev0/copulas/univariate/student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/truncated_gaussian.py` & `copulas-0.9.0.dev0/copulas/univariate/truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/univariate/uniform.py` & `copulas-0.9.0.dev0/copulas/univariate/uniform.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas/visualization.py` & `copulas-0.9.0.dev0/copulas/visualization.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas.egg-info/PKG-INFO` & `copulas-0.9.0.dev0/copulas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copulas
-Version: 0.9.0
+Version: 0.9.0.dev0
 Summary: Create tabular synthetic data using copulas-based modeling.
 Home-page: https://github.com/sdv-dev/Copulas
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: copulas
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copulas Version: 0.9.0 Summary: Create tabular
+Metadata-Version: 2.1 Name: copulas Version: 0.9.0.dev0 Summary: Create tabular
 synthetic data using copulas-based modeling. Home-page: https://github.com/sdv-
 dev/Copulas Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: copulas Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `copulas-0.9.0/copulas.egg-info/SOURCES.txt` & `copulas-0.9.0.dev0/copulas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/copulas.egg-info/requires.txt` & `copulas-0.9.0.dev0/copulas.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/Makefile` & `copulas-0.9.0.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/conf.py` & `copulas-0.9.0.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/copulas-200.png` & `copulas-0.9.0.dev0/docs/images/copulas-200.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/copulas.png` & `copulas-0.9.0.dev0/docs/images/copulas.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/copulas_sample_dataset.png` & `copulas-0.9.0.dev0/docs/images/copulas_sample_dataset.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/dai-logo-white.png` & `copulas-0.9.0.dev0/docs/images/dai-logo-white.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/dice_cdf.png` & `copulas-0.9.0.dev0/docs/images/dice_cdf.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/pdf_cdf.png` & `copulas-0.9.0.dev0/docs/images/pdf_cdf.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/pit.png` & `copulas-0.9.0.dev0/docs/images/pit.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/images/quickstart.png` & `copulas-0.9.0.dev0/docs/images/quickstart.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/index.rst` & `copulas-0.9.0.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/docs/make.bat` & `copulas-0.9.0.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/setup.cfg` & `copulas-0.9.0.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.0
+current_version = 0.9.0.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `copulas-0.9.0/setup.py` & `copulas-0.9.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,10 +133,10 @@
     name='copulas',
     packages=find_packages(include=['copulas', 'copulas.*']),
     python_requires='>=3.7,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/Copulas',
-    version='0.9.0',
+    version='0.9.0.dev0',
     zip_safe=False,
 )
```

### Comparing `copulas-0.9.0/tests/__init__.py` & `copulas-0.9.0.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/README.md` & `copulas-0.9.0.dev0/tests/end-to-end/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/bivariate/test_base.py` & `copulas-0.9.0.dev0/tests/end-to-end/bivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/multivariate/test_base.py` & `copulas-0.9.0.dev0/tests/end-to-end/multivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/multivariate/test_gaussian.py` & `copulas-0.9.0.dev0/tests/end-to-end/multivariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/multivariate/test_vine.py` & `copulas-0.9.0.dev0/tests/end-to-end/multivariate/test_vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/test___init__.py` & `copulas-0.9.0.dev0/tests/end-to-end/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/univariate/test_beta.py` & `copulas-0.9.0.dev0/tests/end-to-end/univariate/test_beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/univariate/test_gamma.py` & `copulas-0.9.0.dev0/tests/end-to-end/univariate/test_gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/univariate/test_gaussian.py` & `copulas-0.9.0.dev0/tests/end-to-end/univariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/univariate/test_gaussian_kde.py` & `copulas-0.9.0.dev0/tests/end-to-end/univariate/test_gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/univariate/test_student_t.py` & `copulas-0.9.0.dev0/tests/end-to-end/univariate/test_student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/end-to-end/univariate/test_truncated_gaussian.py` & `copulas-0.9.0.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/large_scale_evaluation.py` & `copulas-0.9.0.dev0/tests/large_scale_evaluation.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/README.md` & `copulas-0.9.0.dev0/tests/numerical/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/scripts/bivariate_cdf_input.py` & `copulas-0.9.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/scripts/bivariate_cdf_output.R` & `copulas-0.9.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/scripts/bivariate_cdf_output.m` & `copulas-0.9.0.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/cdf/test_cdf.py` & `copulas-0.9.0.dev0/tests/numerical/cdf/test_cdf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/scripts/bivariate_fit_output.R` & `copulas-0.9.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/scripts/bivariate_fit_output.m` & `copulas-0.9.0.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/fit/test_fit.py` & `copulas-0.9.0.dev0/tests/numerical/fit/test_fit.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/scripts/bivariate_pdf_input.py` & `copulas-0.9.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/scripts/bivariate_pdf_output.R` & `copulas-0.9.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/scripts/bivariate_pdf_output.m` & `copulas-0.9.0.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/numerical/pdf/test_pdf.py` & `copulas-0.9.0.dev0/tests/numerical/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/bivariate/test_base.py` & `copulas-0.9.0.dev0/tests/unit/bivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/bivariate/test_clayton.py` & `copulas-0.9.0.dev0/tests/unit/bivariate/test_clayton.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/bivariate/test_frank.py` & `copulas-0.9.0.dev0/tests/unit/bivariate/test_frank.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/bivariate/test_gumbel.py` & `copulas-0.9.0.dev0/tests/unit/bivariate/test_gumbel.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/bivariate/test_independence.py` & `copulas-0.9.0.dev0/tests/unit/bivariate/test_independence.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/multivariate/test_gaussian.py` & `copulas-0.9.0.dev0/tests/unit/multivariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/multivariate/test_tree.py` & `copulas-0.9.0.dev0/tests/unit/multivariate/test_tree.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/multivariate/test_vine.py` & `copulas-0.9.0.dev0/tests/unit/multivariate/test_vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/optimize/test___init__.py` & `copulas-0.9.0.dev0/tests/unit/optimize/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/test___init__.py` & `copulas-0.9.0.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/test__addons.py` & `copulas-0.9.0.dev0/tests/unit/test__addons.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_base.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_beta.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_gamma.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_gaussian.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_gaussian_kde.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_log_laplace.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_log_laplace.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_selection.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_selection.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_student_t.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_truncated_gaussian.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.0/tests/unit/univariate/test_uniform.py` & `copulas-0.9.0.dev0/tests/unit/univariate/test_uniform.py`

 * *Files identical despite different names*

